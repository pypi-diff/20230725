# Comparing `tmp/pygmi-3.2.6.5.tar.gz` & `tmp/pygmi-3.2.7.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmi-3.2.6.5.tar", last modified: Wed Mar 29 07:26:59 2023, max compression
+gzip compressed data, was "pygmi-3.2.7.16.tar", last modified: Tue Jul 25 09:29:13 2023, max compression
```

## Comparing `pygmi-3.2.6.5.tar` & `pygmi-3.2.7.16.tar`

### file list

```diff
@@ -1,174 +1,182 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:59.710265 pygmi-3.2.6.5/
--rw-rw-rw-   0        0        0    33109 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/COPYING
--rw-rw-rw-   0        0        0    33109 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/LICENSE.txt
--rw-rw-rw-   0        0        0      224 2023-03-28 08:19:27.000000 pygmi-3.2.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6897 2023-03-29 07:26:59.697133 pygmi-3.2.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     5241 2023-03-28 10:15:03.000000 pygmi-3.2.6.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:57.616095 pygmi-3.2.6.5/pygmi/
--rw-rw-rw-   0        0        0      543 2023-03-29 07:22:11.000000 pygmi-3.2.6.5/pygmi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:57.753003 pygmi-3.2.6.5/pygmi/clust/
--rw-rw-rw-   0        0        0       39 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/clust/__init__.py
--rw-rw-rw-   0        0        0    20733 2023-03-16 07:58:57.000000 pygmi-3.2.6.5/pygmi/clust/cluster.py
--rw-rw-rw-   0        0        0    30212 2023-03-14 07:03:09.000000 pygmi-3.2.6.5/pygmi/clust/crisp_clust.py
--rw-rw-rw-   0        0        0    35017 2023-03-14 07:02:19.000000 pygmi-3.2.6.5/pygmi/clust/fuzzy_clust.py
--rw-rw-rw-   0        0        0    12042 2023-03-15 06:49:21.000000 pygmi-3.2.6.5/pygmi/clust/graphs.py
--rw-rw-rw-   0        0        0    28242 2023-03-14 06:58:57.000000 pygmi-3.2.6.5/pygmi/clust/graphtool.py
--rw-rw-rw-   0        0        0     6887 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/clust/menu.py
--rw-rw-rw-   0        0        0    16924 2023-03-15 07:48:27.000000 pygmi-3.2.6.5/pygmi/clust/segmentation.py
--rw-rw-rw-   0        0        0    34309 2023-03-14 06:56:27.000000 pygmi-3.2.6.5/pygmi/clust/super_class.py
--rw-rw-rw-   0        0        0     3095 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/clust/var_ratio.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:57.785497 pygmi-3.2.6.5/pygmi/em/
--rw-rw-rw-   0        0        0       25 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/em/__init__.py
--rw-rw-rw-   0        0        0     1958 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/em/menu.py
--rw-rw-rw-   0        0        0    25057 2023-03-16 08:22:19.000000 pygmi-3.2.6.5/pygmi/em/tdem.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:57.842476 pygmi-3.2.6.5/pygmi/grav/
--rw-rw-rw-   0        0        0       30 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/grav/__init__.py
--rw-rw-rw-   0        0        0    17029 2023-03-14 07:13:51.000000 pygmi-3.2.6.5/pygmi/grav/dataprep.py
--rw-rw-rw-   0        0        0    13942 2023-03-15 07:48:54.000000 pygmi-3.2.6.5/pygmi/grav/iodefs.py
--rw-rw-rw-   0        0        0     2432 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/grav/menu.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:58.392416 pygmi-3.2.6.5/pygmi/helpdocs/
--rw-rw-rw-   0        0        0      874 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.bhole.rawcore.html
--rw-rw-rw-   0        0        0     2469 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.clust.cluster.html
--rw-rw-rw-   0        0        0      902 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.clust.segmentation.html
--rw-rw-rw-   0        0        0     2406 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.em.tdem1d.html
--rw-rw-rw-   0        0        0     1842 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.grav.dataprep.processdata.html
--rw-rw-rw-   0        0        0      851 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.grav.iodefs.importpointdata.html
--rw-rw-rw-   0        0        0     1848 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.main.html
--rw-rw-rw-   0        0        0     1223 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.mt.edit.html
--rw-rw-rw-   0        0        0     2769 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.mt.occam1d.html
--rw-rw-rw-   0        0        0     1221 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.mt.rotate.html
--rw-rw-rw-   0        0        0     1212 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.mt.static.html
--rw-rw-rw-   0        0        0     1177 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.ddisp.html
--rw-rw-rw-   0        0        0      764 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.iodefs.exportkmz.html
--rw-rw-rw-   0        0        0      813 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.iodefs.importpicture.html
--rw-rw-rw-   0        0        0     3970 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.mext.html
--rw-rw-rw-   0        0        0     4068 2022-12-01 11:31:34.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.minv.html
--rw-rw-rw-   0        0        0      828 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.misc.mergemod3d.html
--rw-rw-rw-   0        0        0      883 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.misc.rangedcopy.html
--rw-rw-rw-   0        0        0     2829 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.param.html
--rw-rw-rw-   0        0        0     3855 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.prof.html
--rw-rw-rw-   0        0        0      508 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.cooper.agc.html
--rw-rw-rw-   0        0        0      840 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.cooper.gradients.html
--rw-rw-rw-   0        0        0      737 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.cooper.tilt.html
--rw-rw-rw-   0        0        0      665 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.cooper.visibility.html
--rw-rw-rw-   0        0        0      608 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.dataprep.cont.html
--rw-rw-rw-   0        0        0      568 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.dataprep.datalayerstack.html
--rw-rw-rw-   0        0        0     1723 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.dataprep.datamerge.html
--rw-rw-rw-   0        0        0      390 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.dataprep.datareproj.html
--rw-rw-rw-   0        0        0      454 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.dataprep.rtp.html
--rw-rw-rw-   0        0        0     2543 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.ginterp.html
--rw-rw-rw-   0        0        0     1393 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.igrf.html
--rw-rw-rw-   0        0        0      822 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.normalisation.html
--rw-rw-rw-   0        0        0     1339 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.smooth.html
--rw-rw-rw-   0        0        0     1457 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.tiltdepth.html
--rw-rw-rw-   0        0        0      690 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.cind.html
--rw-rw-rw-   0        0        0      554 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.iodefs.exportbatch.html
--rw-rw-rw-   0        0        0      746 2023-03-22 06:17:37.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.iodefs.importsentinel5p.html
--rw-rw-rw-   0        0        0      561 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.landsat_composite.html
--rw-rw-rw-   0        0        0     1503 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.mnf.html
--rw-rw-rw-   0        0        0     1327 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.pca.html
--rw-rw-rw-   0        0        0     1179 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.pfeat.html
--rw-rw-rw-   0        0        0      721 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.ratios.html
--rw-rw-rw-   0        0        0      969 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.vector.dataprep.datagrid.html
--rw-rw-rw-   0        0        0      396 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/helpdocs/pygmi.vector.iodefs.importpointdata.html
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:58.593729 pygmi-3.2.6.5/pygmi/images/
--rw-rw-rw-   0        0        0     9831 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/images/Help.png
--rw-rw-rw-   0        0        0      293 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/images/bringtofront.png
--rw-rw-rw-   0        0        0    15761 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/images/cgslogo.png
--rw-rw-rw-   0        0        0      831 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/images/delete.png
--rw-rw-rw-   0        0        0      141 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/images/linepointer.png
--rw-rw-rw-   0        0        0   270398 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/images/logo256.ico
--rw-rw-rw-   0        0        0      536 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/images/play.png
--rw-rw-rw-   0        0        0      173 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/images/pointer.png
--rw-rw-rw-   0        0        0     4651 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/images/pygmi.png
--rw-rw-rw-   0        0        0      318 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/images/sendtoback.png
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:58.692933 pygmi-3.2.6.5/pygmi/mag/
--rw-rw-rw-   0        0        0   151290 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/mag/IGRF13.COF
--rw-rw-rw-   0        0        0       31 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/mag/__init__.py
--rw-rw-rw-   0        0        0    18704 2023-03-14 07:30:33.000000 pygmi-3.2.6.5/pygmi/mag/dataprep.py
--rw-rw-rw-   0        0        0    27276 2023-03-15 06:49:21.000000 pygmi-3.2.6.5/pygmi/mag/igrf.py
--rw-rw-rw-   0        0        0     3117 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/mag/menu.py
--rw-rw-rw-   0        0        0    14369 2023-03-14 07:33:04.000000 pygmi-3.2.6.5/pygmi/mag/tiltdepth.py
--rw-rw-rw-   0        0        0    44327 2023-03-15 07:46:17.000000 pygmi-3.2.6.5/pygmi/main.py
--rw-rw-rw-   0        0        0     7530 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/menu_default.py
--rw-rw-rw-   0        0        0    14262 2023-03-15 09:56:22.000000 pygmi-3.2.6.5/pygmi/misc.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:58.785745 pygmi-3.2.6.5/pygmi/mt/
--rw-rw-rw-   0        0        0       25 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/mt/__init__.py
--rw-rw-rw-   0        0        0    26432 2023-03-15 07:49:18.000000 pygmi-3.2.6.5/pygmi/mt/birrp.py
--rw-rw-rw-   0        0        0    57229 2023-03-16 08:42:38.000000 pygmi-3.2.6.5/pygmi/mt/dataprep.py
--rw-rw-rw-   0        0        0    12045 2023-03-14 07:35:55.000000 pygmi-3.2.6.5/pygmi/mt/graphs.py
--rw-rw-rw-   0        0        0     8190 2023-03-15 08:23:59.000000 pygmi-3.2.6.5/pygmi/mt/iodefs.py
--rw-rw-rw-   0        0        0     5642 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/mt/menu.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:58.988893 pygmi-3.2.6.5/pygmi/pfmod/
--rw-rw-rw-   0        0        0    12976 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/pfmod/DirectionDial.png
--rw-rw-rw-   0        0        0       33 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/pfmod/__init__.py
--rw-rw-rw-   0        0        0    12943 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/pfmod/datatypes.py
--rw-rw-rw-   0        0        0    48386 2023-02-28 12:16:39.000000 pygmi-3.2.6.5/pygmi/pfmod/grvmag3d.py
--rw-rw-rw-   0        0        0    46000 2023-03-29 06:55:48.000000 pygmi-3.2.6.5/pygmi/pfmod/iodefs.py
--rw-rw-rw-   0        0        0     4130 2022-12-01 11:31:35.000000 pygmi-3.2.6.5/pygmi/pfmod/menu.py
--rw-rw-rw-   0        0        0    16003 2023-03-15 06:52:30.000000 pygmi-3.2.6.5/pygmi/pfmod/misc.py
--rw-rw-rw-   0        0        0    72286 2023-03-14 11:19:17.000000 pygmi-3.2.6.5/pygmi/pfmod/mvis3d.py
--rw-rw-rw-   0        0        0    39792 2023-03-16 13:15:58.000000 pygmi-3.2.6.5/pygmi/pfmod/pfinvert.py
--rw-rw-rw-   0        0        0     8918 2023-03-14 11:52:01.000000 pygmi-3.2.6.5/pygmi/pfmod/pfmod.py
--rw-rw-rw-   0        0        0    21967 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/pfmod/tab_mext.py
--rw-rw-rw-   0        0        0    28403 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/pfmod/tab_param.py
--rw-rw-rw-   0        0        0    90712 2023-03-16 11:21:28.000000 pygmi-3.2.6.5/pygmi/pfmod/tab_prof.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:59.224941 pygmi-3.2.6.5/pygmi/raster/
--rw-rw-rw-   0        0        0       26 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/raster/__init__.py
--rw-rw-rw-   0        0        0    24637 2023-03-15 06:52:57.000000 pygmi-3.2.6.5/pygmi/raster/anaglyph.py
--rw-rw-rw-   0        0        0    27224 2023-03-13 13:16:29.000000 pygmi-3.2.6.5/pygmi/raster/cooper.py
--rw-rw-rw-   0        0        0    98340 2023-03-15 08:18:43.000000 pygmi-3.2.6.5/pygmi/raster/dataprep.py
--rw-rw-rw-   0        0        0     7325 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/raster/datatypes.py
--rw-rw-rw-   0        0        0    16227 2023-03-15 06:58:13.000000 pygmi-3.2.6.5/pygmi/raster/equation_editor.py
--rw-rw-rw-   0        0        0    54902 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/raster/gcs.csv
--rw-rw-rw-   0        0        0    64857 2023-03-16 11:45:33.000000 pygmi-3.2.6.5/pygmi/raster/ginterp.py
--rw-rw-rw-   0        0        0    19687 2023-03-15 06:58:35.000000 pygmi-3.2.6.5/pygmi/raster/graphs.py
--rw-rw-rw-   0        0        0    54053 2023-03-15 10:21:12.000000 pygmi-3.2.6.5/pygmi/raster/iodefs.py
--rw-rw-rw-   0        0        0    11532 2023-03-15 11:52:45.000000 pygmi-3.2.6.5/pygmi/raster/menu.py
--rw-rw-rw-   0        0        0    25888 2023-03-08 13:04:54.000000 pygmi-3.2.6.5/pygmi/raster/modest_image.py
--rw-rw-rw-   0        0        0     7412 2023-03-14 06:26:39.000000 pygmi-3.2.6.5/pygmi/raster/normalisation.py
--rw-rw-rw-   0        0        0   803602 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/raster/pcs.csv
--rw-rw-rw-   0        0        0     9676 2023-03-14 06:30:18.000000 pygmi-3.2.6.5/pygmi/raster/show_table.py
--rw-rw-rw-   0        0        0    18373 2023-03-14 06:32:02.000000 pygmi-3.2.6.5/pygmi/raster/smooth.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:59.372104 pygmi-3.2.6.5/pygmi/rsense/
--rw-rw-rw-   0        0        0       32 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/rsense/__init__.py
--rw-rw-rw-   0        0        0    30611 2023-03-15 08:12:38.000000 pygmi-3.2.6.5/pygmi/rsense/change.py
--rw-rw-rw-   0        0        0     3819 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/rsense/features.py
--rw-rw-rw-   0        0        0    42185 2023-03-23 09:50:33.000000 pygmi-3.2.6.5/pygmi/rsense/hyperspec.py
--rw-rw-rw-   0        0        0    82828 2023-03-22 09:19:53.000000 pygmi-3.2.6.5/pygmi/rsense/iodefs.py
--rw-rw-rw-   0        0        0    11209 2023-03-15 08:14:50.000000 pygmi-3.2.6.5/pygmi/rsense/landsat_composite.py
--rw-rw-rw-   0        0        0    10861 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/rsense/menu.py
--rw-rw-rw-   0        0        0    40575 2023-03-17 09:08:13.000000 pygmi-3.2.6.5/pygmi/rsense/ratios.py
--rw-rw-rw-   0        0        0    28652 2023-03-22 09:35:24.000000 pygmi-3.2.6.5/pygmi/rsense/transforms.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:59.506937 pygmi-3.2.6.5/pygmi/seis/
--rw-rw-rw-   0        0        0       28 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/seis/__init__.py
--rw-rw-rw-   0        0        0    25790 2023-03-15 08:15:22.000000 pygmi-3.2.6.5/pygmi/seis/beachball.py
--rw-rw-rw-   0        0        0    21999 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/seis/datatypes.py
--rw-rw-rw-   0        0        0    16846 2023-03-14 12:06:29.000000 pygmi-3.2.6.5/pygmi/seis/del_rec.py
--rw-rw-rw-   0        0        0    29919 2023-03-27 07:16:19.000000 pygmi-3.2.6.5/pygmi/seis/graphs.py
--rw-rw-rw-   0        0        0    75241 2023-03-27 07:07:47.000000 pygmi-3.2.6.5/pygmi/seis/iodefs.py
--rw-rw-rw-   0        0        0     5946 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/seis/menu.py
--rw-rw-rw-   0        0        0     6781 2023-03-14 11:58:52.000000 pygmi-3.2.6.5/pygmi/seis/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:59.592544 pygmi-3.2.6.5/pygmi/test/
--rw-rw-rw-   0        0        0       24 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/test/__init__.py
--rw-rw-rw-   0        0        0     3687 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/test/test_cluster.py
--rw-rw-rw-   0        0        0     2846 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/test/test_gravity.py
--rw-rw-rw-   0        0        0     4582 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/test/test_mag.py
--rw-rw-rw-   0        0        0    12376 2022-12-01 11:31:36.000000 pygmi-3.2.6.5/pygmi/test/test_pfmod.py
--rw-rw-rw-   0        0        0    17729 2023-03-15 08:46:29.000000 pygmi-3.2.6.5/pygmi/test/test_raster.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:59.680107 pygmi-3.2.6.5/pygmi/vector/
--rw-rw-rw-   0        0        0       29 2022-12-01 11:31:37.000000 pygmi-3.2.6.5/pygmi/vector/__init__.py
--rw-rw-rw-   0        0        0    26100 2023-03-29 06:22:56.000000 pygmi-3.2.6.5/pygmi/vector/dataprep.py
--rw-rw-rw-   0        0        0    27406 2023-03-14 06:43:03.000000 pygmi-3.2.6.5/pygmi/vector/graphs.py
--rw-rw-rw-   0        0        0    13222 2023-03-15 08:16:56.000000 pygmi-3.2.6.5/pygmi/vector/iodefs.py
--rw-rw-rw-   0        0        0     6554 2022-12-01 11:31:37.000000 pygmi-3.2.6.5/pygmi/vector/menu.py
--rw-rw-rw-   0        0        0    18086 2022-12-01 11:31:37.000000 pygmi-3.2.6.5/pygmi/vector/minc.py
-drwxrwxrwx   0        0        0        0 2023-03-29 07:26:57.661296 pygmi-3.2.6.5/pygmi.egg-info/
--rw-rw-rw-   0        0        0     6897 2023-03-29 07:26:57.000000 pygmi-3.2.6.5/pygmi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4513 2023-03-29 07:26:57.000000 pygmi-3.2.6.5/pygmi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 07:26:57.000000 pygmi-3.2.6.5/pygmi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-03-29 07:26:57.000000 pygmi-3.2.6.5/pygmi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      197 2023-03-29 07:26:57.000000 pygmi-3.2.6.5/pygmi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-29 07:26:57.000000 pygmi-3.2.6.5/pygmi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2546 2023-03-28 13:33:34.000000 pygmi-3.2.6.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-29 07:26:59.710265 pygmi-3.2.6.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:13.700840 pygmi-3.2.7.16/
+-rw-rw-rw-   0        0        0    33109 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/COPYING
+-rw-rw-rw-   0        0        0    33109 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/LICENSE.txt
+-rw-rw-rw-   0        0        0      261 2023-03-29 10:52:05.000000 pygmi-3.2.7.16/MANIFEST.in
+-rw-rw-rw-   0        0        0     6940 2023-07-25 09:29:13.694838 pygmi-3.2.7.16/PKG-INFO
+-rw-rw-rw-   0        0        0     5283 2023-07-17 07:26:26.000000 pygmi-3.2.7.16/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:12.287693 pygmi-3.2.7.16/pygmi/
+-rw-rw-rw-   0        0        0      544 2023-07-21 11:41:12.000000 pygmi-3.2.7.16/pygmi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:12.378218 pygmi-3.2.7.16/pygmi/bholes/
+-rw-rw-rw-   0        0        0       27 2023-05-04 06:06:18.000000 pygmi-3.2.7.16/pygmi/bholes/__init__.py
+-rw-rw-rw-   0        0        0    20083 2023-07-18 13:08:27.000000 pygmi-3.2.7.16/pygmi/bholes/graphs.py
+-rw-rw-rw-   0        0        0     4366 2023-05-16 05:41:08.000000 pygmi-3.2.7.16/pygmi/bholes/iodefs.py
+-rw-rw-rw-   0        0        0     2472 2023-05-04 06:13:47.000000 pygmi-3.2.7.16/pygmi/bholes/menu.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:12.479727 pygmi-3.2.7.16/pygmi/clust/
+-rw-rw-rw-   0        0        0       39 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/clust/__init__.py
+-rw-rw-rw-   0        0        0    21067 2023-07-19 06:37:37.000000 pygmi-3.2.7.16/pygmi/clust/cluster.py
+-rw-rw-rw-   0        0        0    30141 2023-07-19 07:16:17.000000 pygmi-3.2.7.16/pygmi/clust/crisp_clust.py
+-rw-rw-rw-   0        0        0    34802 2023-07-19 07:18:39.000000 pygmi-3.2.7.16/pygmi/clust/fuzzy_clust.py
+-rw-rw-rw-   0        0        0    12107 2023-07-19 06:24:32.000000 pygmi-3.2.7.16/pygmi/clust/graphs.py
+-rw-rw-rw-   0        0        0    28233 2023-07-19 09:05:47.000000 pygmi-3.2.7.16/pygmi/clust/graphtool.py
+-rw-rw-rw-   0        0        0     6887 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/clust/menu.py
+-rw-rw-rw-   0        0        0    16870 2023-07-18 08:11:56.000000 pygmi-3.2.7.16/pygmi/clust/segmentation.py
+-rw-rw-rw-   0        0        0    34247 2023-07-19 07:04:32.000000 pygmi-3.2.7.16/pygmi/clust/super_class.py
+-rw-rw-rw-   0        0        0     3095 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/clust/var_ratio.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:12.503728 pygmi-3.2.7.16/pygmi/em/
+-rw-rw-rw-   0        0        0       25 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/em/__init__.py
+-rw-rw-rw-   0        0        0     1958 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/em/menu.py
+-rw-rw-rw-   0        0        0    25030 2023-07-19 10:26:01.000000 pygmi-3.2.7.16/pygmi/em/tdem.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:12.543245 pygmi-3.2.7.16/pygmi/grav/
+-rw-rw-rw-   0        0        0       30 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/grav/__init__.py
+-rw-rw-rw-   0        0        0    17082 2023-06-28 13:28:11.000000 pygmi-3.2.7.16/pygmi/grav/dataprep.py
+-rw-rw-rw-   0        0        0    14055 2023-07-06 08:52:46.000000 pygmi-3.2.7.16/pygmi/grav/iodefs.py
+-rw-rw-rw-   0        0        0     2432 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/grav/menu.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:12.967316 pygmi-3.2.7.16/pygmi/helpdocs/
+-rw-rw-rw-   0        0        0      874 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.bhole.rawcore.html
+-rw-rw-rw-   0        0        0     2469 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.clust.cluster.html
+-rw-rw-rw-   0        0        0      902 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.clust.segmentation.html
+-rw-rw-rw-   0        0        0     2406 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.em.tdem1d.html
+-rw-rw-rw-   0        0        0     1842 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.grav.dataprep.processdata.html
+-rw-rw-rw-   0        0        0      851 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.grav.iodefs.importpointdata.html
+-rw-rw-rw-   0        0        0     1848 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.main.html
+-rw-rw-rw-   0        0        0     1223 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.mt.edit.html
+-rw-rw-rw-   0        0        0     2769 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.mt.occam1d.html
+-rw-rw-rw-   0        0        0     1221 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.mt.rotate.html
+-rw-rw-rw-   0        0        0     1212 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.mt.static.html
+-rw-rw-rw-   0        0        0     1177 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.ddisp.html
+-rw-rw-rw-   0        0        0      764 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.iodefs.exportkmz.html
+-rw-rw-rw-   0        0        0      813 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.iodefs.importpicture.html
+-rw-rw-rw-   0        0        0     3970 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.mext.html
+-rw-rw-rw-   0        0        0     4068 2022-12-01 11:31:34.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.minv.html
+-rw-rw-rw-   0        0        0      828 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.misc.mergemod3d.html
+-rw-rw-rw-   0        0        0      883 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.misc.rangedcopy.html
+-rw-rw-rw-   0        0        0     2829 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.param.html
+-rw-rw-rw-   0        0        0     3855 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.prof.html
+-rw-rw-rw-   0        0        0      508 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.cooper.agc.html
+-rw-rw-rw-   0        0        0      840 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.cooper.gradients.html
+-rw-rw-rw-   0        0        0      944 2023-06-20 06:27:33.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.cooper.tilt.html
+-rw-rw-rw-   0        0        0      665 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.cooper.visibility.html
+-rw-rw-rw-   0        0        0      608 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.dataprep.cont.html
+-rw-rw-rw-   0        0        0      568 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.dataprep.datalayerstack.html
+-rw-rw-rw-   0        0        0     1723 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.dataprep.datamerge.html
+-rw-rw-rw-   0        0        0      390 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.dataprep.datareproj.html
+-rw-rw-rw-   0        0        0      454 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.dataprep.rtp.html
+-rw-rw-rw-   0        0        0     2543 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.ginterp.html
+-rw-rw-rw-   0        0        0     1393 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.igrf.html
+-rw-rw-rw-   0        0        0      822 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.normalisation.html
+-rw-rw-rw-   0        0        0     1339 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.smooth.html
+-rw-rw-rw-   0        0        0     1457 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.tiltdepth.html
+-rw-rw-rw-   0        0        0      690 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.cind.html
+-rw-rw-rw-   0        0        0      727 2023-07-21 13:28:51.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.iodefs.exportbatch.html
+-rw-rw-rw-   0        0        0      746 2023-03-22 06:17:37.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.iodefs.importsentinel5p.html
+-rw-rw-rw-   0        0        0      561 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.landsat_composite.html
+-rw-rw-rw-   0        0        0     1503 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.mnf.html
+-rw-rw-rw-   0        0        0     1327 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.pca.html
+-rw-rw-rw-   0        0        0     1179 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.pfeat.html
+-rw-rw-rw-   0        0        0      721 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.ratios.html
+-rw-rw-rw-   0        0        0      969 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.vector.dataprep.datagrid.html
+-rw-rw-rw-   0        0        0      678 2023-07-10 12:54:52.000000 pygmi-3.2.7.16/pygmi/helpdocs/pygmi.vector.iodefs.importxyzdata.html
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:13.056840 pygmi-3.2.7.16/pygmi/images/
+-rw-rw-rw-   0        0        0     9831 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/images/Help.png
+-rw-rw-rw-   0        0        0      293 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/images/bringtofront.png
+-rw-rw-rw-   0        0        0    15761 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/images/cgslogo.png
+-rw-rw-rw-   0        0        0      831 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/images/delete.png
+-rw-rw-rw-   0        0        0      141 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/images/linepointer.png
+-rw-rw-rw-   0        0        0     2021 2021-12-09 12:09:14.000000 pygmi-3.2.7.16/pygmi/images/load.png
+-rw-rw-rw-   0        0        0   270398 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/images/logo256.ico
+-rw-rw-rw-   0        0        0      536 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/images/play.png
+-rw-rw-rw-   0        0        0      173 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/images/pointer.png
+-rw-rw-rw-   0        0        0     4651 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/images/pygmi.png
+-rw-rw-rw-   0        0        0      318 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/images/sendtoback.png
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:13.112842 pygmi-3.2.7.16/pygmi/mag/
+-rw-rw-rw-   0        0        0   151290 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/mag/IGRF13.COF
+-rw-rw-rw-   0        0        0       31 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/mag/__init__.py
+-rw-rw-rw-   0        0        0    19229 2023-07-18 10:07:51.000000 pygmi-3.2.7.16/pygmi/mag/dataprep.py
+-rw-rw-rw-   0        0        0    27253 2023-05-16 13:29:52.000000 pygmi-3.2.7.16/pygmi/mag/igrf.py
+-rw-rw-rw-   0        0        0     3117 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/mag/menu.py
+-rw-rw-rw-   0        0        0    16603 2023-07-19 10:48:08.000000 pygmi-3.2.7.16/pygmi/mag/tiltdepth.py
+-rw-rw-rw-   0        0        0    44948 2023-07-20 08:28:08.000000 pygmi-3.2.7.16/pygmi/main.py
+-rw-rw-rw-   0        0        0     7530 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/menu_default.py
+-rw-rw-rw-   0        0        0    14516 2023-07-18 08:11:56.000000 pygmi-3.2.7.16/pygmi/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:13.171878 pygmi-3.2.7.16/pygmi/mt/
+-rw-rw-rw-   0        0        0       25 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/mt/__init__.py
+-rw-rw-rw-   0        0        0    26404 2023-05-11 05:56:37.000000 pygmi-3.2.7.16/pygmi/mt/birrp.py
+-rw-rw-rw-   0        0        0    57238 2023-07-19 10:57:56.000000 pygmi-3.2.7.16/pygmi/mt/dataprep.py
+-rw-rw-rw-   0        0        0    12069 2023-07-19 10:54:38.000000 pygmi-3.2.7.16/pygmi/mt/graphs.py
+-rw-rw-rw-   0        0        0     5874 2023-06-29 12:57:00.000000 pygmi-3.2.7.16/pygmi/mt/iodefs.py
+-rw-rw-rw-   0        0        0     5050 2023-06-29 12:52:27.000000 pygmi-3.2.7.16/pygmi/mt/menu.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:13.311057 pygmi-3.2.7.16/pygmi/pfmod/
+-rw-rw-rw-   0        0        0    12976 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/pfmod/DirectionDial.png
+-rw-rw-rw-   0        0        0       33 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/pfmod/__init__.py
+-rw-rw-rw-   0        0        0    12943 2022-12-01 11:31:35.000000 pygmi-3.2.7.16/pygmi/pfmod/datatypes.py
+-rw-rw-rw-   0        0        0    48354 2023-07-18 08:12:34.000000 pygmi-3.2.7.16/pygmi/pfmod/grvmag3d.py
+-rw-rw-rw-   0        0        0    47005 2023-05-16 13:30:49.000000 pygmi-3.2.7.16/pygmi/pfmod/iodefs.py
+-rw-rw-rw-   0        0        0     4488 2023-07-17 12:55:43.000000 pygmi-3.2.7.16/pygmi/pfmod/menu.py
+-rw-rw-rw-   0        0        0    15937 2023-05-16 13:31:07.000000 pygmi-3.2.7.16/pygmi/pfmod/misc.py
+-rw-rw-rw-   0        0        0    72238 2023-05-30 10:53:44.000000 pygmi-3.2.7.16/pygmi/pfmod/mvis3d.py
+-rw-rw-rw-   0        0        0    37942 2023-07-19 12:33:08.000000 pygmi-3.2.7.16/pygmi/pfmod/pfinvert.py
+-rw-rw-rw-   0        0        0     8892 2023-07-19 11:30:31.000000 pygmi-3.2.7.16/pygmi/pfmod/pfmod.py
+-rw-rw-rw-   0        0        0     7091 2023-07-18 05:40:01.000000 pygmi-3.2.7.16/pygmi/pfmod/show_table.py
+-rw-rw-rw-   0        0        0    21967 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/pfmod/tab_mext.py
+-rw-rw-rw-   0        0        0    28403 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/pfmod/tab_param.py
+-rw-rw-rw-   0        0        0    90328 2023-07-19 11:25:29.000000 pygmi-3.2.7.16/pygmi/pfmod/tab_prof.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:13.481083 pygmi-3.2.7.16/pygmi/raster/
+-rw-rw-rw-   0        0        0       26 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/raster/__init__.py
+-rw-rw-rw-   0        0        0    24624 2023-07-18 11:09:59.000000 pygmi-3.2.7.16/pygmi/raster/anaglyph.py
+-rw-rw-rw-   0        0        0    27159 2023-07-18 08:27:25.000000 pygmi-3.2.7.16/pygmi/raster/cooper.py
+-rw-rw-rw-   0        0        0    83875 2023-07-20 11:07:35.000000 pygmi-3.2.7.16/pygmi/raster/dataprep.py
+-rw-rw-rw-   0        0        0    10117 2023-07-18 08:49:45.000000 pygmi-3.2.7.16/pygmi/raster/datatypes.py
+-rw-rw-rw-   0        0        0    16205 2023-07-18 08:51:22.000000 pygmi-3.2.7.16/pygmi/raster/equation_editor.py
+-rw-rw-rw-   0        0        0    54902 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/raster/gcs.csv
+-rw-rw-rw-   0        0        0    65045 2023-07-18 11:20:43.000000 pygmi-3.2.7.16/pygmi/raster/ginterp.py
+-rw-rw-rw-   0        0        0    19546 2023-07-18 11:11:38.000000 pygmi-3.2.7.16/pygmi/raster/graphs.py
+-rw-rw-rw-   0        0        0    58198 2023-07-18 09:59:21.000000 pygmi-3.2.7.16/pygmi/raster/iodefs.py
+-rw-rw-rw-   0        0        0    11533 2023-07-18 10:53:09.000000 pygmi-3.2.7.16/pygmi/raster/menu.py
+-rw-rw-rw-   0        0        0    25888 2023-03-08 13:04:54.000000 pygmi-3.2.7.16/pygmi/raster/modest_image.py
+-rw-rw-rw-   0        0        0     7405 2023-05-11 05:58:35.000000 pygmi-3.2.7.16/pygmi/raster/normalisation.py
+-rw-rw-rw-   0        0        0   803602 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/raster/pcs.csv
+-rw-rw-rw-   0        0        0     9672 2023-07-18 10:06:14.000000 pygmi-3.2.7.16/pygmi/raster/show_table.py
+-rw-rw-rw-   0        0        0    18034 2023-07-18 08:24:30.000000 pygmi-3.2.7.16/pygmi/raster/smooth.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:13.546320 pygmi-3.2.7.16/pygmi/rsense/
+-rw-rw-rw-   0        0        0       32 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/rsense/__init__.py
+-rw-rw-rw-   0        0        0    32090 2023-05-16 13:34:59.000000 pygmi-3.2.7.16/pygmi/rsense/change.py
+-rw-rw-rw-   0        0        0     3819 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/rsense/features.py
+-rw-rw-rw-   0        0        0    37856 2023-07-21 10:02:05.000000 pygmi-3.2.7.16/pygmi/rsense/hyperspec.py
+-rw-rw-rw-   0        0        0   105332 2023-07-21 12:21:48.000000 pygmi-3.2.7.16/pygmi/rsense/iodefs.py
+-rw-rw-rw-   0        0        0    11227 2023-07-21 06:50:16.000000 pygmi-3.2.7.16/pygmi/rsense/landsat_composite.py
+-rw-rw-rw-   0        0        0     7505 2023-07-21 09:58:39.000000 pygmi-3.2.7.16/pygmi/rsense/menu.py
+-rw-rw-rw-   0        0        0    40183 2023-07-21 13:19:13.000000 pygmi-3.2.7.16/pygmi/rsense/ratios.py
+-rw-rw-rw-   0        0        0    30059 2023-07-21 06:15:59.000000 pygmi-3.2.7.16/pygmi/rsense/transforms.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:13.610324 pygmi-3.2.7.16/pygmi/seis/
+-rw-rw-rw-   0        0        0       28 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/seis/__init__.py
+-rw-rw-rw-   0        0        0    23999 2023-07-21 10:44:10.000000 pygmi-3.2.7.16/pygmi/seis/beachball.py
+-rw-rw-rw-   0        0        0    21999 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/seis/datatypes.py
+-rw-rw-rw-   0        0        0    16635 2023-05-16 13:39:12.000000 pygmi-3.2.7.16/pygmi/seis/del_rec.py
+-rw-rw-rw-   0        0        0    50506 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/seis/descriptions.txt
+-rw-rw-rw-   0        0        0    27731 2023-07-21 11:35:07.000000 pygmi-3.2.7.16/pygmi/seis/graphs.py
+-rw-rw-rw-   0        0        0    75774 2023-07-21 11:03:11.000000 pygmi-3.2.7.16/pygmi/seis/iodefs.py
+-rw-rw-rw-   0        0        0     5946 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/seis/menu.py
+-rw-rw-rw-   0        0        0     6767 2023-05-11 05:58:05.000000 pygmi-3.2.7.16/pygmi/seis/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:13.649836 pygmi-3.2.7.16/pygmi/test/
+-rw-rw-rw-   0        0        0       24 2022-12-01 11:31:36.000000 pygmi-3.2.7.16/pygmi/test/__init__.py
+-rw-rw-rw-   0        0        0     3788 2023-07-19 07:07:24.000000 pygmi-3.2.7.16/pygmi/test/test_cluster.py
+-rw-rw-rw-   0        0        0     2840 2023-06-28 13:32:36.000000 pygmi-3.2.7.16/pygmi/test/test_gravity.py
+-rw-rw-rw-   0        0        0     4582 2023-07-18 09:08:14.000000 pygmi-3.2.7.16/pygmi/test/test_mag.py
+-rw-rw-rw-   0        0        0    12400 2023-05-05 07:36:35.000000 pygmi-3.2.7.16/pygmi/test/test_pfmod.py
+-rw-rw-rw-   0        0        0    17990 2023-07-18 09:46:00.000000 pygmi-3.2.7.16/pygmi/test/test_raster.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:13.686838 pygmi-3.2.7.16/pygmi/vector/
+-rw-rw-rw-   0        0        0       29 2022-12-01 11:31:37.000000 pygmi-3.2.7.16/pygmi/vector/__init__.py
+-rw-rw-rw-   0        0        0    26710 2023-07-18 11:44:45.000000 pygmi-3.2.7.16/pygmi/vector/dataprep.py
+-rw-rw-rw-   0        0        0    25107 2023-07-18 12:32:08.000000 pygmi-3.2.7.16/pygmi/vector/graphs.py
+-rw-rw-rw-   0        0        0    21350 2023-07-19 05:47:12.000000 pygmi-3.2.7.16/pygmi/vector/iodefs.py
+-rw-rw-rw-   0        0        0     6282 2023-07-10 10:48:35.000000 pygmi-3.2.7.16/pygmi/vector/menu.py
+-rw-rw-rw-   0        0        0    17987 2023-07-18 12:02:02.000000 pygmi-3.2.7.16/pygmi/vector/minc.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:29:12.342215 pygmi-3.2.7.16/pygmi.egg-info/
+-rw-rw-rw-   0        0        0     6940 2023-07-25 09:29:11.000000 pygmi-3.2.7.16/pygmi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4679 2023-07-25 09:29:12.000000 pygmi-3.2.7.16/pygmi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 09:29:11.000000 pygmi-3.2.7.16/pygmi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-07-25 09:29:11.000000 pygmi-3.2.7.16/pygmi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      218 2023-07-25 09:29:11.000000 pygmi-3.2.7.16/pygmi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-25 09:29:11.000000 pygmi-3.2.7.16/pygmi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2627 2023-07-25 09:28:03.000000 pygmi-3.2.7.16/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 09:29:13.701838 pygmi-3.2.7.16/setup.cfg
```

### Comparing `pygmi-3.2.6.5/COPYING` & `pygmi-3.2.7.16/COPYING`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/LICENSE.txt` & `pygmi-3.2.7.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/PKG-INFO` & `pygmi-3.2.7.16/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi
-Version: 3.2.6.5
+Version: 3.2.7.16
 Summary: Python Geoscience Modelling and Interpretation
 Author-email: Patrick Cole <pcole@geoscience.org.za>
 Maintainer-email: Patrick Cole <pcole@geoscience.org.za>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, http://patrick-cole.github.io/pygmi/
 Project-URL: documentation, https://patrick-cole.github.io/pygmi/wiki.html
 Project-URL: repository, https://github.com/Patrick-Cole/pygmi.git
@@ -22,15 +22,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: COPYING
 
 Overview
 ========
 
@@ -57,45 +57,49 @@
 
 You may need to install the `Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019 <https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads>`_.
 
 If you have any comments or queries, you can contact the author either through `GitHub <https://github.com/Patrick-Cole/pygmi>`_ or via email at pcole@geoscience.org.za
 
 Requirements
 ------------
-PyGMI will run on both Windows and Linux. It should be noted that the main development is done in Python 3.10 on Windows.
+PyGMI will run on both Windows and Linux. It should be noted that the main development is done in Python 3.11 on Windows.
 
-PyGMI should still work with Python 3.8 and Python 3.9.
+PyGMI should still work with Python 3.9 and Python 3.10.
 
 PyGMI is developed and has been tested with the following libraries in order to function:
 
-* python 3.10.9
+* python 3.11.4
 * contextily 1.3.0
-* discretize 0.8.3
-* fiona 1.8.22
-* geopandas 0.12.1
-* llvmlite 0.39.1
-* matplotlib 3.7.1
+* discretize 0.9.0
+* fiona 1.9.4.post1
+* gdal 3.7.1
+* geopandas 0.13.2
+* llvmlite 0.40.1
+* matplotlib 3.7.2
 * mtpy 1.1.5
-* natsort 8.2.0
-* numba 0.56.4
+* natsort 8.4.0
+* numba 0.57.1
 * numexpr 2.8.4
-* numpy 1.23.5+mkl
-* pandas 1.5.2
-* pillow 9.3.0
-* psutil 5.9.0
-* pyopengl 3.1.6
-* pyproj 3.4.1
-* PyQt5 5.15.6
-* pytest 7.1.1
-* rasterio 1.3.4
-* scikit-image 0.19.3
-* scikit-learn 1.1.3
-* scipy 1.9.3
-* shapely 1.8.5.post1
-* SimPEG 0.18.1
+* numpy 1.24.4
+* openpyxl 3.1.2
+* pandas 2.0.3
+* pillow 10.0.0
+* psutil 5.9.5
+* pyogrio 0.6.0
+* pyopengl 3.1.7
+* pyproj 3.6.0
+* PyQt5 5.15.9
+* pytest 7.4.0
+* rasterio 1.3.8
+* scikit-image 0.21.0
+* scikit-learn 1.3.0
+* scipy 1.11.1
+* shapely 2.0.1
+* SimPEG 0.19.0
+* utm 0.7.0
 
 Installation
 ------------
 General (Not Anaconda)
 ----------------------
 The easiest way to install pygmi if you are working in a python environment is to use the pip command as follows:
 
@@ -128,15 +132,15 @@
 * numexpr
 * numba
 * llvmlite
 * GDAL
 * discretize
 * fiona
 
-They can be obtained from the `website <http://www.lfd.uci.edu/~gohlke/pythonlibs/>`_ by Christoph Gohlke.
+They can be obtained from the `website <https://www.cgohlke.com/>`_ by Christoph Gohlke.
 
 Linux
 -----
 Linux normally comes with python installed, but the additional libraries will still need to be installed.
 
 Typically, packages can be installed using pip. The process is as follows:
```

### Comparing `pygmi-3.2.6.5/README.rst` & `pygmi-3.2.7.16/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -24,45 +24,49 @@
 
 You may need to install the `Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019 <https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads>`_.
 
 If you have any comments or queries, you can contact the author either through `GitHub <https://github.com/Patrick-Cole/pygmi>`_ or via email at pcole@geoscience.org.za
 
 Requirements
 ------------
-PyGMI will run on both Windows and Linux. It should be noted that the main development is done in Python 3.10 on Windows.
+PyGMI will run on both Windows and Linux. It should be noted that the main development is done in Python 3.11 on Windows.
 
-PyGMI should still work with Python 3.8 and Python 3.9.
+PyGMI should still work with Python 3.9 and Python 3.10.
 
 PyGMI is developed and has been tested with the following libraries in order to function:
 
-* python 3.10.9
+* python 3.11.4
 * contextily 1.3.0
-* discretize 0.8.3
-* fiona 1.8.22
-* geopandas 0.12.1
-* llvmlite 0.39.1
-* matplotlib 3.7.1
+* discretize 0.9.0
+* fiona 1.9.4.post1
+* gdal 3.7.1
+* geopandas 0.13.2
+* llvmlite 0.40.1
+* matplotlib 3.7.2
 * mtpy 1.1.5
-* natsort 8.2.0
-* numba 0.56.4
+* natsort 8.4.0
+* numba 0.57.1
 * numexpr 2.8.4
-* numpy 1.23.5+mkl
-* pandas 1.5.2
-* pillow 9.3.0
-* psutil 5.9.0
-* pyopengl 3.1.6
-* pyproj 3.4.1
-* PyQt5 5.15.6
-* pytest 7.1.1
-* rasterio 1.3.4
-* scikit-image 0.19.3
-* scikit-learn 1.1.3
-* scipy 1.9.3
-* shapely 1.8.5.post1
-* SimPEG 0.18.1
+* numpy 1.24.4
+* openpyxl 3.1.2
+* pandas 2.0.3
+* pillow 10.0.0
+* psutil 5.9.5
+* pyogrio 0.6.0
+* pyopengl 3.1.7
+* pyproj 3.6.0
+* PyQt5 5.15.9
+* pytest 7.4.0
+* rasterio 1.3.8
+* scikit-image 0.21.0
+* scikit-learn 1.3.0
+* scipy 1.11.1
+* shapely 2.0.1
+* SimPEG 0.19.0
+* utm 0.7.0
 
 Installation
 ------------
 General (Not Anaconda)
 ----------------------
 The easiest way to install pygmi if you are working in a python environment is to use the pip command as follows:
 
@@ -95,15 +99,15 @@
 * numexpr
 * numba
 * llvmlite
 * GDAL
 * discretize
 * fiona
 
-They can be obtained from the `website <http://www.lfd.uci.edu/~gohlke/pythonlibs/>`_ by Christoph Gohlke.
+They can be obtained from the `website <https://www.cgohlke.com/>`_ by Christoph Gohlke.
 
 Linux
 -----
 Linux normally comes with python installed, but the additional libraries will still need to be installed.
 
 Typically, packages can be installed using pip. The process is as follows:
```

### Comparing `pygmi-3.2.6.5/pygmi/__init__.py` & `pygmi-3.2.7.16/pygmi/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,8 +10,8 @@
  * Convenient display of data using pseudo-color, ternary and sunshaded representation
 
 It is released under the Gnu General Public License version 3.0
 """
 
 from pygmi.main import main
 
-__version__ = '3.2.6.5'
+__version__ = '3.2.7.16'
```

### Comparing `pygmi-3.2.6.5/pygmi/clust/cluster.py` & `pygmi-3.2.7.16/pygmi/clust/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.min_samples = 5
         self.bthres = 0.5
         self.branchfac = 50
 
         self.setupui()
 
         self.combobox_alg.addItems(['Mini Batch K-Means (fast)', 'K-Means',
-                                    'DBSCAN', 'Birch'])
+                                    'Bisecting K-Means', 'DBSCAN', 'Birch'])
         self.combobox_alg.currentIndexChanged.connect(self.combo)
         self.combo()
 
     def setupui(self):
         """
         Set up UI.
 
@@ -178,15 +178,15 @@
         self.doublespinbox_bthres.hide()
 
         if i == 'DBSCAN':
             self.label_eps.show()
             self.label_minsamples.show()
             self.spinbox_minsamples.show()
             self.doublespinbox_eps.show()
-        elif i in ['K-Means', 'Mini Batch K-Means (fast)']:
+        elif 'K-Means' in i:
             self.label_minclusters.show()
             self.spinbox_minclusters.show()
             self.label_maxclusters.show()
             self.spinbox_maxclusters.show()
             self.label_maxerror.show()
             self.doublespinbox_maxerror.show()
             self.label_maxiter.show()
@@ -213,22 +213,22 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         tst = np.unique([i.data.shape for i in self.indata['Raster']])
 
         if tst.size > 2:
-            self.showprocesslog('Error: Your input datasets have different '
-                                'sizes. Merge the data first')
+            self.showlog('Error: Your input datasets have different '
+                         'sizes. Merge the data first')
             return False
 
         self.min_samples = len(self.indata['Raster'])+1
         self.spinbox_minsamples.setProperty('value', self.min_samples)
 
         if not nodialog:
             temp = self.exec_()
@@ -325,15 +325,15 @@
 
         """
         data = self.indata['Raster']
         self.update_vars()
 
         no_clust = range(self.min_cluster, self.max_cluster+1)
 
-        self.showprocesslog('Cluster analysis started')
+        self.showlog('Cluster analysis started')
 
         # Section to deal with different bands having different null values.
         masktmp = ~data[0].data.mask
         for i in data:
             masktmp += ~i.data.mask
         masktmp = ~masktmp
 
@@ -342,54 +342,63 @@
             tmp = copy.deepcopy(band)
             tmp.data.mask = masktmp
             X.append(tmp.data.compressed())
             del tmp
         X = np.transpose(X)
 
         if self.radiobutton_sscale.isChecked():
-            self.showprocesslog('Applying standard scaling')
+            self.showlog('Applying standard scaling')
             X = skp.StandardScaler().fit_transform(X)
         elif self.radiobutton_rscale.isChecked():
-            self.showprocesslog('Applying robust scaling')
+            self.showlog('Applying robust scaling')
             X = skp.RobustScaler().fit_transform(X)
 
         dat_out = []
         for i in self.piter(no_clust):
             if self.cltype != 'DBSCAN':
-                self.showprocesslog('Number of Clusters:'+str(i))
+                self.showlog('Number of Clusters:'+str(i))
             elif i > no_clust[0]:
                 continue
 
+            cfit = None
             if self.cltype == 'Mini Batch K-Means (fast)':
                 bsize = max(os.cpu_count()*256, 1024)
                 cfit = skc.MiniBatchKMeans(n_clusters=i, tol=self.tol,
                                            max_iter=self.max_iter,
-                                           # n_init='auto',
+                                           n_init='auto',
                                            batch_size=bsize).fit(X)
             elif self.cltype == 'K-Means':
-                cfit = skc.KMeans(n_clusters=i, tol=self.tol, # n_init='auto',
+                cfit = skc.BisectingKMeans(n_clusters=i, tol=self.tol,
+                                           max_iter=self.max_iter).fit(X)
+
+            elif self.cltype == 'Bisecting K-Means':
+                cfit = skc.KMeans(n_clusters=i, tol=self.tol, n_init='auto',
                                   max_iter=self.max_iter).fit(X)
 
             elif self.cltype == 'DBSCAN':
                 cfit = skc.DBSCAN(eps=self.eps,
                                   min_samples=self.min_samples).fit(X)
 
             elif self.cltype == 'Birch':
                 X = np.ascontiguousarray(X)  # Birch gave an error without this
                 cfit = skc.Birch(n_clusters=i, threshold=self.bthres,
                                  branching_factor=self.branchfac).fit(X)
 
+            if cfit is None:
+                self.showlog('Could not find any clusters. '
+                             'Please change settings.')
+
             if cfit.labels_.max() < i-1 and self.cltype != 'DBSCAN':
-                self.showprocesslog('Could not find '+str(i)+' clusters. '
-                                    'Please change settings.')
+                self.showlog('Could not find '+str(i)+' clusters. '
+                             'Please change settings.')
 
                 return False
             if cfit.labels_.max() < 0 and self.cltype == 'DBSCAN':
-                self.showprocesslog('Could not find any clusters. '
-                                    'Please change settings.')
+                self.showlog('Could not find any clusters. '
+                             'Please change settings.')
 
                 return False
 
             dat_out.append(Data())
 
             dat_out[-1].metadata['Cluster']['input_type'] = []
             for k in data:
@@ -397,15 +406,16 @@
 
             zonal = np.ma.masked_all(data[0].data.shape)
             zonal[~masktmp] = cfit.labels_
 
             dat_out[-1].data = zonal
             dat_out[-1].nodata = zonal.fill_value
             dat_out[-1].metadata['Cluster']['no_clusters'] = i
-            dat_out[-1].metadata['Cluster']['center'] = np.zeros([i, len(data)])
+            dat_out[-1].metadata['Cluster']['center'] = np.zeros([i,
+                                                                  len(data)])
             dat_out[-1].metadata['Cluster']['center_std'] = np.zeros([i, len(data)])
             if cfit.labels_.max() > 0:
                 dat_out[-1].metadata['Cluster']['vrc'] = calinski_harabasz_score(X, cfit.labels_)
 
             # Reloading this hear to save memory. Need unscaled values.
             X = []
             for band in data:
@@ -429,19 +439,19 @@
             i.dataid = 'Clusters: '+str(i.metadata['Cluster']['no_clusters'])
             if self.cltype == 'DBSCAN':
                 i.dataid = 'Clusters: '+str(int(i.data.max()+1))
             i.nodata = data[0].nodata
             i.set_transform(transform=data[0].transform)
             i.crs = data[0].crs
 
-        self.showprocesslog('Cluster complete' + ' ('+self.cltype + ' ' + ')')
+        self.showlog('Cluster complete' + ' ('+self.cltype + ' ' + ')')
 
         for i in dat_out:
             i.data += 1
-            i.data = i.data.astype(np.uint8)
+            i.data = np.ma.masked_equal(i.data.filled(0).astype(int), 0)
             i.nodata = 0
 
         self.outdata['Cluster'] = dat_out
         self.outdata['Raster'] = self.indata['Raster']
 
         return True
 
@@ -538,16 +548,14 @@
 
     mdata = np.ma.mean(cdata2, 0)
     plt.figure(dpi=150)
     plt.imshow(mdata)
     plt.colorbar()
     plt.show()
 
-    breakpoint()
-
 
 def _test_marinda2():
     import sys
     import matplotlib.pyplot as plt
     from pygmi.raster.iodefs import get_raster
     from pygmi.raster.ginterp import norm2
 
@@ -582,20 +590,17 @@
     # Get cluster centers
     colormap = np.ma.ones((rows, cols, 4))
     colormap[:, :, 0] = norm2(cdata[0].data)
     colormap[:, :, 1] = norm2(cdata[1].data)
     colormap[:, :, 2] = norm2(cdata[2].data)
     colormap[:, :, 3] = np.logical_not(mask)
 
-
     # colormap[:, :, 3][colormap[:, :, 0]==0] = 0
 
     plt.figure(dpi=150)
     plt.imshow(colormap)
     plt.colorbar()
     plt.show()
 
-    breakpoint()
-
 
 if __name__ == "__main__":
     _testfn()
```

### Comparing `pygmi-3.2.6.5/pygmi/clust/crisp_clust.py` & `pygmi-3.2.7.16/pygmi/clust/crisp_clust.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import os
 import copy
 from PyQt5 import QtWidgets, QtCore
 import numpy as np
 
 from pygmi.raster.datatypes import Data
 import pygmi.clust.var_ratio as vr
-from pygmi.misc import ProgressBarText, BasicModule
+from pygmi.misc import BasicModule
 
 
 class CrispClust(BasicModule):
     """Crisp Cluster Class."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
@@ -174,21 +174,21 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         tst = np.unique([i.data.shape for i in self.indata['Raster']])
         if tst.size > 2:
-            self.showprocesslog('Error: Your input datasets have different '
-                                'sizes. Merge the data first')
+            self.showlog('Error: Your input datasets have different '
+                         'sizes. Merge the data first')
             return False
 
         self.update_vars()
 
         if not nodialog:
             temp = self.exec_()
             if temp == 0:
@@ -283,17 +283,17 @@
 
         cltype = self.cltype
         cov_constr = self.constrain
         no_runs = self.runs
         max_iter = self.max_iter
         term_thresh = self.term_thresh
         no_clust = np.array([self.min_cluster, self.max_cluster])
-        de_norm = self.denorm
+        # de_norm = self.denorm
 
-        self.showprocesslog('Crisp Clustering started')
+        self.showlog('Crisp Clustering started')
 
 # #############################################################################
 # Section to deal with different bands having different null values.
 # Start with the first entry
 #         masktmp = data[0].data.mask
 # # Add the all the masks to this. This promotes False values to True.
 #         for i in data:
@@ -303,15 +303,15 @@
 
         masktmp = ~data[0].data.mask
         for i in data:
             masktmp += ~i.data.mask
         masktmp = ~masktmp
         for datai in data:
             if datai.nodata != 0.0:
-                self.showprocesslog('Setting '+datai.dataid+' nodata to 0.')
+                self.showlog('Setting '+datai.dataid+' nodata to 0.')
                 datai.data = np.ma.array(datai.data.filled(0))
             datai.data.mask = masktmp
 
 # #############################################################################
 
         dat_in = np.array([i.data.compressed() for i in data]).T
 
@@ -370,18 +370,18 @@
                         smtmp = dummy_mod[cnt]
                     startmfix = {i: smtmp}
 
         cnt = -1
         dat_out = [Data() for i in range(no_clust[0], no_clust[1]+1)]
 
         for i in range(no_clust[0], no_clust[1]+1):
-            self.showprocesslog('Number of Clusters:'+str(i))
+            self.showlog('Number of Clusters:'+str(i))
             cnt = cnt + 1
             if self.radiobutton_datadriven.isChecked() is True:
-                self.showprocesslog('Initial guess: data driven')
+                self.showlog('Initial guess: data driven')
                 no_samp = dat_in.shape[0]
                 dno_samp = no_samp/i
                 idx = np.arange(0, no_samp+dno_samp, dno_samp)
                 idx[0] = 1
                 startmdat = {i: np.zeros([i, dat_in.shape[1]])}
                 dat_in1 = dat_in
                 smtmp = np.zeros([i, dat_in.shape[1]])
@@ -394,26 +394,26 @@
 
                 clidx, clcent, clobj_fcn, clvrc = self.crisp_means(
                     dat_in, i, startmdat[i], startmfix[i], max_iter,
                     term_thresh, cltype, cov_constr)
 
             elif self.radiobutton_manual.isChecked() is True:
 
-                self.showprocesslog('Initial guess: manual')
+                self.showlog('Initial guess: manual')
 
                 clidx, clcent, clobj_fcn, clvrc = self.crisp_means(
                     dat_in, i, startmdat[i], startmfix[i], max_iter,
                     term_thresh, cltype, cov_constr)
 
             elif self.radiobutton_random.isChecked() is True:
-                self.showprocesslog('Initial guess: random')
+                self.showlog('Initial guess: random')
 
                 clobj_fcn = np.array([np.inf])
                 for j in range(no_runs):
-                    self.showprocesslog('Run '+str(j+1)+' of'+str(no_runs))
+                    self.showlog(f'Run {j+1} of {no_runs}')
 
                     xmins = np.minimum(dat_in, 1)
                     xmaxs = np.maximum(dat_in, 1)
                     startm1dat = {i: np.random.uniform(
                         xmins[np.zeros(i, int), :],
                         xmaxs[np.zeros(i, int), :])}
                     startmfix = {i: np.array([])}
@@ -454,20 +454,20 @@
         for i in dat_out:
             i.dataid = ('Crisp Cluster: ' +
                         str(i.metadata['Cluster']['no_clusters']))
             i.nodata = data[0].nodata
             i.set_transform(transform=data[0].transform)
             i.crs = data[0].crs
 
-        self.showprocesslog('Crisp Cluster complete ('+self.cltype + ' ' +
-                            self.init_type+')')
+        self.showlog('Crisp Cluster complete ('+self.cltype + ' ' +
+                     self.init_type+')')
 
         for i in dat_out:
             i.data += 1
-            i.data = i.data.astype(np.uint8)
+            i.data = np.ma.masked_equal(i.data.filled(0).astype(int), 0)
             i.nodata = 0
         self.outdata['Cluster'] = dat_out
         self.outdata['Raster'] = self.indata['Raster']
 
         return True
 
     def crisp_means(self, data, no_clust, cent, centfix, maxit, term_thresh,
@@ -522,15 +522,15 @@
             matrix with cluster centre positions after last iteration, one
             cluster centre per row
         obj_fcn : numpy array
             Vector, size of the objective function after each iteration
         vrc : numpy array
             Variance Ratio Criterion
         """
-        self.showprocesslog(' ')
+        self.showlog(' ')
 
         no_samples = data.shape[0]
         if cent.size == 0:  # if no center values are provided
             xmins = np.minimum(data, 1)
             xmaxs = np.maximum(data, 1)
             cent = np.random.uniform(xmins[np.zeros(no_clust, int), :],
                                      xmaxs[np.zeros(no_clust, int), :])
@@ -556,42 +556,44 @@
 
         for i in self.piter(range(maxit)):  # =1:maxit. loop over all iters
             cent_prev = cent  # store result of last iteration
             idx_prev = idx
             dist_prev = edist
             # calc new cluster centre positions
             cent, idx = gcentroids(data, idx, no_clust, mindist)
-            # constrain the cluster center positions to keep it in  the given interval
+            # constrain the cluster center positions to keep it in  the given
+            # interval
             if centfix.size > 0:
                 # constrain the center positions within the given limits
                 cent_idx = cent > (cent_orig+centfix)
                 cent[cent_idx == 1] = (cent_orig(cent_idx == 1) +
                                        centfix(cent_idx == 1))
                 cent_idx = cent < (cent_orig-centfix)
                 cent[cent_idx == 1] = (cent_orig(cent_idx == 1) -
                                        centfix(cent_idx == 1))
 
             # calc new cluster centre distances
             edist = gdist(data, cent, idx, no_clust, cltype, cov_constr)
-            # get new index values for each data point and the distance from each
-            # sample to its cluster center
+            # get new index values for each data point and the distance from
+            # each sample to its cluster center
             mindist = edist.min(0)
             idx = edist.argmin(0)
 
             # calc new objective function size
             obj_fcn[i] = np.sum(mindist**2)
 
             if obj_fcn[i] == 0:
                 obj_fcn_dif = 0
             else:
                 obj_fcn_dif = 100 * ((obj_fcn_prev-obj_fcn[i]) / obj_fcn[i])
 
-            self.showprocesslog(f'Iteration: {i} Threshold: {term_thresh})'
-                                f' Current: {obj_fcn_dif:.2e}', True)
-            # if no termination threshold provided, ignore this and do all iterations
+            self.showlog(f'Iteration: {i} Threshold: {term_thresh})'
+                         f' Current: {obj_fcn_dif:.2e}', True)
+            # if no termination threshold provided, ignore this and do all
+            # iterations
             if term_thresh > 0:
                 # if the improvement between the last two iterations was less
                 # than a defined threshold in percent
                 if (obj_fcn_dif < term_thresh or obj_fcn[i] > obj_fcn_prev):
                     # go back to the results of the previous iteration
                     idx = idx_prev
                     cent = cent_prev
```

### Comparing `pygmi-3.2.6.5/pygmi/clust/fuzzy_clust.py` & `pygmi-3.2.7.16/pygmi/clust/fuzzy_clust.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,21 +183,21 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         tst = np.unique([i.data.shape for i in self.indata['Raster']])
         if tst.size > 2:
-            self.showprocesslog('Error: Your input datasets have different '
-                                'sizes. Merge the data first')
+            self.showlog('Error: Your input datasets have different '
+                         'sizes. Merge the data first')
             return False
 
         if not nodialog:
             self.update_vars()
             temp = self.exec_()
             if temp == 0:
                 return False
@@ -298,15 +298,15 @@
         no_runs = self.runs
         max_iter = self.max_iter
         term_thresh = self.term_thresh
         no_clust = np.array([self.min_cluster, self.max_cluster])
         de_norm = self.denorm
         expo = self.fexp
 
-        self.showprocesslog('Fuzzy Clustering started')
+        self.showlog('Fuzzy Clustering started')
 
 # #############################################################################
 # Section to deal with different bands having different null values.
 #         masktmp = data[0].data.mask   # Start with the first entry
 # # Add the masks to this.This promotes False values to True if necessary
 #         for i in data:
 #             masktmp += i.data.mask
@@ -315,15 +315,15 @@
 
         masktmp = ~data[0].data.mask
         for i in data:
             masktmp += ~i.data.mask
         masktmp = ~masktmp
         for datai in data:
             if datai.nodata != 0.0:
-                self.showprocesslog('Setting '+datai.dataid+' nodata to 0.')
+                self.showlog('Setting '+datai.dataid+' nodata to 0.')
                 datai.data = np.ma.array(datai.data.filled(0))
             datai.data.mask = masktmp
 
 # #############################################################################
 
         dat_in = np.array([i.data.compressed() for i in data]).T
 
@@ -382,18 +382,18 @@
                         smtmp = dummy_mod[cnt]
                     startmfix = {i: smtmp}
 
         cnt = -1
         dat_out = [Data() for i in range(no_clust[0], no_clust[1] + 1)]
 
         for i in range(no_clust[0], no_clust[1] + 1):
-            self.showprocesslog('Number of Clusters:' + str(i))
+            self.showlog(f'Number of Clusters: {i}')
             cnt = cnt + 1
             if self.radiobutton_datadriven.isChecked() is True:
-                self.showprocesslog('Initial guess: data driven')
+                self.showlog('Initial guess: data driven')
 
                 no_samp = dat_in.shape[0]
                 dno_samp = no_samp / i
                 idx = np.arange(0, no_samp + dno_samp, dno_samp)
                 idx[0] = 1
                 startmdat = {i: np.zeros([i, dat_in.shape[1]])}
                 dat_in1 = dat_in
@@ -406,27 +406,26 @@
                 del dat_in1
 
                 clu, clcent, clobj_fcn, clvrc, clnce, clxbi = self.fuzzy_means(
                     dat_in, i, startmdat[i], startmfix[i], max_iter,
                     term_thresh, expo, cltype, cov_constr)
 
             elif self.radiobutton_manual.isChecked() is True:
-                self.showprocesslog('Initial guess: manual')
+                self.showlog('Initial guess: manual')
 
                 clu, clcent, clobj_fcn, clvrc, clnce, clxbi = self.fuzzy_means(
                     dat_in, i, startmdat[i], startmfix[i],
                     max_iter, term_thresh, expo, cltype, cov_constr)
 
             elif self.radiobutton_random.isChecked() is True:
-                self.showprocesslog('Initial guess: random')
+                self.showlog('Initial guess: random')
 
                 clobj_fcn = np.array([np.Inf])
                 for j in range(no_runs):
-                    self.showprocesslog('Run ' + str(j+1) + ' of' +
-                                        str(no_runs))
+                    self.showlog(f'Run {j+1} of {no_runs}')
 
                     xmins = np.minimum(dat_in, 1)
                     xmaxs = np.maximum(dat_in, 1)
                     startm1dat = {i: np.random.uniform(
                         xmins[np.zeros(i, int), :],
                         xmaxs[np.zeros(i, int), :])}
                     startmfix = {i: np.array([])}
@@ -474,30 +473,30 @@
             dat_out[cnt].metadata['Cluster']['center_std'] = cent_std
 
             dat_out[cnt].metadata['Cluster']['memdat'] = []
             for k in range(clcent.shape[0]):
                 dummy = np.ones(data[0].data.shape) * np.nan
                 alpha1 = (data[0].data.mask == 0)
                 dummy[alpha1 == 1] = clu[k, :]
+                dummy = np.ma.masked_invalid(dummy)
                 dat_out[cnt].metadata['Cluster']['memdat'].append(dummy)
             dat_out[cnt].metadata['Cluster']['vrc'] = clvrc
             dat_out[cnt].metadata['Cluster']['nce'] = clnce
             dat_out[cnt].metadata['Cluster']['xbi'] = clxbi
             dat_out[cnt].metadata['Cluster']['obj_fcn'] = clobj_fcn
 
         for i in dat_out:
             i.dataid = ('Fuzzy Cluster: ' +
                         str(i.metadata['Cluster']['no_clusters']))
             i.nodata = data[0].nodata
             i.set_transform(transform=data[0].transform)
             i.data += 1
             i.crs = data[0].crs
 
-        self.showprocesslog('Fuzzy Cluster complete' + ' (' + self.cltype +
-                            ' ' + self.init_type + ')')
+        self.showlog(f'Fuzzy Cluster complete ({self.cltype} {self.init_type})')
 
         self.outdata['Cluster'] = dat_out
         self.outdata['Raster'] = self.indata['Raster']
 
         return True
 
     def fuzzy_means(self, data, no_clust, init, centfix, maxit, term_thresh,
@@ -559,15 +558,15 @@
         vrc : numpy array
             Variance ration criterion.
         nce :
             Normalised class entropy.
         xbi : numpy array
             Xie beni index.
         """
-        self.showprocesslog(' ')
+        self.showlog(' ')
 
         if cltype == 'fuzzy c-means':
             cltype = 'fcm'
         if cltype == 'advanced fuzzy c-means':
             cltype = 'det'
         if cltype == 'Gustafson-Kessel':
             cltype = 'gk'
@@ -605,15 +604,15 @@
             tmp = edist ** (-2.0 / (expo - 1))  # calc new U, suppose expo != 1
             uuu = tmp / (np.ones([no_clust, 1]) * np.sum(tmp, 0))
             m_f = uuu ** expo  # MF matrix after exponential modification
 
         # if membership matrix is provided
         elif init.shape[0] == no_clust and init.shape[1] == no_samples:
             if init[init < 0].size > 0:  # check for negative memberships
-                self.showprocesslog('No negative memberships allowed!')
+                self.showlog('No negative memberships allowed!')
                 # scale given memberships to a column sum of unity
             uuu = init / (np.ones([no_clust, 1]) * init.sum())
             # MF matrix after exponential modification
             m_f = uuu ** expo
             # new inital center matrix based on the given membership
             cent = m_f * data / ((np.ones([np.size(data, 2), 1]) *
                                   (m_f.T).sum()).T)
@@ -636,20 +635,19 @@
             # calc distances of each data point to each cluster centre
             edist = fuzzy_dist(cent, data, uuu, expo, cltype, cov_constr)
             tmp = edist ** (-2 / (expo - 1))  # calc new uuu, suppose expo != 1
             uuu = tmp / np.sum(tmp, 0)
             m_f = uuu ** expo
             obj_fcn[i] = np.sum((edist ** 2) * m_f)  # objective function
             if i > 0:
-                self.showprocesslog('Iteration: ' + str(i) + ' Threshold: ' +
-                                    str(term_thresh) + ' Current: ' +
-                                    '{:.2e}'.format(100*((obj_fcn[i - 1] -
-                                                          obj_fcn[i]) /
-                                                         obj_fcn[i - 1])),
-                                    True)
+                self.showlog('Iteration: ' + str(i) + ' Threshold: ' +
+                             str(term_thresh) + ' Current: ' +
+                             '{:.2e}'.format(100*((obj_fcn[i - 1] -
+                                                   obj_fcn[i]) /
+                                                  obj_fcn[i - 1])), True)
 
                 # if objective function has increased
                 if obj_fcn[i] > obj_fcn[i - 1]:
                     uuu = uprev  # use memberships and
                     cent = cent_prev  # centers od the previous iteration
                     #  eliminate last value for objective function and
                     obj_fcn = np.delete(obj_fcn, np.s_[i::])
```

### Comparing `pygmi-3.2.6.5/pygmi/clust/graphs.py` & `pygmi-3.2.7.16/pygmi/clust/graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     axes : matplotlib subplot
     parent : parent
         reference to the parent routine
     """
 
     def __init__(self, parent=None):
         # figure stuff
-        fig = Figure()
+        fig = Figure(layout='constrained')
         self.axes = fig.add_subplot(111)
         self.line = None
         self.ind = None
 
         super().__init__(fig)
 
     def update_classes(self, data1):
@@ -381,14 +381,16 @@
             self.mmc.update_wireframe(x.T, y.T, np.log(z))
 
         if (j == 'Variance Ratio Criterion' and
                 data[0].metadata['Cluster']['vrc'] is not None):
             x = [k.metadata['Cluster']['no_clusters'] for k in data]
             y = [k.metadata['Cluster']['vrc'] for k in data]
             self.mmc.update_scatter(x, y)
+
+        # nce and xbi are fuzzy clustering only.
         if (j == 'Normalized Class Entropy' and
                 data[0].metadata['Cluster']['nce'] is not None):
             x = [k.metadata['Cluster']['no_clusters'] for k in data]
             y = [k.metadata['Cluster']['nce'] for k in data]
             self.mmc.update_scatter(x, y)
         if (j == 'Xie-Beni Index' and
                 data[0].metadata['Cluster']['xbi'] is not None):
@@ -418,15 +420,15 @@
         if 'nce' in meta and len(data) > 1:
             items += ['Normalized Class Entropy']
 
         if 'xbi' in meta and len(data) > 1:
             items += ['Xie-Beni Index']
 
         if len(items) == 0:
-            self.showprocesslog('Your dataset does not qualify')
+            self.showlog('Your dataset does not qualify')
             return
 
         self.combobox1.addItems(items)
 
         self.label1.setText('Graph Type:')
         self.combobox1.setCurrentIndex(0)
         self.show()
```

### Comparing `pygmi-3.2.6.5/pygmi/clust/graphtool.py` & `pygmi-3.2.7.16/pygmi/clust/graphtool.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from matplotlib.lines import Line2D
 from matplotlib.path import Path
 from matplotlib.ticker import NullFormatter
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 
 from pygmi.misc import BasicModule
 
+
 class GraphHist(FigureCanvasQTAgg):
     """Graph Hist."""
 
     def __init__(self, parent=None):
         self.figure = Figure()
 
         super().__init__(self.figure)
@@ -74,16 +75,16 @@
         Returns
         -------
         xymahist : numpy array
             Output data.
 
         """
         xyhist = np.zeros((bins + 1, bins + 1))
-        xxx = self.xcoord.compressed()
-        yyy = self.ycoord.compressed()
+        xxx = self.xcoord.compressed().astype(int)
+        yyy = self.ycoord.compressed().astype(int)
 
         xyhist = np.histogram2d(xxx, yyy, bins + 1)
 
         xymahist = np.ma.masked_equal(xyhist[0], 0)
         return xymahist
 
     def get_clust_scat(self, bins, dattmp, ctmp):
@@ -104,16 +105,16 @@
         xymahist : numpy array
             Output data.
 
         """
         clust = np.ma.array(dattmp[ctmp[2] - 1].data.flatten())
         clust.mask = np.ma.getmaskarray(self.xcoord)
         clust = clust.compressed()
-        xxx = self.xcoord.compressed()
-        yyy = self.ycoord.compressed()
+        xxx = self.xcoord.compressed().astype(int)
+        yyy = self.ycoord.compressed().astype(int)
         xyhist = np.zeros((bins + 1, bins + 1))
 
         xyhist[xxx, yyy] = (clust + 1)
 
         xymahist = np.ma.masked_equal(xyhist, 0)
         return xymahist
 
@@ -190,14 +191,15 @@
         self.ycoord -= self.ycoord.min()
         xptp = self.xcoord.ptp()
         yptp = self.ycoord.ptp()
         xstep = xptp / 50
         ystep = yptp / 50
         self.xcoord = self.xcoord/xstep
         self.ycoord = self.ycoord/ystep
+
         self.xcoord = self.xcoord.astype(int)
         self.ycoord = self.ycoord.astype(int)
 
     def setup_hist(self):
         """
         Routine to setup the 1D histograms.
 
@@ -590,15 +592,14 @@
         -------
         None.
 
         """
         self.polymask = Path(self.poly.xy).contains_points(self.pntxy)
         self.polyi_changed.emit()
 
-
     def motion_notify_callback(self, event):
         """
         Mouse notify callback.
 
         Parameters
         ----------
         event : TYPE
@@ -703,15 +704,15 @@
         On cp delete polygon.
 
         Returns
         -------
         None.
 
         """
-        self.hist.polyi.new_poly([[10, 10]])
+        self.hist.polyi.new_poly([[1, 1]])
 
         mtmp = self.map_combo.currentIndex()
         mask = self.indata['Raster'][mtmp].data.mask
 
         dattmp = self.map.csp.get_array()
         dattmp.mask = mask
         self.map.csp.changed()
@@ -722,15 +723,15 @@
         On map delete polygon.
 
         Returns
         -------
         None.
 
         """
-        self.map.polyi.new_poly([[10, 10]])
+        self.map.polyi.new_poly([[1, 1]])
         dattmp = self.hist.csp.get_array()
         dattmp.mask = np.ma.getmaskarray(np.ma.masked_equal(dattmp.data, 0.))
         self.hist.csp.changed()
         self.hist.figure.canvas.draw()
 
     def on_cp_combo(self):
         """
@@ -817,17 +818,16 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('Error: You must have a multi-band raster '
-                                'dataset in addition to your cluster analysis'
-                                ' results')
+            self.showlog('Error: You must have a multi-band raster dataset '
+                         'in addition to your cluster analysis results')
             return False
 
         self.dat_tmp = self.indata['Raster']
         self.map.data = self.indata['Raster']
         self.hist.data = self.indata['Raster']
 
         bands = [i.dataid for i in self.indata['Raster']]
@@ -873,15 +873,14 @@
         self.map.polyi.polyi_changed.connect(self.update_hist)
 
         self.hist.update_graph(clearaxis=True)
         self.map.update_graph()
 
         self.exec_()
 
-
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
         Parameters
@@ -949,15 +948,15 @@
             return
 
         dattmp = self.hist.csp.get_array()
         atmp = np.array([self.hist.xcoord[polymask],
                          self.hist.ycoord[polymask]]).T
         dattmp.mask = np.ones_like(np.ma.getmaskarray(dattmp))
         for i in atmp:
-            dattmp.mask[i[1], i[0]] = False
+            dattmp.mask[int(i[1]), int(i[0])] = False
         self.hist.csp.changed()
         self.hist.figure.canvas.draw()
 
 
 def dist_point_to_segment(p, s0, s1):
     """
     Dist point to segment.
@@ -1015,12 +1014,10 @@
     app = QtWidgets.QApplication(sys.argv)
 
     DM = ScatterPlot()
     DM.indata['Raster'] = dat
     DM.indata['Cluster'] = dat2
     DM.settings()
 
-    aaa=1
-
 
 if __name__ == "__main__":
     _testfn()
```

### Comparing `pygmi-3.2.6.5/pygmi/clust/menu.py` & `pygmi-3.2.7.16/pygmi/clust/menu.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/clust/segmentation.py` & `pygmi-3.2.7.16/pygmi/clust/segmentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         data1 = []
         for i in self.indata['Raster']:
             data1.append(i.data.data)
 
         data1 = np.array(data1)
@@ -244,15 +244,15 @@
         -------
         omap : numpy array
             Output data.
 
         """
         rows, cols, bands = data.shape
 
-        self.showprocesslog('Initialising...')
+        self.showlog('Initialising...')
 
         olist = {}
         slist = {}
         mlist = {}
         nlist = {}
         omap = np.zeros((rows, cols))
 
@@ -267,20 +267,20 @@
                 olist[i*cols+j] = set(tmp)
                 for k in range(bands):
                     slist[(k, i*cols+j)] = 0
                     mlist[(k, i*cols+j)] = data[i, j, k]
                     nlist[(k, i*cols+j)] = 1
                 omap[i, j] = i*cols+j
 
-        self.showprocesslog('merging...')
+        self.showlog('merging...')
 
         omap = self._segment2(omap, olist, slist, mlist, nlist, bands,
                               doshape, wcompact, wcolor, scale)
 
-        self.showprocesslog('renumbering...')
+        self.showlog('renumbering...')
         tmp = np.unique(omap)
 
         for i, val in enumerate(tmp):
             omap[omap == val] = i
 
         return omap.astype(int)
 
@@ -337,15 +337,15 @@
             elist = set(olist.keys())
 
             clen = len(elist)
             if self.pbar is not None:
                 self.pbar.setMaximum(clen)
                 self.pbar.setMinimum(0)
                 self.pbar.setValue(0)
-            self.showprocesslog('Iteration number: '+str(cnt))
+            self.showlog('Iteration number: '+str(cnt))
             oldperc = 0
 
             olist3 = olist.copy()
 
             while elist:
                 i = elist.pop()
 
@@ -483,15 +483,16 @@
                     if self.pbar is not None:
                         self.pbar.setValue(cnow)
                     oldperc = cnow*1000//clen
 
                 rmin, rmax = rminmax[i]
                 cmin, cmax = cminmax[i]
 
-                omap[rmin:rmax+1, cmin:cmax+1][omap[rmin:rmax+1, cmin:cmax+1] == hind] = i
+                omap[rmin:rmax+1, cmin:cmax+1][omap[rmin:rmax+1,
+                                                    cmin:cmax+1] == hind] = i
 
         return omap
 
 
 @jit(nopython=True, fastmath=True)
 def get_l(data):
     """
@@ -522,46 +523,43 @@
 
 
 def _testfn():
     """Test routine."""
     import sys
     import matplotlib.pyplot as plt
     from pygmi.raster.datatypes import Data
-    from pygmi.misc import PTime
     from matplotlib import rcParams
 
     rcParams['figure.dpi'] = 300
 
     app = QtWidgets.QApplication(sys.argv)
 
     data1 = skimage.data.coffee()  # 400x600 48.5 secs
 
     plt.imshow(data1)
     plt.axis('off')
     plt.show()
 
-    wcolor = 0.5
-    wcompact = 0.5
-    doshape = True
-    scale = 1000
+    # wcolor = 0.5
+    # wcompact = 0.5
+    # doshape = True
+    # scale = 1000
 
     b1 = Data()
     b1.data = np.ma.array(data1[:, :, 0])
     b2 = Data()
     b2.data = np.ma.array(data1[:, :, 1])
     b3 = Data()
     b3.data = np.ma.array(data1[:, :, 2])
 
     data = [b1, b2, b3]
 
-    ttt = PTime()
     IS = ImageSeg()
     IS.indata = {'Raster': data}
     IS.settings()
-    ttt.since_last_call()
 
     odata = IS.outdata['Raster'][0]
 
     plt.imshow(odata.data)
     plt.axis('off')
     plt.show()
```

### Comparing `pygmi-3.2.6.5/pygmi/clust/super_class.py` & `pygmi-3.2.7.16/pygmi/clust/super_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -845,17 +845,16 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('Error: You must have a multi-band raster '
-                                'dataset in addition to your cluster '
-                                'analysis results')
+            self.showlog('Error: You must have a multi-band raster dataset in '
+                         'addition to your cluster analysis results')
             return False
 
         self.map.data = self.indata['Raster']
 
         bands = [i.dataid for i in self.indata['Raster']]
 
         self.combo.clear()
@@ -897,15 +896,16 @@
 
         i = len(lbls)
 
         dat_out[-1].data = zonal
         dat_out[-1].nodata = zonal.fill_value
         dat_out[-1].metadata['Cluster']['no_clusters'] = i
         dat_out[-1].metadata['Cluster']['center'] = np.zeros([i, len(data)])
-        dat_out[-1].metadata['Cluster']['center_std'] = np.zeros([i, len(data)])
+        dat_out[-1].metadata['Cluster']['center_std'] = np.zeros([i,
+                                                                  len(data)])
 
         m = []
         s = []
         for i2 in lbls:
             m.append(datall[yout1 == i2].mean(0))
             s.append(datall[yout1 == i2].std(0))
 
@@ -915,19 +915,18 @@
         dat_out[-1].crs = data[0].crs
         dat_out[-1].dataid = 'Clusters: '+str(dat_out[-1].metadata['Cluster']['no_clusters'])
         dat_out[-1].nodata = data[0].nodata
         dat_out[-1].set_transform(transform=data[0].transform)
 
         for i in dat_out:
             i.data += 1
-            i.data = i.data.astype(np.uint8)
+            i.data = np.ma.masked_equal(i.data.filled(0).astype(int), 0)
             i.nodata = 0
-            i.data.data[i.data.mask] = 0
 
-        self.showprocesslog('Cluster complete')
+        self.showlog('Cluster complete')
 
         self.outdata['Cluster'] = dat_out
         self.outdata['Raster'] = self.indata['Raster']
 
         return True
 
     def loadproj(self, projdata):
@@ -1045,15 +1044,15 @@
             tlbls.append(lbl)
 
         y = np.array(y)
         x = np.vstack(x)
         lbls = np.unique(y)
 
         if len(lbls) < 2:
-            self.showprocesslog('Error: You need at least two classes')
+            self.showlog('Error: You need at least two classes')
 
         X_train, X_test, y_train, y_test = train_test_split(x, y, stratify=y)
 
         classifier.fit(X_train, y_train)
 
         return classifier, lbls, datall, X_test, y_test, tlbls
 
@@ -1153,15 +1152,14 @@
     from pygmi.raster import iodefs
 
     app = QtWidgets.QApplication(sys.argv)
 
     ifile = r"D:\Workdata\PyGMI Test Data\Classification\Cut_K_Th_U.ers"
 
     data = iodefs.get_raster(ifile)
-    # os.chdir(r'd:\Workdata\people\janinetest2')
 
     tmp = SuperClass(None)
     tmp.indata['Raster'] = data
     tmp.settings()
 
 
 if __name__ == "__main__":
```

### Comparing `pygmi-3.2.6.5/pygmi/clust/var_ratio.py` & `pygmi-3.2.7.16/pygmi/clust/var_ratio.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/em/menu.py` & `pygmi-3.2.7.16/pygmi/em/menu.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/em/tdem.py` & `pygmi-3.2.7.16/pygmi/em/tdem.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from pygmi.misc import QLabelVStack, BasicModule
 
 
 class MyMplCanvas2(FigureCanvasQTAgg):
     """MPL Canvas class."""
 
     def __init__(self, parent=None):
-        fig = Figure()
+        fig = Figure(layout='constrained')
         super().__init__(fig)
 
     def update_line(self, sigma, z, times_off, zobs, zpred):
         """
         Update the plot from data.
 
         Parameters
@@ -91,15 +91,15 @@
         ax2.set_xlim(times_off.min()*1.2, times_off.max()*1.1)
         ax2.set_xlabel(r"Time ($\mu s$)")
         ax2.set_ylabel("dBz / dt (V/A-m$^4$)")
         ax2.set_title("High-moment")
         ax2.grid(True)
         ax2.legend(loc=3)
 
-        self.figure.tight_layout()
+        # self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def disp_wave(self, times, wave, title):
         """
         Display waveform.
 
         Returns
@@ -113,15 +113,15 @@
         ax1.grid(True)
         ax1.set_ylabel('Amplitude')
         ax1.set_xlabel('Time (s)')
         ax1.set_title(title)
 
         ax1.plot(times, wave)
 
-        self.figure.tight_layout()
+        # self.figure.tight_layout()
         self.figure.canvas.draw()
 
 
 class TDEM1D(BasicModule):
     """Occam 1D inversion."""
 
     def __init__(self, parent=None):
@@ -504,31 +504,33 @@
 
         Returns
         -------
         wform : tdem waveform.
             Waveform.
 
         """
+        starttime = 0.
         offtime = float(self.txofftime.text())
         peaktime = float(self.txpeaktime.text())
         rampoff1 = float(self.txrampoff1.text())
 
-        rampon = np.array([0, peaktime])
+        rampon = np.array([starttime, peaktime])
         rampoff = np.array([rampoff1, offtime])
 
         wtype = self.combowtype.currentText()
 
         if wtype == 'VTEMWaveform':
             wform = time_domain.sources.VTEMWaveform(off_time=offtime,
                                                      peak_time=peaktime)
         elif wtype == 'TrapezoidWaveform':
             wform = time_domain.sources.TrapezoidWaveform(ramp_on=rampon,
                                                           ramp_off=rampoff)
         elif wtype == 'TriangularWaveform':
-            wform = time_domain.sources.TriangularWaveform(peak_time=peaktime,
+            wform = time_domain.sources.TriangularWaveform(start_time=starttime,
+                                                           peak_time=peaktime,
                                                            off_time=offtime)
         elif wtype == 'QuarterSineRampOnWaveform':
             wform = time_domain.sources.QuarterSineRampOnWaveform(
                 ramp_on=rampon, ramp_off=rampoff)
         elif wtype == 'HalfSineWaveform':
             wform = time_domain.sources.HalfSineWaveform(ramp_on=rampon,
                                                          ramp_off=rampoff)
@@ -591,30 +593,27 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
-        if 'Line' in self.indata:
-            self.data = copy.deepcopy(self.indata['Line'])
-            self.data = list(self.data.values())[0]
+        if 'Vector' in self.indata:
+            self.data = copy.deepcopy(self.indata['Vector'][0])
         else:
-            self.showprocesslog('No line data')
+            self.showlog('No line data')
             return False
 
         self.comboline.currentIndexChanged.disconnect()
         self.comboline.clear()
         self.combofid.clear()
         self.combobalt.clear()
 
         filt = ((self.data.columns != 'geometry') &
-                (self.data.columns != 'line') &
-                (self.data.columns != 'pygmiX') &
-                (self.data.columns != 'pygmiY'))
+                (self.data.columns != 'line'))
 
         cnames = list(self.data.columns[filt])
 
         self.combobalt.addItems(cnames)
         for i, tmp in enumerate(cnames):
             tmp = tmp.lower()
             if ('elev' in tmp or 'alt' in tmp or 'height' in tmp or
@@ -699,23 +698,23 @@
         return float(test)
 
     return int(test)
 
 
 def _testfn():
     """Test routine."""
-    from pygmi.vector.iodefs import ImportLineData
+    from pygmi.vector.iodefs import ImportXYZ
 
     app = QtWidgets.QApplication(sys.argv)
 
     # Load in line data
     filename = r'D:\Workdata\PyGMI Test Data\EM\SK655CS_Bookpurnong_ZX_HM_TxInc_newDTM.txt'
     wfile = r'D:\Workdata\PyGMI Test Data\EM\wtimes.txt'
 
-    IO = ImportLineData()
+    IO = ImportXYZ()
     IO.filt = 'Tab Delimited (*.txt)'
     IO.ifile = filename
     IO.xchan.setCurrentText('e')
     IO.ychan.setCurrentText('n')
     IO.nodata.setText('-99999')
     IO.settings(True)
```

### Comparing `pygmi-3.2.6.5/pygmi/grav/dataprep.py` & `pygmi-3.2.7.16/pygmi/grav/dataprep.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         self.dataid = QtWidgets.QComboBox()
         self.density = QtWidgets.QLineEdit('2670')
         self.knownstat = QtWidgets.QLineEdit('None')
         self.knownbase = QtWidgets.QLineEdit('978000.0')
         self.absbase = QtWidgets.QLineEdit('978032.67715')
         self.basethres = QtWidgets.QLineEdit('10000')
 
+        self.gdata = None
+
         self.setupui()
 
     def setupui(self):
         """
         Set up UI.
 
         Returns
@@ -112,41 +114,48 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
+        self.gdata = None
         tmp = []
-        if 'Line' not in self.indata:
-            self.showprocesslog('No Line Data')
+        if 'Vector' not in self.indata:
+            self.showlog('No Line Data')
             return False
-        if 'Gravity' not in self.indata['Line']:
-            self.showprocesslog('Not Gravity Data')
+
+        for i in self.indata['Vector']:
+            if 'Gravity' in i.attrs:
+                self.gdata = i
+                break
+
+        if self.gdata is None:
+            self.showlog('Not Gravity Data')
             return False
 
         if not nodialog:
             tmp = self.exec_()
         else:
             tmp = 1
 
         try:
             float(self.density.text())
             float(self.absbase.text())
             float(self.basethres.text())
             float(self.knownbase.text())
         except ValueError:
-            self.showprocesslog('Value Error')
+            self.showlog('Value Error')
             return False
 
         if self.knownstat.text() != 'None':
             try:
                 float(self.knownstat.text())
             except ValueError:
-                self.showprocesslog('Value Error')
+                self.showlog('Value Error')
                 return False
 
         if tmp != 1:
             return False
 
         self.acceptall(nodialog)
 
@@ -208,15 +217,15 @@
         Updates self.outdata, which is used as input to other modules.
 
         Returns
         -------
         None.
 
         """
-        pdat = self.indata['Line']['Gravity']
+        pdat = self.gdata
         pdat.sort_values(by=['DECTIMEDATE'], inplace=True)
 
         basethres = float(self.basethres.text())
         kstat = self.knownstat.text()
         if kstat == 'None':
             kstat = -1.0
         else:
@@ -242,16 +251,16 @@
         fp = driftdat['GRAV'].values
 
         x = pdat['DECTIMEDATE'].values
         xp = driftdat['DECTIMEDATE'].values
 
         dcor = np.interp(x, xp, fp)
 
-        self.showprocesslog('Quality Control')
-        self.showprocesslog('---------------')
+        self.showlog('Quality Control')
+        self.showlog('---------------')
         tmp = driftdat['DECTIMEDATE'].values.astype(int)
         tmp2 = []
         ix = []
         tcnt = 0
         for i, val in enumerate(tmp[:-1]):
             tmp2.append(tcnt)
             if tmp[i+1] != val:
@@ -266,22 +275,22 @@
         dday = []
         for iday in np.unique(ix):
             filt = (ix == iday)
             x2 = xp1[filt].values/60.
             dcor2 = fp[filt]
             drifttime = (x2[-1]-x2[0])
             if drifttime == 0.:
-                self.showprocesslog(f'Day {iday+1} drift: Only one reading, '
-                                    'no drift result possible.')
+                self.showlog(f'Day {iday+1} drift: Only one reading, '
+                             'no drift result possible.')
                 driftrate = np.nan
 
             else:
                 driftrate = (dcor2[-1]-dcor2[0])/drifttime
-                self.showprocesslog(f'Day {iday+1} drift: {driftrate:.3e} '
-                                    f'mGal/min over {drifttime:.3f} minutes.')
+                self.showlog(f'Day {iday+1} drift: {driftrate:.3e} '
+                             f'mGal/min over {drifttime:.3f} minutes.')
             dday.append(iday+1+x2[-1]/1440)
             drate.append(driftrate)
             dtime.append(drifttime)
 
         xp2 = xp1/86400 + ix+1
 
         if not nodialog:
@@ -326,29 +335,29 @@
         pdat = pdat.assign(gATM=gATM)
         pdat = pdat.assign(gHC=gHC)
         pdat = pdat.assign(gSB=gSB)
         pdat = pdat.assign(BOUGUER=gba)
 
         pdat.sort_values(by=['LINE', 'STATION'], inplace=True)
 
-        self.outdata['Line'] = {'Gravity': pdat}
+        self.outdata['Vector'] = [pdat]
 
     def calcbase(self):
         """
         Calculate local base station value.
 
         Ties in the local base station to a known absolute base station.
 
         Returns
         -------
         None.
 
 
         """
-        pdat = self.indata['Line']['Gravity']
+        pdat = self.gdata
 
         basethres = float(self.basethres.text())
 
         if self.knownstat.text() == 'None':
             txt = ('Invalid base station number.')
             QtWidgets.QMessageBox.warning(self.parent, 'Error',
                                           txt, QtWidgets.QMessageBox.Ok)
@@ -570,17 +579,17 @@
     PD.basethres.setText(bthres)
     PD.knownstat.setText(kbase)
     PD.knownbase.setText('978794.53')
     PD.calcbase()
 
     PD.settings(True)
 
-    datout = PD.outdata['Line']
+    datout = PD.outdata['Vector']
 
-    gdf = datout['Gravity']
+    gdf = datout[0]
 
     for i in ['GRAV', 'gobs_drift', 'BOUGUER', 'dcor', 'elevation',
               'gT', 'gATM', 'gHC', 'gSB']:
         plt.title(i)
 
         plt.plot(gdf.x, gdf[i])
         plt.show()
```

### Comparing `pygmi-3.2.6.5/pygmi/grav/iodefs.py` & `pygmi-3.2.7.16/pygmi/grav/iodefs.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # -----------------------------------------------------------------------------
 """Import Data."""
 
 import os
 from PyQt5 import QtWidgets, QtCore
 import numpy as np
 import pandas as pd
+import geopandas as gpd
 
 from pygmi import menu_default
 from pygmi.misc import BasicModule
 
 
 class ImportCG5(BasicModule):
     """
@@ -141,29 +142,29 @@
         if not nodialog:
             tmp = self.exec_()
 
             if tmp != 1 or self.df_cg5 is None or self.df_gps is None:
                 return False
 
         if self.line.currentText() == self.station.currentText():
-            self.showprocesslog('Your line column cannot be the same as your '
-                                'station column')
+            self.showlog('Your line column cannot be the same as your '
+                         'station column')
             return False
 
         tmp = [self.line.currentText(),
                self.station.currentText(),
                self.xchan.currentText(),
                self.ychan.currentText(),
                self.zchan.currentText()]
 
         if len(set(tmp)) != len(tmp):
-            self.showprocesslog('Unable to import, two of your GPS file '
-                                'columns are the same. Make sure you have a '
-                                'line column in your GPS file, and that you '
-                                'did not specify the same column twice.')
+            self.showlog('Unable to import, two of your GPS file '
+                         'columns are the same. Make sure you have a '
+                         'line column in your GPS file, and that you '
+                         'did not specify the same column twice.')
             return False
 
         # Rename columns
         cren = {}
         cren[self.line.currentText()] = 'line'
         cren[self.station.currentText()] = 'station'
         cren[self.xchan.currentText()] = 'longitude'
@@ -176,28 +177,28 @@
             filt = self.df_gps.latitude.str.contains('S')
             self.df_gps.latitude.loc[filt] = '-'+self.df_gps.latitude[filt]
             self.df_gps.latitude.replace('S', '', inplace=True, regex=True)
             self.df_gps.latitude.replace('N', '', inplace=True, regex=True)
             try:
                 self.df_gps.latitude = pd.to_numeric(self.df_gps.latitude)
             except ValueError:
-                self.showprocesslog('You have characters in your latitude'
-                                    ' string which could not be converted.')
+                self.showlog('You have characters in your latitude'
+                             ' string which could not be converted.')
                 return False
 
         if self.df_gps.longitude.dtype == 'O':
             filt = self.df_gps.longitude.str.contains('W')
             self.df_gps.longitude.loc[filt] = '-'+self.df_gps.longitude[filt]
             self.df_gps.longitude.replace('W', '', inplace=True, regex=True)
             self.df_gps.longitude.replace('E', '', inplace=True, regex=True)
             try:
                 self.df_gps.longitude = pd.to_numeric(self.df_gps.longitude)
             except ValueError:
-                self.showprocesslog('You have characters in your longitude'
-                                    ' string which could not be converted.')
+                self.showlog('You have characters in your longitude'
+                             ' string which could not be converted.')
                 return False
 
         # Get rid of text in line columns
         if self.df_gps['line'].dtype == object:
             self.df_gps['line'] = self.df_gps['line'].str.replace(r'\D', '')
 
         # Convert line and station to numbers
@@ -217,28 +218,32 @@
         # eliminate ordinary stations (not base stations) without coordinates
         filt = dfmerge['STATION'] < float(self.basethres.text())
 
         filt = filt & dfmerge['longitude'].isna()
 
         dfmerge = dfmerge[~filt]
 
-        dfmerge['pygmiX'] = dfmerge['longitude']
-        dfmerge['pygmiY'] = dfmerge['latitude']
+        x = dfmerge['longitude']
+        y = dfmerge['latitude']
+        dfmerge = gpd.GeoDataFrame(dfmerge, geometry=gpd.points_from_xy(x, y))
 
         dfmerge['line'] = dfmerge['line'].astype(str)
-        self.outdata['Line'] = {'Gravity': dfmerge}
+        dfmerge.attrs['Gravity'] = True
+        dfmerge.attrs['source'] = str(self.cg5file.text())
+        self.outdata['Vector'] = [dfmerge]
 
+        # Check for duplicates
         dtest = dfmerge.duplicated(['LINE', 'STATION'])
         dlist = dfmerge[['LINE', 'STATION']].loc[dtest]
         dlist = dlist[~dlist.duplicated()]
         dlist = dlist[dlist.STATION < float(self.basethres.text())]
 
         if dlist.size > 0:
-            self.showprocesslog('Warning, the following are duplicated:')
-            self.showprocesslog(dlist.to_string(index=False))
+            self.showlog('Warning, the following are duplicated:')
+            self.showlog(dlist.to_string(index=False))
 
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
```

### Comparing `pygmi-3.2.6.5/pygmi/grav/menu.py` & `pygmi-3.2.7.16/pygmi/grav/menu.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.bhole.rawcore.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.bhole.rawcore.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.clust.cluster.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.clust.cluster.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.clust.segmentation.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.clust.segmentation.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.em.tdem1d.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.em.tdem1d.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.grav.dataprep.processdata.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.grav.dataprep.processdata.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.grav.iodefs.importpointdata.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.grav.iodefs.importpointdata.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.main.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.main.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.mt.edit.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.mt.edit.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.mt.occam1d.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.mt.occam1d.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.mt.rotate.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.mt.rotate.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.mt.static.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.mt.static.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.ddisp.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.ddisp.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.iodefs.exportkmz.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.iodefs.exportkmz.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.iodefs.importpicture.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.iodefs.importpicture.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.mext.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.mext.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.minv.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.minv.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.misc.mergemod3d.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.misc.mergemod3d.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.misc.rangedcopy.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.misc.rangedcopy.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.param.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.param.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.pfmod.prof.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.pfmod.prof.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.cooper.gradients.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.cooper.gradients.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.cooper.tilt.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.cooper.tilt.html`

 * *Files 14% similar despite different names*

```diff
@@ -5,10 +5,11 @@
 		<p>This calculates the tilt angle of the data. It allows for smoothing as well. It outputs the Standard tilt angle, Hyperbolic tilt angle, 2nd order tilt angle, Tilt Based Directional Derivative and the Total Derivative</p>
 		<h2>Options</h2>
 		<ul>
 			<li>Smoothing Matrix - an odd matrix used to smooth the data</li>
 			<li>Azimuth - This is the direction of the tilt angle, in degrees from east. It is used in the tilt based directional derivative.</li>
 		</ul>
 		<h2>References</h2>
-		<p>Cooper,G.R.J.,Cowan, D.R. 2006. Enhancing potential field data using filters based on the local phase. Computers and Geosciences,32, p.1585-1591</p>
+		<p>Cooper,G.R.J., Cowan, D.R. 2006. Enhancing potential field data using filters based on the local phase. Computers and Geosciences,32, p.1585-1591</p>
+		<p>Ferreira, F., Souza, J., Bongiolo, A., Castro, L. (2013). Enhancement of the total horizontal gradient of magnetic anomalies using the tilt angle. GEOPHYSICS. 78. J33-J41. 10.1190/geo2011-0441.1.</p>
 	</body>
 </html>
```

#### html2text {}

```diff
@@ -3,9 +3,12 @@
 outputs the Standard tilt angle, Hyperbolic tilt angle, 2nd order tilt angle,
 Tilt Based Directional Derivative and the Total Derivative
 ***** Options *****
     * Smoothing Matrix - an odd matrix used to smooth the data
     * Azimuth - This is the direction of the tilt angle, in degrees from east.
       It is used in the tilt based directional derivative.
 ***** References *****
-Cooper,G.R.J.,Cowan, D.R. 2006. Enhancing potential field data using filters
+Cooper,G.R.J., Cowan, D.R. 2006. Enhancing potential field data using filters
 based on the local phase. Computers and Geosciences,32, p.1585-1591
+Ferreira, F., Souza, J., Bongiolo, A., Castro, L. (2013). Enhancement of the
+total horizontal gradient of magnetic anomalies using the tilt angle.
+GEOPHYSICS. 78. J33-J41. 10.1190/geo2011-0441.1.
```

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.cooper.visibility.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.cooper.visibility.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.dataprep.cont.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.dataprep.cont.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.dataprep.datalayerstack.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.dataprep.datalayerstack.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.dataprep.datamerge.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.dataprep.datamerge.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.ginterp.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.ginterp.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.igrf.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.igrf.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.normalisation.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.normalisation.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.smooth.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.smooth.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.raster.tiltdepth.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.raster.tiltdepth.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.cind.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.cind.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.iodefs.exportbatch.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.iodefs.exportbatch.html`

 * *Files 12% similar despite different names*

```diff
@@ -7,10 +7,12 @@
 		<ul>
 			<li>Output Directory - location for output files.</li>
 			<li>Output format - file format to export data to.</li>
 			<li>Ternary Export - checkbox if only three band are to be exported.</li>
 			<li>Red Band - used in ternary export.</li>
 			<li>Green Band - used in ternary export.</li>
 			<li>Blue Band - used in ternary export.</li>
+			<li>Sunshade Band - the band used for the sunshading layer. This can be an external dataset.</li>
+			<li>Sunshade Level - used to set the severity of sun shading.</li>
 		</ul>
 	</body>
 </html>
```

#### html2text {}

```diff
@@ -4,7 +4,10 @@
 ***** Options *****
     * Output Directory - location for output files.
     * Output format - file format to export data to.
     * Ternary Export - checkbox if only three band are to be exported.
     * Red Band - used in ternary export.
     * Green Band - used in ternary export.
     * Blue Band - used in ternary export.
+    * Sunshade Band - the band used for the sunshading layer. This can be an
+      external dataset.
+    * Sunshade Level - used to set the severity of sun shading.
```

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.iodefs.importsentinel5p.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.iodefs.importsentinel5p.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.landsat_composite.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.landsat_composite.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.mnf.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.mnf.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.pca.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.pca.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.pfeat.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.pfeat.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.rsense.ratios.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.rsense.ratios.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/helpdocs/pygmi.vector.dataprep.datagrid.html` & `pygmi-3.2.7.16/pygmi/helpdocs/pygmi.vector.dataprep.datagrid.html`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/images/Help.png` & `pygmi-3.2.7.16/pygmi/images/Help.png`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/images/cgslogo.png` & `pygmi-3.2.7.16/pygmi/images/cgslogo.png`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/images/delete.png` & `pygmi-3.2.7.16/pygmi/images/delete.png`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/images/logo256.ico` & `pygmi-3.2.7.16/pygmi/images/logo256.ico`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/images/play.png` & `pygmi-3.2.7.16/pygmi/images/play.png`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/images/pygmi.png` & `pygmi-3.2.7.16/pygmi/images/pygmi.png`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/mag/IGRF13.COF` & `pygmi-3.2.7.16/pygmi/mag/IGRF13.COF`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/mag/dataprep.py` & `pygmi-3.2.7.16/pygmi/mag/dataprep.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 """A set of Magnetic Data routines."""
 
 import copy
 from PyQt5 import QtWidgets, QtCore
 import numpy as np
-from scipy.signal import tukey
+from scipy.signal.windows import tukey
 import scipy.interpolate as si
 from scipy import signal
 from pygmi import menu_default
 
 from pygmi.raster.datatypes import Data
 from pygmi.misc import BasicModule
 
@@ -111,47 +111,53 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         if not nodialog:
             temp = self.exec_()
             if temp == 0:
                 return False
 
         self.smooth = self.sb_s.value()
         self.azi = self.sb_azi.value()
 
         data = copy.deepcopy(self.indata['Raster'])
         data2 = []
 
         for i in self.piter(range(len(data))):
-            t1, th, t2, ta, tdx = tilt1(data[i].data, self.azi, self.smooth)
+            t1, th, t2, ta, tdx, tahg = tilt1(data[i].data, self.azi,
+                                              self.smooth)
             data2.append(copy.deepcopy(data[i]))
             data2.append(copy.deepcopy(data[i]))
             data2.append(copy.deepcopy(data[i]))
             data2.append(copy.deepcopy(data[i]))
             data2.append(copy.deepcopy(data[i]))
-            data2[-5].data = t1
-            data2[-4].data = th
-            data2[-3].data = t2
-            data2[-2].data = ta
-            data2[-1].data = tdx
-            data2[-5].dataid += ' Standard Tilt Angle'
-            data2[-4].dataid += ' Hyperbolic Tilt Angle'
-            data2[-3].dataid += ' 2nd Order Tilt Angle'
-            data2[-2].dataid += ' Tilt Based Directional Derivative'
-            data2[-1].dataid += ' Total Derivative'
+            data2.append(copy.deepcopy(data[i]))
+            data2[-6].data = t1
+            data2[-5].data = th
+            data2[-4].data = t2
+            data2[-3].data = ta
+            data2[-2].data = tdx
+            data2[-1].data = tahg
+            data2[-6].dataid += ' Standard Tilt Angle'
+            data2[-5].dataid += ' Hyperbolic Tilt Angle'
+            data2[-4].dataid += ' 2nd Order Tilt Angle'
+            data2[-3].dataid += ' Tilt Based Directional Derivative'
+            data2[-2].dataid += ' Total Derivative'
+            data2[-1].dataid += ' Tilt Angle of the Horizontal Gradient'
 
         for i in data2:
+            if i.nodata is None:
+                continue
             i.data.data[i.data.mask] = i.nodata
 
         self.outdata['Raster'] = data2
         return True
 
     def loadproj(self, projdata):
         """
@@ -263,15 +269,24 @@
     dzs = vertical(ts, npts, 1)
     dxtots = np.ma.sqrt(dxs*dxs+dys*dys)
     t2 = np.ma.arctan(dzs/dxtots)
 
     # Standard tilt angle, hyperbolic tilt angle, 2nd order tilt angle,
     # Tilt Based Directional Derivative, Total Derivative
 
-    return t1, th, t2, ta, tdx
+    data = dxtot
+    nr, nc = data.shape
+    dy, dx = np.gradient(data)
+    dxtot = np.ma.sqrt(dx*dx+dy*dy)
+    nmax = np.max([nr, nc])
+    npts = int(2**nextpow2(nmax))
+    dz = vertical(data, npts, 1)
+    tahg = np.ma.arctan(dz/dxtot)
+
+    return t1, th, t2, ta, tdx, tahg
 
 
 def nextpow2(n):
     """
     Next power of 2.
 
     Based on work by Gordon Cooper (School of Geosciences, University of the
@@ -418,15 +433,15 @@
         -------
         bool
             True if successful, False otherwise.
 
         """
         tmp = []
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         for i in self.indata['Raster']:
             tmp.append(i.dataid)
 
         self.dataid.clear()
         self.dataid.addItems(tmp)
@@ -681,15 +696,15 @@
     get_ipython().run_line_magic('matplotlib', 'inline')
 
     ifile = 'd:/Workdata/bugs/detlef/TMI_norm_wdw.tif'
     ifile = r'C:/Workdata/raster/ER Mapper/magmicrolevel.PD.ers'
 
     dat = get_raster(ifile)[0]
 
-    t1, th, t2, ta, tdx = tilt1(dat.data, 75, 0)
+    t1, th, t2, ta, tdx, tahg = tilt1(dat.data, 75, 0)
 
     plt.figure(dpi=150)
     plt.imshow(t2)
     plt.colorbar()
     plt.show()
 
     plt.figure(dpi=150)
```

### Comparing `pygmi-3.2.6.5/pygmi/mag/igrf.py` & `pygmi-3.2.7.16/pygmi/mag/igrf.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,21 +196,21 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         for i in self.indata['Raster']:
             if i.crs is None:
-                self.showprocesslog(f'{i.dataid} has no projection. '
-                                    'Please assign one.')
+                self.showlog(f'{i.dataid} has no projection. '
+                             'Please assign one.')
                 return False
 
         if self.wkt is None:
             self.wkt = self.indata['Raster'][0].crs.wkt
 
         self.proj.set_current(self.wkt)
 
@@ -234,15 +234,15 @@
         i = self.combobox_mag.currentIndex()
 
         for i in data:
             if i.dataid == self.combobox_mag.currentText():
                 dxy = min(i.xdim, i.ydim)
 
         data = dp.lstack(data, dxy=dxy, piter=self.piter,
-                         pprint=self.showprocesslog)
+                         showlog=self.showlog)
 
         for i in data:
             if i.dataid == self.combobox_mag.currentText():
                 maggrid = i
             if i.dataid == self.combobox_dtm.currentText():
                 data = i
                 wkt = i.crs.wkt
@@ -250,15 +250,15 @@
         sdate = self.dateedit.date()
         sdate = sdate.year()+sdate.dayOfYear()/sdate.daysInYear()
         alt = self.dsb_alt.value()
 
         odata, fmean, imean, dmean = calc_igrf(data, sdate, alt=alt, wkt=wkt,
                                                igrfonly=False,
                                                piter=self.piter,
-                                               pprint=self.showprocesslog)
+                                               showlog=self.showlog)
         bname = 'Magnetic Data: IGRF Corrected '
         bname = bname + f'F:{fmean:.2f} I:{imean:.2f} D:{dmean:.2f}'
 
         self.outdata['Raster'] = odata
 
         self.outdata['Raster'].append(copy.deepcopy(maggrid))
         self.outdata['Raster'][-1].data -= odata[0].data
@@ -303,15 +303,15 @@
         projdata['alt'] = self.dsb_alt.value()
         projdata['date'] = self.dateedit.date().toString()
 
         return projdata
 
 
 def calc_igrf(data, sdate, alt=100, wkt=None, igrfonly=True, piter=iter,
-              pprint=print):
+              showlog=print):
     """
     Calculate IGRF.
 
     Parameters
     ----------
     data : PyGMI data
         Input magnetic data.
@@ -321,15 +321,15 @@
         Sensor clearance. The default is 100.
     wkt : str, optional
         WKT projection. The default is None.
     igrfonly : bool, optional
         Output IGRF only. The default is True.
     piter : iter, optional
         Progress bar iterator. The default is iter.
-    pprint : print, optional
+    showlog : print, optional
         Print routine. The default is print.
 
     Returns
     -------
     outdata : PyGMI data
         Output data.
     fmean : float
@@ -393,17 +393,17 @@
     igrf_D = altgrid * 0
     # Pick model
     yrmax = np.array(yrmax)
     modelI = sum(yrmax < sdate)
     igdgc = 1
 
     if maxyr < sdate < maxyr+1:
-        pprint('Warning: The date ' + str(sdate) + ' is out of range,')
-        pprint('but still within one year of model expiration date.')
-        pprint('An updated model file is available before 1.1.' + str(maxyr))
+        showlog('Warning: The date ' + str(sdate) + ' is out of range,')
+        showlog('but still within one year of model expiration date.')
+        showlog('An updated model file is available before 1.1.' + str(maxyr))
 
     if max2[modelI] == 0:
         gh = getshc(modbuff, 1, irec_pos[modelI], max1[modelI], 0, gh)
         gh = getshc(modbuff, 1, irec_pos[modelI+1], max1[modelI+1], 1, gh)
         nmax, gh = interpsh(sdate, yrmin[modelI], max1[modelI],
                             yrmin[modelI+1], max1[modelI+1], 2, gh)
         nmax, gh = interpsh(sdate+1, yrmin[modelI], max1[modelI],
@@ -454,19 +454,19 @@
     igrf_D.shape = data.data.shape
     igrf_D.mask = np.ma.getmaskarray(data.data)
 
     fmean = igrf_F.mean()
     imean = igrf_I.mean()
     dmean = igrf_D.mean()
 
-    pprint('Mean Values in Calculation')
-    pprint('=============================')
-    pprint(f'Total Intensity: {fmean:.2f}')
-    pprint(f'Inclination: {imean:.2f}')
-    pprint(f'Declination: {dmean:.2f}')
+    showlog('Mean Values in Calculation')
+    showlog('=============================')
+    showlog(f'Total Intensity: {fmean:.2f}')
+    showlog(f'Inclination: {imean:.2f}')
+    showlog(f'Declination: {dmean:.2f}')
 
     outdata = []
     outdata.append(copy.deepcopy(data))
     outdata[-1].data = igrf_F
     outdata[-1].dataid = 'IGRF'
 
     if not igrfonly:
```

### Comparing `pygmi-3.2.6.5/pygmi/mag/menu.py` & `pygmi-3.2.7.16/pygmi/mag/menu.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/mag/tiltdepth.py` & `pygmi-3.2.7.16/pygmi/mag/tiltdepth.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.backends.backend_qt5 import NavigationToolbar2QT
 from numba import jit
 
 from pygmi.raster.datatypes import Data
 from pygmi.raster.cooper import vertical
 from pygmi.raster.dataprep import lstack
-from pygmi.mag.dataprep import rtp
+from pygmi.mag.dataprep import rtp, nextpow2
 from pygmi.vector.dataprep import quickgrid
 from pygmi.misc import frm, ProgressBar, BasicModule
 from pygmi import menu_default
 
 
 class TiltDepth(BasicModule):
     """
@@ -85,14 +85,15 @@
 
         self.cbox_band1 = QtWidgets.QComboBox()
         self.cbox_cbar = QtWidgets.QComboBox(self)
         self.dsb_inc = QtWidgets.QDoubleSpinBox()
         self.dsb_dec = QtWidgets.QDoubleSpinBox()
         self.btn_apply = QtWidgets.QPushButton('Calculate Tilt Depth')
         self.btn_save = QtWidgets.QPushButton('Save Depths to Text File')
+        self.do_rtp = QtWidgets.QCheckBox('Perform RTP on data')
         self.pbar = ProgressBar()
 
         self.setupui()
 
     def setupui(self):
         """
         Set up UI.
@@ -110,32 +111,35 @@
 
         self.dsb_inc.setMaximum(90.0)
         self.dsb_inc.setMinimum(-90.0)
         self.dsb_inc.setValue(-67.)
         self.dsb_dec.setMaximum(360.0)
         self.dsb_dec.setMinimum(-360.0)
         self.dsb_dec.setValue(-17.)
+        self.do_rtp.setChecked(True)
 
         vbl_raster = QtWidgets.QVBoxLayout()
         hbl_all = QtWidgets.QHBoxLayout(self)
         vbl_right = QtWidgets.QVBoxLayout()
 
         mpl_toolbar = NavigationToolbar2QT(self.mmc, self)
         spacer = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum,
                                        QtWidgets.QSizePolicy.Expanding)
         tmp = sorted(colormaps.keys())
-        self.cbox_cbar.addItem('jet')
+        self.cbox_cbar.addItem('viridis')
         self.cbox_cbar.addItems(tmp)
 
         self.setWindowTitle('Tilt Depth Interpretation')
 
         vbl_raster.addWidget(label2)
         vbl_raster.addWidget(self.cbox_band1)
         vbl_raster.addWidget(labelc)
         vbl_raster.addWidget(self.cbox_cbar)
+
+        vbl_raster.addWidget(self.do_rtp)
         vbl_raster.addWidget(label_inc)
         vbl_raster.addWidget(self.dsb_inc)
         vbl_raster.addWidget(label_dec)
         vbl_raster.addWidget(self.dsb_dec)
         vbl_raster.addWidget(self.btn_apply)
         vbl_raster.addWidget(self.pbar)
         vbl_raster.addItem(spacer)
@@ -144,16 +148,33 @@
         vbl_right.addWidget(self.mmc)
         vbl_right.addWidget(mpl_toolbar)
 
         hbl_all.addLayout(vbl_raster)
         hbl_all.addLayout(vbl_right)
 
         self.cbox_cbar.currentIndexChanged.connect(self.change_cbar)
-        self.btn_apply.clicked.connect(self.change_band1)
+        self.btn_apply.clicked.connect(self.calculate)
         self.btn_save.clicked.connect(self.save_depths)
+        self.do_rtp.clicked.connect(self.rtp_choice)
+
+    def rtp_choice(self):
+        """
+        Check if RTP must be done.
+
+        Returns
+        -------
+        None.
+
+        """
+        if self.do_rtp.isChecked():
+            self.dsb_inc.setEnabled(True)
+            self.dsb_dec.setEnabled(True)
+        else:
+            self.dsb_inc.setEnabled(False)
+            self.dsb_dec.setEnabled(False)
 
     def save_depths(self):
         """
         Save depths.
 
         Returns
         -------
@@ -177,15 +198,15 @@
                    header='x, y, id, depth')
 
         QtWidgets.QMessageBox.information(self.parent, 'Information',
                                           'Save completed!')
 
         return True
 
-    def change_cbar(self):
+    def change_cbar_old(self):
         """
         Change the colour map for the colour bar.
 
         Returns
         -------
         None.
 
@@ -214,41 +235,75 @@
             self.axes.plot(self.x1[i], self.y1[i], 'oy')
             self.axes.plot(self.x0[i], self.y0[i], 'sy')
             self.axes.plot(self.x2[i], self.y2[i], 'oy')
 
         self.axes.xaxis.set_major_formatter(frm)
         self.axes.yaxis.set_major_formatter(frm)
 
-        self.figure.colorbar(ims, format=frm)
+        self.figure.colorbar(ims, format=frm, label='Tilt Angle')
+
+        self.figure.canvas.draw()
+
+    def change_cbar(self):
+        """
+        Change the colour map for the colour bar.
+
+        Returns
+        -------
+        None.
+
+        """
+        if 'Raster' not in self.outdata:
+            return
+
+        zout = self.outdata['Raster'][0]
+        txt = str(self.cbox_cbar.currentText())
+
+        self.figure.clear()
+        self.axes = self.figure.add_subplot(111)
+
+        cmap = colormaps[txt]
+
+        vmin = zout.data.mean() - 2.5*zout.data.std()
+        vmax = zout.data.mean() + 2.5*zout.data.std()
+
+        ims = self.axes.imshow(zout.data, extent=zout.extent, cmap=cmap,
+                               interpolation='nearest', vmin=vmin, vmax=vmax)
+
+        self.axes.xaxis.set_major_formatter(frm)
+        self.axes.yaxis.set_major_formatter(frm)
+
+        self.figure.colorbar(ims, format=frm, label='Depth')
 
         self.figure.canvas.draw()
 
-    def change_band1(self):
+    def calculate(self):
         """
         Routine which occurs when apply button is pressed.
 
         Returns
         -------
         None.
 
         """
         txt = str(self.cbox_band1.currentText())
 
         self.btn_apply.setText('Calculating...')
-        QtWidgets.QApplication.processEvents()
         self.btn_apply.setEnabled(False)
 
         for i in self.indata['Raster']:
             if i.dataid == txt:
-                self.tiltdepth(i)
-                self.change_cbar()
+                dat = i
+                break
+
+        self.tiltdepth(dat)
+        self.change_cbar()
 
         self.btn_apply.setEnabled(True)
         self.btn_apply.setText('Calculate Tilt Depth')
-        QtWidgets.QApplication.processEvents()
 
     def settings(self, nodialog=False):
         """
         Entry point into item.
 
         Parameters
         ----------
@@ -258,30 +313,36 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         self.indata['Raster'] = lstack(self.indata['Raster'])
 
         data = self.indata['Raster']
         blist = []
         for i in data:
             blist.append(i.dataid)
 
         self.cbox_band1.clear()
         self.cbox_band1.addItems(blist)
 
-        if nodialog is False:
-            self.show()
-        QtWidgets.QApplication.processEvents()
+        # if nodialog is False:
+        #     self.show()
+        if not nodialog:
+            tmp = self.exec_()
+        else:
+            tmp = 1
+
+        if tmp != 1:
+            return False
 
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
@@ -331,23 +392,31 @@
         self.pbar.setValue(0)
         self.pbar.setMaximum(4)
 
         # RTP
         inc = self.dsb_inc.value()
         dec = self.dsb_dec.value()
 
-        zout = rtp(data, inc, dec)
+        if self.do_rtp.isChecked():
+            zout = rtp(data, inc, dec)
+        else:
+            zout = data
 
         # Tilt
         self.pbar.setValue(1)
 
         nr, nc = zout.data.shape
         dy, dx = np.gradient(zout.data)
-        dxtot = np.sqrt(dx**2+dy**2)
-        dz = vertical(zout.data)
+        dxtot = np.ma.sqrt(dx**2+dy**2)
+
+        nmax = np.max([nr, nc])
+        npts = int(2**nextpow2(nmax))
+        dz = vertical(zout.data, npts, 1)
+
+        # dz = vertical(zout.data)
         t1 = np.arctan(dz/dxtot)
 
         self.pbar.setValue(2)
         # A negative number implies we are straddling 0
 
         # Contour tilt
         x = zout.extent[0] + np.arange(nc)*zout.xdim+zout.xdim/2
@@ -417,30 +486,30 @@
         self.y0 = gy0
         self.y1 = dy1+gy0
         self.y2 = dy2+gy0
 
         self.depths = np.transpose([gx0, gy0, cntid0.astype(int), dist])
 
         tmp = quickgrid(gx0, gy0, dist, data.xdim,
-                        showprocesslog=self.showprocesslog)
+                        showlog=self.showlog)
 
         mask = np.ma.getmaskarray(tmp)
         gdat = tmp.data
 
         dat = Data()
         dat.data = np.ma.masked_invalid(gdat[::-1])
         dat.data.mask = mask[::-1]
         dat.nodata = dat.data.fill_value
         dat.set_transform(data.xdim, gx0.min(), data.ydim, gy0.max())
-        dat.dataid = data.dataid
+        dat.dataid = data.dataid+' depths'
 
         self.outdata['Raster'] = [dat]
 
 
-@jit(nopython=True, nogil=True)
+@jit(nopython=True)
 def distpc(dx, dy, dx0, dy0, dcnt):
     """
     Find closest distances.
 
     Parameters
     ----------
     dx : numpy array
@@ -515,7 +584,33 @@
 
     cgrad = np.arctan2(dy2, dx2)
     cgrad = np.rad2deg(cgrad)
     cgrad[cgrad > 90] -= 180.
     cgrad[cgrad < -90] += 180.
 
     return np.array(gx), np.array(gy), cgrad, np.array(cntid)
+
+
+def _testfn():
+    """RTP testing routine."""
+    import sys
+    from pygmi.raster.iodefs import get_raster
+
+    ifile = r"D:\Workdata\PyGMI Test Data\IGRF_RTP.tif"
+
+    dat = get_raster(ifile)
+
+    app = QtWidgets.QApplication(sys.argv)
+
+    tmp1 = TiltDepth()
+    tmp1.indata['Raster'] = dat
+    tmp1.do_rtp.setChecked(False)
+    tmp1.dsb_inc.setValue(-63.)
+    tmp1.dsb_dec.setValue(-16.)
+
+    tmp1.settings()
+
+    dat = tmp1.outdata
+
+
+if __name__ == "__main__":
+    _testfn()
```

### Comparing `pygmi-3.2.6.5/pygmi/main.py` & `pygmi-3.2.7.16/pygmi/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 import sys
 import os
 import pkgutil
 import math
 import importlib
 from PyQt5 import QtWidgets, QtCore, QtGui
 import numpy as np
+import psutil
 from matplotlib import rcParams
 from matplotlib import interactive
 
 import pygmi
 from pygmi import menu_default
 from pygmi import misc
 
@@ -203,15 +204,15 @@
 
         self.diagram_type = diagram_type
         self.context_menu = context_menu
         self.my_class = my_class
         self.is_import = False
         self.text_item = None
         self.my_class_name = ''
-        self.showprocesslog = parent.showprocesslog
+        self.showlog = parent.showlog
 
         if hasattr(self.my_class, 'arrows'):
             self.my_class.arrows = self.arrows
 
         path = QtGui.QPainterPath()
         if self.diagram_type == 'StartEnd':
             path.moveTo(200, 50)
@@ -372,21 +373,21 @@
         if self.my_class.indata == {} and self.is_import is False:
             QtWidgets.QMessageBox.warning(self.parent, 'Warning',
                                           ' You need to connect data first!',
                                           QtWidgets.QMessageBox.Ok)
             return False
 
         self.my_class.parent.process_is_active()
-        self.showprocesslog(self.my_class_name+' busy...')
+        self.showlog(self.my_class_name+' busy...')
         iflag = self.my_class.settings(nodialog)
         self.my_class.parent.process_is_active(False)
         if iflag:
-            self.showprocesslog(self.my_class_name+' finished!')
+            self.showlog(self.my_class_name+' finished!')
         else:
-            self.showprocesslog(self.my_class_name+' cancelled.')
+            self.showlog(self.my_class_name+' cancelled.')
         return iflag
 
 
 class DiagramScene(QtWidgets.QGraphicsScene):
     """Diagram Scene."""
 
     def __init__(self, item_menu, parent=None):
@@ -424,29 +425,31 @@
 
         self.selected_item_info()
 
     # now display the information about the selected data
     def selected_item_info(self):
         """Display info about selected item."""
         tmp = self.selectedItems()
+        self.parent.showdatainfo('')
+
         if not tmp:
             return
 
         if not hasattr(tmp[0], 'my_class'):
             return
 
         text = ''
 
         if hasattr(tmp[0].my_class, 'indata'):
             idata = tmp[0].my_class.indata
 
             for i in idata:
                 text += '\nInput ' + i + ' dataset: '
                 if i in 'Raster':
-                    if hasattr(idata[i][0], 'filename'):
+                    if idata[i] and hasattr(idata[i][0], 'filename'):
                         file = idata[i][0].filename
                     else:
                         file = i
                     if '.SAFE' in file:
                         file = file.split('.SAFE')[0]+'.SAFE'
                     text += os.path.basename(file) + '\n'
                     for j in idata[i]:
@@ -456,15 +459,15 @@
             odata = tmp[0].my_class.outdata
 
             for i in odata:
                 text += '\nOutput ' + i + ' dataset: '
                 if i == 'RasterFileList':
                     text += i + '\n'
                     for j in odata[i]:
-                        text += os.path.basename(j) + '\n'
+                        text += os.path.basename(j.filename) + '\n'
                 if i in ('Raster', 'Cluster'):
                     if hasattr(odata[i][0], 'filename'):
                         file = odata[i][0].filename
                     else:
                         file = i
                     if '.SAFE' in file:
                         file = file.split('.SAFE')[0]+'.SAFE'
@@ -612,15 +615,19 @@
         start.update()
 
         menuimports = []
         for i in menus:
             if i == 'pygmi.__pycache__.menu':
                 continue
             start.update()
-            menuimports.append(importlib.import_module(i))
+            try:
+                menuimports.append(importlib.import_module(i))
+            except ModuleNotFoundError as err:
+                self.showlog(f'{i} cannot be loaded, {err}')
+            # menuimports.append(importlib.import_module(i))
         start.close()
 
         self.menus = []
         self.menus.append(menu_default.FileMenu(self))
         for i in menuimports:
             self.menus.append(i.MenuWidget(self))
         self.menus.append(menu_default.HelpMenu(self))
@@ -660,14 +667,19 @@
         self.graphics_view.setSizePolicy(sizepolicy)
         self.graphics_view.setTransformationAnchor(
             QtWidgets.QGraphicsView.AnchorUnderMouse)
 
         self.textbrowser_datainfo.setSizePolicy(sizepolicy)
         self.textbrowser_processlog.setSizePolicy(sizepolicy)
 
+        fstyle = (QtWidgets.QFrame.Shape.Box | QtWidgets.QFrame.Shadow.Plain)
+        self.textbrowser_datainfo.setFrameStyle(fstyle)
+        self.textbrowser_processlog.setFrameStyle(fstyle)
+        self.graphics_view.setFrameStyle(fstyle)
+
         self.grid_layout.addWidget(self.graphics_view, 0, 0, 4, 2)
         self.grid_layout.addWidget(self.textbrowser_datainfo, 1, 2, 1, 1)
         self.grid_layout.addWidget(self.textbrowser_processlog, 3, 2, 1, 1)
         self.grid_layout.addWidget(self.pbar, 5, 0, 1, 3)
 
         label = QtWidgets.QLabel('Dataset Information:')
         label_2 = QtWidgets.QLabel('Process Log:')
@@ -946,15 +958,15 @@
         Change process log colour when a process is active.
 
         Parameters
         ----------
         isactive : bool, optional
             boolean variable indicating if a process is active.
         """
-        if isactive:
+        if isactive is True:
             self.textbrowser_processlog.setStyleSheet(
                 'QTextBrowser { background-color: rgba(255, 0, 0, 127); }')
             self.pbar.setValue(0)
         else:
             self.textbrowser_processlog.setStyleSheet(
                 'QTextBrowser { background-color: rgb(255, 255, 255); }')
 
@@ -964,15 +976,15 @@
 
         Returns
         -------
         None.
 
         """
         self.process_is_active()
-        self.showprocesslog('Project load busy...')
+        self.showlog('Project load busy...')
 
         ifile, _ = QtWidgets.QFileDialog.getOpenFileName(
             self, 'Open Project', '.', 'PyGMI project (*.json);;')
         if ifile == '':
             return False
 
         with open(ifile, 'r', encoding='utf-8') as fromdisk:
@@ -1075,15 +1087,15 @@
         # get all arrows
         alist = {}
         for item in self.scene.items():
             if isinstance(item, Arrow):
                 alist[str(item)] = item
 
         if not alist:
-            self.showprocesslog('No connections. Aborting run.')
+            self.showlog('No connections. Aborting run.')
             return
 
         # Collect only items receiving data
         ilist = []
         slist = []
         for item in self.scene.items():
             if isinstance(item, DiagramItem):
@@ -1165,15 +1177,15 @@
             Message to be displayed in the datainfo panel
         """
         self.textbrowser_datainfo.setPlainText(txt)
         tmp = self.textbrowser_datainfo.verticalScrollBar()
         tmp.setValue(tmp.maximumHeight())
         self.repaint()
 
-    def showprocesslog(self, txt, replacelast=False):
+    def showlog(self, txt, replacelast=False):
         """
         Show text on the process log.
 
         Parameters
         ----------
         txt : str
             Message to be displayed in the process log
@@ -1251,14 +1263,17 @@
         self.pbar.setValue(self.pbar.value() + 1)
         QtWidgets.QApplication.processEvents()
 
 
 def main(nocgs=False):
     """Entry point for the PyGMI software."""
     # Set environment variables.
+    # The line below is to fix a problem in windows with loky library.
+    os.environ['LOKY_MAX_CPU_COUNT'] = str(psutil.cpu_count(logical=False))
+
     if 'GDAL_DATA' not in os.environ:
         import osgeo
         gdalpath = os.path.join(osgeo.__path__[0], r'data\gdal')
         if os.path.exists(gdalpath):
             os.environ['GDAL_DATA'] = gdalpath
         else:
             print('GDAL_PATH not set.')
```

### Comparing `pygmi-3.2.6.5/pygmi/menu_default.py` & `pygmi-3.2.7.16/pygmi/menu_default.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/misc.py` & `pygmi-3.2.7.16/pygmi/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 """
 Misc is a collection of routines which can be used in PyGMI in general.
 """
 
+import os
 import sys
 import types
 import time
 import psutil
 import numpy as np
 from matplotlib import ticker
-from PyQt5 import QtWidgets, QtCore
+from PyQt5 import QtWidgets, QtCore, QtGui
 
 
 PBAR_STYLE = """
 QProgressBar{
     border: 2px solid grey;
     border-radius: 5px;
     text-align: center
@@ -110,37 +111,39 @@
         dictionary of output datasets
     ifile : str
         input file, used in IO routines and to pass filename back to main.py
     piter : iter
         reference to a progress bar iterator.
     pbar : progressbar
         reference to a progress bar.
-    showprocesslog: stdout or alternative
+    showlog: stdout or alternative
         reference to a way to view messages, normally stdout or a Qt text box.
     """
 
     def __init__(self, parent=None):
         super().__init__(parent)
         if parent is None:
             self.stdout_redirect = sys.stdout
-            self.showprocesslog = print
+            self.showlog = print
             self.pbar = ProgressBarText()
-            self.process_is_active = print
+            self.process_is_active = lambda *args, **kwargs: None
         else:
-            self.stdout_redirect = EmittingStream(parent.showprocesslog)
-            self.showprocesslog = parent.showprocesslog
+            self.stdout_redirect = EmittingStream(parent.showlog)
+            self.showlog = parent.showlog
             self.pbar = parent.pbar
             self.process_is_active = parent.process_is_active
 
         self.piter = self.pbar.iter
 
         self.indata = {}
         self.outdata = {}
         self.parent = parent
         self.ifile = ''
+        self.ipth = os.path.dirname(__file__)+r'/images/'
+        self.setWindowIcon(QtGui.QIcon(self.ipth+'logo256.ico'))
 
     def settings(self, nodialog=False):
         """
         Entry point into item.
 
         Parameters
         ----------
@@ -213,37 +216,40 @@
         dictionary of input datasets
     outdata : dictionary
         dictionary of output datasets
     piter : iter
         reference to a progress bar iterator.
     pbar : progressbar
         reference to a progress bar.
-    showprocesslog: stdout or alternative
+    showlog: stdout or alternative
         reference to a way to view messages, normally stdout or a Qt text box.
     """
 
     def __init__(self, parent=None):
         super().__init__(parent)
         if parent is None:
             self.stdout_redirect = sys.stdout
-            self.showprocesslog = print
+            self.showlog = print
             self.pbar = ProgressBarText()
-            self.process_is_active = print
+            self.process_is_active = lambda *args, **kwargs: None
         else:
-            self.stdout_redirect = EmittingStream(parent.showprocesslog)
-            self.showprocesslog = parent.showprocesslog
+            self.stdout_redirect = EmittingStream(parent.showlog)
+            self.showlog = parent.showlog
             self.pbar = parent.pbar
             self.process_is_active = parent.process_is_active
 
         self.piter = self.pbar.iter
 
         self.indata = {}
         self.outdata = {}
         self.parent = parent
 
+        self.ipth = os.path.dirname(__file__)+r'/images/'
+        self.setWindowIcon(QtGui.QIcon(self.ipth+'logo256.ico'))
+
     def run(self):
         """
         Run context menu item.
 
         Returns
         -------
         None.
@@ -535,16 +541,16 @@
     x : float/int
         Number to be formatted.
     pos : int
         Position of tick.
 
     Returns
     -------
-    newx : TYPE
-        DESCRIPTION.
+    newx : str
+        Formatted coordinate.
 
     """
     if np.ma.is_masked(x):
         return '--'
 
     newx = f'{x:,.5f}'.rstrip('0').rstrip('.')
```

### Comparing `pygmi-3.2.6.5/pygmi/mt/birrp.py` & `pygmi-3.2.7.16/pygmi/mt/birrp.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         data = data.replace('\n', ' ')
         data = data.replace(',', ' ')
 
         data = data.split()
 
         ilev = data.pop(0)
         if int(ilev) != 0:
-            self.showprocesslog('not supported')
+            self.showlog('not supported')
             return
         nout = int(data.pop(0))
         ninp = int(data.pop(0))
         tbw = data.pop(0)
         deltat = data.pop(0)
         nfft = data.pop(0)
         nsctmax = data.pop(0)
@@ -297,33 +297,33 @@
         uin = data.pop(0)
         ainuin = data.pop(0)
         c2threshe = data.pop(0)
         nz = 0
         if nout == 3:
             nz = int(data.pop(0))
         elif nout == 1:
-            self.showprocesslog('not supported')
+            self.showlog('not supported')
             return
         c2threshe1 = ''
         if int(nout) == 3 and int(nz) == 0:
             c2threshe1 = data.pop(0)
         ofil = data.pop(0)
         nlev = int(data.pop(0))
         npcs = data.pop(0)
         nar = data.pop(0)
         imode = int(data.pop(0))
         jmode = int(data.pop(0))
         if imode != 0:
-            self.showprocesslog('not supported')
+            self.showlog('not supported')
             return
         nread = ''
         if jmode == 0:
             nread = data.pop(0)
         else:
-            self.showprocesslog('not supported')
+            self.showlog('not supported')
             return
 
         nfil = {}
         fpar = {}
         cpar = {}
         arfilnam = {}
         filnam = {}
```

### Comparing `pygmi-3.2.6.5/pygmi/mt/dataprep.py` & `pygmi-3.2.7.16/pygmi/mt/dataprep.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             if self.dsb_utmx.text() != 'None':
                 odata.east = float(self.dsb_utmx.text())
             if self.dsb_utmy.text() != 'None':
                 odata.north = float(self.dsb_utmy.text())
             odata.elev = float(self.dsb_elev.text())
             odata.rotation_angle = float(self.dsb_rot.text())
         except ValueError:
-            self.showprocesslog('Value error - abandoning changes')
+            self.showlog('Value error - abandoning changes')
 
         indx = self.combobox_bandid.currentIndex()
         txt = self.combobox_bandid.itemText(indx)
         self.oldtxt = txt
         idata = self.banddata[txt]
 
         self.dsb_lat.setText(str(idata.lat))
@@ -266,15 +266,15 @@
         return True
 
 
 class MyMplCanvas(FigureCanvasQTAgg):
     """MPL Canvas class."""
 
     def __init__(self, parent=None):
-        fig = Figure()
+        fig = Figure(layout='constrained')
         super().__init__(fig)
 
     def update_line(self, data, ival, itype):
         """
         Update the plot from point data.
 
         Parameters
@@ -352,15 +352,15 @@
 
         ax2.set_xscale('log')
         ax2.set_yscale('linear')
         ax2.legend(loc='upper left')
         ax2.set_xlabel('Period (s)')
         ax2.set_ylabel(r'Phase (Degrees)')
 
-        self.figure.tight_layout()
+        # self.figure.tight_layout()
         self.figure.canvas.draw()
 
 
 class StaticShiftEDI(BasicModule):
     """Static shift EDI data."""
 
     def __init__(self, parent=None):
@@ -511,15 +511,15 @@
         bool
             True if successful, False otherwise.
 
         """
         if 'MT - EDI' in self.indata:
             self.data = copy.deepcopy(self.indata['MT - EDI'])
         else:
-            self.showprocesslog('No EDI data')
+            self.showlog('No EDI data')
             return False
 
         self.combobox1.currentIndexChanged.disconnect()
 
         self.combobox1.clear()
         for i in self.data:
             self.combobox1.addItem(i)
@@ -722,15 +722,15 @@
         bool
             True if successful, False otherwise.
 
         """
         if 'MT - EDI' in self.indata:
             self.data = copy.deepcopy(self.indata['MT - EDI'])
         else:
-            self.showprocesslog('No EDI data')
+            self.showlog('No EDI data')
             return False
 
         self.combobox1.currentIndexChanged.disconnect()
         self.combobox1.clear()
 
         for i in self.data:
             self.combobox1.addItem(i)
@@ -1202,15 +1202,15 @@
         bool
             True if successful, False otherwise.
 
         """
         if 'MT - EDI' in self.indata:
             self.data = copy.deepcopy(self.indata['MT - EDI'])
         else:
-            self.showprocesslog('No EDI data')
+            self.showlog('No EDI data')
             return False
 
         self.combobox1.currentIndexChanged.disconnect()
         self.combobox1.clear()
 
         for i in self.data:
             self.combobox1.addItem(i)
@@ -1311,15 +1311,15 @@
                                                                self.width()))
 
 
 class MyMplCanvas2(FigureCanvasQTAgg):
     """MPL Canvas class."""
 
     def __init__(self, parent=None):
-        fig = Figure()
+        fig = Figure(layout='constrained')
         super().__init__(fig)
 
     def update_line(self, x, pdata, rdata, depths=None, res=None, title=None):
         """
         Update the plot from data.
 
         Parameters
@@ -1384,15 +1384,15 @@
         ax3.yaxis.set_label_position("right")
         ax3.set_xlabel(r'Res. ($\Omega.m$)')
         ax3.set_ylabel(r'Depth (km)')
 
         if depths is not None:
             ax3.plot(res, np.array(depths)/1000)
 
-        gs.tight_layout(self.figure)
+        # gs.tight_layout(self.figure)
         self.figure.canvas.draw()
 
 
 class Occam1D(BasicModule):
     """Occam 1D inversion."""
 
     def __init__(self, parent=None):
@@ -1733,15 +1733,15 @@
         bool
             True if successful, False otherwise.
 
         """
         if 'MT - EDI' in self.indata:
             self.data = copy.deepcopy(self.indata['MT - EDI'])
         else:
-            self.showprocesslog('No EDI data')
+            self.showlog('No EDI data')
             return False
 
         self.combobox1.currentIndexChanged.disconnect()
         self.combobox1.clear()
 
         for i in self.data:
             self.combobox1.addItem(i)
```

### Comparing `pygmi-3.2.6.5/pygmi/mt/graphs.py` & `pygmi-3.2.7.16/pygmi/mt/graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from PyQt5 import QtWidgets, QtCore
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qt5 import NavigationToolbar2QT
 
 from pygmi.misc import ContextModule
 
+
 class GraphWindow(ContextModule):
     """Graph Window - Main QT Dialog class for graphs."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         self.setAttribute(QtCore.Qt.WA_DeleteOnClose)
@@ -72,15 +73,15 @@
     """
     MPL Canvas class.
 
     This routine will also allow the picking and movement of nodes of data.
     """
 
     def __init__(self, parent=None):
-        fig = Figure()
+        fig = Figure(layout='constrained')
         self.axes = fig.add_subplot(111)
         self.line = None
         self.ind = None
         self.background = None
 
         super().__init__(fig)
 
@@ -271,15 +272,15 @@
         ax4.set_xlabel('Period (s)')
         ax4.set_ylabel(r'Tipper Angle (Degrees)')
         ax4.grid(True)
 
         self.figure.canvas.draw()
         self.background = self.figure.canvas.copy_from_bbox(ax1.bbox)
 
-        self.figure.tight_layout()
+        # self.figure.tight_layout()
         self.figure.canvas.draw()
 
 
 class PlotPoints(GraphWindow):
     """Plot points class."""
 
     def __init__(self, parent=None):
```

### Comparing `pygmi-3.2.6.5/pygmi/mt/iodefs.py` & `pygmi-3.2.7.16/pygmi/mt/iodefs.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,110 +24,20 @@
 # -----------------------------------------------------------------------------
 """Import and export EDI data."""
 
 import os
 from PyQt5 import QtWidgets
 import mtpy.core.mt
 import numpy as np
-import pandas as pd
 
 from pygmi.misc import ContextModule, BasicModule
 
-
-class ImportLEMI417Data(BasicModule):
-    """
-    Import LEMI-417 ASCII MT Data.
-
-    This is a class used to import LEMI-417 MT Data in ASCII format.
-    """
-
-    def __init__(self, parent=None):
-        super().__init__(parent)
-
-    def settings(self, nodialog=False):
-        """
-        Entry point into item.
-
-        Parameters
-        ----------
-        nodialog : bool, optional
-            Run settings without a dialog. The default is False.
-
-        Returns
-        -------
-        bool
-            True if successful, False otherwise.
-
-        """
-        if not nodialog:
-
-            ext = 'LEMI-417 Text DataAll Files (*.t*)'
-
-            self.ifile, _ = QtWidgets.QFileDialog.getOpenFileName(
-                self.parent, 'Open File', '.', ext)
-            if self.ifile == '':
-                return False
-        os.chdir(os.path.dirname(self.ifile))
-
-        dataid = ['Year', 'Month', 'Day', 'Hour', 'Minute', 'Second',
-                  'Bx (nT)', 'By (nT)', 'Bz (nT)', 'TE (degrees C)',
-                  'TF (degrees C)', 'E1 ('+chr(956)+'V/m)',
-                  'E2 ('+chr(956)+'V/m)', 'E3 ('+chr(956)+'V/m)',
-                  'E4 ('+chr(956)+'V/m)']
-
-        gdf = pd.read_csv(self.ifile, sep=None, engine='python', names=dataid,
-                          skipinitialspace=True, index_col=False)
-
-        gdf['pygmiX'] = np.nan
-        gdf['pygmiY'] = np.nan
-        gdf['line'] = 'None'
-
-        if 'Line' not in self.outdata:
-            self.outdata['Line'] = {}
-
-        self.outdata['Line'][self.ifile] = gdf
-
-        return True
-
-    def loadproj(self, projdata):
-        """
-        Load project data into class.
-
-        Parameters
-        ----------
-        projdata : dictionary
-            Project data loaded from JSON project file.
-
-        Returns
-        -------
-        chk : bool
-            A check to see if settings was successfully run.
-
-        """
-        self.ifile = projdata['ifile']
-
-        chk = self.settings(True)
-
-        return chk
-
-    def saveproj(self):
-        """
-        Save project data from class.
-
-        Returns
-        -------
-        projdata : dictionary
-            Project data to be saved to JSON project file.
-
-        """
-        projdata = {}
-
-        projdata['ifile'] = self.ifile
-
-        return projdata
+# The lines below are a temporary fix for mtpy. Removed in future.
+np.float = float
+np.complex = complex
 
 
 class ImportEDI(BasicModule):
     """
     Import Data.
 
     Attributes
@@ -272,15 +182,15 @@
 
         """
         self.parent.process_is_active(True)
 
         if 'MT - EDI' in self.indata:
             data = self.indata['MT - EDI']
         else:
-            self.showprocesslog('No EDI data')
+            self.showlog('No EDI data')
             self.parent.process_is_active(False)
             return False
 
         ext = 'EDI (*.edi)'
 
         self.ofile, _ = QtWidgets.QFileDialog.getSaveFileName(
             self.parent, 'Save File', '.', ext)
@@ -288,21 +198,21 @@
         if self.ofile == '':
             self.parent.process_is_active(False)
             return False
         os.chdir(os.path.dirname(self.ofile))
 
         ext = self.ofile[-3:]
 
-        self.showprocesslog('Export Data Busy...')
+        self.showlog('Export Data Busy...')
 
         # Pop up save dialog box
         if ext == 'edi':
             self.export_edi(data)
 
-        self.showprocesslog('Export EDI Finished!')
+        self.showlog('Export EDI Finished!')
         self.parent.process_is_active(False)
         return True
 
     def export_edi(self, dat):
         """
         Export to EDI format.
```

### Comparing `pygmi-3.2.6.5/pygmi/mt/menu.py` & `pygmi-3.2.7.16/pygmi/seis/menu.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -----------------------------------------------------------------------------
 # Name:        menu.py (part of PyGMI)
 #
 # Author:      Patrick Cole
 # E-Mail:      pcole@geoscience.org.za
 #
-# Copyright:   (c) 2019 Council for Geoscience
+# Copyright:   (c) 2013 Council for Geoscience
 # Licence:     GPL-3.0
 #
 # This file is part of PyGMI
 #
 # PyGMI is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -18,134 +18,138 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
-"""EM Menu Routines."""
+"""Seis Menu Routines."""
 
 from PyQt5 import QtWidgets
 
-from pygmi.mt import iodefs
-from pygmi.mt import dataprep
-from pygmi.mt import graphs
-from pygmi.mt import birrp
+from pygmi.seis import del_rec
+from pygmi.seis import iodefs
+from pygmi.seis import beachball
+from pygmi.seis import graphs
+from pygmi.seis import utils
 
 
 class MenuWidget():
     """
     Widget class to call the main interface.
 
-    This widget class creates menus to be found on the main
+    This widget class creates the seismology menus to be found on the main
     interface. Normal as well as context menus are defined here.
 
     Attributes
     ----------
     parent : pygmi.main.MainWidget
         Reference to MainWidget class found in main.py
     """
 
     def __init__(self, parent=None):
 
         self.parent = parent
-        self.parent.add_to_context('MT - EDI')
+        self.parent.add_to_context('Seis')
         context_menu = self.parent.context_menu
 
-        # Normal menus
-        self.menumt = QtWidgets.QMenu('MT')
-        parent.menubar.addAction(self.menumt.menuAction())
-
-        self.action_birrp = QtWidgets.QAction('BIRRP - Beta')
-        self.menumt.addAction(self.action_birrp)
-        self.action_birrp.triggered.connect(self.birrp)
-
-        self.menumt.addSeparator()
-
-        self.action_import_data = QtWidgets.QAction('Import EDI Data')
-        self.menumt.addAction(self.action_import_data)
-        self.action_import_data.triggered.connect(self.import_data)
-
-        self.action_import_lemi417_data = QtWidgets.QAction('Import LEMI-417 '
-                                                            'Data to Point '
-                                                            'Data')
-        self.menumt.addAction(self.action_import_lemi417_data)
-        self.action_import_lemi417_data.triggered.connect(
-            self.import_lemi417_data)
-
-        self.menumt.addSeparator()
-
-        self.action_rotate_data = QtWidgets.QAction('Rotate EDI Data')
-        self.menumt.addAction(self.action_rotate_data)
-        self.action_rotate_data.triggered.connect(self.rotate_data)
-
-        self.action_sshift_data = QtWidgets.QAction('Remove Static Shift')
-        self.menumt.addAction(self.action_sshift_data)
-        self.action_sshift_data.triggered.connect(self.sshift_data)
-
-        self.action_mi_data = QtWidgets.QAction('Mask and Interpolate')
-        self.menumt.addAction(self.action_mi_data)
-        self.action_mi_data.triggered.connect(self.mi_data)
-
-        self.menumt.addSeparator()
-
-        self.action_occam1d = QtWidgets.QAction('Occam 1D Inversion')
-        self.menumt.addAction(self.action_occam1d)
-        self.action_occam1d.triggered.connect(self.occam1d)
+        self.menu = QtWidgets.QMenu('Seismology')
+        parent.menubar.addAction(self.menu.menuAction())
+
+        self.action_import_seisan = QtWidgets.QAction('Import SEISAN Data')
+        self.menu.addAction(self.action_import_seisan)
+        self.action_import_seisan.triggered.connect(self.import_seisan)
+
+        self.action_import_genfps = QtWidgets.QAction('Import Generic FPS')
+        self.menu.addAction(self.action_import_genfps)
+        self.action_import_genfps.triggered.connect(self.import_genfps)
+
+        self.menu.addSeparator()
+
+        self.action_check_desc = QtWidgets.QAction('Correct SEISAN Type 3'
+                                                   ' Descriptions')
+        self.menu.addAction(self.action_check_desc)
+        self.action_check_desc.triggered.connect(self.correct_desc)
+
+        self.action_filter_seisan = QtWidgets.QAction('Filter SEISAN Data')
+        self.menu.addAction(self.action_filter_seisan)
+        self.action_filter_seisan.triggered.connect(self.filter_seisan)
+
+        self.menu.addSeparator()
+
+        self.action_beachball = QtWidgets.QAction('Fault Plane Solutions')
+        self.menu.addAction(self.action_beachball)
+        self.action_beachball.triggered.connect(self.beachball)
+
+        self.action_quarry = QtWidgets.QAction('Remove Quarry Events')
+        self.menu.addAction(self.action_quarry)
+        self.action_quarry.triggered.connect(self.quarry)
 
         # Context menus
-        context_menu['MT - EDI'].addSeparator()
 
-        self.action_metadata = QtWidgets.QAction('Display/Edit Metadata')
-        context_menu['MT - EDI'].addAction(self.action_metadata)
-        self.action_metadata.triggered.connect(self.metadata)
-
-        self.action_show_graphs = QtWidgets.QAction('Show Graphs')
-        context_menu['MT - EDI'].addAction(self.action_show_graphs)
-        self.action_show_graphs.triggered.connect(self.show_graphs)
-
-        self.action_export_data = QtWidgets.QAction('Export EDI')
-        context_menu['MT - EDI'].addAction(self.action_export_data)
-        self.action_export_data.triggered.connect(self.export_data)
-
-    def birrp(self):
-        """BIRRP."""
-        self.parent.item_insert('Step', 'BIRRP', birrp.BIRRP)
-
-    def export_data(self):
-        """Export data."""
-        self.parent.launch_context_item(iodefs.ExportEDI)
-
-    def import_data(self):
-        """Import data."""
-        self.parent.item_insert('Io', 'Import EDI Data', iodefs.ImportEDI)
-
-    def import_lemi417_data(self):
-        """Import LEMI-417 MT data."""
-        self.parent.item_insert('Io', 'Import LEMI-417 Data',
-                                iodefs.ImportLEMI417Data)
-
-    def occam1d(self):
-        """Occam 1D inversion."""
-        self.parent.item_insert('Step', 'Occam 1D Inversion', dataprep.Occam1D)
-
-    def rotate_data(self):
-        """Rotate data."""
-        self.parent.item_insert('Step', 'Rotate EDI Data', dataprep.RotateEDI)
-
-    def sshift_data(self):
-        """Calculate Static Shift."""
-        self.parent.item_insert('Step', 'Static Shift EDI Data',
-                                dataprep.StaticShiftEDI)
-
-    def mi_data(self):
-        """Mask and interpolate data."""
-        self.parent.item_insert('Step', 'Mask and Interpolate EDI Data',
-                                dataprep.EditEDI)
-
-    def metadata(self):
-        """Metadata."""
-        self.parent.launch_context_item(dataprep.Metadata)
-
-    def show_graphs(self):
-        """Show graphs."""
-        self.parent.launch_context_item(graphs.PlotPoints)
+        context_menu['Seis'].addSeparator()
+
+        self.action_show_QC_plots = QtWidgets.QAction('Show QC Plots')
+        context_menu['Seis'].addAction(self.action_show_QC_plots)
+        self.action_show_QC_plots.triggered.connect(self.show_QC_plots)
+
+        self.action_export_seisan = QtWidgets.QAction('Export SEISAN Data')
+        context_menu['Seis'].addAction(self.action_export_seisan)
+        self.action_export_seisan.triggered.connect(self.export_seisan)
+
+        self.action_export_csv = QtWidgets.QAction('Export to CSV')
+        context_menu['Seis'].addAction(self.action_export_csv)
+        self.action_export_csv.triggered.connect(self.export_csv)
+
+        self.action_sexport = QtWidgets.QAction('Export Summary to CSV, XLSX '
+                                                'or SHP')
+        context_menu['Seis'].addAction(self.action_sexport)
+        self.action_sexport.triggered.connect(self.sexport)
+
+    def export_seisan(self):
+        """Export Seisan data."""
+        self.parent.launch_context_item(iodefs.ExportSeisan)
+
+    def export_csv(self):
+        """Export Seisan data to csv."""
+        self.parent.launch_context_item(iodefs.ExportCSV)
+
+    def sexport(self):
+        """Export Summary data."""
+        self.parent.launch_context_item(iodefs.ExportSummary)
+
+    def beachball(self):
+        """Create Beachballs from Fault Plane Solutions."""
+        self.parent.item_insert('Step', 'Fault Plane Solutions',
+                                beachball.BeachBall)
+
+    def import_seisan(self):
+        """Import Seisan."""
+        self.parent.item_insert('Io', 'Import SEISAN Data',
+                                iodefs.ImportSeisan)
+
+    def correct_desc(self):
+        """Correct Seisan descriptions."""
+        self.parent.item_insert('Step', 'Correct SEISAN Descriptions',
+                                utils.CorrectDescriptions)
+
+    def filter_seisan(self):
+        """Filter Seisan."""
+        self.parent.item_insert('Step', 'Filter SEISAN Data',
+                                iodefs.FilterSeisan)
+
+    def import_genfps(self):
+        """Import Generic Fault Plane Solution."""
+        self.parent.item_insert('Io', 'Import Generic FPS',
+                                iodefs.ImportGenericFPS)
+
+    def delete_recs(self):
+        """Delete Records."""
+        self.parent.item_insert('Step', 'Delete Records', del_rec.DeleteRecord)
+
+    def quarry(self):
+        """Remove quarry events."""
+        self.parent.item_insert('Step', 'Remove Quarry Events', del_rec.Quarry)
+
+    def show_QC_plots(self):
+        """Show QC plots."""
+        self.parent.launch_context_item(graphs.PlotQC)
```

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/DirectionDial.png` & `pygmi-3.2.7.16/pygmi/pfmod/DirectionDial.png`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/datatypes.py` & `pygmi-3.2.7.16/pygmi/pfmod/datatypes.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/grvmag3d.py` & `pygmi-3.2.7.16/pygmi/pfmod/grvmag3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -880,16 +880,15 @@
 
     """
     data = lmod.griddata[rtxt]
     data2 = lmod.griddata[ctxt]
 
     rows2, cols2 = data2.data.shape
 
-    dat = data_reproject(data, data.crs, data2.crs, data2.transform,
-                         rows2, cols2)
+    dat = data_reproject(data, data2.crs, data2.transform, rows2, cols2)
 
     return dat.data
 
 
 def calc_field(lmod, pbars=None, showtext=None, parent=None,
                showreports=False, magcalc=False, demag=False):
     """
@@ -924,15 +923,15 @@
         piter = pbars.iter
     else:
         piter = iter
     if np.max(lmod.lith_index) == -1:
         showtext('Error: Create a model first')
         return None
 
-    ttt = PTime()
+    ptime = PTime()
     # Init some variables for convenience
     lmod.update_lithlist()
 
     numx = int(lmod.numx)
     numy = int(lmod.numy)
     numz = int(lmod.numz)
 
@@ -1100,15 +1099,15 @@
     if parent is not None:
         tmp = list(set(lmod.griddata.values()))
         parent.outdata['Raster'] = tmp
     showtext('Calculation Finished')
     if pbars is not None:
         pbars.maxall()
 
-    tdiff = ttt.since_last_call(show=False)
+    tdiff = ptime.since_last_call(show=False)
     mins = int(tdiff/60)
     secs = tdiff-mins*60
 
     if magcalc:
         lmod.lith_index_mag_old = np.copy(lmod.lith_index)
     else:
         lmod.lith_index_grv_old = np.copy(lmod.lith_index)
```

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/iodefs.py` & `pygmi-3.2.7.16/pygmi/pfmod/iodefs.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,33 +22,33 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 """Import Data."""
 
 import sys
 import os
-import re
 import zipfile
 from PyQt5 import QtWidgets, QtCore
 import numpy as np
-from osgeo import ogr
 import matplotlib.pyplot as plt
 import pandas as pd
+import geopandas as gpd
 from rasterio.crs import CRS
+from shapely.geometry import Polygon
 
 from pygmi.pfmod.datatypes import LithModel
 from pygmi.pfmod import grvmag3d
 from pygmi.pfmod import mvis3d
 from pygmi import menu_default
 import pygmi.raster.dataprep as dp
 from pygmi.misc import BasicModule, ContextModule
+from pygmi.vector.dataprep import reprojxy
 # This is necessary for loading npz files, since I moved the location of
 # datatypes.
 from pygmi.pfmod import datatypes
-from pygmi.vector.dataprep import reprojxy
 
 sys.modules['datatypes'] = datatypes
 
 
 class ImportMod3D(BasicModule):
     """Import Data."""
 
@@ -275,15 +275,15 @@
         names = ['x', 'y', 'z', 'label']
         try:
             if filename.find('.csv') > -1:
                 df1 = pd.read_csv(filename, sep=',', names=names)
             else:
                 df1 = pd.read_csv(filename, sep=' ', names=names)
         except:
-            self.showprocesslog('Unable to import file')
+            self.showlog('Unable to import file')
             return
 
         x = df1.x.to_numpy(float)
         y = df1.y.to_numpy(float)
         z = df1.z.to_numpy(float)
         label = df1.label.to_numpy(str)
 
@@ -516,39 +516,41 @@
 
         Returns
         -------
         None.
 
         """
         if 'Model3D' not in self.indata:
-            self.showprocesslog('Error: You need to have a model first!')
+            self.showlog('Error: You need to have a model first!')
             return
 
         for self.lmod in self.indata['Model3D']:
             self.ofile, _ = QtWidgets.QFileDialog.getSaveFileName(
                 self.parent, 'Save File', '.',
                 'npz (*.npz);;shapefile (*.shp);;kmz (*.kmz);;csv (*.csv)')
 
             if self.ofile == '':
                 return
 
             os.chdir(os.path.dirname(self.ofile))
             ext = self.ofile[-3:]
 
-            self.showprocesslog('Saving '+self.ofile+'...')
+            self.parent.process_is_active()
+
+            self.showlog('Saving '+self.ofile+'...')
 
-        # Pop up save dialog box
             if ext == 'npz':
                 self.savemodel()
             if ext == 'kmz':
                 self.mod3dtokmz()
             if ext == 'shp':
                 self.mod3dtoshp()
             if ext == 'csv':
                 self.mod3dtocsv()
+            self.parent.process_is_active(False)
 
     def savemodel(self):
         """
         Save model.
 
         Returns
         -------
@@ -558,17 +560,17 @@
         # Construct output dictionary
         outdict = {}
         outdict = self.lmod2dict(outdict)
 
         # Save data
         try:
             np.savez_compressed(self.ofile, **outdict)
-            self.showprocesslog('Model save complete!')
+            self.showlog('Model save complete!')
         except:
-            self.showprocesslog('ERROR! Model save failed!')
+            self.showlog('ERROR! Model save failed!')
 
     def lmod2dict(self, outdict, pre=''):
         """
         Convert LithModel to a dictionary.
 
         Parameters
         ----------
@@ -641,15 +643,15 @@
         Save the 3D model in a csv file.
 
         Returns
         -------
         None.
 
         """
-        self.showprocesslog('csv export starting...')
+        self.showlog('csv export starting...')
 
         self.lmod.update_lith_list_reverse()
         lithname = self.lmod.lith_list_reverse.copy()
         lithlist = self.lmod.lith_list.copy()
 
         tmp = []
         ltmp = []
@@ -681,15 +683,15 @@
         stmp['lith'] = tmp[:, 5]
         stmp['lithname'] = ltmp
 
         head = 'X, Y, Z, Density, Susceptibility, Lithology Code, Lithology'
         np.savetxt(self.ofile, stmp, fmt="%f, %f, %f, %f, %f, %i, %s",
                    header=head)
 
-        self.showprocesslog('csv export complete!')
+        self.showlog('csv export complete!')
 
     def mod3dtokmz(self):
         """
         Save the 3D model and grids in a kmz file.
 
         Only the boundary of the area is in degrees. The actual coordinates
         are still in meters.
@@ -732,31 +734,31 @@
 
         lonwest, loneast = res[0]
         latsouth, latnorth = res[1]
 
         # Get Save Name
         filename = self.ofile
 
-        self.showprocesslog('kmz export starting...')
+        self.showlog('kmz export starting...')
 
         # Move to 3d model tab to update the model stuff
-        self.showprocesslog('updating 3d model...')
+        self.showlog('updating 3d model...')
 
         mvis_3d.spacing = [self.lmod.dxy, self.lmod.dxy, self.lmod.d_z]
         mvis_3d.origin = [xrng[0], yrng[0], zrng[0]]
         mvis_3d.gdata = self.lmod.lith_index[::1, ::1, ::-1]
         itmp = np.sort(np.unique(self.lmod.lith_index))
         itmp = itmp[itmp > 0]
         tmp = np.ones((255, 4))*255
         for i in itmp:
             tmp[i, :3] = self.lmod.mlut[i]
         mvis_3d.lut = tmp
         mvis_3d.update_model(smooth)
 
-        self.showprocesslog('creating kmz file')
+        self.showlog('creating kmz file')
         heading = str(0.)
         tilt = str(45.)  # angle from vertical
         lat = str(np.mean([latsouth, latnorth]))  # coord of object
         lon = str(np.mean([lonwest, loneast]))  # coord of object
         rng = str(max(xrng.ptp(), yrng.ptp(), zrng.ptp()))  # range to object
         alt = str(0)  # alt of object eye is looking at (meters)
         lato = str(latsouth)
@@ -812,16 +814,16 @@
                 points += [xrng.ptp(), yrng.ptp(), 0]
 
             norm = np.abs(mvis_3d.gnorms[lith])
             clrtmp = np.array(self.lmod.mlut[lith])/255.
             curmod = self.lmod.lith_list_reverse[lith]
 
             if len(points) > 60000:
-                self.showprocesslog(curmod + ' has too many points (' +
-                                    str(len(points))+'). Not exported')
+                self.showlog(curmod + ' has too many points (' +
+                             str(len(points))+'). Not exported')
                 points = points[:60000]
                 norm = norm[:60000]
                 faces = faces[faces.max(1) < 60000]
 
             lithcnt += 1
 
             dockml += (
@@ -1025,17 +1027,17 @@
             dockml += (
                 '  </Folder>\r\n'
                 '  \r\n'
                 '  </kml>')
 
             zfile.writestr('doc.kml', dockml)
 
-        self.showprocesslog('kmz export complete!')
+        self.showlog('kmz export complete!')
 
-    def mod3dtoshp(self):
+    def mod3dtoshp(self, nodialog=False):
         """
         Save the 3D model and grids in a shapefile file.
 
         Only the boundary of the area is in degrees. The actual coordinates
         are still in meters.
 
         Returns
@@ -1051,108 +1053,136 @@
         zrng = np.array(self.lmod.zrange, dtype=float)
 
         if 'Raster' in self.indata:
             wkt = self.indata['Raster'][0].crs.wkt
         else:
             wkt = ''
         prjkmz = Exportkmz(wkt)
-        tmp = prjkmz.exec_()
-
-        if tmp == 0:
-            return
+        prjkmz.checkbox_smooth.hide()
 
-        smooth = prjkmz.checkbox_smooth.isChecked()
+        if nodialog is False:
+            tmp = prjkmz.exec()
+            if tmp == 0:
+                return
 
-        self.showprocesslog('shapefile export starting...')
+        self.showlog('Shapefile export starting...')
 
         # Move to 3d model tab to update the model stuff
-        if smooth is True:
-            self.showprocesslog('updating and smoothing 3d model...')
-        else:
-            self.showprocesslog('updating 3d model...')
+        self.showlog('Updating 3d model...')
 
         mvis_3d.spacing = [self.lmod.dxy, self.lmod.dxy, self.lmod.d_z]
         mvis_3d.origin = [xrng[0], yrng[0], zrng[0]]
         mvis_3d.gdata = self.lmod.lith_index[::1, ::1, ::-1]
         itmp = np.sort(np.unique(self.lmod.lith_index))
         itmp = itmp[itmp > 0]
         tmp = np.ones((255, 4))*255
         for i in itmp:
             tmp[i, :3] = self.lmod.mlut[i]
         mvis_3d.lut = tmp
-        mvis_3d.update_model(smooth)
-
-        self.showprocesslog('creating shapefile file')
+        mvis_3d.update_model(False)
 
-        driver = ogr.GetDriverByName('ESRI Shapefile')
+        self.showlog('creating polygons')
 
         # update colours
         self.lmod.update_lith_list_reverse()
 
         mvis_3d.update_for_kmz()
 
         lkey = list(mvis_3d.faces.keys())
         lkey.pop(lkey.index(0))
 
-        for lith in lkey:
+        gdf = {}
+        for lith in self.piter(lkey):
             lithtext = mvis_3d.lmod1.lith_list_reverse[lith]
             lithsusc = self.lmod.lith_list[lithtext].susc
             lithdens = self.lmod.lith_list[lithtext].density
-            self.showprocesslog(' '+lithtext)
+
+            self.showlog(' '+lithtext)
+            QtWidgets.QApplication.processEvents()
 
             faces = np.array(mvis_3d.gfaces[lith])
 
             if faces.size == 0:
                 continue
 
-            ifile = self.ofile[:-4]+'_'+re.sub(r'[^A-Za-z]+', '_',
-                                               lithtext)+'.shp'
-            datasource = driver.CreateDataSource(ifile)
-            layer = datasource.CreateLayer('Model',
-                                           geom_type=ogr.wkbMultiPolygon25D)
-
-            layer.CreateField(ogr.FieldDefn('Lithology', ogr.OFTString))
-            layer.CreateField(ogr.FieldDefn('Susc', ogr.OFTReal))
-            layer.CreateField(ogr.FieldDefn('Density', ogr.OFTReal))
+            xfaces = []
+            yfaces = []
+            zfaces = []
+            badfaces = 0
+            for f in faces:
+                tmp = mvis_3d.gpoints[lith][f]
+                if np.unique(tmp[:, 0]).size == 1:
+                    xfaces.append(tmp)
+                elif np.unique(tmp[:, 1]).size == 1:
+                    yfaces.append(tmp)
+                elif np.unique(tmp[:, 2]).size == 1:
+                    zfaces.append(tmp)
+                else:
+                    badfaces += 1
 
-            points = mvis_3d.gpoints[lith]
+            gdfxyz = {}
+            for ifaces, faces in enumerate([xfaces, yfaces, zfaces]):
+                layer = {'Lithology': [],
+                         'Susc': [],
+                         'Density': [],
+                         'const': [],
+                         'geometry': []}
+
+                for tmp1 in faces:
+                    layer['Lithology'].append(lithtext)
+                    layer['Susc'].append(lithsusc)
+                    layer['Density'].append(lithdens)
+                    layer['const'].append(tmp1[0, ifaces])
+
+                    tmp = np.roll(tmp1, -(ifaces+1), axis=1)
+
+                    pverts = []
+                    pverts.append([tmp[0, 0], tmp[0, 1], tmp[0, 2]])
+                    pverts.append([tmp[1, 0], tmp[1, 1], tmp[1, 2]])
+                    pverts.append([tmp[2, 0], tmp[2, 1], tmp[2, 2]])
+                    pverts.append([tmp[0, 0], tmp[0, 1], tmp[0, 2]])
+                    pverts = Polygon(pverts)
+                    layer['geometry'].append(pverts)
+
+                ofaces = gpd.GeoDataFrame(layer)
+                ofaces = ofaces.dissolve(by='const', as_index=False,
+                                         sort=False)
+
+                ofaces = ofaces.explode(ignore_index=True)
+                ofaces = ofaces.set_crs(prjkmz.proj.wkt)
+
+                filt = ofaces.geometry.is_empty
+                ofaces = ofaces[~filt]
+
+                if ifaces == 2:
+                    gdfxyz[ifaces] = ofaces
+                    continue
+
+                coords = ofaces.geometry.apply(lambda geom:
+                                               np.array(geom.exterior.coords))
+
+                geom = []
+                for i in coords:
+                    tmp = np.roll(i, ifaces+1, axis=1)
+                    pverts = Polygon(tmp)
+                    geom.append(pverts)
+                ofaces['geometry'] = geom
+                ofaces.pop('const')
+
+                gdfxyz[ifaces] = ofaces
+
+            gdf[lithtext] = pd.concat(gdfxyz, ignore_index=True)
 
-            for f in faces:
-                multipolygon = ogr.Geometry(ogr.wkbMultiPolygon25D)
-                tmp = points[f]
+        self.showlog('Combining all lithologies...')
+        gdf = pd.concat(gdf, ignore_index=True)
 
-                ring1 = ogr.Geometry(ogr.wkbLinearRing)
-                ring1.AddPoint(tmp[0, 0], tmp[0, 1], tmp[0, 2])
-                ring1.AddPoint(tmp[1, 0], tmp[1, 1], tmp[1, 2])
-                ring1.AddPoint(tmp[2, 0], tmp[2, 1], tmp[2, 2])
-                ring1.AddPoint(tmp[0, 0], tmp[0, 1], tmp[0, 2])
-
-                # Create polygon #1
-                poly1 = ogr.Geometry(ogr.wkbPolygon25D)
-                poly1.AddGeometry(ring1)
-                multipolygon.AddGeometry(poly1)
-
-                ring1 = None
-                poly1 = None
-
-                feature = ogr.Feature(layer.GetLayerDefn())
-                feature.SetGeometry(multipolygon)
-                feature.SetField('Lithology', lithtext)
-                feature.SetField('Susc', lithsusc)
-                feature.SetField('Density', lithdens)
-                layer.CreateFeature(feature)
-
-                multipolygon = None
-
-            # flush memory
-            layer = None
-            feature = None
-            datasource = None
+        self.showlog('Exporting to shapefile...')
+        gdf.to_file(self.ofile)
 
-        self.showprocesslog('shapefile export complete!')
+        self.showlog('Shapefile export complete!')
 
 
 class Exportkmz(QtWidgets.QDialog):
     """Export kmz dialog."""
 
     def __init__(self, wkt, parent=None):
         super().__init__(parent)
@@ -1253,29 +1283,27 @@
 
 
 def _testfn():
     """Test."""
     from IPython import get_ipython
     get_ipython().run_line_magic('matplotlib', 'inline')
 
-    print('Starting')
-
     ifile = r"d:\Workdata\modelling\small_upper.npz"
+    ifile = r"D:\Workdata\modelling\Magmodel_Upper22km_AveAll_diapir_withDeepDens_newdens.npz"
+    ofile = r"d:\Workdata\modelling\hope2.shp"
 
     app = QtWidgets.QApplication(sys.argv)
 
     DM = ImportMod3D()
     DM.ifile = ifile
     DM.settings(nodialog=True)
 
-    odata = DM.outdata['Raster']
-
-    for dat in odata:
-        plt.figure(dpi=150)
-        plt.title(dat.dataid)
-        plt.imshow(dat.data, extent=dat.extent)
-        plt.colorbar()
-        plt.show()
+    EM = ExportMod3D()
+    EM.indata = DM.outdata
+    EM.ofile = ofile
+    EM.lmod = EM.indata['Model3D'][0]
+    EM.mod3dtoshp(nodialog=False)
+    # EM.exec()
 
 
 if __name__ == "__main__":
     _testfn()
```

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/menu.py` & `pygmi-3.2.7.16/pygmi/pfmod/menu.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from PyQt5 import QtWidgets
 
 from pygmi.pfmod import pfmod
 from pygmi.pfmod import mvis3d
 from pygmi.pfmod import iodefs
 from pygmi.pfmod import misc
 from pygmi.pfmod import pfinvert
+from pygmi.pfmod import show_table
 
 
 class MenuWidget():
     """
     Widget class to call the main interface.
 
     This widget class creates the modelling menus to be found on the main
@@ -79,14 +80,18 @@
         # Context Menu
         context_menu['Model3D'].addSeparator()
 
         self.action_mod3d = QtWidgets.QAction('3D Model Display')
         context_menu['Model3D'].addAction(self.action_mod3d)
         self.action_mod3d.triggered.connect(self.mod3d)
 
+        self.action_stat3d = QtWidgets.QAction('3D Model Statisitics')
+        context_menu['Model3D'].addAction(self.action_stat3d)
+        self.action_stat3d.triggered.connect(self.stat3d)
+
         self.action_export_mod3d = QtWidgets.QAction('Export 3D Model')
         context_menu['Model3D'].addAction(self.action_export_mod3d)
         self.action_export_mod3d.triggered.connect(self.export_mod3d)
 
     def export_mod3d(self):
         """Export 3D Model."""
         self.parent.launch_context_item(iodefs.ExportMod3D)
@@ -101,14 +106,18 @@
         self.parent.item_insert('Step', '3D Magnetic Inversion',
                                 pfinvert.MagInvert)
 
     def mod3d(self):
         """3D display of data."""
         self.parent.launch_context_item(mvis3d.Mod3dDisplay)
 
+    def stat3d(self):
+        """3D display of data."""
+        self.parent.launch_context_item(show_table.BasicStats3D)
+
     def import_mod3d(self):
         """Import data."""
         self.parent.item_insert('Io', 'Import 3D Model', iodefs.ImportMod3D)
 
     def merge_mod3d(self):
         """Merge models."""
         self.parent.item_insert('Step', 'Merge 3D Models', misc.MergeMod3D)
```

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/misc.py` & `pygmi-3.2.7.16/pygmi/pfmod/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,15 @@
             True if successful, False otherwise.
 
         """
         tmp = []
         if 'Model3D' not in self.indata:
             return False
         if len(self.indata['Model3D']) != 2:
-            self.showprocesslog('You need two datasets connected!')
+            self.showlog('You need two datasets connected!')
             return False
 
         for i in self.indata['Model3D']:
             tmp.append(i.name)
 
         self.master.addItems(tmp)
         self.slave.addItems(tmp)
@@ -384,16 +384,16 @@
         Returns
         -------
         bool
             True if successful, False otherwise
 
         """
         if self.master.currentText() == self.slave.currentText():
-            self.showprocesslog('Your master dataset must be different'
-                                ' to the slave dataset!')
+            self.showlog('Your master dataset must be different'
+                         ' to the slave dataset!')
             return False
 
         for data in self.indata['Model3D']:
             if data.name == self.master.currentText():
                 datmaster = data
             if data.name == self.slave.currentText():
                 datslave = data
@@ -515,16 +515,15 @@
     cols = int((xmax - xmin)//xdim)+1
     rows = int((ymax - ymin)//ydim)+1
     otransform = rasterio.Affine(xdim, 0, xmin, 0, -1*ydim, ymax)
 
     dat = []
 
     for data in [master, slave]:
-        dat.append(data_reproject(data, data.crs, data.crs, otransform,
-                                  rows, cols))
+        dat.append(data_reproject(data, data.crs, otransform, rows, cols))
 
     imask = np.logical_and(dat[0].data.mask, np.logical_not(dat[1].data.mask))
     if imask.size > 1:
         dat[0].data.data[imask] = dat[1].data.data[imask]
         dat[0].data.mask[imask] = False
 
     return dat[0]
```

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/mvis3d.py` & `pygmi-3.2.7.16/pygmi/pfmod/mvis3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,29 +379,29 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Model3D' not in self.indata:
-            self.showprocesslog('No 3D model. You may need to execute that '
-                                'module first')
+            self.showlog('No 3D model. You may need to execute that '
+                         'module first')
             return False
 
         self.lmod1 = self.indata['Model3D'][0]
 
         liths = np.unique(self.lmod1.lith_index[::1, ::1, ::-1])
         liths = np.array(liths).astype(int)  # needed for use in faces array
         if liths[0] == -1:
             liths = liths[1:]
         if liths[0] == 0:
             liths = liths[1:]
         if liths.size == 0:
-            self.showprocesslog('No 3D model. You need to draw in at least '
-                                'part of a lithology first.')
+            self.showlog('No 3D model. You need to draw in at least '
+                         'part of a lithology first.')
             return False
 
         self.show()
 
         misc.update_lith_lw(self.lmod1, self.lw_3dmod_defs)
         for i in range(self.lw_3dmod_defs.count()-1, -1, -1):
             if self.lw_3dmod_defs.item(i).text() == 'Background':
@@ -617,15 +617,15 @@
 
 # shrink cc to match only visible lithology? Origin offset would need to be
 # checked.
 
                 c[1:-1, 1:-1, 1:-1] = cc
 
                 faces, vtx = MarchingCubes(xx, yy, zz, c, .1,
-                                           self.showprocesslog)
+                                           self.showlog)
 
                 if vtx.size == 0:
                     self.lmod1.update_lith_list_reverse()
 
                     self.faces[lno] = []
                     self.corners[lno] = []
                     self.norms[lno] = []
@@ -1377,15 +1377,15 @@
     lens[lens == 0] = 1  # Get rid of divide by zero.
 
     arr /= lens[:, np.newaxis]
 
     return arr
 
 
-def MarchingCubes(x, y, z, c, iso, showprocesslog=print):
+def MarchingCubes(x, y, z, c, iso, showlog=print):
     """
     Marching cubes.
 
     Use marching cubes algorithm to compute a triangulated mesh of the
     isosurface within the 3D matrix of scalar values C at isosurface value
     ISO. The 3D matrices (X,Y,Z) represent a Cartesian, axis-aligned grid
     specifying the points at which the data C is given. These coordinate
@@ -1413,15 +1413,15 @@
         Y coordinates.
     z : numpy array
         Z coordinates.
     c : numpy array
         Data.
     iso : float
         Isosurface level.
-    showprocesslog : function, optional
+    showlog : function, optional
         Routine to show text messages. The default is print.
 
     Returns
     -------
     F : numpy array
         Face list.
     V : numpy array
@@ -1463,16 +1463,16 @@
 
     # intersected edges for each cube ([n1 x n2 x n3] mtx)
     cedge = edgeTable[cc]
     # voxels which are intersected (col of indcs into cedge)
     iden = np.nonzero(cedge.flatten(order='F'))[0]
 
     if iden.size == 0:          # all voxels are above or below iso
-        showprocesslog('Warning: No such lithology, or all voxels are above '
-                       'or below iso')
+        showlog('Warning: No such lithology, or all voxels are above '
+                'or below iso')
         F = np.array([])
         V = np.array([])
         return F, V
 
     # calculate the list of intersection points
     xyz_off = np.array([[1, 1, 1],
                         [2, 1, 1],
@@ -1609,15 +1609,15 @@
         mu[nid] = (isolevel - valp1[nid]) / (valp2[nid] - valp1[nid])
         p[nid, 0] = p1x[nid] + mu[nid] * (p2x[nid] - p1x[nid])
         p[nid, 1] = p1y[nid] + mu[nid] * (p2y[nid] - p1y[nid])
         p[nid, 2] = p1z[nid] + mu[nid] * (p2z[nid] - p1z[nid])
     return p
 
 
-@jit
+@jit(nopython=True)
 def fancyindex(out, var1, ii, jj, kk):
     """
     Fancy index.
 
     Parameters
     ----------
     out : numpy array
```

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/pfinvert.py` & `pygmi-3.2.7.16/pygmi/pfmod/pfinvert.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 
 import sys
 from contextlib import redirect_stdout
 import numpy as np
 from PyQt5 import QtWidgets, QtCore
 import scipy.interpolate as si
 from discretize import TensorMesh
+from discretize.utils import active_from_xyz
 from SimPEG.potential_fields import magnetics
-from SimPEG.utils import surface2ind_topo,  model_builder
+from SimPEG.utils import model_builder
 from SimPEG import (maps, data, inverse_problem, data_misfit,
                     regularization, optimization, directives,
                     inversion)
 import sklearn.cluster as skc
 
 from pygmi import menu_default
 from pygmi.misc import BasicModule
@@ -277,15 +278,15 @@
         Apply changes.
 
         Returns
         -------
         None.
 
         """
-        self.showprocesslog('Working...')
+        self.showlog('Working...')
 
         self.choose_combo(self.combo_dtm, 'DTM Dataset')
         self.choose_combo(self.combo_mag, 'Magnetic Dataset')
         self.choose_combo(self.combo_dataset, 'Study Area Dataset')
 
         cols = self.sb_cols.value()
         rows = self.sb_rows.value()
@@ -301,15 +302,15 @@
 
         self.update_vals()
 
         # This line is to avoid duplicates since study area and dtm are often
         # the same dataset
         tmp = list(set(self.lmod1.griddata.values()))
         self.outdata['Raster'] = tmp
-        self.showprocesslog('Changes applied.')
+        self.showlog('Changes applied.')
 
         self.accept()
 
     def choose_combo(self, combo, dtxt):
         """
         Combo box choice routine.
 
@@ -699,16 +700,18 @@
         -------
         None.
 
         """
         dat = [self.lmod1.griddata['Magnetic Dataset'],
                self.lmod1.griddata['DTM Dataset']]
 
-        dat = lstack(dat, masterid=0, commonmask=True, piter=self.piter,
-                     pprint=self.showprocesslog)
+        masterid = self.lmod1.griddata['Magnetic Dataset'].dataid
+
+        dat = lstack(dat, masterid=masterid, commonmask=True,
+                     piter=self.piter, showlog=self.showlog)
 
         mag = dat[0]
         dtm = dat[1]
 
         dobs = mag.data.compressed()
 
         xmin, xmax, ymin, ymax = mag.extent
@@ -717,21 +720,14 @@
         ydim = mag.ydim
 
         rows, cols = mag.data.shape
 
         xxx = np.linspace(xmin, xmax, cols, False) + xdim/2
         yyy = np.linspace(ymin, ymax, rows, False) + ydim/2
 
-        # xxx = np.arange(xmin, xmax, xdim) + xdim/2
-        # yyy = np.arange(ymin, ymax, ydim) + ydim/2
-
-        # Get rid of the extra values due to round off error
-        # xxx = xxx[xxx < xmax]
-        # yyy = yyy[yyy < ymax]
-
         xy = np.meshgrid(xxx, yyy[::-1])
         z = dtm.data + self.dsb_mht.value()
 
         xxx = xy[0][~mag.data.mask]
         yyy = xy[1][~mag.data.mask]
         z = z.compressed()
 
@@ -749,17 +745,14 @@
                                                   components=components)
         receiver_list = [receiver_list]
 
         inclination = self.dsb_hinc.value()
         declination = self.dsb_hdec.value()
         strength = self.dsb_hint.value()
 
-        # inducing_field = (strength, inclination, declination)
-        # source_field = magnetics.sources.SourceField(
-        #     receiver_list=receiver_list, parameters=inducing_field)
         source_field = magnetics.UniformBackgroundField(
             receiver_list=receiver_list, amplitude=strength,
             inclination=inclination, declination=declination)
 
         # Define the survey, data and tensor mesh
         survey = magnetics.survey.Survey(source_field)
         data_object = data.Data(survey, dobs=dobs, standard_deviation=std)
@@ -772,42 +765,33 @@
 
         x0 = xmin-(np.sum([dhxy*1.3**(i+1) for i in range(5)])+5)
         y0 = ymin-(np.sum([dhxy*1.3**(i+1) for i in range(5)])+5)
         z0 = -(dh*self.lmod1.numz)-(np.sum([dh*1.3**(i+1) for i in range(5)]))
 
         mesh = TensorMesh([hx, hy, hz], [x0, y0, z0])
 
-        # hx = [(dhxy, self.lmod1.numx)]
-        # hy = [(dhxy, self.lmod1.numy)]
-        # hz = [(dh, self.lmod1.numz)]
-
-        # x0 = xmin-5
-        # y0 = ymin-5
-        # z0 = -dh*self.lmod1.numz
-
-        # mesh = TensorMesh([hx, hy, hz], [x0, y0, z0])
-        # mesh = TensorMesh([hx, hy, hz], "CCN")
-
         # Starting/Reference Model and Mapping on Tensor Mesh
         background_susceptibility = 1e-4
-        ind_active = surface2ind_topo(mesh, topo_xyz)
+
+        ind_active = active_from_xyz(mesh, topo_xyz)
         nC = int(ind_active.sum())
         model_map = maps.IdentityMap(nP=nC)
         starting_model = background_susceptibility * np.ones(nC)
 
         # Define the Physics
         simulation = magnetics.simulation.Simulation3DIntegral(
             survey=survey, mesh=mesh, model_type="scalar", chiMap=model_map,
             ind_active=ind_active)
 
         # Define Inverse Problem
         dmis = data_misfit.L2DataMisfit(data=data_object,
                                         simulation=simulation)
         reg = regularization.Sparse(mesh, active_cells=ind_active,
-                                    mapping=model_map, reference_model=starting_model,
+                                    mapping=model_map,
+                                    reference_model=starting_model,
                                     gradient_type="total")
         reg.norms = [0, 0, 0, 0]
 
         opt = optimization.ProjectedGNCG(maxIter=20, lower=0.0, upper=1.0,
                                          maxIterLS=20, maxIterCG=10,
                                          tolCG=1e-3)
         inv_prob = inverse_problem.BaseInvProblem(dmis, reg, opt)
@@ -818,31 +802,29 @@
         update_IRLS = directives.Update_IRLS(f_min_change=1e-4,
                                              max_irls_iterations=30,
                                              coolEpsFact=1.5, beta_tol=1e-2)
         update_jacobi = directives.UpdatePreconditioner()
 
         target_misfit = directives.TargetMisfit(chifact=1)
         sensitivity_weights = directives.UpdateSensitivityWeights(
-            everyIter=False)
+            every_iteration=False)
         directives_list = [sensitivity_weights, starting_beta, save_iteration,
                            update_IRLS, update_jacobi]
 
         # Running the Inversion
         inv = inversion.BaseInversion(inv_prob, directives_list)
 
         try:
             with redirect_stdout(self.stdout_redirect):
                 recovered_model = inv.run(starting_model)
         except Exception as e:
-            self.showprocesslog('Error: '+str(e))
+            self.showlog('Error: '+str(e))
             return False
 
         # Recreate True Model
-        # -------------------
-
         background_susceptibility = 0.0001
         sphere_susceptibility = 0.01
 
         true_model = background_susceptibility * np.ones(nC)
         ind_sphere = model_builder.getIndicesSphere(
             np.r_[0.0, 0.0, -45.0], 15.0, mesh.cell_centers
         )
@@ -858,37 +840,33 @@
                     mesh.shape_cells[1],
                     mesh.shape_cells[0])
         r2 = r2[::-1]
 
         r3 = r2[:-5, 5:-5, 5:-5]
         r3 = np.ma.masked_invalid(r3)
         r3 = np.ma.array(r3)
-        # X = skp.StandardScaler().fit_transform(r3.flatten())
 
         X = r3.compressed().reshape(-1, 1)
 
-        # cfit = skc.KMeans(n_clusters=i, tol=self.tol,
-        #                   max_iter=self.max_iter).fit(X)
         numclasses = self.sb_classes.value()
-        cfit = skc.KMeans(n_clusters=numclasses).fit(X)
+        cfit = skc.KMeans(n_clusters=numclasses, n_init='auto').fit(X)
 
         zout = cfit.labels_
         r3[~r3.mask] = zout
 
         r4 = np.moveaxis(r3, [0, 1, 2], [2, 1, 0])
         r4 = r4.filled(-1)
 
         cnt = cfit.labels_.max()+1
         susc = [0.]*cnt
         inputliths = ['']*cnt
         dens = [2.67]*cnt
         for i2 in range(cnt):
             susc[i2] = X[cfit.labels_ == i2].mean()
             inputliths[i2] = str(susc[i2])
-            # print(i2, susc[i2])
 
         bsusc = np.min(susc)
         bindx = np.nonzero(susc == bsusc)[0][0]
 
         if bindx != 0:
             r4[r4 == bindx] = 999
             r4[r4 == 0] = bindx
@@ -1029,29 +1007,14 @@
                                 vmax=np.max(recovered_model))
     cbar = mpl.colorbar.ColorbarBase(ax2, norm=norm, orientation="vertical",
                                      cmap=mpl.colormaps['viridis'],
                                      format="%.1e")
     cbar.set_label("SI", rotation=270, labelpad=15, size=12)
     plt.show()
 
-    # r2 = plotting_map * recovered_model
-    # r2.shape = (mesh.shape_cells[2], mesh.shape_cells[1], mesh.shape_cells[0])
-
-    # r2 = r2[::-1]
-    # r2 = r2[:-5]
-
-    # plt.imshow(r2[:, r2.shape[1]//2])
-    # plt.show()
-
-    # 3D Display
-    # tmp = Mod3dDisplay()
-    # tmp.indata = DM.outdata
-    # tmp.run()
-    # tmp.exec_()
-
     get_ipython().run_line_magic('matplotlib', 'Qt5')
 
     tmp = MainWidget()
     tmp.indata = DM.outdata
     tmp.settings()
 
 
@@ -1062,29 +1025,17 @@
     from pygmi.raster.iodefs import get_raster
     from pygmi.pfmod.pfmod import MainWidget
     from IPython import get_ipython
     get_ipython().run_line_magic('matplotlib', 'inline')
 
     app = QtWidgets.QApplication(sys.argv)
 
-    # mfile = r"d:\Workdata\MagInv\pcmag.tif"
-
-    # mdat = get_raster(mfile)
-    # ddat = copy.deepcopy(mdat)
-    # ddat[0].data = ddat[0].data * 0.
-
     mfile = r"D:\Workdata\PyGMI Test Data\Potential Field Modelling\MagInv\pcmagdem.tif"
     dfile = r"D:\Workdata\PyGMI Test Data\Potential Field Modelling\MagInv\pcdem.tif"
 
-    # mfile = r"c:\Workdata\PyGMI Test Data\Test_Mar2022\Data\Testing\mag_igrfremoved.tif"
-    # dfile = r"c:\Workdata\PyGMI Test Data\Test_Mar2022\Data\ER Mapper\dtmmicrolevel.PD.ers"
-
-    # mfile = r"c:\Workdata\PyGMI Test Data\Test_Mar2022\Data\VIS_ModelArea_TMA_utm35s.tif"
-    # dfile = r"c:\Workdata\PyGMI Test Data\Test_Mar2022\Data\VIS_ModelArea_SRTM90m_utm35s.tif"
-
     mdat = get_raster(mfile)
     ddat = get_raster(dfile)
 
     mdat[0].dataid = 'mag'
     ddat[0].dataid = 'dem'
 
     DM = MagInvert()
@@ -1121,18 +1072,14 @@
     DM.combo_dtm.setCurrentText('dem')
     DM.combo_mag.setCurrentText('mag')
     DM.combo_dataset.setCurrentText('mag')
 
     DM.choose_dtm()
 
     DM.dsb_mht.setValue(mht)
-    # DM.dsb_hdec.setValue(0)
-    # DM.dsb_hint.setValue(50000)
-    # DM.dsb_hinc.setValue(90)
-
     DM.settings(True)
 
     maps1, mesh, ind_active, recovered_model, true_model = DM.tmp
 
     # Plot True Model
     fig = plt.figure(figsize=(9, 4), dpi=150)
     plotting_map = maps1.InjectActiveCells(mesh, ind_active, np.nan)
```

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/pfmod.py` & `pygmi-3.2.7.16/pygmi/pfmod/pfmod.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 """The main program for the modelling package."""
 
-import sys
 from PyQt5 import QtWidgets, QtCore
 
 from pygmi.pfmod import misc
 from pygmi.pfmod import tab_prof
 from pygmi.pfmod import tab_param
 from pygmi.pfmod import tab_mext
 from pygmi.pfmod import grvmag3d
@@ -41,17 +40,17 @@
 class MainWidget(QtWidgets.QMainWindow):
     """MainWidget - Widget class to call the main interface."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         if parent is None:
-            self.showprocesslog = print
+            self.showlog = print
         else:
-            self.showprocesslog = parent.showprocesslog
+            self.showlog = parent.showlog
 
         self.indata = {'tmp': True}
         self.inraster = {}
         self.outdata = {}
         self.parent = parent
         self.lmod1 = LithModel()  # actual model
 
@@ -141,15 +140,15 @@
 
         Returns
         -------
         None.
 
         """
         self.showtext('Saving model, please do not close the interface...')
-        tmp = iodefs.ExportMod3D(self)
+        tmp = iodefs.ExportMod3D(self.parent)
         tmp.indata = self.outdata
         tmp.run()
 
         del tmp
         self.showtext('Model save complete!')
 
     def help_docs(self):
```

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/tab_mext.py` & `pygmi-3.2.7.16/pygmi/pfmod/tab_mext.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/tab_param.py` & `pygmi-3.2.7.16/pygmi/pfmod/tab_param.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/pfmod/tab_prof.py` & `pygmi-3.2.7.16/pygmi/pfmod/tab_prof.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,36 +31,36 @@
 import numpy as np
 from scipy import ndimage
 from scipy import interpolate
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.backends.backend_qt5 import NavigationToolbar2QT
 from matplotlib.figure import Figure
 from matplotlib import colormaps
-from osgeo import osr
 import pandas as pd
 import pygmi.raster.iodefs as ir
 
 from pygmi.pfmod import grvmag3d
 from pygmi.pfmod import misc
 from pygmi import menu_default
 from pygmi.raster.dataprep import data_reproject
 from pygmi.raster.iodefs import get_raster
 from pygmi.misc import frm, BasicModule
+from pygmi.vector.dataprep import reprojxy
 
 
 class ProfileDisplay(QtWidgets.QWidget):
     """Widget class to call the main interface."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         if parent is None:
-            self.showprocesslog = print
+            self.showlog = print
         else:
-            self.showprocesslog = parent.showprocesslog
+            self.showlog = parent.showlog
 
         self.parent = parent
         self.lmod1 = parent.lmod1
         self.showtext = parent.showtext
         self.pbar = self.parent.pbar_sub
         self.viewmagnetics = True
         self.plot_custmin = 0.
@@ -471,55 +471,46 @@
         None.
 
         """
         lmod = self.lmod1
         if 'Borehole' not in self.parent.indata:
             return
 
-        if self.parent.indata['Raster'][0].crs.wkt == '':
+        if self.parent.indata['Raster'][0].crs is None:
             return
 
         data = self.parent.indata['Borehole']
 
-        orig = osr.SpatialReference()
-        orig.ImportFromEPSG(4326)  # WGS84 degrees
-        orig.SetAxisMappingStrategy(osr.OAMS_TRADITIONAL_GIS_ORDER)
-
-        targ = osr.SpatialReference()
-        targ.ImportFromWkt(self.parent.indata['Raster'][0].crs.wkt)
-        targ.SetAxisMappingStrategy(osr.OAMS_TRADITIONAL_GIS_ORDER)
-
-        prj = osr.CoordinateTransformation(orig, targ)
-
         for bnum in data:
             hdr = data[bnum]['header']
             log = data[bnum]['log']
             try:
                 lat = float(hdr['Declat'])
                 lon = float(hdr['Declon'])
                 elev = float(hdr['Elevation'])
             except TypeError:
                 continue
-            res = prj.TransformPoint(lon, lat)
-            x, y = res[0], res[1]
+
+            x, y = reprojxy(lon, lat, 4326,
+                            self.parent.indata['Raster'][0].crs.wkt)
 
             if x < self.lmod1.xrange[0] or x > self.lmod1.xrange[1]:
                 continue
             if y < self.lmod1.yrange[0] or y > self.lmod1.yrange[1]:
                 continue
             dfrom = elev - np.abs(log['Depth from'].values)
             dto = elev - np.abs(log['Depth to'].values)
             lith = log.Lithology.values
 
             xind = int((x-self.lmod1.xrange[0])//self.lmod1.dxy)
             yind = int((y-self.lmod1.yrange[0])//self.lmod1.dxy)
             ifrom = []
             ito = []
-            for i, _ in enumerate(dfrom):
-                z1 = int((self.lmod1.zrange[1]-dfrom[i])//self.lmod1.d_z)
+            for i, dfromi in enumerate(dfrom):
+                z1 = int((self.lmod1.zrange[1]-dfromi)//self.lmod1.d_z)
                 z2 = int((self.lmod1.zrange[1]-dto[i])//self.lmod1.d_z)
                 ifrom.append(z1)
                 ito.append(z2)
             # Now do the bit which creates combos of liths per pixel.
 
             lithfin = {}
             for i, _ in enumerate(ifrom):
@@ -619,15 +610,15 @@
             for i in self.lmod1.griddata:
                 if i in ('Study Area Dataset', 'Gravity Residual',
                          'Magnetic Residual'):
                     continue
 
                 data1 = copy.deepcopy(self.lmod1.griddata[i])
                 if data1.isrgb is True:
-                    # self.showprocesslog(f'Skipping RGB image {data1.dataid}')
+                    # self.showlog(f'Skipping RGB image {data1.dataid}')
                     continue
                 if 'Calculated Gravity' in i:
                     data1.data = data1.data + self.lmod1.gregional
 
                 dtlx = data.extent[0]
                 d2tlx = data1.extent[0]
                 # dtly = data.extent[-1]
@@ -911,21 +902,21 @@
         None.
 
         """
         x1, x2 = self.lmod1.custprofx['adhoc']
         y1, y2 = self.lmod1.custprofy['adhoc']
         px1, px2 = self.lmod1.custprofx['rotate']
 
-        if not(self.lmod1.xrange[0] <= x1 <= self.lmod1.xrange[1]):
+        if not (self.lmod1.xrange[0] <= x1 <= self.lmod1.xrange[1]):
             return False
-        if not(self.lmod1.xrange[0] <= x2 <= self.lmod1.xrange[1]):
+        if not (self.lmod1.xrange[0] <= x2 <= self.lmod1.xrange[1]):
             return False
-        if not(self.lmod1.yrange[0] <= y1 <= self.lmod1.yrange[1]):
+        if not (self.lmod1.yrange[0] <= y1 <= self.lmod1.yrange[1]):
             return False
-        if not(self.lmod1.yrange[0] <= y2 <= self.lmod1.yrange[1]):
+        if not (self.lmod1.yrange[0] <= y2 <= self.lmod1.yrange[1]):
             return False
 
         # convert units to cells
         bly = self.lmod1.yrange[0]
         tlx = self.lmod1.xrange[0]
         dxy = self.lmod1.dxy
 
@@ -1424,15 +1415,15 @@
             d2tlx = data2.extent[0]
             dbly = data.extent[-2]
             d2bly = data2.extent[-2]
 
             rxxx2 = (dtlx-d2tlx+self.rxxx*data.xdim)/data2.xdim+1
             ryyy2 = (dbly-d2bly+self.ryyy*data.ydim)/data2.ydim+1
 
-            pdtmp = data2.data.filled(np.nan)
+            pdtmp = data2.data.astype(float).filled(np.nan)
             tmprng2 = np.linspace(px1, px2, len(rxxx2))
             tmpprof2 = ndimage.map_coordinates(pdtmp[::-1],
                                                [ryyy2-0.5, rxxx2-0.5],
                                                order=1, cval=np.nan)
 
             tmprng2 = tmprng2[np.logical_not(np.isnan(tmpprof2))]
             tmpprof2 = tmpprof2[np.logical_not(np.isnan(tmpprof2))]
@@ -1517,15 +1508,15 @@
         self.combo_overview.currentIndexChanged.connect(self.pic_overview)
 
 
 class MyMplCanvas(FigureCanvasQTAgg):
     """Matplotlib Canvas."""
 
     def __init__(self, parent=None):
-        fig = Figure()
+        fig = Figure(layout='tight')
         super().__init__(fig)
 
         self.lmod1 = parent.lmod1
         self.cbar = colormaps['jet']
         self.curmodel = 0
         self.mywidth = 1
         self.xold = None
@@ -1700,16 +1691,16 @@
             else:
 
                 rrr = np.sqrt((self.xold-xdata)**2+(self.yold-ydata)**2)
                 steps = int(rrr)+1
                 xxx = np.linspace(self.xold, xdata, steps)
                 yyy = np.linspace(self.yold, ydata, steps)
 
-                for i, _ in enumerate(xxx):
-                    self.set_mdata(xxx[i], yyy[i], mdata)
+                for i, xxxi in enumerate(xxx):
+                    self.set_mdata(xxxi, yyy[i], mdata)
 
             self.xold = xdata
             self.yold = ydata
 
             curlayer = self.myparent.sb_layer.value()
 
             xxx = self.myparent.xxx
@@ -1814,15 +1805,15 @@
             Unused.
 
         Returns
         -------
         None.
 
         """
-        self.figure.tight_layout()
+        # self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def init_grid(self, dat, dat2=None, opac=0.0):
         """
         Initialise grid.
 
         Parameters
@@ -1936,15 +1927,15 @@
         self.laxes.set_xlim(self.xlims)
         self.laxes.set_ylim(self.ylims)
         self.laxes.xaxis.set_major_formatter(frm)
         self.laxes.yaxis.set_major_formatter(frm)
 
         self.lims.set_visible(True)
 
-        self.figure.tight_layout()
+        # self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def slide_grid(self, dat, dat2=None, opac=None):
         """
         Slide grid.
 
         Parameters
@@ -2813,15 +2804,15 @@
 
         self.lmod.custprofx[curline] = [x1, x2, x1a, x2a]
         self.lmod.custprofy[curline] = [y1, y2, y1a, y2a]
         self.lmod.profpics[curline] = None
 
         imptext = self.importfile.text()
         if imptext != '':
-            dat = get_raster(imptext, showprocesslog=self.showprocesslog)
+            dat = get_raster(imptext, showlog=self.showlog)
 
             if dat is None:
                 QtWidgets.QMessageBox.warning(self.parent, 'Error',
                                               'Could not import the image.',
                                               QtWidgets.QMessageBox.Ok)
                 return curline
 
@@ -2892,16 +2883,15 @@
         Output data.
 
     """
     data = rgrv
     data2 = cgrv
     rows2, cols2 = data2.data.shape
 
-    dat = data_reproject(data, data.crs, data2.crs, data2.transform,
-                         rows2, cols2)
+    dat = data_reproject(data, data2.crs, data2.transform, rows2, cols2)
 
     return dat.data
 
 
 def rotate2d(pts, cntr, ang=np.pi/4):
     """
     Rotate 2D.
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/anaglyph.py` & `pygmi-3.2.7.16/pygmi/raster/anaglyph.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     ----------
     axes : matplotlib subplot
     parent : parent
         reference to the parent routine
     """
 
     def __init__(self, parent=None):
-        fig = Figure()
+        fig = Figure(layout='constrained')
         super().__init__(fig)
 
         self.axes = fig.add_subplot(111)
         self.scale = 7
         self.rotang = 10
         self.red1 = None
         self.blue1 = None
@@ -140,24 +140,24 @@
                 x1 = x1 + xmax
                 lines.append(np.transpose([x1, y1]))
 
         lc = mc.LineCollection(lines, colors=[0, 1, 1, 0.5])
         self.axes.add_collection(lc)
 
         self.axes.autoscale()
+        self.axes.set_aspect('equal')
 
         self.axes.set_xlabel('Eastings')
         self.axes.set_ylabel('Northings')
 
         self.axes.xaxis.set_major_formatter(frm)
         self.axes.yaxis.set_major_formatter(frm)
         self.axes.tick_params(axis='y', labelrotation=0)
         self.axes.tick_params(axis='x', labelrotation=90)
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_raster(self, data1, scale=7, rotang=10, atype='dubois',
                       cmap=colormaps['jet'], shade=False):
         """
         Update the raster plot.
 
@@ -268,15 +268,14 @@
         self.axes.set_ylabel('Northings')
 
         self.axes.tick_params(axis='y', labelrotation=0)
         self.axes.tick_params(axis='x', labelrotation=90)
         self.axes.xaxis.set_major_formatter(frm)
         self.axes.yaxis.set_major_formatter(frm)
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
 
 class PlotAnaglyph(ContextModule):
     """Graph Window - The QDialog window which will contain our image."""
 
     def __init__(self, parent=None):
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/cooper.py` & `pygmi-3.2.7.16/pygmi/raster/cooper.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         if not nodialog:
             temp = self.exec_()
             if temp == 0:
                 return False
 
@@ -150,16 +150,16 @@
             elif self.rb_dratio.isChecked():
                 data[i].data = derivative_ratio(data[i].data, self.azi,
                                                 self.order)
             elif self.rb_thg.isChecked():
                 data[i].data = thgrad(data[i].data, data[i].xdim, data[i].ydim)
             else:
                 if data[i].xdim != data[i].ydim:
-                    self.showprocesslog('X and Y dimension are different. '
-                                        'Please resample')
+                    self.showlog('X and Y dimension are different. '
+                                 'Please resample')
                     return False
 
                 mask = np.ma.getmaskarray(data[i].data)
                 dxy = data[i].xdim
                 data[i].data = np.ma.array(vertical(data[i].data, xint=dxy))
                 data[i].data.mask = mask
 
@@ -417,33 +417,33 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         if not nodialog:
             temp = self.exec_()
             if temp == 0:
                 return False
 
         self.wsize = self.sb_wsize.value()
         self.dh = self.sb_dh.value()
 
         data = copy.deepcopy(self.indata['Raster'])
         data2 = []
 
         for i, datai in enumerate(data):
-            self.showprocesslog(datai.dataid+':')
+            self.showlog(datai.dataid+':')
 
             vtot, vstd, vsum = visibility2d(datai.data, self.wsize,
-                                            self.dh*data[i].data.std()/100.,
+                                            self.dh*datai.data.std()/100.,
                                             self.piter)
 
             buff = self.wsize//2
 
             xmin, ymax = datai.transform*(buff, buff)
             xdim = datai.transform[0]
             ydim = abs(datai.transform[4])
@@ -463,15 +463,15 @@
 
             for i in [-3, -2, -1]:
                 mask = data2[i].data.mask
                 data2[i].data = data2[i].data.filled(data2[i].nodata)
                 data2[i].data = np.ma.array(data2[i].data, mask=mask)
 
         self.outdata['Raster'] = data2
-        self.showprocesslog('Finished!')
+        self.showlog('Finished!')
 
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
@@ -823,15 +823,15 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         if not nodialog:
             temp = self.exec_()
             if temp == 0:
                 return False
 
@@ -843,24 +843,24 @@
 
         self.wsize = self.sb_wsize.value()
 
         data = copy.deepcopy(self.indata['Raster'])
         data2 = []
 
         for datai in data:
-            self.showprocesslog(datai.dataid+':')
+            self.showlog(datai.dataid+':')
 
             agcdata = agc(datai.data, self.wsize, atype, nodata=datai.nodata,
                           piter=self.piter)
             data2.append(copy.deepcopy(datai))
             data2[-1].data = agcdata
             data2[-1].dataid += ' AGC'
 
         self.outdata['Raster'] = data2
-        self.showprocesslog('Finished!')
+        self.showlog('Finished!')
 
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/dataprep.py` & `pygmi-3.2.7.16/pygmi/rsense/iodefs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -----------------------------------------------------------------------------
-# Name:        dataprep.py (part of PyGMI)
+# Name:        iodefs.py (part of PyGMI)
 #
 # Author:      Patrick Cole
 # E-Mail:      pcole@geoscience.org.za
 #
-# Copyright:   (c) 2013 Council for Geoscience
+# Copyright:   (c) 2020 Council for Geoscience
 # Licence:     GPL-3.0
 #
 # This file is part of PyGMI
 #
 # PyGMI is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -18,212 +18,204 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
-"""A set of Raster Data Preparation routines."""
+"""Import remote sensing data."""
 
-import tempfile
-import math
 import os
 import sys
-import glob
 import copy
-from collections import Counter
+import xml.etree.ElementTree as ET
+import glob
+import tarfile
+import zipfile
+import datetime
+from collections import defaultdict
+import warnings
+
 from PyQt5 import QtWidgets, QtCore
 import numpy as np
+import numexpr as ne
 import pandas as pd
-from scipy.signal import tukey
+import geopandas as gpd
+from geopandas import GeoDataFrame
+from shapely.geometry import Point
 import rasterio
-import rasterio.merge
 from rasterio.crs import CRS
-from rasterio.warp import calculate_default_transform, reproject
-from rasterio.mask import mask as riomask
-import geopandas as gpd
-from shapely.geometry import LineString, Polygon, box
+from rasterio import Affine
+from natsort import natsorted
 
 from pygmi import menu_default
-from pygmi.raster.datatypes import Data
+from pygmi.raster.datatypes import Data, RasterMeta
+from pygmi.raster.iodefs import get_raster, export_raster
+from pygmi.raster.ginterp import histcomp, norm255, norm2, currentshader
 from pygmi.misc import ProgressBarText, ContextModule, BasicModule
-from pygmi.raster.datatypes import numpy_to_pygmi
-
-
-class DataCut(BasicModule):
-    """
-    Cut Data using shapefiles.
+from pygmi.raster.dataprep import lstack, data_reproject
+from pygmi.vector.dataprep import reprojxy
 
-    This class cuts raster datasets using a boundary defined by a polygon
-    shapefile.
-    """
-
-    def __init__(self, parent=None):
-        super().__init__(parent)
-
-    def settings(self, nodialog=False):
-        """
-        Entry point into item.
 
-        Parameters
-        ----------
-        nodialog : bool, optional
-            Run settings without a dialog. The default is False.
+warnings.filterwarnings("ignore",
+                        category=rasterio.errors.NotGeoreferencedWarning)
 
-        Returns
-        -------
-        bool
-            True if successful, False otherwise.
+EDIST = {1: 0.98331, 2: 0.9833, 3: 0.9833, 4: 0.9833,
+         5: 0.9833, 6: 0.98332, 7: 0.98333, 8: 0.98335,
+         9: 0.98338, 10: 0.98341, 11: 0.98345, 12: 0.98349,
+         13: 0.98354, 14: 0.98359, 15: 0.98365, 16: 0.98371,
+         17: 0.98378, 18: 0.98385, 19: 0.98393, 20: 0.98401,
+         21: 0.9841, 22: 0.98419, 23: 0.98428, 24: 0.98439,
+         25: 0.98449, 26: 0.9846, 27: 0.98472, 28: 0.98484,
+         29: 0.98496, 30: 0.98509, 31: 0.98523, 32: 0.98536,
+         33: 0.98551, 34: 0.98565, 35: 0.9858, 36: 0.98596,
+         37: 0.98612, 38: 0.98628, 39: 0.98645, 40: 0.98662,
+         41: 0.9868, 42: 0.98698, 43: 0.98717, 44: 0.98735,
+         45: 0.98755, 46: 0.98774, 47: 0.98794, 48: 0.98814,
+         49: 0.98835, 50: 0.98856, 51: 0.98877, 52: 0.98899,
+         53: 0.98921, 54: 0.98944, 55: 0.98966, 56: 0.98989,
+         57: 0.99012, 58: 0.99036, 59: 0.9906, 60: 0.99084,
+         61: 0.99108, 62: 0.99133, 63: 0.99158, 64: 0.99183,
+         65: 0.99208, 66: 0.99234, 67: 0.9926, 68: 0.99286,
+         69: 0.99312, 70: 0.99339, 71: 0.99365, 72: 0.99392,
+         73: 0.99419, 74: 0.99446, 75: 0.99474, 76: 0.99501,
+         77: 0.99529, 78: 0.99556, 79: 0.99584, 80: 0.99612,
+         81: 0.9964, 82: 0.99669, 83: 0.99697, 84: 0.99725,
+         85: 0.99754, 86: 0.99782, 87: 0.99811, 88: 0.9984,
+         89: 0.99868, 90: 0.99897, 91: 0.99926, 92: 0.99954,
+         93: 0.99983, 94: 1.00012, 95: 1.00041, 96: 1.00069,
+         97: 1.00098, 98: 1.00127, 99: 1.00155, 100: 1.00184,
+         101: 1.00212, 102: 1.0024, 103: 1.00269, 104: 1.00297,
+         105: 1.00325, 106: 1.00353, 107: 1.00381, 108: 1.00409,
+         109: 1.00437, 110: 1.00464, 111: 1.00492, 112: 1.00519,
+         113: 1.00546, 114: 1.00573, 115: 1.006, 116: 1.00626,
+         117: 1.00653, 118: 1.00679, 119: 1.00705, 120: 1.00731,
+         121: 1.00756, 122: 1.00781, 123: 1.00806, 124: 1.00831,
+         125: 1.00856, 126: 1.0088, 127: 1.00904, 128: 1.00928,
+         129: 1.00952, 130: 1.00975, 131: 1.00998, 132: 1.0102,
+         133: 1.01043, 134: 1.01065, 135: 1.01087, 136: 1.01108,
+         137: 1.01129, 138: 1.0115, 139: 1.0117, 140: 1.01191,
+         141: 1.0121, 142: 1.0123, 143: 1.01249, 144: 1.01267,
+         145: 1.01286, 146: 1.01304, 147: 1.01321, 148: 1.01338,
+         149: 1.01355, 150: 1.01371, 151: 1.01387, 152: 1.01403,
+         153: 1.01418, 154: 1.01433, 155: 1.01447, 156: 1.01461,
+         157: 1.01475, 158: 1.01488, 159: 1.015, 160: 1.01513,
+         161: 1.01524, 162: 1.01536, 163: 1.01547, 164: 1.01557,
+         165: 1.01567, 166: 1.01577, 167: 1.01586, 168: 1.01595,
+         169: 1.01603, 170: 1.0161, 171: 1.01618, 172: 1.01625,
+         173: 1.01631, 174: 1.01637, 175: 1.01642, 176: 1.01647,
+         177: 1.01652, 178: 1.01656, 179: 1.01659, 180: 1.01662,
+         181: 1.01665, 182: 1.01667, 183: 1.01668, 184: 1.0167,
+         185: 1.0167, 186: 1.0167, 187: 1.0167, 188: 1.01669,
+         189: 1.01668, 190: 1.01666, 191: 1.01664, 192: 1.01661,
+         193: 1.01658, 194: 1.01655, 195: 1.0165, 196: 1.01646,
+         197: 1.01641, 198: 1.01635, 199: 1.01629, 200: 1.01623,
+         201: 1.01616, 202: 1.01609, 203: 1.01601, 204: 1.01592,
+         205: 1.01584, 206: 1.01575, 207: 1.01565, 208: 1.01555,
+         209: 1.01544, 210: 1.01533, 211: 1.01522, 212: 1.0151,
+         213: 1.01497, 214: 1.01485, 215: 1.01471, 216: 1.01458,
+         217: 1.01444, 218: 1.01429, 219: 1.01414, 220: 1.01399,
+         221: 1.01383, 222: 1.01367, 223: 1.01351, 224: 1.01334,
+         225: 1.01317, 226: 1.01299, 227: 1.01281, 228: 1.01263,
+         229: 1.01244, 230: 1.01225, 231: 1.01205, 232: 1.01186,
+         233: 1.01165, 234: 1.01145, 235: 1.01124, 236: 1.01103,
+         237: 1.01081, 238: 1.0106, 239: 1.01037, 240: 1.01015,
+         241: 1.00992, 242: 1.00969, 243: 1.00946, 244: 1.00922,
+         245: 1.00898, 246: 1.00874, 247: 1.0085, 248: 1.00825,
+         249: 1.008, 250: 1.00775, 251: 1.0075, 252: 1.00724,
+         253: 1.00698, 254: 1.00672, 255: 1.00646, 256: 1.0062,
+         257: 1.00593, 258: 1.00566, 259: 1.00539, 260: 1.00512,
+         261: 1.00485, 262: 1.00457, 263: 1.0043, 264: 1.00402,
+         265: 1.00374, 266: 1.00346, 267: 1.00318, 268: 1.0029,
+         269: 1.00262, 270: 1.00234, 271: 1.00205, 272: 1.00177,
+         273: 1.00148, 274: 1.00119, 275: 1.00091, 276: 1.00062,
+         277: 1.00033, 278: 1.00005, 279: 0.99976, 280: 0.99947,
+         281: 0.99918, 282: 0.9989, 283: 0.99861, 284: 0.99832,
+         285: 0.99804, 286: 0.99775, 287: 0.99747, 288: 0.99718,
+         289: 0.9969, 290: 0.99662, 291: 0.99634, 292: 0.99605,
+         293: 0.99577, 294: 0.9955, 295: 0.99522, 296: 0.99494,
+         297: 0.99467, 298: 0.9944, 299: 0.99412, 300: 0.99385,
+         301: 0.99359, 302: 0.99332, 303: 0.99306, 304: 0.99279,
+         305: 0.99253, 306: 0.99228, 307: 0.99202, 308: 0.99177,
+         309: 0.99152, 310: 0.99127, 311: 0.99102, 312: 0.99078,
+         313: 0.99054, 314: 0.9903, 315: 0.99007, 316: 0.98983,
+         317: 0.98961, 318: 0.98938, 319: 0.98916, 320: 0.98894,
+         321: 0.98872, 322: 0.98851, 323: 0.9883, 324: 0.98809,
+         325: 0.98789, 326: 0.98769, 327: 0.9875, 328: 0.98731,
+         329: 0.98712, 330: 0.98694, 331: 0.98676, 332: 0.98658,
+         333: 0.98641, 334: 0.98624, 335: 0.98608, 336: 0.98592,
+         337: 0.98577, 338: 0.98562, 339: 0.98547, 340: 0.98533,
+         341: 0.98519, 342: 0.98506, 343: 0.98493, 344: 0.98481,
+         345: 0.98469, 346: 0.98457, 347: 0.98446, 348: 0.98436,
+         349: 0.98426, 350: 0.98416, 351: 0.98407, 352: 0.98399,
+         353: 0.98391, 354: 0.98383, 355: 0.98376, 356: 0.9837,
+         357: 0.98363, 358: 0.98358, 359: 0.98353, 360: 0.98348,
+         361: 0.98344, 362: 0.9834, 363: 0.98337, 364: 0.98335,
+         365: 0.98333, 366: 0.98331}
+
+K1 = [3040.136402, 2482.375199, 1935.060183, 866.468575, 641.326517]
+K2 = [1735.337945, 1666.398761, 1585.420044, 1350.069147, 1271.221673]
+ESUN = [1848, 1549, 1114, 225.4, 86.63, 81.85, 74.85, 66.49, 59.85]
 
-        """
-        if 'Raster' in self.indata:
-            data = self.indata['Raster']
-        else:
-            self.showprocesslog('No raster data')
-            return False
 
-        if not nodialog:
-            self.ifile, _ = QtWidgets.QFileDialog.getOpenFileName(
-                self.parent, 'Open Shape File', '.', 'Shape file (*.shp)')
-            if self.ifile == '':
-                return False
+class ImportData(BasicModule):
+    """Import Data - Interfaces with rasterio routines."""
 
-        os.chdir(os.path.dirname(self.ifile))
-        data = cut_raster(data, self.ifile, pprint=self.showprocesslog)
-
-        if data is None:
-            return False
-
-        self.outdata['Raster'] = data
-
-        return True
-
-    def loadproj(self, projdata):
-        """
-        Load project data into class.
-
-        Parameters
-        ----------
-        projdata : dictionary
-            Project data loaded from JSON project file.
+    def __init__(self, parent=None):
+        super().__init__(parent)
 
-        Returns
-        -------
-        chk : bool
-            A check to see if settings was successfully run.
+        self.filt = ''
 
-        """
-        self.ifile = projdata['shapefile']
+        self.sfile = QtWidgets.QLineEdit('')
+        self.lw_tnames = QtWidgets.QListWidget()
+        self.ftype = QtWidgets.QLabel('File Type:')
+        self.ensuresutm = QtWidgets.QCheckBox('Ensure WGS84 UTM is for '
+                                              'southern hemisphere')
 
-        return False
+        self.setupui()
 
-    def saveproj(self):
+    def setupui(self):
         """
-        Save project data from class.
+        Set up UI.
 
         Returns
         -------
-        projdata : dictionary
-            Project data to be saved to JSON project file.
+        None.
 
         """
-        projdata = {}
-
-        projdata['shapefile'] = self.ifile
-
-        return projdata
+        pb_sfile = QtWidgets.QPushButton(' Filename')
 
+        pixmapi = QtWidgets.QStyle.SP_DialogOpenButton
+        icon = self.style().standardIcon(pixmapi)
+        pb_sfile.setIcon(icon)
 
-class DataLayerStack(BasicModule):
-    """
-    Data Layer Stack.
+        self.setWindowTitle('Import Satellite Data')
+        self.ensuresutm.setChecked(True)
 
-    This class merges datasets which have different rows and columns. It
-    resamples them so that they have the same rows and columns.
-    """
+        gridlayout = QtWidgets.QGridLayout(self)
 
-    def __init__(self, parent=None):
-        super().__init__(parent)
-        self.dxy = None
-        self.piter = parent.pbar.iter
-        self.cmask = QtWidgets.QCheckBox('Common mask for all bands')
-
-        self.dsb_dxy = QtWidgets.QDoubleSpinBox()
-        self.label_rows = QtWidgets.QLabel('Rows: 0')
-        self.label_cols = QtWidgets.QLabel('Columns: 0')
-
-        self.setupui()
-
-    def setupui(self):
-        """
-        Set up UI.
+        self.lw_tnames.setSelectionMode(QtWidgets.QAbstractItemView.MultiSelection)
 
-        Returns
-        -------
-        None.
+        gridlayout.addWidget(pb_sfile, 1, 0, 1, 1)
+        gridlayout.addWidget(self.sfile, 1, 1, 1, 1)
+        gridlayout.addWidget(self.ftype, 2, 0, 1, 2)
+        gridlayout.addWidget(self.lw_tnames, 3, 0, 1, 2)
+        gridlayout.addWidget(self.ensuresutm, 4, 0, 1, 2)
 
-        """
-        gridlayout_main = QtWidgets.QGridLayout(self)
         buttonbox = QtWidgets.QDialogButtonBox()
-        helpdocs = menu_default.HelpButton('pygmi.raster.dataprep.'
-                                           'datalayerstack')
-        label_dxy = QtWidgets.QLabel('Cell Size:')
-
-        self.dsb_dxy.setMaximum(9999999999.0)
-        self.dsb_dxy.setMinimum(0.00001)
-        self.dsb_dxy.setDecimals(5)
-        self.dsb_dxy.setValue(40.)
         buttonbox.setOrientation(QtCore.Qt.Horizontal)
         buttonbox.setCenterButtons(True)
-        buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
-
-        self.cmask.setChecked(True)
+        buttonbox.setStandardButtons(
+            QtWidgets.QDialogButtonBox.Cancel | QtWidgets.QDialogButtonBox.Ok)
 
-        self.setWindowTitle('Dataset Layer Stack and Resample')
-
-        gridlayout_main.addWidget(label_dxy, 0, 0, 1, 1)
-        gridlayout_main.addWidget(self.dsb_dxy, 0, 1, 1, 1)
-        gridlayout_main.addWidget(self.label_rows, 1, 0, 1, 2)
-        gridlayout_main.addWidget(self.label_cols, 2, 0, 1, 2)
-        gridlayout_main.addWidget(self.cmask, 3, 0, 1, 2)
-        gridlayout_main.addWidget(helpdocs, 4, 0, 1, 1)
-        gridlayout_main.addWidget(buttonbox, 4, 1, 1, 1)
+        gridlayout.addWidget(buttonbox, 9, 0, 1, 2)
 
         buttonbox.accepted.connect(self.accept)
         buttonbox.rejected.connect(self.reject)
-        self.dsb_dxy.valueChanged.connect(self.dxy_change)
-
-    def dxy_change(self):
-        """
-        Update dxy.
-
-        This is the size of a grid cell in the x and y directions.
-
-        Returns
-        -------
-        None.
-
-        """
-        data = self.indata['Raster'][0]
-        dxy = self.dsb_dxy.value()
-
-        xmin0, xmax0, ymin0, ymax0 = data.extent
-
-        for data in self.indata['Raster']:
-            xmin, xmax, ymin, ymax = data.extent
-            xmin = min(xmin, xmin0)
-            xmax = max(xmax, xmax0)
-            ymin = min(ymin, ymin0)
-            ymax = max(ymax, ymax0)
-
-        cols = int((xmax - xmin)/dxy)
-        rows = int((ymax - ymin)/dxy)
-
-        self.label_rows.setText('Rows: '+str(rows))
-        self.label_cols.setText('Columns: '+str(cols))
+        pb_sfile.pressed.connect(self.get_sfile)
 
     def settings(self, nodialog=False):
         """
         Entry point into item.
 
         Parameters
         ----------
@@ -232,55 +224,99 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
-        if 'RasterFileList' in self.indata:
-            from pygmi.rsense.iodefs import get_data
+        self.lw_tnames.clear()
+        self.indata['Raster'] = []
+        self.sfile.setText('')
+        self.ftype.setText('File Type:')
 
-            ifiles = self.indata['RasterFileList']
-            self.showprocesslog('Warning: Layer stacking a file list assumes '
-                                'all datasets overlap in the same area')
-            self.indata['Raster'] = []
-            for ifile in ifiles:
-                self.showprocesslog('Processing '+os.path.basename(ifile))
-                dat = get_data(ifile, piter=self.piter,
-                               showprocesslog=self.showprocesslog,
-                               extscene='Bands Only')
-                for i in dat:
-                    i.data = i.data.astype(np.float32)
-                self.indata['Raster'] += dat
+        if not nodialog:
+            tmp = self.exec_()
+
+            if tmp != 1:
+                return tmp
 
-        if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+        tnames = []
+        for i in range(self.lw_tnames.count()):
+            item = self.lw_tnames.item(i)
+            if item.isSelected():
+                tnames.append(str(item.text()))
+
+        if not tnames:
             return False
 
-        if not nodialog:
-            data = self.indata['Raster'][0]
+        os.chdir(os.path.dirname(self.ifile))
 
-            if self.dxy is None:
-                self.dxy = min(data.xdim, data.ydim)
-                for data in self.indata['Raster']:
-                    self.dxy = min(self.dxy, data.xdim, data.ydim)
+        dat = get_data(self.ifile, self.piter, self.showlog, tnames)
 
-            self.dsb_dxy.setValue(self.dxy)
-            self.dxy_change()
+        if dat is None:
+            QtWidgets.QMessageBox.warning(self.parent, 'Error',
+                                          'Could not import the data.',
+                                          QtWidgets.QMessageBox.Ok)
+            return False
 
-            tmp = self.exec_()
-            if tmp != 1:
-                return False
+        if self.ensuresutm.isChecked() is True:
+            dat = utm_to_south(dat)
+
+        self.outdata['Raster'] = dat
+
+        return True
+
+    def get_sfile(self):
+        """Get the satellite filename."""
+        self.lw_tnames.clear()
+        self.indata['Raster'] = []
+        self.sfile.setText('')
+        self.ftype.setText('File Type:')
+
+        ext = ('Common formats (*.zip *.hdf *.tar *.tar.gz *.xml *.h5);;')
+
+        self.ifile, _ = QtWidgets.QFileDialog.getOpenFileName(
+            self.parent, 'Open File', '.', ext)
 
-        self.acceptall()
+        if not self.ifile:
+            return False
+
+        self.sfile.setText(self.ifile)
 
-        if self.outdata['Raster'] is None:
-            self.outdata = {}
+        self.indata['Raster'] = get_data(self.ifile, self.piter,
+                                         self.showlog, metaonly=True)
+
+        if self.indata['Raster'] is None:
+            self.showlog('Error: could not import data.')
+            self.sfile.setText('')
+            self.ftype.setText('File Type: Unknown')
             return False
 
+        tmp = []
+        for i in self.indata['Raster']:
+            tmp.append(i.dataid)
+
+        self.lw_tnames.clear()
+        self.lw_tnames.addItems(tmp)
+
+        for i in range(self.lw_tnames.count()):
+            item = self.lw_tnames.item(i)
+
+            if item.text()[0] == 'B':
+                item.setSelected(True)
+
+        # If nothing is selected, then select everything.
+        if not self.lw_tnames.selectedItems():
+            for i in range(self.lw_tnames.count()):
+                self.lw_tnames.item(i).setSelected(True)
+
+        instr = self.indata['Raster'][0].metadata['Raster']['Sensor']
+
+        self.ftype.setText(f' File Type: {instr}')
+
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
         Parameters
@@ -290,264 +326,230 @@
 
         Returns
         -------
         chk : bool
             A check to see if settings was successfully run.
 
         """
-        self.dxy = projdata['dxy']
-        self.cmask.setChecked(projdata['cmask'])
+        self.ifile = projdata['ifile']
+        self.filt = projdata['filt']
+
+        chk = self.settings(True)
 
-        return False
+        return chk
 
     def saveproj(self):
         """
         Save project data from class.
 
         Returns
         -------
         projdata : dictionary
             Project data to be saved to JSON project file.
 
         """
         projdata = {}
 
-        projdata['dxy'] = self.dsb_dxy.value()
-        projdata['cmask'] = self.cmask.isChecked()
+        projdata['ifile'] = self.ifile
+        projdata['filt'] = self.filt
 
         return projdata
 
-    def acceptall(self):
-        """
-        Accept option.
-
-        Updates self.outdata, which is used as input to other modules.
-
-        Returns
-        -------
-        None.
-
-        """
-        dxy = self.dsb_dxy.value()
-        self.dxy = dxy
-        dat = lstack(self.indata['Raster'], self.piter, dxy,
-                     pprint=self.showprocesslog,
-                     commonmask=self.cmask.isChecked())
-        self.outdata['Raster'] = dat
 
-
-class DataMerge(BasicModule):
+class ImportBatch(BasicModule):
     """
-    Data Merge.
+    Batch Import Data Interface.
+
+    This does not actually import data, but rather defines a list of datasets
+    to be used by other routines.
 
-    This class merges datasets which have different rows and columns. It
-    resamples them so that they have the same rows and columns.
+    Attributes
+    ----------
+    idir : str
+        Input directory.
     """
 
     def __init__(self, parent=None):
         super().__init__(parent)
-        self.idir = None
-        self.method = merge_median
-        self.rb_first = QtWidgets.QRadioButton('First - copy first file over '
-                                               'last file at overlap.')
-        self.rb_last = QtWidgets.QRadioButton('Last - copy last file over '
-                                              'first file at overlap.')
-        self.rb_min = QtWidgets.QRadioButton('Min - copy pixel wise minimum '
-                                             'at overlap.')
-        self.rb_max = QtWidgets.QRadioButton('Max - copy pixel wise maximum '
-                                             'at overlap.')
-        self.rb_median = QtWidgets.QRadioButton('Median - shift last file to '
-                                                'median '
-                                                'overlap value and copy over '
-                                                'first file at overlap.')
 
-        self.idirlist = QtWidgets.QLineEdit('')
+        self.idir = ''
+        self.tnames = None
+        self.filelist = []
+        self.bands = {}
+        self.tnames = {}
+        self.oldsensor = None
+
+        self.combo_sensor = QtWidgets.QComboBox()
         self.sfile = QtWidgets.QLineEdit('')
-        self.files_diff = QtWidgets.QCheckBox('Mosaic by band labels, '
-                                              'since band order may differ, '
-                                              'or input files have different '
-                                              'numbers of bands or '
-                                              'nodata values.')
-        self.shift_to_median = QtWidgets.QCheckBox('Shift bands to median '
-                                                   'value before mosaic. May '
-                                                   'allow for cleaner mosaic '
-                                                   'if datasets are offset.')
-
-        self.bands_to_files = QtWidgets.QCheckBox('Save each band separately '
-                                                  'in a "mosaic" '
-                                                  'subdirectory.')
-        self.forcetype = None
-        self.singleband = False
+        self.lw_tnames = QtWidgets.QListWidget()
+        self.ftype = QtWidgets.QLabel('File Type:')
+        self.ensuresutm = QtWidgets.QCheckBox('Ensure WGS84 UTM is for '
+                                              'southern hemisphere')
+
         self.setupui()
 
     def setupui(self):
         """
         Set up UI.
 
         Returns
         -------
         None.
 
         """
-        gridlayout_main = QtWidgets.QGridLayout(self)
-        buttonbox = QtWidgets.QDialogButtonBox()
-        helpdocs = menu_default.HelpButton('pygmi.raster.dataprep.datamerge')
-        pb_idirlist = QtWidgets.QPushButton('Batch Directory')
-        pb_sfile = QtWidgets.QPushButton('Shapefile for boundary (optional)')
-
-        self.files_diff.setChecked(True)
-        self.shift_to_median.setChecked(False)
-        self.rb_median.setChecked(True)
+        pb_sfile = QtWidgets.QPushButton(' Directory')
 
-        buttonbox.setOrientation(QtCore.Qt.Horizontal)
-        buttonbox.setCenterButtons(True)
-        buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
+        pixmapi = QtWidgets.QStyle.SP_DialogOpenButton
+        icon = self.style().standardIcon(pixmapi)
+        pb_sfile.setIcon(icon)
 
-        self.setWindowTitle('Dataset Mosaic')
+        self.setWindowTitle('Import Batch Data')
+        self.ensuresutm.setChecked(True)
 
-        gb_merge_method = QtWidgets.QGroupBox('Mosiac method')
-        gl_merge_method = QtWidgets.QVBoxLayout(gb_merge_method)
+        gridlayout = QtWidgets.QGridLayout(self)
 
-        gl_merge_method.addWidget(self.rb_median)
-        gl_merge_method.addWidget(self.rb_first)
-        gl_merge_method.addWidget(self.rb_last)
-        gl_merge_method.addWidget(self.rb_min)
-        gl_merge_method.addWidget(self.rb_max)
-
-        gridlayout_main.addWidget(pb_idirlist, 1, 0, 1, 1)
-        gridlayout_main.addWidget(self.idirlist, 1, 1, 1, 1)
-        gridlayout_main.addWidget(pb_sfile, 2, 0, 1, 1)
-        gridlayout_main.addWidget(self.sfile, 2, 1, 1, 1)
-        gridlayout_main.addWidget(self.files_diff, 3, 0, 1, 2)
-        gridlayout_main.addWidget(self.shift_to_median, 4, 0, 1, 2)
-        gridlayout_main.addWidget(gb_merge_method, 5, 0, 1, 2)
-        gridlayout_main.addWidget(self.bands_to_files, 6, 0, 1, 2)
-        gridlayout_main.addWidget(helpdocs, 7, 0, 1, 1)
-        gridlayout_main.addWidget(buttonbox, 7, 1, 1, 1)
+        self.lw_tnames.setSelectionMode(QtWidgets.QAbstractItemView.MultiSelection)
+
+        gridlayout.addWidget(pb_sfile, 1, 0, 1, 1)
+        gridlayout.addWidget(self.sfile, 1, 1, 1, 1)
+        gridlayout.addWidget(self.ftype, 2, 0, 1, 1)
+        gridlayout.addWidget(self.combo_sensor, 2, 1, 1, 1)
+        gridlayout.addWidget(self.lw_tnames, 3, 0, 1, 2)
+        gridlayout.addWidget(self.ensuresutm, 4, 0, 1, 2)
+
+        buttonbox = QtWidgets.QDialogButtonBox()
+        buttonbox.setOrientation(QtCore.Qt.Horizontal)
+        buttonbox.setCenterButtons(True)
+        buttonbox.setStandardButtons(
+            QtWidgets.QDialogButtonBox.Cancel | QtWidgets.QDialogButtonBox.Ok)
+
+        gridlayout.addWidget(buttonbox, 9, 0, 1, 2)
 
         buttonbox.accepted.connect(self.accept)
         buttonbox.rejected.connect(self.reject)
-        pb_idirlist.pressed.connect(self.get_idir)
         pb_sfile.pressed.connect(self.get_sfile)
-        self.shift_to_median.stateChanged.connect(self.shiftchanged)
-        self.files_diff.stateChanged.connect(self.filesdiffchanged)
-        self.rb_first.clicked.connect(self.method_change)
-        self.rb_last.clicked.connect(self.method_change)
-        self.rb_min.clicked.connect(self.method_change)
-        self.rb_max.clicked.connect(self.method_change)
-        self.rb_median.clicked.connect(self.method_change)
-
-    def method_change(self):
-        """
-        Change method.
-
-        Returns
-        -------
-        None.
+        self.combo_sensor.currentIndexChanged.connect(self.setsensor)
 
+    def settings(self, nodialog=False):
         """
-        if self.rb_first.isChecked():
-            self.method = 'first'
-        if self.rb_last.isChecked():
-            self.method = 'last'
-        if self.rb_min.isChecked():
-            self.method = merge_min
-        if self.rb_max.isChecked():
-            self.method = merge_max
-        if self.rb_median.isChecked():
-            self.method = merge_median
+        Entry point into item.
 
-    def shiftchanged(self):
-        """
-        Shift mean clicked.
+        Parameters
+        ----------
+        nodialog : bool, optional
+            Run settings without a dialog. The default is False.
 
         Returns
         -------
-        None.
-
-        """
-        if self.shift_to_median.isChecked():
-            self.files_diff.setChecked(True)
+        bool
+            True if successful, False otherwise.
 
-    def filesdiffchanged(self):
         """
-        Files different clicked.
+        if not nodialog or self.idir == '':
+            tmp = self.exec_()
 
-        Returns
-        -------
-        None.
+            if tmp != 1:
+                return tmp
 
-        """
-        if not self.files_diff.isChecked():
-            self.shift_to_median.setChecked(False)
-            self.bands_to_files.hide()
-        else:
-            self.bands_to_files.show()
+        if not self.filelist:
+            QtWidgets.QMessageBox.warning(self.parent, 'Error',
+                                          'No valid files in the directory.',
+                                          QtWidgets.QMessageBox.Ok)
+            return False
 
-    def get_idir(self):
-        """
-        Get the input directory.
+        self.setsensor()
 
-        Returns
-        -------
-        None.
+        for i in self.filelist:
+            i.to_sutm = self.ensuresutm.isChecked()
 
-        """
-        self.idir = QtWidgets.QFileDialog.getExistingDirectory(
-             self.parent, 'Select Directory')
+        self.outdata['RasterFileList'] = self.filelist
 
-        self.idirlist.setText(self.idir)
+        return True
 
-        if self.idir == '':
-            self.idir = None
+    def get_sfile(self, nodialog=False):
+        """Get the satellite filenames."""
+        if not nodialog:
+            self.idir = QtWidgets.QFileDialog.getExistingDirectory(
+                self.parent, 'Select Directory')
 
-    def get_sfile(self):
-        """
-        Get the input shapefile.
+            if not self.idir:
+                return False
 
-        Returns
-        -------
-        None.
+        self.sfile.setText(self.idir)
 
-        """
-        ext = ('ESRI Shapefile (*.shp);;')
+        types = ['*.tif', '*.hdr', '*.hdf', '*.zip', '*.tar', '*.tar.gz',
+                 '*.xml', '*.h5']
 
-        sfile, _ = QtWidgets.QFileDialog.getOpenFileName(
-            self.parent, 'Open File', '.', ext)
+        allfiles = []
+        for i in types:
+            allfiles += glob.glob(os.path.join(self.idir, i))
+
+        allfiles = consolidate_aster_list(allfiles)
+
+        self.bands = {}
+        self.tnames = {}
+        self.filelist = []
+        for ifile in self.piter(allfiles):
+            dat = get_data(ifile, showlog=self.showlog,
+                           metaonly=True, piter=iter)
+            if dat is None:
+                continue
+            datm = RasterMeta()
+            datm.fromData(dat)
 
-        if not sfile:
-            return False
+            self.bands[datm.sensor] = datm.bands
+            self.tnames[datm.sensor] = datm.tnames
+            self.filelist.append(datm)
+
+        self.combo_sensor.disconnect()
+        self.combo_sensor.clear()
+        self.combo_sensor.addItems(self.bands.keys())
+        self.combo_sensor.currentIndexChanged.connect(self.setsensor)
 
-        self.sfile.setText(sfile)
+        if not self.filelist:
+            self.showlog('No valid files in the directory.')
+        else:
+            self.setsensor()
 
         return True
 
-    def settings(self, nodialog=False):
+    def setsensor(self):
         """
-        Entry point into item.
-
-        Parameters
-        ----------
-        nodialog : bool, optional
-            Run settings without a dialog. The default is False.
+        Set the sensor band data.
 
         Returns
         -------
-        bool
-            True if successful, False otherwise.
+        None.
 
         """
-        if not nodialog:
-            tmp = self.exec_()
-            if tmp != 1:
-                return False
-
-        tmp = self.acceptall()
+        if self.lw_tnames.count() > 0:
+            self.tnames[self.oldsensor] = []
+            for i in range(self.lw_tnames.count()):
+                item = self.lw_tnames.item(i)
+                if item.isSelected():
+                    self.tnames[self.oldsensor].append(str(item.text()))
+
+            for i in self.filelist:
+                if i.sensor == self.oldsensor:
+                    i.tnames = self.tnames[self.oldsensor]
+
+        sensor = self.combo_sensor.currentText()
+        tmp = self.bands[sensor]
+
+        self.lw_tnames.clear()
+        self.lw_tnames.addItems(tmp)
+
+        for i in range(self.lw_tnames.count()):
+            item = self.lw_tnames.item(i)
+            if sensor == 'Generic':
+                item.setSelected(True)
+            elif item.text() in self.tnames[sensor]:
+                item.setSelected(True)
 
-        return tmp
+        self.oldsensor = sensor
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
         Parameters
         ----------
@@ -557,437 +559,120 @@
         Returns
         -------
         chk : bool
             A check to see if settings was successfully run.
 
         """
         self.idir = projdata['idir']
-        self.idirlist.setText(self.idir)
-        self.files_diff.setChecked(projdata['files_diff'])
-        self.shift_to_median.setChecked(projdata['mean_shift'])
 
-        return False
+        chk = self.settings(True)
+
+        return chk
 
     def saveproj(self):
         """
         Save project data from class.
 
         Returns
         -------
         projdata : dictionary
             Project data to be saved to JSON project file.
 
         """
         projdata = {}
 
         projdata['idir'] = self.idir
-        projdata['files_diff'] = self.files_diff.isChecked()
-        projdata['mean_shift'] = self.shift_to_median.isChecked()
 
         return projdata
 
-    def acceptall(self):
-        """
-        Accept option.
 
-        Updates self.outdata, which is used as input to other modules.
-
-        Returns
-        -------
-        bool
-            Success of routine.
-
-        """
-        if self.files_diff.isChecked():
-            tmp = self.merge_different()
-        else:
-            tmp = self.merge_same()
-
-        return tmp
-
-    def merge_different(self):
-        """
-        Merge files with different numbers of bands and/or band order.
-
-        This uses more memory, but is flexible.
-
-        Returns
-        -------
-        bool
-            Success of routine.
-
-        """
-        # The next line is only to avoid circular dependancies with merge
-        # function.
-
-        from pygmi.raster.iodefs import get_raster, export_raster
-
-        indata = []
-        if 'Raster' in self.indata:
-            for i in self.indata['Raster']:
-                indata.append(i)
-
-        if self.idir is not None:
-            ifiles = []
-            for ftype in ['*.tif', '*.hdr', '*.img', '*.ers']:
-                ifiles += glob.glob(os.path.join(self.idir, ftype))
-
-            if not ifiles:
-                self.showprocesslog('No input files in that directory')
-                return False
-
-            for ifile in self.piter(ifiles):
-                indata += get_raster(ifile, piter=iter, metaonly=True)
-
-        if indata is None:
-            self.showprocesslog('No input datasets')
-            return False
-
-        # Get projection information
-        wkt = []
-        crs = []
-        for i in indata:
-            if i.crs is None:
-                self.showprocesslog(f'{i.dataid} has no projection. '
-                                    'Please assign one.')
-                return False
-
-            wkt.append(i.crs.to_wkt())
-            crs.append(i.crs)
-            nodata = i.nodata
-
-        wkt, iwkt, numwkt = np.unique(wkt, return_index=True,
-                                      return_counts=True)
-        if len(wkt) > 1:
-            self.showprocesslog('Error: Mismatched input projections. '
-                                'Selecting most common projection')
-
-            crs = crs[iwkt[numwkt == numwkt.max()][0]]
-        else:
-            crs = indata[0].crs
-
-        bounds = get_shape_bounds(self.sfile.text(), crs, self.showprocesslog)
-
-        # Start Merge
-        bandlist = []
-        for i in indata:
-            bandlist.append(i.dataid)
-
-        bandlist = list(set(bandlist))
-
-        if self.singleband is True:
-            bandlist = ['Band_1']
-
-        outdat = []
-        for dataid in bandlist:
-            self.showprocesslog('Extracting '+dataid+'...')
-
-            if self.bands_to_files.isChecked():
-                odir = os.path.join(self.idir, 'mosaic')
-                os.makedirs(odir, exist_ok=True)
-                ofile = dataid+'.tif'
-                ofile = ofile.replace(' ', '_')
-                ofile = ofile.replace(',', '_')
-                ofile = ofile.replace('*', 'mult')
-                ofile = os.path.join(odir, ofile)
-
-                if os.path.exists(ofile):
-                    self.showprocesslog('Output file exists, skipping.')
-                    continue
-
-            ifiles = []
-            allmval = []
-            for i in self.piter(indata):
-                if i.dataid != dataid and self.singleband is False:
-                    continue
-                metadata = i.metadata
-
-                i2 = get_raster(i.filename, piter=iter, dataid=i.dataid)
-
-                if i2 is None:
-                    continue
-
-                i2 = i2[0]
-
-                if i2.crs != crs:
-                    src_height, src_width = i2.data.shape
-
-                    transform, width, height = calculate_default_transform(
-                        i2.crs, crs, src_width, src_height, *i2.bounds)
-
-                    i2 = data_reproject(i2, i2.crs, crs, transform, height,
-                                        width)
-
-                if self.forcetype is not None:
-                    i2.data = i2.data.astype(self.forcetype)
-
-                if self.shift_to_median.isChecked():
-                    mval = np.ma.median(i2.data)
-                else:
-                    mval = 0
-                allmval.append(mval)
-
-                if self.singleband is True:
-                    i2.dataid = 'Band_1'
-
-                trans = rasterio.transform.from_origin(i2.extent[0],
-                                                       i2.extent[3],
-                                                       i2.xdim, i2.ydim)
-
-                tmpfile = os.path.join(tempfile.gettempdir(),
-                                       os.path.basename(i.filename))
-
-                tmpid = i2.dataid
-                tmpid = tmpid.replace(' ', '_')
-                tmpid = tmpid.replace(',', '_')
-                tmpid = tmpid.replace('*', 'mult')
-                tmpid = tmpid.replace(r'/', 'div')
-
-                tmpfile = tmpfile[:-4]+'_'+tmpid+'.tif'
-
-                raster = rasterio.open(tmpfile, 'w', driver='GTiff',
-                                       height=i2.data.shape[0],
-                                       width=i2.data.shape[1], count=1,
-                                       dtype=i2.data.dtype,
-                                       transform=trans)
-
-                if np.issubdtype(i2.data.dtype, np.floating):
-                    nodata = 1.0e+20
-                else:
-                    nodata = -99999
-
-                tmpdat = i2.data-mval
-                tmpdat = tmpdat.filled(nodata)
-                tmpdat = np.ma.masked_equal(tmpdat, nodata)
-
-                raster.write(tmpdat, 1)
-                raster.write_mask(~np.ma.getmaskarray(i2.data))
-
-                raster.close()
-                ifiles.append(tmpfile)
-                del i2
-
-            if len(ifiles) < 2:
-                self.showprocesslog('Too few bands of name '+dataid)
-                continue
-
-            self.showprocesslog('Mosaicing '+dataid+'...')
-            # print(ifiles)
-
-            with rasterio.Env(CPL_DEBUG=True):
-                mosaic, otrans = rasterio.merge.merge(ifiles, nodata=nodata,
-                                                      method=self.method,
-                                                      bounds=bounds)
-
-            for j in ifiles:
-                if os.path.exists(j):
-                    os.remove(j)
-                if os.path.exists(j+'.msk'):
-                    os.remove(j+'.msk')
-
-            mosaic = mosaic.squeeze()
-            mosaic = np.ma.masked_equal(mosaic, nodata)
-            mosaic = mosaic + np.median(allmval)
-            outdat.append(numpy_to_pygmi(mosaic, dataid=dataid))
-            outdat[-1].set_transform(transform=otrans)
-            outdat[-1].crs = crs
-            outdat[-1].nodata = nodata
-            outdat[-1].metadata = metadata
-
-            if self.bands_to_files.isChecked():
-                export_raster(ofile, outdat, 'GTiff', compression='ZSTD')
-
-                del outdat
-                del mosaic
-                outdat = []
-
-        if bounds is not None:
-            outdat = cut_raster(outdat, self.sfile.text(), deepcopy=False)
-
-        self.outdata['Raster'] = outdat
-
-        return True
-
-    def merge_same(self):
-        """
-        Mosaic files with same numbers of bands and band order.
-
-        This uses much less memory, but is less flexible.
-
-        Returns
-        -------
-        bool
-            Success of routine.
-
-        """
-        ifiles = []
-        if 'Raster' in self.indata:
-            for i in self.indata['Raster']:
-                ifiles.append(i.filename)
-
-        if self.idir is not None:
-            for ftype in ['*.tif', '*.hdr', '*.img', '*.ers']:
-                ifiles += glob.glob(os.path.join(self.idir, ftype))
-
-        if not ifiles:
-            self.showprocesslog('No input datasets')
-            return False
-
-        for i, ifile in enumerate(ifiles):
-            if ifile[-3:] == 'hdr':
-                ifile = ifile[:-4]
-                if os.path.exists(ifile+'.dat'):
-                    ifiles[i] = ifile+'.dat'
-                elif os.path.exists(ifile+'.raw'):
-                    ifiles[i] = ifile+'.raw'
-                elif os.path.exists(ifile+'.img'):
-                    ifiles[i] = ifile+'.img'
-                elif not os.path.exists(ifile):
-                    return False
-
-        # Get projection information
-        wkt = []
-        nodata = []
-        for ifile in ifiles:
-            with rasterio.open(ifile) as dataset:
-                if dataset.crs is None:
-                    self.showprocesslog(f'{ifile} has no projection. '
-                                        'Please assign one.')
-                    return False
-                wkt.append(dataset.crs.wkt)
-                crs = dataset.crs
-                nodata.append(dataset.nodata)
-
-        wkt = list(set(wkt))
-        if len(wkt) > 1:
-            self.showprocesslog('Error: Mismatched input projections')
-            return False
-
-        nodata = list(set(nodata))
-        if len(nodata) > 1:
-            self.showprocesslog('Error: Mismatched nodata values. '
-                                'Try using merge by band labels merge option. '
-                                'Please confirm bands to be merged have the '
-                                'same label.')
-            return False
-
-        # Get band names and nodata
-        with rasterio.open(ifiles[0]) as dataset:
-            bnames = dataset.descriptions
-            if None in bnames:
-                bnames = ['Band '+str(i) for i in dataset.indexes]
-            nodata = dataset.nodata
-
-        # Start Merge
-        mosaic, otrans = rasterio.merge.merge(ifiles, nodata=nodata,
-                                              method=self.method)
-        mosaic = np.ma.masked_equal(mosaic, nodata)
-
-        outdat = []
-        for i, dataid in enumerate(bnames):
-            outdat.append(numpy_to_pygmi(mosaic[i], dataid=dataid))
-            outdat[-1].set_transform(transform=otrans)
-            outdat[-1].crs = crs
-            outdat[-1].nodata = nodata
-
-        self.outdata['Raster'] = outdat
-
-        return True
-
-
-class DataReproj(BasicModule):
-    """
-    Reprojections.
-
-    This class reprojects datasets using the rasterio routines.
-    """
+class ImportSentinel5P(BasicModule):
+    """Import Sentinel 5P data to shapefile."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
-        self.orig_wkt = None
-        self.targ_wkt = None
 
-        self.groupboxb = QtWidgets.QGroupBox()
-        self.combobox_inp_epsg = QtWidgets.QComboBox()
-        self.inp_epsg_info = QtWidgets.QLabel(wordWrap=True)
-        self.groupbox2b = QtWidgets.QGroupBox()
-        self.combobox_out_epsg = QtWidgets.QComboBox()
-        self.out_epsg_info = QtWidgets.QLabel()
-        self.in_proj = GroupProj('Input Projection')
-        self.out_proj = GroupProj('Output Projection')
+        self.sfile = ''
+        self.filt = ''
+        self.indx = 0
+
+        self.subdata = QtWidgets.QComboBox()
+        self.lonmin = QtWidgets.QLineEdit('16')
+        self.lonmax = QtWidgets.QLineEdit('34')
+        self.latmin = QtWidgets.QLineEdit('-35')
+        self.latmax = QtWidgets.QLineEdit('-21')
+        self.qathres = QtWidgets.QLineEdit('50')
+        self.cclip = QtWidgets.QRadioButton('Clip using coordinates')
+        self.sclip = QtWidgets.QRadioButton('Clip using shapefile')
+        self.shpfile = QtWidgets.QLineEdit(self.sfile)
+        self.label_sfile = QtWidgets.QPushButton('Load shapefile')
+        self.label_lonmin = QtWidgets.QLabel('Minimum Longitude:')
+        self.label_lonmax = QtWidgets.QLabel('Maximum Longitude:')
+        self.label_latmin = QtWidgets.QLabel('Minimum Latitude:')
+        self.label_latmax = QtWidgets.QLabel('Maximum Latitude:')
 
         self.setupui()
 
     def setupui(self):
         """
         Set up UI.
 
         Returns
         -------
         None.
 
         """
         gridlayout_main = QtWidgets.QGridLayout(self)
         buttonbox = QtWidgets.QDialogButtonBox()
-        helpdocs = menu_default.HelpButton('pygmi.raster.dataprep.datareproj')
+        helpdocs = menu_default.HelpButton('pygmi.rsense.iodefs.'
+                                           'importsentinel5p')
+        label_subdata = QtWidgets.QLabel('Product:')
+        label_qathres = QtWidgets.QLabel('QA Threshold (0-100):')
 
         buttonbox.setOrientation(QtCore.Qt.Horizontal)
         buttonbox.setCenterButtons(True)
         buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
+        self.cclip.setChecked(True)
+        self.label_sfile.hide()
+        self.shpfile.hide()
 
-        self.setWindowTitle('Dataset Reprojection')
-
-        gridlayout_main.addWidget(self.in_proj, 0, 0, 1, 1)
-        gridlayout_main.addWidget(self.out_proj, 0, 1, 1, 1)
-        gridlayout_main.addWidget(helpdocs, 1, 0, 1, 1)
-        gridlayout_main.addWidget(buttonbox, 1, 1, 1, 1)
+        self.setWindowTitle(r'Import Sentinel-5P Data')
 
-        buttonbox.accepted.connect(self.accept)
-        buttonbox.rejected.connect(self.reject)
+        gridlayout_main.addWidget(label_subdata, 0, 0, 1, 1)
+        gridlayout_main.addWidget(self.subdata, 0, 1, 1, 1)
 
-    def acceptall(self):
-        """
-        Accept option.
+        gridlayout_main.addWidget(self.cclip, 1, 0, 1, 2)
+        gridlayout_main.addWidget(self.sclip, 2, 0, 1, 2)
 
-        Updates self.outdata, which is used as input to other modules.
+        gridlayout_main.addWidget(self.label_lonmin, 3, 0, 1, 1)
+        gridlayout_main.addWidget(self.lonmin, 3, 1, 1, 1)
 
-        Returns
-        -------
-        None.
+        gridlayout_main.addWidget(self.label_lonmax, 4, 0, 1, 1)
+        gridlayout_main.addWidget(self.lonmax, 4, 1, 1, 1)
 
-        """
-        if self.in_proj.wkt == 'Unknown' or self.out_proj.wkt == 'Unknown':
-            self.showprocesslog('Unknown Projection. Could not reproject')
-            return
+        gridlayout_main.addWidget(self.label_latmin, 5, 0, 1, 1)
+        gridlayout_main.addWidget(self.latmin, 5, 1, 1, 1)
 
-        if self.in_proj.wkt == '' or self.out_proj.wkt == '':
-            self.showprocesslog('Unknown Projection. Could not reproject')
-            return
+        gridlayout_main.addWidget(self.label_latmax, 6, 0, 1, 1)
+        gridlayout_main.addWidget(self.latmax, 6, 1, 1, 1)
 
-        # Input stuff
-        src_crs = CRS.from_wkt(self.in_proj.wkt)
+        gridlayout_main.addWidget(self.label_sfile, 7, 0, 1, 1)
+        gridlayout_main.addWidget(self.shpfile, 7, 1, 1, 1)
 
-        # Output stuff
-        dst_crs = CRS.from_wkt(self.out_proj.wkt)
+        gridlayout_main.addWidget(label_qathres, 8, 0, 1, 1)
+        gridlayout_main.addWidget(self.qathres, 8, 1, 1, 1)
 
-        # Now create virtual dataset
-        dat = []
-        for data in self.piter(self.indata['Raster']):
-            src_height, src_width = data.data.shape
+        gridlayout_main.addWidget(helpdocs, 10, 0, 1, 1)
+        gridlayout_main.addWidget(buttonbox, 10, 1, 1, 3)
 
-            transform, width, height = calculate_default_transform(
-                src_crs, dst_crs, src_width, src_height, *data.bounds)
-
-            # Work out the boundaries of the new dataset in target projection
-            data2 = data_reproject(data, src_crs, dst_crs, transform,
-                                   height, width)
-
-            dat.append(data2)
-
-        self.outdata['Raster'] = dat
+        buttonbox.accepted.connect(self.accept)
+        buttonbox.rejected.connect(self.reject)
+        self.cclip.clicked.connect(self.clipchoice)
+        self.sclip.clicked.connect(self.clipchoice)
+        self.label_sfile.clicked.connect(self.loadshp)
 
     def settings(self, nodialog=False):
         """
         Entry point into item.
 
         Parameters
         ----------
@@ -996,2376 +681,2606 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
-        if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
-            return False
+        if not nodialog:
+            ext = ('Sentinel-5P (*.nc)')
+
+            self.ifile, self.filt = QtWidgets.QFileDialog.getOpenFileName(
+                self.parent, 'Open File', '.', ext)
+            if self.ifile == '':
+                return False
 
-        if self.indata['Raster'][0].crs is None:
-            self.showprocesslog('Your input data has no projection. '
-                                'Please assign one in the metadata summary.')
+        os.chdir(os.path.dirname(self.ifile))
+
+        meta = self.get_5P_meta()
+
+        if meta is None:
             return False
 
-        if self.orig_wkt is None:
-            self.orig_wkt = self.indata['Raster'][0].crs.wkt
-        if self.targ_wkt is None:
-            self.targ_wkt = self.indata['Raster'][0].crs.wkt
+        tmp = []
+        for i in meta:
+            if i in ['latitude', 'longitude', 'qa_value']:
+                continue
+            tmp.append(i)
 
-        self.in_proj.set_current(self.orig_wkt)
-        self.out_proj.set_current(self.targ_wkt)
+        self.subdata.clear()
+        self.subdata.addItems(tmp)
+        self.subdata.setCurrentIndex(self.indx)
 
         if not nodialog:
             tmp = self.exec_()
+
             if tmp != 1:
-                return False
+                return tmp
 
-        self.acceptall()
+        try:
+            _ = float(self.lonmin.text())
+            _ = float(self.latmin.text())
+            _ = float(self.lonmax.text())
+            _ = float(self.latmax.text())
+        except ValueError:
+            self.showlog('Value error - abandoning import')
+            return False
 
-        return True
+        gdf = self.get_5P_data(meta)
 
-    def loadproj(self, projdata):
-        """
-        Load project data into class.
+        if gdf is None:
+            return False
 
-        Parameters
-        ----------
-        projdata : dictionary
-            Project data loaded from JSON project file.
+        if gdf.geom_type.loc[0] == 'Point':
+            if 'line' not in gdf.columns:
+                gdf['line'] = 'None'
+            else:
+                gdf['line'] = gdf['line'].astype(str)
 
-        Returns
-        -------
-        chk : bool
-            A check to see if settings was successfully run.
+        gdf.attrs['source'] = os.path.basename(self.ifile)
 
-        """
-        self.orig_wkt = projdata['orig_wkt']
-        self.targ_wkt = projdata['targ_wkt']
+        self.outdata['Vector'] = [gdf]
 
-        return False
+        return True
 
-    def saveproj(self):
+    def clipchoice(self):
         """
-        Save project data from class.
+        Choose clip style.
 
         Returns
         -------
-        projdata : dictionary
-            Project data to be saved to JSON project file.
+        None.
 
         """
-        projdata = {}
-
-        projdata['orig_wkt'] = self.in_proj.wkt
-        projdata['targ_wkt'] = self.out_proj.wkt
-
-        return projdata
-
-
-class GetProf(BasicModule):
-    """
-    Get a Profile.
-
-    This class extracts a profile from a raster dataset using a line shapefile.
-    """
-
-    def __init__(self, parent=None):
-        super().__init__(parent)
+        if self.cclip.isChecked():
+            self.label_sfile.hide()
+            self.shpfile.hide()
+            self.lonmin.show()
+            self.lonmax.show()
+            self.latmin.show()
+            self.latmax.show()
+            self.label_lonmin.show()
+            self.label_lonmax.show()
+            self.label_latmin.show()
+            self.label_latmax.show()
+        else:
+            self.lonmin.hide()
+            self.lonmax.hide()
+            self.latmin.hide()
+            self.latmax.hide()
+            self.label_lonmin.hide()
+            self.label_lonmax.hide()
+            self.label_latmin.hide()
+            self.label_latmax.hide()
+            self.label_sfile.show()
+            self.shpfile.show()
 
-    def settings(self, nodialog=False):
+    def loadproj(self, projdata):
         """
-        Entry point into item.
+        Load project data into class.
 
         Parameters
         ----------
-        nodialog : bool, optional
-            Run settings without a dialog. The default is False.
+        projdata : dictionary
+            Project data loaded from JSON project file.
 
         Returns
         -------
-        bool
-            True if successful, False otherwise.
+        chk : bool
+            A check to see if settings was successfully run.
 
         """
-        if 'Raster' in self.indata:
-            data = copy.deepcopy(self.indata['Raster'])
-        else:
-            self.showprocesslog('No raster data')
-            return False
-
-        ext = 'Shape file (*.shp)'
+        self.ifile = projdata['ifile']
+        self.filt = projdata['filt']
 
-        if not nodialog:
-            self.ifile, _ = QtWidgets.QFileDialog.getOpenFileName(
-                self.parent, 'Open Shape File', '.', ext)
-            if self.ifile == '':
-                return False
+        chk = self.settings(True)
 
-        os.chdir(os.path.dirname(self.ifile))
+        return chk
 
-        try:
-            gdf = gpd.read_file(self.ifile)
-        except:
-            self.showprocesslog('There was a problem importing the shapefile. '
-                                'Please make sure you have at all the '
-                                'individual files which make up the '
-                                'shapefile.')
-            return None
-
-        gdf = gdf[gdf.geometry != None]
-
-        if gdf.geom_type.iloc[0] != 'LineString':
-            self.showprocesslog('You need lines in that shape file')
-            return False
-
-        data = lstack(data, self.piter, pprint=self.showprocesslog)
-        dxy = min(data[0].xdim, data[0].ydim)
-        ogdf2 = None
-
-        icnt = 0
-        for line in gdf.geometry:
-            line2 = redistribute_vertices(line, dxy)
-            x, y = line2.coords.xy
-            xy = np.transpose([x, y])
-            ogdf = None
-
-            for idata in self.piter(data):
-                mdata = idata.to_mem()
-                z = []
-                for pnt in xy:
-                    z.append(idata.data[mdata.index(pnt[0], pnt[1])])
-
-                if ogdf is None:
-                    ogdf = pd.DataFrame(xy[:, 0], columns=['X'])
-                    ogdf['Y'] = xy[:, 1]
-                    ogdf['pygmiX'] = ogdf['X']
-                    ogdf['pygmiY'] = ogdf['Y']
-
-                ogdf[idata.dataid] = z
-
-            icnt += 1
-            ogdf['line'] = str(icnt)
-            if ogdf2 is None:
-                ogdf2 = ogdf
-            else:
-                ogdf2 = ogdf2.append(ogdf, ignore_index=True)
-
-        self.outdata['Line'] = {'profile': ogdf2}
-
-        return True
-
-    def loadproj(self, projdata):
+    def loadshp(self):
         """
-        Load project data into class.
-
-        Parameters
-        ----------
-        projdata : dictionary
-            Project data loaded from JSON project file.
+        Load shapefile filename.
 
         Returns
         -------
-        chk : bool
-            A check to see if settings was successfully run.
+        None.
 
         """
-        self.ifile = projdata['shapefile']
+        ext = ('Shapefile (*.shp)')
 
-        return False
+        self.sfile, _ = QtWidgets.QFileDialog.getOpenFileName(
+            self.parent, 'Open File', '.', ext)
+
+        self.shpfile.setText(self.sfile)
 
     def saveproj(self):
         """
         Save project data from class.
 
         Returns
         -------
         projdata : dictionary
             Project data to be saved to JSON project file.
 
         """
         projdata = {}
 
-        projdata['shapefile'] = self.ifile
+        projdata['ifile'] = self.ifile
+        projdata['filt'] = self.filt
 
         return projdata
 
+    def get_5P_meta(self):
+        """
+        Get 5P metadata.
 
-class GroupProj(QtWidgets.QWidget):
-    """
-    Group Proj.
-
-    Custom widget
-    """
-
-    def __init__(self, title='Projection', parent=None):
-        super().__init__(parent)
+        Returns
+        -------
+        meta : Dictionary
+            Dictionary containing metadata.
 
-        self.wkt = ''
+        """
+        with rasterio.open(self.ifile) as dataset:
+            subdata = dataset.subdatasets
 
-        self.gridlayout = QtWidgets.QGridLayout(self)
-        self.groupbox = QtWidgets.QGroupBox(title)
-        self.combodatum = QtWidgets.QComboBox()
-        self.comboproj = QtWidgets.QComboBox()
-        self.label = QtWidgets.QLabel()
-        self.label.setWordWrap(True)
-
-        self.gridlayout.addWidget(self.groupbox, 1, 0, 1, 2)
-
-        gridlayout = QtWidgets.QGridLayout(self.groupbox)
-        gridlayout.addWidget(self.combodatum, 0, 0, 1, 1)
-        gridlayout.addWidget(self.comboproj, 1, 0, 1, 1)
-        gridlayout.addWidget(self.label, 2, 0, 1, 1)
-
-        self.epsg_proj = getepsgcodes()
-        self.epsg_proj[r'Current / Current'] = self.wkt
-        tmp = list(self.epsg_proj.keys())
-        tmp.sort(key=lambda c: c.lower())
+        meta = {}
+        for i in subdata:
+            tmp = i.split(':')
+            if 'SUPPORT_DATA' in i:
+                continue
+            if 'METADATA' in i:
+                continue
+            if 'time_utc' in i:
+                continue
+            if 'delta_time' in i:
+                continue
+            # if 'qa_value' in i:
+            #     continue
+            if 'precision' in i:
+                continue
 
-        self.plist = {}
-        for i in tmp:
-            if r' / ' in i:
-                datum, proj = i.split(r' / ')
-            else:
-                datum = i
-                proj = i
+            tmp = tmp[-1].replace('//PRODUCT/', '')
+            tmp = tmp.replace('/PRODUCT/', '')
+            tmp = tmp.replace('/', '')
 
-            if datum not in self.plist:
-                self.plist[datum] = []
-            self.plist[datum].append(proj)
+            meta[tmp] = i
 
-        tmp = list(set(self.plist.keys()))
-        tmp.sort()
-        tmp = ['Current', 'WGS 84']+tmp
+        dataset = None
 
-        for i in tmp:
-            j = self.plist[i]
-            if r'Geodetic Geographic' in j and j[0] != r'Geodetic Geographic':
-                self.plist[i] = [r'Geodetic Geographic']+self.plist[i]
-
-        self.combodatum.addItems(tmp)
-        self.comboproj.addItem('Current')
-        self.combodatum.currentIndexChanged.connect(self.combo_datum_change)
-        self.comboproj.currentIndexChanged.connect(self.combo_change)
+        return meta
 
-    def set_current(self, wkt):
+    def get_5P_data(self, meta):
         """
-        Set new WKT for current option.
+        Get 5P data.
 
         Parameters
         ----------
-        wkt : str
-            Well Known Text descriptions for coordinates (WKT) .
+        meta : Dictionary
+            Dictionary containing metadata.
 
         Returns
         -------
-        None.
+        gdf : DataFrame
+            geopandas dataframe.
 
         """
-        self.wkt = wkt
-        self.epsg_proj[r'Current / Current'] = self.wkt
-        self.combo_change()
+        try:
+            thres = int(self.qathres.text())
+        except ValueError:
+            self.showlog('Threshold text not an integer')
+            return None
 
-    def combo_datum_change(self):
-        """
-        Change Combo.
+        with rasterio.open(meta['latitude']) as dataset:
+            lats = dataset.read(1)
 
-        Returns
-        -------
-        None.
+        with rasterio.open(meta['longitude']) as dataset:
+            lons = dataset.read(1)
 
-        """
-        indx = self.combodatum.currentIndex()
-        txt = self.combodatum.itemText(indx)
-        self.comboproj.currentIndexChanged.disconnect()
+        with rasterio.open(meta['qa_value']) as dataset:
+            qaval = dataset.read(1)
 
-        self.comboproj.clear()
-        self.comboproj.addItems(self.plist[txt])
+        with rasterio.open(meta['longitude']) as dataset:
+            lons = dataset.read(1)
 
-        self.comboproj.currentIndexChanged.connect(self.combo_change)
+        del meta['latitude']
+        del meta['longitude']
 
-        self.combo_change()
+        if lats is None:
+            self.showlog('No Latitudes in dataset')
+            return None
 
-    def combo_change(self):
-        """
-        Change Combo.
+        lats = lats.flatten()
+        lons = lons.flatten()
+        pnts = np.transpose([lons, lats])
+
+        if self.cclip.isChecked():
+            lonmin = float(self.lonmin.text())
+            latmin = float(self.latmin.text())
+            lonmax = float(self.lonmax.text())
+            latmax = float(self.latmax.text())
+        else:
+            shp = gpd.read_file(self.sfile)
+            shp = shp.to_crs(4326)
 
-        Returns
-        -------
-        None.
+            lonmin = float(shp.bounds.minx)
+            lonmax = float(shp.bounds.maxx)
+            latmin = float(shp.bounds.miny)
+            latmax = float(shp.bounds.maxy)
 
-        """
-        dtxt = self.combodatum.currentText()
-        ptxt = self.comboproj.currentText()
+        mask = ((lats > latmin) & (lats < latmax) & (lons < lonmax) &
+                (lons > lonmin))
 
-        txt = dtxt + r' / '+ptxt
+        idfile = self.subdata.currentText()
 
-        self.wkt = self.epsg_proj[txt]
+        dfile = meta[idfile]
 
-        if not isinstance(self.wkt, str):
-            self.wkt = epsgtowkt(self.wkt)
+        with rasterio.open(dfile) as dataset:
+            dat = dataset.read(1)
 
-        # The next two lines make sure we have spaces after ALL commas.
-        wkttmp = self.wkt.replace(', ', ',')
-        wkttmp = wkttmp.replace(',', ', ')
+        dat1 = dat.flatten()
+        qaval1 = qaval.flatten()
 
-        self.label.setText(wkttmp)
+        if mask.shape != dat1.shape:
+            return None
 
+        dat1 = dat1[mask]
+        pnts1 = pnts[mask]
+        qaval1 = qaval1[mask]
 
-class Metadata(ContextModule):
-    """
-    Edit Metadata.
+        qaval1 = qaval1[dat1 != 9.96921e+36]
+        pnts1 = pnts1[dat1 != 9.96921e+36]
+        dat1 = dat1[dat1 != 9.96921e+36]
 
-    This class allows the editing of the metadata for a raster dataset using a
-    GUI.
+        pnts1 = pnts1[qaval1 >= thres]
+        dat1 = dat1[qaval1 >= thres]
 
-    Attributes
-    ----------
-    banddata : dictionary
-        band data
-    bandid : dictionary
-        dictionary of strings containing band names.
-    """
+        df = pd.DataFrame({'lon': pnts1[:, 0], 'lat': pnts1[:, 1]})
+        df['data'] = dat1
+
+        gdf = GeoDataFrame(df.drop(['lon', 'lat'], axis=1),
+                           geometry=[Point(xy) for xy in zip(df.lon, df.lat)])
+
+        gdf = gdf.set_crs("EPSG:4326")
+
+        if self.sclip.isChecked():
+            gdf = gdf.clip(shp)
+
+        if gdf.size == 0:
+            self.showlog(idfile, 'is empty.')
+            return None
+
+        return gdf
+
+
+class ExportBatch(ContextModule):
+    """Export Raster File List."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
-        self.banddata = {}
-        self.dataid = {}
-        self.oldtxt = ''
-
-        self.combobox_bandid = QtWidgets.QComboBox()
-        self.pb_rename_id = QtWidgets.QPushButton('Rename Band Name')
-        self.lbl_rows = QtWidgets.QLabel()
-        self.lbl_cols = QtWidgets.QLabel()
-        self.inp_epsg_info = QtWidgets.QLabel()
-        self.txt_null = QtWidgets.QLineEdit()
-        self.dsb_tlx = QtWidgets.QLineEdit()
-        self.dsb_tly = QtWidgets.QLineEdit()
-        self.dsb_xdim = QtWidgets.QLineEdit()
-        self.dsb_ydim = QtWidgets.QLineEdit()
-        self.led_units = QtWidgets.QLineEdit()
-        self.lbl_min = QtWidgets.QLabel()
-        self.lbl_max = QtWidgets.QLabel()
-        self.lbl_mean = QtWidgets.QLabel()
 
-        self.proj = GroupProj('Input Projection')
+        self.ofilt = QtWidgets.QComboBox()
+        self.odir = QtWidgets.QLineEdit('')
+        self.red = QtWidgets.QComboBox()
+        self.green = QtWidgets.QComboBox()
+        self.blue = QtWidgets.QComboBox()
+        self.sunshade = QtWidgets.QComboBox()
+        self.slvl = QtWidgets.QComboBox()
+        self.ternary = QtWidgets.QCheckBox('Ternary Export')
 
         self.setupui()
 
     def setupui(self):
         """
         Set up UI.
 
         Returns
         -------
         None.
 
         """
         gridlayout_main = QtWidgets.QGridLayout(self)
         buttonbox = QtWidgets.QDialogButtonBox()
-        groupbox = QtWidgets.QGroupBox('Dataset')
+        helpdocs = menu_default.HelpButton('pygmi.rsense.iodefs.exportbatch')
+        label_ofilt = QtWidgets.QLabel('Output Format:')
+        label_red = QtWidgets.QLabel('Red Band:')
+        label_green = QtWidgets.QLabel('Green Band:')
+        label_blue = QtWidgets.QLabel('Blue Band:')
+        label_shade = QtWidgets.QLabel('Sunshade Band:')
+        label_slvl = QtWidgets.QLabel('Sunshade Level:')
+        pb_odir = QtWidgets.QPushButton('Output Directory')
+
+        ext = ('GeoTiff', 'GeoTiff compressed using DEFLATE',
+               'GeoTiff compressed using ZSTD', 'ENVI', 'ERMapper',
+               'ERDAS Imagine')
+
+        self.ofilt.addItems(ext)
+        self.ofilt.setCurrentText('GeoTiff compressed using DEFLATE')
+        self.slvl.addItems(['Standard', 'Heavy'])
+        self.slvl.setCurrentText('Standard')
+
+        self.ternary.setChecked(False)
+        self.red.setEnabled(False)
+        self.green.setEnabled(False)
+        self.blue.setEnabled(False)
+        self.sunshade.setEnabled(False)
+        self.slvl.setEnabled(False)
 
-        gridlayout = QtWidgets.QGridLayout(groupbox)
-        label_tlx = QtWidgets.QLabel('Top Left X Coordinate:')
-        label_tly = QtWidgets.QLabel('Top Left Y Coordinate:')
-        label_xdim = QtWidgets.QLabel('X Dimension:')
-        label_ydim = QtWidgets.QLabel('Y Dimension:')
-        label_null = QtWidgets.QLabel('Null/Nodata value:')
-        label_rows = QtWidgets.QLabel('Rows:')
-        label_cols = QtWidgets.QLabel('Columns:')
-        label_min = QtWidgets.QLabel('Dataset Minimum:')
-        label_max = QtWidgets.QLabel('Dataset Maximum:')
-        label_mean = QtWidgets.QLabel('Dataset Mean:')
-        label_units = QtWidgets.QLabel('Dataset Units:')
-        label_bandid = QtWidgets.QLabel('Band Name:')
-
-        sizepolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred,
-                                           QtWidgets.QSizePolicy.Expanding)
-        groupbox.setSizePolicy(sizepolicy)
         buttonbox.setOrientation(QtCore.Qt.Horizontal)
         buttonbox.setCenterButtons(True)
         buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
 
-        self.setWindowTitle('Dataset Metadata')
+        self.setWindowTitle(r'Export File List')
 
-        gridlayout_main.addWidget(label_bandid, 0, 0, 1, 1)
-        gridlayout_main.addWidget(self.combobox_bandid, 0, 1, 1, 3)
-        gridlayout_main.addWidget(self.pb_rename_id, 1, 1, 1, 3)
-        gridlayout_main.addWidget(groupbox, 2, 0, 1, 2)
-        gridlayout_main.addWidget(self.proj, 2, 2, 1, 2)
-        gridlayout_main.addWidget(buttonbox, 4, 0, 1, 4)
-
-        gridlayout.addWidget(label_tlx, 0, 0, 1, 1)
-        gridlayout.addWidget(self.dsb_tlx, 0, 1, 1, 1)
-        gridlayout.addWidget(label_tly, 1, 0, 1, 1)
-        gridlayout.addWidget(self.dsb_tly, 1, 1, 1, 1)
-        gridlayout.addWidget(label_xdim, 2, 0, 1, 1)
-        gridlayout.addWidget(self.dsb_xdim, 2, 1, 1, 1)
-        gridlayout.addWidget(label_ydim, 3, 0, 1, 1)
-        gridlayout.addWidget(self.dsb_ydim, 3, 1, 1, 1)
-        gridlayout.addWidget(label_null, 4, 0, 1, 1)
-        gridlayout.addWidget(self.txt_null, 4, 1, 1, 1)
-        gridlayout.addWidget(label_rows, 5, 0, 1, 1)
-        gridlayout.addWidget(self.lbl_rows, 5, 1, 1, 1)
-        gridlayout.addWidget(label_cols, 6, 0, 1, 1)
-        gridlayout.addWidget(self.lbl_cols, 6, 1, 1, 1)
-        gridlayout.addWidget(label_min, 7, 0, 1, 1)
-        gridlayout.addWidget(self.lbl_min, 7, 1, 1, 1)
-        gridlayout.addWidget(label_max, 8, 0, 1, 1)
-        gridlayout.addWidget(self.lbl_max, 8, 1, 1, 1)
-        gridlayout.addWidget(label_mean, 9, 0, 1, 1)
-        gridlayout.addWidget(self.lbl_mean, 9, 1, 1, 1)
-        gridlayout.addWidget(label_units, 10, 0, 1, 1)
-        gridlayout.addWidget(self.led_units, 10, 1, 1, 1)
+        gridlayout_main.addWidget(self.odir, 0, 0, 1, 1)
+        gridlayout_main.addWidget(pb_odir, 0, 1, 1, 1)
 
-        buttonbox.accepted.connect(self.accept)
-        buttonbox.rejected.connect(self.reject)
+        gridlayout_main.addWidget(label_ofilt, 1, 0, 1, 1)
+        gridlayout_main.addWidget(self.ofilt, 1, 1, 1, 1)
 
-        self.combobox_bandid.currentIndexChanged.connect(self.update_vals)
-        self.pb_rename_id.clicked.connect(self.rename_id)
+        gridlayout_main.addWidget(self.ternary, 2, 0, 1, 2)
 
-    def acceptall(self):
-        """
-        Accept option.
+        gridlayout_main.addWidget(label_red, 3, 0, 1, 1)
+        gridlayout_main.addWidget(self.red, 3, 1, 1, 1)
 
-        Returns
-        -------
-        None.
+        gridlayout_main.addWidget(label_green, 4, 0, 1, 1)
+        gridlayout_main.addWidget(self.green, 4, 1, 1, 1)
 
-        """
-        wkt = self.proj.wkt
+        gridlayout_main.addWidget(label_blue, 5, 0, 1, 1)
+        gridlayout_main.addWidget(self.blue, 5, 1, 1, 1)
 
-        self.update_vals()
-        for tmp in self.indata['Raster']:
-            for j in self.dataid.items():
-                if j[1] == tmp.dataid:
-                    i = self.banddata[j[0]]
-                    tmp.dataid = j[0]
-                    tmp.set_transform(transform=i.transform)
-                    tmp.nodata = i.nodata
-                    if wkt == 'None':
-                        tmp.crs = None
-                    else:
-                        tmp.crs = CRS.from_wkt(wkt)
-                    tmp.units = i.units
-                    tmp.data.mask = (tmp.data.data == i.nodata)
+        gridlayout_main.addWidget(label_shade, 6, 0, 1, 1)
+        gridlayout_main.addWidget(self.sunshade, 6, 1, 1, 1)
 
-    def rename_id(self):
-        """
-        Rename the band name.
+        gridlayout_main.addWidget(label_slvl, 7, 0, 1, 1)
+        gridlayout_main.addWidget(self.slvl, 7, 1, 1, 1)
 
-        Returns
-        -------
-        None.
+        gridlayout_main.addWidget(helpdocs, 8, 0, 1, 1)
+        gridlayout_main.addWidget(buttonbox, 8, 1, 1, 3)
 
-        """
-        ctxt = str(self.combobox_bandid.currentText())
-        (skey, isokay) = QtWidgets.QInputDialog.getText(
-            self.parent, 'Rename Band Name',
-            'Please type in the new name for the band',
-            QtWidgets.QLineEdit.Normal, ctxt)
-
-        if isokay:
-            self.combobox_bandid.currentIndexChanged.disconnect()
-            indx = self.combobox_bandid.currentIndex()
-            txt = self.combobox_bandid.itemText(indx)
-            self.banddata[skey] = self.banddata.pop(txt)
-            self.dataid[skey] = self.dataid.pop(txt)
-            self.oldtxt = skey
-            self.combobox_bandid.setItemText(indx, skey)
-            self.combobox_bandid.currentIndexChanged.connect(self.update_vals)
+        buttonbox.accepted.connect(self.accept)
+        buttonbox.rejected.connect(self.reject)
+        pb_odir.pressed.connect(self.get_odir)
+        self.ternary.clicked.connect(self.click_ternary)
 
-    def update_vals(self):
+    def click_ternary(self):
         """
-        Update the values on the interface.
+        Click ternary event.
 
         Returns
         -------
         None.
 
         """
-        odata = self.banddata[self.oldtxt]
-        odata.units = self.led_units.text()
-
-        try:
-            odata.nodata = float(self.txt_null.text())
-            left = float(self.dsb_tlx.text())
-            top = float(self.dsb_tly.text())
-            xdim = float(self.dsb_xdim.text())
-            ydim = float(self.dsb_ydim.text())
-
-            odata.set_transform(xdim, left, ydim, top)
+        if self.ternary.isChecked():
+            self.red.setEnabled(True)
+            self.green.setEnabled(True)
+            self.blue.setEnabled(True)
+            self.ofilt.setCurrentText('GeoTiff')
+            self.ofilt.setEnabled(False)
+            self.sunshade.setEnabled(True)
+            self.slvl.setEnabled(True)
 
-        except ValueError:
-            self.showprocesslog('Value error - abandoning changes')
-
-        indx = self.combobox_bandid.currentIndex()
-        txt = self.combobox_bandid.itemText(indx)
-        self.oldtxt = txt
-        idata = self.banddata[txt]
-
-        irows = idata.data.shape[0]
-        icols = idata.data.shape[1]
-
-        self.lbl_cols.setText(str(icols))
-        self.lbl_rows.setText(str(irows))
-        self.txt_null.setText(str(idata.nodata))
-        self.dsb_tlx.setText(str(idata.extent[0]))
-        self.dsb_tly.setText(str(idata.extent[-1]))
-        self.dsb_xdim.setText(str(idata.xdim))
-        self.dsb_ydim.setText(str(idata.ydim))
-        self.lbl_min.setText(str(idata.data.min()))
-        self.lbl_max.setText(str(idata.data.max()))
-        self.lbl_mean.setText(str(idata.data.mean()))
-        self.led_units.setText(str(idata.units))
+        else:
+            self.red.setEnabled(False)
+            self.green.setEnabled(False)
+            self.blue.setEnabled(False)
+            self.ofilt.setEnabled(True)
+            self.sunshade.setEnabled(False)
+            self.slvl.setEnabled(False)
 
     def run(self):
         """
-        Entry point to start this routine.
+        Run.
 
         Returns
         -------
-        tmp : bool
+        bool
             True if successful, False otherwise.
 
         """
-        bandid = []
-        if self.indata['Raster'][0].crs is None:
-            self.proj.set_current('None')
-        else:
-            self.proj.set_current(self.indata['Raster'][0].crs.wkt)
-
-        for i in self.indata['Raster']:
-            bandid.append(i.dataid)
-            self.banddata[i.dataid] = Data()
-            tmp = self.banddata[i.dataid]
-            self.dataid[i.dataid] = i.dataid
-            tmp.data = i.data
-            tmp.set_transform(transform=i.transform)
-            tmp.nodata = i.nodata
-            tmp.crs = i.crs
-            tmp.units = i.units
-
-        self.combobox_bandid.currentIndexChanged.disconnect()
-        self.combobox_bandid.addItems(bandid)
-        indx = self.combobox_bandid.currentIndex()
-        self.oldtxt = self.combobox_bandid.itemText(indx)
-        self.combobox_bandid.currentIndexChanged.connect(self.update_vals)
-
-        idata = self.banddata[self.oldtxt]
-
-        irows = idata.data.shape[0]
-        icols = idata.data.shape[1]
-
-        self.lbl_cols.setText(str(icols))
-        self.lbl_rows.setText(str(irows))
-        self.txt_null.setText(str(idata.nodata))
-        self.dsb_tlx.setText(str(idata.extent[0]))
-        self.dsb_tly.setText(str(idata.extent[-1]))
-        self.dsb_xdim.setText(str(idata.xdim))
-        self.dsb_ydim.setText(str(idata.ydim))
-        self.lbl_min.setText(str(idata.data.min()))
-        self.lbl_max.setText(str(idata.data.max()))
-        self.lbl_mean.setText(str(idata.data.mean()))
-        self.led_units.setText(str(idata.units))
+        self.process_is_active(True)
 
-        self.update_vals()
-
-        tmp = self.exec_()
-
-        if tmp != 1:
+        if 'RasterFileList' not in self.indata:
+            self.showlog('No raster file list')
+            self.process_is_active(False)
             return False
 
-        self.acceptall()
-
-        return True
+        dat = self.indata['RasterFileList'][0]
+        bnames = dat.tnames
 
+        bnames = natsorted(bnames)
 
-class Continuation(BasicModule):
-    """Perform upward and downward continuation on potential field data."""
+        if 'Explained Variance Ratio' in bnames[0]:
+            bnames = [i.split('Explained Variance Ratio')[0] for i in bnames]
 
-    def __init__(self, parent=None):
-        super().__init__(parent)
-        self.dataid = QtWidgets.QComboBox()
-        self.continuation = QtWidgets.QComboBox()
-        self.dsb_height = QtWidgets.QDoubleSpinBox()
+        self.red.addItems(bnames)
+        self.green.addItems(bnames)
+        self.blue.addItems(bnames)
+        self.sunshade.addItems(['None', 'External File (first band)']+bnames)
 
-        self.setupui()
-
-    def setupui(self):
-        """
-        Set up UI.
-
-        Returns
-        -------
-        None.
-
-        """
-        gridlayout_main = QtWidgets.QGridLayout(self)
-        buttonbox = QtWidgets.QDialogButtonBox()
-        helpdocs = menu_default.HelpButton('pygmi.raster.dataprep.cont')
-        label_band = QtWidgets.QLabel('Band to perform continuation:')
-        label_cont = QtWidgets.QLabel('Continuation type:')
-        label_height = QtWidgets.QLabel('Continuation distance:')
-
-        self.dsb_height.setMaximum(1000000.0)
-        self.dsb_height.setMinimum(0.0)
-        self.dsb_height.setValue(0.0)
-        self.continuation.clear()
-        self.continuation.addItems(['Upward', 'Downward'])
-
-        buttonbox.setOrientation(QtCore.Qt.Horizontal)
-        buttonbox.setCenterButtons(True)
-        buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
-
-        self.setWindowTitle('Continuation')
-
-        gridlayout_main.addWidget(label_band, 0, 0, 1, 1)
-        gridlayout_main.addWidget(self.dataid, 0, 1, 1, 1)
-
-        gridlayout_main.addWidget(label_cont, 1, 0, 1, 1)
-        gridlayout_main.addWidget(self.continuation, 1, 1, 1, 1)
-        gridlayout_main.addWidget(label_height, 2, 0, 1, 1)
-        gridlayout_main.addWidget(self.dsb_height, 2, 1, 1, 1)
-        gridlayout_main.addWidget(helpdocs, 3, 0, 1, 1)
-        gridlayout_main.addWidget(buttonbox, 3, 1, 1, 3)
-
-        buttonbox.accepted.connect(self.accept)
-        buttonbox.rejected.connect(self.reject)
-
-    def settings(self, nodialog=False):
-        """
-        Entry point into item.
-
-        Parameters
-        ----------
-        nodialog : bool, optional
-            Run settings without a dialog. The default is False.
-
-        Returns
-        -------
-        bool
-            True if successful, False otherwise.
+        tmp = self.exec_()
 
-        """
-        tmp = []
-        if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+        if tmp != 1 or self.odir.text() == '':
             return False
 
-        for i in self.indata['Raster']:
-            tmp.append(i.dataid)
-
-        self.dataid.clear()
-        self.dataid.addItems(tmp)
-
-        if not nodialog:
-            tmp = self.exec_()
-
-            if tmp != 1:
-                return False
+        filt = self.ofilt.currentText()
+        odir = self.odir.text()
+        sunfile = None
+
+        if self.ternary.isChecked():
+            tnames = [self.red.currentText(),
+                      self.green.currentText(),
+                      self.blue.currentText()]
+            otype = 'RGB'
+            sunfile = self.sunshade.currentText()
+            slevel = self.slvl.currentText()
+            if slevel == 'Standard':
+                cell = 25.
+                alpha = .75
+            else:
+                cell = 1.
+                alpha = .99
 
-        self.acceptall()
+            if sunfile == 'External File (first band)':
+                ext = ('Common formats (*.ers *.hdr *.tif *.tiff *.sdat *.img '
+                       '*.pix *.bil);;')
+
+                sunfile, _ = QtWidgets.QFileDialog.getOpenFileName(
+                    self.parent, 'Open File', '.', ext)
+                if sunfile == '':
+                    return False
+        else:
+            otype = None
+            tnames = None
+            slevel = None
+            cell = 25.
+            alpha = .75
+
+        self.showlog('Export Data Busy...')
+
+        export_batch(self.indata, odir, filt, tnames, piter=self.piter,
+                     showlog=self.showlog, otype=otype, sunfile=sunfile,
+                     cell=cell, alpha=alpha)
 
+        self.showlog('Export Data Finished!')
+        self.process_is_active(False)
         return True
 
-    def loadproj(self, projdata):
+    def get_odir(self, odir=''):
         """
-        Load project data into class.
+        Get output directory.
 
         Parameters
         ----------
-        projdata : dictionary
-            Project data loaded from JSON project file.
-
-        Returns
-        -------
-        chk : bool
-            A check to see if settings was successfully run.
-
-        """
-        self.dataid.setCurrentText(projdata['band'])
-        self.continuation.setCurrenText(projdata['ctype'])
-        self.dsb_height.setValue(projdata['height'])
-
-        return False
-
-    def saveproj(self):
-        """
-        Save project data from class.
-
-        Returns
-        -------
-        projdata : dictionary
-            Project data to be saved to JSON project file.
-
-        """
-        projdata = {}
-
-        projdata['band'] = self.dataid.currentText()
-        projdata['ctype'] = self.continuation.currentText()
-        projdata['height'] = self.dsb_height.value()
-
-        return projdata
-
-    def acceptall(self):
-        """
-        Accept option.
-
-        Updates self.outdata, which is used as input to other modules.
+        odir : str, optional
+            Output directory submitted for testing. The default is ''.
 
         Returns
         -------
         None.
 
         """
-        h = self.dsb_height.value()
-        ctype = self.continuation.currentText()
+        if odir == '':
+            odir = QtWidgets.QFileDialog.getExistingDirectory(
+                self.parent, 'Select Output Directory')
 
-        # Get data
-        for i in self.indata['Raster']:
-            if i.dataid == self.dataid.currentText():
-                data = i
-                break
-
-        if ctype == 'Downward':
-            dat = taylorcont(data, h)
-        else:
-            dat = fftcont(data, h)
+            if odir == '':
+                return
 
-        self.outdata['Raster'] = [dat]
+        self.odir.setText(odir)
 
 
-def redistribute_vertices(geom, distance):
+def calculate_toa(dat, showlog=print):
     """
-    Redistribute vertices in a geometry.
+    Top of atmosphere correction.
 
-    From https://stackoverflow.com/questions/34906124/interpolating-every-x-distance-along-multiline-in-shapely,
-    and by Mike-T.
+    Includes VNIR, SWIR and TIR bands.
 
     Parameters
     ----------
-    geom : shapely geometry
-        Geometry from geopandas.
-    distance : float
-        sampling distance.
-
-    Raises
-    ------
-    ValueError
-        Error when there is an unknown geometry.
+    dat : Data
+        PyGMI raster dataset
+    showlog : function, optional
+        Routine to show text messages. The default is print.
 
     Returns
     -------
-    shapely geometry
-        New geometry.
-
-    """
-    if geom.geom_type == 'LineString':
-        num_vert = int(round(geom.length / distance))
-        if num_vert == 0:
-            num_vert = 1
-        return LineString(
-            [geom.interpolate(float(n) / num_vert, normalized=True)
-             for n in range(num_vert + 1)])
-    if geom.geom_type == 'MultiLineString':
-        parts = [redistribute_vertices(part, distance)
-                 for part in geom]
-        return type(geom)([p for p in parts if not p.is_empty])
-    raise ValueError('unhandled geometry %s', (geom.geom_type,))
-
-
-def data_reproject(data, icrs, ocrs, otransform, orows, ocolumns):
+    out : Data
+        PyGMI raster dataset
     """
-    Reproject dataset.
+    showlog('Calculating top of atmosphere...')
 
-    Parameters
-    ----------
-    data : PyGMI Data
-        PyGMI dataset.
-    icrs : CRS
-        input crs.
-    ocrs : CRS
-        output crs.
-    otransform : Affine
-        Output affine transform.
-    orows : int
-        output rows.
-    ocolumns : int
-        output columns.
-
-    Returns
-    -------
-    data2 : TYPE
-        DESCRIPTION.
-
-    """
-    odata = np.zeros((orows, ocolumns), dtype=data.data.dtype)
-    odata, _ = reproject(source=data.data,
-                         destination=odata,
-                         src_transform=data.transform,
-                         src_crs=icrs,
-                         dst_transform=otransform,
-                         dst_crs=ocrs,
-                         src_nodata=data.nodata)
-
-    data2 = Data()
-    data2.data = odata
-    data2.crs = ocrs
-    data2.set_transform(transform=otransform)
-    data2.data = data2.data.astype(data.data.dtype)
-    data2.dataid = data.dataid
-    data2.wkt = CRS.to_wkt(ocrs)
-
-    data2.data = np.ma.masked_equal(data2.data, data.nodata)
-    data2.nodata = data.nodata
+    datanew = {}
+    for datai in dat:
+        datanew[datai.dataid.split()[1]] = copy.deepcopy(datai)
+
+    out = []
+    for i in range(len(dat)):
+        idtmp = 'ImageData'+str(i+1)
+        if i+1 == 3:
+            idtmp += 'N'
+        datai = datanew[idtmp]
+
+        gain = datai.metadata['Gain']
+        sunelev = datai.metadata['SolarElev']
+        jday = datai.metadata['JulianDay']
+
+        lrad = (datai.data-1)*gain
+
+        if i < 9:
+            theta = np.deg2rad(90-sunelev)
+            datai.data = np.pi*lrad*EDIST[jday]**2/(ESUN[i]*np.cos(theta))
+        else:
+            datai.data = K2[i-9]/np.log(K1[i-9]/lrad+1)
+        datai.data.set_fill_value(datai.nodata)
+        dmask = datai.data.mask
+        datai.data = np.ma.array(datai.data.filled(), mask=dmask)
+        out.append(datai)
 
-    return data2
+    return out
 
 
-def merge_median(merged_data, new_data, merged_mask, new_mask, index=None,
-                 roff=None, coff=None):
+def consolidate_aster_list(flist):
     """
-    Merge using median for rasterio, taking minimum value.
+    Consolidate ASTER files from a file list, getting rid of extra files.
 
     Parameters
     ----------
-    merged_data : numpy array
-        Old data.
-    new_data : numpy array
-        New data to merge to old data.
-    merged_mask : float
-        Old mask.
-    new_mask : float
-        New mask.
-    index : int, optional
-        index of the current dataset within the merged dataset collection.
-        The default is None.
-    roff : int, optional
-        row offset in base array. The default is None.
-    coff : int, optional
-        col offset in base array. The default is None.
+    flist : list
+        List of filenames.
 
     Returns
     -------
-    None.
+    flist : list
+        List of filenames.
 
     """
-    merged_data = np.ma.array(merged_data, mask=merged_mask)
-    new_data = np.ma.array(new_data, mask=new_mask)
-
-    mtmp1 = np.logical_and(~merged_mask, ~new_mask)
-    mtmp2 = np.logical_and(~merged_mask, new_mask)
+    asterhfiles = []
+    asterzfiles = []
+    otherfiles = []
+
+    for ifile in flist:
+        bfile = os.path.basename(ifile)
+        ext = os.path.splitext(ifile)[1].lower()
+
+        if 'AST_' in bfile and ext == '.hdf':
+            asterhfiles.append(ifile)
+        if 'AST_' in bfile and ext == '.zip':
+            asterzfiles.append(ifile)
+        else:
+            otherfiles.append(ifile)
 
-    tmp1 = new_data.copy()
+    asterfiles = []
+    tmp = {}
 
-    if True in mtmp1:
-        tmp1 = tmp1 - np.ma.median(new_data[mtmp1])
-        tmp1 = tmp1 + np.ma.median(merged_data[mtmp1])
-        # tmp1 = tmp1 - new_data[mtmp1].mean()
-        # tmp1 = tmp1 + merged_data[mtmp1].mean()
+    for ifile in asterzfiles:
+        adate = os.path.basename(ifile).split('_')[2]
+        tmp[adate] = ifile
+    asterfiles += list(tmp.values())
 
-    tmp1[mtmp2] = merged_data[mtmp2]
+    for ifile in asterhfiles:
+        adate = os.path.basename(ifile).split('_')[2]
+        tmp[adate] = ifile
 
-    # import matplotlib.pyplot as plt
+    asterfiles += list(tmp.values())
 
-    # plt.figure(dpi=150)
-    # plt.suptitle(f'{roff} {coff}')
-    # plt.subplot(221)
-    # plt.title('merged_data')
-    # plt.imshow(merged_data[0], vmin=0.5, vmax=3.0, interpolation='nearest')
-    # plt.colorbar()
-
-    # plt.subplot(222)
-    # plt.title('new_data')
-    # plt.imshow(new_data[0], vmin=0.5, vmax=3.0, interpolation='nearest')
-    # plt.colorbar()
-    # plt.tight_layout()
-
-    # plt.subplot(223)
-    # plt.title('tmp1')
-    # plt.imshow(tmp1[0], vmin=0.5, vmax=3.0, interpolation='nearest')
-    # plt.colorbar()
-    # plt.tight_layout()
-    # plt.show()
+    flist = asterfiles+otherfiles
 
-    merged_data[:] = tmp1
+    return flist
 
 
-def merge_min(merged_data, new_data, merged_mask, new_mask, index=None,
-              roff=None, coff=None):
+def etree_to_dict(t):
     """
-    Merge using minimum for rasterio, taking minimum value.
+    Convert an ElementTree to dictionary.
+
+    From K3--rnc: https://stackoverflow.com/questions/7684333/converting-xml-to-dictionary-using-elementtree
 
     Parameters
     ----------
-    merged_data : numpy array
-        Old data.
-    new_data : numpy array
-        New data to merge to old data.
-    merged_mask : float
-        Old mask.
-    new_mask : float
-        New mask.
-    index : int, optional
-        index of the current dataset within the merged dataset collection.
-        The default is None.
-    roff : int, optional
-        row offset in base array. The default is None.
-    coff : int, optional
-        col offset in base array. The default is None.
+    t : Elementtree
+        Root.
 
     Returns
     -------
-    None.
+    d : dictionary
+        DESCRIPTION.
 
     """
-    tmp = np.logical_and(~merged_mask, ~new_mask)
-
-    tmp1 = merged_data.copy()
-    tmp1[~new_mask] = new_data[~new_mask]
-    tmp1[tmp] = np.minimum(merged_data[tmp], new_data[tmp])
-
-    merged_data[:] = tmp1
+    d = {t.tag: {} if t.attrib else None}
+    children = list(t)
+    if children:
+        dd = defaultdict(list)
+        for dc in map(etree_to_dict, children):
+            for k, v in dc.items():
+                dd[k].append(v)
+        d = {t.tag: {k: v[0] if len(v) == 1 else v
+                     for k, v in dd.items()}}
+    if t.attrib:
+        d[t.tag].update(('@' + k, v)
+                        for k, v in t.attrib.items())
+    if t.text:
+        text = t.text.strip()
+        if children or t.attrib:
+            if text:
+                d[t.tag]['#text'] = text
+        else:
+            d[t.tag] = text
+    return d
 
 
-def merge_max(merged_data, new_data, merged_mask, new_mask, index=None,
-              roff=None, coff=None):
+def export_batch(indata, odir, filt, tnames=None, piter=None,
+                 showlog=print, otype=None, sunfile=None,
+                 cell=25., alpha=.75):
     """
-    Merge using maximum for rasterio, taking maximum value.
+    Export a batch of files directly from satellite format to disk.
 
     Parameters
     ----------
-    merged_data : numpy array
-        Old data.
-    new_data : numpy array
-        New data to merge to old data.
-    merged_mask : float
-        Old mask.
-    new_mask : float
-        New mask.
-    index : int, optional
-        index of the current dataset within the merged dataset collection.
-        The default is None.
-    roff : int, optional
-        row offset in base array. The default is None.
-    coff : int, optional
-        col offset in base array. The default is None.
+    indata : dictionary
+        Dictionary containing 'RasterFileList' as one of its keys.
+    odir : str
+        Output Directory.
+    filt : str
+        type of file to export.
+    tnames : list, optional
+        list of band names to import, in order. the default is None.
+    piter : iter, optional
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    otype : str
+        output type of file, regular or RGB ternary (with possible sunshading)
+    sunfile : str
+        either a filename of an external file to be used for sunshading, or an
+        existing band name. the default is None.
+    cell : float
+        Between 1 and 100 - controls sunshade detail. The default is 25.
+    alpha : float
+        How much incident light is reflected (0 to 1). The default is .75.
 
     Returns
     -------
     None.
 
     """
-    tmp = np.logical_and(~merged_mask, ~new_mask)
-
-    tmp1 = merged_data.copy()
-    tmp1[~new_mask] = new_data[~new_mask]
-    tmp1[tmp] = np.maximum(merged_data[tmp], new_data[tmp])
+    if 'RasterFileList' not in indata:
+        showlog('You need a raster file list')
+        return
+
+    ifiles = indata['RasterFileList']
+
+    if sunfile == 'None':
+        sunfile = None
+    elif tnames is not None and otype == 'RGB':
+        if sunfile in ifiles[0].bands and sunfile not in tnames:
+            tnames += [sunfile]
+
+    filt2gdal = {'GeoTiff compressed using ZSTD': 'GTiff',
+                 'GeoTiff compressed using DEFLATE': 'GTiff',
+                 'GeoTiff': 'GTiff',
+                 'ENVI': 'ENVI',
+                 'ERMapper': 'ERS',
+                 'ERDAS Imagine': 'HFA'}
+
+    compression = 'NONE'
+    ofilt = filt2gdal[filt]
+    if filt == 'GeoTiff compressed using ZSTD':
+        compression = 'ZSTD'
+    elif filt == 'GeoTiff compressed using DEFLATE':
+        compression = 'DEFLATE'
 
-    merged_data[:] = tmp1
+    os.makedirs(odir, exist_ok=True)
 
+    for ifile in ifiles:
+        dat = get_from_rastermeta(ifile, piter=piter,
+                                  showlog=showlog,
+                                  tnames=tnames)
+
+        ofile = set_export_filename(dat, odir, otype)
+
+        odat = []
+        if tnames is not None:
+            for i in tnames:
+                for j in dat:
+                    if i == j.dataid:
+                        odat.append(j)
+                        break
+        else:
+            odat = dat
+        showlog('Exporting '+os.path.basename(ofile))
 
-def fftprep(data):
-    """
-    FFT preparation.
-
-    Parameters
-    ----------
-    data : PyGMI Data type
-        Input dataset.
+        if otype == 'RGB':
+            odat = get_ternary(odat, sunfile=sunfile, cell=cell, alpha=alpha,
+                               piter=piter, showlog=showlog)
+            export_raster(ofile, odat, 'GTiff', piter=piter,
+                          bandsort=False, updatestats=False,
+                          showlog=showlog)
+        else:
+            export_raster(ofile, odat, ofilt, piter=piter,
+                          compression=compression, showlog=showlog)
 
-    Returns
-    -------
-    zfin : numpy array.
-        Output prepared data.
-    rdiff : int
-        rows divided by 2.
-    cdiff : int
-        columns divided by 2.
-    datamedian : float
-        Median of data.
 
+def get_data(ifile, piter=None, showlog=print, tnames=None,
+             metaonly=False):
     """
-    datamedian = np.ma.median(data.data)
-    ndat = data.data - datamedian
-
-    nr, nc = data.data.shape
-    cdiff = nc//2
-    rdiff = nr//2
-
-    z1 = np.zeros((nr+2*rdiff, nc+2*cdiff))+np.nan
-    x1, y1 = np.mgrid[0: nr+2*rdiff, 0: nc+2*cdiff]
-    z1[rdiff:-rdiff, cdiff:-cdiff] = ndat.filled(np.nan)
+    Load a raster dataset off the disk using the rasterio libraries.
 
-    for j in range(2):
-        z1[0] = 0
-        z1[-1] = 0
-        z1[:, 0] = 0
-        z1[:, -1] = 0
-
-        vert = np.zeros_like(z1)
-        hori = np.zeros_like(z1)
-
-        for i in range(z1.shape[0]):
-            mask = ~np.isnan(z1[i])
-            y = y1[i][mask]
-            z = z1[i][mask]
-            hori[i] = np.interp(y1[i], y, z)
-
-        for i in range(z1.shape[1]):
-            mask = ~np.isnan(z1[:, i])
-            x = x1[:, i][mask]
-            z = z1[:, i][mask]
-
-            vert[:, i] = np.interp(x1[:, i], x, z)
-
-        hori[hori == 0] = np.nan
-        vert[vert == 0] = np.nan
-
-        hv = hori.copy()
-        hv[np.isnan(hori)] = vert[np.isnan(hori)]
-        hv[~np.isnan(hv)] = np.nanmean([hori[~np.isnan(hv)],
-                                        vert[~np.isnan(hv)]], 0)
-
-        z1[np.isnan(z1)] = hv[np.isnan(z1)]
-
-    zfin = z1
-
-    nr, nc = zfin.shape
-    zfin *= tukey(nc)
-    zfin *= tukey(nr)[:, np.newaxis]
-
-    return zfin, rdiff, cdiff, datamedian
-
-
-def fft_getkxy(fftmod, xdim, ydim):
-    """
-    Get KX and KY.
+    It returns the data in a PyGMI data object.
 
     Parameters
     ----------
-    fftmod : numpy array
-        FFT data.
-    xdim : float
-        cell x dimension.
-    ydim : float
-        cell y dimension.
+    ifile : str
+        filename to import
+    piter : iter, optional
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    tnames : list, optional
+        list of band names to import, in order. The default is None.
+    metaonly : bool, optional
+        Retrieve only the metadata for the file. The default is False.
 
     Returns
     -------
-    KX : numpy array
-        x sample frequencies.
-    KY : numpy array
-        y sample frequencies.
-
+    dat : PyGMI raster Data
+        dataset imported
     """
-    ny, nx = fftmod.shape
-    kx = np.fft.fftfreq(nx, xdim)*2*np.pi
-    ky = np.fft.fftfreq(ny, ydim)*2*np.pi
+    ifile = ifile[:]
+    bfile = os.path.basename(ifile)
+    ext = os.path.splitext(ifile)[1].lower()
+
+    showlog('Importing', bfile)
+    dtree = {}
+    if '.xml' in bfile.lower():
+        dtree = etree_to_dict(ET.parse(ifile).getroot())
+
+    if 'AST_' in bfile and ext == '.hdf':
+        idir = os.path.dirname(ifile)
+        adate = os.path.basename(ifile).split('_')[2]
+        ifiles = glob.glob(os.path.join(idir, '*'+adate+'*.hdf'))
+        dat = []
+        for afile in ifiles:
+            dat += get_aster_hdf(afile, piter, showlog, tnames, metaonly)
+    elif 'AST_' in bfile and ext == '.zip':
+        idir = os.path.dirname(ifile)
+        adate = os.path.basename(ifile).split('_')[2]
+        ifiles = glob.glob(os.path.join(idir, '*'+adate+'*.zip'))
+        dat = []
+        for afile in ifiles:
+            dat += get_aster_zip(afile, piter, showlog, tnames, metaonly)
+    elif (bfile[:4] in ['LT04', 'LT05', 'LE07', 'LC08', 'LM05', 'LC09'] and
+          ('.tar' in bfile.lower() or '_MTL.txt' in bfile)):
+        dat = get_landsat(ifile, piter, showlog, tnames, metaonly)
+    elif ((ext == '.xml' and '.SAFE' in ifile) or
+          ('S2A_' in bfile and ext == '.zip') or
+          ('S2B_' in bfile and ext == '.zip')):
+        dat = get_sentinel2(ifile, piter, showlog, tnames, metaonly)
+    elif (('MOD' in bfile or 'MCD' in bfile) and ext == '.hdf' and
+          '.006.' in bfile):
+        dat = get_modisv6(ifile, piter, showlog, tnames, metaonly)
+    elif 'AG1' in bfile and ext == '.h5':
+        dat = get_aster_ged(ifile, piter, showlog, tnames, metaonly)
+    elif ext == '.zip' and 'EO1H' in bfile:
+        dat = get_hyperion(ifile, piter, showlog, tnames, metaonly)
+    elif ext == '.xml' and 'isd' in dtree:
+        dat = get_worldview(ifile, piter, showlog, tnames, metaonly)
+    else:
+        dat = get_raster(ifile, piter=piter, showlog=showlog,
+                         tnames=tnames, metaonly=metaonly)
 
-    KX, KY = np.meshgrid(kx, ky)
-    KY = -KY
-    return KX, KY
+    if dat is not None:
+        for i in dat:
+            if i.dataid is None:
+                i.dataid = ''
+            i.dataid = i.dataid.replace(',', ' ')
+
+        # Sort in band order.
+        dataid = [i.dataid for i in dat]
+        dorder = [i for _, i in natsorted(zip(dataid, range(len(dataid))))]
+        dat = [dat[i] for i in dorder]
+
+    return dat
 
 
-def verticalp(data, order=1):
+def get_from_rastermeta(ldata, piter=None, showlog=print, tnames=None):
     """
-    Vertical derivative.
+    Import data from a RasterMeta item.
 
     Parameters
     ----------
-    data : numpy array
-        Input data.
-    order : float, optional
-        Order. The default is 1.
+    ldata : RasterMeta or list
+        List of RasterMeta or single item.
+    piter : iter, optional
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    tnames : list, optional
+        list of band names to import, in order. The default is None.
 
     Returns
     -------
-    dout : numpy array
-        Output data
+    dat : list
+        List of data.
 
     """
-    xdim = data.xdim
-    ydim = data.ydim
+    if tnames is None:
+        tnames = ldata.tnames
 
-    ndat, rdiff, cdiff, _ = fftprep(data)
-    fftmod = np.fft.fft2(ndat)
+    ifile = ldata.banddata[0].filename
+    dat = get_data(ifile, piter=piter, showlog=showlog, tnames=tnames)
 
-    KX, KY = fft_getkxy(fftmod, xdim, ydim)
+    # ifiles = []
+    # for band in ldata.banddata:
+    #     ifiles.append(band.filename)
 
-    k = np.sqrt(KX**2+KY**2)
-    filt = k**order
+    # ifiles = list(set(ifiles))
 
-    zout = np.real(np.fft.ifft2(fftmod*filt))
-    zout = zout[rdiff:-rdiff, cdiff:-cdiff]
+    # dat = []
+    # for ifile in ifiles:
+    #     dat += get_data(ldata.filename, piter=piter,
+    #                     showlog=showlog, tnames=tnames)
 
-    return zout
+    if ldata.to_sutm is True:
+        dat = utm_to_south(dat)
+
+    return dat
 
 
-def fftcont(data, h):
+def get_modisv6(ifile, piter=None, showlog=print, tnames=None,
+                metaonly=False):
     """
-    Continuation.
+    Get MODIS v006 data.
 
     Parameters
     ----------
-    data : PyGMI Data
-        PyGMI raster data.
-    h : float
-        Height.
+    ifile : str
+        filename to import
+    piter : iter, optional
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    tnames : list, optional
+        list of band names to import, in order. The default is None.
+    metaonly : bool, optional
+        Retrieve only the metadata for the file. The default is False.
 
     Returns
     -------
-    dat : PyGMI Data
-        PyGMI raster data.
-
+    dat : PyGMI raster Data
+        dataset imported
     """
-    xdim = data.xdim
-    ydim = data.ydim
+    if piter is None:
+        piter = ProgressBarText().iter
 
-    ndat, rdiff, cdiff, datamedian = fftprep(data)
+    dat = []
+    ifile = ifile[:]
 
-    fftmod = np.fft.fft2(ndat)
+    with rasterio.open(ifile) as dataset:
+        if dataset is None:
+            return None
+        subdata = dataset.subdatasets
 
-    ny, nx = fftmod.shape
+    dat = []
+    lulc = None
 
-    KX, KY = fft_getkxy(fftmod, xdim, ydim)
-    k = np.sqrt(KX**2+KY**2)
+    for ifile2 in subdata:
+        dataset = rasterio.open(ifile2)
 
-    filt = np.exp(-np.abs(k)*h)
+        wkt = dataset.crs.wkt
+        crs = dataset.crs
+        if 'Sinusoidal' in wkt:
+            wkt = wkt.replace('PROJCS["unnamed"', 'PROJCS["Sinusoidal"')
+            wkt = wkt.replace('GEOGCS["Unknown datum based upon the custom '
+                              'spheroid"',
+                              'GEOGCS["GCS_Unknown"')
+            wkt = wkt.replace('DATUM["Not specified '
+                              '(based on custom spheroid)"',
+                              'DATUM["D_Unknown"')
+            wkt = wkt.replace('SPHEROID["Custom spheroid"',
+                              'SPHEROID["S_Unknown"')
+            crs = CRS.from_wkt(wkt)
+
+        meta = dataset.tags()
+        bandid = dataset.descriptions[0]
+        nval = dataset.nodata
 
-    zout = np.real(np.fft.ifft2(fftmod*filt))
-    zout = zout[rdiff:-rdiff, cdiff:-cdiff]
+        if bandid is None and ':' in ifile2:
+            bandid = ifile2[ifile2.rindex(':')+1:]
 
-    zout = zout + datamedian
+        if tnames is not None and bandid not in tnames:
+            continue
 
-    zout[data.data.mask] = data.data.fill_value
+        if 'scale_factor' in meta:
+            scale = float(meta['scale_factor'])
+        else:
+            scale = 1
 
-    dat = Data()
-    dat.data = np.ma.masked_invalid(zout)
-    dat.data.mask = np.ma.getmaskarray(data.data)
-    dat.nodata = data.data.fill_value
-    dat.dataid = 'Upward_'+str(h)+'_'+data.dataid
-    dat.set_transform(transform=data.transform)
-    dat.crs = data.crs
+        if 'MOD13' in ifile and scale > 1:
+            scale = 1./scale
 
-    return dat
+        if 'MOD44B' in ifile and '_SD' in bandid and scale == 1:
+            scale = 0.01
 
+        if 'add_offset' in meta:
+            offset = float(meta['add_offset'])
+        else:
+            offset = 0
 
-def taylorcont(data, h):
-    """
-    Continuation.
+        dat.append(Data())
+        if metaonly is False:
+            rtmp2 = dataset.read(1)
+            rtmp2 = rtmp2.astype(float)
+
+            if nval == 32767:
+                mask = (rtmp2 > 32760)
+                lulc = np.zeros_like(rtmp2)
+                lulc[mask] = rtmp2[mask]-32760
+                lulc = np.ma.masked_equal(lulc, 0)
+            else:
+                mask = (rtmp2 == nval)
 
-    Parameters
-    ----------
-    data : PyGMI Data
-        PyGMI raster data.
-    h : float
-        Height.
+            rtmp2 = rtmp2*scale+offset
+            rtmp2[mask] = 1e+20
 
-    Returns
-    -------
-    dat : PyGMI Data
-        PyGMI raster data.
+            dat[-1].data = np.ma.array(rtmp2, mask=mask)
 
-    """
-    dz = verticalp(data, order=1)
-    dz2 = verticalp(data, order=2)
-    dz3 = verticalp(data, order=3)
-    zout = (data.data + h*dz + h**2*dz2/math.factorial(2) +
-            h**3*dz3/math.factorial(3))
-
-    dat = Data()
-    dat.data = np.ma.masked_invalid(zout)
-    dat.data.mask = np.ma.getmaskarray(data.data)
-    dat.nodata = data.data.fill_value
-    dat.dataid = 'Downward_'+str(h)+'_'+data.dataid
-    dat.set_transform(transform=data.transform)
-    dat.crs = data.crs
+        dat[-1].dataid = bandid
+        dat[-1].nodata = 1e+20
+        dat[-1].meta_from_rasterio(dataset)
+        dat[-1].crs = crs
+        dat[-1].filename = ifile
+        dat[-1].units = dataset.units[0]
+        dat[-1].metadata['Raster']['Sensor'] = 'MODIS'
+
+        dataset.close()
+
+    if lulc is not None:
+        dat.append(copy.deepcopy(dat[0]))
+        dat[-1].data = lulc
+        dat[-1].dataid = ('LULC: out of earth=7, water=6, barren=5, snow=4, '
+                          'wetland=3, urban=2, unclassifed=1')
+        dat[-1].nodata = 0
+
+    showlog('Import complete')
     return dat
 
 
-def check_dataid(out):
+def get_landsat(ifilet, piter=None, showlog=print, tnames=None,
+                metaonly=False):
     """
-    Check dataid for duplicates and renames where necessary.
+    Get Landsat Data.
 
     Parameters
     ----------
-    out : PyGMI Data
-        PyGMI raster data.
+    ifilet : str
+        filename to import
+    piter : iter, optional
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    tnames : list, optional
+        list of band names to import, in order. The default is None.
+    metaonly : bool, optional
+        Retrieve only the metadata for the file. The default is False.
 
     Returns
     -------
-    out : PyGMI Data
-        PyGMI raster data.
-
+    out : Data
+        PyGMI raster dataset
     """
-    tmplist = []
-    for i in out:
-        tmplist.append(i.dataid)
-
-    tmpcnt = Counter(tmplist)
-    for elt, count in tmpcnt.items():
-        j = 1
-        for i in out:
-            if elt == i.dataid and count > 1:
-                i.dataid += '('+str(j)+')'
-                j += 1
+    if piter is None:
+        piter = ProgressBarText().iter
 
-    return out
+    platform = os.path.basename(ifilet)[2: 4]
+    satbands = None
+    lstband = None
+
+    if platform in ('04', '05'):
+        satbands = {'B1': [450, 520],
+                    'B2': [520, 600],
+                    'B3': [630, 690],
+                    'B4': [760, 900],
+                    'B5': [1550, 1750],
+                    'B6': [10400, 12500],
+                    'B7': [2080, 2350]}
+
+    if platform == '07':
+        satbands = {'B1': [450, 520],
+                    'B2': [520, 600],
+                    'B3': [630, 690],
+                    'B4': [770, 900],
+                    'B5': [1550, 1750],
+                    'B6': [10400, 12500],
+                    'B7': [2090, 2350],
+                    'B8': [520, 900]}
+
+    if platform in ('08', '09'):
+        satbands = {'B1': [430, 450],
+                    'B2': [450, 510],
+                    'B3': [530, 590],
+                    'B4': [640, 670],
+                    'B5': [850, 880],
+                    'B6': [1570, 1650],
+                    'B7': [2110, 2290],
+                    'B8': [500, 680],
+                    'B9': [1360, 1380],
+                    'B10': [1060, 11190],
+                    'B11': [11500, 12510]}
+
+    idir = os.path.dirname(ifilet)
+
+    if '.tar' in ifilet:
+        with tarfile.open(ifilet) as tar:
+            tarnames = tar.getnames()
+            ifile = next((i for i in tarnames if '_MTL.txt' in i), None)
+            if ifile is None:
+                showlog('Could not find MTL.txt file in tar archive')
+                return None
+            showlog('Extracting tar...')
+
+            tar.extractall(idir)
+            ifile = os.path.join(idir, ifile)
+    elif '_MTL.txt' in ifilet:
+        ifile = ifilet
+    else:
+        showlog('Input needs to be tar or _MTL.txt for Landsat. '
+                'Trying regular import')
+        return None
 
+    files = glob.glob(ifile[:-7]+'*.tif')
 
-def cluster_to_raster(indata):
-    """
-    Convert cluster datasets to raster datasets.
+    if glob.glob(ifile[:-7]+'*ST_QA.tif'):
+        if 'LC08' in ifile or 'LC09' in ifile:
+            lstband = 'B10'
+        else:
+            lstband = 'B6'
+        satbands['LST'] = satbands[lstband]
 
-    Some routines will not understand the datasets produced by cluster
-    analysis routines, since they are designated 'Cluster' and not 'Raster'.
-    This provides a work-around for that.
+    showlog('Importing Landsat data...')
 
-    Parameters
-    ----------
-    indata : Data
-        PyGMI raster dataset
+    bnamelen = len(ifile[:-7])
+    nval = 0
+    dat = []
+    for ifile2 in piter(files):
+        fext = ifile2[bnamelen:-4]
+        fext = fext.upper().replace('BAND', 'B')
+        fext = fext.replace('SR_B', 'B')
+        fext = fext.replace('ST_B', 'B')
 
-    Returns
-    -------
-    indata : Data
-        PyGMI raster dataset
+        if fext == lstband:
+            fext = 'LST'
 
-    """
-    if 'Cluster' not in indata:
-        return indata
-    if 'Raster' not in indata:
-        indata['Raster'] = []
+        if tnames is not None and fext.replace(',', ' ') not in tnames:
+            continue
 
-    for i in indata['Cluster']:
-        indata['Raster'].append(i)
-        indata['Raster'][-1].data = indata['Raster'][-1].data + 1
+        showlog('Importing Band '+fext)
+        dataset = rasterio.open(ifile2)
 
-    return indata
+        if dataset is None:
+            showlog('Problem with band '+fext)
+            continue
 
+        dat.append(Data())
 
-def cut_raster(data, ifile, pprint=print, deepcopy=True):
-    """Cuts a raster dataset.
+        if metaonly is False:
+            dat[-1].data = dataset.read(1)
+            dat[-1].data = np.ma.masked_invalid(dat[-1].data)
+
+        nval = 0
+        if fext in ['QA_PIXEL', 'SR_QA_AEROSOL']:
+            nval = 1
+        if fext in ['ST_CDIST', 'ST_QA']:
+            nval = -9999
+        if fext in ['ST_TRAD', 'ST_URAD', 'ST_DRAD']:
+            nval = -9999
+        if fext in ['ST_ATRAN', 'ST_EMIS', 'ST_EMSD']:
+            nval = -9999
+
+        dat[-1].data.mask = dat[-1].data.mask | (dat[-1].data == nval)
+        if dat[-1].data.mask.size == 1:
+            dat[-1].data.mask = (np.ma.make_mask_none(dat[-1].data.shape) +
+                                 dat[-1].data.mask)
+
+        if 'L2SP' in ifile2:
+            if fext == 'LST':
+                showlog('Converting band '+lstband+' to Kelvin. '
+                        'Band renamed as LST')
+                dat[-1].data = dat[-1].data*0.00341802 + 149.0
+            elif fext in satbands:
+                showlog('Converting band '+fext+' to reflectance.')
+                dat[-1].data = dat[-1].data*0.0000275 - 0.2
+            elif fext in ['ST_CDIST', 'ST_QA']:
+                dat[-1].data = dat[-1].data*0.01
+            elif fext in ['ST_TRAD', 'ST_URAD', 'ST_DRAD']:
+                dat[-1].data = dat[-1].data*0.001
+            elif fext in ['ST_ATRAN', 'ST_EMIS', 'ST_EMSD']:
+                dat[-1].data = dat[-1].data*0.0001
+
+        dat[-1].dataid = fext
+        dat[-1].nodata = nval
+        dat[-1].meta_from_rasterio(dataset)
+        dat[-1].filename = ifilet
+
+        bmeta = dat[-1].metadata['Raster']
+
+        platform = os.path.basename(ifilet)[:4]
+        bmeta['Sensor'] = f'Landsat {platform}'
+
+        if satbands is not None and fext in satbands:
+            bmeta['WavelengthMin'] = satbands[fext][0]
+            bmeta['WavelengthMax'] = satbands[fext][1]
+            bmeta['wavelength'] = (satbands[fext][1] + satbands[fext][1])/2
+
+        dataset.close()
+
+    if not dat:
+        dat = None
+
+    if '.tar' in ifilet:
+        showlog('Cleaning Extracted tar files...')
+        for tfile in piter(tarnames):
+            os.remove(os.path.join(os.path.dirname(ifile), tfile))
+    showlog('Import complete')
+    return dat
 
-    Cut a raster dataset using a shapefile.
+
+def get_worldview(ifilet, piter=None, showlog=print, tnames=None,
+                  metaonly=False):
+    """
+    Get WorldView Data.
 
     Parameters
     ----------
-    data : Data
-        PyGMI Dataset
-    ifile : str
-        shapefile used to cut data
-    pprint : function, optional
-        Function for printing text. The default is print.
+    ifilet : str
+        filename to import
+    piter : iter, optional
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    tnames : list, optional
+        list of band names to import, in order. The default is None.
+    metaonly : bool, optional
+        Retrieve only the metadata for the file. The default is False.
 
     Returns
     -------
-    data : Data
-        PyGMI Dataset
+    out : Data
+        PyGMI raster dataset
     """
+    if piter is None:
+        piter = ProgressBarText().iter
 
-    if deepcopy is True:
-        data = copy.deepcopy(data)
+    dtree = etree_to_dict(ET.parse(ifilet).getroot())
 
-    try:
-        gdf = gpd.read_file(ifile)
-    except:
-        pprint('There was a problem importing the shapefile. Please make '
-               'sure you have at all the individual files which make up '
-               'the shapefile.')
+    if 'isd' not in dtree:
+        showlog('Wrong xml file. Please choose the xml file in the '
+                'PAN or MUL directory')
         return None
 
-    gdf = gdf[gdf.geometry != None]
+    platform = dtree['isd']['TIL']['BANDID']
+    satid = dtree['isd']['IMD']['IMAGE']['SATID']
+    satbands = None
+
+    if platform == 'P':
+        satbands = {'1': [450, 800]}
+        bnum2name = {0: 'BAND_P'}
+
+    if platform == 'Multi' and 'WV' in satid:
+        satbands = {'1': [400, 450],
+                    '2': [450, 510],
+                    '3': [510, 580],
+                    '4': [585, 625],
+                    '5': [630, 690],
+                    '6': [705, 745],
+                    '7': [770, 895],
+                    '8': [860, 1040]}
+
+        bnum2name = {0: 'BAND_C',
+                     1: 'BAND_B',
+                     2: 'BAND_G',
+                     3: 'BAND_Y',
+                     4: 'BAND_R',
+                     5: 'BAND_RE',
+                     6: 'BAND_N',
+                     7: 'BAND_N2'}
+
+    if platform == 'Multi' and 'GE' in satid:
+        satbands = {'1': [450, 510],
+                    '2': [510, 580],
+                    '3': [655, 690],
+                    '4': [780, 920]}
+
+        bnum2name = {0: 'BAND_B',
+                     1: 'BAND_G',
+                     2: 'BAND_R',
+                     3: 'BAND_N'}
+
+    if satid == 'WV03':
+        Esun = {'BAND_P': 1574.41,
+                'BAND_C': 1757.89,
+                'BAND_B': 2004.61,
+                'BAND_G': 1830.18,
+                'BAND_Y': 1712.07,
+                'BAND_R': 1535.33,
+                'BAND_RE': 1348.08,
+                'BAND_N': 1055.94,
+                'BAND_N2': 858.77}
+    elif satid == 'WV02':
+        Esun = {'BAND_P': 1580.8140,
+                'BAND_C': 1758.2229,
+                'BAND_B': 1974.2416,
+                'BAND_G': 1856.4104,
+                'BAND_Y': 1738.4791,
+                'BAND_R': 1559.4555,
+                'BAND_RE': 1342.0695,
+                'BAND_N': 1069.7302,
+                'BAND_N2': 861.2866}
+    elif satid == 'GE01':
+        Esun = {'BAND_B': 1960.0,
+                'BAND_G': 1853.0,
+                'BAND_R': 1505.0,
+                'BAND_N': 1039.0}
+
+    idir = os.path.dirname(ifilet)
+
+    showlog('Importing WorldView tiles...')
+
+    rmax = int(dtree['isd']['IMD']['NUMROWS'])
+    cmax = int(dtree['isd']['IMD']['NUMCOLUMNS'])
+
+    xmin = float(dtree['isd']['IMD']['MAP_PROJECTED_PRODUCT']['ORIGINX'])
+    ymax = float(dtree['isd']['IMD']['MAP_PROJECTED_PRODUCT']['ORIGINY'])
+    xdim = float(dtree['isd']['IMD']['MAP_PROJECTED_PRODUCT']['COLSPACING'])
+    ydim = float(dtree['isd']['IMD']['MAP_PROJECTED_PRODUCT']['ROWSPACING'])
 
-    if gdf.geom_type.iloc[0] == 'MultiPolygon':
-        pprint('You have a MultiPolygon. Only the first overlapping Polygon '
-               'of the MultiPolygon will be used.')
-        poly = gdf['geometry'].iloc[0]
-        tmp = poly.geoms[0]
-
-        dext = list(data[0].bounds)
-        dpoly = box(dext[0], dext[1], dext[2], dext[3])
-
-        for i in list(poly.geoms):
-            if i.overlaps(dpoly):
-                tmp = i
-                break
+    dat = []
+    nval = 0
+    for i in range(len(satbands)):
+        bname = f'Band {i+1}'
+        if tnames is not None and bname not in tnames:
+            continue
 
-        gdf.geometry.iloc[0] = tmp
+        fext = str(i+1)
+        dat.append(Data())
+        if metaonly is False:
+            dat[-1].data = np.zeros((rmax, cmax))
+
+        dat[-1].dataid = bname
+        dat[-1].nodata = nval
+        dat[-1].set_transform(xdim, xmin, ydim, ymax)
+
+        bmeta = dat[-1].metadata['Raster']
+
+        bmeta['Sensor'] = f'WorldView {satid} {platform}'
+
+        if satbands is not None and fext in satbands:
+            bmeta['WavelengthMin'] = satbands[fext][0]
+            bmeta['WavelengthMax'] = satbands[fext][1]
+        bmeta['wavelength'] = (satbands[fext][0]+satbands[fext][1])/2
+
+    for tile in dtree['isd']['TIL']['TILE']:
+        ifile = os.path.join(idir, tile['FILENAME'])
+
+        rmin = int(tile['ULROWOFFSET'])
+        rmax = int(tile['LRROWOFFSET'])
+        cmin = int(tile['ULCOLOFFSET'])
+        cmax = int(tile['LRCOLOFFSET'])
+
+        showlog('Importing '+tile['FILENAME'])
+        dataset = rasterio.open(ifile)
+
+        for i in piter(dataset.indexes):
+            if metaonly is False:
+                dat[i-1].data[rmin:rmax+1, cmin:cmax+1] = dataset.read(i)
+
+            bmeta = dataset.tags(i)
+            dat[i-1].crs = dataset.crs
+            dat[i-1].filename = ifile
+        dataset.close()
+
+    showlog('Calculating radiance and reflectance...')
+    indx = -1
+    for i in piter(dat):
+        if metaonly is True:
+            continue
+        indx += 1
+        mask = (i.data == nval)
 
-    if gdf.geom_type.iloc[0] != 'Polygon':
-        pprint('You need a polygon in that shape file')
-        return None
+        scale = float(dtree['isd']['IMD'][bnum2name[indx]]['ABSCALFACTOR'])
+        bwidth = float(dtree['isd']['IMD'][bnum2name[indx]]['EFFECTIVEBANDWIDTH'])
 
-    for idata in data:
-        # Convert the layer extent to image pixel coordinates
-        poly = gdf['geometry'].iloc[0]
-        dext = idata.bounds
-        lext = poly.bounds
-
-        if ((dext[0] > lext[2]) or (dext[2] < lext[0])
-                or (dext[1] > lext[3]) or (dext[3] < lext[1])):
-
-            pprint('The shapefile is not in the same area as the raster '
-                   'dataset. Please check its coordinates and make sure its '
-                   'projection is the same as the raster dataset')
-            return None
+        i.data = i.data.astype(np.float32)
 
-        # This section converts PolygonZ to Polygon, and takes first polygon.
-        coords = gdf['geometry'].loc[0].exterior.coords
-        coords = [Polygon([[p[0], p[1]] for p in coords])]
+        date = dtree['isd']['IMD']['IMAGE']['FIRSTLINETIME']
 
-        dat, trans = riomask(idata.to_mem(), coords, crop=True)
+        year = int(date[:4])
+        month = int(date[5:7])
+        day = int(date[8:10])
+        hour = int(date[11:13])
+        minute = int(date[14:16])
+        sec = float(date[17:-1])
 
-        idata.data = np.ma.masked_equal(dat.squeeze(), idata.nodata)
+        UT = hour + minute/60. + sec/3600.
 
-        idata.set_transform(transform=trans)
+        # Julian day
 
-    return data
+        if month in (1, 2):
+            year -= 1
+            month += 12
 
+        A = int(year/100.)
+        B = 2 - A + int(A/4.)
 
-def epsgtowkt(epsg):
-    """
-    Routine to get a WKT from an epsg code.
+        JD = int(365.25*(year+4716))+int(30.6001*(month+1))+day+UT/24.+B-1524.5
 
-    Parameters
-    ----------
-    epsg : str or int
-        EPSG code.
+        D = JD - 2451545.0
+        g = np.deg2rad(357.529 + 0.98560028 * D)
 
-    Returns
-    -------
-    out : str
-        WKT description.
+        dES = 1.00014 - 0.01671*np.cos(g) - 0.00014*np.cos(2*g)
 
-    """
-    out = CRS.from_epsg(int(epsg)).to_wkt()
-    return out
+        szenith = 90. - float(dtree['isd']['IMD']['IMAGE']['MEANSUNEL'])
+        szenith = np.deg2rad(szenith)
 
+        tmp = dES**2 * np.pi / (Esun[bnum2name[indx]] * np.cos(szenith))
+        tmp = tmp * scale / bwidth
 
-def getepsgcodes():
-    """
-    Routine used to get a list of EPSG codes.
+        idata = i.data
+        i.data = ne.evaluate('idata * tmp')
 
-    Returns
-    -------
-    pcodes : dictionary
-        Dictionary of codes per projection in WKT format.
+        i.data = np.ma.array(i.data, mask=mask)
 
-    """
-    with open(os.path.join(os.path.dirname(__file__), 'gcs.csv'),
-              encoding='utf-8') as dfile:
-        dlines = dfile.readlines()
-
-    dlines = dlines[1:]
-    dcodes = {}
-    for i in dlines:
-        tmp = i.split(',')
-        if tmp[1][0] == '"':
-            tmp[1] = tmp[1][1:-1]
-
-        dcodes[tmp[1]] = int(tmp[0])
-
-    with open(os.path.join(os.path.dirname(__file__), 'pcs.csv'),
-              encoding='utf-8') as pfile:
-        plines = pfile.readlines()
-
-    pcodes = {}
-    for i in dcodes:
-        pcodes[i+r' / Geodetic Geographic'] = dcodes[i]
-
-    plines = plines[1:]
-    for i in plines:
-        tmp = i.split(',')
-        if tmp[1][0] == '"':
-            tmp[1] = tmp[1][1:-1]
-
-        pcodes[tmp[1]] = int(tmp[0])
-
-    for datum in ['Cape', 'Hartebeesthoek94']:
-        for clong in range(15, 35, 2):
-            if 'Cape' in datum:
-                wkt = ('PROJCS["Cape / TM'+str(clong)+'",'
-                       'GEOGCS["Cape",'
-                       'DATUM["Cape",'
-                       'SPHEROID["Clarke 1880 (Arc)",'
-                       '6378249.145,293.4663077,'
-                       'AUTHORITY["EPSG","7013"]],'
-                       'AUTHORITY["EPSG","6222"]],'
-                       'PRIMEM["Greenwich",0,'
-                       'AUTHORITY["EPSG","8901"]],'
-                       'UNIT["degree",0.0174532925199433,'
-                       'AUTHORITY["EPSG","9122"]],'
-                       'AUTHORITY["EPSG","4222"]],'
-                       'PROJECTION["Transverse_Mercator"],'
-                       'PARAMETER["latitude_of_origin",0],'
-                       'PARAMETER["central_meridian",'+str(clong)+'],'
-                       'PARAMETER["scale_factor",1],'
-                       'PARAMETER["false_easting",0],'
-                       'PARAMETER["false_northing",0],'
-                       'UNIT["metre",1,AUTHORITY["EPSG","9001"]],'
-                       'AXIS["Easting",EAST],'
-                       'AXIS["Northing",NORTH]]')
-
-            elif 'Hartebeesthoek94' in datum:
-                wkt = ('PROJCS["Hartebeesthoek94 / TM'+str(clong)+'",'
-                       'GEOGCS["Hartebeesthoek94",'
-                       'DATUM["Hartebeesthoek94",'
-                       'SPHEROID["WGS 84",6378137,298.257223563,'
-                       'AUTHORITY["EPSG","7030"]],'
-                       'AUTHORITY["EPSG","6148"]],'
-                       'PRIMEM["Greenwich",0,'
-                       'AUTHORITY["EPSG","8901"]],'
-                       'UNIT["degree",0.0174532925199433,'
-                       'AUTHORITY["EPSG","9122"]],'
-                       'AUTHORITY["EPSG","4148"]],'
-                       'PROJECTION["Transverse_Mercator"],'
-                       'PARAMETER["latitude_of_origin",0],'
-                       'PARAMETER["central_meridian",'+str(clong)+'],'
-                       'PARAMETER["scale_factor",1],'
-                       'PARAMETER["false_easting",0],'
-                       'PARAMETER["false_northing",0],'
-                       'UNIT["metre",1,AUTHORITY["EPSG","9001"]],'
-                       'AXIS["Easting",EAST],'
-                       'AXIS["Northing",NORTH]]')
-
-            pcodes[datum+r' / TM'+str(clong)] = wkt
-
-    return pcodes
+    if not dat:
+        dat = None
 
+    # Standardize labels for band ratioing.
 
-def lstack(dat, piter=None, dxy=None, pprint=print, commonmask=False,
-           masterid=None, nodeepcopy=False):
-    """
-    Layer stack datasets found in a single PyGMI data object.
+    wvlabels = {'CoastalBlue': 'B1',
+                'Blue': 'B2',
+                'Green': 'B3',
+                'Yellow': 'B4',
+                'Red': 'B5',
+                'RedEdge': 'B6',
+                'NIR1': 'B7',
+                'NIR2': 'B8'}
+    for i in dat:
+        if i.dataid.split()[0] in wvlabels:
+            i.dataid = wvlabels[i.dataid.split()[0]]
+
+    showlog('Import complete')
+    return dat
 
-    The aim is to ensure that all datasets have the same number of rows and
-    columns.
+
+def get_hyperion(ifile, piter=None, showlog=print, tnames=None,
+                 metaonly=False):
+    """
+    Get Hyperion Data.
 
     Parameters
     ----------
-    dat : PyGMI Data
-        data object which stores datasets
+    ifile : str
+        filename to import
     piter : iter, optional
-        Progress bar iterator. The default is None.
-    dxy : float, optional
-        Cell size. The default is None.
-    pprint : function, optional
-        Print function. The default is print.
-    commonmask : bool, optional
-        Create a common mask for all bands. The default is False.
-    masterid : int, optional
-        ID of master dataset. The default is None.
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    tnames : list, optional
+        list of band names to import, in order. The default is None.
+    metaonly : bool, optional
+        Retrieve only the metadata for the file. The default is False.
 
     Returns
     -------
-    out : PyGMI Data
-        data object which stores datasets
-
+    out : Data
+        PyGMI raster dataset
     """
     if piter is None:
         piter = ProgressBarText().iter
 
-    if dat[0].isrgb:
-        return dat
+    wavelength = [
+        355.59,  365.76,  375.94,  386.11,  396.29,  406.46,  416.64,  426.82,
+        436.99,  447.17,  457.34,  467.52,  477.69,  487.87,  498.04,  508.22,
+        518.39,  528.57,  538.74,  548.92,  559.09,  569.27,  579.45,  589.62,
+        599.80,  609.97,  620.15,  630.32,  640.50,  650.67,  660.85,  671.02,
+        681.20,  691.37,  701.55,  711.72,  721.90,  732.07,  742.25,  752.43,
+        762.60,  772.78,  782.95,  793.13,  803.30,  813.48,  823.65,  833.83,
+        844.00,  854.18,  864.35,  874.53,  884.70,  894.88,  905.05,  915.23,
+        925.41,  935.58,  945.76,  955.93,  966.11,  976.28,  986.46,  996.63,
+        1006.81, 1016.98, 1027.16, 1037.33, 1047.51, 1057.68,  851.92,  862.01,
+        872.10,  882.19,  892.28,  902.36,  912.45,  922.54,  932.64,  942.73,
+        952.82,  962.91,  972.99,  983.08,  993.17, 1003.30, 1013.30, 1023.40,
+        1033.49, 1043.59, 1053.69, 1063.79, 1073.89, 1083.99, 1094.09, 1104.19,
+        1114.19, 1124.28, 1134.38, 1144.48, 1154.58, 1164.68, 1174.77, 1184.87,
+        1194.97, 1205.07, 1215.17, 1225.17, 1235.27, 1245.36, 1255.46, 1265.56,
+        1275.66, 1285.76, 1295.86, 1305.96, 1316.05, 1326.05, 1336.15, 1346.25,
+        1356.35, 1366.45, 1376.55, 1386.65, 1396.74, 1406.84, 1416.94, 1426.94,
+        1437.04, 1447.14, 1457.23, 1467.33, 1477.43, 1487.53, 1497.63, 1507.73,
+        1517.83, 1527.92, 1537.92, 1548.02, 1558.12, 1568.22, 1578.32, 1588.42,
+        1598.51, 1608.61, 1618.71, 1628.81, 1638.81, 1648.90, 1659.00, 1669.10,
+        1679.20, 1689.30, 1699.40, 1709.50, 1719.60, 1729.70, 1739.70, 1749.79,
+        1759.89, 1769.99, 1780.09, 1790.19, 1800.29, 1810.38, 1820.48, 1830.58,
+        1840.58, 1850.68, 1860.78, 1870.87, 1880.98, 1891.07, 1901.17, 1911.27,
+        1921.37, 1931.47, 1941.57, 1951.57, 1961.66, 1971.76, 1981.86, 1991.96,
+        2002.06, 2012.15, 2022.25, 2032.35, 2042.45, 2052.45, 2062.55, 2072.65,
+        2082.75, 2092.84, 2102.94, 2113.04, 2123.14, 2133.24, 2143.34, 2153.34,
+        2163.43, 2173.53, 2183.63, 2193.73, 2203.83, 2213.93, 2224.03, 2234.12,
+        2244.22, 2254.22, 2264.32, 2274.42, 2284.52, 2294.61, 2304.71, 2314.81,
+        2324.91, 2335.01, 2345.11, 2355.21, 2365.20, 2375.30, 2385.40, 2395.50,
+        2405.60, 2415.70, 2425.80, 2435.89, 2445.99, 2456.09, 2466.09, 2476.19,
+        2486.29, 2496.39, 2506.48, 2516.59, 2526.68, 2536.78, 2546.88, 2556.98,
+        2566.98, 2577.08]
+
+    fwhm = [
+        11.3871, 11.3871, 11.3871, 11.3871, 11.3871, 11.3871, 11.3871, 11.3871,
+        11.3871, 11.3871, 11.3871, 11.3871, 11.3871, 11.3784, 11.3538, 11.3133,
+        11.2580, 11.1907, 11.1119, 11.0245, 10.9321, 10.8368, 10.7407, 10.6482,
+        10.5607, 10.4823, 10.4147, 10.3595, 10.3188, 10.2942, 10.2856, 10.2980,
+        10.3349, 10.3909, 10.4592, 10.5322, 10.6004, 10.6562, 10.6933, 10.7058,
+        10.7276, 10.7907, 10.8833, 10.9938, 11.1044, 11.1980, 11.2600, 11.2824,
+        11.2822, 11.2816, 11.2809, 11.2797, 11.2782, 11.2771, 11.2765, 11.2756,
+        11.2754, 11.2754, 11.2754, 11.2754, 11.2754, 11.2754, 11.2754, 11.2754,
+        11.2754, 11.2754, 11.2754, 11.2754, 11.2754, 11.2754, 11.0457, 11.0457,
+        11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0457,
+        11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0451,
+        11.0423, 11.0372, 11.0302, 11.0218, 11.0122, 11.0013, 10.9871, 10.9732,
+        10.9572, 10.9418, 10.9248, 10.9065, 10.8884, 10.8696, 10.8513, 10.8335,
+        10.8154, 10.7979, 10.7822, 10.7663, 10.7520, 10.7385, 10.7270, 10.7174,
+        10.7091, 10.7022, 10.6970, 10.6946, 10.6937, 10.6949, 10.6996, 10.7058,
+        10.7163, 10.7283, 10.7437, 10.7612, 10.7807, 10.8034, 10.8267, 10.8534,
+        10.8818, 10.9110, 10.9422, 10.9743, 11.0074, 11.0414, 11.0759, 11.1108,
+        11.1461, 11.1811, 11.2156, 11.2496, 11.2826, 11.3146, 11.3460, 11.3753,
+        11.4037, 11.4302, 11.4538, 11.4760, 11.4958, 11.5133, 11.5286, 11.5404,
+        11.5505, 11.5580, 11.5621, 11.5634, 11.5617, 11.5563, 11.5477, 11.5346,
+        11.5193, 11.5002, 11.4789, 11.4548, 11.4279, 11.3994, 11.3688, 11.3366,
+        11.3036, 11.2696, 11.2363, 11.2007, 11.1666, 11.1333, 11.1018, 11.0714,
+        11.0424, 11.0155, 10.9912, 10.9698, 10.9508, 10.9355, 10.9230, 10.9139,
+        10.9083, 10.9069, 10.9057, 10.9013, 10.8951, 10.8854, 10.8740, 10.8591,
+        10.8429, 10.8242, 10.8039, 10.7820, 10.7592, 10.7342, 10.7092, 10.6834,
+        10.6572, 10.6312, 10.6052, 10.5803, 10.5560, 10.5328, 10.5101, 10.4904,
+        10.4722, 10.4552, 10.4408, 10.4285, 10.4197, 10.4129, 10.4088, 10.4077,
+        10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077,
+        10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077,
+        10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077,
+        10.4077, 10.4077]
+
+    showlog('Extracting zip...')
+
+    idir = os.path.dirname(ifile)
+    with zipfile.ZipFile(ifile) as zfile:
+        zipnames = zfile.namelist()
+        zfile.extractall(idir)
+
+    zipnames2 = [i for i in zipnames if i[-3:].lower() == 'tif']
+
+    # This section is to import the correct scale factors
+    # Pick first txt file since other should be readme.txt
+    header = [i for i in zipnames if '.txt' in i.lower()]
+
+    scale_vnir = 40.
+    scale_swir = 80.
+
+    if len(header) > 0:
+        hfile = header[0]
+
+        with open(os.path.join(idir, hfile), encoding='utf-8') as headerfile:
+            txt = headerfile.read()
+
+        txt = txt.split('\n')
+        scale_vnir = [i for i in txt if 'SCALING_FACTOR_VNIR' in i][0]
+        scale_swir = [i for i in txt if 'SCALING_FACTOR_SWIR' in i][0]
 
-    needsmerge = False
-    rows, cols = dat[0].data.shape
+        scale_vnir = float(scale_vnir.split(' = ')[-1])
+        scale_swir = float(scale_swir.split(' = ')[-1])
 
-    dtypes = []
-    for i in dat:
-        irows, icols = i.data.shape
-        if irows != rows or icols != cols:
-            needsmerge = True
-        if dxy is not None and (i.xdim != dxy or i.ydim != dxy):
-            needsmerge = True
-        if commonmask is True:
-            needsmerge = True
-        if i.extent != dat[0].extent:
-            needsmerge = True
-        dtypes.append(i.data.dtype)
-
-    dtypes = np.unique(dtypes)
-    dtype = None
-    nodata = None
-    if len(dtypes) > 1:
-        needsmerge = True
-        for i in dtypes:
-            if np.issubdtype(i, np.floating):
-                dtype = np.float64
-                nodata = 1e+20
-            elif dtype is None:
-                dtype = np.int32
-                nodata = 999999
-
-    if needsmerge is False:
-        if not nodeepcopy:
-            dat = copy.deepcopy(dat)
-        dat = check_dataid(dat)
-        return dat
-
-    pprint('Merging data...')
-    if masterid is not None:
-        data = dat[masterid]
-        xmin, xmax, ymin, ymax = data.extent
-        if dxy is None:
-            dxy = min(data.xdim, data.ydim)
-    else:
-        data = dat[0]
+    showlog('Importing Hyperion data...')
 
-        if dxy is None:
-            dxy = min(data.xdim, data.ydim)
-            for data in dat:
-                dxy = min(dxy, data.xdim, data.ydim)
-
-        xmin0, xmax0, ymin0, ymax0 = data.extent
-        for data in dat:
-            xmin, xmax, ymin, ymax = data.extent
-            xmin = min(xmin, xmin0)
-            xmax = max(xmax, xmax0)
-            ymin = min(ymin, ymin0)
-            ymax = max(ymax, ymax0)
-
-    cols = int((xmax - xmin)/dxy)
-    rows = int((ymax - ymin)/dxy)
-    trans = rasterio.Affine(dxy, 0, xmin, 0, -1*dxy, ymax)
-
-    if cols == 0 or rows == 0:
-        pprint('Your rows or cols are zero. '
-               'Your input projection may be wrong')
-        return None
+    nval = 0
+    dat = []
+    maskall = None
+    for ifile2 in piter(zipnames2):
+        fext = ifile2.split('_')[1]
+        bandno = int(fext[1:])
 
-    dat2 = []
-    cmask = None
-    for data in piter(dat):
-
-        if dtype is not None:
-            data.data = data.data.astype(dtype)
-            data.nodata = nodata
-
-        if data.crs is None:
-            pprint(f'{data.dataid} has no defined projection. '
-                   'Assigning local.')
-
-            data.crs = CRS.from_string('LOCAL_CS["Arbitrary",UNIT["metre",1,'
-                                       'AUTHORITY["EPSG","9001"]],'
-                                       'AXIS["Easting",EAST],'
-                                       'AXIS["Northing",NORTH]]')
-
-        doffset = 0.0
-        data.data.set_fill_value(data.nodata)
-        data.data = np.ma.array(data.data.filled(), mask=data.data.mask)
-
-        if data.data.min() <= 0:
-            doffset = data.data.min()-1.
-            data.data = data.data - doffset
-
-        trans0 = data.transform
-
-        height, width = data.data.shape
-
-        odata = np.zeros((rows, cols), dtype=data.data.dtype)
-        odata, _ = reproject(source=data.data,
-                             destination=odata,
-                             src_transform=trans0,
-                             src_crs=data.crs,
-                             src_nodata=data.nodata,
-                             dst_transform=trans,
-                             dst_crs=data.crs)
-
-        data2 = Data()
-        data2.data = np.ma.masked_equal(odata, data.nodata)
-        data2.data.mask = np.ma.getmaskarray(data2.data)
-        data2.nodata = data.nodata
-        data2.crs = data.crs
-        data2.set_transform(transform=trans)
-        data2.data = data2.data.astype(data.data.dtype)
-        data2.dataid = data.dataid
-        data2.filename = data.filename
+        # Eliminate bands not illuminated
+        if bandno <= 7 or bandno >= 225:
+            continue
 
-        dat2.append(data2)
+        # Overlap Region
+        if 58 <= bandno <= 78:
+            continue
 
-        if cmask is None:
-            cmask = dat2[-1].data.mask
-        else:
-            cmask = np.logical_or(cmask, dat2[-1].data.mask)
+        bname = f'Band {bandno}: {wavelength[bandno-1]} nm'
+        if tnames is not None and bname not in tnames:
+            continue
 
-        dat2[-1].metadata = data.metadata
-        dat2[-1].data = dat2[-1].data + doffset
+        showlog(f'Importing band {bandno}: {wavelength[bandno-1]} nm')
+        dataset = rasterio.open(os.path.join(idir, ifile2))
 
-        dat2[-1].nodata = data.nodata
-        dat2[-1].data.set_fill_value(data.nodata)
-        dat2[-1].data = np.ma.array(dat2[-1].data.filled(),
-                                    mask=dat2[-1].data.mask)
+        if dataset is None:
+            showlog(f'Problem with band {bandno}')
+            continue
 
-        data.data = data.data + doffset
+        dat.append(Data())
 
-    if commonmask is True:
-        for idat in piter(dat2):
-            idat.data.mask = cmask
-            idat.data = np.ma.array(idat.data.filled(idat.nodata), mask=cmask)
+        if metaonly is False:
+            rtmp = dataset.read(1)
 
-    out = check_dataid(dat2)
+            if bandno <= 70:
+                rtmp = rtmp / scale_vnir
+            else:
+                rtmp = rtmp / scale_swir
 
-    return out
+            dat[-1].data = rtmp
 
+            dat[-1].data = np.ma.masked_invalid(dat[-1].data)
+            dat[-1].data.mask = dat[-1].data.mask | (dat[-1].data == nval)
+            if dat[-1].data.mask.size == 1:
+                dat[-1].data.mask = (np.ma.make_mask_none(dat[-1].data.shape) +
+                                     dat[-1].data.mask)
 
-def trim_raster(olddata):
-    """
-    Trim nulls from a raster dataset.
+            if maskall is None:
+                maskall = dat[-1].data.mask
+            else:
+                maskall = np.logical_and(maskall, dat[-1].data.mask)
 
-    This function trims entire rows or columns of data which are masked,
-    and are on the edges of the dataset. Masked values are set to the null
-    value.
+        dat[-1].dataid = bname
+        dat[-1].nodata = nval
+        dat[-1].meta_from_rasterio(dataset)
+        dat[-1].filename = ifile
 
-    Parameters
-    ----------
-    olddata : Data
-        PyGMI dataset
+        bmeta = {}
+        bmeta['Sensor'] = 'Hyperion EO1H'
+        # if satbands is not None and fext in satbands:
 
-    Returns
-    -------
-    olddata : Data
-        PyGMI dataset
-    """
-    for data in olddata:
-        mask = np.ma.getmaskarray(data.data)
-        data.data.data[mask] = data.nodata
-
-        rowstart = 0
-        for i in range(mask.shape[0]):
-            if bool(mask[i].min()) is False:
-                break
-            rowstart += 1
-
-        rowend = mask.shape[0]
-        for i in range(mask.shape[0]-1, -1, -1):
-            if bool(mask[i].min()) is False:
-                break
-            rowend -= 1
+        dat[-1].metadata['Raster']['wavelength'] = wavelength[bandno-1]
+        bmeta['WavelengthMin'] = wavelength[bandno-1]-fwhm[bandno-1]/2
+        bmeta['WavelengthMax'] = wavelength[bandno-1]+fwhm[bandno-1]/2
 
-        colstart = 0
-        for i in range(mask.shape[1]):
-            if bool(mask[:, i].min()) is False:
-                break
-            colstart += 1
+        dat[-1].metadata['Raster'].update(bmeta)
 
-        colend = mask.shape[1]
-        for i in range(mask.shape[1]-1, -1, -1):
-            if bool(mask[:, i].min()) is False:
-                break
-            colend -= 1
+        dataset.close()
 
-        drows, dcols = data.data.shape
-        data.data = data.data[rowstart:rowend, colstart:colend]
-        data.data.mask = (data.data.data == data.nodata)
-        xmin = data.extent[0] + colstart*data.xdim
-        ymax = data.extent[-1] - rowstart*data.ydim
+    if not dat:
+        dat = None
 
-        data.set_transform(data.xdim, xmin, data.ydim, ymax)
+    for i in dat:
+        i.data.mask = maskall
 
-    return olddata
+    showlog('Cleaning Extracted zip files...')
+    for zfile in zipnames:
+        os.remove(os.path.join(idir, zfile))
 
+    showlog('Import complete')
+    return dat
 
-def cut_raster_basic(data, ifile, pprint=print):
-    """Cuts a raster dataset.
 
-    Cut a raster dataset using a shapefile.
+def get_sentinel1(ifile, piter=None, showlog=print, tnames=None,
+                  metaonly=False):
+    """
+    Get Sentinel-1 Data.
 
     Parameters
     ----------
-    data : Data
-        PyGMI Dataset
     ifile : str
-        shapefile used to cut data
-    pprint : function, optional
-        Function for printing text. The default is print.
+        filename to import
+    piter : iter, optional
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    tnames : list, optional
+        list of band names to import, in order. The default is None.
+    metaonly : bool, optional
+        Retrieve only the metadata for the file. The default is False.
 
     Returns
     -------
-    data : Data
-        PyGMI Dataset
+    dat : PyGMI raster Data
+        dataset imported
     """
-    data = copy.deepcopy(data)
+    if piter is None:
+        piter = ProgressBarText().iter
 
-    try:
-        gdf = gpd.read_file(ifile)
-    except:
-        pprint('There was a problem importing the shapefile. Please make '
-               'sure you have at all the individual files which make up '
-               'the shapefile.')
-        return None
+    ifile = ifile[:]
 
-    gdf = gdf[gdf.geometry != None]
+    with rasterio.open(ifile) as dataset:
+        if dataset is None:
+            return None
+        subdata = dataset.subdatasets
+        # tmp = dataset.tags(ns='derived_subdatasets')
 
-    if gdf.geom_type.iloc[0] == 'MultiPolygon':
-        pprint('You have a MultiPolygon. Only the first overlapping Polygon '
-               'of the MultiPolygon will be used.')
-        poly = gdf['geometry'].iloc[0]
-        tmp = poly.geoms[0]
-
-        dext = list(data[0].bounds)
-        dpoly = box(dext[0], dext[1], dext[2], dext[3])
-
-        for i in list(poly.geoms):
-            if i.overlaps(dpoly):
-                tmp = i
-                break
+    # subdata = [i for i in subdata if 'IW1' in i]
+    # subdata = [i for i in subdata if 'COMPLEX' not in i]
 
-        gdf.geometry.iloc[0] = tmp
+    nval = 0
+    dat = []
 
-    if gdf.geom_type.iloc[0] != 'Polygon':
-        pprint('You need a polygon in that shape file')
-        return None
+    for bfile in subdata:
+        tmp = bfile.split(':')
+        bname = f'{tmp[0]}_{tmp[1]}_{tmp[-2]}_{tmp[-1]}'
+
+        dataset1 = rasterio.open(bfile)
+        showlog('Importing '+bname)
+        if dataset1 is None:
+            showlog('Problem with '+ifile)
+            continue
 
-    for idata in data:
-        # Convert the layer extent to image pixel coordinates
-        poly = gdf['geometry'].iloc[0]
-        dext = idata.bounds
-        lext = poly.bounds
-
-        if ((dext[0] > lext[2]) or (dext[2] < lext[0])
-                or (dext[1] > lext[3]) or (dext[3] < lext[1])):
-
-            pprint('The shapefile is not in the same area as the raster '
-                   'dataset. Please check its coordinates and make sure its '
-                   'projection is the same as the raster dataset')
-            return None
+        dataset = rasterio.vrt.WarpedVRT(dataset1)
+
+        for i in piter(dataset.indexes):
+            bmeta = dataset.tags(i)
+            print(bmeta)
+
+            if tnames is not None and bname not in tnames:
+                continue
+
+            dat.append(Data())
 
-        # This section convers PolygonZ to Polygon, and takes first polygon.
-        coords = gdf['geometry'].loc[0].exterior.coords
-        coords = [Polygon([[p[0], p[1]] for p in coords])]
+            if not metaonly:
+                rtmp = dataset.read(i)
 
-        dat, trans = riomask(idata.to_mem(), coords, crop=True)
+                dat[-1].data = rtmp
+                dat[-1].data = np.ma.masked_invalid(dat[-1].data)
+                dat[-1].data.mask = dat[-1].data.mask | (dat[-1].data == nval)
+                if dat[-1].data.mask.size == 1:
+                    dat[-1].mask = np.ma.getmaskarray(dat[-1].data)
+                # dat[-1].data = dat[-1].data.astype(float)
+                # dat[-1].data = dat[-1].data / 10000.
+
+            dat[-1].dataid = bname
+            dat[-1].nodata = nval
+            dat[-1].meta_from_rasterio(dataset)
+            dat[-1].filename = ifile
+            # dat[-1].units = 'Reflectance'
+
+            bmeta['Raster'] = dat[-1].metadata['Raster']
+            bmeta['Raster']['Sensor'] = 'Sentinel-1'
 
-        idata.data = np.ma.masked_equal(dat.squeeze(), idata.nodata)
+            dat[-1].metadata.update(bmeta)
 
-        idata.set_transform(transform=trans)
+        dataset.close()
 
-    return data
+    if not dat:
+        dat = None
+
+    return dat
 
 
-def get_shape_bounds(sfile, crs=None, pprint=print):
+def get_sentinel2(ifile, piter=None, showlog=print, tnames=None,
+                  metaonly=False):
     """
-    Get bounds from a shape file.
+    Get Sentinel-2 Data.
 
     Parameters
     ----------
-    sfile : str
-        Filename for shapefile.
-    crs : rasterio CRS
-        target crs for shapefile
-    pprint : TYPE, optional
-        Print. The default is print.
+    ifile : str
+        filename to import
+    piter : iter, optional
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    tnames : list, optional
+        list of band names to import, in order. The default is None.
+    metaonly : bool, optional
+        Retrieve only the metadata for the file. The default is False.
 
     Returns
     -------
-    bounds : list
-        Rasterio bounds.
-
+    dat : PyGMI raster Data
+        dataset imported
     """
-    if sfile == '' or sfile is None:
-        return None
-
-    gdf = gpd.read_file(sfile)
+    if piter is None:
+        piter = ProgressBarText().iter
 
-    gdf = gdf[gdf.geometry != None]
+    ifile = ifile[:]
 
-    if crs is not None:
-        gdf = gdf.to_crs(crs)
+    with rasterio.open(ifile) as dataset:
+        if dataset is None:
+            return None
+        subdata = dataset.subdatasets
 
-    if gdf.geom_type.iloc[0] == 'MultiPolygon':
-        pprint('You have a MultiPolygon. Only the first Polygon '
-               'of the MultiPolygon will be used.')
-        poly = gdf['geometry'].iloc[0]
-        tmp = poly.geoms[0]
+    subdata = [i for i in subdata if 'TCI' not in i]  # TCI is true color
 
-        gdf.geometry.iloc[0] = tmp
+    nval = 0
+    dat = []
+    for bfile in subdata:
+        dataset = rasterio.open(bfile)
+        showlog('Importing '+os.path.basename(bfile))
+        if dataset is None:
+            showlog('Problem with '+ifile)
+            continue
 
-    if gdf.geom_type.iloc[0] != 'Polygon':
-        pprint('You need a polygon in that shape file')
-        return None
+        for i in piter(dataset.indexes):
+            bmeta = dataset.tags(i)
 
-    bounds = gdf.geometry.iloc[0].bounds
+            bname = dataset.descriptions[i-1]+f' ({dataset.transform[0]}m)'
+            bname = bname.replace(',', ' ')
+            if tnames is not None and bname not in tnames:
+                continue
 
-    return bounds
+            dat.append(Data())
 
+            if not metaonly:
+                rtmp = dataset.read(i)
 
-def data_merge(idir, sfile='', singleband=False, method='median', fdiff=True):
-    """Test Merge."""
-    app = QtWidgets.QApplication(sys.argv)
+                dat[-1].data = rtmp
+                dat[-1].data = np.ma.masked_invalid(dat[-1].data)
+                dat[-1].data.mask = dat[-1].data.mask | (dat[-1].data == nval)
+                if dat[-1].data.mask.size == 1:
+                    dat[-1].mask = np.ma.getmaskarray(dat[-1].data)
+                dat[-1].data = dat[-1].data.astype(np.float32)
+                dat[-1].data = dat[-1].data / 10000.
+
+            dat[-1].dataid = bname
+            dat[-1].nodata = nval
+            dat[-1].meta_from_rasterio(dataset)
+            dat[-1].filename = ifile
+            dat[-1].units = 'Reflectance'
+
+            bmeta['Raster'] = dat[-1].metadata['Raster']
+            bmeta['Raster']['Sensor'] = 'Sentinel-2'
+            if 'WAVELENGTH' in bmeta and 'BANDWIDTH' in bmeta:
+                wlen = float(bmeta['WAVELENGTH'])
+                bwidth = float(bmeta['BANDWIDTH'])
+                bmeta['Raster']['WavelengthMin'] = wlen - bwidth/2
+                bmeta['Raster']['WavelengthMax'] = wlen + bwidth/2
+                dat[-1].metadata['Raster']['wavelength'] = wlen
+
+            dat[-1].metadata.update(bmeta)
 
-    DM = DataMerge()
-    DM.idir = idir
-    DM.idirlist.setText(idir)
-    DM.sfile.setText(sfile)
-    DM.singleband = singleband
-    DM.forcetype = np.float32
-
-    if method == 'first':
-        DM.rb_first.setChecked(True)
-        DM.files_diff.setChecked(fdiff)
-    elif method == 'median':
-        DM.rb_median.setChecked(True)
+            if 'SOLAR_IRRADIANCE_UNIT' in bmeta:
+                dat[-1].units = bmeta['SOLAR_IRRADIANCE_UNIT']
 
-    DM.method_change()
-    DM.settings(True)
+        dataset.close()
 
-    dat = DM.outdata['Raster']
+    if not dat:
+        dat = None
 
     return dat
 
 
-def _testdown():
-    """Continuation testing routine."""
-    import matplotlib.pyplot as plt
-    from pygmi.pfmod.grvmag3d import quick_model, calc_field
-    from IPython import get_ipython
-    get_ipython().run_line_magic('matplotlib', 'inline')
-
-    h = 4
-    dxy = 1
-    magcalc = True
-
-    # quick model
-    lmod = quick_model(numx=100, numy=100, numz=10, dxy=dxy, d_z=1)
-    lmod.lith_index[45:55, :, 1] = 1
-    lmod.lith_index[45:50, :, 0] = 1
-    lmod.ght = 10
-    lmod.mht = 10
-    calc_field(lmod, magcalc=magcalc)
-    if magcalc:
-        z = lmod.griddata['Calculated Magnetics']
-        z.data = z.data + 5
-    else:
-        z = lmod.griddata['Calculated Gravity']
-
-    # Calculate the field
-    lmod = quick_model(numx=100, numy=100, numz=10, dxy=dxy, d_z=1)
-    lmod.lith_index[45:55, :, 1] = 1
-    lmod.lith_index[45:50, :, 0] = 1
-    lmod.ght = 10 - h
-    lmod.mht = 10 - h
-    calc_field(lmod, magcalc=magcalc)
-    if magcalc:
-        downz0 = lmod.griddata['Calculated Magnetics']
-        downz0.data = downz0.data + 5
-    else:
-        downz0 = lmod.griddata['Calculated Gravity']
-
-    downz0, z = z, downz0
-
-    dz = verticalp(z, order=1)
-    dz2 = verticalp(z, order=2)
-    dz3 = verticalp(z, order=3)
-
-    # normal downward
-    zdownn = fftcont(z, h)
-
-    # downward, taylor
-    h = -h
-    zdown = (z.data + h*dz + h**2*dz2/math.factorial(2) +
-             h**3*dz3/math.factorial(3))
-
-    # Plotting
-    plt.plot(downz0.data[50], 'r.')
-    # plt.plot(zdown.data[50], 'b')
-    plt.plot(zdownn.data[50], 'k')
-    plt.show()
-
-
-def _testgrid():
+def get_aster_zip(ifile, piter=None, showlog=print, tnames=None,
+                  metaonly=False):
     """
-    Test routine.
+    Get ASTER zip Data.
+
+    Parameters
+    ----------
+    ifile : str
+        filename to import
+    piter : iter, optional
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    tnames : list, optional
+        list of band names to import, in order. The default is None.
+    metaonly : bool, optional
+        Retrieve only the metadata for the file. The default is False.
 
     Returns
     -------
-    None.
-
+    dat : PyGMI raster Data
+        dataset imported
     """
-    from pygmi.raster.iodefs import get_raster
-    from pygmi.misc import PTime
-    import matplotlib.pyplot as plt
+    if piter is None:
+        piter = ProgressBarText().iter
 
-    ttt = PTime()
+    satbands = {'1': [520, 600],
+                '2': [630, 690],
+                '3N': [780, 860],
+                '3B': [780, 860],
+                '4': [1600, 1700],
+                '5': [2145, 2185],
+                '6': [2185, 2225],
+                '7': [2235, 2285],
+                '8': [2295, 2365],
+                '9': [2360, 2430],
+                '10': [8125, 8475],
+                '11': [8475, 8825],
+                '12': [8925, 9275],
+                '13': [10250, 10950],
+                '14': [10950, 11650]}
+
+    if 'AST_07' in ifile:
+        scalefactor = 0.001
+        units = 'Surface Reflectance'
+    elif 'AST_05' in ifile:
+        scalefactor = 0.001
+        units = 'Surface Emissivity'
+    elif 'AST_08' in ifile:
+        scalefactor = 0.1
+        units = 'Surface Kinetic Temperature'
+    else:
+        return None
 
-    ifile = r'd:\Work\Workdata\upward\EB_MTEF_Mag_IGRFrem.ers'
-    dat = get_raster(ifile)[0]
+    showlog('Extracting zip...')
 
-    nr, nc = dat.data.shape
+    idir = os.path.dirname(ifile)
+    with zipfile.ZipFile(ifile) as zfile:
+        zipnames = zfile.namelist()
+        zfile.extractall(idir)
+
+    platform = os.path.basename(ifile).split('_')[1]
+
+    if 'VNIR' in zipnames[0]:
+        platform += ' VNIR'
+    elif 'SWIR' in zipnames[0]:
+        platform += ' SWIR'
 
-    datamedian = np.ma.median(dat.data)
-    ndat = dat.data - datamedian
+    dat = []
+    nval = 0
+    for zfile in piter(zipnames):
+        if zfile.lower()[-4:] != '.tif':
+            continue
 
-    cdiff = nc//2
-    rdiff = nr//2
+        bname = zfile[zfile.index('Band'):zfile.index('.tif')]
+        if tnames is not None and bname not in tnames:
+            continue
 
-    # Section to pad data
+        dataset1 = rasterio.open(os.path.join(idir, zfile))
+        if dataset1 is None:
+            showlog('Problem with '+zfile)
+            continue
 
-    z1 = np.zeros((nr+2*rdiff, nc+2*cdiff))+np.nan
-    x1, y1 = np.mgrid[0: nr+2*rdiff, 0: nc+2*cdiff]
-    z1[rdiff:-rdiff, cdiff:-cdiff] = ndat.filled(np.nan)
+        dataset = rasterio.vrt.WarpedVRT(dataset1)
 
-    ttt.since_last_call('Preparation')
+        dat.append(Data())
 
-    for j in range(2):
-        z1[0] = 0
-        z1[-1] = 0
-        z1[:, 0] = 0
-        z1[:, -1] = 0
+        if metaonly is False:
+            dat[-1].data = dataset.read(1)
+            dat[-1].data = np.ma.masked_invalid(dat[-1].data)*scalefactor
+            dat[-1].data.mask = dat[-1].data.mask | (dat[-1].data == nval)
+            if dat[-1].data.mask.size == 1:
+                dat[-1].mask = np.ma.getmaskarray(dat[-1].data)
+
+        dat[-1].dataid = bname
+        dat[-1].nodata = nval
+        dat[-1].meta_from_rasterio(dataset)
+        dat[-1].filename = ifile
+        dat[-1].units = units
+
+        bmeta = dat[-1].metadata['Raster']
+        fext = dat[-1].dataid[4:]
+
+        bmeta['Sensor'] = f'ASTER {platform}'
+        bmeta['WavelengthMin'] = satbands[fext][0]
+        bmeta['WavelengthMax'] = satbands[fext][1]
+        bmeta['wavelength'] = (satbands[fext][1]+satbands[fext][1])/2
+
+        dataset.close()
+        dataset1.close()
+
+    showlog('Cleaning Extracted zip files...')
+    for zfile in zipnames:
+        os.remove(os.path.join(idir, zfile))
 
-        vert = np.zeros_like(z1)
-        hori = np.zeros_like(z1)
+    return dat
 
-        for i in range(z1.shape[0]):
-            mask = ~np.isnan(z1[i])
-            y = y1[i][mask]
-            z = z1[i][mask]
-            hori[i] = np.interp(y1[i], y, z)
 
-        for i in range(z1.shape[1]):
-            mask = ~np.isnan(z1[:, i])
-            x = x1[:, i][mask]
-            z = z1[:, i][mask]
+def get_aster_hdf(ifile, piter=None, showlog=print, tnames=None,
+                  metaonly=False):
+    """
+    Get ASTER hdf Data.
 
-            vert[:, i] = np.interp(x1[:, i], x, z)
+    Parameters
+    ----------
+    ifile : str
+        filename to import
+    piter : iter, optional
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    tnames : list, optional
+        list of band names to import, in order. The default is None.
+    metaonly : bool, optional
+        Retrieve only the metadata for the file. The default is False.
 
-        hori[hori == 0] = np.nan
-        vert[vert == 0] = np.nan
+    Returns
+    -------
+    dat : PyGMI raster Data
+        dataset imported
+    """
+    if piter is None:
+        piter = ProgressBarText().iter
 
-        hv = hori.copy()
-        hv[np.isnan(hori)] = vert[np.isnan(hori)]
-        hv[~np.isnan(hv)] = np.nanmean([hori[~np.isnan(hv)],
-                                        vert[~np.isnan(hv)]], 0)
+    satbands = {'1': [520, 600],
+                '2': [630, 690],
+                '3N': [780, 860],
+                '3B': [780, 860],
+                '4': [1600, 1700],
+                '5': [2145, 2185],
+                '6': [2185, 2225],
+                '7': [2235, 2285],
+                '8': [2295, 2365],
+                '9': [2360, 2430],
+                '10': [8125, 8475],
+                '11': [8475, 8825],
+                '12': [8925, 9275],
+                '13': [10250, 10950],
+                '14': [10950, 11650]}
+
+    ifile = ifile[:]
+
+    if 'AST_07' in ifile:
+        ptype = '07'
+    elif 'AST_L1T' in ifile:
+        ptype = 'L1T'
+    elif 'AST_05' in ifile:
+        ptype = '05'
+    elif 'AST_08' in ifile:
+        ptype = '08'
+    else:
+        return None
+    with rasterio.open(ifile) as dataset:
+        meta = dataset.tags()
+        subdata = dataset.subdatasets
+
+    if ptype == 'L1T':
+        ucc = {'ImageData1': float(meta['INCL1']),
+               'ImageData2': float(meta['INCL2']),
+               'ImageData3N': float(meta['INCL3N']),
+               'ImageData4': float(meta['INCL4']),
+               'ImageData5': float(meta['INCL5']),
+               'ImageData6': float(meta['INCL6']),
+               'ImageData7': float(meta['INCL7']),
+               'ImageData8': float(meta['INCL8']),
+               'ImageData9': float(meta['INCL9']),
+               'ImageData10': float(meta['INCL10']),
+               'ImageData11': float(meta['INCL11']),
+               'ImageData12': float(meta['INCL12']),
+               'ImageData13': float(meta['INCL13']),
+               'ImageData14': float(meta['INCL14'])}
+
+    solarelev = float(meta['SOLARDIRECTION'].split()[1])
+    cdate = meta['CALENDARDATE']
+    if len(cdate) == 8:
+        fmt = '%Y%m%d'
+    else:
+        fmt = '%Y-%m-%d'
+    dte = datetime.datetime.strptime(cdate, fmt)
+    jdate = dte.timetuple().tm_yday
+
+    if ptype == '07':
+        subdata = [i for i in subdata if 'SurfaceReflectance' in i]
+        scalefactor = 0.001
+        units = 'Surface Reflectance'
+    elif ptype == '05':
+        subdata = [i for i in subdata if 'SurfaceEmissivity' in i]
+        scalefactor = 0.001
+        units = 'Surface Emissivity'
+    elif ptype == '08':
+        scalefactor = 0.1
+        units = 'Surface Kinetic Temperature'
+    elif ptype == 'L1T':
+        subdata = [i for i in subdata if 'ImageData' in i]
+        scalefactor = 1
+        units = ''
+    else:
+        return None
 
-        z1[np.isnan(z1)] = hv[np.isnan(z1)]
+    platform = os.path.basename(ifile).split('_')[1]
 
-    plt.imshow(z1)
-    plt.show()
+    if 'VNIR' in subdata[0]:
+        platform += ' VNIR'
+    elif 'SWIR' in subdata[0]:
+        platform += ' SWIR'
 
-    ttt.since_last_call('Griddata, nearest')
+    dat = []
+    nval = 0
+    calctoa = False
+    for bfile in piter(subdata):
+        if 'QA' in bfile:
+            continue
+        if ptype == 'L1T' and 'ImageData3B' in bfile:
+            continue
 
+        bname = bfile.split(':')[-1]
+        if tnames is not None and bname not in tnames:
+            continue
 
-def _testfft():
-    """Test FFT."""
-    import matplotlib.pyplot as plt
-    from matplotlib import colormaps
-    import scipy
-    from IPython import get_ipython
-    from pygmi.raster.iodefs import get_raster
-
-    get_ipython().run_line_magic('matplotlib', 'inline')
-
-    ifile = r'D:\Workdata\geothermal\bushveldrtp.hdr'
-    data = get_raster(ifile)[0]
-
-    # quick model
-    plt.imshow(data.data, cmap=colormaps['jet'], vmin=-500, vmax=500)
-    plt.colorbar()
-    plt.show()
+        dat.append(Data())
 
-    # Start new stuff
-    xdim = data.xdim
-    ydim = data.ydim
+        dataset1 = rasterio.open(bfile)
+        dataset = rasterio.vrt.WarpedVRT(dataset1)
 
-    ndat, rdiff, cdiff, datamedian = fftprep(data)
+        if metaonly is False:
+            dat[-1].data = dataset.read(1)
+            if ptype == '08':
+                dat[-1].data[dat[-1].data == 2000] = nval
+            dat[-1].data = np.ma.masked_invalid(dat[-1].data)*scalefactor
+            dat[-1].data.mask = dat[-1].data.mask | (dat[-1].data == nval)
+            if dat[-1].data.mask.size == 1:
+                dat[-1].mask = np.ma.getmaskarray(dat[-1].data)
+
+        dat[-1].meta_from_rasterio(dataset)
+
+        dataset.close()
+        dataset1.close()
+
+        dat[-1].dataid = bname
+        dat[-1].nodata = nval
+        dat[-1].metadata['SolarElev'] = solarelev
+        dat[-1].metadata['JulianDay'] = jdate
+        dat[-1].metadata['CalendarDate'] = cdate
+        dat[-1].metadata['ShortName'] = meta['SHORTNAME']
+        dat[-1].filename = ifile
+        dat[-1].units = units
+
+        if 'band' in dat[-1].dataid.lower():
+            bmeta = dat[-1].metadata['Raster']
+            fext = dat[-1].dataid[4:].split()[0]
+
+            platform = os.path.basename(ifile).split('_')[1]
+            bmeta['Sensor'] = f'ASTER {platform}'
+
+            bmeta['WavelengthMin'] = satbands[fext][0]
+            bmeta['WavelengthMax'] = satbands[fext][1]
+            bmeta['wavelength'] = (satbands[fext][1] + satbands[fext][1])/2
+
+            if ptype == 'L1T' and 'ImageData' in ifile:
+                dat[-1].metadata['Gain'] = ucc[ifile[ifile.rindex('ImageData'):]]
+                calctoa = True
 
-    datamedian = np.ma.median(data.data)
-    ndat = data.data - datamedian
+    if not dat:
+        dat = None
 
-    fftmod = np.fft.fft2(ndat)
+    elif ptype == 'L1T' and calctoa is True:
+        dat = calculate_toa(dat)
 
-    KX, KY = fft_getkxy(fftmod, xdim, ydim)
+    showlog('Import complete')
+    return dat
 
-    vmin = fftmod.real.mean()-2*fftmod.real.std()
-    vmax = fftmod.real.mean()+2*fftmod.real.std()
-    plt.imshow(np.fft.fftshift(fftmod.real), vmin=vmin, vmax=vmax)
-    plt.show()
 
-    knrm = np.sqrt(KX**2+KY**2)
+def get_aster_ged(ifile, piter=None, showlog=print, tnames=None,
+                  metaonly=False):
+    """
+    Get ASTER GED data.
 
-    plt.imshow(knrm)
+    Parameters
+    ----------
+    ifile : str
+        filename to import
+    piter : iter, optional
+        Progress bar iterable. Default is None.
+    showlog : function, optional
+        Routine to show text messages. The default is print.
+    tnames : list, optional
+        list of band names to import, in order. The default is None.
+    metaonly : bool, optional
+        Retrieve only the metadata for the file. The default is False.
 
-    plt.show()
+    Returns
+    -------
+    dat : PyGMI raster Data
+        dataset imported
+    """
+    if piter is None:
+        piter = ProgressBarText().iter
 
-    knrm = knrm.flatten()
-    fftamp = np.abs(fftmod)**2
-    fftamp = fftamp.flatten()
+    dat = []
+    ifile = ifile[:]
 
-    plt.plot(knrm, fftamp, '.')
-    plt.yscale('log')
-    plt.show()
+    with rasterio.open(ifile) as dataset:
+        subdata = dataset.subdatasets
 
-    bins = max(fftmod.shape)//2
+    i = -1
+    for ifile2 in subdata:
+        dataset = rasterio.open(ifile2)
+        units = ''
+
+        if 'ASTER_GDEM' in ifile2:
+            bandid = 'ASTER GDEM'
+            units = 'meters'
+        if 'Land_Water_Map' in ifile2:
+            bandid = 'Land_water_map'
+        if 'Observations' in ifile2:
+            bandid = 'Observations'
+            units = 'number per pixel'
 
-    abins, bedge, _ = scipy.stats.binned_statistic(knrm, fftamp,
-                                                   statistic='mean',
-                                                   bins=bins)
-
-    bins = (bedge[:-1] + bedge[1:])/2
-    plt.plot(bins, abins)
-    plt.yscale('log')
-    plt.show()
+        if tnames is not None and bandid not in tnames:
+            continue
 
+        nbands = 1
 
-def _testmerge():
-    """Test Merge."""
-    from pygmi.raster.iodefs import export_raster
+        if metaonly is False:
+            rtmp2 = dataset.read()
+            if 'Latitude' in ifile2:
+                ymax = rtmp2.max()
+                ydim = abs((rtmp2.max()-rtmp2.min())/rtmp2.shape[1])
+                continue
 
-    app = QtWidgets.QApplication(sys.argv)
+            if 'Longitude' in ifile2:
+                xmin = rtmp2.min()
+                xdim = abs((rtmp2.max()-rtmp2.min())/rtmp2.shape[2])
+                continue
 
-    # sfile = r"E:\WorkProjects\ST-2022-1355 Onshore Mapping\Niger\shapefiles\Agadez_block.shp"
-    # idir = r"E:\WorkProjects\ST-2022-1355 Onshore Mapping\Niger\Landsat_9\PCA"
-    # ifilt = r"E:/WorkProjects/ST-2022-1355 Onshore Mapping/Niger/Landsat_9/RGB*/"
+            if rtmp2.shape[-1] == min(rtmp2.shape) and rtmp2.ndim == 3:
+                rtmp2 = np.transpose(rtmp2, (2, 0, 1))
 
-    # sfile = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\Mining-areas.shp"
-    # idir = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\WV2-2021"
+            if rtmp2.ndim == 3:
+                nbands = rtmp2.shape[0]
 
-    idir = r'D:\Workdata\PyGMI Test Data\Raster\mosaic'
+        for i2 in range(nbands):
+            nval = -9999
+            i += 1
+
+            dat.append(Data())
+            if metaonly is False:
+                if rtmp2.ndim == 3:
+                    dat[i].data = rtmp2[i2]
+                else:
+                    dat[i].data = rtmp2
 
-    # idirs = glob.glob(ifilt)
-    idirs = [idir]
+            dat[i].data = np.ma.masked_invalid(dat[i].data)
+            dat[i].data.mask = (np.ma.getmaskarray(dat[i].data)
+                                | (dat[i].data == nval))
+            if dat[i].data.mask.size == 1:
+                dat[-1].mask = np.ma.getmaskarray(dat[-1].data)
+
+            dat[i].data = dat[i].data * 1.0
+            if 'Emissivity/Mean' in ifile2:
+                bandid = 'Emissivity_mean_band_'+str(10+i2)
+                dat[i].data = dat[i].data * 0.001
+            if 'Emissivity/SDev' in ifile2:
+                bandid = 'Emissivity_std_dev_band_'+str(10+i2)
+                dat[i].data = dat[i].data * 0.0001
+            if 'NDVI/Mean' in ifile2:
+                bandid = 'NDVI_mean'
+                dat[i].data = dat[i].data * 0.01
+            if 'NDVI/SDev' in ifile2:
+                bandid = 'NDVI_std_dev'
+                dat[i].data = dat[i].data * 0.01
+            if 'Temperature/Mean' in ifile2:
+                bandid = 'Temperature_mean'
+                units = 'Kelvin'
+                dat[i].data = dat[i].data * 0.01
+            if 'Temperature/SDev' in ifile2:
+                bandid = 'Temperature_std_dev'
+                units = 'Kelvin'
+                dat[i].data = dat[i].data * 0.01
+
+            dat[i].dataid = bandid
+            dat[i].nodata = nval
+            dat[i].crs = CRS.from_epsg(4326)  # WGS84 geodetic
+            dat[i].units = units
+            dat[i].metadata['Raster']['Sensor'] = 'ASTER GED'
+        dataset.close()
+
+    if metaonly is False:
+        for i in dat:
+            i.set_transform(xdim, xmin, ydim, ymax)
 
-    for idir in idirs:
-        print(idir)
-        DM = DataMerge()
-        DM.idir = idir
-        DM.idirlist.setText(idir)
-        # DM.sfile.setText(sfile)
-        # DM.singleband = True
+    showlog('Import complete')
+    return dat
 
-        DM.forcetype = np.float32
-        DM.settings()
 
-        dat = DM.outdata['Raster']
+def get_aster_ged_bin(ifile):
+    """
+    Get ASTER GED binary format.
 
-        del DM
+    Emissivity_Mean_Description: Mean Emissivity for each pixel on grid-box
+    using all ASTER data from 2000-2010
+    Emissivity_SDev_Description: Emissivity Standard Deviation for each pixel
+    on grid-box using all ASTER data from 2000-2010
+    Temperature_Mean_Description: Mean Temperature (K) for each pixel on
+    grid-box using all ASTER data from 2000-2010
+    Temperature_SDev_Description: Temperature Standard Deviation for each pixel
+    on grid-box using all ASTER data from 2000-2010
+    NDVI_Mean_Description: Mean NDVI for each pixel on grid-box using all ASTER
+    data from 2000-2010
+    NDVI_SDev_Description: NDVI Standard Deviation for each pixel on grid-box
+    using all ASTER data from 2000-2010
+    Land_Water_Map_LWmap_Description: Land Water Map using ASTER visible bands
+    Observations_NumObs_Description: Number of values used in computing mean
+    and standard deviation for each pixel.
+    Geolocation_Latitude_Description: Latitude
+    Geolocation_Longitude_Description: Longitude
+    ASTER_GDEM_ASTGDEM_Description: ASTER GDEM resampled to NAALSED
 
-        if dat:
-            ofile = idir+'.tif'
-            # export_raster(ofile, dat, 'GTiff', compression='ZSTD')
-            del dat
+    Parameters
+    ----------
+    ifile : str
+        filename to import
 
+    Returns
+    -------
+    dat : PyGMI raster Data
+        dataset imported
+    """
+    dat = []
+    nval = -9999
+    bandid = {}
 
-def _testreproj():
-    """Test Reprojection."""
-    from pygmi.raster.iodefs import get_raster
-    import matplotlib.pyplot as plt
+    bandid[0] = 'Emissivity_mean_band_10'
+    bandid[1] = 'Emissivity_mean_band_11'
+    bandid[2] = 'Emissivity_mean_band_12'
+    bandid[3] = 'Emissivity_mean_band_13'
+    bandid[4] = 'Emissivity_mean_band_14'
+    bandid[5] = 'Emissivity_std_dev_band_10'
+    bandid[6] = 'Emissivity_std_dev_band_11'
+    bandid[7] = 'Emissivity_std_dev_band_12'
+    bandid[8] = 'Emissivity_std_dev_band_13'
+    bandid[9] = 'Emissivity_std_dev_band_14'
+    bandid[10] = 'Temperature_mean'
+    bandid[11] = 'Temperature_std_dev'
+    bandid[12] = 'NDVI_mean'
+    bandid[13] = 'NDVI_std_dev'
+    bandid[14] = 'Land_water_map'
+    bandid[15] = 'Observations'
+    bandid[16] = 'Latitude'
+    bandid[17] = 'Longitude'
+    bandid[18] = 'ASTER GDEM'
+
+    scale = [0.001, 0.001, 0.001, 0.001, 0.001,
+             0.0001, 0.0001, 0.0001, 0.0001, 0.0001,
+             0.01, 0.01, 0.01, 0.01,
+             1, 1, 0.001, 0.001, 1]
+
+    units = ['', '', '', '', '', '', '', '', '', '', 'Kelvin', 'Kelvin',
+             '', '', '', 'Number per pixel', 'degrees', 'degrees', 'meters']
+
+    data = np.fromfile(ifile, dtype=np.int32)
+    rows_cols = int((data.size/19)**0.5)
+    data.shape = (19, rows_cols, rows_cols)
+
+    lats = data[16]*scale[16]
+    lons = data[17]*scale[17]
+
+    latsdim = (lats.max()-lats.min())/(lats.shape[0]-1)
+    lonsdim = (lons.max()-lons.min())/(lons.shape[0]-1)
+
+    tlx = lons.min()-abs(lonsdim/2)
+    tly = lats.max()+abs(latsdim/2)
+
+    for i in range(19):
+        dat.append(Data())
+
+        dat[i].data = data[i]*scale[i]
+
+        dat[i].dataid = bandid[i]
+        dat[i].nodata = nval*scale[i]
+        dat[i].xdim = lonsdim
+        dat[i].ydim = latsdim
+        dat[i].units = units[i]
+
+        rows, cols = dat[i].data.shape
+        xmin = tlx
+        ymax = tly
+        ymin = ymax - rows*dat[i].ydim
+        xmax = xmin + cols*dat[i].xdim
 
-    ifile = r""
+        dat[i].extent = [xmin, xmax, ymin, ymax]
 
-    piter = ProgressBarText().iter
+    dat.pop(17)
+    dat.pop(16)
 
-    dat = get_raster(ifile, piter=piter)
+    return dat
 
-    app = QtWidgets.QApplication(sys.argv)
 
-    DM = DataReproj()
-    DM.indata['Raster'] = dat
-    DM.settings()
+def get_ternary(dat, sunfile=None, clippercl=1., clippercu=1.,
+                cell=25., alpha=.75, piter=iter, showlog=print):
+    """
+    Create a ternary image, with optional sunshading.
 
-    plt.figure(dpi=150)
-    plt.imshow(DM.indata['Raster'][0].data,
-               extent=DM.indata['Raster'][0].extent)
-    plt.colorbar()
-    plt.show()
+    Parameters
+    ----------
+    dat : list
+        PyGMI Data.
+    sunfile : str, optional
+        Sunshading band or filename. The default is None.
+    clippercl : float, optional
+        Lower clip percentage for colour bar. The default is 1.
+    clippercu : float, optional
+        Upper clip percentage for colour bar. The default is 1.
+    cell : float, optional
+        Between 1 and 100 - controls sunshade detail. The default is 25.
+    alpha : float, optional
+        How much incident light is reflected (0 to 1). The default is .75.
 
-    plt.figure(dpi=150)
-    plt.imshow(DM.outdata['Raster'][0].data,
-               extent=DM.outdata['Raster'][0].extent)
-    plt.colorbar()
-    plt.show()
+    Returns
+    -------
+    newimg : list
+        list of PyGMI data.
 
+    """
+    data = lstack(dat, nodeepcopy=True, checkdataid=False, piter=piter,
+                  showlog=showlog)
+    sundata = None
+
+    if sunfile is not None:
+        sdata = None
+        for i in data:
+            if i.dataid == sunfile:
+                sdata = i
+                break
 
-def _testcut():
-    """Test Reprojection."""
-    from pygmi.raster.iodefs import get_raster, export_raster
-    import matplotlib.pyplot as plt
+        if sdata is None:
+            sundata = get_raster(sunfile, metaonly=True, piter=piter,
+                                 showlog=showlog)
 
-    sfile = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\NRFproj\Mining-areas.shp"
-    ifile = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\2016mosaic.tif"
-    ofile = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\2016mines.tif"
+            owkt = sundata[0].crs.to_wkt()
+            iwkt = data[0].crs.to_wkt()
 
-    dat = get_raster(ifile)
+            x = data[0].extent[:2]
+            y = data[0].extent[2:]
 
-    for i in dat:
-        i.data = i.data.astype(np.float32)
+            xx, yy = reprojxy(x, y, iwkt, owkt)
 
+            bounds = [xx[0], yy[0], xx[1], yy[1]]
 
-    dat = cut_raster(dat, sfile, deepcopy=False)
+            sundata = get_raster(sunfile, bounds=bounds, piter=piter,
+                                 showlog=showlog)
+            sundata = data_reproject(sundata[0], data[0].crs)
 
-    # app = QtWidgets.QApplication(sys.argv)
+            sdata = [data[0], sundata]
+            masterid = sdata[0].dataid
+            sdata = lstack(sdata, nodeepcopy=True, masterid=masterid,
+                           resampling='bilinear', checkdataid=False,
+                           piter=piter, showlog=showlog)[1]
 
-    # DM = DataCut()
-    # DM.indata['Raster'] = dat
-    # DM.ifile = sfile
-    # DM.settings(nodialog=True)
+    red = data[0].data
+    green = data[1].data
+    blue = data[2].data
 
-    export_raster(ofile, dat, compression='ZSTD')
+    mask = np.logical_or(red.mask, green.mask)
+    mask = np.logical_or(mask, blue.mask)
+    mask = np.logical_not(mask)
 
-    # plt.figure(dpi=150)
-    # plt.imshow(DM.indata['Raster'][0].data,
-    #            extent=DM.indata['Raster'][0].extent)
-    # plt.colorbar()
-    # plt.show()
+    red, _, _ = histcomp(red, perc=clippercl, uperc=clippercu)
+    green, _, _ = histcomp(green, perc=clippercl, uperc=clippercu)
+    blue, _, _ = histcomp(blue, perc=clippercl, uperc=clippercu)
 
-    # plt.figure(dpi=150)
-    # plt.imshow(DM.outdata['Raster'][0].data,
-    #            extent=DM.outdata['Raster'][0].extent)
-    # plt.colorbar()
-    # plt.show()
+    img = np.ones((red.shape[0], red.shape[1], 4), dtype=np.uint8)
+    img[:, :, 3] = mask*254+1
 
+    img[:, :, 0] = norm255(red)
+    img[:, :, 1] = norm255(green)
+    img[:, :, 2] = norm255(blue)
 
-def _testprof():
-    """Test Reprojection."""
-    from pygmi.raster.iodefs import get_raster
-    import matplotlib.pyplot as plt
+    phi = -np.pi/4.
+    theta = np.pi/4.
 
-    ifile = r"d:\Workdata\bugs\Au5_SRTM30_utm36s.tif"
-    sfile = r"d:\Workdata\bugs\Profiles_utm36s.shp"
+    # sundata = None
+    if sundata is not None:
+        sunshader = currentshader(sdata.data, cell, theta, phi, alpha)
 
-    piter = ProgressBarText().iter
+        snorm = norm2(sunshader)
 
-    dat = get_raster(ifile, piter=piter)
+        img[:, :, 0] = img[:, :, 0]*snorm  # red
+        img[:, :, 1] = img[:, :, 1]*snorm  # green
+        img[:, :, 2] = img[:, :, 2]*snorm  # blue
+        img = img.astype(np.uint8)
 
-    app = QtWidgets.QApplication(sys.argv)
+    # plt.figure(dpi=150)
+    # plt.imshow(img)
+    # plt.show()
 
-    DM = GetProf()
-    DM.indata['Raster'] = dat
-    DM.ifile = sfile
-    DM.settings(nodialog=True)
+    newimg = [copy.deepcopy(data[0]),
+              copy.deepcopy(data[0]),
+              copy.deepcopy(data[0]),
+              copy.deepcopy(data[0])]
 
-    plt.figure(dpi=150)
-    plt.imshow(DM.indata['Raster'][0].data,
-               extent=DM.indata['Raster'][0].extent)
-    plt.colorbar()
-    plt.show()
+    newimg[0].data = img[:, :, 0]
+    newimg[1].data = img[:, :, 1]
+    newimg[2].data = img[:, :, 2]
+    newimg[3].data = img[:, :, 3]
 
-    plt.figure(dpi=150)
-    plt.imshow(DM.outdata['Raster'][0].data,
-               extent=DM.outdata['Raster'][0].extent)
-    plt.colorbar()
-    plt.show()
+    mask = img[:, :, 3]
+    newimg[0].data[newimg[0].data == 0] = 1
+    newimg[1].data[newimg[1].data == 0] = 1
+    newimg[2].data[newimg[2].data == 0] = 1
 
+    newimg[0].data[mask <= 1] = 0
+    newimg[1].data[mask <= 1] = 0
+    newimg[2].data[mask <= 1] = 0
 
-def _testlstack():
-    from pygmi.raster.iodefs import get_raster, export_raster
-    import matplotlib.pyplot as plt
+    newimg[0].nodata = 0
+    newimg[1].nodata = 0
+    newimg[2].nodata = 0
+    newimg[3].nodata = 0
 
-    idir = r'd:\Workdata\LULC\stack'
+    newimg[0].dataid = data[0].dataid
+    newimg[1].dataid = data[1].dataid
+    newimg[2].dataid = data[2].dataid
+    newimg[3].dataid = 'Alpha'
 
-    ifiles = glob.glob(os.path.join(idir, '*.tif'))
+    return newimg
 
-    dat = []
-    for ifile in ifiles:
-        dat += get_raster(ifile)
 
-    for i in dat:
-        plt.figure(dpi=150)
-        plt.title(i.dataid)
-        plt.imshow(i.data)
-        plt.colorbar()
-        plt.show()
-        print(i.nodata)
-        print(i.data.dtype)
+def set_export_filename(dat, odir, otype=None):
+    """
+    Set the export filename according to convention.
 
-    dat2 = lstack(dat, dxy=30)
+    Different satellite products have different simplified conventions for
+    output filenames to avoid names getting too long.
 
-    for i in dat2:
-        plt.figure(dpi=150)
-        plt.title(i.dataid)
-        plt.imshow(i.data)
-        plt.colorbar()
-        plt.show()
-        print(i.nodata)
-        print(i.data.dtype)
+    Parameters
+    ----------
+    dat : list
+        List of PyGMI data.
+    odir : str
+        Output directory.
+    otype : str, optional.
+        Output file type. Default is None.
 
-    ofile = r'd:/Workdata/LULC/2001_stack_norm_pc.tif'
-    export_raster(ofile, dat2, 'GTiff')
+    Returns
+    -------
+    ofile : str
+        Output file name.
 
+    """
+    sensor = dat[0].metadata['Raster']['Sensor']
+    filename = os.path.basename(dat[0].filename)
+    filename = os.path.splitext(filename)[0]
 
-def _testcut2():
-    """Test Reprojection."""
-    from pygmi.raster.iodefs import get_raster, export_raster
+    filename = filename.replace('_stack', '')
+    filename = filename.replace('_ratio', '')
 
-    sfile = r"D:\hypercut\shape\Areas_utm33s_east.shp"
-    ifilt = r"D:\hypercut\*.hdr"
-    odir = r"D:\hypercut\cut"
+    if otype is None:
+        otype = 'stack'
 
-    pprint = print
+    if 'ASTER' in sensor:
+        tmp = [os.path.basename(i.filename).split('_')[1] for i in dat]
+        tmp = list(set(tmp))
+        tmp.sort()
+        plev = ''
+        for i in tmp:
+            plev += f'_{i}'
 
-    ifiles = glob.glob(ifilt)
+        tmp = filename.split('_')
+        month = tmp[2][3:5]
+        day = tmp[2][5:7]
+        year = tmp[2][7:11]
+        uid = tmp[-1]
+        ofile = f'AST{plev}_{year}{month}{day}_{uid}'
+    elif 'Landsat' in sensor:
+        ofile = '_'.join(filename.split('_')[:4])
+    elif 'Sentinel-2' in sensor:
+        tmp = filename.split('_')
+        mission = tmp[0]
+        date = tmp[2].split('T')[0]
+        tile = tmp[5]
+        ofile = f'{mission}_{tile}_{date}'
+    else:
+        ofile = filename
 
-    for ifile in ifiles:
-        print(ifile)
-        gdf = gpd.read_file(sfile)
+    if otype == 'RGB':
+        tmp = [i.dataid.split()[0] for i in dat]
+        for i in tmp:
+            ofile += f'_{i.lower().replace("band", "b")}'
+    else:
+        ofile += f'_{otype}'
 
-        gdf = gdf[gdf.geometry != None]
+    ofile = os.path.join(odir, ofile)
 
-        if gdf.geom_type.iloc[0] == 'MultiPolygon':
-            pprint('You have a MultiPolygon. Only the first Polygon '
-                   'of the MultiPolygon will be used.')
-            poly = gdf['geometry'].iloc[0]
-            tmp = poly.geoms[0]
+    return ofile
 
-            gdf.geometry.iloc[0] = tmp
 
-        if gdf.geom_type.iloc[0] != 'Polygon':
-            pprint('You need a polygon in that shape file')
-            return
+def utm_to_south(dat):
+    """
+    Make sure all UTM labels are for southern hemisphere.
 
-        bounds = gdf.geometry.iloc[0].bounds
+    Parameters
+    ----------
+    dat : list
+        List fo Data.
 
-        dat = get_raster(ifile, bounds=bounds)
+    Returns
+    -------
+    dat : list
+        List of Data.
 
-        if dat is None:
+    """
+    for band in dat:
+        epsgcode = band.crs.to_epsg()
+        if epsgcode is None:
             continue
+        if 32600 <= epsgcode <= 32660:
+            epsgcode += 100
+            band.crs = CRS.from_epsg(epsgcode)
+
+            left, right, bottom, top = band.extent
+            top = top + 10000000
+            bottom = bottom + 10000000
+            xdim = band.xdim
+            ydim = band.ydim
+
+            band.transform = Affine(xdim, 0, left, 0, -ydim, top)
+            band.extent = (left, right, bottom, top)
+            band.bounds = (left, bottom, right, top)
 
-        for idat in dat:
-            idat.nodata = 0
-
-        ofile = os.path.join(odir, os.path.basename(ifile))
-        ofile = ofile[:-4]+'new.tif'
-        export_raster(ofile, dat, 'GTiff', bandsort=False)
-
-
-def _testnewnull():
-    """Test New null data assignment."""
-    from pygmi.raster.iodefs import get_raster, export_raster
-
-    ifilt = r"D:\hypercut\*.hdr"
-    odir = r"D:\hypercut\cut"
-
-    ifiles = glob.glob(ifilt)
-
-    for ifile in ifiles:
-        print(ifile)
-        dat = get_raster(ifile)
-        for idat in dat:
-            idat.nodata = 0
-            # idat.data = np.ma.masked_equal(idat.data, 0)
-
-        ofile = os.path.join(odir, os.path.basename(ifile))
-        ofile = ofile[:-4]+'.tif'
-        export_raster(ofile, dat, 'GTiff', bandsort=False)
-        # break
-
-
-def _testlower():
-    """Lowers resolution."""
-    from pygmi.raster.iodefs import get_raster
-    from pygmi.raster.iodefs import export_raster
-
-    ifilt = r"e:\WorkProjects\ST-2022-1355 Onshore Mapping\Niger\ratios\*.tif"
-    odir = r"e:\WorkProjects\ST-2022-1355 Onshore Mapping\Niger\ratios2"
-    dataid = 'B4divB2 Iron Oxide'
-
-    ifiles = glob.glob(ifilt)
-
-    for ifile in ifiles:
-        print(ifile)
-        dat = get_raster(ifile, dataid=dataid)
-        dat = lstack(dat, dxy=20)
-
-        ofile = os.path.join(odir, os.path.basename(ifile))
-        export_raster(ofile, dat, 'GTiff', compression='ZSTD')
-
-
-def _testcmask():
-    """Lowers resolution."""
-    from pygmi.raster.iodefs import get_raster
-    from pygmi.raster.iodefs import export_raster
-
-    file2019 = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\2019diff\change_2019_time1_time2_stacked.hdr"
-    file2021 = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\2021diff\change_2021_time1_time2_stacked.hdr"
-
-    ofile2016 = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\change_2016.tif"
-    ofile2019 = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\change_2019.tif"
-    ofile2021 = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\change_2021.tif"
-
-    dat2019 = get_raster(file2019)
-    for i in dat2019:
-        i.nodata = 0.
-        i.data = np.ma.masked_equal(i.data, i.data[-1, -1])
-        i.data = np.ma.filled(i.data, 0.)
-        i.data = np.ma.masked_equal(i.data, 0.)
-
-    dat2019 = dat2019[8:]
-
-    dat2021 = get_raster(file2021)
-    for i in dat2021:
-        i.nodata = 0.
-        i.data = np.ma.masked_equal(i.data, i.data[-1, -1])
-        i.data = np.ma.filled(i.data, 0.)
-        i.data = np.ma.masked_equal(i.data, 0.)
+    return dat
 
-    dat2016 = dat2021[:8]
-    dat2021 = dat2021[8:]
 
-    datall = [dat2019[0]]+dat2021
-    datall = lstack(datall, commonmask=True)
-    datall.pop(0)
-    datall = trim_raster(datall)
+def _test5P():
+    """Test routine."""
+    import matplotlib.pyplot as plt
 
-    export_raster(ofile2021, datall, 'GTiff', compression='ZSTD')
-    del dat2021
+    sfile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\Sentinel-5P\CCUS_Sept2021_25kmbuffer.shp"
+    ifile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\Sentinel-5P\S5P_OFFL_L2__CH4____20230111T102529_20230111T120700_27184_03_020400_20230113T024518.nc"
 
-    datall = [dat2019[0]]+dat2016
-    datall = lstack(datall, commonmask=True)
-    datall.pop(0)
-    datall = trim_raster(datall)
+    os.chdir(r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\Sentinel-5P")
 
-    export_raster(ofile2016, datall, 'GTiff', compression='ZSTD')
+    app = QtWidgets.QApplication(sys.argv)
+    tmp = ImportSentinel5P()
+    tmp.ifile = ifile
+    tmp.settings()
+
+    if 'Vector' not in tmp.outdata:
+        print('No data')
+        return
 
-    datall = [dat2016[0]]+dat2019
-    datall = lstack(datall, commonmask=True)
-    datall.pop(0)
-    datall = trim_raster(datall)
+    shp = gpd.read_file(sfile)
+    shp = shp.to_crs(4326)
 
-    export_raster(ofile2019, datall, 'GTiff', compression='ZSTD')
+    plt.figure(dpi=150)
+    ax = plt.gca()
+    shp.plot(ax=ax, fc='none', ec='black')
 
+    # try:
+    #     ctx.add_basemap(ax, crs=shp.crs,
+    #                     source=ctx.providers.OpenStreetMap.Mapnik)
+    # except:
+    #     print('No internet')
 
-def _teststd():
-    """Calculate Standard Devation."""
-    from pygmi.raster.iodefs import get_raster
-    from pygmi.raster.iodefs import export_raster
+    tmp.outdata['Vector']['Point'].plot(ax=ax, column='data')
+    plt.show()
 
-    ifile2016 = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\change_2016_ratio.tif"
-    ifile2019 = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\change_2019_ratio.tif"
-    ifile2021 = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\change_2021_ratio.tif"
 
-    ofile = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\change_ratio_std.tif"
+def _testfn2():
+    """Test routine."""
+    app = QtWidgets.QApplication(sys.argv)
 
-    dat2016 = get_raster(ifile2016)
-    dat2019 = get_raster(ifile2019)
-    dat2021 = get_raster(ifile2021)
-    datstd = copy.deepcopy(dat2021)
+    tmp1 = ImportBatch()
+    tmp1.idir = r"D:\Landsat"
+    tmp1.get_sfile(True)
+    tmp1.settings(True)
+
+    dat = tmp1.outdata
+
+    tmp2 = ExportBatch()
+    tmp2.indata = dat
+    tmp2.get_odir(r"D:\Sentinel2\test")
+    tmp2.ternary.setChecked(True)
+    tmp2.click_ternary()
+    tmp2.run()
 
-    dat = {}
-    for band in dat2016:
-        if band.dataid not in dat:
-            dat[band.dataid] = []
-        dat[band.dataid].append(band.data)
 
-    for band in dat2019:
-        if band.dataid not in dat:
-            dat[band.dataid] = []
-        dat[band.dataid].append(band.data)
+def _testfn3():
+    """Test routine."""
+    import matplotlib.pyplot as plt
 
-    for band in dat2021:
-        if band.dataid not in dat:
-            dat[band.dataid] = []
-        dat[band.dataid].append(band.data)
+    ifile = r"D:\Sentinel1\S1A_IW_SLC__1SDV_20220207T170247_20220207T170314_041809_04F9FB_F500.SAFE"
+    ifile = r"D:\ASTER\AST_05_00307102005081903_20230417033828_30889.zip"
+    ifile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\ASTER\GED\AG100.v003.-27.022.0001.h5"
+    ifile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\MODIS\MOD16A2.A2013073.h20v11.006.2017101224330.hdf"
 
-    for band in datstd:
-        dstack = np.ma.array(dat[band.dataid])
-        band.data = dstack.std(0)
+    dat = get_data(ifile)
 
-    export_raster(ofile, datstd, 'GTiff', compression='ZSTD')
+    for i in dat:
+        plt.figure(dpi=150)
+        plt.title(i.dataid)
+        plt.imshow(i.data, extent=i.extent)
+        plt.colorbar()
+        plt.show()
 
 
 if __name__ == "__main__":
-    _testmerge()
+    _testfn2()
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/datatypes.py` & `pygmi-3.2.7.16/pygmi/raster/datatypes.py`

 * *Files 20% similar despite different names*

```diff
@@ -125,43 +125,74 @@
         grid null or no data value
     units : str
         description of units to be used with colour bars
     isrgb : bool
         Flag to signify an RGB image.
     metadata : dictionary
         Miscellaneous metadata for file.
+    meta : dictionary
+        Rasterio metadata for file.
     filename : str
         Filename of file.
     transform : list of Affine, optional
         rasterio transform. The default is None.
     crs : CRS
         rasterio crs of data
+    datetime : date
+        Date of dataset.
     """
 
     def __init__(self):
         self.data = np.ma.array([[0]])
         self.extent = None  # left, right, bottom, top
         self.bounds = None  # left, bottom, right, top
         self.xdim = None
         self.ydim = None
         self.dataid = ''
-        self.nodata = 1e+20
+        self.nodata = None
         self.units = ''
         self.isrgb = False
-        self.metadata = {'Cluster': {}, 'Raster': {}}
+        self.metadata = {'Cluster': {}, 'Raster': {'Sensor': 'Generic'}}
+        self.meta = {}  # rasterio meta
         self.filename = ''
         self.transform = None
         self.crs = None
+        self.datetime = None
 
         self.set_transform(1, 0, 1, 0)
 
+    def meta_from_rasterio(self, dataset):
+        """
+        Set transform, bounds, extent, xdim and ydim from a rasterio dataset.
+
+        Parameters
+        ----------
+        dataset : rasterio dataset
+            Rasterio dataset.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.xdim = dataset.transform[0]
+        self.ydim = abs(dataset.transform[4])
+
+        left, bottom, right, top = dataset.bounds
+
+        self.extent = (left, right, bottom, top)
+        self.bounds = (left, bottom, right, top)
+        self.transform = dataset.transform
+        self.crs = dataset.crs
+        self.meta = dataset.meta
+
     def set_transform(self, xdim=None, xmin=None, ydim=None, ymax=None,
-                      transform=None, iraster=None):
+                      transform=None, iraster=None, rows=None, cols=None):
         """
-        Set the transform.
+        Set the transform, xdim, ydim, extent and bounds.
 
         This requires either transform as input OR xdim, ydim, xmin, ymax.
 
         Parameters
         ----------
         xdim : float, optional
             x dimension. The default is None.
@@ -170,16 +201,20 @@
         ydim : float, optional
             y dimension. The default is None.
         ymax : float, optional
             y maximum. The default is None.
         transform : list of Affine, optional
             transform. The default is None.
         iraster : list, optional
-            list containing offsets etc in even of cutting data. The default
+            list containing offsets etc in event of cutting data. The default
             is None.
+        rows : int, optional
+            rows in dataset. The default is None.
+        cols : int, optional
+            columns in dataset. The default is None.
 
         Returns
         -------
         None.
 
         """
         if transform is not None:
@@ -193,16 +228,18 @@
         if iraster is None:
             xoff = 0
             yoff = 0
         else:
             xoff, yoff, _, _ = iraster
 
         # get rows and cols this way because RGB images have three dims
-        rows = self.data.shape[0]
-        cols = self.data.shape[1]
+        if rows is None:
+            rows = self.data.shape[0]
+        if cols is None:
+            cols = self.data.shape[1]
 
         left = xmin + xoff*xdim
         top = ymax - yoff*ydim
         right = left + xdim*cols
         bottom = top - ydim*rows
 
         self.transform = Affine(xdim, 0, left, 0, -ydim, top)
@@ -253,7 +290,78 @@
         """
         mean = self.data.mean()
         std = self.data.std()
         vmin = mean-2*std
         vmax = mean+2*std
 
         return vmin, vmax
+
+
+class RasterMeta():
+    """
+    PyGMI Raster Metadata Object.
+
+    Attributes
+    ----------
+    sensor : str
+        Sensor used to measure data.
+    filename : str
+        Filename of file.
+    crs : CRS
+        rasterio crs of data.
+    bands : list
+        list of bands in dataset.
+    tnames : list
+        list fo bands to process.
+    banddata : list
+        list of band data.
+    to_sutm : bool
+        flag to convert a file to SUTM.
+
+    """
+
+    def __init__(self):
+        self.sensor = 'Generic'
+        self.crs = None
+        self.filename = ''
+        self.bands = []
+        self.tnames = []
+        self.banddata = []
+        self.to_sutm = False
+
+    def fromData(self, dat):
+        """
+        Populate class from a Data class.
+
+        Parameters
+        ----------
+        dat : Data
+            PyGMI data object.
+
+        Returns
+        -------
+        None.
+
+        """
+        data = dat[0]
+        self.sensor = data.metadata['Raster']['Sensor']
+        self.crs = data.crs
+        self.filename = data.filename
+
+        self.bands = []
+        self.tnames = []
+        self.banddata = []
+        for i in dat:
+            self.bands.append(i.dataid)
+            self.banddata.append(i)
+            if i.dataid[0] == 'B':
+                self.tnames.append(i.dataid)
+
+        if not self.tnames:
+            self.tnames = self.bands.copy()
+
+        if 'ASTER' in self.sensor:
+            self.sensor = 'ASTER'
+            # if len(self.bands) == 3:
+            #     self.sensor += 'v1'
+            # else:
+            #     self.sensor += 'v2'
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/equation_editor.py` & `pygmi-3.2.7.16/pygmi/raster/equation_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         self.combobox.addItem('all data')
 
         if 'Cluster' in self.indata:
             intype = 'Cluster'
         elif 'Raster' in self.indata:
             intype = 'Raster'
         else:
-            self.showprocesslog('No raster data.')
+            self.showlog('No raster data.')
             return False
 
         indata = dataprep.lstack(self.indata[intype])
 
         for j, i in enumerate(indata):
             self.combobox.addItem(i.dataid)
             self.bands[i.dataid] = 'i'+str(j)
@@ -495,15 +495,15 @@
         projdata['equation'] = self.equation
 
         return projdata
 
 
 def hmode(data):
     """
-    Mode - this uses a histogram to generate a fast mode estimate.
+    Use a histogram to generate a fast mode estimate.
 
     Parameters
     ----------
     data : list
         list of values to generate the mode from.
 
     Returns
@@ -539,15 +539,14 @@
     app = QtWidgets.QApplication(sys.argv)
 
     EE = EquationEditor()
     EE.indata['Raster'] = dat
 
     EE.settings()
 
-
     out = EE.outdata['Raster']
 
     plt.figure(dpi=150)
     plt.imshow(out[0].data)
     plt.show()
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/gcs.csv` & `pygmi-3.2.7.16/pygmi/raster/gcs.csv`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/raster/ginterp.py` & `pygmi-3.2.7.16/pygmi/raster/ginterp.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,16 +455,16 @@
         binave = np.arange(0, 1, 1/(bins.size-2))
 
         if hno == 0:
             bincol = self.newcmp(binave)
         else:
             bincol = colormaps['gray'](binave)
 
-        for j, _ in enumerate(patches):
-            patches[j].set_color(bincol[j])
+        for j, patchesj in enumerate(patches):
+            patchesj.set_color(bincol[j])
 
         # This section draws the black line.
         if zval is None or np.ma.is_masked(zval) is True:
             self.update_hist_text(self.htxt[hno], None)
             return 0
 
         binnum = (bins < zval).sum()-1
@@ -783,15 +783,15 @@
     sun: matplotlib plot instance
         plot of a circle 'o' showing where the sun is
     axes: matplotlib axes instance
         axes on which the sun is drawn
     """
 
     def __init__(self, parent=None):
-        fig = Figure()
+        fig = Figure(layout='constrained')
         super().__init__(fig)
 
         self.sun = None
         self.axes = fig.add_subplot(111, polar=True)
 
         self.setParent(parent)
         self.setMaximumSize(200, 200)
@@ -810,15 +810,15 @@
         self.axes.tick_params(labelleft=False, labelright=False)
         self.axes.set_autoscaley_on(False)
         self.axes.set_rmax(1.0)
         self.axes.set_rmin(0.0)
         self.axes.set_xticklabels([])
 
         self.sun, = self.axes.plot(np.pi/4., cos(np.pi/4.), 'o')
-        self.figure.tight_layout()
+        # self.figure.tight_layout()
         self.figure.canvas.draw()
 
 
 class PlotInterp(BasicModule):
     """
     The primary class for the raster data interpretation module.
 
@@ -1322,15 +1322,15 @@
         # Get rid of RGB bands.
         indata = []
         for i in self.indata['Raster']:
             if i.isrgb is True:
                 continue
             indata.append(i)
 
-        indata = dataprep.lstack(indata, pprint=self.showprocesslog,
+        indata = dataprep.lstack(indata, showlog=self.showlog,
                                  piter=self.piter)
 
         # Add membership data.
         if 'Cluster' in self.indata:
             newdat = copy.copy(indata)
             for i in self.indata['Cluster']:
                 if 'memdat' not in i.metadata['Cluster']:
@@ -1487,14 +1487,16 @@
 
             if not okay:
                 return False
 
         htype = str(self.cbox_htype.currentText())
         clippercl = self.mmc.clippercl
         clippercu = self.mmc.clippercu
+        cmin = None
+        cmax = None
 
         if dtype == 'Single Colour Map':
 
             for i in self.mmc.data:
                 if i.dataid == self.mmc.hband[0]:
                     pseudo = i.data
 
@@ -1634,55 +1636,56 @@
 
         newimg[0].dataid = rtext
         newimg[1].dataid = gtext
         newimg[2].dataid = btext
         newimg[3].dataid = 'Alpha'
 
         iodefs.export_raster(str(filename), newimg, 'GTiff', piter=self.piter,
-                             bandsort=False)
+                             bandsort=False, updatestats=False,
+                             showlog=self.showlog)
 
         # Section for colorbars
         if 'Ternary' not in dtype:
             txt = str(self.cbox_cbar.currentText())
             cmap = colormaps[txt]
             norm = mcolors.Normalize(vmin=cmin, vmax=cmax)
 
             # Horizontal Bar
-            fig = Figure()
+            fig = Figure(layout='constrained')
             canvas = FigureCanvasQTAgg(fig)
             fig.set_figwidth(blen)
             fig.set_figheight(bwid+0.75)
-            fig.set_tight_layout(True)
+            # fig.set_tight_layout(True)
             ax = fig.gca()
 
             cb = mcolorbar.ColorbarBase(ax, cmap=cmap, norm=norm,
                                         orientation='horizontal')
             cb.set_label(text)
 
             fname = filename[:-4]+'_hcbar.png'
             canvas.print_figure(fname, dpi=300)
 
             # Vertical Bar
-            fig = Figure()
+            fig = Figure(layout='constrained')
             canvas = FigureCanvasQTAgg(fig)
             fig.set_figwidth(bwid+1)
             fig.set_figheight(blen)
-            fig.set_tight_layout(True)
+            # fig.set_tight_layout(True)
             ax = fig.gca()
 
             cb = mcolorbar.ColorbarBase(ax, cmap=cmap, norm=norm,
                                         orientation='vertical')
             cb.set_label(text)
 
             fname = filename[:-4]+'_vcbar.png'
             canvas.print_figure(fname, dpi=300)
         else:
-            fig = Figure(figsize=[blen, blen])
+            fig = Figure(figsize=[blen, blen], layout='constrained')
             canvas = FigureCanvasQTAgg(fig)
-            fig.set_tight_layout(True)
+            # fig.set_tight_layout(True)
 
             tmp = np.array([[list(range(255))]*255])
             tmp.shape = (255, 255)
             tmp = np.transpose(tmp)
 
             red = ndimage.rotate(tmp, 0)
             green = ndimage.rotate(tmp, 120)
@@ -1757,19 +1760,19 @@
             True if successful, False otherwise.
 
         """
         if nodialog:
             return True
 
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         if self.indata['Raster'][0].isrgb:
-            self.showprocesslog('RGB images cannot be used in this module.')
+            self.showlog('RGB images cannot be used in this module.')
             return False
 
         self.show()
         self.mmc.init_graph()
         self.msc.init_graph()
 
         tmp = self.exec_()
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/graphs.py` & `pygmi-3.2.7.16/pygmi/raster/graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     ----------
     axes : matplotlib subplot
     parent : parent
         reference to the parent routine
     """
 
     def __init__(self, parent=None):
-        fig = Figure()
+        fig = Figure(layout='constrained')
         self.axes = fig.add_subplot(111)
         super().__init__(fig)
 
     def update_ccoef(self, data1, dmat):
         """
         Update the correlation coefficient plot.
 
@@ -106,15 +106,14 @@
 
         self.axes.set_yticklabels(dat_mat, rotation='horizontal')
         self.axes.set_xlim(0, len(data1))
         self.axes.set_ylim(0, len(data1))
 
         cbar = self.figure.colorbar(rdata, format=frm)
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_raster(self, data1, cmap):
         """
         Update the raster plot.
 
         Parameters
@@ -151,15 +150,14 @@
         else:
             self.axes.set_xlabel('Eastings')
             self.axes.set_ylabel('Northings')
 
         self.axes.xaxis.set_major_formatter(frm)
         self.axes.yaxis.set_major_formatter(frm)
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_hexbin(self, data1, data2):
         """
         Update the hexbin plot.
 
         Parameters
@@ -198,15 +196,14 @@
 
         self.axes.xaxis.set_major_formatter(frm)
         self.axes.yaxis.set_major_formatter(frm)
 
         self.axes.set_xlabel(data1.units)
         self.axes.set_ylabel(data2.units)
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_surface(self, data, cmap):
         """
         Update the surface plot.
 
         Parameters
@@ -257,15 +254,14 @@
         self.axes.zaxis.set_major_formatter(frm)
 
         self.axes.set_title('')
         self.axes.set_xlabel('X')
         self.axes.set_ylabel('Y')
         self.axes.set_zlabel('Z')
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_hist(self, data1, ylog):
         """
         Update the histogram plot.
 
         Parameters
@@ -291,15 +287,14 @@
 
         self.axes.xaxis.set_major_formatter(frm)
         self.axes.yaxis.set_major_formatter(frm)
 
         if ylog is True:
             self.axes.set_yscale('log')
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
 
 class PlotCCoef(ContextModule):
     """Plot 2D Correlation Coefficients."""
 
     def __init__(self, parent=None):
@@ -398,14 +393,15 @@
 
         Returns
         -------
         None.
 
         """
         self.show()
+        data = []
         if 'Raster' in self.indata:
             data = self.indata['Raster']
         elif 'Cluster' in self.indata:
             data = self.indata['Cluster']
 
         for i in data:
             self.combobox1.addItem(i.dataid)
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/iodefs.py` & `pygmi-3.2.7.16/pygmi/raster/iodefs.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 """Import raster data."""
 
 import warnings
 import os
 import copy
+import datetime
+import xml.etree.ElementTree as ET
 from PyQt5 import QtWidgets, QtCore
 import numpy as np
 from natsort import natsorted
 import rasterio
-# from rasterio.plot import plotting_extent
 from rasterio.windows import Window
 from rasterio.crs import CRS
 
 from pygmi.raster.datatypes import Data
 from pygmi.raster.dataprep import lstack
 from pygmi.misc import ProgressBarText, ContextModule, BasicModule
 
@@ -191,18 +192,18 @@
             nval, ok = QtWidgets.QInputDialog.getDouble(self.parent,
                                                         'Null Value',
                                                         'Enter Null Value',
                                                         nval)
             if not ok:
                 nval = 0.0
             dat = get_raster(self.ifile, nval, piter=self.piter,
-                             showprocesslog=self.showprocesslog)
+                             showlog=self.showlog)
         else:
             dat = get_raster(self.ifile, piter=self.piter,
-                             showprocesslog=self.showprocesslog)
+                             showlog=self.showlog)
 
         if dat is None:
             if self.filt == 'Geosoft UNCOMPRESSED grid (*.grd)':
                 QtWidgets.QMessageBox.warning(self.parent, 'Error',
                                               'Could not import the grid. '
                                               'Please make sure it is a '
                                               'Geosoft FLOAT grid, and not a '
@@ -222,17 +223,17 @@
         if 'Cluster' in dat[0].dataid:
             dat = clusterprep(dat)
             output_type = 'Cluster'
 
         self.outdata[output_type] = dat
 
         if dat[0].crs is None:
-            self.showprocesslog('Warning: Your data has no projection. '
-                                'Please add a projection in the Display/Edit '
-                                'Metadata interface.')
+            self.showlog('Warning: Your data has no projection. '
+                         'Please add a projection in the Display/Edit '
+                         'Metadata interface.')
 
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
@@ -300,15 +301,15 @@
                 self.parent, 'Open File', '.', ext)
             if self.ifile == '':
                 return False
 
         os.chdir(os.path.dirname(self.ifile))
 
         dat = get_raster(self.ifile, piter=self.piter,
-                         showprocesslog=self.showprocesslog)
+                         showlog=self.showlog)
 
         if dat is None:
             QtWidgets.QMessageBox.warning(self.parent, 'Error',
                                           'Could not import the image.',
                                           QtWidgets.QMessageBox.Ok)
             return False
 
@@ -433,15 +434,21 @@
 
     if isESRI:
         nbands = 1
         ncols = int(adata[1])
         nrows = int(adata[3])
         xdim = float(adata[9])
         ydim = float(adata[9])
-        nval = float(adata[11])
+        nval = adata[11]
+
+        if nval == 'None':
+            nval = None
+        else:
+            nval = float(nval)
+
         ulxmap = float(adata[5])
         ulymap = float(adata[7])+ydim*nrows
         if 'center' in adata[4].lower():
             ulxmap = ulxmap - xdim/2
         if 'center' in adata[6].lower():
             ulymap = ulymap - ydim/2
         adata = adata[12:]
@@ -488,65 +495,69 @@
                                  'AUTHORITY["EPSG","9001"]],'
                                  'AXIS["Easting",EAST],'
                                  'AXIS["Northing",NORTH]]')
 
     return dat
 
 
-def get_raster(ifile, nval=None, piter=None, showprocesslog=print,
+def get_raster(ifile, nval=None, piter=None, showlog=print,
                iraster=None, driver=None, bounds=None, dataid=None,
                tnames=None, metaonly=False):
     """
     Get raster dataset.
 
     This function loads a raster dataset off the disk using the rasterio
     libraries. It returns the data in a PyGMI data object.
 
     Parameters
     ----------
     ifile : str
         filename to import
     nval : float, optional
-        No data/null value. The default is None.
+        Nodata/null value. The default is None.
     piter : iterable from misc.ProgressBar or misc.ProgressBarText
         progress bar iterable, default is None.
-    showprocesslog : function, optional
+    showlog : function, optional
         Routine to show text messages. The default is print.
     iraster : None or tuple
         Incremental raster import, to import a section of a file. The tuple is
         (xoff, yoff, xsize, ysize)
     driver : str
         GDAL raster driver name. The default is None.
 
     Returns
     -------
     dat : PyGMI raster Data
         dataset imported
     """
+    # Exclusions
+    if 'AG1' in ifile and 'h5' in ifile.lower():
+        return None
+
     if piter is None:
         piter = ProgressBarText().iter
 
     dat = []
     bname = os.path.basename(ifile).rpartition('.')[0]
     ext = ifile[-3:]
     custom_wkt = ''
     filename = ifile
 
-    # Envi Case
+    # ENVI Case
     if ext == 'hdr':
         ifile = ifile[:-4]
         if os.path.exists(ifile+'.dat'):
             ifile = ifile+'.dat'
         elif os.path.exists(ifile+'.raw'):
             ifile = ifile+'.raw'
         elif os.path.exists(ifile+'.img'):
             ifile = ifile+'.img'
         elif not os.path.exists(ifile):
             return None
-
+    # ER Mapper case
     if ext == 'ers':
         with open(ifile, encoding='utf-8') as f:
             metadata = f.read()
             if 'STMLO' in metadata:
                 clong = metadata.split('STMLO')[1][:2]
 
                 if 'CAPE' in metadata:
@@ -591,44 +602,62 @@
                                   'PARAMETER["false_easting",0],'
                                   'PARAMETER["false_northing",0],'
                                   'UNIT["metre",1,AUTHORITY["EPSG","9001"]],'
                                   'AXIS["Easting",EAST],'
                                   'AXIS["Northing",NORTH]]')
 
     dmeta = {}
-    with rasterio.open(ifile, driver=driver) as dataset:
-        if dataset is None:
-            return None
-
-        # allns = dataset.tag_namespaces()
-
-        gmeta = dataset.tags()
-        istruct = dataset.tags(ns='IMAGE_STRUCTURE')
-        driver = dataset.driver
+    rdate = None
+    try:
+        with rasterio.open(ifile, driver=driver) as dataset:
+            if dataset is None:
+                return None
+            # allns = dataset.tag_namespaces()
+
+            gmeta = dataset.tags()
+            istruct = dataset.tags(ns='IMAGE_STRUCTURE')
+            driver = dataset.driver
+            if 'TIFFTAG_DATETIME' in gmeta:
+                dtimestr = gmeta['TIFFTAG_DATETIME']
+                rdate = datetime.datetime.strptime(dtimestr,
+                                                   '%Y:%m:%d %H:%M:%S')
+
+            if driver == 'ENVI':
+                dmeta = dataset.tags(ns='ENVI')
+                if 'fwhm' in dmeta:
+                    dmeta['fwhm'] = [float(i) for i in
+                                     dmeta['fwhm'][1:-1].split(',')]
+
+            wavelengthmax = 0.
+            for i in piter(range(dataset.count)):
+                index = dataset.indexes[i]
+                dest = dataset.tags(index)
+                for j in ['Wavelength', 'WAVELENGTH']:
+                    if j in dest:
+                        dest['wavelength'] = dest[j]
+                        del dest[j]
+
+                if 'wavelength' in dest:
+                    wavelengthmax = max(wavelengthmax,
+                                        float(dest['wavelength']))
 
-        if driver == 'ENVI':
-            dmeta = dataset.tags(ns='ENVI')
+    except rasterio.errors.RasterioIOError:
+        return None
 
-    if custom_wkt == '' and dataset.crs is not None:
-        custom_wkt = dataset.crs.to_wkt()
-
-    cols = dataset.width
-    rows = dataset.height
-    bands = dataset.count
     if nval is None:
         nval = dataset.nodata
     dtype = rasterio.band(dataset, 1).dtype
 
     if bounds is not None:
         xdim, ydim = dataset.res
         xmin, ymin, xmax, ymax = dataset.bounds
         xmin1, ymin1, xmax1, ymax1 = bounds
 
         if xmin1 >= xmax or xmax1 <= xmin or ymin1 >= ymax or ymax1 <= ymin:
-            showprocesslog('Warning: No data in polygon.')
+            showlog('Warning: No data in polygon.')
             return None
 
         xmin2 = max(xmin, xmin1)
         ymin2 = max(ymin, ymin1)
         xmax2 = min(xmax, xmax1)
         ymax2 = min(ymax, ymax1)
 
@@ -650,30 +679,39 @@
         newbounds = (xmin+xoff*xdim,
                      ymax-yoff*ydim-ysize*ydim,
                      xmin+xoff*xdim+xsize*xdim,
                      ymax-yoff*ydim)
     else:
         newbounds = None
 
+    # Projection
+    if custom_wkt == '' and dataset.crs is not None:
+        custom_wkt = dataset.crs.to_wkt()
     if custom_wkt != '':
         crs = CRS.from_string(custom_wkt)
     else:
-        showprocesslog('Warning: Your data does not have a projection. '
-                       'Assigning local coordinate system.')
+        showlog('Warning: Your data does not have a projection. '
+                'Assigning local coordinate system.')
         crs = CRS.from_string('LOCAL_CS["Arbitrary",UNIT["metre",1,'
                               'AUTHORITY["EPSG","9001"]],'
                               'AXIS["Easting",EAST],'
                               'AXIS["Northing",NORTH]]')
 
+    # Perform BIL or BIP with internal routine, because its faster.
     isbil = False
     if ('INTERLEAVE' in istruct and driver in ['ENVI', 'ERS', 'EHdr'] and
             dataid is None and metaonly is False):
-        if istruct['INTERLEAVE'] == 'LINE':
+        interleave = istruct['INTERLEAVE']
+        if interleave in ['LINE', 'PIXEL']:
             isbil = True
-            datin = get_bil(ifile, bands, cols, rows, dtype, piter, iraster)
+            cols = dataset.width
+            rows = dataset.height
+            bands = dataset.count
+            datin = get_bil(ifile, bands, cols, rows, dtype, piter, iraster,
+                            interleave)
 
     with rasterio.open(ifile) as dataset:
         for i in piter(range(dataset.count)):
             index = dataset.indexes[i]
             bandid = dataset.descriptions[i]
 
             if bandid == '' or bandid is None:
@@ -681,83 +719,86 @@
 
             if dataid is not None and bandid != dataid:
                 continue
 
             if tnames is not None and bandid not in tnames:
                 continue
 
+            dat.append(Data())
+
+            # Determine units
             unit = dataset.units[i]
-            if unit is None:
+            if unit is None and 'wavelength_units' in dmeta:
+                unit = dmeta['wavelength_units']
+            elif unit is None and 0. < wavelengthmax < 100.:
+                unit = 'micrometers'
+            elif unit is None and wavelengthmax >= 100.:
+                unit = 'nanometers'
+            elif unit is None:
                 unit = ''
             if unit.lower() == 'micrometers':
-                dat[i].units = 'μm'
+                dat[-1].units = 'μm'
             elif unit.lower() == 'nanometers':
-                dat[i].units = 'nm'
+                dat[-1].units = 'nm'
             if nval is None:
                 nval = dataset.nodata
 
-            dat.append(Data())
+            # Get data
             if isbil is True and metaonly is False:
                 dat[-1].data = datin[i]
             elif iraster is None and metaonly is False:
                 dat[-1].data = dataset.read(index)
             elif metaonly is False:
                 xoff, yoff, xsize, ysize = iraster
                 dat[-1].data = dataset.read(index, window=Window(xoff, yoff,
                                                                  xsize, ysize))
-            # print(dataset.meta['dtype'])
-            if 'uint' in dataset.meta['dtype']:
-                if nval is None or np.isnan(nval):
-                    nval = 0
-                    # showprocesslog(f'Adjusting null value to {nval}')
-                nval = int(nval)
-
-            elif 'int' in dataset.meta['dtype']:
-                if nval is None or np.isnan(nval):
-                    nval = 999999
-                    # showprocesslog(f'Adjusting null value to {nval}')
-                nval = int(nval)
-            else:
-                if nval is None or np.isnan(nval):
-                    nval = 1e+20
+
+            # Set Null Value
+            if nval is not None and np.isnan(nval):
+                nval = None
+
+            if 'int' not in dataset.meta['dtype'] and nval is not None:
                 nval = float(nval)
                 if nval not in dat[-1].data and np.isclose(dat[-1].data.min(),
                                                            nval):
                     nval = dat[-1].data.min()
+                    showlog(f'{bandid}: Adjusting nodata value to {nval}')
+
                 if nval not in dat[-1].data and np.isclose(dat[-1].data.max(),
                                                            nval):
                     nval = dat[-1].data.max()
-                # showprocesslog(f'Adjusting null value to {nval}')
+                    showlog(f'{bandid}: Adjusting nodata value to {nval}')
 
             if ext == 'ers' and nval == -1.0e+32 and metaonly is False:
                 dat[-1].data[dat[-1].data <= nval] = -1.0e+32
 
-    # Note that because the data is stored in a masked array, the array ends up
-    # being double the size that it was on the disk.
-
             if metaonly is False:
                 dat[-1].data = np.ma.masked_invalid(dat[-1].data)
                 dat[-1].data = dat[-1].data.filled(nval)
                 dat[-1].data = np.ma.masked_equal(dat[-1].data, nval)
                 dat[-1].data.set_fill_value(nval)
-
-            # dat[-1].data.mask = (np.ma.getmaskarray(dat[-1].data) |
-            #                      (dat[-1].data == nval))
+                rows = None
+                cols = None
+            else:
+                rows = dataset.height
+                cols = dataset.width
 
             if newbounds is not None:
                 xmin, _, _, ymax = newbounds
                 xdim, ydim = dataset.res
-                dat[-1].set_transform(xdim, xmin, ydim, ymax, iraster=iraster)
+                dat[-1].set_transform(xdim, xmin, ydim, ymax,
+                                      rows=rows, cols=cols)
             else:
-                dat[-1].set_transform(transform=dataset.transform)
+                dat[-1].set_transform(transform=dataset.transform,
+                                      rows=rows, cols=cols)
 
             dat[-1].dataid = bandid
             dat[-1].nodata = nval
             dat[-1].filename = filename
-            dat[-1].units = unit
+            dat[-1].datetime = rdate
 
             if driver == 'netCDF' and dataset.crs is None:
                 if 'x#actual_range' in gmeta and 'y#actual_range' in gmeta:
                     xrng = gmeta['x#actual_range']
                     xrng = xrng.strip('}{').split(',')
                     xrng = [float(i) for i in xrng]
                     xmin = min(xrng)
@@ -767,39 +808,55 @@
                     yrng = yrng.strip('}{').split(',')
                     yrng = [float(i) for i in yrng]
                     ymin = min(yrng)
                     ydim = (yrng[1]-yrng[0])/rows
                     dat[-1].set_transform(xdim, xmin, ydim, ymin)
 
             dat[-1].crs = crs
-            # dat[i].xdim, dat[i].ydim = dataset.res
             dat[-1].meta = dataset.meta
 
             dest = dataset.tags(index)
             for j in ['Wavelength', 'WAVELENGTH']:
                 if j in dest:
                     dest[j.lower()] = dest[j]
                     del dest[j]
 
-            if 'fwhm' in dmeta:
-                fwhm = [float(i) for i in dmeta['fwhm'][1:-1].split(',')]
-                dest['fwhm'] = fwhm[index-1]
+            if 'wavelength' in dest:
+                dest['wavelength'] = float(dest['wavelength'])
 
-            if '.raw' in ifile:
-                dmeta['reflectance_scale_factor'] = 10000.
+            if 'fwhm' in dmeta:
+                dest['fwhm'] = dmeta['fwhm'][index-1]
+                dest['WavelengthMin'] = dest['wavelength']-dest['fwhm']/2
+                dest['WavelengthMax'] = dest['wavelength']+dest['fwhm']/2
+
+            if 'wavelength' in dest and dat[-1].units == 'μm':
+                dest['wavelength'] = dest['wavelength'] * 1000.
+                dat[-1].units = 'nm'
+                dest['wavelength_units'] = 'Nanometers'
+                if 'fwhm' in dest:
+                    dest['fwhm'] = dest['fwhm'] * 1000.
+                if 'WavelengthMin' in dest:
+                    dest['WavelengthMin'] = dest['WavelengthMin'] * 1000
+                    dest['WavelengthMax'] = dest['WavelengthMax'] * 1000
 
             if 'reflectance scale factor' in dmeta:
                 dmeta['reflectance_scale_factor'] = dmeta['reflectance scale factor']
 
-            dat[-1].metadata['Raster'] = {**dmeta, **dest}
+            if '.raw' in ifile and 'reflectance_scale_factor' not in dmeta:
+                dmeta['reflectance_scale_factor'] = 10000.
+
+            dat[-1].metadata['Raster'].update(dmeta)
+            # dest overwrites same keys in dmeta.
+            dat[-1].metadata['Raster'].update(dest)
 
     return dat
 
 
-def get_bil(ifile, bands, cols, rows, dtype, piter, iraster=None):
+def get_bil(ifile, bands, cols, rows, dtype, piter, iraster=None,
+            interleave='LINE'):
     """
     Get BIL format file.
 
     This routine is called from get_raster
 
     Parameters
     ----------
@@ -847,77 +904,26 @@
     extra = int(count-offset/dsize)
     if extra > 0:
         tmp = np.fromfile(ifile, dtype=dtype, sep='', count=extra,
                           offset=offset)
         datin.append(tmp)
 
     datin = np.concatenate(datin)
-    datin.shape = (ysize, bands, cols)
-    datin = np.swapaxes(datin, 0, 1)
-
-    if iraster is not None:
-        datin = datin[:, :, xoff:xoff+xsize]
-
-    return datin
-
-
-def get_bil_old(ifile, bands, cols, rows, dtype, piter, iraster=None):
-    """
-    Get BIL format file.
-
-    This routine is called from get_raster
-
-    Parameters
-    ----------
-    ifile : str
-        filename to import
-    bands : int
-        Number of bands.
-    cols : int
-        Number of columns.
-    rows : int
-        Number of rows.
-    dtype : data type
-        Data type.
-    piter : iterable from misc.ProgressBar or misc.ProgressBarText
-        progress bar iterable
 
-    Returns
-    -------
-    datin : PyGMI raster Data
-        dataset imported
-
-    """
-    dtype = np.dtype(dtype)
-
-    count = bands*cols*rows
-
-    offset = 0
-    icount = count//10
-    datin = []
-    dsize = dtype.itemsize
-    for _ in piter(range(0, 10)):
-        tmp = np.fromfile(ifile, dtype=dtype, sep='', count=icount,
-                          offset=offset)
-        offset += icount*dsize
-        datin.append(tmp)
-
-    extra = int(count-offset/dsize)
-    if extra > 0:
-        tmp = np.fromfile(ifile, dtype=dtype, sep='', count=extra,
-                          offset=offset)
-        datin.append(tmp)
-
-    datin = np.concatenate(datin)
-    datin.shape = (rows, bands, cols)
-    datin = np.swapaxes(datin, 0, 1)
+    if interleave == 'LINE':
+        datin.shape = (ysize, bands, cols)
+        datin = np.swapaxes(datin, 0, 1)
+    else:
+        datin.shape = (ysize, cols, bands)
+        # datin = np.swapaxes(datin, 0, 2)
+        # datin = np.swapaxes(datin, 1, 2)
+        datin = np.moveaxis(datin, [0, 1, 2], [1, 2, 0])
 
     if iraster is not None:
-        xoff, yoff, xsize, ysize = iraster
-        datin = datin[:, yoff:yoff+ysize, xoff:xoff+xsize]
+        datin = datin[:, :, xoff:xoff+xsize]
 
     return datin
 
 
 def get_geopak(hfile):
     """
     Geopak Import.
@@ -1097,21 +1103,17 @@
         #     nb = np.fromfile(f, dtype=np.int32, count=1)[0]
         #     vpb = np.fromfile(f, dtype=np.int32, count=1)[0]
 
         #     ob = np.fromfile(f, dtype=np.int64, count=nb)
         #     cbs = np.fromfile(f, dtype=np.int32, count=nb)
 
         #     for i in range(nb):
-        #         # breakpoint()
         #         blk = f.read(cbs[i])
-        #         # breakpoint()
         #         blk2 = lzrw1.decompress_chunk(blk)
 
-        #         breakpoint()
-
         else:
             return None
 
         data = np.ma.masked_equal(data, nval)
 
         data = data/zmult + zbase
         data.shape = (nrows, ncols)
@@ -1180,20 +1182,21 @@
                                   + ': '+tmp.dataid)
                     newdat.append(tmp)
             data = newdat
 
         elif 'Raster' in self.indata:
             data = self.indata['Raster']
         else:
-            self.showprocesslog('No raster data')
+            self.showlog('No raster data')
             self.parent.process_is_active(False)
             return False
 
-        ext = ('GeoTiff (*.tif);;'
+        ext = ('GeoTiff compressed using DEFLATE (*.tif);;'
                'GeoTiff compressed using ZSTD (*.tif);;'
+               'GeoTiff (*.tif);;'
                'ENVI (*.hdr);;'
                'ERMapper (*.ers);;'
                'Geosoft (*.gxf);;'
                'ERDAS Imagine (*.img);;'
                'SAGA binary grid (*.sdat);;'
                'Surfer grid (*.grd);;'
                'ArcInfo ASCII (*.asc);;'
@@ -1203,47 +1206,57 @@
         self.ofile, filt = QtWidgets.QFileDialog.getSaveFileName(
             self.parent, 'Save File', '.', ext)
         if self.ofile == '':
             self.parent.process_is_active(False)
             return False
         os.chdir(os.path.dirname(self.ofile))
 
-        self.showprocesslog('Export Data Busy...')
+        self.showlog('Export Data Busy...')
 
         # Pop up save dialog box
         if filt == 'ArcInfo ASCII (*.asc)':
             self.export_ascii(data)
         if filt == 'ASCII XYZ (*.xyz)':
             self.export_ascii_xyz(data)
         if filt == 'Geosoft (*.gxf)':
             self.export_gxf(data)
         if filt == 'Surfer grid (*.grd)':
             self.export_surfer(data)
         if filt == 'ERDAS Imagine (*.img)':
-            export_raster(self.ofile, data, 'HFA', piter=self.piter)
+            export_raster(self.ofile, data, 'HFA', piter=self.piter,
+                          showlog=self.showlog)
         if filt == 'ERMapper (*.ers)':
-            export_raster(self.ofile, data, 'ERS', piter=self.piter)
+            export_raster(self.ofile, data, 'ERS', piter=self.piter,
+                          showlog=self.showlog)
         if filt == 'SAGA binary grid (*.sdat)':
             if len(data) > 1:
                 for i, dat in enumerate(data):
                     file_out = self.get_filename(dat, 'sdat')
-                    export_raster(file_out, [dat], 'SAGA', piter=self.piter)
+                    export_raster(file_out, [dat], 'SAGA', piter=self.piter,
+                                  showlog=self.showlog)
+            else:
+                export_raster(self.ofile, data, 'SAGA', piter=self.piter,
+                              showlog=self.showlog)
+        if 'GeoTiff' in filt:
+            if 'ZSTD' in filt:
+                compression = 'ZSTD'
+            elif 'DEFLATE' in filt:
+                compression = 'DEFLATE'
             else:
-                export_raster(self.ofile, data, 'SAGA', piter=self.piter)
-        if filt == 'GeoTiff (*.tif)':
-            export_raster(self.ofile, data, 'GTiff', piter=self.piter)
-        if filt == 'GeoTiff compressed using ZSTD (*.tif)':
+                compression = 'NONE'
             export_raster(self.ofile, data, 'GTiff', piter=self.piter,
-                          compression='ZSTD')
+                          compression=compression, showlog=self.showlog)
         if filt == 'ENVI (*.hdr)':
-            export_raster(self.ofile, data, 'ENVI', piter=self.piter)
+            export_raster(self.ofile, data, 'ENVI', piter=self.piter,
+                          showlog=self.showlog)
         if filt == 'ArcGIS BIL (*.bil)':
-            export_raster(self.ofile, data, 'EHdr', piter=self.piter)
+            export_raster(self.ofile, data, 'EHdr', piter=self.piter,
+                          showlog=self.showlog)
 
-        self.showprocesslog('Export Data Finished!')
+        self.showlog('Export Data Finished!')
         self.parent.process_is_active(False)
         return True
 
     def export_gxf(self, data):
         """
         Export GXF data.
 
@@ -1254,17 +1267,17 @@
 
         Returns
         -------
         None.
 
         """
         if len(data) > 1:
-            self.showprocesslog('Band names will be appended to the output '
-                                'filenames since you have a multiple band '
-                                'image')
+            self.showlog('Band names will be appended to the output '
+                         'filenames since you have a multiple band '
+                         'image')
 
         file_out = self.ofile.rpartition('.')[0]+'.gxf'
         for k in data:
             if len(data) > 1:
                 file_out = self.get_filename(k, 'gxf')
 
             with open(file_out, 'w', encoding='utf-8') as fno:
@@ -1304,30 +1317,30 @@
                             fno.write('\n')
 
                         fno.write(str(tmp[i, j]) + '  ')
                         kkk += 1
 
     def export_surfer(self, data):
         """
-        Export a surfer binary grid.
+        Routine to export a surfer binary grid.
 
         Parameters
         ----------
         data : PyGMI raster Data
             dataset to export
 
         Returns
         -------
         None.
 
         """
         if len(data) > 1:
-            self.showprocesslog('Band names will be appended to the output '
-                                'filenames since you have a multiple band '
-                                'image')
+            self.showlog('Band names will be appended to the output '
+                         'filenames since you have a multiple band '
+                         'image')
 
         file_out = self.ofile.rpartition('.')[0] + '.grd'
         for k0 in data:
             k = copy.deepcopy(k0)
             if len(data) > 1:
                 file_out = self.get_filename(k, 'grd')
 
@@ -1347,17 +1360,17 @@
 
         Returns
         -------
         None.
 
         """
         if len(data) > 1:
-            self.showprocesslog('Band names will be appended to the output '
-                                'filenames since you have a multiple band '
-                                'image')
+            self.showlog('Band names will be appended to the output '
+                         'filenames since you have a multiple band '
+                         'image')
 
         file_out = self.ofile.rpartition('.')[0]+'.asc'
         for k in data:
             if len(data) > 1:
                 file_out = self.get_filename(k, 'asc')
             with open(file_out, 'w', encoding='utf-8') as fno:
                 extent = k.extent
@@ -1391,17 +1404,17 @@
 
         Returns
         -------
         None.
 
         """
         if len(data) > 1:
-            self.showprocesslog('Band names will be appended to the output '
-                                'filenames since you have a multiple band '
-                                'image')
+            self.showlog('Band names will be appended to the output '
+                         'filenames since you have a multiple band '
+                         'image')
 
         file_out = self.ofile.rpartition('.')[0]+'.xyz'
         for k in data:
             if len(data) > 1:
                 file_out = self.get_filename(k, 'xyz')
             with open(file_out, 'w', encoding='utf-8') as fno:
                 tmp = k.data.filled(k.nodata)
@@ -1439,23 +1452,24 @@
 
         file_out = self.ofile.rpartition('.')[0]+'_'+file_band+'.'+ext
 
         return file_out
 
 
 def export_raster(ofile, dat, drv='GTiff', envimeta='', piter=None,
-                  compression='NONE', bandsort=True, pprint=print):
+                  compression='NONE', bandsort=True, showlog=print,
+                  updatestats=True):
     """
     Export to rasterio format.
 
     Parameters
     ----------
     ofile : str
         Output file name.
-    dat : PyGMI raster Data
+    dat : list or dictionary of PyGMI raster Data
         dataset to export
     drv : str
         name of the rasterio driver to use
     envimeta : str, optional
         ENVI metadata. The default is ''.
     piter : ProgressBar.iter/ProgressBarText.iter, optional
         Progressbar iterable from misc. The default is None.
@@ -1487,44 +1501,48 @@
         data = [i for _, i in natsorted(zip(dataid, data))]
 
     dtype = data[0].data.dtype
     nodata = data[0].nodata
     trans = data[0].transform
     crs = data[0].crs
 
-    try:
-        nodata = dtype.type(nodata)
-    except OverflowError:
-        print('Invalid nodata for dtype, resetting to 0')
-        nodata = 0
+    if nodata is not None:
+        try:
+            nodata = dtype.type(nodata)
+        except OverflowError:
+            print(f'Invalid nodata for {dtype}, resetting to None')
+            nodata = None
 
     if trans is None:
         trans = rasterio.transform.from_origin(data[0].extent[0],
                                                data[0].extent[3],
                                                data[0].xdim, data[0].ydim)
 
-    tmp = ofile.rpartition('.')
+    tmp = os.path.splitext(ofile)
 
+    xfile = None
     if drv == 'GTiff':
         tmpfile = tmp[0] + '.tif'
     elif drv == 'EHdr':
         dtype = np.float32
         tmpfile = tmp[0] + '.bil'
     elif drv == 'GSBG':
         tmpfile = tmp[0]+'.grd'
         dtype = np.float32
     elif drv == 'SAGA':
         tmpfile = tmp[0]+'.sdat'
         nodata = -99999.0
     elif drv == 'HFA':
         tmpfile = tmp[0]+'.img'
+        updatestats = False
     elif drv == 'ENVI':
         tmpfile = tmp[0]+'.dat'
-    elif drv == 'ERS':  # ER Mapper
+    elif drv == 'ERS':
         tmpfile = tmp[0]
+        xfile = tmpfile+'.ers.aux.xml'
     else:
         tmpfile = ofile
 
     drows, dcols = data[0].data.shape
 
     kwargs = {}
     if drv == 'GTiff':
@@ -1534,64 +1552,120 @@
                   'INTERLEAVE': 'BAND',
                   'TFW': 'YES',
                   'PROFILE': 'GeoTIFF'}
         if compression == 'ZSTD':
             kwargs['ZSTD_LEVEL'] = '1'
         if dtype in (np.float32, np.float64):
             kwargs['PREDICTOR'] = '3'
+        else:
+            kwargs['PREDICTOR'] = '2'
 
     with rasterio.open(tmpfile, 'w', driver=drv,
                        width=int(dcols), height=int(drows), count=len(data),
                        dtype=dtype, transform=trans, crs=crs,
                        nodata=nodata, **kwargs) as out:
         numbands = len(data)
         wavelength = []
         fwhm = []
 
         for i in piter(range(numbands)):
             datai = data[i]
 
             out.set_band_description(i+1, datai.dataid)
 
-            dtmp = np.ma.array(datai.data)
-            dtmp.set_fill_value(nodata)
-            dtmp = dtmp.filled()
+            if nodata is None:
+                dtmp = datai.data
+            else:
+                dtmp = np.ma.array(datai.data)
+                dtmp.set_fill_value(nodata)
+                dtmp = dtmp.filled()
 
             out.write(dtmp, i+1)
 
             del dtmp
 
-            out.update_tags(i+1, STATISTICS_EXCLUDEDVALUES='')
-            out.update_tags(i+1, STATISTICS_MAXIMUM=datai.data.max())
-            out.update_tags(i+1, STATISTICS_MEAN=datai.data.mean())
-            out.update_tags(i+1, STATISTICS_MINIMUM=datai.data.min())
-            out.update_tags(i+1, STATISTICS_SKIPFACTORX=1)
-            out.update_tags(i+1, STATISTICS_SKIPFACTORY=1)
-            try:
-                out.update_tags(i+1, STATISTICS_STDDEV=datai.data.std())
-            except MemoryError:
-                pprint('Unable to calculate std deviation. Not enough memory')
-
             if 'Raster' in datai.metadata:
-                if 'wavelength' in datai.metadata['Raster']:
-                    out.update_tags(i+1, wavelength=str(datai.metadata['Raster']['wavelength']))
-                    wavelength.append(datai.metadata['Raster']['wavelength'])
-
-                if 'fwhm' in datai.metadata['Raster']:
-                    fwhm.append(datai.metadata['Raster']['fwhm'])
-
-                if 'reflectance_scale_factor' in datai.metadata['Raster']:
-                    out.update_tags(i+1, reflectance_scale_factor=str(datai.metadata['Raster']['reflectance_scale_factor']))
-
-            if 'WavelengthMin' in datai.metadata:
-                out.update_tags(i+1, WavelengthMin=str(datai.metadata['WavelengthMin']))
-                out.update_tags(i+1, WavelengthMax=str(datai.metadata['WavelengthMax']))
-            elif 'WavelengthMin' in datai.metadata['Raster']:
-                out.update_tags(i+1, WavelengthMin=str(datai.metadata['Raster']['WavelengthMin']))
-                out.update_tags(i+1, WavelengthMax=str(datai.metadata['Raster']['WavelengthMax']))
+                rmeta = datai.metadata['Raster']
+                if 'wavelength' in rmeta:
+                    out.update_tags(i+1, Wavelength=str(rmeta['wavelength']))
+                    # out.update_tags(i+1, wavelength=str(rmeta['wavelength']))
+                    wavelength.append(rmeta['wavelength'])
+
+                if 'fwhm' in rmeta:
+                    fwhm.append(rmeta['fwhm'])
+
+                if 'reflectance_scale_factor' in rmeta:
+                    out.update_tags(i+1,
+                                    reflectance_scale_factor=str(rmeta['reflectance_scale_factor']))
+
+                if 'WavelengthMin' in rmeta:
+                    out.update_tags(i+1,
+                                    WavelengthMin=str(rmeta['WavelengthMin']))
+                    out.update_tags(i+1,
+                                    WavelengthMax=str(rmeta['WavelengthMax']))
+
+    if updatestats is True:
+        dcov = None  # Disabled because it uses too much memory.
+        # dcov = calccov(data, showlog)
+
+        if xfile is None:
+            xfile = tmpfile+'.aux.xml'
+        tree = ET.parse(xfile)
+        root = tree.getroot()
+
+        showlog('Calculating statistics...')
+        # for child in piter(root):
+        for child in piter(root.findall('PAMRasterBand')):
+            band = int(child.attrib['band'])-1
+            datai = data[band]
+            donly = datai.data.compressed()
+
+            # Histogram section
+            dhist = np.histogram(donly, 256)
+            dmin = str(dhist[1][0])
+            dmax = str(dhist[1][-1])
+            dhist = str(dhist[0].tolist()).replace(', ', '|')[1:-1]
+
+            hist = ET.SubElement(child, 'Histograms')
+            histitem = ET.SubElement(hist, 'HistItem')
+            ET.SubElement(histitem, 'HistMin').text = dmin
+            ET.SubElement(histitem, 'HistMax').text = dmax
+            ET.SubElement(histitem, 'BucketCount').text = '256'
+            ET.SubElement(histitem, 'IncludeOutOfRange').text = '1'
+            ET.SubElement(histitem, 'Approximate').text = '0'
+            ET.SubElement(histitem, 'HistCounts').text = dhist
+
+            # Metadata, statistics
+            dmin = str(donly.min())
+            dmax = str(donly.max())
+            dmean = str(donly.mean())
+            dmedian = str(np.median(donly))
+            dstd = str(donly.std())
+
+            meta = child.find('Metadata')
+            if meta is None:
+                meta = ET.SubElement(child, 'Metadata')
+            if dcov is not None:
+                dcovi = str(dcov[:, band].tolist()).replace(' ', '')[1:-1]
+                ET.SubElement(meta, 'MDI',
+                              key='STATISTICS_COVARIANCES').text = dcovi
+            ET.SubElement(meta, 'MDI', key='STATISTICS_EXCLUDEDVALUES')
+            ET.SubElement(meta, 'MDI', key='STATISTICS_MAXIMUM').text = dmax
+            ET.SubElement(meta, 'MDI', key='STATISTICS_MEAN').text = dmean
+            ET.SubElement(meta, 'MDI', key='STATISTICS_MEDIAN').text = dmedian
+            ET.SubElement(meta, 'MDI', key='STATISTICS_MINIMUM').text = dmin
+            ET.SubElement(meta, 'MDI', key='STATISTICS_SKIPFACTORX').text = '1'
+            ET.SubElement(meta, 'MDI', key='STATISTICS_SKIPFACTORY').text = '2'
+            ET.SubElement(meta, 'MDI', key='STATISTICS_STDDEV').text = dstd
+
+            # meta[:] = sorted(meta, key=lambda x: x.tag)
+            child[:] = sorted(child, key=lambda x: x.tag)
+
+        ET.indent(tree)
+        tree.write(xfile, encoding='utf-8')
 
     if drv == 'ENVI':
         wout = ''
         if (wavelength and envimeta is not None and
                 'wavelength' not in envimeta):
             wout = str(wavelength)
             wout = wout.replace('[', '{')
@@ -1611,52 +1685,82 @@
                      + '\n')
 
         with open(tmpfile[:-4]+'.hdr', 'a', encoding='utf-8') as myfile:
             myfile.write(wout)
             myfile.write(envimeta)
 
 
+def calccov(data, showlog=print):
+    """
+    Calculate covariance from PyGMI Data.
+
+    This routine assumes all bands are co-located, with the same size.
+    Otherwise, run lstack first.
+
+    Parameters
+    ----------
+    data : list
+        List of PyGMI data.
+
+    Returns
+    -------
+    dcov : numpy array
+        Covariances.
+
+    """
+    showlog('Calculating covariances...')
+
+    mask = np.ma.getmaskarray(data[0].data)
+    for band in data:
+        mask2 = np.ma.getmaskarray(band.data)
+        mask = np.logical_or(mask, mask2)
+
+    data2 = []
+    for band in data:
+        data2.append(band.data[~mask])
+
+    try:
+        dcov = np.cov(data2)
+    except MemoryError:
+        showlog('Cannot calculate covariance: ran out of memory')
+        return None
+
+    del data2
+
+    if dcov.size == 1:
+        dcov.shape = (1, 1)
+
+    return dcov
+
+
 def _filespeedtest():
     """Test."""
-    import matplotlib.pyplot as plt
     from pygmi.misc import getinfo
     print('Starting')
 
-    ifile = r"D:\Workdata\PyGMI Test Data\Raster\mosaic\Box1_rad_3band.ers"
+    ifile = r"D:\Hyper\cut_048-055_ref_rect.hdr"
+    ifile = r"D:\Hyper\103A_0825-0943_ref_rect.hdr"
 
-    # ifile = r"D:\Workdata\PyGMI Test Data\Raster\Geosoft\FCR2613 CGS Block 2&3 TMI.GRD"
+    # ifile = ifile[:-4]+'_zstd.tif'
+    dataset = get_raster(ifile, metaonly=False)
 
-    # iraster = None
+    for i in dataset:
+        i.dataid = i.dataid.replace('band*', 'band ')
+        i.dataid = i.dataid.replace('band   ', 'band ')
+        i.dataid = i.dataid.replace('band  ', 'band ')
 
     getinfo('Start')
 
-    dataset = get_raster(ifile)
-    for dat in dataset:
-        dat.data = dat.data.astype(float)
-        dat.nodata = 0
-    export_raster(r'c:\workdata\temp.tif', dataset)
-    dataset = get_raster(r'c:\workdata\temp.tif')
-
-
-    # plt.figure(dpi=150)
-    # plt.imshow(dataset[0].data, extent=dataset[0].extent)
-    # plt.colorbar()
-    # plt.show()
-
-    # for i in dataset:
-    #     i.data = i.data*10000
-    #     i.data = i.data.astype(np.int16)
-
-    # export_raster(ofile, dataset, 'GTiff', compression='PACKBITS')  # 182s
-    # export_raster(ofile, dataset, 'GTiff', compression='LZW')  # 191, 140 with pred=3
-    # export_raster(ofile, dataset, 'GTiff', compression='LZMA')  #
-    # export_raster(ifile[:-4]+'_DEFLATE3ZL1.tiff', dataset, 'GTiff', compression='DEFLATE')  # 318, 277 PRED 3
-    # export_raster(ifile[:-4]+'_ZSTD3ZL1.tiff', dataset, 'GTiff', compression='ZSTD')  # 241, 281 pred=3
+    # export_raster(ifile[:-4]+'_NONE.tif', dataset, 'GTiff')  # 65s
+    # export_raster(ifile[:-4]+'_PACKBITS.tif', dataset, 'GTiff', compression='PACKBITS')  # 82s
+    # export_raster(ifile[:-4]+'_LZW.tif', dataset, 'GTiff', compression='LZW') # 132
+    # export_raster(ifile[:-4]+'_LZWA.tif', dataset, 'GTiff', compression='LZMA')  #>900s
+    # export_raster(ifile[:-4]+'_ZSTD.tif', dataset, 'GTiff', compression='ZSTD')  # 74s
 
-    # best is zstd pred 3 zlvl 1
-    # then deflade pred 3 zlvl 1
+    export_raster(ifile[:-4]+'_DEFLATE.tif', dataset, 'GTiff',
+                  compression='DEFLATE', bandsort=True)  # 104s, 4,246,330
 
     getinfo('End')
 
 
 if __name__ == "__main__":
     _filespeedtest()
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/menu.py` & `pygmi-3.2.7.16/pygmi/raster/menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
     def reproj(self):
         """Reproject a dataset."""
         self.parent.item_insert('Step', 'Data Reprojection',
                                 dataprep.DataReproj)
 
     def merge(self):
         """Merge datasets."""
-        self.parent.item_insert('Io', 'Data Merge', dataprep.DataMerge)
+        self.parent.item_insert('Io', 'Data Mosaic', dataprep.DataMerge)
 
     def lstack(self):
         """Layer stack datasets."""
         self.parent.item_insert('Step', 'Data Layer Stack',
                                 dataprep.DataLayerStack)
 
     def import_data(self):
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/modest_image.py` & `pygmi-3.2.7.16/pygmi/raster/modest_image.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/raster/normalisation.py` & `pygmi-3.2.7.16/pygmi/raster/normalisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         if not nodialog:
             temp = self.exec_()
             if temp == 0:
                 return False
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/pcs.csv` & `pygmi-3.2.7.16/pygmi/raster/pcs.csv`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/raster/show_table.py` & `pygmi-3.2.7.16/pygmi/raster/show_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         self.show()
         data = self.indata['Cluster']
 
         self.bands = ['Clusters: ' + str(i.metadata['Cluster']['no_clusters'])
                       for i in data]
 
         if 'input_type' not in data[0].metadata['Cluster']:
-            self.showprocesslog('Your dataset does not qualify')
+            self.showlog('Your dataset does not qualify')
             return False
 
         self.cols = list(data[0].metadata['Cluster']['input_type'])
         self.data = []
 
         for i in data:
             val = i.metadata['Cluster']['center'].tolist()
@@ -336,16 +336,16 @@
 
     """
     with open(ofile, 'a', encoding='utf-8') as fobj:
         htmp = cols[0]
         for i in cols[1:]:
             htmp += ',' + i
 
-        for k, _ in enumerate(bands):
-            fobj.write(bands[k]+'\n')
+        for k, bandsk in enumerate(bands):
+            fobj.write(bandsk+'\n')
             fobj.write(htmp+'\n')
             for i, _ in enumerate(data[k]):
                 rtmp = str(data[k][i][0])
                 for j in range(1, len(data[k][0])):
                     rtmp += ','+str(data[k][i][j])
                 fobj.write(rtmp+'\n')
             fobj.write('\n')
```

### Comparing `pygmi-3.2.6.5/pygmi/raster/smooth.py` & `pygmi-3.2.7.16/pygmi/raster/smooth.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,41 +147,39 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('No Raster Data.')
+            self.showlog('No Raster Data.')
             return False
 
         if not nodialog:
             temp = self.exec_()
             if temp == 0:
                 return False
             self.parent.process_is_active(True)
 
-        self.showprocesslog('Smoothing ')
+        self.showlog('Smoothing ')
         data = copy.deepcopy(self.indata['Raster'])
+
         if self.radiobutton_2dmean.isChecked():
-            for i, _ in enumerate(data):
-                data[i].data = self.mov_win_filt(data[i].data, self.fmat,
-                                                 '2D Mean')
-                data[i].dataid = data[i].dataid+' 2D Mean'
-
-        if self.radiobutton_2dmedian.isChecked():
-            for i, _ in enumerate(data):
-                data[i].data = self.mov_win_filt(data[i].data, self.fmat,
-                                                 '2D Median')
-                data[i].dataid = data[i].dataid+' 2D Median'
+            filt = '2D Mean'
+        else:
+            filt = '2D Median'
+
+        for dat in data:
+            dat.data = self.mov_win_filt(dat.data, self.fmat, filt)
+            dat.dataid = dat.dataid+' '+filt
 
         if not nodialog:
             self.parent.process_is_active(False)
         self.outdata['Raster'] = data
-        self.showprocesslog('Finished!', True)
+        self.showlog('Finished!', True)
 
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
@@ -407,15 +405,15 @@
         dat = dat.astype(float)
         dat.data[dat.mask] = np.nan
 
         if itype == '2D Mean':
             out = ssig.correlate(dat, fmat, 'same', method='direct')
 
         elif itype == '2D Median':
-            self.showprocesslog('Calculating Median...')
+            self.showlog('Calculating Median...')
             out = np.ma.zeros([rowd, cold])*np.nan
             out.mask = np.ma.getmaskarray(dat)
             fmat = fmat.astype(bool)
             dummy = dummy.data
 
             for i in self.piter(range(rowd)):
                 for j in range(cold):
```

### Comparing `pygmi-3.2.6.5/pygmi/rsense/change.py` & `pygmi-3.2.7.16/pygmi/rsense/change.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,27 +26,27 @@
 
 import datetime
 from pathlib import Path
 from xml.etree import ElementTree
 from PyQt5 import QtWidgets, QtCore
 import numpy as np
 import pandas as pd
-from osgeo import gdal, osr, ogr
+import geopandas as gpd
 from shapely.geometry.polygon import Polygon
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
 from matplotlib import colormaps
 import matplotlib.animation as manimation
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.backends.backend_qt5 import NavigationToolbar2QT
 
-from pygmi.raster.datatypes import Data
 from pygmi.misc import frm
 from pygmi.raster.ginterp import histcomp, norm255
 from pygmi.misc import BasicModule
+from pygmi.raster.iodefs import get_raster
 
 
 class CreateSceneList(BasicModule):
     """
     Create Scene List.
 
     This class creates a list of scenes for use in change detection.
@@ -126,83 +126,84 @@
         sfile = self.shapefile.text()
 
         if idir == '' or sfile == '':
             return False
 
         if not self.useall.isChecked():
             if sfile[-3:] == 'shp':
-                ddpoints = get_shape_coords(sfile)
+                ddpoints = get_shape_coords(sfile, True)
             else:
                 ddpoints = get_kml_coords(sfile)
             ddpoints2 = Polygon(ddpoints)
 
         if self.isrecursive.isChecked():
             subfiles = Path(idir).rglob('*.tif')
         else:
             subfiles = Path(idir).glob('*.tif')
 
         subfiles = list(subfiles)
         dtime = []
         flist = []
         nodates = False
         for ifile in self.piter(subfiles):
-            dataset = gdal.Open(str(ifile), gdal.GA_ReadOnly)
-            metadata = dataset.GetMetadata()
+            dattmp = get_raster(str(ifile), metaonly=True)
 
             if not self.useall.isChecked():
-                gtr = dataset.GetGeoTransform()
-                cols = dataset.RasterXSize
-                rows = dataset.RasterYSize
-                dxlim = (gtr[0], gtr[0]+gtr[1]*cols)
-                dylim = (gtr[3]+gtr[5]*rows, gtr[3])
+                dxlim = dattmp[0].extent[:2]
+                dylim = dattmp[0].extent[2:]
 
                 coords = [[dxlim[0], dylim[0]],
                           [dxlim[0], dylim[1]],
                           [dxlim[1], dylim[1]],
                           [dxlim[1], dylim[0]],
                           [dxlim[0], dylim[0]]]
 
                 coords2 = Polygon(coords)
-                if not coords2.contains(ddpoints2):
+                gdf = gpd.GeoDataFrame(geometry=[coords2])
+                gdf = gdf.set_crs(dattmp[0].crs)
+                gdf = gdf.to_crs(epsg=4326)
+
+                gdf2 = gpd.GeoDataFrame(geometry=[ddpoints2])
+                gdf2 = gdf2.set_crs(4326)
+
+                if not gdf.intersects(ddpoints2).loc[0]:
                     continue
 
-            if 'TIFFTAG_DATETIME' not in metadata:
+            dt = dattmp[0].datetime
+            if dt is None:
                 dt = datetime.datetime(1900, 1, 1)
                 nodates = True
-            else:
-                dtimestr = metadata['TIFFTAG_DATETIME']
-                dt = datetime.datetime.strptime(dtimestr, '%Y:%m:%d %H:%M:%S')
 
             dtime.append(dt)
             flist.append(ifile)
 
         if nodates is True:
-            self.showprocesslog('Some of your scenes do not have dates. '
-                                'Correct this in the output spreadsheet')
+            self.showlog('Some of your scenes do not have dates. '
+                         'Correct this in the output spreadsheet')
 
         if not flist:
-            self.showprocesslog('No scenes could be found. Please make sure '
-                                'that your shapefile or kml file is in the '
-                                'area of your scenes and in the same '
-                                'projection.')
+            self.showlog('No scenes could be found. Please make sure '
+                         'that your shapefile or kml file is in the '
+                         'area of your scenes and in the same '
+                         'projection.')
             return False
 
-        self.showprocesslog('Updating spreadsheet...')
+        self.showlog('Updating spreadsheet...')
 
         df = pd.DataFrame()
         df['Datetime'] = dtime
         df['Filename'] = flist
         df['Use'] = True
         df['Shapefile'] = sfile
 
         df.sort_values('Datetime', inplace=True)
 
         self.outdata['SceneList'] = df
 
-        self.showprocesslog('Saving to disk...')
+        self.showlog('Saving to disk...')
 
         ext = ('Scene List File (*.xlsx)')
 
         filename, _ = QtWidgets.QFileDialog.getSaveFileName(
             self.parent, 'Save File', '.', ext)
         if filename == '':
             return False
@@ -448,15 +449,16 @@
         rtmp2 = dat[self.bands[1]].data
         rtmp3 = dat[self.bands[0]].data
 
         rtmp1 = (rtmp1-rtmp1.min())/rtmp1.ptp()
         rtmp2 = (rtmp2-rtmp2.min())/rtmp2.ptp()
         rtmp3 = (rtmp3-rtmp3.min())/rtmp3.ptp()
 
-        alpha = np.logical_not(rtmp1 == 0.)
+        # alpha = np.logical_not(rtmp1 == 0.)
+        alpha = ~rtmp1.mask
 
         dtmp = np.array([rtmp1, rtmp2, rtmp3, alpha])
         dtmp = np.moveaxis(dtmp, 0, 2)
         dtmp = dtmp*255
         dtmp = dtmp.astype(np.uint8)
 
         extent = dat[self.bands[0]].extent
@@ -512,17 +514,17 @@
                 self.cbar = None
 
             mask = (dat[self.bands[2]].data == 0.)
             red = np.ma.array(dat[self.bands[2]].data, mask=mask)
             green = np.ma.array(dat[self.bands[1]].data, mask=mask)
             blue = np.ma.array(dat[self.bands[0]].data, mask=mask)
 
-            red = histcomp(red, nbr_bins=10000, perc=2.)
-            green = histcomp(green, nbr_bins=10000, perc=2.)
-            blue = histcomp(blue, nbr_bins=10000, perc=2.)
+            red, _, _ = histcomp(red, nbr_bins=10000, perc=2.)
+            green, _, _ = histcomp(green, nbr_bins=10000, perc=2.)
+            blue, _, _ = histcomp(blue, nbr_bins=10000, perc=2.)
 
             red = norm255(red)
             green = norm255(green)
             blue = norm255(blue)
 
             red[mask] = 0
             green[mask] = 0
@@ -600,15 +602,17 @@
         vlayout = QtWidgets.QVBoxLayout(self)
         hlayout = QtWidgets.QHBoxLayout()
         hlayout2 = QtWidgets.QHBoxLayout()
 
         self.canvas = MyMplCanvas(self, width=5, height=4, dpi=100)
 
         mpl_toolbar = NavigationToolbar2QT(self.canvas, self)
-        self.slider = QtWidgets.QScrollBar(QtCore.Qt.Horizontal)
+        self.slider = MySlider()
+        self.slider.setOrientation(QtCore.Qt.Horizontal)
+
         self.button1 = QtWidgets.QPushButton('Start Capture')
         self.button2 = QtWidgets.QPushButton('Update Scene List File')
         self.button3 = QtWidgets.QPushButton('Next Scene')
         self.cb_use = QtWidgets.QCheckBox('Use Scene')
         self.cb_display = QtWidgets.QCheckBox('Only Display Scenes Flagged '
                                               'for Use')
         self.cb_display.setChecked(True)
@@ -653,15 +657,15 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'SceneList' not in self.indata:
-            self.showprocesslog('You need a scene list.')
+            self.showlog('You need a scene list.')
             return False
 
         self.df = self.indata['SceneList']
         sfile = self.df['Shapefile'][0]
 
         dates = self.df.Datetime[self.curimage]
         dat = self.get_tiff(self.df.Filename[self.curimage], firstrun=True)
@@ -899,96 +903,158 @@
         datall : dictionary or None
             Data images
 
         """
         datall = {}
         ifile = str(ifile)
 
-        dataset = gdal.Open(ifile, gdal.GA_ReadOnly)
+        dataset = get_raster(ifile)
 
-        self.pbar2.setMinimum(0)
-        self.pbar2.setValue(0)
-        self.pbar2.setMaximum(dataset.RasterCount-1)
-
-        gtr = dataset.GetGeoTransform()
-        cols = dataset.RasterXSize
-        rows = dataset.RasterYSize
-        dx = abs(gtr[1])
-        dy = abs(gtr[5])
-        dxlim = (gtr[0], gtr[0]+gtr[1]*cols)
-        dylim = (gtr[3]+gtr[5]*rows, gtr[3])
+        for i, band in enumerate(dataset):
+            datall[i+1] = band
+        # dx = dataset[0].xdim
+        # dy = dataset[0].ydim
+        dxlim = dataset[0].extent[:2]
+        dylim = dataset[0].extent[2:]
+        # rows, cols = dataset[0].data.shape
+
+        # # dataset = gdal.Open(ifile, gdal.GA_ReadOnly)
+
+        # self.pbar2.setMinimum(0)
+        # self.pbar2.setValue(0)
+        # self.pbar2.setMaximum(dataset.RasterCount-1)
+
+        # # gtr = dataset.GetGeoTransform()
+        # # cols = dataset.RasterXSize
+        # # rows = dataset.RasterYSize
+        # # dx = abs(gtr[1])
+        # # dy = abs(gtr[5])
+        # # dxlim = (gtr[0], gtr[0]+gtr[1]*cols)
+        # # dylim = (gtr[3]+gtr[5]*rows, gtr[3])
 
         axes = self.canvas.ax1
 
         if firstrun is True:
             axes.set_xlim(dxlim[0], dxlim[1])
             axes.set_ylim(dylim[0], dylim[1])
 
-        ext = (axes.transAxes.transform([(1, 1)]) -
-               axes.transAxes.transform([(0, 0)]))[0]
+        # ext = (axes.transAxes.transform([(1, 1)]) -
+        #        axes.transAxes.transform([(0, 0)]))[0]
 
-        xlim, ylim = axes.get_xlim(), axes.get_ylim()
+        # xlim, ylim = axes.get_xlim(), axes.get_ylim()
 
-        xoff = max(int((xlim[0]-dxlim[0])/dx), 0)
-        yoff = max(-int((ylim[1]-dylim[1])/dy), 0)
+        # xoff = max(int((xlim[0]-dxlim[0])/dx), 0)
+        # yoff = max(-int((ylim[1]-dylim[1])/dy), 0)
 
-        xoff1 = min(int((xlim[1]-dxlim[1])/dx), 0)
-        yoff1 = min(-int((ylim[0]-dylim[0])/dy), 0)
+        # xoff1 = min(int((xlim[1]-dxlim[1])/dx), 0)
+        # yoff1 = min(-int((ylim[0]-dylim[0])/dy), 0)
+
+        # xsize = cols-xoff+xoff1
+        # ysize = rows-yoff+yoff1
+
+        # xdim = dx*xsize/int(ext[0])
+        # ydim = dy*ysize/int(ext[1])
+
+        # xbuf = min(xsize, int(ext[0]))
+        # ybuf = min(ysize, int(ext[1]))
+
+        # for i in range(dataset.RasterCount):
+
+        #     rtmp = dataset.GetRasterBand(i+1)
+        #     nval = rtmp.GetNoDataValue()
+        #     bandid = rtmp.GetDescription()
+        #     if bandid == '':
+        #         bandid = 'Band '+str(i+1)
+
+        #     dat = Data()
+        #     dat.data = rtmp.ReadAsArray(xoff, yoff, xsize, ysize, xbuf, ybuf)
+
+        #     if dat.data is None:
+        #         self.showlog('Error: Dataset could not be read '
+        #                             'properly')
+
+        #     if dat.data.dtype.kind == 'i':
+        #         if nval is None:
+        #             nval = 999999
+        #         nval = int(nval)
+        #     elif dat.data.dtype.kind == 'u':
+        #         if nval is None:
+        #             nval = 0
+        #         nval = int(nval)
+        #     else:
+        #         if nval is None:
+        #             nval = 1e+20
+        #         nval = float(nval)
+
+        #     dat.nodata = nval
+        #     dat.xdim = xdim
+        #     dat.ydim = ydim
+        #     dat.wkt = dataset.GetProjection()
+        #     datall[i+1] = dat
 
-        xsize = cols-xoff+xoff1
-        ysize = rows-yoff+yoff1
+        #     self.pbar2.setValue(i)
 
-        xdim = dx*xsize/int(ext[0])
-        ydim = dy*ysize/int(ext[1])
+        if datall == {}:
+            datall = None
 
-        xbuf = min(xsize, int(ext[0]))
-        ybuf = min(ysize, int(ext[1]))
+        # dataset = None
 
-        for i in range(dataset.RasterCount):
+        return datall
 
-            rtmp = dataset.GetRasterBand(i+1)
-            nval = rtmp.GetNoDataValue()
-            bandid = rtmp.GetDescription()
-            if bandid == '':
-                bandid = 'Band '+str(i+1)
 
-            dat = Data()
-            dat.data = rtmp.ReadAsArray(xoff, yoff, xsize, ysize, xbuf, ybuf)
+class MySlider(QtWidgets.QSlider):
+    """
+    My Slider.
 
-            if dat.data is None:
-                self.showprocesslog('Error: Dataset could not be read '
-                                    'properly')
+    Custom class which allows clicking on a horizontal slider bar with slider
+    moving to click in a single step.
+    """
 
-            if dat.data.dtype.kind == 'i':
-                if nval is None:
-                    nval = 999999
-                nval = int(nval)
-            elif dat.data.dtype.kind == 'u':
-                if nval is None:
-                    nval = 0
-                nval = int(nval)
-            else:
-                if nval is None:
-                    nval = 1e+20
-                nval = float(nval)
-
-            dat.nodata = nval
-            dat.xdim = xdim
-            dat.ydim = ydim
-            dat.wkt = dataset.GetProjection()
-            datall[i+1] = dat
+    def __init__(self, parent=None):
+        super().__init__(parent)
 
-            self.pbar2.setValue(i)
+    def mousePressEvent(self, event):
+        """
+        Mouse press event.
 
-        if datall == {}:
-            datall = None
+        Parameters
+        ----------
+        event : event
+            Event variable.
 
-        dataset = None
+        Returns
+        -------
+        None.
 
-        return datall
+        """
+        self.setValue(QtWidgets.QStyle.sliderValueFromPosition(self.minimum(),
+                                                               self.maximum(),
+                                                               event.x(),
+                                                               self.width()))
+
+    def mouseMoveEvent(self, event):
+        """
+        Mouse move event.
+
+        Jump to pointer position while moving.
+
+        Parameters
+        ----------
+        event : event
+            Event variable.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.setValue(QtWidgets.QStyle.sliderValueFromPosition(self.minimum(),
+                                                               self.maximum(),
+                                                               event.x(),
+                                                               self.width()))
 
 
 def get_shape_coords(sfile, todegrees=False):
     """
     Get coordinates from a shapefile.
 
     Parameters
@@ -1000,53 +1066,26 @@
 
     Returns
     -------
     ddpoints : numpy array
         Output coordinates.
 
     """
-    sr = osr.SpatialReference()
-    sr.ImportFromEPSG(32735)  # utm 35s
-    sr.SetAxisMappingStrategy(osr.OAMS_TRADITIONAL_GIS_ORDER)
-
-    vec = ogr.Open(sfile)
-    layer = vec.GetLayer(0)
-
-    srdd = osr.SpatialReference()
-    srdd.ImportFromEPSG(4326)  # degrees
-    srdd.SetAxisMappingStrategy(osr.OAMS_TRADITIONAL_GIS_ORDER)
-
-    coordtrans = osr.CoordinateTransformation(sr, srdd)
-
-    points = []
-    poly = layer.GetNextFeature()
-    geom = poly.GetGeometryRef()
-
-    ifin = 0
-    imax = 0
-    if geom.GetGeometryName() == 'MULTIPOLYGON':
-        for i in range(geom.GetGeometryCount()):
-            geom.GetGeometryRef(i)
-            itmp = geom.GetGeometryRef(i)
-            itmp = itmp.GetGeometryRef(0).GetPointCount()
-            if itmp > imax:
-                imax = itmp
-                ifin = i
-        geom = geom.GetGeometryRef(ifin)
-
-    pts = geom.GetGeometryRef(0)
-    for p in range(pts.GetPointCount()):
-        points.append((pts.GetX(p), pts.GetY(p)))
+    gdf = gpd.read_file(sfile)
+    gdf = gdf[gdf.geometry != None]
 
     if todegrees is True:
-        ddpoints = np.array(coordtrans.TransformPoints(points))
-        ddpoints = ddpoints[:, :2]
-    else:
-        ddpoints = np.array(points)
+        gdf = gdf.to_crs(epsg=4326)
 
+    gdf = gdf.explode(index_parts=False)
+    coords = gdf.geometry.apply(lambda geom: np.array(geom.exterior.coords))
+
+    ddpoints = np.vstack(coords)
+
+    ddpoints = ddpoints[:, :2]
     return ddpoints
 
 
 def get_kml_coords(kml):
     """
     Extract points from kml.
 
@@ -1079,28 +1118,51 @@
     coordinates = np.array(coordinates)
     return coordinates
 
 
 def _testfn():
     """Test routine."""
     import sys
-    sfile = r'd:\Work\Workdata\change\fl35.shp'
-    pdir = r'd:\Work\Workdata\change\Planet'
+    from IPython import get_ipython
+    get_ipython().run_line_magic('matplotlib', 'inline')
+
+    sfile = r'd:\Workdata\change\fl35.shp'
+    sfile = r'd:\Workdata\change\Planet\area-dd.shp'
+    pdir = r'd:\Workdata\change\Planet'
 
     app = QtWidgets.QApplication(sys.argv)
 
     CSL = CreateSceneList(None)
     CSL.isrecursive.setChecked(True)
     CSL.shapefile.setText(sfile)
     CSL.scenefile.setText(pdir)
     CSL.settings(True)
 
     plt.show()
 
 
+def _testview():
+    """Test routine."""
+    import sys
+    from IPython import get_ipython
+    get_ipython().run_line_magic('matplotlib', 'inline')
+
+    ifile = r'd:\Workdata\change\planet\paddock.xlsx'
+
+    app = QtWidgets.QApplication(sys.argv)
+
+    LSL = LoadSceneList()
+    LSL.ifile = ifile
+    LSL.settings(True)
+
+    SV = SceneViewer()
+    SV.indata = LSL.outdata
+    SV.settings()
+
+
 def _testanim():
     """Test for animation."""
     wfile = r'd:\Work\Workdata\change\tmp.gif'
 
     fig = plt.figure(dpi=150)
 
     writer = manimation.PillowWriter(fps=4)
@@ -1114,8 +1176,8 @@
         fig.suptitle(str(i))
         writer.grab_frame()
     plt.show()
     writer.finish()
 
 
 if __name__ == "__main__":
-    _testanim()
+    _testview()
```

### Comparing `pygmi-3.2.6.5/pygmi/rsense/features.py` & `pygmi-3.2.7.16/pygmi/rsense/features.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/rsense/hyperspec.py` & `pygmi-3.2.7.16/pygmi/rsense/hyperspec.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     Attributes
     ----------
     parent : parent
         reference to the parent routine
     """
 
     def __init__(self, parent=None):
-        self.figure = Figure()
+        self.figure = Figure(layout='constrained')
 
         super().__init__(self.figure)
         self.setParent(parent)
 
         self.parent = parent
         self.datarr = []
         self.wvl = []
@@ -114,23 +114,29 @@
         ax1.set_ylim((0, rows))
         ax1.xaxis.set_visible(False)
         ax1.yaxis.set_visible(False)
 
         ax1.xaxis.set_major_formatter(frm)
         ax1.yaxis.set_major_formatter(frm)
 
-        ax1.plot(self.col, self.row, '+w')
+        if self.rotate is True:
+            ax1.plot(self.row, self.col, '+w')
+        else:
+            ax1.plot(self.col, self.row, '+w')
+        # print(self.col, self.row)
 
         ax2 = self.figure.add_subplot(212)
 
-        prof = []
-        for i in self.datarr:
-            prof.append(i[self.row, self.col])
+        # prof = []
+        # for i in self.datarr:
+        #     prof.append(i[self.row, self.col])
 
-        prof = np.ma.stack(prof)/self.refl
+        prof = [i[self.row, self.col] for i in self.datarr]
+
+        prof = np.ma.stack(prof).filled(0)/self.refl
 
         ax2.format_coord = lambda x, y: f'Wavelength: {x:1.2f}, Y: {y:1.2f}'
         ax2.grid(True)
         ax2.set_xlabel('Wavelength')
 
         if self.remhull is True:
             hull = phull(prof)
@@ -160,15 +166,15 @@
         bmax = self.feature[2]
 
         rect = mpatches.Rectangle((bmin, zmin), bmax-bmin, zmax-zmin)
         rect.set_facecolor([0, 1, 0])
         rect.set_alpha(0.5)
         ax2.add_patch(rect)
 
-        self.figure.tight_layout()
+        # self.figure.tight_layout()
         self.figure.canvas.draw()
 
 
 class AnalSpec(BasicModule):
     """Analyse spectra."""
 
     def __init__(self, parent=None):
@@ -424,37 +430,37 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if 'Raster' not in self.indata:
-            self.showprocesslog('Error: You must have a multi-band raster '
-                                'dataset in addition to your cluster '
-                                'analysis results')
+            self.showlog('Error: You must have a multi-band raster '
+                         'dataset in addition to your cluster '
+                         'analysis results')
             return False
 
         if 'wavelength' not in self.indata['Raster'][0].metadata['Raster']:
-            self.showprocesslog('Error: Your data should have wavelengths in'
-                                ' the metadata')
+            self.showlog('Error: Your data should have wavelengths in'
+                         ' the metadata')
             return False
 
         dat = self.indata['Raster']
 
         needsmerge = False
         rows, cols = dat[0].data.shape
 
         for i in dat:
             irows, icols = i.data.shape
             if irows != rows or icols != cols:
                 needsmerge = True
 
         if needsmerge is True:
-            self.showprocesslog('Error: Your data bands have different sizes. '
-                                'Use Layer Stack to fix this first')
+            self.showlog('Error: Your data bands have different sizes. '
+                         'Use Layer Stack to fix this first')
             return False
 
         wavelengths = []
         dat2 = []
         for i in dat:
             if 'wavelength' in i.metadata['Raster']:
                 wavelengths.append(i.metadata['Raster']['wavelength'])
@@ -468,21 +474,23 @@
 
         dat2 = []
         wvl = []
         for j in dat:
             dat2.append(j.data)
             wvl.append(float(j.metadata['Raster']['wavelength']))
 
+        dat2 = np.ma.array(dat2)
+
         self.map.datarr = dat2
         self.map.nodata = dat[0].nodata
         self.map.wvl = np.array(wvl)
         if self.map.wvl.max() < 20:
             self.map.wvl = self.map.wvl*1000.
-            self.showprocesslog('Wavelengths appear to be in nanometers. '
-                                'Converting to micrometers.')
+            self.showlog('Wavelengths appear to be in nanometers. '
+                         'Converting to micrometers.')
 
         bands = [i.dataid for i in self.indata['Raster']]
 
         self.combo.clear()
         self.combo.addItems(bands)
         self.combo.currentIndexChanged.connect(self.on_combo)
 
@@ -685,15 +693,15 @@
         -------
         bool
             True if successful, False otherwise.
 
         """
         tmp = []
         if 'Raster' not in self.indata and 'RasterFileList' not in self.indata:
-            self.showprocesslog('No Satellite Data')
+            self.showlog('No Satellite Data')
             return False
 
         self.feature = features.feature
         self.ratio = features.ratio
 
         self.cb_ratios.disconnect()
         self.product = features.product.copy()
@@ -780,29 +788,30 @@
 
         if 'RasterFileList' in self.indata:
             flist = self.indata['RasterFileList']
             odir = os.path.join(os.path.dirname(flist[0]), 'feature')
 
             os.makedirs(odir, exist_ok=True)
             for ifile in flist:
-                self.showprocesslog('Processing '+os.path.basename(ifile))
+                self.showlog('Processing '+os.path.basename(ifile))
 
                 dat = get_raster(ifile)
                 datfin = calcfeatures(dat, mineral, self.feature, self.ratio,
                                       product, rfilt, piter=self.piter)
 
                 ofile = (os.path.basename(ifile).split('.')[0] + '_' +
                          mineral.replace(' ', '_') + '.tif')
                 ofile = os.path.join(odir, ofile)
                 if datfin[0].data.mask.min() == True:
-                    self.showprocesslog(' Could not find any ' + mineral +
-                                        '. No data to export.')
+                    self.showlog(' Could not find any ' + mineral +
+                                 '. No data to export.')
                 else:
-                    self.showprocesslog('Exporting '+os.path.basename(ofile))
-                    export_raster(ofile, datfin, 'GTiff', piter=self.piter)
+                    self.showlog('Exporting '+os.path.basename(ofile))
+                    export_raster(ofile, datfin, 'GTiff', piter=self.piter,
+                                  showlog=self.showlog)
 
         elif 'Raster' in self.indata:
             dat = self.indata['Raster']
             datfin = calcfeatures(dat, mineral, self.feature, self.ratio,
                                   product, rfilt, piter=self.piter)
 
         if datfin[0].data.mask.min() == True:
@@ -1254,36 +1263,20 @@
 
 def _testfn():
     """Test routine."""
     from pygmi.rsense.iodefs import get_data
 
     app = QtWidgets.QApplication(sys.argv)
 
-    # ifile = r"d:\Workdata\Hyperspectral\080_0824-0920_ref_rect_clip.hdr"
-    # ifile = r"d:\Workdata\Remote Sensing\hyperion\EO1H1760802013198110KF_1T.ZIP"
     ifile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\hyperspectral\071_0818-0932_ref_rect_BSQ.hdr"
 
-    xoff = 0
-    yoff = 2000
-    xsize = None
-    ysize = 1000
-    nodata = 15000
-    nodata = 0
-
-    iraster = (xoff, yoff, xsize, ysize)
-    iraster = None
-
-    # data = get_raster(ifile, nval=nodata, iraster=iraster, piter=pbar.iter)
     data = get_data(ifile)
 
-    # data = get_raster(ifile, piter=pbar.iter)
-
     tmp = ProcFeatures(None)
     tmp.indata['Raster'] = data
-    # tmp.cb_ratios.setCurrentText('ferric iron')
     tmp.settings()
 
     dat = tmp.outdata['Raster'][0]
 
     plt.figure(dpi=150)
     plt.imshow(dat.data)
     plt.colorbar()
@@ -1312,149 +1305,9 @@
 
     app = QtWidgets.QApplication(sys.argv)
     tmp = AnalSpec()
     tmp.indata['Raster'] = data
     tmp.settings()
 
 
-def _testfn3():
-    """Test."""
-    ifile1 = r'd:\Workdata\Lithosphere\merge\cut-087-0824_iMNF15.hdr'
-    ifile2 = r'd:\Workdata\Lithosphere\merge\cut-088-0824_iMNF15.hdr'
-    ifile3 = r'd:\Workdata\Lithosphere\merge\cut-089-0824_iMNF15.hdr'
-
-    feat = 18
-
-    yoff = 2425
-    ysize = 400
-    nodata = 0
-    iraster = (0, yoff, None, ysize)
-
-    data1 = get_raster(ifile1, nval=nodata, iraster=iraster)
-    data2 = get_raster(ifile2, nval=nodata, iraster=iraster)
-    data3 = get_raster(ifile3, nval=nodata, iraster=iraster)
-
-    plt.figure(dpi=150)
-    plt.imshow(data1[0].data, extent=data1[0].extent)
-    plt.plot(277545, 6774900, '+k')
-    plt.show()
-
-    plt.figure(dpi=150)
-    plt.imshow(data2[0].data, extent=data2[0].extent)
-    plt.plot(277545, 6774900, '+k')
-    plt.plot(279900, 6774900, '+k')
-    plt.show()
-
-    plt.figure(dpi=150)
-    plt.imshow(data3[0].data, extent=data3[0].extent)
-    plt.plot(279900, 6774900, '+k')
-    plt.show()
-
-    yoff = 2625
-    ysize = 1
-    nodata = 0
-    iraster = (0, yoff, None, ysize)
-
-    data1 = get_raster(ifile1, nval=nodata, iraster=iraster)
-    data2 = get_raster(ifile2, nval=nodata, iraster=iraster)
-    data3 = get_raster(ifile3, nval=nodata, iraster=iraster)
-
-    for i in range(2):
-        if i == 0:
-            xxx = 277545
-            yyy = 6774900
-        else:
-            xxx = 279900
-            yyy = 6774900
-            data1 = data3
-
-        i1 = int((xxx-data1[0].extent[0])/data1[0].xdim)
-        i2 = int((xxx-data2[0].extent[0])/data2[0].xdim)
-
-        # Get list of wavelengths and data
-        dat1 = []
-        xval1 = []
-        for j in data1:
-            dat1.append(j.data)
-            refl = round(float(re.findall(r'[\d\.\d]+', j.dataid)[-1])*1000, 2)
-            xval1.append(refl)
-
-        xval1 = np.array(xval1)
-        dat1 = np.array(dat1)
-
-        dat2 = []
-        xval2 = []
-        for j in data2:
-            dat2.append(j.data)
-            refl = round(float(re.findall(r'[\d\.\d]+', j.dataid)[-1])*1000, 2)
-            xval2.append(refl)
-
-        xval2 = np.array(xval2)
-        dat2 = np.array(dat2)
-
-        dat1 = dat1[55: 98]
-        dat2 = dat2[55: 98]
-        xval1 = xval1[55: 98]
-        xval2 = xval2[55: 98]
-
-        fdat = []
-        xdat = []
-        fdat.append(dat1[:, 0, i1])
-        fdat.append(dat2[:, 0, i2])
-        xdat = xval1
-
-        fdat = np.array(fdat)
-
-        ptmp = np.array([0, 0])
-        dtmp = np.array([0, 0])
-
-        ptmp, dtmp = fproc(fdat, ptmp, dtmp, 11, 19, xdat)
-
-        spec1 = dat1[:, 0, i1]
-        spec2 = dat2[:, 0, i2]
-
-        plt.figure(dpi=150)
-        plt.title(str(i)+': '+str(i1))
-        plt.plot(xval1, spec1)
-        plt.plot(xval2, spec2, '-.')
-        ymin, ymax = plt.gca().get_ylim()
-        plt.vlines(ptmp[0], ymin, ymax, 'k')
-        plt.vlines(ptmp[1], ymin, ymax, 'k')
-
-        spec1 = spec1/phull(spec1)
-        spec2 = spec2/phull(spec2)
-
-        plt.figure(dpi=150)
-        plt.title(str(i)+': '+str(i1))
-        plt.plot(xval1, spec1)
-        plt.plot(xval2, spec2, 'r-.')
-
-        plt.plot(xval1[11:19], spec1[11:19], '.')
-        plt.plot(xval2[11:19], spec2[11:19], '.')
-
-        ymin, ymax = plt.gca().get_ylim()
-        plt.vlines(ptmp[0], ymin, ymax, label=str(ptmp[0]))
-        plt.vlines(ptmp[1], ymin, ymax, colors='r', linestyles='-.',
-                   label=str(ptmp[1]))
-        plt.legend()
-        plt.show()
-
-        plt.figure(dpi=150)
-
-        dat1 = np.ma.masked_equal(dat1, 0)
-        dat2 = np.ma.masked_equal(dat2, 0)
-
-        x1 = np.linspace(data1[0].extent[0], data1[0].extent[1],
-                         dat1[feat, 0].size)
-        x2 = np.linspace(data2[0].extent[0], data2[0].extent[1],
-                         dat2[feat, 0].size)
-        plt.plot(x1, dat1[feat, 0])
-        plt.plot(x2, dat2[feat, 0], '-.')
-
-        ymin, ymax = plt.gca().get_ylim()
-
-        plt.vlines(xxx, ymin, ymax, 'k')
-        plt.show()
-
-
 if __name__ == "__main__":
-    _testfn()
+    _testfn2()
```

### Comparing `pygmi-3.2.6.5/pygmi/rsense/iodefs.py` & `pygmi-3.2.7.16/pygmi/raster/dataprep.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -----------------------------------------------------------------------------
-# Name:        iodefs.py (part of PyGMI)
+# Name:        dataprep.py (part of PyGMI)
 #
 # Author:      Patrick Cole
 # E-Mail:      pcole@geoscience.org.za
 #
-# Copyright:   (c) 2020 Council for Geoscience
+# Copyright:   (c) 2013 Council for Geoscience
 # Licence:     GPL-3.0
 #
 # This file is part of PyGMI
 #
 # PyGMI is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -18,154 +18,91 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
-"""Import remote sensing data."""
-
+"""A set of Raster Data Preparation routines."""
 
+import tempfile
+import math
 import os
-import sys
-import copy
-import xml.etree.ElementTree as ET
 import glob
-import tarfile
-import zipfile
-import datetime
-from collections import defaultdict
-import warnings
-
+import copy
+from collections import Counter
 from PyQt5 import QtWidgets, QtCore
 import numpy as np
-import numexpr as ne
 import pandas as pd
-import geopandas as gpd
-from geopandas import GeoDataFrame
-from shapely.geometry import Point
+from scipy.signal import tukey
 import rasterio
+import rasterio.merge
 from rasterio.crs import CRS
-from natsort import natsorted
-# import contextily as ctx
+from rasterio.warp import calculate_default_transform, reproject
+from rasterio.mask import mask as riomask
+import geopandas as gpd
+from shapely.geometry import LineString
 
 from pygmi import menu_default
 from pygmi.raster.datatypes import Data
-from pygmi.raster.iodefs import get_raster, export_raster
 from pygmi.misc import ProgressBarText, ContextModule, BasicModule
+from pygmi.raster.datatypes import numpy_to_pygmi
 
-warnings.filterwarnings("ignore",
-                        category=rasterio.errors.NotGeoreferencedWarning)
 
-EDIST = {1: 0.98331, 2: 0.9833, 3: 0.9833, 4: 0.9833,
-         5: 0.9833, 6: 0.98332, 7: 0.98333, 8: 0.98335,
-         9: 0.98338, 10: 0.98341, 11: 0.98345, 12: 0.98349,
-         13: 0.98354, 14: 0.98359, 15: 0.98365, 16: 0.98371,
-         17: 0.98378, 18: 0.98385, 19: 0.98393, 20: 0.98401,
-         21: 0.9841, 22: 0.98419, 23: 0.98428, 24: 0.98439,
-         25: 0.98449, 26: 0.9846, 27: 0.98472, 28: 0.98484,
-         29: 0.98496, 30: 0.98509, 31: 0.98523, 32: 0.98536,
-         33: 0.98551, 34: 0.98565, 35: 0.9858, 36: 0.98596,
-         37: 0.98612, 38: 0.98628, 39: 0.98645, 40: 0.98662,
-         41: 0.9868, 42: 0.98698, 43: 0.98717, 44: 0.98735,
-         45: 0.98755, 46: 0.98774, 47: 0.98794, 48: 0.98814,
-         49: 0.98835, 50: 0.98856, 51: 0.98877, 52: 0.98899,
-         53: 0.98921, 54: 0.98944, 55: 0.98966, 56: 0.98989,
-         57: 0.99012, 58: 0.99036, 59: 0.9906, 60: 0.99084,
-         61: 0.99108, 62: 0.99133, 63: 0.99158, 64: 0.99183,
-         65: 0.99208, 66: 0.99234, 67: 0.9926, 68: 0.99286,
-         69: 0.99312, 70: 0.99339, 71: 0.99365, 72: 0.99392,
-         73: 0.99419, 74: 0.99446, 75: 0.99474, 76: 0.99501,
-         77: 0.99529, 78: 0.99556, 79: 0.99584, 80: 0.99612,
-         81: 0.9964, 82: 0.99669, 83: 0.99697, 84: 0.99725,
-         85: 0.99754, 86: 0.99782, 87: 0.99811, 88: 0.9984,
-         89: 0.99868, 90: 0.99897, 91: 0.99926, 92: 0.99954,
-         93: 0.99983, 94: 1.00012, 95: 1.00041, 96: 1.00069,
-         97: 1.00098, 98: 1.00127, 99: 1.00155, 100: 1.00184,
-         101: 1.00212, 102: 1.0024, 103: 1.00269, 104: 1.00297,
-         105: 1.00325, 106: 1.00353, 107: 1.00381, 108: 1.00409,
-         109: 1.00437, 110: 1.00464, 111: 1.00492, 112: 1.00519,
-         113: 1.00546, 114: 1.00573, 115: 1.006, 116: 1.00626,
-         117: 1.00653, 118: 1.00679, 119: 1.00705, 120: 1.00731,
-         121: 1.00756, 122: 1.00781, 123: 1.00806, 124: 1.00831,
-         125: 1.00856, 126: 1.0088, 127: 1.00904, 128: 1.00928,
-         129: 1.00952, 130: 1.00975, 131: 1.00998, 132: 1.0102,
-         133: 1.01043, 134: 1.01065, 135: 1.01087, 136: 1.01108,
-         137: 1.01129, 138: 1.0115, 139: 1.0117, 140: 1.01191,
-         141: 1.0121, 142: 1.0123, 143: 1.01249, 144: 1.01267,
-         145: 1.01286, 146: 1.01304, 147: 1.01321, 148: 1.01338,
-         149: 1.01355, 150: 1.01371, 151: 1.01387, 152: 1.01403,
-         153: 1.01418, 154: 1.01433, 155: 1.01447, 156: 1.01461,
-         157: 1.01475, 158: 1.01488, 159: 1.015, 160: 1.01513,
-         161: 1.01524, 162: 1.01536, 163: 1.01547, 164: 1.01557,
-         165: 1.01567, 166: 1.01577, 167: 1.01586, 168: 1.01595,
-         169: 1.01603, 170: 1.0161, 171: 1.01618, 172: 1.01625,
-         173: 1.01631, 174: 1.01637, 175: 1.01642, 176: 1.01647,
-         177: 1.01652, 178: 1.01656, 179: 1.01659, 180: 1.01662,
-         181: 1.01665, 182: 1.01667, 183: 1.01668, 184: 1.0167,
-         185: 1.0167, 186: 1.0167, 187: 1.0167, 188: 1.01669,
-         189: 1.01668, 190: 1.01666, 191: 1.01664, 192: 1.01661,
-         193: 1.01658, 194: 1.01655, 195: 1.0165, 196: 1.01646,
-         197: 1.01641, 198: 1.01635, 199: 1.01629, 200: 1.01623,
-         201: 1.01616, 202: 1.01609, 203: 1.01601, 204: 1.01592,
-         205: 1.01584, 206: 1.01575, 207: 1.01565, 208: 1.01555,
-         209: 1.01544, 210: 1.01533, 211: 1.01522, 212: 1.0151,
-         213: 1.01497, 214: 1.01485, 215: 1.01471, 216: 1.01458,
-         217: 1.01444, 218: 1.01429, 219: 1.01414, 220: 1.01399,
-         221: 1.01383, 222: 1.01367, 223: 1.01351, 224: 1.01334,
-         225: 1.01317, 226: 1.01299, 227: 1.01281, 228: 1.01263,
-         229: 1.01244, 230: 1.01225, 231: 1.01205, 232: 1.01186,
-         233: 1.01165, 234: 1.01145, 235: 1.01124, 236: 1.01103,
-         237: 1.01081, 238: 1.0106, 239: 1.01037, 240: 1.01015,
-         241: 1.00992, 242: 1.00969, 243: 1.00946, 244: 1.00922,
-         245: 1.00898, 246: 1.00874, 247: 1.0085, 248: 1.00825,
-         249: 1.008, 250: 1.00775, 251: 1.0075, 252: 1.00724,
-         253: 1.00698, 254: 1.00672, 255: 1.00646, 256: 1.0062,
-         257: 1.00593, 258: 1.00566, 259: 1.00539, 260: 1.00512,
-         261: 1.00485, 262: 1.00457, 263: 1.0043, 264: 1.00402,
-         265: 1.00374, 266: 1.00346, 267: 1.00318, 268: 1.0029,
-         269: 1.00262, 270: 1.00234, 271: 1.00205, 272: 1.00177,
-         273: 1.00148, 274: 1.00119, 275: 1.00091, 276: 1.00062,
-         277: 1.00033, 278: 1.00005, 279: 0.99976, 280: 0.99947,
-         281: 0.99918, 282: 0.9989, 283: 0.99861, 284: 0.99832,
-         285: 0.99804, 286: 0.99775, 287: 0.99747, 288: 0.99718,
-         289: 0.9969, 290: 0.99662, 291: 0.99634, 292: 0.99605,
-         293: 0.99577, 294: 0.9955, 295: 0.99522, 296: 0.99494,
-         297: 0.99467, 298: 0.9944, 299: 0.99412, 300: 0.99385,
-         301: 0.99359, 302: 0.99332, 303: 0.99306, 304: 0.99279,
-         305: 0.99253, 306: 0.99228, 307: 0.99202, 308: 0.99177,
-         309: 0.99152, 310: 0.99127, 311: 0.99102, 312: 0.99078,
-         313: 0.99054, 314: 0.9903, 315: 0.99007, 316: 0.98983,
-         317: 0.98961, 318: 0.98938, 319: 0.98916, 320: 0.98894,
-         321: 0.98872, 322: 0.98851, 323: 0.9883, 324: 0.98809,
-         325: 0.98789, 326: 0.98769, 327: 0.9875, 328: 0.98731,
-         329: 0.98712, 330: 0.98694, 331: 0.98676, 332: 0.98658,
-         333: 0.98641, 334: 0.98624, 335: 0.98608, 336: 0.98592,
-         337: 0.98577, 338: 0.98562, 339: 0.98547, 340: 0.98533,
-         341: 0.98519, 342: 0.98506, 343: 0.98493, 344: 0.98481,
-         345: 0.98469, 346: 0.98457, 347: 0.98446, 348: 0.98436,
-         349: 0.98426, 350: 0.98416, 351: 0.98407, 352: 0.98399,
-         353: 0.98391, 354: 0.98383, 355: 0.98376, 356: 0.9837,
-         357: 0.98363, 358: 0.98358, 359: 0.98353, 360: 0.98348,
-         361: 0.98344, 362: 0.9834, 363: 0.98337, 364: 0.98335,
-         365: 0.98333, 366: 0.98331}
-
-K1 = [3040.136402, 2482.375199, 1935.060183, 866.468575, 641.326517]
-K2 = [1735.337945, 1666.398761, 1585.420044, 1350.069147, 1271.221673]
-ESUN = [1848, 1549, 1114, 225.4, 86.63, 81.85, 74.85, 66.49, 59.85]
+class Continuation(BasicModule):
+    """Perform upward and downward continuation on potential field data."""
 
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        self.dataid = QtWidgets.QComboBox()
+        self.continuation = QtWidgets.QComboBox()
+        self.dsb_height = QtWidgets.QDoubleSpinBox()
 
-class ImportData(BasicModule):
-    """Import Data - Interfaces with rasterio routines."""
+        self.setupui()
 
-    def __init__(self, parent=None, extscene=None):
-        super().__init__(parent)
+    def setupui(self):
+        """
+        Set up UI.
+
+        Returns
+        -------
+        None.
+
+        """
+        gridlayout_main = QtWidgets.QGridLayout(self)
+        buttonbox = QtWidgets.QDialogButtonBox()
+        helpdocs = menu_default.HelpButton('pygmi.raster.dataprep.cont')
+        label_band = QtWidgets.QLabel('Band to perform continuation:')
+        label_cont = QtWidgets.QLabel('Continuation type:')
+        label_height = QtWidgets.QLabel('Continuation distance:')
+
+        self.dsb_height.setMaximum(1000000.0)
+        self.dsb_height.setMinimum(0.0)
+        self.dsb_height.setValue(0.0)
+        self.continuation.clear()
+        self.continuation.addItems(['Upward', 'Downward'])
+
+        buttonbox.setOrientation(QtCore.Qt.Horizontal)
+        buttonbox.setCenterButtons(True)
+        buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
 
-        self.filt = ''
-        self.extscene = extscene
+        self.setWindowTitle('Continuation')
+
+        gridlayout_main.addWidget(label_band, 0, 0, 1, 1)
+        gridlayout_main.addWidget(self.dataid, 0, 1, 1, 1)
+
+        gridlayout_main.addWidget(label_cont, 1, 0, 1, 1)
+        gridlayout_main.addWidget(self.continuation, 1, 1, 1, 1)
+        gridlayout_main.addWidget(label_height, 2, 0, 1, 1)
+        gridlayout_main.addWidget(self.dsb_height, 2, 1, 1, 1)
+        gridlayout_main.addWidget(helpdocs, 3, 0, 1, 1)
+        gridlayout_main.addWidget(buttonbox, 3, 1, 1, 3)
+
+        buttonbox.accepted.connect(self.accept)
+        buttonbox.rejected.connect(self.reject)
 
     def settings(self, nodialog=False):
         """
         Entry point into item.
 
         Parameters
         ----------
@@ -174,43 +111,32 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
-        piter = self.parent.pbar.iter
-
-        if self.extscene is None:
+        tmp = []
+        if 'Raster' not in self.indata:
+            self.showlog('No Raster Data.')
             return False
 
-        if not nodialog:
-            self.ifile, self.filt = QtWidgets.QFileDialog.getOpenFileName(
-                self.parent, 'Open File', '.', self.extscene)
-            if self.ifile == '':
-                return False
-        os.chdir(os.path.dirname(self.ifile))
+        for i in self.indata['Raster']:
+            tmp.append(i.dataid)
 
-        dat = get_data(self.ifile, piter, self.showprocesslog, self.extscene)
+        self.dataid.clear()
+        self.dataid.addItems(tmp)
 
-        if dat is None:
-            if self.filt == 'hdf (*.hdf *.h5)':
-                QtWidgets.QMessageBox.warning(self.parent, 'Error',
-                                              'Could not import the data.'
-                                              'Currently only ASTER'
-                                              'is supported.',
-                                              QtWidgets.QMessageBox.Ok)
-            else:
-                QtWidgets.QMessageBox.warning(self.parent, 'Error',
-                                              'Could not import the data.',
-                                              QtWidgets.QMessageBox.Ok)
-            return False
+        if not nodialog:
+            tmp = self.exec_()
 
-        output_type = 'Raster'
-        self.outdata[output_type] = dat
+            if tmp != 1:
+                return False
+
+        self.acceptall()
 
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
@@ -221,59 +147,77 @@
 
         Returns
         -------
         chk : bool
             A check to see if settings was successfully run.
 
         """
-        self.ifile = projdata['ifile']
-        self.filt = projdata['filt']
-        self.extscene = projdata['extscene']
-
-        chk = self.settings(True)
+        self.dataid.setCurrentText(projdata['band'])
+        self.continuation.setCurrenText(projdata['ctype'])
+        self.dsb_height.setValue(projdata['height'])
 
-        return chk
+        return False
 
     def saveproj(self):
         """
         Save project data from class.
 
         Returns
         -------
         projdata : dictionary
             Project data to be saved to JSON project file.
 
         """
         projdata = {}
 
-        projdata['ifile'] = self.ifile
-        projdata['filt'] = self.filt
-        projdata['extscene'] = self.extscene
+        projdata['band'] = self.dataid.currentText()
+        projdata['ctype'] = self.continuation.currentText()
+        projdata['height'] = self.dsb_height.value()
 
         return projdata
 
+    def acceptall(self):
+        """
+        Accept option.
 
-class ImportBatch(BasicModule):
-    """
-    Batch Import Data Interface.
+        Updates self.outdata, which is used as input to other modules.
 
-    This does not actually import data, but rather defines a list of datasets
-    to be used by other routines.
+        Returns
+        -------
+        None.
 
-    Attributes
-    ----------
-    idir : str
-        Input directory.
+        """
+        h = self.dsb_height.value()
+        ctype = self.continuation.currentText()
+
+        # Get data
+        for i in self.indata['Raster']:
+            if i.dataid == self.dataid.currentText():
+                data = i
+                break
+
+        if ctype == 'Downward':
+            dat = taylorcont(data, h)
+        else:
+            dat = fftcont(data, h)
+
+        self.outdata['Raster'] = [dat]
+
+
+class DataCut(BasicModule):
+    """
+    Cut Data using shapefiles.
+
+    This class cuts raster datasets using a boundary defined by a polygon
+    shapefile.
     """
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
-        self.idir = ''
-
     def settings(self, nodialog=False):
         """
         Entry point into item.
 
         Parameters
         ----------
         nodialog : bool, optional
@@ -281,55 +225,33 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
-        if not nodialog or self.idir == '':
-            self.idir = QtWidgets.QFileDialog.getExistingDirectory(
-                self.parent, 'Select Directory')
-            if self.idir == '':
+        if 'Raster' in self.indata:
+            data = self.indata['Raster']
+        else:
+            self.showlog('No raster data')
+            return False
+
+        if not nodialog:
+            self.ifile, _ = QtWidgets.QFileDialog.getOpenFileName(
+                self.parent, 'Open Shape File', '.', 'Shape file (*.shp)')
+            if self.ifile == '':
                 return False
-        os.chdir(self.idir)
 
-        zipdat = glob.glob(self.idir+'//AST*.zip')
-        hdfdat = glob.glob(self.idir+'//AST*.hdf')
-        targzdat = glob.glob(self.idir+'//L*.tar*')
-        mtldat = glob.glob(self.idir+'//L*MTL.txt')
-        rasterdat = []
-        for ftype in ['*.tif', '*.hdr', '*.img', '*.ers']:
-            rasterdat += glob.glob(os.path.join(self.idir, ftype))
-
-        sendat = glob.glob(self.idir+'//S2?_*.zip')
-        sendir = [f.path for f in os.scandir(self.idir) if f.is_dir() and
-                  'SAFE' in f.path]
-        for i in sendir:
-            sendat.extend(glob.glob(i+'//MTD*.xml'))
-
-        if (not hdfdat and not zipdat and not targzdat and not mtldat and not
-                sendat and not rasterdat):
-            QtWidgets.QMessageBox.warning(self.parent, 'Error',
-                                          'No valid files in the directory.',
-                                          QtWidgets.QMessageBox.Ok)
-            return False
+        os.chdir(os.path.dirname(self.ifile))
+        data = cut_raster(data, self.ifile, showlog=self.showlog)
 
-        dat = []
-        for i in hdfdat:
-            if 'met' not in i:
-                dat.append(i)
-
-        dat.extend(mtldat)
-        dat.extend(targzdat)
-        dat.extend(zipdat)
-        dat.extend(sendat)
-        dat.extend(rasterdat)
+        if data is None:
+            return False
 
-        output_type = 'RasterFileList'
-        self.outdata[output_type] = dat
+        self.outdata['Raster'] = data
 
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
@@ -340,120 +262,122 @@
 
         Returns
         -------
         chk : bool
             A check to see if settings was successfully run.
 
         """
-        self.idir = projdata['idir']
-
-        chk = self.settings(True)
+        self.ifile = projdata['shapefile']
 
-        return chk
+        return False
 
     def saveproj(self):
         """
         Save project data from class.
 
         Returns
         -------
         projdata : dictionary
             Project data to be saved to JSON project file.
 
         """
         projdata = {}
 
-        projdata['idir'] = self.idir
+        projdata['shapefile'] = self.ifile
 
         return projdata
 
 
-class ImportSentinel5P(BasicModule):
-    """Import Sentinel 5P data to shapefile."""
+class DataLayerStack(BasicModule):
+    """
+    Data Layer Stack.
+
+    This class merges datasets which have different rows and columns. It
+    resamples them so that they have the same rows and columns.
+    """
 
     def __init__(self, parent=None):
         super().__init__(parent)
-
-        self.sfile = ''
-        self.filt = ''
-        self.indx = 0
-
-        self.subdata = QtWidgets.QComboBox()
-        self.lonmin = QtWidgets.QLineEdit('16')
-        self.lonmax = QtWidgets.QLineEdit('34')
-        self.latmin = QtWidgets.QLineEdit('-35')
-        self.latmax = QtWidgets.QLineEdit('-21')
-        self.qathres = QtWidgets.QLineEdit('50')
-        self.cclip = QtWidgets.QRadioButton('Clip using coordinates')
-        self.sclip = QtWidgets.QRadioButton('Clip using shapefile')
-        self.shpfile = QtWidgets.QLineEdit(self.sfile)
-        self.label_sfile = QtWidgets.QPushButton('Load shapefile')
-        self.label_lonmin = QtWidgets.QLabel('Minimum Longitude:')
-        self.label_lonmax = QtWidgets.QLabel('Maximum Longitude:')
-        self.label_latmin = QtWidgets.QLabel('Minimum Latitude:')
-        self.label_latmax = QtWidgets.QLabel('Maximum Latitude:')
+        self.dxy = None
+        self.piter = parent.pbar.iter
+        self.cmask = QtWidgets.QCheckBox('Common mask for all bands')
+
+        self.dsb_dxy = QtWidgets.QDoubleSpinBox()
+        self.label_rows = QtWidgets.QLabel('Rows: 0')
+        self.label_cols = QtWidgets.QLabel('Columns: 0')
 
         self.setupui()
 
     def setupui(self):
         """
         Set up UI.
 
         Returns
         -------
         None.
 
         """
         gridlayout_main = QtWidgets.QGridLayout(self)
         buttonbox = QtWidgets.QDialogButtonBox()
-        helpdocs = menu_default.HelpButton('pygmi.rsense.iodefs.importsentinel5p')
-        label_subdata = QtWidgets.QLabel('Product:')
-        label_qathres = QtWidgets.QLabel('QA Threshold (0-100):')
-
+        helpdocs = menu_default.HelpButton('pygmi.raster.dataprep.'
+                                           'datalayerstack')
+        label_dxy = QtWidgets.QLabel('Cell Size:')
+
+        self.dsb_dxy.setMaximum(9999999999.0)
+        self.dsb_dxy.setMinimum(0.00001)
+        self.dsb_dxy.setDecimals(5)
+        self.dsb_dxy.setValue(40.)
         buttonbox.setOrientation(QtCore.Qt.Horizontal)
         buttonbox.setCenterButtons(True)
         buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
-        self.cclip.setChecked(True)
-        self.label_sfile.hide()
-        self.shpfile.hide()
 
-        self.setWindowTitle(r'Import Sentinel-5P Data')
+        self.cmask.setChecked(True)
 
-        gridlayout_main.addWidget(label_subdata, 0, 0, 1, 1)
-        gridlayout_main.addWidget(self.subdata, 0, 1, 1, 1)
+        self.setWindowTitle('Dataset Layer Stack and Resample')
 
-        gridlayout_main.addWidget(self.cclip, 1, 0, 1, 2)
-        gridlayout_main.addWidget(self.sclip, 2, 0, 1, 2)
+        gridlayout_main.addWidget(label_dxy, 0, 0, 1, 1)
+        gridlayout_main.addWidget(self.dsb_dxy, 0, 1, 1, 1)
+        gridlayout_main.addWidget(self.label_rows, 1, 0, 1, 2)
+        gridlayout_main.addWidget(self.label_cols, 2, 0, 1, 2)
+        gridlayout_main.addWidget(self.cmask, 3, 0, 1, 2)
+        gridlayout_main.addWidget(helpdocs, 4, 0, 1, 1)
+        gridlayout_main.addWidget(buttonbox, 4, 1, 1, 1)
 
-        gridlayout_main.addWidget(self.label_lonmin, 3, 0, 1, 1)
-        gridlayout_main.addWidget(self.lonmin, 3, 1, 1, 1)
+        buttonbox.accepted.connect(self.accept)
+        buttonbox.rejected.connect(self.reject)
+        self.dsb_dxy.valueChanged.connect(self.dxy_change)
 
-        gridlayout_main.addWidget(self.label_lonmax, 4, 0, 1, 1)
-        gridlayout_main.addWidget(self.lonmax, 4, 1, 1, 1)
+    def dxy_change(self):
+        """
+        Update dxy.
 
-        gridlayout_main.addWidget(self.label_latmin, 5, 0, 1, 1)
-        gridlayout_main.addWidget(self.latmin, 5, 1, 1, 1)
+        This is the size of a grid cell in the x and y directions.
 
-        gridlayout_main.addWidget(self.label_latmax, 6, 0, 1, 1)
-        gridlayout_main.addWidget(self.latmax, 6, 1, 1, 1)
+        Returns
+        -------
+        None.
 
-        gridlayout_main.addWidget(self.label_sfile, 7, 0, 1, 1)
-        gridlayout_main.addWidget(self.shpfile, 7, 1, 1, 1)
+        """
+        data = self.indata['Raster'][0]
+        dxy = self.dsb_dxy.value()
 
-        gridlayout_main.addWidget(label_qathres, 8, 0, 1, 1)
-        gridlayout_main.addWidget(self.qathres, 8, 1, 1, 1)
+        xmin0, xmax0, ymin0, ymax0 = data.extent
 
-        gridlayout_main.addWidget(helpdocs, 10, 0, 1, 1)
-        gridlayout_main.addWidget(buttonbox, 10, 1, 1, 3)
+        for data in self.indata['Raster']:
+            xmin, xmax, ymin, ymax = data.extent
+            xmin = min(xmin, xmin0)
+            xmax = max(xmax, xmax0)
+            ymin = min(ymin, ymin0)
+            ymax = max(ymax, ymax0)
 
-        buttonbox.accepted.connect(self.accept)
-        buttonbox.rejected.connect(self.reject)
-        self.cclip.clicked.connect(self.clipchoice)
-        self.sclip.clicked.connect(self.clipchoice)
-        self.label_sfile.clicked.connect(self.loadshp)
+        cols = int((xmax - xmin)/dxy)
+        rows = int((ymax - ymin)/dxy)
+
+        self.label_rows.setText('Rows: '+str(rows))
+        self.label_cols.setText('Columns: '+str(cols))
 
     def settings(self, nodialog=False):
         """
         Entry point into item.
 
         Parameters
         ----------
@@ -462,295 +386,839 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
+        if 'RasterFileList' in self.indata:
+            from pygmi.rsense.iodefs import get_data
+
+            ifiles = self.indata['RasterFileList']
+            self.showlog('Warning: Layer stacking a file list assumes '
+                         'all datasets overlap in the same area')
+            self.indata['Raster'] = []
+            for ifile in ifiles:
+                self.showlog('Processing '+os.path.basename(ifile))
+                dat = get_data(ifile, piter=self.piter,
+                               showlog=self.showlog)
+                for i in dat:
+                    i.data = i.data.astype(np.float32)
+                self.indata['Raster'] += dat
+
+        if 'Raster' not in self.indata:
+            self.showlog('No Raster Data.')
+            return False
+
         if not nodialog:
-            ext = ('Sentinel-5P (*.nc)')
+            data = self.indata['Raster'][0]
 
-            self.ifile, self.filt = QtWidgets.QFileDialog.getOpenFileName(
-                self.parent, 'Open File', '.', ext)
-            if self.ifile == '':
-                return False
+            if self.dxy is None:
+                self.dxy = min(data.xdim, data.ydim)
+                for data in self.indata['Raster']:
+                    self.dxy = min(self.dxy, data.xdim, data.ydim)
 
-        os.chdir(os.path.dirname(self.ifile))
+            self.dsb_dxy.setValue(self.dxy)
+            self.dxy_change()
+
+            tmp = self.exec_()
+            if tmp != 1:
+                return False
 
-        meta = self.get_5P_meta()
+        self.acceptall()
 
-        if meta is None:
+        if self.outdata['Raster'] is None:
+            self.outdata = {}
             return False
 
-        tmp = []
-        for i in meta:
-            if i in ['latitude', 'longitude', 'qa_value']:
-                continue
-            tmp.append(i)
+        return True
 
-        self.subdata.clear()
-        self.subdata.addItems(tmp)
-        self.subdata.setCurrentIndex(self.indx)
+    def loadproj(self, projdata):
+        """
+        Load project data into class.
 
-        if not nodialog:
-            tmp = self.exec_()
+        Parameters
+        ----------
+        projdata : dictionary
+            Project data loaded from JSON project file.
 
-            if tmp != 1:
-                return tmp
+        Returns
+        -------
+        chk : bool
+            A check to see if settings was successfully run.
 
-        try:
-            _ = float(self.lonmin.text())
-            _ = float(self.latmin.text())
-            _ = float(self.lonmax.text())
-            _ = float(self.latmax.text())
-        except ValueError:
-            self.showprocesslog('Value error - abandoning import')
-            return False
+        """
+        self.dxy = projdata['dxy']
+        self.cmask.setChecked(projdata['cmask'])
 
-        gdf = self.get_5P_data(meta)
+        return False
 
-        if gdf is None:
-            return False
+    def saveproj(self):
+        """
+        Save project data from class.
 
-        dat = {gdf.geom_type.iloc[0]: gdf}
-        self.outdata['Vector'] = dat
+        Returns
+        -------
+        projdata : dictionary
+            Project data to be saved to JSON project file.
 
-        return True
+        """
+        projdata = {}
+
+        projdata['dxy'] = self.dsb_dxy.value()
+        projdata['cmask'] = self.cmask.isChecked()
 
-    def clipchoice(self):
+        return projdata
+
+    def acceptall(self):
         """
-        Choose clip style.
+        Accept option.
+
+        Updates self.outdata, which is used as input to other modules.
 
         Returns
         -------
         None.
 
         """
-        if self.cclip.isChecked():
-            self.label_sfile.hide()
-            self.shpfile.hide()
-            self.lonmin.show()
-            self.lonmax.show()
-            self.latmin.show()
-            self.latmax.show()
-            self.label_lonmin.show()
-            self.label_lonmax.show()
-            self.label_latmin.show()
-            self.label_latmax.show()
-        else:
-            self.lonmin.hide()
-            self.lonmax.hide()
-            self.latmin.hide()
-            self.latmax.hide()
-            self.label_lonmin.hide()
-            self.label_lonmax.hide()
-            self.label_latmin.hide()
-            self.label_latmax.hide()
-            self.label_sfile.show()
-            self.shpfile.show()
+        dxy = self.dsb_dxy.value()
+        self.dxy = dxy
+        dat = lstack(self.indata['Raster'], self.piter, dxy,
+                     showlog=self.showlog,
+                     commonmask=self.cmask.isChecked())
+        self.outdata['Raster'] = dat
 
-    def loadproj(self, projdata):
+
+class DataMerge(BasicModule):
+    """
+    Data Merge.
+
+    This class merges datasets which have different rows and columns. It
+    resamples them so that they have the same rows and columns.
+    """
+
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        self.idir = None
+        self.method = merge_median
+        self.rb_first = QtWidgets.QRadioButton('First - copy first file over '
+                                               'last file at overlap.')
+        self.rb_last = QtWidgets.QRadioButton('Last - copy last file over '
+                                              'first file at overlap.')
+        self.rb_min = QtWidgets.QRadioButton('Min - copy pixel wise minimum '
+                                             'at overlap.')
+        self.rb_max = QtWidgets.QRadioButton('Max - copy pixel wise maximum '
+                                             'at overlap.')
+        self.rb_median = QtWidgets.QRadioButton('Median - shift last file to '
+                                                'median '
+                                                'overlap value and copy over '
+                                                'first file at overlap.')
+
+        self.idirlist = QtWidgets.QLineEdit('')
+        self.sfile = QtWidgets.QLineEdit('')
+        self.files_diff = QtWidgets.QCheckBox('Mosaic by band labels, '
+                                              'since band order may differ, '
+                                              'or input files have different '
+                                              'numbers of bands or '
+                                              'nodata values.')
+        self.shift_to_median = QtWidgets.QCheckBox('Shift bands to median '
+                                                   'value before mosaic. May '
+                                                   'allow for cleaner mosaic '
+                                                   'if datasets are offset.')
+
+        self.bands_to_files = QtWidgets.QCheckBox('Save each band separately '
+                                                  'in a "mosaic" '
+                                                  'subdirectory.')
+        self.forcetype = None
+        self.singleband = False
+        self.setupui()
+
+    def setupui(self):
         """
-        Load project data into class.
+        Set up UI.
 
-        Parameters
-        ----------
-        projdata : dictionary
-            Project data loaded from JSON project file.
+        Returns
+        -------
+        None.
+
+        """
+        gridlayout_main = QtWidgets.QGridLayout(self)
+        buttonbox = QtWidgets.QDialogButtonBox()
+        helpdocs = menu_default.HelpButton('pygmi.raster.dataprep.datamerge')
+        pb_idirlist = QtWidgets.QPushButton('Batch Directory')
+        pb_sfile = QtWidgets.QPushButton('Shapefile for boundary (optional)')
+
+        self.files_diff.setChecked(True)
+        self.shift_to_median.setChecked(False)
+        self.rb_median.setChecked(True)
+
+        buttonbox.setOrientation(QtCore.Qt.Horizontal)
+        buttonbox.setCenterButtons(True)
+        buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
+
+        self.setWindowTitle('Dataset Mosaic')
+
+        gb_merge_method = QtWidgets.QGroupBox('Mosiac method')
+        gl_merge_method = QtWidgets.QVBoxLayout(gb_merge_method)
+
+        gl_merge_method.addWidget(self.rb_median)
+        gl_merge_method.addWidget(self.rb_first)
+        gl_merge_method.addWidget(self.rb_last)
+        gl_merge_method.addWidget(self.rb_min)
+        gl_merge_method.addWidget(self.rb_max)
+
+        gridlayout_main.addWidget(pb_idirlist, 1, 0, 1, 1)
+        gridlayout_main.addWidget(self.idirlist, 1, 1, 1, 1)
+        gridlayout_main.addWidget(pb_sfile, 2, 0, 1, 1)
+        gridlayout_main.addWidget(self.sfile, 2, 1, 1, 1)
+        gridlayout_main.addWidget(self.files_diff, 3, 0, 1, 2)
+        gridlayout_main.addWidget(self.shift_to_median, 4, 0, 1, 2)
+        gridlayout_main.addWidget(gb_merge_method, 5, 0, 1, 2)
+        gridlayout_main.addWidget(self.bands_to_files, 6, 0, 1, 2)
+        gridlayout_main.addWidget(helpdocs, 7, 0, 1, 1)
+        gridlayout_main.addWidget(buttonbox, 7, 1, 1, 1)
+
+        buttonbox.accepted.connect(self.accept)
+        buttonbox.rejected.connect(self.reject)
+        pb_idirlist.pressed.connect(self.get_idir)
+        pb_sfile.pressed.connect(self.get_sfile)
+        self.shift_to_median.stateChanged.connect(self.shiftchanged)
+        self.files_diff.stateChanged.connect(self.filesdiffchanged)
+        self.rb_first.clicked.connect(self.method_change)
+        self.rb_last.clicked.connect(self.method_change)
+        self.rb_min.clicked.connect(self.method_change)
+        self.rb_max.clicked.connect(self.method_change)
+        self.rb_median.clicked.connect(self.method_change)
+
+    def method_change(self):
+        """
+        Change method.
 
         Returns
         -------
-        chk : bool
-            A check to see if settings was successfully run.
+        None.
 
         """
-        self.ifile = projdata['ifile']
-        self.filt = projdata['filt']
+        if self.rb_first.isChecked():
+            self.method = 'first'
+        if self.rb_last.isChecked():
+            self.method = 'last'
+        if self.rb_min.isChecked():
+            self.method = merge_min
+        if self.rb_max.isChecked():
+            self.method = merge_max
+        if self.rb_median.isChecked():
+            self.method = merge_median
 
-        chk = self.settings(True)
+    def shiftchanged(self):
+        """
+        Shift mean clicked.
 
-        return chk
+        Returns
+        -------
+        None.
+
+        """
+        if self.shift_to_median.isChecked():
+            self.files_diff.setChecked(True)
+
+    def filesdiffchanged(self):
+        """
+        Files different clicked.
+
+        Returns
+        -------
+        None.
+
+        """
+        if not self.files_diff.isChecked():
+            self.shift_to_median.setChecked(False)
+            self.bands_to_files.hide()
+        else:
+            self.bands_to_files.show()
+
+    def get_idir(self):
+        """
+        Get the input directory.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.idir = QtWidgets.QFileDialog.getExistingDirectory(
+             self.parent, 'Select Directory')
 
-    def loadshp(self):
+        self.idirlist.setText(self.idir)
+
+        if self.idir == '':
+            self.idir = None
+
+    def get_sfile(self):
         """
-        Load shapefile filename.
+        Get the input shapefile.
 
         Returns
         -------
         None.
 
         """
-        ext = ('Shapefile (*.shp)')
+        ext = ('ESRI Shapefile (*.shp);;')
 
-        self.sfile, _ = QtWidgets.QFileDialog.getOpenFileName(
+        sfile, _ = QtWidgets.QFileDialog.getOpenFileName(
             self.parent, 'Open File', '.', ext)
 
-        self.shpfile.setText(self.sfile)
+        if not sfile:
+            return False
+
+        self.sfile.setText(sfile)
+
+        return True
+
+    def settings(self, nodialog=False):
+        """
+        Entry point into item.
+
+        Parameters
+        ----------
+        nodialog : bool, optional
+            Run settings without a dialog. The default is False.
+
+        Returns
+        -------
+        bool
+            True if successful, False otherwise.
+
+        """
+        if not nodialog:
+            tmp = self.exec_()
+            if tmp != 1:
+                return False
+
+        tmp = self.acceptall()
+
+        return tmp
+
+    def loadproj(self, projdata):
+        """
+        Load project data into class.
+
+        Parameters
+        ----------
+        projdata : dictionary
+            Project data loaded from JSON project file.
+
+        Returns
+        -------
+        chk : bool
+            A check to see if settings was successfully run.
+
+        """
+        self.idir = projdata['idir']
+        self.idirlist.setText(self.idir)
+        self.files_diff.setChecked(projdata['files_diff'])
+        self.shift_to_median.setChecked(projdata['mean_shift'])
+
+        return False
 
     def saveproj(self):
         """
         Save project data from class.
 
         Returns
         -------
         projdata : dictionary
             Project data to be saved to JSON project file.
 
         """
         projdata = {}
 
-        projdata['ifile'] = self.ifile
-        projdata['filt'] = self.filt
+        projdata['idir'] = self.idir
+        projdata['files_diff'] = self.files_diff.isChecked()
+        projdata['mean_shift'] = self.shift_to_median.isChecked()
 
         return projdata
 
-    def get_5P_meta(self):
+    def acceptall(self):
         """
-        Get 5P metadata.
+        Accept option.
+
+        Updates self.outdata, which is used as input to other modules.
 
         Returns
         -------
-        meta : Dictionary
-            Dictionary containing metadata.
+        bool
+            Success of routine.
 
         """
-        with rasterio.open(self.ifile) as dataset:
-            subdata = dataset.subdatasets
+        if self.files_diff.isChecked():
+            tmp = self.merge_different()
+        else:
+            tmp = self.merge_same()
 
-        meta = {}
-        for i in subdata:
-            tmp = i.split(':')
-            if 'SUPPORT_DATA' in i:
-                continue
-            if 'METADATA' in i:
-                continue
-            if 'time_utc' in i:
-                continue
-            if 'delta_time' in i:
-                continue
-            # if 'qa_value' in i:
-            #     continue
-            if 'precision' in i:
+        return tmp
+
+    def merge_different(self):
+        """
+        Merge files with different numbers of bands and/or band order.
+
+        This uses more memory, but is flexible.
+
+        Returns
+        -------
+        bool
+            Success of routine.
+
+        """
+        # The next line is only to avoid circular dependancies with merge
+        # function.
+
+        from pygmi.raster.iodefs import get_raster, export_raster
+
+        indata = []
+        if 'Raster' in self.indata:
+            for i in self.indata['Raster']:
+                indata.append(i)
+
+        if self.idir is not None:
+            ifiles = []
+            for ftype in ['*.tif', '*.hdr', '*.img', '*.ers']:
+                ifiles += glob.glob(os.path.join(self.idir, ftype))
+
+            if not ifiles:
+                self.showlog('No input files in that directory')
+                return False
+
+            for ifile in self.piter(ifiles):
+                indata += get_raster(ifile, piter=iter, metaonly=True)
+
+        if indata is None:
+            self.showlog('No input datasets')
+            return False
+
+        # Get projection information
+        wkt = []
+        crs = []
+        for i in indata:
+            if i.crs is None:
+                self.showlog(f'{i.dataid} has no projection. '
+                             'Please assign one.')
+                return False
+
+            wkt.append(i.crs.to_wkt())
+            crs.append(i.crs)
+            nodata = i.nodata
+
+        wkt, iwkt, numwkt = np.unique(wkt, return_index=True,
+                                      return_counts=True)
+        if len(wkt) > 1:
+            self.showlog('Error: Mismatched input projections. '
+                         'Selecting most common projection')
+
+            crs = crs[iwkt[numwkt == numwkt.max()][0]]
+        else:
+            crs = indata[0].crs
+
+        bounds = get_shape_bounds(self.sfile.text(), crs, self.showlog)
+
+        # Start Merge
+        bandlist = []
+        for i in indata:
+            bandlist.append(i.dataid)
+
+        bandlist = list(set(bandlist))
+
+        if self.singleband is True:
+            bandlist = ['Band_1']
+
+        outdat = []
+        for dataid in bandlist:
+            self.showlog('Extracting '+dataid+'...')
+
+            if self.bands_to_files.isChecked():
+                odir = os.path.join(self.idir, 'mosaic')
+                os.makedirs(odir, exist_ok=True)
+                ofile = dataid+'.tif'
+                ofile = ofile.replace(' ', '_')
+                ofile = ofile.replace(',', '_')
+                ofile = ofile.replace('*', 'mult')
+                ofile = os.path.join(odir, ofile)
+
+                if os.path.exists(ofile):
+                    self.showlog('Output file exists, skipping.')
+                    continue
+
+            ifiles = []
+            allmval = []
+            for i in self.piter(indata):
+                if i.dataid != dataid and self.singleband is False:
+                    continue
+                metadata = i.metadata
+
+                i2 = get_raster(i.filename, piter=iter, dataid=i.dataid)
+
+                if i2 is None:
+                    continue
+
+                i2 = i2[0]
+
+                if i2.crs != crs:
+                    src_height, src_width = i2.data.shape
+
+                    transform, width, height = calculate_default_transform(
+                        i2.crs, crs, src_width, src_height, *i2.bounds)
+
+                    i2 = data_reproject(i2, crs, transform, height, width)
+
+                if self.forcetype is not None:
+                    i2.data = i2.data.astype(self.forcetype)
+
+                if self.shift_to_median.isChecked():
+                    mval = np.ma.median(i2.data)
+                else:
+                    mval = 0
+                allmval.append(mval)
+
+                if self.singleband is True:
+                    i2.dataid = 'Band_1'
+
+                trans = rasterio.transform.from_origin(i2.extent[0],
+                                                       i2.extent[3],
+                                                       i2.xdim, i2.ydim)
+
+                tmpfile = os.path.join(tempfile.gettempdir(),
+                                       os.path.basename(i.filename))
+
+                tmpid = i2.dataid
+                tmpid = tmpid.replace(' ', '_')
+                tmpid = tmpid.replace(',', '_')
+                tmpid = tmpid.replace('*', 'mult')
+                tmpid = tmpid.replace(r'/', 'div')
+
+                tmpfile = tmpfile[:-4]+'_'+tmpid+'.tif'
+
+                raster = rasterio.open(tmpfile, 'w', driver='GTiff',
+                                       height=i2.data.shape[0],
+                                       width=i2.data.shape[1], count=1,
+                                       dtype=i2.data.dtype,
+                                       transform=trans)
+
+                if np.issubdtype(i2.data.dtype, np.floating):
+                    nodata = 1.0e+20
+                else:
+                    nodata = -99999
+
+                tmpdat = i2.data-mval
+                tmpdat = tmpdat.filled(nodata)
+                tmpdat = np.ma.masked_equal(tmpdat, nodata)
+
+                raster.write(tmpdat, 1)
+                raster.write_mask(~np.ma.getmaskarray(i2.data))
+
+                raster.close()
+                ifiles.append(tmpfile)
+                del i2
+
+            if len(ifiles) < 2:
+                self.showlog('Too few bands of name '+dataid)
                 continue
 
-            tmp = tmp[-1].replace('//PRODUCT/', '')
-            tmp = tmp.replace('/PRODUCT/', '')
-            tmp = tmp.replace('/', '')
+            self.showlog('Mosaicing '+dataid+'...')
+            # print(ifiles)
+
+            with rasterio.Env(CPL_DEBUG=True):
+                mosaic, otrans = rasterio.merge.merge(ifiles, nodata=nodata,
+                                                      method=self.method,
+                                                      bounds=bounds)
+
+            for j in ifiles:
+                if os.path.exists(j):
+                    os.remove(j)
+                if os.path.exists(j+'.msk'):
+                    os.remove(j+'.msk')
+
+            mosaic = mosaic.squeeze()
+            mosaic = np.ma.masked_equal(mosaic, nodata)
+            mosaic = mosaic + np.median(allmval)
+            outdat.append(numpy_to_pygmi(mosaic, dataid=dataid))
+            outdat[-1].set_transform(transform=otrans)
+            outdat[-1].crs = crs
+            outdat[-1].nodata = nodata
+            outdat[-1].metadata = metadata
+
+            if self.bands_to_files.isChecked():
+                export_raster(ofile, outdat, 'GTiff', compression='ZSTD',
+                              showlog=self.showlog)
+
+                del outdat
+                del mosaic
+                outdat = []
 
-            meta[tmp] = i
+        if bounds is not None:
+            outdat = cut_raster(outdat, self.sfile.text(), deepcopy=False)
 
-        dataset = None
+        self.outdata['Raster'] = outdat
 
-        return meta
+        return True
 
-    def get_5P_data(self, meta):
+    def merge_same(self):
         """
-        Get 5P data.
+        Mosaic files with same numbers of bands and band order.
 
-        Parameters
-        ----------
-        meta : Dictionary
-            Dictionary containing metadata.
+        This uses much less memory, but is less flexible.
 
         Returns
         -------
-        gdf : DataFrame
-            geopandas dataframe.
+        bool
+            Success of routine.
 
         """
-        try:
-            thres = int(self.qathres.text())
-        except ValueError:
-            self.showprocesslog('Threshold text not an integer')
-            return None
+        ifiles = []
+        if 'Raster' in self.indata:
+            for i in self.indata['Raster']:
+                ifiles.append(i.filename)
 
-        with rasterio.open(meta['latitude']) as dataset:
-            lats = dataset.read(1)
+        if self.idir is not None:
+            for ftype in ['*.tif', '*.hdr', '*.img', '*.ers']:
+                ifiles += glob.glob(os.path.join(self.idir, ftype))
 
-        with rasterio.open(meta['longitude']) as dataset:
-            lons = dataset.read(1)
+        if not ifiles:
+            self.showlog('No input datasets')
+            return False
 
-        with rasterio.open(meta['qa_value']) as dataset:
-            qaval = dataset.read(1)
+        for i, ifile in enumerate(ifiles):
+            if ifile[-3:] == 'hdr':
+                ifile = ifile[:-4]
+                if os.path.exists(ifile+'.dat'):
+                    ifiles[i] = ifile+'.dat'
+                elif os.path.exists(ifile+'.raw'):
+                    ifiles[i] = ifile+'.raw'
+                elif os.path.exists(ifile+'.img'):
+                    ifiles[i] = ifile+'.img'
+                elif not os.path.exists(ifile):
+                    return False
+
+        # Get projection information
+        wkt = []
+        nodata = []
+        for ifile in ifiles:
+            with rasterio.open(ifile) as dataset:
+                if dataset.crs is None:
+                    self.showlog(f'{ifile} has no projection. '
+                                 'Please assign one.')
+                    return False
+                wkt.append(dataset.crs.wkt)
+                crs = dataset.crs
+                nodata.append(dataset.nodata)
+
+        wkt = list(set(wkt))
+        if len(wkt) > 1:
+            self.showlog('Error: Mismatched input projections')
+            return False
 
-        with rasterio.open(meta['longitude']) as dataset:
-            lons = dataset.read(1)
+        nodata = list(set(nodata))
+        if len(nodata) > 1:
+            self.showlog('Error: Mismatched nodata values. Try using merge '
+                         'by band labels merge option. Please confirm bands '
+                         'to be merged have the same label.')
+            return False
 
-        del meta['latitude']
-        del meta['longitude']
+        # Get band names and nodata
+        with rasterio.open(ifiles[0]) as dataset:
+            bnames = dataset.descriptions
+            if None in bnames:
+                bnames = ['Band '+str(i) for i in dataset.indexes]
+            nodata = dataset.nodata
+
+        # Start Merge
+        mosaic, otrans = rasterio.merge.merge(ifiles, nodata=nodata,
+                                              method=self.method)
+        mosaic = np.ma.masked_equal(mosaic, nodata)
+
+        outdat = []
+        for i, dataid in enumerate(bnames):
+            outdat.append(numpy_to_pygmi(mosaic[i], dataid=dataid))
+            outdat[-1].set_transform(transform=otrans)
+            outdat[-1].crs = crs
+            outdat[-1].nodata = nodata
 
-        if lats is None:
-            self.showprocesslog('No Latitudes in dataset')
-            return None
+        self.outdata['Raster'] = outdat
 
-        lats = lats.flatten()
-        lons = lons.flatten()
-        pnts = np.transpose([lons, lats])
-
-        if self.cclip.isChecked():
-            lonmin = float(self.lonmin.text())
-            latmin = float(self.latmin.text())
-            lonmax = float(self.lonmax.text())
-            latmax = float(self.latmax.text())
-        else:
-            shp = gpd.read_file(self.sfile)
-            shp = shp.to_crs(4326)
+        return True
 
-            lonmin = float(shp.bounds.minx)
-            lonmax = float(shp.bounds.maxx)
-            latmin = float(shp.bounds.miny)
-            latmax = float(shp.bounds.maxy)
 
-        mask = ((lats > latmin) & (lats < latmax) & (lons < lonmax) &
-                (lons > lonmin))
+class DataReproj(BasicModule):
+    """
+    Reprojections.
 
-        idfile = self.subdata.currentText()
+    This class reprojects datasets using the rasterio routines.
+    """
 
-        dfile = meta[idfile]
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        self.orig_wkt = None
+        self.targ_wkt = None
 
-        with rasterio.open(dfile) as dataset:
-            dat = dataset.read(1)
+        self.groupboxb = QtWidgets.QGroupBox()
+        self.combobox_inp_epsg = QtWidgets.QComboBox()
+        self.inp_epsg_info = QtWidgets.QLabel(wordWrap=True)
+        self.groupbox2b = QtWidgets.QGroupBox()
+        self.combobox_out_epsg = QtWidgets.QComboBox()
+        self.out_epsg_info = QtWidgets.QLabel()
+        self.in_proj = GroupProj('Input Projection')
+        self.out_proj = GroupProj('Output Projection')
 
-        dat1 = dat.flatten()
-        qaval1 = qaval.flatten()
+        self.setupui()
 
-        if mask.shape != dat1.shape:
-            return None
+    def setupui(self):
+        """
+        Set up UI.
 
-        dat1 = dat1[mask]
-        pnts1 = pnts[mask]
-        qaval1 = qaval1[mask]
+        Returns
+        -------
+        None.
 
-        qaval1 = qaval1[dat1 != 9.96921e+36]
-        pnts1 = pnts1[dat1 != 9.96921e+36]
-        dat1 = dat1[dat1 != 9.96921e+36]
+        """
+        gridlayout_main = QtWidgets.QGridLayout(self)
+        buttonbox = QtWidgets.QDialogButtonBox()
+        helpdocs = menu_default.HelpButton('pygmi.raster.dataprep.datareproj')
 
-        pnts1 = pnts1[qaval1 >= thres]
-        dat1 = dat1[qaval1 >= thres]
+        buttonbox.setOrientation(QtCore.Qt.Horizontal)
+        buttonbox.setCenterButtons(True)
+        buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
 
-        df = pd.DataFrame({'lon': pnts1[:, 0], 'lat': pnts1[:, 1]})
-        df['data'] = dat1
+        self.setWindowTitle('Dataset Reprojection')
 
-        gdf = GeoDataFrame(df.drop(['lon', 'lat'], axis=1),
-                           geometry=[Point(xy) for xy in zip(df.lon, df.lat)])
+        gridlayout_main.addWidget(self.in_proj, 0, 0, 1, 1)
+        gridlayout_main.addWidget(self.out_proj, 0, 1, 1, 1)
+        gridlayout_main.addWidget(helpdocs, 1, 0, 1, 1)
+        gridlayout_main.addWidget(buttonbox, 1, 1, 1, 1)
 
-        gdf = gdf.set_crs("EPSG:4326")
+        buttonbox.accepted.connect(self.accept)
+        buttonbox.rejected.connect(self.reject)
 
-        if self.sclip.isChecked():
-            gdf = gdf.clip(shp)
+    def acceptall(self):
+        """
+        Accept option.
 
-        if gdf.size == 0:
-            self.showprocesslog(idfile, 'is empty.')
-            return None
+        Updates self.outdata, which is used as input to other modules.
+
+        Returns
+        -------
+        None.
+
+        """
+        if self.in_proj.wkt == 'Unknown' or self.out_proj.wkt == 'Unknown':
+            self.showlog('Unknown Projection. Could not reproject')
+            return
+
+        if self.in_proj.wkt == '' or self.out_proj.wkt == '':
+            self.showlog('Unknown Projection. Could not reproject')
+            return
+
+        # Input stuff
+        src_crs = CRS.from_wkt(self.in_proj.wkt)
+
+        # Output stuff
+        dst_crs = CRS.from_wkt(self.out_proj.wkt)
+
+        # Now create virtual dataset
+        dat = []
+        for data in self.piter(self.indata['Raster']):
+            data2 = data_reproject(data, dst_crs, icrs=src_crs)
+
+            dat.append(data2)
+
+        self.outdata['Raster'] = dat
+
+    def settings(self, nodialog=False):
+        """
+        Entry point into item.
+
+        Parameters
+        ----------
+        nodialog : bool, optional
+            Run settings without a dialog. The default is False.
+
+        Returns
+        -------
+        bool
+            True if successful, False otherwise.
+
+        """
+        if 'Raster' not in self.indata:
+            self.showlog('No Raster Data.')
+            return False
+
+        if self.indata['Raster'][0].crs is None:
+            self.showlog('Your input data has no projection. '
+                         'Please assign one in the metadata summary.')
+            return False
+
+        if self.orig_wkt is None:
+            self.orig_wkt = self.indata['Raster'][0].crs.wkt
+        if self.targ_wkt is None:
+            self.targ_wkt = self.indata['Raster'][0].crs.wkt
+
+        self.in_proj.set_current(self.orig_wkt)
+        self.out_proj.set_current(self.targ_wkt)
+
+        if not nodialog:
+            tmp = self.exec_()
+            if tmp != 1:
+                return False
+
+        self.acceptall()
+
+        return True
+
+    def loadproj(self, projdata):
+        """
+        Load project data into class.
+
+        Parameters
+        ----------
+        projdata : dictionary
+            Project data loaded from JSON project file.
+
+        Returns
+        -------
+        chk : bool
+            A check to see if settings was successfully run.
+
+        """
+        self.orig_wkt = projdata['orig_wkt']
+        self.targ_wkt = projdata['targ_wkt']
 
-        return gdf
+        return False
 
+    def saveproj(self):
+        """
+        Save project data from class.
+
+        Returns
+        -------
+        projdata : dictionary
+            Project data to be saved to JSON project file.
+
+        """
+        projdata = {}
 
-class ImportShapeData(BasicModule):
-    """Import Shapefile Data."""
+        projdata['orig_wkt'] = self.in_proj.wkt
+        projdata['targ_wkt'] = self.out_proj.wkt
+
+        return projdata
+
+
+class GetProf(BasicModule):
+    """
+    Get a Profile.
+
+    This class extracts a profile from a raster dataset using a line shapefile.
+    """
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
     def settings(self, nodialog=False):
         """
         Entry point into item.
@@ -762,28 +1230,80 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
-        if not nodialog:
-            ext = 'Shapefile (*.shp);;' + 'All Files (*.*)'
+        if 'Raster' in self.indata:
+            data = copy.deepcopy(self.indata['Raster'])
+        else:
+            self.showlog('No raster data')
+            return False
+
+        ext = 'Shape file (*.shp)'
 
-            self.ifile, _ = QtWidgets.QFileDialog.getOpenFileName(self.parent,
-                                                                  'Open File',
-                                                                  '.', ext)
+        if not nodialog:
+            self.ifile, _ = QtWidgets.QFileDialog.getOpenFileName(
+                self.parent, 'Open Shape File', '.', ext)
             if self.ifile == '':
                 return False
+
         os.chdir(os.path.dirname(self.ifile))
 
-        gdf = gpd.read_file(self.ifile)
-        dat = {gdf.geom_type.iloc[0]: gdf}
+        try:
+            gdf = gpd.read_file(self.ifile, engine='pyogrio')
+        except:
+            self.showlog('There was a problem importing the shapefile. '
+                         'Please make sure you have at all the '
+                         'individual files which make up the shapefile.')
+            return None
+
+        gdf = gdf[gdf.geometry != None]
 
-        self.outdata['Vector'] = dat
+        if gdf.geom_type.iloc[0] != 'LineString':
+            self.showlog('You need lines in that shape file')
+            return False
+
+        data = lstack(data, self.piter, showlog=self.showlog)
+        dxy = min(data[0].xdim, data[0].ydim)
+        ogdf2 = None
+
+        icnt = 0
+        for line in gdf.geometry:
+            line2 = redistribute_vertices(line, dxy)
+            x, y = line2.coords.xy
+            xy = np.transpose([x, y])
+            ogdf = None
+
+            for idata in self.piter(data):
+                mdata = idata.to_mem()
+                z = []
+                for pnt in xy:
+                    z.append(idata.data[mdata.index(pnt[0], pnt[1])])
+
+                if ogdf is None:
+                    ogdf = pd.DataFrame(xy[:, 0], columns=['X'])
+                    ogdf['Y'] = xy[:, 1]
+
+                    x = ogdf['X']
+                    y = ogdf['Y']
+                    ogdf = gpd.GeoDataFrame(ogdf,
+                                            geometry=gpd.points_from_xy(x, y))
+
+                ogdf[idata.dataid] = z
+
+            icnt += 1
+            ogdf['line'] = str(icnt)
+            if ogdf2 is None:
+                ogdf2 = ogdf
+            else:
+                ogdf2 = ogdf2.append(ogdf, ignore_index=True)
+
+        self.outdata['Vector'] = [ogdf2]
 
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
@@ -794,1765 +1314,1535 @@
 
         Returns
         -------
         chk : bool
             A check to see if settings was successfully run.
 
         """
-        self.ifile = projdata['ifile']
-        chk = self.settings(True)
+        self.ifile = projdata['shapefile']
 
-        return chk
+        return False
 
     def saveproj(self):
         """
         Save project data from class.
 
         Returns
         -------
         projdata : dictionary
             Project data to be saved to JSON project file.
 
         """
         projdata = {}
-        projdata['ifile'] = self.ifile
+
+        projdata['shapefile'] = self.ifile
 
         return projdata
 
 
-class ExportBatch(ContextModule):
-    """Export Raster File List."""
+class GroupProj(QtWidgets.QWidget):
+    """
+    Group Proj.
+
+    Custom widget
+    """
+
+    def __init__(self, title='Projection', parent=None):
+        super().__init__(parent)
+
+        self.wkt = ''
+
+        self.gridlayout = QtWidgets.QGridLayout(self)
+        self.groupbox = QtWidgets.QGroupBox(title)
+        self.combodatum = QtWidgets.QComboBox()
+        self.comboproj = QtWidgets.QComboBox()
+        self.label = QtWidgets.QLabel()
+        self.label.setWordWrap(True)
+
+        self.gridlayout.addWidget(self.groupbox, 1, 0, 1, 2)
+
+        gridlayout = QtWidgets.QGridLayout(self.groupbox)
+        gridlayout.addWidget(self.combodatum, 0, 0, 1, 1)
+        gridlayout.addWidget(self.comboproj, 1, 0, 1, 1)
+        gridlayout.addWidget(self.label, 2, 0, 1, 1)
+
+        self.epsg_proj = getepsgcodes()
+        self.epsg_proj[r'Current / Current'] = self.wkt
+        self.epsg_proj[r'None / None'] = ''
+        tmp = list(self.epsg_proj.keys())
+        tmp.sort(key=lambda c: c.lower())
+
+        self.plist = {}
+        for i in tmp:
+            if r' / ' in i:
+                datum, proj = i.split(r' / ')
+            else:
+                datum = i
+                proj = i
+
+            if datum not in self.plist:
+                self.plist[datum] = []
+            self.plist[datum].append(proj)
+
+        tmp = list(set(self.plist.keys()))
+        tmp.sort()
+        tmp = ['Current', 'WGS 84']+tmp
+
+        for i in tmp:
+            j = self.plist[i]
+            if r'Geodetic Geographic' in j and j[0] != r'Geodetic Geographic':
+                self.plist[i] = [r'Geodetic Geographic']+self.plist[i]
+
+        self.combodatum.addItems(tmp)
+        self.comboproj.addItem('Current')
+        self.combodatum.currentIndexChanged.connect(self.combo_datum_change)
+        self.comboproj.currentIndexChanged.connect(self.combo_change)
+
+    def set_current(self, wkt):
+        """
+        Set new WKT for current option.
+
+        Parameters
+        ----------
+        wkt : str
+            Well Known Text descriptions for coordinates (WKT).
+
+        Returns
+        -------
+        None.
+
+        """
+        if wkt in ['', 'None']:
+            self.combodatum.setCurrentText('None')
+            return
+
+        self.wkt = wkt
+        self.epsg_proj[r'Current / Current'] = self.wkt
+        self.combo_change()
+
+    def combo_datum_change(self):
+        """
+        Change Combo.
+
+        Returns
+        -------
+        None.
+
+        """
+        indx = self.combodatum.currentIndex()
+        txt = self.combodatum.itemText(indx)
+        self.comboproj.currentIndexChanged.disconnect()
+
+        self.comboproj.clear()
+        self.comboproj.addItems(self.plist[txt])
+
+        self.comboproj.currentIndexChanged.connect(self.combo_change)
+
+        self.combo_change()
+
+    def combo_change(self):
+        """
+        Change Combo.
+
+        Returns
+        -------
+        None.
+
+        """
+        dtxt = self.combodatum.currentText()
+        ptxt = self.comboproj.currentText()
+
+        txt = dtxt + r' / '+ptxt
+
+        self.wkt = self.epsg_proj[txt]
+
+        if not isinstance(self.wkt, str):
+            self.wkt = epsgtowkt(self.wkt)
+
+        # The next two lines make sure we have spaces after ALL commas.
+        wkttmp = self.wkt.replace(', ', ',')
+        wkttmp = wkttmp.replace(',', ', ')
+
+        self.label.setText(wkttmp)
+
+
+class Metadata(ContextModule):
+    """
+    Edit Metadata.
+
+    This class allows the editing of the metadata for a raster dataset using a
+    GUI.
+
+    Attributes
+    ----------
+    banddata : dictionary
+        band data
+    bandid : dictionary
+        dictionary of strings containing band names.
+    """
 
     def __init__(self, parent=None):
         super().__init__(parent)
+        self.banddata = {}
+        self.dataid = {}
+        self.oldtxt = ''
+
+        self.combobox_bandid = QtWidgets.QComboBox()
+        self.pb_rename_id = QtWidgets.QPushButton('Rename Band Name')
+        self.lbl_rows = QtWidgets.QLabel()
+        self.lbl_cols = QtWidgets.QLabel()
+        self.inp_epsg_info = QtWidgets.QLabel()
+        self.txt_null = QtWidgets.QLineEdit()
+        self.dsb_tlx = QtWidgets.QLineEdit()
+        self.dsb_tly = QtWidgets.QLineEdit()
+        self.dsb_xdim = QtWidgets.QLineEdit()
+        self.dsb_ydim = QtWidgets.QLineEdit()
+        self.led_units = QtWidgets.QLineEdit()
+        self.lbl_min = QtWidgets.QLabel()
+        self.lbl_max = QtWidgets.QLabel()
+        self.lbl_mean = QtWidgets.QLabel()
+        self.lbl_dtype = QtWidgets.QLabel()
 
-        self.ofilt = QtWidgets.QComboBox()
-        self.odir = QtWidgets.QLineEdit('')
-        self.red = QtWidgets.QComboBox()
-        self.green = QtWidgets.QComboBox()
-        self.blue = QtWidgets.QComboBox()
-        self.ternary = QtWidgets.QCheckBox('Ternary Export')
+        self.proj = GroupProj('Input Projection')
 
         self.setupui()
 
     def setupui(self):
         """
         Set up UI.
 
         Returns
         -------
         None.
 
         """
         gridlayout_main = QtWidgets.QGridLayout(self)
         buttonbox = QtWidgets.QDialogButtonBox()
-        helpdocs = menu_default.HelpButton('pygmi.rsense.iodefs.exportbatch')
-        label_ofilt = QtWidgets.QLabel('Output Format:')
-        label_red = QtWidgets.QLabel('Red Band:')
-        label_green = QtWidgets.QLabel('Green Band:')
-        label_blue = QtWidgets.QLabel('Blue Band:')
-        pb_odir = QtWidgets.QPushButton('Output Directory')
-
-        ext = ('GeoTiff compressed using ZSTD', 'GeoTiff', 'ENVI', 'ERMapper',
-               'ERDAS Imagine')
-
-        self.ofilt.addItems(ext)
-
-        self.ternary.setChecked(False)
-        self.red.setEnabled(False)
-        self.green.setEnabled(False)
-        self.blue.setEnabled(False)
+        groupbox = QtWidgets.QGroupBox('Dataset')
 
+        gridlayout = QtWidgets.QGridLayout(groupbox)
+        label_tlx = QtWidgets.QLabel('Top Left X Coordinate:')
+        label_tly = QtWidgets.QLabel('Top Left Y Coordinate:')
+        label_xdim = QtWidgets.QLabel('X Dimension:')
+        label_ydim = QtWidgets.QLabel('Y Dimension:')
+        label_null = QtWidgets.QLabel('Null/Nodata value:')
+        label_rows = QtWidgets.QLabel('Rows:')
+        label_cols = QtWidgets.QLabel('Columns:')
+        label_min = QtWidgets.QLabel('Dataset Minimum:')
+        label_max = QtWidgets.QLabel('Dataset Maximum:')
+        label_mean = QtWidgets.QLabel('Dataset Mean:')
+        label_units = QtWidgets.QLabel('Dataset Units:')
+        label_bandid = QtWidgets.QLabel('Band Name:')
+        label_dtype = QtWidgets.QLabel('Data Type:')
+
+        sizepolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred,
+                                           QtWidgets.QSizePolicy.Expanding)
+        groupbox.setSizePolicy(sizepolicy)
         buttonbox.setOrientation(QtCore.Qt.Horizontal)
         buttonbox.setCenterButtons(True)
         buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
 
-        self.setWindowTitle(r'Export File List')
+        self.setWindowTitle('Dataset Metadata')
+
+        gridlayout_main.addWidget(label_bandid, 0, 0, 1, 1)
+        gridlayout_main.addWidget(self.combobox_bandid, 0, 1, 1, 3)
+        gridlayout_main.addWidget(self.pb_rename_id, 1, 1, 1, 3)
+        gridlayout_main.addWidget(groupbox, 2, 0, 1, 2)
+        gridlayout_main.addWidget(self.proj, 2, 2, 1, 2)
+        gridlayout_main.addWidget(buttonbox, 4, 0, 1, 4)
+
+        gridlayout.addWidget(label_tlx, 0, 0, 1, 1)
+        gridlayout.addWidget(self.dsb_tlx, 0, 1, 1, 1)
+        gridlayout.addWidget(label_tly, 1, 0, 1, 1)
+        gridlayout.addWidget(self.dsb_tly, 1, 1, 1, 1)
+        gridlayout.addWidget(label_xdim, 2, 0, 1, 1)
+        gridlayout.addWidget(self.dsb_xdim, 2, 1, 1, 1)
+        gridlayout.addWidget(label_ydim, 3, 0, 1, 1)
+        gridlayout.addWidget(self.dsb_ydim, 3, 1, 1, 1)
+        gridlayout.addWidget(label_null, 4, 0, 1, 1)
+        gridlayout.addWidget(self.txt_null, 4, 1, 1, 1)
+        gridlayout.addWidget(label_rows, 5, 0, 1, 1)
+        gridlayout.addWidget(self.lbl_rows, 5, 1, 1, 1)
+        gridlayout.addWidget(label_cols, 6, 0, 1, 1)
+        gridlayout.addWidget(self.lbl_cols, 6, 1, 1, 1)
+        gridlayout.addWidget(label_min, 7, 0, 1, 1)
+        gridlayout.addWidget(self.lbl_min, 7, 1, 1, 1)
+        gridlayout.addWidget(label_max, 8, 0, 1, 1)
+        gridlayout.addWidget(self.lbl_max, 8, 1, 1, 1)
+        gridlayout.addWidget(label_mean, 9, 0, 1, 1)
+        gridlayout.addWidget(self.lbl_mean, 9, 1, 1, 1)
+        gridlayout.addWidget(label_units, 10, 0, 1, 1)
+        gridlayout.addWidget(self.led_units, 10, 1, 1, 1)
+        gridlayout.addWidget(label_dtype, 11, 0, 1, 1)
+        gridlayout.addWidget(self.lbl_dtype, 11, 1, 1, 1)
+
+        buttonbox.accepted.connect(self.accept)
+        buttonbox.rejected.connect(self.reject)
 
-        gridlayout_main.addWidget(self.odir, 0, 0, 1, 1)
-        gridlayout_main.addWidget(pb_odir, 0, 1, 1, 1)
+        self.combobox_bandid.currentIndexChanged.connect(self.update_vals)
+        self.pb_rename_id.clicked.connect(self.rename_id)
 
-        gridlayout_main.addWidget(label_ofilt, 1, 0, 1, 1)
-        gridlayout_main.addWidget(self.ofilt, 1, 1, 1, 1)
+    def acceptall(self):
+        """
+        Accept option.
 
-        gridlayout_main.addWidget(self.ternary, 2, 0, 1, 2)
+        Returns
+        -------
+        None.
 
-        gridlayout_main.addWidget(label_red, 3, 0, 1, 1)
-        gridlayout_main.addWidget(self.red, 3, 1, 1, 1)
+        """
+        wkt = self.proj.wkt
 
-        gridlayout_main.addWidget(label_green, 4, 0, 1, 1)
-        gridlayout_main.addWidget(self.green, 4, 1, 1, 1)
+        self.update_vals()
+        for tmp in self.indata['Raster']:
+            for j in self.dataid.items():
+                if j[1] == tmp.dataid:
+                    i = self.banddata[j[0]]
+                    tmp.dataid = j[0]
+                    tmp.set_transform(transform=i.transform)
+                    tmp.nodata = i.nodata
+                    if wkt == 'None':
+                        tmp.crs = None
+                    else:
+                        tmp.crs = CRS.from_wkt(wkt)
+                    tmp.units = i.units
+                    tmp.data.mask = (tmp.data.data == i.nodata)
 
-        gridlayout_main.addWidget(label_blue, 5, 0, 1, 1)
-        gridlayout_main.addWidget(self.blue, 5, 1, 1, 1)
+    def rename_id(self):
+        """
+        Rename the band name.
 
-        gridlayout_main.addWidget(helpdocs, 8, 0, 1, 1)
-        gridlayout_main.addWidget(buttonbox, 8, 1, 1, 3)
+        Returns
+        -------
+        None.
 
-        buttonbox.accepted.connect(self.accept)
-        buttonbox.rejected.connect(self.reject)
-        pb_odir.pressed.connect(self.get_odir)
-        self.ternary.clicked.connect(self.click_ternary)
+        """
+        ctxt = str(self.combobox_bandid.currentText())
+        (skey, isokay) = QtWidgets.QInputDialog.getText(
+            self.parent, 'Rename Band Name',
+            'Please type in the new name for the band',
+            QtWidgets.QLineEdit.Normal, ctxt)
+
+        if isokay:
+            self.combobox_bandid.currentIndexChanged.disconnect()
+            indx = self.combobox_bandid.currentIndex()
+            txt = self.combobox_bandid.itemText(indx)
+            self.banddata[skey] = self.banddata.pop(txt)
+            self.dataid[skey] = self.dataid.pop(txt)
+            self.oldtxt = skey
+            self.combobox_bandid.setItemText(indx, skey)
+            self.combobox_bandid.currentIndexChanged.connect(self.update_vals)
 
-    def click_ternary(self):
+    def update_vals(self):
         """
-        Click ternary event.
+        Update the values on the interface.
 
         Returns
         -------
         None.
 
         """
-        if self.ternary.isChecked():
-            self.red.setEnabled(True)
-            self.green.setEnabled(True)
-            self.blue.setEnabled(True)
-        else:
-            self.red.setEnabled(False)
-            self.green.setEnabled(False)
-            self.blue.setEnabled(False)
+        odata = self.banddata[self.oldtxt]
+        odata.units = self.led_units.text()
+
+        try:
+            if self.txt_null.text().lower() != 'none':
+                odata.nodata = float(self.txt_null.text())
+            left = float(self.dsb_tlx.text())
+            top = float(self.dsb_tly.text())
+            xdim = float(self.dsb_xdim.text())
+            ydim = float(self.dsb_ydim.text())
+
+            odata.set_transform(xdim, left, ydim, top)
+
+        except ValueError:
+            self.showlog('Value error - abandoning changes')
+
+        indx = self.combobox_bandid.currentIndex()
+        txt = self.combobox_bandid.itemText(indx)
+        self.oldtxt = txt
+        idata = self.banddata[txt]
+
+        irows = idata.data.shape[0]
+        icols = idata.data.shape[1]
+
+        self.lbl_cols.setText(str(icols))
+        self.lbl_rows.setText(str(irows))
+        self.txt_null.setText(str(idata.nodata))
+        self.dsb_tlx.setText(str(idata.extent[0]))
+        self.dsb_tly.setText(str(idata.extent[-1]))
+        self.dsb_xdim.setText(str(idata.xdim))
+        self.dsb_ydim.setText(str(idata.ydim))
+        self.lbl_min.setText(str(idata.data.min()))
+        self.lbl_max.setText(str(idata.data.max()))
+        self.lbl_mean.setText(str(idata.data.mean()))
+        self.led_units.setText(str(idata.units))
+        self.lbl_dtype.setText(str(idata.data.dtype))
 
     def run(self):
         """
-        Run.
+        Entry point to start this routine.
 
         Returns
         -------
-        bool
+        tmp : bool
             True if successful, False otherwise.
 
         """
-        self.process_is_active(True)
+        bandid = []
+        if self.indata['Raster'][0].crs is None:
+            self.proj.set_current('None')
+        else:
+            self.proj.set_current(self.indata['Raster'][0].crs.wkt)
 
-        if 'RasterFileList' not in self.indata:
-            self.showprocesslog('No raster file list')
-            self.process_is_active(False)
-            return False
+        for i in self.indata['Raster']:
+            bandid.append(i.dataid)
+            self.banddata[i.dataid] = Data()
+            tmp = self.banddata[i.dataid]
+            self.dataid[i.dataid] = i.dataid
+            tmp.data = i.data
+            tmp.set_transform(transform=i.transform)
+            tmp.nodata = i.nodata
+            tmp.crs = i.crs
+            tmp.units = i.units
+
+        self.combobox_bandid.currentIndexChanged.disconnect()
+        self.combobox_bandid.addItems(bandid)
+        indx = self.combobox_bandid.currentIndex()
+        self.oldtxt = self.combobox_bandid.itemText(indx)
+        self.combobox_bandid.currentIndexChanged.connect(self.update_vals)
+
+        idata = self.banddata[self.oldtxt]
+
+        irows = idata.data.shape[0]
+        icols = idata.data.shape[1]
+
+        self.lbl_cols.setText(str(icols))
+        self.lbl_rows.setText(str(irows))
+        self.txt_null.setText(str(idata.nodata))
+        self.dsb_tlx.setText(str(idata.extent[0]))
+        self.dsb_tly.setText(str(idata.extent[-1]))
+        self.dsb_xdim.setText(str(idata.xdim))
+        self.dsb_ydim.setText(str(idata.ydim))
+        self.lbl_min.setText(str(idata.data.min()))
+        self.lbl_max.setText(str(idata.data.max()))
+        self.lbl_mean.setText(str(idata.data.mean()))
+        self.led_units.setText(str(idata.units))
+        self.lbl_dtype.setText(str(idata.data.dtype))
 
-        ifile = self.indata['RasterFileList'][0]
-        dat = get_data(ifile, piter=self.piter,
-                       showprocesslog=self.showprocesslog,
-                       extscene='Bands Only', metaonly=True)
-
-        bnames = [i.dataid for i in dat]
-
-        if 'Explained Variance Ratio' in bnames[0]:
-            bnames = [i.split('Explained Variance Ratio')[0] for i in bnames]
-
-        self.red.addItems(bnames)
-        self.green.addItems(bnames)
-        self.blue.addItems(bnames)
+        self.update_vals()
 
         tmp = self.exec_()
 
-        if tmp != 1 or self.odir.text() == '':
+        if tmp != 1:
             return False
 
-        filt = self.ofilt.currentText()
-        odir = self.odir.text()
-
-        if self.ternary.isChecked():
-            tnames = [self.red.currentText(),
-                      self.green.currentText(),
-                      self.blue.currentText()]
-        else:
-            tnames = None
-
-        self.showprocesslog('Export Data Busy...')
-
-        export_batch(self.indata, odir, filt, tnames, piter=self.piter,
-                     showprocesslog=self.showprocesslog)
+        self.acceptall()
 
-        self.showprocesslog('Export Data Finished!')
-        self.process_is_active(False)
         return True
 
-    def get_odir(self, odir=''):
-        """
-        Get output directory.
 
-        Parameters
-        ----------
-        odir : str, optional
-            Output directory submitted for testing. The default is ''.
+def check_dataid(out):
+    """
+    Check dataid for duplicates and renames where necessary.
 
-        Returns
-        -------
-        None.
+    Parameters
+    ----------
+    out : PyGMI Data
+        PyGMI raster data.
 
-        """
-        if odir == '':
-            odir = QtWidgets.QFileDialog.getExistingDirectory(
-                self.parent, 'Select Output Directory')
+    Returns
+    -------
+    out : PyGMI Data
+        PyGMI raster data.
 
-            if odir == '':
-                return
+    """
+    tmplist = []
+    for i in out:
+        tmplist.append(i.dataid)
+
+    tmpcnt = Counter(tmplist)
+    for elt, count in tmpcnt.items():
+        j = 1
+        for i in out:
+            if elt == i.dataid and count > 1:
+                i.dataid += '('+str(j)+')'
+                j += 1
 
-        self.odir.setText(odir)
+    return out
 
 
-def calculate_toa(dat, showprocesslog=print):
+def cluster_to_raster(indata):
     """
-    Top of atmosphere correction.
+    Convert cluster datasets to raster datasets.
 
-    Includes VNIR, SWIR and TIR bands.
+    Some routines will not understand the datasets produced by cluster
+    analysis routines, since they are designated 'Cluster' and not 'Raster'.
+    This provides a work-around for that.
 
     Parameters
     ----------
-    dat : Data
+    indata : Data
         PyGMI raster dataset
-    showprocesslog : function, optional
-        Routine to show text messages. The default is print.
 
     Returns
     -------
-    out : Data
+    indata : Data
         PyGMI raster dataset
+
     """
-    showprocesslog('Calculating top of atmosphere...')
+    if 'Cluster' not in indata:
+        return indata
+    if 'Raster' not in indata:
+        indata['Raster'] = []
 
-    datanew = {}
-    for datai in dat:
-        datanew[datai.dataid.split()[1]] = copy.deepcopy(datai)
-
-    out = []
-    for i in range(len(dat)):
-        idtmp = 'ImageData'+str(i+1)
-        if i+1 == 3:
-            idtmp += 'N'
-        datai = datanew[idtmp]
-
-        gain = datai.metadata['Gain']
-        sunelev = datai.metadata['SolarElev']
-        jday = datai.metadata['JulianDay']
-
-        lrad = (datai.data-1)*gain
-
-        if i < 9:
-            theta = np.deg2rad(90-sunelev)
-            datai.data = np.pi*lrad*EDIST[jday]**2/(ESUN[i]*np.cos(theta))
-        else:
-            datai.data = K2[i-9]/np.log(K1[i-9]/lrad+1)
-        datai.data.set_fill_value(datai.nodata)
-        dmask = datai.data.mask
-        datai.data = np.ma.array(datai.data.filled(), mask=dmask)
-        out.append(datai)
+    for i in indata['Cluster']:
+        indata['Raster'].append(i)
+        indata['Raster'][-1].data = indata['Raster'][-1].data + 1
 
-    return out
+    return indata
 
 
-def get_data(ifile, piter=None, showprocesslog=print, extscene=None,
-             alldata=False, tnames=None, metaonly=False):
+def cut_raster(data, ifile, showlog=print, deepcopy=True):
     """
-    Load a raster dataset off the disk using the rasterio libraries.
+    Cut a raster dataset.
 
-    It returns the data in a PyGMI data object.
+    Cut a raster dataset using a shapefile.
 
     Parameters
     ----------
+    data : Data
+        PyGMI Dataset
     ifile : str
-        filename to import
-    piter : iter, optional
-        Progress bar iterable. Default is None.
-    showprocesslog : function, optional
-        Routine to show text messages. The default is print.
-    extscene : str or None, optional
-        String used currently to give an option to limit bands in Sentinel-2.
-        The default is None.
-    alldata : bool, optional
-        Used to import all data. Currently used for Landsat. The default is
-        False.
-    tnames : list, optional
-        list of band names to import, in order. the default is None.
+        shapefile used to cut data
+    showlog : function, optional
+        Function for printing text. The default is print.
 
     Returns
     -------
-    dat : PyGMI raster Data
-        dataset imported
+    data : Data
+        PyGMI Dataset
     """
-    ifile = ifile[:]
-    bfile = os.path.basename(ifile)
+    if deepcopy is True:
+        data = copy.deepcopy(data)
 
-    if extscene is None:
-        extscene = ['']
+    try:
+        gdf = gpd.read_file(ifile)
+    except:
+        showlog('There was a problem importing the shapefile. Please make '
+                'sure you have at all the individual files which make up '
+                'the shapefile.')
+        return None
 
-    showprocesslog('Importing', bfile)
-
-    if 'AST_' in bfile and 'hdf' in bfile.lower():
-        dat = get_aster_hdf(ifile, piter)
-    elif 'AST_' in bfile and 'zip' in bfile.lower():
-        dat = get_aster_zip(ifile, piter, showprocesslog)
-    elif bfile[:4] in ['LT04', 'LT05', 'LE07', 'LC08', 'LM05', 'LC09']:
-        dat = get_landsat(ifile, piter, showprocesslog, alldata=alldata,
-                          tnames=tnames)
-        if dat is None and '.tar' not in ifile:
-            dat = get_raster(ifile, piter=piter, showprocesslog=showprocesslog,
-                             tnames=tnames)
-    elif (('.xml' in bfile and '.SAFE' in ifile) or
-          'Sentinel-2' in extscene or
-          ('S2A_' in bfile and 'zip' in bfile.lower()) or
-          ('S2B_' in bfile and 'zip' in bfile.lower())):
-        dat = get_sentinel2(ifile, piter, showprocesslog, extscene, tnames,
-                            metaonly)
-    elif (('MOD' in bfile or 'MCD' in bfile) and 'hdf' in bfile.lower() and
-          '.006.' in bfile):
-        dat = get_modisv6(ifile, piter)
-    elif 'AG1' in bfile and 'h5' in bfile.lower():
-        dat = get_aster_ged(ifile, piter)
-    elif 'Hyperion' in extscene:
-        dat = get_hyperion(ifile, piter, showprocesslog)
-    elif 'WorldView' in extscene:
-        dat = get_worldview(ifile, piter, showprocesslog)
-    else:
-        dat = get_raster(ifile, piter=piter, showprocesslog=showprocesslog,
-                         tnames=tnames, metaonly=metaonly)
+    gdf = gdf[gdf.geometry != None]
 
-    if dat is not None:
-        for i in dat:
-            if i.dataid is None:
-                i.dataid = ''
-            i.dataid = i.dataid.replace(',', ' ')
-
-        # Sort in band order.
-        dataid = [i.dataid for i in dat]
-        dorder = [i for _, i in natsorted(zip(dataid, range(len(dataid))))]
-        dat = [dat[i] for i in dorder]
+    if 'Polygon' not in gdf.geom_type.iloc[0]:
+        showlog('You need a polygon in that shape file')
+        return None
 
-    return dat
+    for idata in data:
+        # Convert the layer extent to image pixel coordinates
+        # poly = gdf['geometry'].iloc[0]
+        dext = idata.bounds
+        lext = gdf['geometry'].total_bounds
+
+        if ((dext[0] > lext[2]) or (dext[2] < lext[0])
+                or (dext[1] > lext[3]) or (dext[3] < lext[1])):
+
+            showlog('The shapefile is not in the same area as the raster '
+                    'dataset. Please check its coordinates and make sure its '
+                    'projection is the same as the raster dataset')
+            return None
+
+        # This section converts PolygonZ to Polygon, and takes first polygon.
+        # coords = gdf['geometry'].loc[0].exterior.coords
+        # coords = [Polygon([[p[0], p[1]] for p in coords])]
+        coords = gdf['geometry']
 
+        dat, trans = riomask(idata.to_mem(), coords, crop=True)
 
-def get_modisv6(ifile, piter=None):
+        idata.data = np.ma.masked_equal(dat.squeeze(), idata.nodata)
+
+        idata.set_transform(transform=trans)
+
+    data = trim_raster(data)
+
+    return data
+
+
+def data_reproject(data, ocrs, otransform=None, orows=None,
+                   ocolumns=None, icrs=None):
     """
-    Get MODIS v006 data.
+    Reproject dataset.
 
     Parameters
     ----------
-    ifile : str
-        filename to import
-    piter : iter, optional
-        Progress bar iterable. Default is None.
+    data : PyGMI Data
+        PyGMI dataset.
+    ocrs : CRS
+        output crs.
+    otransform : Affine, optional
+        Output affine transform. The default is None.
+    orows : int, optional
+        output rows. The default is None.
+    ocolumns : int, optional
+        output columns. The default is None.
+    icrs : CRS, optional
+        input crs. The default is None.
 
     Returns
     -------
-    dat : PyGMI raster Data
-        dataset imported
+    data2 : PyGMI Data
+        Reprojected dataset.
+
     """
-    if piter is None:
-        piter = ProgressBarText().iter
+    if icrs is None:
+        icrs = data.crs
 
-    dat = []
-    ifile = ifile[:]
+    if otransform is None:
+        src_height, src_width = data.data.shape
 
-    with rasterio.open(ifile) as dataset:
-        if dataset is None:
-            return None
-        subdata = dataset.subdatasets
+        otransform, ocolumns, orows = calculate_default_transform(
+            icrs, ocrs, src_width, src_height, *data.bounds)
 
-    dat = []
-    lulc = None
+    odata = np.zeros((orows, ocolumns), dtype=data.data.dtype)
+    odata, _ = reproject(source=data.data,
+                         destination=odata,
+                         src_transform=data.transform,
+                         src_crs=icrs,
+                         dst_transform=otransform,
+                         dst_crs=ocrs,
+                         src_nodata=data.nodata,
+                         resampling=rasterio.enums.Resampling['bilinear'])
 
-    for ifile2 in subdata:
-        dataset = rasterio.open(ifile2)
+    data2 = Data()
+    data2.data = odata
+    data2.crs = ocrs
+    data2.set_transform(transform=otransform)
+    data2.data = data2.data.astype(data.data.dtype)
+    data2.dataid = data.dataid
+    data2.wkt = CRS.to_wkt(ocrs)
+    data2.filename = data.filename[:-4]+'_prj'+data.filename[-4:]
 
-        wkt = dataset.crs.wkt
-        crs = dataset.crs
-        if 'Sinusoidal' in wkt:
-            wkt = wkt.replace('PROJCS["unnamed"', 'PROJCS["Sinusoidal"')
-            wkt = wkt.replace('GEOGCS["Unknown datum based upon the custom '
-                              'spheroid"',
-                              'GEOGCS["GCS_Unknown"')
-            wkt = wkt.replace('DATUM["Not specified '
-                              '(based on custom spheroid)"',
-                              'DATUM["D_Unknown"')
-            wkt = wkt.replace('SPHEROID["Custom spheroid"',
-                              'SPHEROID["S_Unknown"')
-            crs = CRS.from_wkt(wkt)
-
-        meta = dataset.tags()
-        bandid = dataset.descriptions[0]
-        nval = dataset.nodata
+    data2.data = np.ma.masked_equal(data2.data, data.nodata)
+    data2.nodata = data.nodata
+    data2.metadata = data.metadata
 
-        if bandid is None and ':' in ifile2:
-            bandid = ifile2[ifile2.rindex(':')+1:]
+    return data2
 
-        if 'scale_factor' in meta:
-            scale = float(meta['scale_factor'])
-        else:
-            scale = 1
 
-        if 'MOD13' in ifile and scale > 1:
-            scale = 1./scale
+def fftprep(data):
+    """
+    FFT preparation.
 
-        if 'MOD44B' in ifile and '_SD' in bandid and scale == 1:
-            scale = 0.01
+    Parameters
+    ----------
+    data : PyGMI Data type
+        Input dataset.
 
-        if 'add_offset' in meta:
-            offset = float(meta['add_offset'])
-        else:
-            offset = 0
+    Returns
+    -------
+    zfin : numpy array.
+        Output prepared data.
+    rdiff : int
+        rows divided by 2.
+    cdiff : int
+        columns divided by 2.
+    datamedian : float
+        Median of data.
 
-        rtmp2 = dataset.read(1)
-        rtmp2 = rtmp2.astype(float)
+    """
+    datamedian = np.ma.median(data.data)
+    ndat = data.data - datamedian
 
-        if nval == 32767:
-            mask = (rtmp2 > 32760)
-            lulc = np.zeros_like(rtmp2)
-            lulc[mask] = rtmp2[mask]-32760
-            lulc = np.ma.masked_equal(lulc, 0)
-        else:
-            mask = (rtmp2 == nval)
+    nr, nc = data.data.shape
+    cdiff = nc//2
+    rdiff = nr//2
 
-        rtmp2 = rtmp2*scale+offset
-        rtmp2[mask] = 1e+20
+    z1 = np.zeros((nr+2*rdiff, nc+2*cdiff))+np.nan
+    x1, y1 = np.mgrid[0: nr+2*rdiff, 0: nc+2*cdiff]
+    z1[rdiff:-rdiff, cdiff:-cdiff] = ndat.filled(np.nan)
 
-        dat.append(Data())
-        dat[-1].data = np.ma.array(rtmp2, mask=mask)
+    for j in range(2):
+        z1[0] = 0
+        z1[-1] = 0
+        z1[:, 0] = 0
+        z1[:, -1] = 0
 
-        dat[-1].dataid = bandid
-        dat[-1].nodata = 1e+20
-        dat[-1].crs = crs
-        dat[-1].set_transform(transform=dataset.transform)
-        dat[-1].filename = ifile
-        dat[-1].units = dataset.units[0]
-
-        dataset.close()
-
-    if lulc is not None:
-        dat.append(copy.deepcopy(dat[0]))
-        dat[-1].data = lulc
-        dat[-1].dataid = ('LULC: out of earth=7, water=6, barren=5, snow=4, '
-                          'wetland=3, urban=2, unclassifed=1')
-        dat[-1].nodata = 0
+        vert = np.zeros_like(z1)
+        hori = np.zeros_like(z1)
 
-    return dat
+        for i in range(z1.shape[0]):
+            mask = ~np.isnan(z1[i])
+            y = y1[i][mask]
+            z = z1[i][mask]
+            hori[i] = np.interp(y1[i], y, z)
+
+        for i in range(z1.shape[1]):
+            mask = ~np.isnan(z1[:, i])
+            x = x1[:, i][mask]
+            z = z1[:, i][mask]
 
+            vert[:, i] = np.interp(x1[:, i], x, z)
 
-def get_landsat(ifilet, piter=None, showprocesslog=print, alldata=False,
-                tnames=None):
+        hori[hori == 0] = np.nan
+        vert[vert == 0] = np.nan
+
+        hv = hori.copy()
+        hv[np.isnan(hori)] = vert[np.isnan(hori)]
+        hv[~np.isnan(hv)] = np.nanmean([hori[~np.isnan(hv)],
+                                        vert[~np.isnan(hv)]], 0)
+
+        z1[np.isnan(z1)] = hv[np.isnan(z1)]
+
+    zfin = z1
+
+    nr, nc = zfin.shape
+    zfin *= tukey(nc)
+    zfin *= tukey(nr)[:, np.newaxis]
+
+    return zfin, rdiff, cdiff, datamedian
+
+
+def fft_getkxy(fftmod, xdim, ydim):
     """
-    Get Landsat Data.
+    Get KX and KY.
 
     Parameters
     ----------
-    ifilet : str
-        filename to import
-    piter : iter, optional
-        Progress bar iterable. Default is None.
-    showprocesslog : function, optional
-        Routine to show text messages. The default is print.
-    alldata : bool, optional
-        Used to import all data. The default is False.
+    fftmod : numpy array
+        FFT data.
+    xdim : float
+        cell x dimension.
+    ydim : float
+        cell y dimension.
 
     Returns
     -------
-    out : Data
-        PyGMI raster dataset
-    """
-    if piter is None:
-        piter = ProgressBarText().iter
-
-    platform = os.path.basename(ifilet)[2: 4]
-    satbands = None
-    lstband = None
-
-    if platform in ('04', '05'):
-        satbands = {'B1': [450, 520],
-                    'B2': [520, 600],
-                    'B3': [630, 690],
-                    'B4': [760, 900],
-                    'B5': [1550, 1750],
-                    'B6': [10400, 12500],
-                    'B7': [2080, 2350]}
-
-    if platform == '07':
-        satbands = {'B1': [450, 520],
-                    'B2': [520, 600],
-                    'B3': [630, 690],
-                    'B4': [770, 900],
-                    'B5': [1550, 1750],
-                    'B6': [10400, 12500],
-                    'B7': [2090, 2350],
-                    'B8': [520, 900]}
-
-    if platform in ('08', '09'):
-        satbands = {'B1': [430, 450],
-                    'B2': [450, 510],
-                    'B3': [530, 590],
-                    'B4': [640, 670],
-                    'B5': [850, 880],
-                    'B6': [1570, 1650],
-                    'B7': [2110, 2290],
-                    'B8': [500, 680],
-                    'B9': [1360, 1380],
-                    'B10': [1060, 11190],
-                    'B11': [11500, 12510]}
-
-    idir = os.path.dirname(ifilet)
-
-    if '.tar' in ifilet:
-        with tarfile.open(ifilet) as tar:
-            tarnames = tar.getnames()
-            ifile = next((i for i in tarnames if '_MTL.txt' in i), None)
-            if ifile is None:
-                showprocesslog('Could not find MTL.txt file in tar archive')
-                return None
-            showprocesslog('Extracting tar...')
-
-            tar.extractall(idir)
-            ifile = os.path.join(idir, ifile)
-    elif '_MTL.txt' in ifilet:
-        ifile = ifilet
-    else:
-        showprocesslog('Input needs to be tar.gz or _MTL.txt for Landsat. '
-                       'Trying regular import')
-        return None
-
-    if alldata is True:
-        files = glob.glob(ifile[:-7]+'*.tif')
-    else:
-        files = glob.glob(ifile[:-7]+'*[0-9].tif')
+    KX : numpy array
+        x sample frequencies.
+    KY : numpy array
+        y sample frequencies.
 
-    if glob.glob(ifile[:-7]+'*ST_QA.tif'):
-        if 'LC08' in ifile or 'LC09' in ifile:
-            lstband = 'B10'
-        else:
-            lstband = 'B6'
-        satbands['LST'] = satbands[lstband]
+    """
+    ny, nx = fftmod.shape
+    kx = np.fft.fftfreq(nx, xdim)*2*np.pi
+    ky = np.fft.fftfreq(ny, ydim)*2*np.pi
 
-    showprocesslog('Importing Landsat data...')
+    KX, KY = np.meshgrid(kx, ky)
+    KY = -KY
+    return KX, KY
 
-    bnamelen = len(ifile[:-7])
-    nval = 0
-    dat = []
-    for ifile2 in piter(files):
-        fext = ifile2[bnamelen:-4]
-        fext = fext.upper().replace('BAND', 'B')
-        fext = fext.replace('SR_B', 'B')
-        fext = fext.replace('ST_B', 'B')
-
-        if fext == lstband:
-            fext = 'LST'
-
-        if tnames is not None and fext.replace(',', ' ') not in tnames:
-            continue
-
-        showprocesslog('Importing Band '+fext)
-        dataset = rasterio.open(ifile2)
-
-        if dataset is None:
-            showprocesslog('Problem with band '+fext)
-            continue
-
-        rtmp = dataset.read(1)
-
-        dat.append(Data())
-        dat[-1].data = rtmp
-        dat[-1].data = np.ma.masked_invalid(dat[-1].data)
-
-        nval = 0
-        if fext in ['QA_PIXEL', 'SR_QA_AEROSOL']:
-            nval = 1
-        if fext in ['ST_CDIST', 'ST_QA']:
-            nval = -9999
-        if fext in ['ST_TRAD', 'ST_URAD', 'ST_DRAD']:
-            nval = -9999
-        if fext in ['ST_ATRAN', 'ST_EMIS', 'ST_EMSD']:
-            nval = -9999
-
-        dat[-1].data.mask = dat[-1].data.mask | (dat[-1].data == nval)
-        if dat[-1].data.mask.size == 1:
-            dat[-1].data.mask = (np.ma.make_mask_none(dat[-1].data.shape) +
-                                 dat[-1].data.mask)
-
-        if 'L2SP' in ifile2:
-            if fext == 'LST':
-                showprocesslog('Converting band '+lstband+' to Kelvin. '
-                               'Band renamed as LST')
-                dat[-1].data = dat[-1].data*0.00341802 + 149.0
-            elif fext in satbands.keys():
-                showprocesslog('Converting band '+fext+' to reflectance.')
-                dat[-1].data = dat[-1].data*0.0000275 - 0.2
-            elif fext in ['ST_CDIST', 'ST_QA']:
-                dat[-1].data = dat[-1].data*0.01
-            elif fext in ['ST_TRAD', 'ST_URAD', 'ST_DRAD']:
-                dat[-1].data = dat[-1].data*0.001
-            elif fext in ['ST_ATRAN', 'ST_EMIS', 'ST_EMSD']:
-                dat[-1].data = dat[-1].data*0.0001
-
-        dat[-1].dataid = fext
-        dat[-1].nodata = nval
-        dat[-1].crs = dataset.crs
-        dat[-1].set_transform(transform=dataset.transform)
-        dat[-1].filename = ifile
-
-        bmeta = dat[-1].metadata
-        if satbands is not None and fext in satbands:
-            bmeta['WavelengthMin'] = satbands[fext][0]
-            bmeta['WavelengthMax'] = satbands[fext][1]
-            bmeta['Raster']['wavelength'] = (satbands[fext][1] +
-                                             satbands[fext][1])/2
-
-        dataset.close()
-
-    if not dat:
-        dat = None
-
-    if '.tar' in ifilet:
-        showprocesslog('Cleaning Extracted tar files...')
-        for tfile in piter(tarnames):
-            os.remove(os.path.join(os.path.dirname(ifile), tfile))
-    showprocesslog('Import complete')
-    return dat
 
-
-def get_worldview(ifilet, piter=None, showprocesslog=print):
+def fftcont(data, h):
     """
-    Get WorldView Data.
+    Continuation.
 
     Parameters
     ----------
-    ifilet : str
-        filename to import
-    piter : iter, optional
-        Progress bar iterable. Default is None.
-    showprocesslog : function, optional
-        Routine to show text messages. The default is print.
+    data : PyGMI Data
+        PyGMI raster data.
+    h : float
+        Height.
 
     Returns
     -------
-    out : Data
-        PyGMI raster dataset
+    dat : PyGMI Data
+        PyGMI raster data.
+
     """
-    if piter is None:
-        piter = ProgressBarText().iter
+    xdim = data.xdim
+    ydim = data.ydim
 
-    dtree = etree_to_dict(ET.parse(ifilet).getroot())
+    ndat, rdiff, cdiff, datamedian = fftprep(data)
 
-    if 'isd' not in dtree:
-        showprocesslog('Wrong xml file. Please choose the xml file in the '
-                       'PAN or MUL directory')
-        return None
+    fftmod = np.fft.fft2(ndat)
+
+    ny, nx = fftmod.shape
 
-    platform = dtree['isd']['TIL']['BANDID']
-    satid = dtree['isd']['IMD']['IMAGE']['SATID']
-    satbands = None
-
-    if platform == 'P':
-        satbands = {'1': [450, 800]}
-        bnum2name = {0: 'BAND_P'}
-
-    if platform == 'Multi' and 'WV' in satid:
-        satbands = {'1': [400, 450],
-                    '2': [450, 510],
-                    '3': [510, 580],
-                    '4': [585, 625],
-                    '5': [630, 690],
-                    '6': [705, 745],
-                    '7': [770, 895],
-                    '8': [860, 1040]}
-
-        bnum2name = {0: 'BAND_C',
-                     1: 'BAND_B',
-                     2: 'BAND_G',
-                     3: 'BAND_Y',
-                     4: 'BAND_R',
-                     5: 'BAND_RE',
-                     6: 'BAND_N',
-                     7: 'BAND_N2'}
-
-    if platform == 'Multi' and 'GE' in satid:
-        satbands = {'1': [450, 510],
-                    '2': [510, 580],
-                    '3': [655, 690],
-                    '4': [780, 920]}
-
-        bnum2name = {0: 'BAND_B',
-                     1: 'BAND_G',
-                     2: 'BAND_R',
-                     3: 'BAND_N'}
-
-    if satid == 'WV03':
-        Esun = {'BAND_P': 1574.41,
-                'BAND_C': 1757.89,
-                'BAND_B': 2004.61,
-                'BAND_G': 1830.18,
-                'BAND_Y': 1712.07,
-                'BAND_R': 1535.33,
-                'BAND_RE': 1348.08,
-                'BAND_N': 1055.94,
-                'BAND_N2': 858.77}
-    elif satid == 'WV02':
-        Esun = {'BAND_P': 1580.8140,
-                'BAND_C': 1758.2229,
-                'BAND_B': 1974.2416,
-                'BAND_G': 1856.4104,
-                'BAND_Y': 1738.4791,
-                'BAND_R': 1559.4555,
-                'BAND_RE': 1342.0695,
-                'BAND_N': 1069.7302,
-                'BAND_N2': 861.2866}
-    elif satid == 'GE01':
-        Esun = {'BAND_B': 1960.0,
-                'BAND_G': 1853.0,
-                'BAND_R': 1505.0,
-                'BAND_N': 1039.0}
-
-    idir = os.path.dirname(ifilet)
-
-    showprocesslog('Importing WorldView tiles...')
-
-    rmax = int(dtree['isd']['IMD']['NUMROWS'])
-    cmax = int(dtree['isd']['IMD']['NUMCOLUMNS'])
-
-    xmin = float(dtree['isd']['IMD']['MAP_PROJECTED_PRODUCT']['ORIGINX'])
-    ymax = float(dtree['isd']['IMD']['MAP_PROJECTED_PRODUCT']['ORIGINY'])
-    xdim = float(dtree['isd']['IMD']['MAP_PROJECTED_PRODUCT']['COLSPACING'])
-    ydim = float(dtree['isd']['IMD']['MAP_PROJECTED_PRODUCT']['ROWSPACING'])
-
-    dat = []
-    nval = 0
-    for i in range(len(satbands)):
-        fext = str(i+1)
-        dat.append(Data())
-        dat[-1].data = np.zeros((rmax, cmax))
-        dat[-1].dataid = f'Band {i+1}'
-        dat[-1].nodata = nval
-        dat[-1].set_transform(xdim, xmin, ydim, ymax)
-
-        bmeta = dat[-1].metadata
-        if satbands is not None and fext in satbands:
-            bmeta['WavelengthMin'] = satbands[fext][0]
-            bmeta['WavelengthMax'] = satbands[fext][1]
-        bmeta['Raster']['wavelength'] = (satbands[fext][0]+satbands[fext][1])/2
-
-    for tile in dtree['isd']['TIL']['TILE']:
-        ifile = os.path.join(idir, tile['FILENAME'])
-
-        rmin = int(tile['ULROWOFFSET'])
-        rmax = int(tile['LRROWOFFSET'])
-        cmin = int(tile['ULCOLOFFSET'])
-        cmax = int(tile['LRCOLOFFSET'])
-
-        showprocesslog('Importing '+tile['FILENAME'])
-        dataset = rasterio.open(ifile)
-
-        for i in piter(dataset.indexes):
-            rtmp = dataset.read(i)
-            bmeta = dataset.tags(i)
-            dat[i-1].data[rmin:rmax+1, cmin:cmax+1] = rtmp
-            dat[i-1].crs = dataset.crs
-            dat[i-1].filename = ifile
-        dataset.close()
-
-    showprocesslog('Calculating radiance and reflectance...')
-    indx = -1
-    for i in piter(dat):
-        indx += 1
-        mask = (i.data == nval)
-
-        scale = float(dtree['isd']['IMD'][bnum2name[indx]]['ABSCALFACTOR'])
-        bwidth = float(dtree['isd']['IMD'][bnum2name[indx]]['EFFECTIVEBANDWIDTH'])
-
-        i.data = i.data.astype(np.float32)
-
-        date = dtree['isd']['IMD']['IMAGE']['FIRSTLINETIME']
-
-        year = int(date[:4])
-        month = int(date[5:7])
-        day = int(date[8:10])
-        hour = int(date[11:13])
-        minute = int(date[14:16])
-        sec = float(date[17:-1])
-
-        UT = hour + minute/60. + sec/3600.
-
-        # Julian day
-
-        if month in (1, 2):
-            year -= 1
-            month += 12
-
-        A = int(year/100.)
-        B = 2 - A + int(A/4.)
-
-        JD = int(365.25*(year+4716))+int(30.6001*(month+1))+day+UT/24.+B-1524.5
-
-        D = JD - 2451545.0
-        g = np.deg2rad(357.529 + 0.98560028 * D)
-
-        dES = 1.00014 - 0.01671*np.cos(g) - 0.00014*np.cos(2*g)
-
-        szenith = 90. - float(dtree['isd']['IMD']['IMAGE']['MEANSUNEL'])
-        szenith = np.deg2rad(szenith)
-
-        tmp = dES**2 * np.pi / (Esun[bnum2name[indx]] * np.cos(szenith))
-        tmp = tmp * scale / bwidth
-        idata = i.data
-        i.data = ne.evaluate('idata * tmp')
+    KX, KY = fft_getkxy(fftmod, xdim, ydim)
+    k = np.sqrt(KX**2+KY**2)
 
-        i.data = np.ma.array(i.data, mask=mask)
+    filt = np.exp(-np.abs(k)*h)
 
-    if not dat:
-        dat = None
+    zout = np.real(np.fft.ifft2(fftmod*filt))
+    zout = zout[rdiff:-rdiff, cdiff:-cdiff]
+
+    zout = zout + datamedian
+
+    zout[data.data.mask] = data.data.fill_value
+
+    dat = Data()
+    dat.data = np.ma.masked_invalid(zout)
+    dat.data.mask = np.ma.getmaskarray(data.data)
+    dat.nodata = data.data.fill_value
+    dat.dataid = 'Upward_'+str(h)+'_'+data.dataid
+    dat.set_transform(transform=data.transform)
+    dat.crs = data.crs
 
-    showprocesslog('Import complete')
     return dat
 
 
-def get_hyperion(ifile, piter=None, showprocesslog=print):
+def get_shape_bounds(sfile, crs=None, showlog=print):
     """
-    Get Landsat Data.
+    Get bounds from a shape file.
 
     Parameters
     ----------
-    ifile : str
-        filename to import
-    piter : iter, optional
-        Progress bar iterable. Default is None.
-    showprocesslog : function, optional
-        Routine to show text messages. The default is print.
+    sfile : str
+        Filename for shapefile.
+    crs : rasterio CRS
+        target crs for shapefile
+    showlog : TYPE, optional
+        Print. The default is print.
 
     Returns
     -------
-    out : Data
-        PyGMI raster dataset
+    bounds : list
+        Rasterio bounds.
+
     """
-    if piter is None:
-        piter = ProgressBarText().iter
+    if sfile == '' or sfile is None:
+        return None
 
-    wavelength = [
-        355.59,  365.76,  375.94,  386.11,  396.29,  406.46,  416.64,  426.82,
-        436.99,  447.17,  457.34,  467.52,  477.69,  487.87,  498.04,  508.22,
-        518.39,  528.57,  538.74,  548.92,  559.09,  569.27,  579.45,  589.62,
-        599.80,  609.97,  620.15,  630.32,  640.50,  650.67,  660.85,  671.02,
-        681.20,  691.37,  701.55,  711.72,  721.90,  732.07,  742.25,  752.43,
-        762.60,  772.78,  782.95,  793.13,  803.30,  813.48,  823.65,  833.83,
-        844.00,  854.18,  864.35,  874.53,  884.70,  894.88,  905.05,  915.23,
-        925.41,  935.58,  945.76,  955.93,  966.11,  976.28,  986.46,  996.63,
-        1006.81, 1016.98, 1027.16, 1037.33, 1047.51, 1057.68,  851.92,  862.01,
-        872.10,  882.19,  892.28,  902.36,  912.45,  922.54,  932.64,  942.73,
-        952.82,  962.91,  972.99,  983.08,  993.17, 1003.30, 1013.30, 1023.40,
-        1033.49, 1043.59, 1053.69, 1063.79, 1073.89, 1083.99, 1094.09, 1104.19,
-        1114.19, 1124.28, 1134.38, 1144.48, 1154.58, 1164.68, 1174.77, 1184.87,
-        1194.97, 1205.07, 1215.17, 1225.17, 1235.27, 1245.36, 1255.46, 1265.56,
-        1275.66, 1285.76, 1295.86, 1305.96, 1316.05, 1326.05, 1336.15, 1346.25,
-        1356.35, 1366.45, 1376.55, 1386.65, 1396.74, 1406.84, 1416.94, 1426.94,
-        1437.04, 1447.14, 1457.23, 1467.33, 1477.43, 1487.53, 1497.63, 1507.73,
-        1517.83, 1527.92, 1537.92, 1548.02, 1558.12, 1568.22, 1578.32, 1588.42,
-        1598.51, 1608.61, 1618.71, 1628.81, 1638.81, 1648.90, 1659.00, 1669.10,
-        1679.20, 1689.30, 1699.40, 1709.50, 1719.60, 1729.70, 1739.70, 1749.79,
-        1759.89, 1769.99, 1780.09, 1790.19, 1800.29, 1810.38, 1820.48, 1830.58,
-        1840.58, 1850.68, 1860.78, 1870.87, 1880.98, 1891.07, 1901.17, 1911.27,
-        1921.37, 1931.47, 1941.57, 1951.57, 1961.66, 1971.76, 1981.86, 1991.96,
-        2002.06, 2012.15, 2022.25, 2032.35, 2042.45, 2052.45, 2062.55, 2072.65,
-        2082.75, 2092.84, 2102.94, 2113.04, 2123.14, 2133.24, 2143.34, 2153.34,
-        2163.43, 2173.53, 2183.63, 2193.73, 2203.83, 2213.93, 2224.03, 2234.12,
-        2244.22, 2254.22, 2264.32, 2274.42, 2284.52, 2294.61, 2304.71, 2314.81,
-        2324.91, 2335.01, 2345.11, 2355.21, 2365.20, 2375.30, 2385.40, 2395.50,
-        2405.60, 2415.70, 2425.80, 2435.89, 2445.99, 2456.09, 2466.09, 2476.19,
-        2486.29, 2496.39, 2506.48, 2516.59, 2526.68, 2536.78, 2546.88, 2556.98,
-        2566.98, 2577.08]
-
-    fwhm = [
-        11.3871, 11.3871, 11.3871, 11.3871, 11.3871, 11.3871, 11.3871, 11.3871,
-        11.3871, 11.3871, 11.3871, 11.3871, 11.3871, 11.3784, 11.3538, 11.3133,
-        11.2580, 11.1907, 11.1119, 11.0245, 10.9321, 10.8368, 10.7407, 10.6482,
-        10.5607, 10.4823, 10.4147, 10.3595, 10.3188, 10.2942, 10.2856, 10.2980,
-        10.3349, 10.3909, 10.4592, 10.5322, 10.6004, 10.6562, 10.6933, 10.7058,
-        10.7276, 10.7907, 10.8833, 10.9938, 11.1044, 11.1980, 11.2600, 11.2824,
-        11.2822, 11.2816, 11.2809, 11.2797, 11.2782, 11.2771, 11.2765, 11.2756,
-        11.2754, 11.2754, 11.2754, 11.2754, 11.2754, 11.2754, 11.2754, 11.2754,
-        11.2754, 11.2754, 11.2754, 11.2754, 11.2754, 11.2754, 11.0457, 11.0457,
-        11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0457,
-        11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0457, 11.0451,
-        11.0423, 11.0372, 11.0302, 11.0218, 11.0122, 11.0013, 10.9871, 10.9732,
-        10.9572, 10.9418, 10.9248, 10.9065, 10.8884, 10.8696, 10.8513, 10.8335,
-        10.8154, 10.7979, 10.7822, 10.7663, 10.7520, 10.7385, 10.7270, 10.7174,
-        10.7091, 10.7022, 10.6970, 10.6946, 10.6937, 10.6949, 10.6996, 10.7058,
-        10.7163, 10.7283, 10.7437, 10.7612, 10.7807, 10.8034, 10.8267, 10.8534,
-        10.8818, 10.9110, 10.9422, 10.9743, 11.0074, 11.0414, 11.0759, 11.1108,
-        11.1461, 11.1811, 11.2156, 11.2496, 11.2826, 11.3146, 11.3460, 11.3753,
-        11.4037, 11.4302, 11.4538, 11.4760, 11.4958, 11.5133, 11.5286, 11.5404,
-        11.5505, 11.5580, 11.5621, 11.5634, 11.5617, 11.5563, 11.5477, 11.5346,
-        11.5193, 11.5002, 11.4789, 11.4548, 11.4279, 11.3994, 11.3688, 11.3366,
-        11.3036, 11.2696, 11.2363, 11.2007, 11.1666, 11.1333, 11.1018, 11.0714,
-        11.0424, 11.0155, 10.9912, 10.9698, 10.9508, 10.9355, 10.9230, 10.9139,
-        10.9083, 10.9069, 10.9057, 10.9013, 10.8951, 10.8854, 10.8740, 10.8591,
-        10.8429, 10.8242, 10.8039, 10.7820, 10.7592, 10.7342, 10.7092, 10.6834,
-        10.6572, 10.6312, 10.6052, 10.5803, 10.5560, 10.5328, 10.5101, 10.4904,
-        10.4722, 10.4552, 10.4408, 10.4285, 10.4197, 10.4129, 10.4088, 10.4077,
-        10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077,
-        10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077,
-        10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077, 10.4077,
-        10.4077, 10.4077]
-
-    showprocesslog('Extracting zip...')
-
-    idir = os.path.dirname(ifile)
-    with zipfile.ZipFile(ifile) as zfile:
-        zipnames = zfile.namelist()
-        zfile.extractall(idir)
-
-    zipnames2 = [i for i in zipnames if i[-3:].lower() == 'tif']
-
-    # This section is to import the correct scale factors
-    # Pick first txt file since other should be readme.txt
-    header = [i for i in zipnames if '.txt' in i.lower()]
-
-    scale_vnir = 40.
-    scale_swir = 80.
-
-    if len(header) > 0:
-        hfile = header[0]
-
-        with open(os.path.join(idir, hfile)) as headerfile:
-            txt = headerfile.read()
-
-        txt = txt.split('\n')
-        scale_vnir = [i for i in txt if 'SCALING_FACTOR_VNIR' in i][0]
-        scale_swir = [i for i in txt if 'SCALING_FACTOR_SWIR' in i][0]
-
-        scale_vnir = float(scale_vnir.split(' = ')[-1])
-        scale_swir = float(scale_swir.split(' = ')[-1])
-
-    showprocesslog('Importing Hyperion data...')
-
-    nval = 0
-    dat = []
-    maskall = None
-    for ifile2 in piter(zipnames2):
-        fext = ifile2.split('_')[1]
-        bandno = int(fext[1:])
-
-        # Eliminate bands not illuminated
-        if bandno <= 7 or bandno >= 225:
-            continue
-
-        # Overlap Region
-        if 58 <= bandno <= 78:
-            continue
-
-        showprocesslog(f'Importing band {bandno}: {wavelength[bandno-1]} nm')
-        dataset = rasterio.open(os.path.join(idir, ifile2))
-
-        if dataset is None:
-            showprocesslog(f'Problem with band {bandno}')
-            continue
+    gdf = gpd.read_file(sfile)
 
-        rtmp = dataset.read(1)
+    gdf = gdf[gdf.geometry != None]
 
-        if bandno <= 70:
-            rtmp = rtmp / scale_vnir
-        else:
-            rtmp = rtmp / scale_swir
+    if crs is not None:
+        gdf = gdf.to_crs(crs)
 
-        dat.append(Data())
-        dat[-1].data = rtmp
+    if gdf.geom_type.iloc[0] == 'MultiPolygon':
+        showlog('You have a MultiPolygon. Only the first Polygon '
+                'of the MultiPolygon will be used.')
+        poly = gdf['geometry'].iloc[0]
+        tmp = poly.geoms[0]
 
-        dat[-1].data = np.ma.masked_invalid(dat[-1].data)
-        dat[-1].data.mask = dat[-1].data.mask | (dat[-1].data == nval)
-        if dat[-1].data.mask.size == 1:
-            dat[-1].data.mask = (np.ma.make_mask_none(dat[-1].data.shape) +
-                                 dat[-1].data.mask)
+        gdf.geometry.iloc[0] = tmp
 
-        if maskall is None:
-            maskall = dat[-1].data.mask
-        else:
-            maskall = np.logical_and(maskall, dat[-1].data.mask)
+    if gdf.geom_type.iloc[0] != 'Polygon':
+        showlog('You need a polygon in that shape file')
+        return None
 
-        dat[-1].dataid = f'Band {bandno}: {wavelength[bandno-1]} nm'
-        dat[-1].nodata = nval
-        dat[-1].crs = dataset.crs
-        dat[-1].set_transform(transform=dataset.transform)
-        dat[-1].filename = ifile
+    bounds = gdf.geometry.iloc[0].bounds
 
-        bmeta = {}
-        # if satbands is not None and fext in satbands:
+    return bounds
 
-        dat[-1].metadata['Raster']['wavelength'] = wavelength[bandno-1]
-        bmeta['WavelengthMin'] = wavelength[bandno-1]-fwhm[bandno-1]/2
-        bmeta['WavelengthMax'] = wavelength[bandno-1]+fwhm[bandno-1]/2
 
-        dat[-1].metadata.update(bmeta)
+def epsgtowkt(epsg):
+    """
+    Routine to get a WKT from an epsg code.
 
-        dataset.close()
+    Parameters
+    ----------
+    epsg : str or int
+        EPSG code.
 
-    if not dat:
-        dat = None
+    Returns
+    -------
+    out : str
+        WKT description.
 
-    for i in dat:
-        i.data.mask = maskall
+    """
+    out = CRS.from_epsg(int(epsg)).to_wkt()
+    return out
 
-    showprocesslog('Cleaning Extracted zip files...')
-    for zfile in zipnames:
-        os.remove(os.path.join(idir, zfile))
 
-    showprocesslog('Import complete')
-    return dat
+def getepsgcodes():
+    """
+    Routine used to get a list of EPSG codes.
 
+    Returns
+    -------
+    pcodes : dictionary
+        Dictionary of codes per projection in WKT format.
 
-def get_sentinel2(ifile, piter=None, showprocesslog=print, extscene=None,
-                  tnames=None, metaonly=False):
     """
-    Get Sentinel-2 Data.
+    with open(os.path.join(os.path.dirname(__file__), 'gcs.csv'),
+              encoding='utf-8') as dfile:
+        dlines = dfile.readlines()
+
+    dlines = dlines[1:]
+    dcodes = {}
+    for i in dlines:
+        tmp = i.split(',')
+        if tmp[1][0] == '"':
+            tmp[1] = tmp[1][1:-1]
+
+        dcodes[tmp[1]] = int(tmp[0])
+
+    with open(os.path.join(os.path.dirname(__file__), 'pcs.csv'),
+              encoding='utf-8') as pfile:
+        plines = pfile.readlines()
+
+    pcodes = {}
+    for i in dcodes:
+        pcodes[i+r' / Geodetic Geographic'] = dcodes[i]
+
+    plines = plines[1:]
+    for i in plines:
+        tmp = i.split(',')
+        if tmp[1][0] == '"':
+            tmp[1] = tmp[1][1:-1]
+
+        pcodes[tmp[1]] = int(tmp[0])
+
+    for datum in ['Cape', 'Hartebeesthoek94']:
+        for clong in range(15, 35, 2):
+            if 'Cape' in datum:
+                wkt = ('PROJCS["Cape / TM'+str(clong)+'",'
+                       'GEOGCS["Cape",'
+                       'DATUM["Cape",'
+                       'SPHEROID["Clarke 1880 (Arc)",'
+                       '6378249.145,293.4663077,'
+                       'AUTHORITY["EPSG","7013"]],'
+                       'AUTHORITY["EPSG","6222"]],'
+                       'PRIMEM["Greenwich",0,'
+                       'AUTHORITY["EPSG","8901"]],'
+                       'UNIT["degree",0.0174532925199433,'
+                       'AUTHORITY["EPSG","9122"]],'
+                       'AUTHORITY["EPSG","4222"]],'
+                       'PROJECTION["Transverse_Mercator"],'
+                       'PARAMETER["latitude_of_origin",0],'
+                       'PARAMETER["central_meridian",'+str(clong)+'],'
+                       'PARAMETER["scale_factor",1],'
+                       'PARAMETER["false_easting",0],'
+                       'PARAMETER["false_northing",0],'
+                       'UNIT["metre",1,AUTHORITY["EPSG","9001"]],'
+                       'AXIS["Easting",EAST],'
+                       'AXIS["Northing",NORTH]]')
+
+            elif 'Hartebeesthoek94' in datum:
+                wkt = ('PROJCS["Hartebeesthoek94 / TM'+str(clong)+'",'
+                       'GEOGCS["Hartebeesthoek94",'
+                       'DATUM["Hartebeesthoek94",'
+                       'SPHEROID["WGS 84",6378137,298.257223563,'
+                       'AUTHORITY["EPSG","7030"]],'
+                       'AUTHORITY["EPSG","6148"]],'
+                       'PRIMEM["Greenwich",0,'
+                       'AUTHORITY["EPSG","8901"]],'
+                       'UNIT["degree",0.0174532925199433,'
+                       'AUTHORITY["EPSG","9122"]],'
+                       'AUTHORITY["EPSG","4148"]],'
+                       'PROJECTION["Transverse_Mercator"],'
+                       'PARAMETER["latitude_of_origin",0],'
+                       'PARAMETER["central_meridian",'+str(clong)+'],'
+                       'PARAMETER["scale_factor",1],'
+                       'PARAMETER["false_easting",0],'
+                       'PARAMETER["false_northing",0],'
+                       'UNIT["metre",1,AUTHORITY["EPSG","9001"]],'
+                       'AXIS["Easting",EAST],'
+                       'AXIS["Northing",NORTH]]')
+
+            pcodes[datum+r' / TM'+str(clong)] = wkt
+
+    return pcodes
+
+
+def lstack(dat, piter=None, dxy=None, showlog=print, commonmask=False,
+           masterid=None, nodeepcopy=False, resampling='nearest',
+           checkdataid=True):
+    """
+    Layer stack datasets found in a single PyGMI data object.
+
+    The aim is to ensure that all datasets have the same number of rows and
+    columns.
 
     Parameters
     ----------
-    ifile : str
-        filename to import
+    dat : PyGMI Data
+        data object which stores datasets
     piter : iter, optional
-        Progress bar iterable. Default is None.
-    showprocesslog : function, optional
-        Routine to show text messages. The default is print.
-    extscene : str or None
-        String used currently to give an option to limit bands in Sentinel-2
-    tnames : list, optional
-        list of band names to import, in order. the default is None.
+        Progress bar iterator. The default is None.
+    dxy : float, optional
+        Cell size. The default is None.
+    showlog : function, optional
+        Print function. The default is print.
+    commonmask : bool, optional
+        Create a common mask for all bands. The default is False.
+    masterid : str, optional
+        ID of master dataset. The default is None.
 
     Returns
     -------
-    dat : PyGMI raster Data
-        dataset imported
+    out : PyGMI Data
+        data object which stores datasets
+
     """
     if piter is None:
         piter = ProgressBarText().iter
 
-    ifile = ifile[:]
+    if dat[0].isrgb:
+        return dat
 
-    with rasterio.open(ifile) as dataset:
-        if dataset is None:
-            return None
-        subdata = dataset.subdatasets
+    resampling = rasterio.enums.Resampling[resampling]
+    needsmerge = False
+    rows, cols = dat[0].data.shape
 
-    subdata = [i for i in subdata if 'TCI' not in i]  # TCI is true color
+    dtypes = []
+    for i in dat:
+        irows, icols = i.data.shape
+        if irows != rows or icols != cols:
+            needsmerge = True
+        if dxy is not None and (i.xdim != dxy or i.ydim != dxy):
+            needsmerge = True
+        if commonmask is True:
+            needsmerge = True
+        if i.extent != dat[0].extent:
+            needsmerge = True
+        dtypes.append(i.data.dtype)
+
+    dtypes = np.unique(dtypes)
+    dtype = None
+    nodata = None
+    if len(dtypes) > 1:
+        needsmerge = True
+        for i in dtypes:
+            if np.issubdtype(i, np.floating):
+                dtype = np.float64
+                nodata = 1e+20
+            elif dtype is None:
+                dtype = np.int32
+                nodata = 999999
+
+    if needsmerge is False:
+        if not nodeepcopy:
+            dat = copy.deepcopy(dat)
+        if checkdataid is True:
+            dat = check_dataid(dat)
+        return dat
 
-    nval = 0
-    dat = []
-    for bfile in subdata:
-        dataset = rasterio.open(bfile)
-        showprocesslog('Importing '+os.path.basename(bfile))
-        if dataset is None:
-            showprocesslog('Problem with '+ifile)
-            continue
-
-        for i in piter(dataset.indexes):
-            bname = dataset.descriptions[i-1]+f' ({dataset.transform[0]}m)'
-            bmeta = dataset.tags(i)
+    showlog('Merging data...')
+    if masterid is not None:
+        for i in dat:
+            if i.dataid == masterid:
+                data = i
+                break
 
-            if ('Bands Only' in extscene and
-                    'central wavelength' not in bname.lower()):
-                continue
+        xmin, xmax, ymin, ymax = data.extent
 
-            bname = bname.replace(',', ' ')
-            if tnames is not None and bname not in tnames:
-                continue
+        if dxy is None:
+            dxy = min(data.xdim, data.ydim)
+    else:
+        data = dat[0]
 
-            dat.append(Data())
+        if dxy is None:
+            dxy = min(data.xdim, data.ydim)
+            for data in dat:
+                dxy = min(dxy, data.xdim, data.ydim)
+
+        xmin0, xmax0, ymin0, ymax0 = data.extent
+        for data in dat:
+            xmin, xmax, ymin, ymax = data.extent
+            xmin = min(xmin, xmin0)
+            xmax = max(xmax, xmax0)
+            ymin = min(ymin, ymin0)
+            ymax = max(ymax, ymax0)
+
+    cols = int((xmax - xmin)/dxy)
+    rows = int((ymax - ymin)/dxy)
+    trans = rasterio.Affine(dxy, 0, xmin, 0, -1*dxy, ymax)
+
+    if cols == 0 or rows == 0:
+        showlog('Your rows or cols are zero. '
+                'Your input projection may be wrong')
+        return None
 
-            if not metaonly:
-                rtmp = dataset.read(i)
+    dat2 = []
+    cmask = None
+    for data in piter(dat):
+
+        if dtype is not None:
+            data.data = data.data.astype(dtype)
+            data.nodata = nodata
+
+        if data.crs is None:
+            showlog(f'{data.dataid} has no defined projection. '
+                    'Assigning local.')
+
+            data.crs = CRS.from_string('LOCAL_CS["Arbitrary",UNIT["metre",1,'
+                                       'AUTHORITY["EPSG","9001"]],'
+                                       'AXIS["Easting",EAST],'
+                                       'AXIS["Northing",NORTH]]')
+
+        doffset = 0.0
+        data.data.set_fill_value(data.nodata)
+        data.data = np.ma.array(data.data.filled(), mask=data.data.mask)
+
+        if data.data.min() <= 0:
+            doffset = data.data.min()-1.
+            data.data = data.data - doffset
+
+        trans0 = data.transform
+
+        height, width = data.data.shape
+
+        odata = np.zeros((rows, cols), dtype=data.data.dtype)
+        odata, _ = reproject(source=data.data,
+                             destination=odata,
+                             src_transform=trans0,
+                             src_crs=data.crs,
+                             src_nodata=data.nodata,
+                             dst_transform=trans,
+                             dst_crs=data.crs,
+                             resampling=resampling)
+
+        data2 = Data()
+        data2.data = np.ma.masked_equal(odata, data.nodata)
+        data2.data.mask = np.ma.getmaskarray(data2.data)
+        data2.nodata = data.nodata
+        data2.crs = data.crs
+        data2.set_transform(transform=trans)
+        data2.data = data2.data.astype(data.data.dtype)
+        data2.dataid = data.dataid
+        data2.filename = data.filename
 
-                dat[-1].data = rtmp
-                dat[-1].data = np.ma.masked_invalid(dat[-1].data)
-                dat[-1].data.mask = dat[-1].data.mask | (dat[-1].data == nval)
-                if dat[-1].data.mask.size == 1:
-                    dat[-1].mask = np.ma.getmaskarray(dat[-1].data)
-                dat[-1].data = dat[-1].data.astype(float)
-                dat[-1].data = dat[-1].data / 10000.
-
-            dat[-1].dataid = bname
-            dat[-1].nodata = nval
-            dat[-1].crs = dataset.crs
-            dat[-1].set_transform(transform=dataset.transform)
-            dat[-1].filename = ifile
-            dat[-1].units = 'Reflectance'
-
-            if 'WAVELENGTH' in bmeta and 'BANDWIDTH' in bmeta:
-                wlen = float(bmeta['WAVELENGTH'])
-                bwidth = float(bmeta['BANDWIDTH'])
-                bmeta['WavelengthMin'] = wlen - bwidth/2
-                bmeta['WavelengthMax'] = wlen + bwidth/2
-                dat[-1].metadata['Raster']['wavelength'] = wlen
-
-            dat[-1].metadata.update(bmeta)
+        dat2.append(data2)
 
-            if 'SOLAR_IRRADIANCE_UNIT' in bmeta:
-                dat[-1].units = bmeta['SOLAR_IRRADIANCE_UNIT']
+        if cmask is None:
+            cmask = dat2[-1].data.mask
+        else:
+            cmask = np.logical_or(cmask, dat2[-1].data.mask)
 
-        dataset.close()
+        dat2[-1].metadata = data.metadata
+        dat2[-1].data = dat2[-1].data + doffset
 
-    if not dat:
-        dat = None
+        dat2[-1].nodata = data.nodata
+        dat2[-1].data.set_fill_value(data.nodata)
+        dat2[-1].data = np.ma.array(dat2[-1].data.filled(),
+                                    mask=dat2[-1].data.mask)
 
-    return dat
+        data.data = data.data + doffset
 
+    if commonmask is True:
+        for idat in piter(dat2):
+            idat.data.mask = cmask
+            idat.data = np.ma.array(idat.data.filled(idat.nodata), mask=cmask)
 
-def get_aster_zip(ifile, piter=None, showprocesslog=print):
+    if checkdataid is True:
+        out = check_dataid(dat2)
+    else:
+        out = dat2
+
+    return out
+
+
+def merge_median(merged_data, new_data, merged_mask, new_mask, index=None,
+                 roff=None, coff=None):
     """
-    Get ASTER zip Data.
+    Merge using median for rasterio, taking minimum value.
 
     Parameters
     ----------
-    ifile : str
-        filename to import
-    piter : iter, optional
-        Progress bar iterable. Default is None.
-    showprocesslog : function, optional
-        Routine to show text messages. The default is print.
+    merged_data : numpy array
+        Old data.
+    new_data : numpy array
+        New data to merge to old data.
+    merged_mask : float
+        Old mask.
+    new_mask : float
+        New mask.
+    index : int, optional
+        index of the current dataset within the merged dataset collection.
+        The default is None.
+    roff : int, optional
+        row offset in base array. The default is None.
+    coff : int, optional
+        col offset in base array. The default is None.
 
     Returns
     -------
-    dat : PyGMI raster Data
-        dataset imported
+    None.
+
     """
-    if piter is None:
-        piter = ProgressBarText().iter
+    merged_data = np.ma.array(merged_data, mask=merged_mask)
+    new_data = np.ma.array(new_data, mask=new_mask)
 
-    satbands = {'1': [520, 600],
-                '2': [630, 690],
-                '3N': [780, 860],
-                '3B': [780, 860],
-                '4': [1600, 1700],
-                '5': [2145, 2185],
-                '6': [2185, 2225],
-                '7': [2235, 2285],
-                '8': [2295, 2365],
-                '9': [2360, 2430],
-                '10': [8125, 8475],
-                '11': [8475, 8825],
-                '12': [8925, 9275],
-                '13': [10250, 10950],
-                '14': [10950, 11650]}
-
-    if 'AST_07' in ifile:
-        scalefactor = 0.001
-        units = 'Surface Reflectance'
-    elif 'AST_05' in ifile:
-        scalefactor = 0.001
-        units = 'Surface Emissivity'
-    elif 'AST_08' in ifile:
-        scalefactor = 0.1
-        units = 'Surface Kinetic Temperature'
-    else:
-        return None
+    mtmp1 = np.logical_and(~merged_mask, ~new_mask)
+    mtmp2 = np.logical_and(~merged_mask, new_mask)
 
-    showprocesslog('Extracting zip...')
+    tmp1 = new_data.copy()
 
-    idir = os.path.dirname(ifile)
-    with zipfile.ZipFile(ifile) as zfile:
-        zipnames = zfile.namelist()
-        zfile.extractall(idir)
-
-    dat = []
-    nval = 0
-    for zfile in piter(zipnames):
-        if zfile.lower()[-4:] != '.tif':
-            continue
-
-        dataset1 = rasterio.open(os.path.join(idir, zfile))
-        if dataset1 is None:
-            showprocesslog('Problem with '+zfile)
-            continue
-
-        dataset = rasterio.vrt.WarpedVRT(dataset1)
-        rtmp = dataset.read(1)
-
-        dat.append(Data())
-        dat[-1].data = rtmp
-        dat[-1].data = np.ma.masked_invalid(dat[-1].data)*scalefactor
-        dat[-1].data.mask = dat[-1].data.mask | (dat[-1].data == nval)
-        if dat[-1].data.mask.size == 1:
-            dat[-1].mask = np.ma.getmaskarray(dat[-1].data)
-
-        dat[-1].dataid = zfile[zfile.index('Band'):zfile.index('.tif')]
-        dat[-1].nodata = nval
-        dat[-1].crs = dataset.crs
-        dat[-1].set_transform(transform=dataset.transform)
-        dat[-1].filename = ifile
-        dat[-1].units = units
-
-        bmeta = dat[-1].metadata
-        fext = dat[-1].dataid[4:]
-        bmeta['WavelengthMin'] = satbands[fext][0]
-        bmeta['WavelengthMax'] = satbands[fext][1]
-        bmeta['Raster']['wavelength'] = (satbands[fext][1]+satbands[fext][1])/2
-
-        dataset.close()
-        dataset1.close()
-
-    showprocesslog('Cleaning Extracted zip files...')
-    for zfile in zipnames:
-        os.remove(os.path.join(idir, zfile))
+    if True in mtmp1:
+        tmp1 = tmp1 - np.ma.median(new_data[mtmp1])
+        tmp1 = tmp1 + np.ma.median(merged_data[mtmp1])
 
-    return dat
+    tmp1[mtmp2] = merged_data[mtmp2]
+
+    merged_data[:] = tmp1
 
 
-def get_aster_hdf(ifile, piter=None):
+def merge_min(merged_data, new_data, merged_mask, new_mask, index=None,
+              roff=None, coff=None):
     """
-    Get ASTER hdf Data.
+    Merge using minimum for rasterio, taking minimum value.
 
     Parameters
     ----------
-    ifile : str
-        filename to import
-    piter : iter, optional
-        Progress bar iterable. Default is None.
+    merged_data : numpy array
+        Old data.
+    new_data : numpy array
+        New data to merge to old data.
+    merged_mask : float
+        Old mask.
+    new_mask : float
+        New mask.
+    index : int, optional
+        index of the current dataset within the merged dataset collection.
+        The default is None.
+    roff : int, optional
+        row offset in base array. The default is None.
+    coff : int, optional
+        col offset in base array. The default is None.
 
     Returns
     -------
-    dat : PyGMI raster Data
-        dataset imported
-    """
-    if piter is None:
-        piter = ProgressBarText().iter
-
-    satbands = {'1': [520, 600],
-                '2': [630, 690],
-                '3N': [780, 860],
-                '3B': [780, 860],
-                '4': [1600, 1700],
-                '5': [2145, 2185],
-                '6': [2185, 2225],
-                '7': [2235, 2285],
-                '8': [2295, 2365],
-                '9': [2360, 2430],
-                '10': [8125, 8475],
-                '11': [8475, 8825],
-                '12': [8925, 9275],
-                '13': [10250, 10950],
-                '14': [10950, 11650]}
-
-    ifile = ifile[:]
-
-    if 'AST_07' in ifile:
-        ptype = '07'
-    elif 'AST_L1T' in ifile:
-        ptype = 'L1T'
-    elif 'AST_05' in ifile:
-        ptype = '05'
-    elif 'AST_08' in ifile:
-        ptype = '08'
-    else:
-        return None
-    with rasterio.open(ifile) as dataset:
-        meta = dataset.tags()
-        subdata = dataset.subdatasets
-
-    if ptype == 'L1T':
-        ucc = {'ImageData1': float(meta['INCL1']),
-               'ImageData2': float(meta['INCL2']),
-               'ImageData3N': float(meta['INCL3N']),
-               'ImageData4': float(meta['INCL4']),
-               'ImageData5': float(meta['INCL5']),
-               'ImageData6': float(meta['INCL6']),
-               'ImageData7': float(meta['INCL7']),
-               'ImageData8': float(meta['INCL8']),
-               'ImageData9': float(meta['INCL9']),
-               'ImageData10': float(meta['INCL10']),
-               'ImageData11': float(meta['INCL11']),
-               'ImageData12': float(meta['INCL12']),
-               'ImageData13': float(meta['INCL13']),
-               'ImageData14': float(meta['INCL14'])}
-
-    solarelev = float(meta['SOLARDIRECTION'].split()[1])
-    cdate = meta['CALENDARDATE']
-    if len(cdate) == 8:
-        fmt = '%Y%m%d'
-    else:
-        fmt = '%Y-%m-%d'
-    dte = datetime.datetime.strptime(cdate, fmt)
-    jdate = dte.timetuple().tm_yday
-
-    if ptype == '07':
-        subdata = [i for i in subdata if 'SurfaceReflectance' in i]
-        scalefactor = 0.001
-        units = 'Surface Reflectance'
-    elif ptype == '05':
-        subdata = [i for i in subdata if 'SurfaceEmissivity' in i]
-        scalefactor = 0.001
-        units = 'Surface Emissivity'
-    elif ptype == '08':
-        scalefactor = 0.1
-        units = 'Surface Kinetic Temperature'
-    elif ptype == 'L1T':
-        subdata = [i for i in subdata if 'ImageData' in i]
-        scalefactor = 1
-        units = ''
-    else:
-        return None
+    None.
 
-    dat = []
-    nval = 0
-    calctoa = False
-    for bfile in piter(subdata):
-        if 'QA' in bfile:
-            continue
-        if ptype == 'L1T' and 'ImageData3B' in bfile:
-            continue
-
-        dataset1 = rasterio.open(bfile)
-        dataset = rasterio.vrt.WarpedVRT(dataset1)
-        # crs = dataset1.gcps[-1]
-        # breakpoint()
-
-        dat.append(Data())
-        dat[-1].data = dataset.read(1)
-        if ptype == '08':
-            dat[-1].data[dat[-1].data == 2000] = nval
-        dat[-1].data = np.ma.masked_invalid(dat[-1].data)*scalefactor
-        dat[-1].data.mask = dat[-1].data.mask | (dat[-1].data == nval)
-        if dat[-1].data.mask.size == 1:
-            dat[-1].mask = np.ma.getmaskarray(dat[-1].data)
-
-        dat[-1].dataid = bfile.split(':')[-1]
-        dat[-1].nodata = nval
-        dat[-1].set_transform(transform=dataset.transform)
-        dat[-1].crs = dataset.crs
-        dat[-1].metadata['SolarElev'] = solarelev
-        dat[-1].metadata['JulianDay'] = jdate
-        dat[-1].metadata['CalendarDate'] = cdate
-        dat[-1].metadata['ShortName'] = meta['SHORTNAME']
-        dat[-1].filename = ifile
-        dat[-1].units = units
-
-        if 'band' in dat[-1].dataid.lower():
-            bmeta = dat[-1].metadata
-            fext = dat[-1].dataid[4:].split()[0]
-            bmeta['WavelengthMin'] = satbands[fext][0]
-            bmeta['WavelengthMax'] = satbands[fext][1]
-            bmeta['Raster']['wavelength'] = (satbands[fext][1] +
-                                             satbands[fext][1])/2
-
-            if ptype == 'L1T' and 'ImageData' in ifile:
-                dat[-1].metadata['Gain'] = ucc[ifile[ifile.rindex('ImageData'):]]
-                calctoa = True
-        dataset.close()
-        dataset1.close()
+    """
+    tmp = np.logical_and(~merged_mask, ~new_mask)
 
-    if not dat:
-        dat = None
+    tmp1 = merged_data.copy()
+    tmp1[~new_mask] = new_data[~new_mask]
+    tmp1[tmp] = np.minimum(merged_data[tmp], new_data[tmp])
 
-    if ptype == 'L1T' and calctoa is True:
-        dat = calculate_toa(dat)
+    merged_data[:] = tmp1
 
-    return dat
 
-
-def get_aster_ged(ifile, piter=None):
+def merge_max(merged_data, new_data, merged_mask, new_mask, index=None,
+              roff=None, coff=None):
     """
-    Get ASTER GED data.
+    Merge using maximum for rasterio, taking maximum value.
 
     Parameters
     ----------
-    ifile : str
-        filename to import
-    piter : iter, optional
-        Progress bar iterable. Default is None
+    merged_data : numpy array
+        Old data.
+    new_data : numpy array
+        New data to merge to old data.
+    merged_mask : float
+        Old mask.
+    new_mask : float
+        New mask.
+    index : int, optional
+        index of the current dataset within the merged dataset collection.
+        The default is None.
+    roff : int, optional
+        row offset in base array. The default is None.
+    coff : int, optional
+        col offset in base array. The default is None.
 
     Returns
     -------
-    dat : PyGMI raster Data
-        dataset imported
+    None.
+
     """
-    if piter is None:
-        piter = ProgressBarText().iter
+    tmp = np.logical_and(~merged_mask, ~new_mask)
 
-    dat = []
-    ifile = ifile[:]
+    tmp1 = merged_data.copy()
+    tmp1[~new_mask] = new_data[~new_mask]
+    tmp1[tmp] = np.maximum(merged_data[tmp], new_data[tmp])
 
-    with rasterio.open(ifile) as dataset:
-        subdata = dataset.subdatasets
+    merged_data[:] = tmp1
 
-    i = -1
-    for ifile2 in subdata:
-        dataset = rasterio.open(ifile2)
-        units = ''
-
-        if 'ASTER_GDEM' in ifile2:
-            bandid = 'ASTER GDEM'
-            units = 'meters'
-        if 'Land_Water_Map' in ifile2:
-            bandid = 'Land_water_map'
-        if 'Observations' in ifile2:
-            bandid = 'Observations'
-            units = 'number per pixel'
-
-        rtmp2 = dataset.read()
-        if 'Latitude' in ifile2:
-            ymax = rtmp2.max()
-            ydim = abs((rtmp2.max()-rtmp2.min())/rtmp2.shape[1])
-            continue
-
-        if 'Longitude' in ifile2:
-            xmin = rtmp2.min()
-            xdim = abs((rtmp2.max()-rtmp2.min())/rtmp2.shape[2])
-            continue
-
-        if rtmp2.shape[-1] == min(rtmp2.shape) and rtmp2.ndim == 3:
-            rtmp2 = np.transpose(rtmp2, (2, 0, 1))
-
-        nbands = 1
-        if rtmp2.ndim == 3:
-            nbands = rtmp2.shape[0]
-
-        for i2 in range(nbands):
-            nval = -9999
-            i += 1
-
-            dat.append(Data())
-            if rtmp2.ndim == 3:
-                dat[i].data = rtmp2[i2]
-            else:
-                dat[i].data = rtmp2
 
-            dat[i].data = np.ma.masked_invalid(dat[i].data)
-            dat[i].data.mask = (np.ma.getmaskarray(dat[i].data)
-                                | (dat[i].data == nval))
-            if dat[i].data.mask.size == 1:
-                dat[-1].mask = np.ma.getmaskarray(dat[-1].data)
-
-            dat[i].data = dat[i].data * 1.0
-            if 'Emissivity/Mean' in ifile2:
-                bandid = 'Emissivity_mean_band_'+str(10+i2)
-                dat[i].data = dat[i].data * 0.001
-            if 'Emissivity/SDev' in ifile2:
-                bandid = 'Emissivity_std_dev_band_'+str(10+i2)
-                dat[i].data = dat[i].data * 0.0001
-            if 'NDVI/Mean' in ifile2:
-                bandid = 'NDVI_mean'
-                dat[i].data = dat[i].data * 0.01
-            if 'NDVI/SDev' in ifile2:
-                bandid = 'NDVI_std_dev'
-                dat[i].data = dat[i].data * 0.01
-            if 'Temperature/Mean' in ifile2:
-                bandid = 'Temperature_mean'
-                units = 'Kelvin'
-                dat[i].data = dat[i].data * 0.01
-            if 'Temperature/SDev' in ifile2:
-                bandid = 'Temperature_std_dev'
-                units = 'Kelvin'
-                dat[i].data = dat[i].data * 0.01
-
-            dat[i].dataid = bandid
-            dat[i].nodata = nval
-            dat[i].crs = CRS.from_epsg(4326)  # WGS84 geodetic
-            dat[i].units = units
-        dataset.close()
+def redistribute_vertices(geom, distance):
+    """
+    Redistribute vertices in a geometry.
 
-    for i in dat:
-        i.set_transform(xdim, xmin, ydim, ymax)
+    From https://stackoverflow.com/questions/34906124/interpolating-every-x-distance-along-multiline-in-shapely,
+    and by Mike-T.
 
-    return dat
+    Parameters
+    ----------
+    geom : shapely geometry
+        Geometry from geopandas.
+    distance : float
+        sampling distance.
+
+    Raises
+    ------
+    ValueError
+        Error when there is an unknown geometry.
 
+    Returns
+    -------
+    shapely geometry
+        New geometry.
 
-def get_aster_ged_bin(ifile):
     """
-    Get ASTER GED binary format.
+    if geom.geom_type == 'LineString':
+        num_vert = int(round(geom.length / distance))
+        if num_vert == 0:
+            num_vert = 1
+        return LineString(
+            [geom.interpolate(float(n) / num_vert, normalized=True)
+             for n in range(num_vert + 1)])
+    if geom.geom_type == 'MultiLineString':
+        parts = [redistribute_vertices(part, distance)
+                 for part in geom]
+        return type(geom)([p for p in parts if not p.is_empty])
+    raise ValueError('unhandled geometry %s', (geom.geom_type,))
 
-    Emissivity_Mean_Description: Mean Emissivity for each pixel on grid-box
-    using all ASTER data from 2000-2010
-    Emissivity_SDev_Description: Emissivity Standard Deviation for each pixel
-    on grid-box using all ASTER data from 2000-2010
-    Temperature_Mean_Description: Mean Temperature (K) for each pixel on
-    grid-box using all ASTER data from 2000-2010
-    Temperature_SDev_Description: Temperature Standard Deviation for each pixel
-    on grid-box using all ASTER data from 2000-2010
-    NDVI_Mean_Description: Mean NDVI for each pixel on grid-box using all ASTER
-    data from 2000-2010
-    NDVI_SDev_Description: NDVI Standard Deviation for each pixel on grid-box
-    using all ASTER data from 2000-2010
-    Land_Water_Map_LWmap_Description: Land Water Map using ASTER visible bands
-    Observations_NumObs_Description: Number of values used in computing mean
-    and standard deviation for each pixel.
-    Geolocation_Latitude_Description: Latitude
-    Geolocation_Longitude_Description: Longitude
-    ASTER_GDEM_ASTGDEM_Description: ASTER GDEM resampled to NAALSED
+
+def taylorcont(data, h):
+    """
+    Taylor Continuation.
 
     Parameters
     ----------
-    ifile : str
-        filename to import
+    data : PyGMI Data
+        PyGMI raster data.
+    h : float
+        Height.
 
     Returns
     -------
-    dat : PyGMI raster Data
-        dataset imported
-    """
-    dat = []
-    nval = -9999
-    bandid = {}
-
-    bandid[0] = 'Emissivity_mean_band_10'
-    bandid[1] = 'Emissivity_mean_band_11'
-    bandid[2] = 'Emissivity_mean_band_12'
-    bandid[3] = 'Emissivity_mean_band_13'
-    bandid[4] = 'Emissivity_mean_band_14'
-    bandid[5] = 'Emissivity_std_dev_band_10'
-    bandid[6] = 'Emissivity_std_dev_band_11'
-    bandid[7] = 'Emissivity_std_dev_band_12'
-    bandid[8] = 'Emissivity_std_dev_band_13'
-    bandid[9] = 'Emissivity_std_dev_band_14'
-    bandid[10] = 'Temperature_mean'
-    bandid[11] = 'Temperature_std_dev'
-    bandid[12] = 'NDVI_mean'
-    bandid[13] = 'NDVI_std_dev'
-    bandid[14] = 'Land_water_map'
-    bandid[15] = 'Observations'
-    bandid[16] = 'Latitude'
-    bandid[17] = 'Longitude'
-    bandid[18] = 'ASTER GDEM'
-
-    scale = [0.001, 0.001, 0.001, 0.001, 0.001,
-             0.0001, 0.0001, 0.0001, 0.0001, 0.0001,
-             0.01, 0.01, 0.01, 0.01,
-             1, 1, 0.001, 0.001, 1]
-
-    units = ['', '', '', '', '', '', '', '', '', '', 'Kelvin', 'Kelvin',
-             '', '', '', 'Number per pixel', 'degrees', 'degrees', 'meters']
-
-    data = np.fromfile(ifile, dtype=np.int32)
-    rows_cols = int((data.size/19)**0.5)
-    data.shape = (19, rows_cols, rows_cols)
-
-    lats = data[16]*scale[16]
-    lons = data[17]*scale[17]
-
-    latsdim = (lats.max()-lats.min())/(lats.shape[0]-1)
-    lonsdim = (lons.max()-lons.min())/(lons.shape[0]-1)
-
-    tlx = lons.min()-abs(lonsdim/2)
-    tly = lats.max()+abs(latsdim/2)
-
-    for i in range(19):
-        dat.append(Data())
-
-        dat[i].data = data[i]*scale[i]
-
-        dat[i].dataid = bandid[i]
-        dat[i].nodata = nval*scale[i]
-        dat[i].xdim = lonsdim
-        dat[i].ydim = latsdim
-        dat[i].units = units[i]
-
-        rows, cols = dat[i].data.shape
-        xmin = tlx
-        ymax = tly
-        ymin = ymax - rows*dat[i].ydim
-        xmax = xmin + cols*dat[i].xdim
-
-        dat[i].extent = [xmin, xmax, ymin, ymax]
-
-    dat.pop(17)
-    dat.pop(16)
+    dat : PyGMI Data
+        PyGMI raster data.
 
+    """
+    dz = verticalp(data, order=1)
+    dz2 = verticalp(data, order=2)
+    dz3 = verticalp(data, order=3)
+    zout = (data.data + h*dz + h**2*dz2/math.factorial(2) +
+            h**3*dz3/math.factorial(3))
+
+    dat = Data()
+    dat.data = np.ma.masked_invalid(zout)
+    dat.data.mask = np.ma.getmaskarray(data.data)
+    dat.nodata = data.data.fill_value
+    dat.dataid = 'Downward_'+str(h)+'_'+data.dataid
+    dat.set_transform(transform=data.transform)
+    dat.crs = data.crs
     return dat
 
 
-def etree_to_dict(t):
+def trim_raster(olddata):
     """
-    Convert an ElementTree to dictionary.
+    Trim nulls from a raster dataset.
 
-    From K3--rnc: https://stackoverflow.com/questions/7684333/converting-xml-to-dictionary-using-elementtree
+    This function trims entire rows or columns of data which are masked,
+    and are on the edges of the dataset. Masked values are set to the null
+    value.
 
     Parameters
     ----------
-    t : Elementtree
-        Root.
+    olddata : Data
+        PyGMI dataset
 
     Returns
     -------
-    d : dictionary
-        DESCRIPTION.
-
+    olddata : Data
+        PyGMI dataset
     """
-    d = {t.tag: {} if t.attrib else None}
-    children = list(t)
-    if children:
-        dd = defaultdict(list)
-        for dc in map(etree_to_dict, children):
-            for k, v in dc.items():
-                dd[k].append(v)
-        d = {t.tag: {k: v[0] if len(v) == 1 else v
-                     for k, v in dd.items()}}
-    if t.attrib:
-        d[t.tag].update(('@' + k, v)
-                        for k, v in t.attrib.items())
-    if t.text:
-        text = t.text.strip()
-        if children or t.attrib:
-            if text:
-                d[t.tag]['#text'] = text
-        else:
-            d[t.tag] = text
-    return d
+    for data in olddata:
+        mask = np.ma.getmaskarray(data.data)
+        # data.data.data[mask] = data.nodata
+
+        rowstart = 0
+        for i in range(mask.shape[0]):
+            if bool(mask[i].min()) is False:
+                break
+            rowstart += 1
+
+        rowend = mask.shape[0]
+        for i in range(mask.shape[0]-1, -1, -1):
+            if bool(mask[i].min()) is False:
+                break
+            rowend -= 1
+
+        colstart = 0
+        for i in range(mask.shape[1]):
+            if bool(mask[:, i].min()) is False:
+                break
+            colstart += 1
+
+        colend = mask.shape[1]
+        for i in range(mask.shape[1]-1, -1, -1):
+            if bool(mask[:, i].min()) is False:
+                break
+            colend -= 1
+
+        drows, dcols = data.data.shape
+        data.data = data.data[rowstart:rowend, colstart:colend]
+        data.data.mask = mask[rowstart:rowend, colstart:colend]
+        # data.data.mask = (data.data.data == data.nodata)
+        xmin = data.extent[0] + colstart*data.xdim
+        ymax = data.extent[-1] - rowstart*data.ydim
+
+        data.set_transform(data.xdim, xmin, data.ydim, ymax)
+
+    return olddata
 
 
-def export_batch(indata, odir, filt, tnames=None, piter=None,
-                 showprocesslog=print):
+def verticalp(data, order=1):
     """
-    Export a batch of files directly from satellite format to disk.
+    Vertical derivative.
 
     Parameters
     ----------
-    indata : dictionary
-        Dictionary containing 'RasterFileList' as one of its keys.
-    odir : str
-        Output Directory.
-    filt : str
-        type of file to export.
-    tnames : list, optional
-        list of band names to import, in order. the default is None.
-    piter : iter, optional
-        Progress bar iterable. Default is None.
-    showprocesslog : function, optional
-        Routine to show text messages. The default is print.
+    data : numpy array
+        Input data.
+    order : float, optional
+        Order. The default is 1.
 
     Returns
     -------
-    None.
+    dout : numpy array
+        Output data
 
     """
-    if 'RasterFileList' not in indata:
-        showprocesslog('You need a raster file list')
-        return
-
-    ifiles = indata['RasterFileList']
-
-    filt2gdal = {'GeoTiff compressed using ZSTD': 'GTiff',
-                 'GeoTiff': 'GTiff',
-                 'ENVI': 'ENVI',
-                 'ERMapper': 'ERS',
-                 'ERDAS Imagine': 'HFA'}
-
-    compression = 'NONE'
-    ofilt = filt2gdal[filt]
-    if filt == 'GeoTiff compressed using ZSTD':
-        compression = 'ZSTD'
-
-    os.makedirs(odir, exist_ok=True)
-
-    for ifile in ifiles:
-        showprocesslog('Processing '+os.path.basename(ifile))
-        ofile = os.path.join(odir, os.path.basename(ifile))
-        ofile = ofile[:-4]+'.tif'
-
-        if tnames is not None:
-            ofile = ofile[:-4]+'_tern.tif'
-
-        if os.path.exists(ofile):
-            showprocesslog('Output file exists, skipping')
-            continue
-
-        dat = get_data(ifile, piter=piter,
-                       showprocesslog=showprocesslog, tnames=tnames,
-                       extscene='Bands Only')
-
-        odat = []
-        if tnames is not None:
-            for i in tnames:
-                for j in dat:
-                    if i in j.dataid:
-                        odat.append(j)
-                        break
-        else:
-            odat = dat
+    xdim = data.xdim
+    ydim = data.ydim
 
-        showprocesslog('Exporting '+os.path.basename(ofile))
-        export_raster(ofile, odat, ofilt, piter=piter, compression=compression)
+    ndat, rdiff, cdiff, _ = fftprep(data)
+    fftmod = np.fft.fft2(ndat)
 
+    KX, KY = fft_getkxy(fftmod, xdim, ydim)
 
-def _test5P():
-    """Test routine."""
-    import sys
-    import matplotlib.pyplot as plt
+    k = np.sqrt(KX**2+KY**2)
+    filt = k**order
 
-    sfile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\Sentinel-5P\CCUS_Sept2021_25kmbuffer.shp"
-    ifile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\Sentinel-5P\S5P_OFFL_L2__CH4____20230111T102529_20230111T120700_27184_03_020400_20230113T024518.nc"
+    zout = np.real(np.fft.ifft2(fftmod*filt))
+    zout = zout[rdiff:-rdiff, cdiff:-cdiff]
 
-    os.chdir(r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\Sentinel-5P")
+    return zout
 
-    app = QtWidgets.QApplication(sys.argv)
-    tmp = ImportSentinel5P()
-    tmp.ifile = ifile
-    tmp.settings()
-
-    if 'Vector' not in tmp.outdata:
-        print('No data')
-        return
-
-    shp = gpd.read_file(sfile)
-    shp = shp.to_crs(4326)
-
-    plt.figure(dpi=150)
-    ax = plt.gca()
-    shp.plot(ax=ax, fc='none', ec='black')
-    try:
-        ctx.add_basemap(ax, crs=shp.crs,
-                        source=ctx.providers.OpenStreetMap.Mapnik)
-    except:
-        print('No internet')
 
-    tmp.outdata['Vector']['Point'].plot(ax=ax, column='data')
+def _testdown():
+    """Continuation testing routine."""
+    import matplotlib.pyplot as plt
+    from pygmi.pfmod.grvmag3d import quick_model, calc_field
+    from IPython import get_ipython
+    get_ipython().run_line_magic('matplotlib', 'inline')
+
+    h = 4
+    dxy = 1
+    magcalc = True
+
+    # quick model
+    lmod = quick_model(numx=100, numy=100, numz=10, dxy=dxy, d_z=1)
+    lmod.lith_index[45:55, :, 1] = 1
+    lmod.lith_index[45:50, :, 0] = 1
+    lmod.ght = 10
+    lmod.mht = 10
+    calc_field(lmod, magcalc=magcalc)
+    if magcalc:
+        z = lmod.griddata['Calculated Magnetics']
+        z.data = z.data + 5
+    else:
+        z = lmod.griddata['Calculated Gravity']
+
+    # Calculate the field
+    lmod = quick_model(numx=100, numy=100, numz=10, dxy=dxy, d_z=1)
+    lmod.lith_index[45:55, :, 1] = 1
+    lmod.lith_index[45:50, :, 0] = 1
+    lmod.ght = 10 - h
+    lmod.mht = 10 - h
+    calc_field(lmod, magcalc=magcalc)
+    if magcalc:
+        downz0 = lmod.griddata['Calculated Magnetics']
+        downz0.data = downz0.data + 5
+    else:
+        downz0 = lmod.griddata['Calculated Gravity']
+
+    downz0, z = z, downz0
+
+    dz = verticalp(z, order=1)
+    dz2 = verticalp(z, order=2)
+    dz3 = verticalp(z, order=3)
+
+    # normal downward
+    zdownn = fftcont(z, h)
+
+    # downward, taylor
+    h = -h
+    zdown = (z.data + h*dz + h**2*dz2/math.factorial(2) +
+             h**3*dz3/math.factorial(3))
+
+    # Plotting
+    plt.plot(downz0.data[50], 'r.')
+    plt.plot(zdown.data[50], 'b')
+    plt.plot(zdownn.data[50], 'k')
     plt.show()
 
 
-def _testfn():
-    """Test routine."""
+def _testfft():
+    """Test FFT."""
     import matplotlib.pyplot as plt
+    from matplotlib import colormaps
+    import scipy
+    from IPython import get_ipython
+    from pygmi.raster.iodefs import get_raster
+
+    get_ipython().run_line_magic('matplotlib', 'inline')
+
+    ifile = r'D:\Workdata\geothermal\bushveldrtp.hdr'
+    data = get_raster(ifile)[0]
+
+    # quick model
+    plt.imshow(data.data, cmap=colormaps['jet'], vmin=-500, vmax=500)
+    plt.colorbar()
+    plt.show()
 
-    extscene = None
+    # Start new stuff
+    xdim = data.xdim
+    ydim = data.ydim
 
-    ifile = r"D:/Workdata/PyGMI Test Data/Remote Sensing/Import/ASTER/AST_09T_00309042002082052_20200518022902_19756.zip"
-    ifile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\ASTER\AG100.v003.-27.022.0001.h5"
+    ndat, rdiff, cdiff, datamedian = fftprep(data)
 
-    dat = get_data(ifile, extscene=extscene)
+    datamedian = np.ma.median(data.data)
+    ndat = data.data - datamedian
 
-    for i in dat[:1]:
-        plt.figure(dpi=300)
-        plt.title(i.dataid)
-        plt.imshow(i.data, interpolation='none')
-        plt.colorbar()
-        plt.show()
+    fftmod = np.fft.fft2(ndat)
 
+    KX, KY = fft_getkxy(fftmod, xdim, ydim)
 
-def _testfn2():
-    """Test routine."""
-    import sys
+    vmin = fftmod.real.mean()-2*fftmod.real.std()
+    vmax = fftmod.real.mean()+2*fftmod.real.std()
+    plt.imshow(np.fft.fftshift(fftmod.real), vmin=vmin, vmax=vmax)
+    plt.show()
 
-    idir = r'e:\WorkProjects\ST-2022-1355 Onshore Mapping\Niger\sentinel_2\full'
+    knrm = np.sqrt(KX**2+KY**2)
 
-    app = QtWidgets.QApplication(sys.argv)
+    plt.imshow(knrm)
 
-    tmp1 = ImportBatch()
-    tmp1.idir = idir
-    tmp1.settings(True)
+    plt.show()
 
-    dat = tmp1.outdata
+    knrm = knrm.flatten()
+    fftamp = np.abs(fftmod)**2
+    fftamp = fftamp.flatten()
 
-    tmp2 = ExportBatch()
-    tmp2.indata = dat
-    tmp2.run()
+    plt.plot(knrm, fftamp, '.')
+    plt.yscale('log')
+    plt.show()
 
+    bins = max(fftmod.shape)//2
+
+    abins, bedge, _ = scipy.stats.binned_statistic(knrm, fftamp,
+                                                   statistic='mean',
+                                                   bins=bins)
+
+    bins = (bedge[:-1] + bedge[1:])/2
+    plt.plot(bins, abins)
+    plt.yscale('log')
+    plt.show()
 
-def _testfn3():
-    """Test routine."""
-    idir = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\WV2-2019"
 
-    ifiles = glob.glob(idir+'//**/*.xml', recursive=True)
+def _testcut():
+    """Test Reprojection."""
+    from pygmi.raster.iodefs import get_raster, export_raster
 
-    ifiles = [i for i in ifiles if 'aux' not in i]
-    ifiles = [i for i in ifiles if 'MUL' in i]
+    sfile = r"D:\WC\Provinces_utm34.shp"
+    ifile = r"D:\WC\ASTER\Original_data\AST_05_07XT_20060411_15908_stack.tif"
+    ofile = r"D:\WC\ASTER\Original_data\AST_05_07XT_20060411_15908_stack_cut.tif"
 
-    for ifile in ifiles:
-        print(os.path.basename(ifile))
-        ofile = os.path.basename(ifile)[:-4]+'.tif'
-        ofile = os.path.join(idir, ofile)
+    dat = get_raster(ifile)
 
-        if os.path.exists(ofile):
-            continue
+    dat = cut_raster(dat, sfile, deepcopy=False)
 
-        dat = get_data(ifile, extscene='WorldView')
-        export_raster(ofile, dat, compression='ZSTD')
+    export_raster(ofile, dat, compression='DEFLATE')
 
 
 if __name__ == "__main__":
-    _test5P()
+    _testcut()
```

### Comparing `pygmi-3.2.6.5/pygmi/rsense/landsat_composite.py` & `pygmi-3.2.7.16/pygmi/rsense/landsat_composite.py`

 * *Files 21% similar despite different names*

```diff
@@ -111,30 +111,31 @@
         """
         if not nodialog:
             tmp = self.exec_()
             if tmp != 1:
                 return False
 
         if self.idir == '':
-            self.showprocesslog('Error: No input directory')
+            self.showlog('Error: No input directory')
             return False
 
         os.chdir(self.idir)
 
         ifiles = glob.glob(os.path.join(self.idir, '**/*MTL.txt'),
                            recursive=True)
 
         if not ifiles:
             QtWidgets.QMessageBox.warning(self.parent, 'Error',
-                                          'No *MTL.txt in the directory.',
+                                          'No *MTL.txt in the directory or '
+                                          'subdirectories.',
                                           QtWidgets.QMessageBox.Ok)
             return False
 
         mean = self.tday.value()
-        dat = composite(self.idir, 10, pprint=self.showprocesslog,
+        dat = composite(self.idir, 10, showlog=self.showlog,
                         piter=self.piter, mean=mean)
 
         self.outdata['Raster'] = dat
 
         return True
 
     def get_idir(self):
@@ -155,30 +156,30 @@
             self.idir = None
             return
 
         ifiles = glob.glob(os.path.join(self.idir, '**/*MTL.txt'),
                            recursive=True)
 
         if not ifiles:
-            self.showprocesslog('Error: No *MTL.txt in the directory.')
+            self.showlog('Error: No *MTL.txt in the directory.')
             return
 
         allday = []
         for ifile in ifiles:
             sdate = os.path.basename(ifile).split('_')[3]
             sdate = datetime.strptime(sdate, '%Y%m%d')
             datday = sdate.timetuple().tm_yday
             allday.append(datday)
-            self.showprocesslog(f'Scene name: {os.path.basename(ifile)}')
-            self.showprocesslog(f'Scene day of year: {datday}')
+            self.showlog(f'Scene name: {os.path.basename(ifile)}')
+            self.showlog(f'Scene day of year: {datday}')
 
         allday = np.array(allday)
         mean = int(allday.mean())
 
-        self.showprocesslog(f'Mean day: {mean}')
+        self.showlog(f'Mean day: {mean}')
 
         self.tday.setValue(mean)
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
@@ -212,28 +213,28 @@
         projdata = {}
 
         projdata['idir'] = self.idir
 
         return projdata
 
 
-def composite(idir, dreq=10, mean=None, pprint=print, piter=None):
+def composite(idir, dreq=10, mean=None, showlog=print, piter=None):
     """
     Create a Landsat composite.
 
     Parameters
     ----------
     idir : str
         Input directory.
     dreq : int, optional
         Distance to cloud in pixels. The default is 10.
     mean : float, optional
         The mean or target day. If not specified, it is calculated
         automatically. The default is None.
-    pprint : function, optional
+    showlog : function, optional
         Function for printing text. The default is print.
     piter : iter, optional
         Progress bar iterable. The default is None.
 
     Returns
     -------
     datfin : list
@@ -253,26 +254,26 @@
 
     allday = np.array(allday)
     if mean is None:
         mean = allday.mean()
     std = allday.std()
 
     dat1 = import_and_score(ifiles[0], dreq, mean, std, piter=piter,
-                            pprint=pprint)
+                            showlog=showlog)
 
     for ifile in ifiles[1:]:
         dat2 = import_and_score(ifile, dreq, mean, std, piter=piter,
-                                pprint=pprint)
+                                showlog=showlog)
 
         tmp1 = {}
         tmp2 = {}
 
         for band in dat1:
             tmp1[band], tmp2[band] = lstack([dat1[band], dat2[band]],
-                                            pprint=pprint, piter=piter)
+                                            showlog=showlog, piter=piter)
 
         filt = (tmp1['score'].data < tmp2['score'].data)
 
         for band in tmp1:
             tmp1[band].data[filt] = tmp2[band].data[filt]
 
         dat1 = tmp1
@@ -283,36 +284,36 @@
     datfin = []
 
     del dat1['score']
     for key, data in dat1.items():
         datfin.append(data)
         datfin[-1].dataid = key
 
-    pprint(f'Range of days for scenes: {allday}')
-    pprint(f'Mean day {mean}')
-    pprint(f'Standard deviation {std:.2f}')
+    showlog(f'Range of days for scenes: {allday}')
+    showlog(f'Mean day {mean}')
+    showlog(f'Standard deviation {std:.2f}')
 
     return datfin
 
 
-def import_and_score(ifile, dreq, mean, std, pprint=print, piter=None):
+def import_and_score(ifile, dreq, mean, std, showlog=print, piter=None):
     """
     Import data and score it.
 
     Parameters
     ----------
     ifile : str
         Input filename.
     dreq : int, optional
         Distance to cloud in pixels. The default is 10.
     mean : float
         The mean or target day.
     std : float
         The standard deviation of all days.
-    pprint : function, optional
+    showlog : function, optional
         Function for printing text. The default is print.
     piter : iter, optional
         Progress bar iterable. The default is None.
 
     Returns
     -------
     dat : dictionary.
@@ -321,15 +322,15 @@
     """
     if piter is None:
         piter = ProgressBarText().iter
 
     bands = [f'B{i+1}' for i in range(11)]
 
     dat = {}
-    tmp = get_data(ifile, alldata=True, piter=piter, showprocesslog=pprint)
+    tmp = get_data(ifile, piter=piter, showlog=showlog)
 
     for i in tmp:
         if i.dataid in bands:
             i.data = i.data.astype(np.float32)
             dat[i.dataid] = i
         if 'ST_CDIST' in i.dataid:
             dat['cdist'] = i
@@ -353,16 +354,16 @@
     cdistscore.nodata = 0
 
     dayscore = (1/(std*np.sqrt(2*np.pi)) *
                 np.exp(-0.5*((datday-mean)/std)**2))
     dat['score'] = cdistscore
     dat['score'].data += dayscore
 
-    pprint(f'Scene name: {os.path.basename(ifile)}')
-    pprint(f'Scene day of year: {datday}')
+    showlog(f'Scene name: {os.path.basename(ifile)}')
+    showlog(f'Scene day of year: {datday}')
 
     filt = (dat['cdist'].data == 0)
     for data in dat.values():
         data.data[filt] = 0
         data.data = np.ma.masked_equal(data.data, 0)
 
     del dat['cdist']
```

### Comparing `pygmi-3.2.6.5/pygmi/rsense/menu.py` & `pygmi-3.2.7.16/pygmi/rsense/menu.py`

 * *Files 19% similar despite different names*

```diff
@@ -53,58 +53,24 @@
         self.parent.add_to_context('RasterFileList')
         context_menu = self.parent.context_menu
 
         # Normal menus
         self.menu = QtWidgets.QMenu('Remote Sensing')
         parent.menubar.addAction(self.menu.menuAction())
 
-        self.menu3 = self.menu.addMenu('Import Data')
-
-        self.action_import_aster = QtWidgets.QAction('Import ASTER')
-        self.menu3.addAction(self.action_import_aster)
-        self.action_import_aster.triggered.connect(self.import_aster)
-
-        self.action_import_landsat = QtWidgets.QAction('Import Landsat 4 to 9')
-        self.menu3.addAction(self.action_import_landsat)
-        self.action_import_landsat.triggered.connect(self.import_landsat)
-
-        self.action_import_sentinel2 = QtWidgets.QAction('Import Sentinel-2')
-        self.menu3.addAction(self.action_import_sentinel2)
-        self.action_import_sentinel2.triggered.connect(self.import_sentinel2)
-
-        self.action_import_sentinel2b = QtWidgets.QAction('Import Sentinel-2 '
-                                                          '(bands only)')
-        self.menu3.addAction(self.action_import_sentinel2b)
-        self.action_import_sentinel2b.triggered.connect(self.import_sentinel2b)
+        self.action_import_sat = QtWidgets.QAction('Import Satellite Data')
+        self.menu.addAction(self.action_import_sat)
+        self.action_import_sat.triggered.connect(self.import_sat)
 
         self.action_import_sentinel5p = QtWidgets.QAction('Import Sentinel-5P')
-        self.menu3.addAction(self.action_import_sentinel5p)
+        self.menu.addAction(self.action_import_sentinel5p)
         self.action_import_sentinel5p.triggered.connect(self.import_sentinel5p)
 
-        self.action_import_modis = QtWidgets.QAction('Import MODIS v6')
-        self.menu3.addAction(self.action_import_modis)
-        self.action_import_modis.triggered.connect(self.import_modis)
-
-        self.action_import_hyperion = QtWidgets.QAction('Import Hyperion L1T')
-        self.menu3.addAction(self.action_import_hyperion)
-        self.action_import_hyperion.triggered.connect(self.import_hyperion)
-
-        self.action_import_wv = QtWidgets.QAction('Import WorldView Tiles')
-        self.menu3.addAction(self.action_import_wv)
-        self.action_import_wv.triggered.connect(self.import_wv)
-
-        self.action_import_ged = QtWidgets.QAction('Import ASTER Global '
-                                                   'Emissivity Database')
-        self.menu3.addAction(self.action_import_ged)
-        self.action_import_ged.triggered.connect(self.import_ged)
-
-        self.menu3.addSeparator()
-
         self.action_batch_list = QtWidgets.QAction('Create Batch List')
-        self.menu3.addAction(self.action_batch_list)
+        self.menu.addAction(self.action_batch_list)
         self.action_batch_list.triggered.connect(self.batch_list)
 
         self.menu.addSeparator()
 
         self.action_calc_ratios = QtWidgets.QAction('Calculate Band Ratios')
         self.menu.addAction(self.action_calc_ratios)
         self.action_calc_ratios.triggered.connect(self.calc_ratios)
@@ -135,27 +101,27 @@
 
         self.action_proc_features = QtWidgets.QAction('Process Features')
         self.menu4.addAction(self.action_proc_features)
         self.action_proc_features.triggered.connect(self.proc_features)
 
         self.menu.addSeparator()
 
-        self.menu2 = self.menu.addMenu('Change Detection')
+        # self.menu2 = self.menu.addMenu('Change Detection')
 
-        self.action_create_list = QtWidgets.QAction('Create Scene List ')
-        self.menu2.addAction(self.action_create_list)
-        self.action_create_list.triggered.connect(self.create_scene)
-
-        self.action_load_list = QtWidgets.QAction('Load Scene List')
-        self.menu2.addAction(self.action_load_list)
-        self.action_load_list.triggered.connect(self.load_scene)
-
-        self.action_data_viewer = QtWidgets.QAction('View Change Data')
-        self.menu2.addAction(self.action_data_viewer)
-        self.action_data_viewer.triggered.connect(self.view_change)
+        # self.action_create_list = QtWidgets.QAction('Create Scene List ')
+        # self.menu2.addAction(self.action_create_list)
+        # self.action_create_list.triggered.connect(self.create_scene)
+
+        # self.action_load_list = QtWidgets.QAction('Load Scene List')
+        # self.menu2.addAction(self.action_load_list)
+        # self.action_load_list.triggered.connect(self.load_scene)
+
+        # self.action_data_viewer = QtWidgets.QAction('View Change Data')
+        # self.menu2.addAction(self.action_data_viewer)
+        # self.action_data_viewer.triggered.connect(self.view_change)
 
         # Context menus
         context_menu['RasterFileList'].addSeparator()
 
         self.action_exportlist = QtWidgets.QAction('Export Raster File List')
         context_menu['RasterFileList'].addAction(self.action_exportlist)
         self.action_exportlist.triggered.connect(self.exportlist)
@@ -214,51 +180,14 @@
                                 hyperspec.ProcFeatures)
 
     def import_sentinel5p(self):
         """Import Sentinel 5P data."""
         self.parent.item_insert('Io', 'Import Sentinel-5P',
                                 iodefs.ImportSentinel5P)
 
-    def import_sentinel2(self):
-        """Import Sentinel 2 data."""
-        self.parent.item_insert('Io', 'Import Sentinel-2', iodefs.ImportData,
-                                extscene='Sentinel-2 (*.xml *.zip);;')
-
-    def import_sentinel2b(self):
-        """Import Sentinel 2 data, bands only."""
-        self.parent.item_insert('Io', 'Import Sentinel-2', iodefs.ImportData,
-                                extscene='Sentinel-2 Bands Only (*.xml *.zip);;')
-
-    def import_modis(self):
-        """Import MODIS data."""
-        self.parent.item_insert('Io', 'Import MODIS v6', iodefs.ImportData,
-                                extscene='MODIS (*.hdf);;')
-
-    def import_aster(self):
-        """Import ASTER HDF data."""
-        self.parent.item_insert('Io', 'Import ASTER', iodefs.ImportData,
-                                extscene='ASTER (AST*.hdf AST*.zip);;')
-
-    def import_ged(self):
-        """Import HDF data."""
-        self.parent.item_insert('Io', 'Import ASTER Global Emissivity Data',
-                                iodefs.ImportData,
-                                extscene='h5 (*.h5);;')
-
-    def import_landsat(self):
-        """Import Landsat data."""
-        self.parent.item_insert('Io', 'Import Landsat', iodefs.ImportData,
-                                extscene='Landsat (L*.tar L*.tar.gz L*_MTL.txt);;')
-
-    def import_hyperion(self):
-        """Import Hyperion data."""
-        self.parent.item_insert('Io', 'Import Hyperion L1T', iodefs.ImportData,
-                                extscene='Hyperion L1T (*.zip);;')
-
-    def import_wv(self):
-        """Import WorldView data."""
-        self.parent.item_insert('Io', 'Import WorldView', iodefs.ImportData,
-                                extscene='WorldView (*.xml);;')
+    def import_sat(self):
+        """Import Satellite data."""
+        self.parent.item_insert('Io', 'Import Satellite', iodefs.ImportData)
 
     def batch_list(self):
         """Import batch list."""
         self.parent.item_insert('Io', 'Import Batch List', iodefs.ImportBatch)
```

### Comparing `pygmi-3.2.6.5/pygmi/rsense/ratios.py` & `pygmi-3.2.7.16/pygmi/rsense/ratios.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import sys
 import re
 import numexpr as ne
 import numpy as np
 from PyQt5 import QtWidgets, QtCore
 
 from pygmi import menu_default
-from pygmi.rsense import iodefs
+from pygmi.rsense.iodefs import get_from_rastermeta, set_export_filename
 from pygmi.raster.iodefs import export_raster
 from pygmi.raster.dataprep import lstack
 from pygmi.misc import BasicModule
 
 
 class SatRatios(BasicModule):
     """Calculate Satellite Ratios."""
@@ -68,15 +68,15 @@
 
         self.lw_ratios.setSelectionMode(self.lw_ratios.MultiSelection)
 
         self.combo_sensor.addItems(['ASTER',
                                     'Landsat 8 and 9 (OLI)',
                                     'Landsat 7 (ETM+)',
                                     'Landsat 4 and 5 (TM)',
-                                    'Sentinel-2', 'WorldView'])
+                                    'Sentinel-2', 'WorldView', 'Unknown'])
         buttonbox.setOrientation(QtCore.Qt.Horizontal)
         buttonbox.setCenterButtons(True)
         buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
 
         self.setWindowTitle('Band Ratio Calculations')
 
         gridlayout_main.addWidget(label_sensor, 0, 0, 1, 1)
@@ -107,32 +107,38 @@
         -------
         bool
             True if successful, False otherwise.
 
         """
         tmp = []
         if 'Raster' not in self.indata and 'RasterFileList' not in self.indata:
-            self.showprocesslog('No Satellite Data')
+            self.showlog('No Satellite Data')
             return False
 
         if 'RasterFileList' in self.indata:
-            bfile = os.path.basename(self.indata['RasterFileList'][0])
+            dat = self.indata['RasterFileList']
+            instr = dat[0].sensor
         else:
-            bfile = os.path.basename(self.indata['Raster'][0].filename)
+            dat = self.indata['Raster']
+            instr = dat[0].metadata['Raster']['Sensor']
 
-        if 'AST_' in bfile and 'hdf' in bfile.lower():
+        if 'ASTER' in instr:
             self.combo_sensor.setCurrentText('ASTER')
-        elif bfile[:4] in ['LC08', 'LC09']:
+        elif 'LC08' in instr or 'LC09' in instr:
             self.combo_sensor.setCurrentText('Landsat 8 and 9 (OLI)')
-        elif bfile[:4] in ['LE07']:
+        elif 'LE07' in instr:
             self.combo_sensor.setCurrentText('Landsat 7 (ETM+)')
-        elif bfile[:4] in ['LT04', 'LT05']:
+        elif 'LT04' in instr or 'LT05' in instr:
             self.combo_sensor.setCurrentText('Landsat 4 and 5 (TM)')
-        else:
+        elif 'WorldView' in instr and 'Multi' in instr:
+            self.combo_sensor.setCurrentText('WorldView')
+        elif 'Sentinel-2' in instr:
             self.combo_sensor.setCurrentText('Sentinel-2')
+        else:
+            self.combo_sensor.setCurrentText('Unknown')
 
         self.setratios()
 
         if not nodialog:
             tmp = self.exec_()
         else:
             tmp = 1
@@ -197,183 +203,75 @@
         Updates self.outdata, which is used as input to other modules.
 
         Returns
         -------
         None.
 
         """
-        datfin = []
         sensor = self.combo_sensor.currentText()
 
+        rlist = []
+        for i in self.lw_ratios.selectedItems():
+            rlist.append(i.text()[2:])
+
+        if 'RasterFileList' in self.indata:
+            data = self.indata['RasterFileList']
+        else:
+            data = self.indata['Raster']
+
         if 'RasterFileList' in self.indata:
             flist = self.indata['RasterFileList']
             if sensor == 'ASTER':
                 flist = get_aster_list(flist)
             elif 'Landsat' in sensor:
                 flist = get_landsat_list(flist, sensor)
             elif 'Sentinel-2' in sensor:
                 flist = get_sentinel_list(flist)
             if not flist:
-                self.showprocesslog('Warning: This might not be ' + sensor +
-                                    ' data. Will attempt to do calculation '
-                                    'anyway.')
+                self.showlog('Warning: This might not be ' + sensor +
+                             ' data. Will attempt to do calculation '
+                             'anyway.')
                 flist = self.indata['RasterFileList']
         else:
             flist = [self.indata['Raster']]
 
         rlist = []
         for i in self.lw_ratios.selectedItems():
             rlist.append(i.text()[2:])
 
         if not rlist:
-            self.showprocesslog('You need to select a ratio to calculate.')
+            self.showlog('You need to select a ratio to calculate.')
             return False
 
         for ifile in flist:
-            if isinstance(ifile, str):
-                dat = iodefs.get_data(ifile,
-                                      showprocesslog=self.showprocesslog,
-                                      piter=self.piter)
-                ofile = ifile
-            elif isinstance(ifile, list) and 'RasterFileList' in self.indata:
-                dat = []
-                for jfile in ifile:
-                    dat += iodefs.get_data(jfile,
-                                           showprocesslog=self.showprocesslog,
-                                           piter=self.piter)
-                ofile = ifile[-1]
+            if 'RasterFileList' in self.indata:
+                dat = get_from_rastermeta(ifile, piter=self.piter,
+                                          showlog=self.showlog)
             else:
                 dat = ifile
-                ofile = dat[0].filename
 
             if dat is None:
                 continue
 
-            datsml = []
-
-            if sensor == 'WorldView':
-                wvlabels = {'CoastalBlue': 'B1',
-                            'Blue': 'B2',
-                            'Green': 'B3',
-                            'Yellow': 'B4',
-                            'Red': 'B5',
-                            'RedEdge': 'B6',
-                            'NIR1': 'B7',
-                            'NIR2': 'B8'}
-                for i in dat:
-                    if i.dataid.split()[0] in wvlabels:
-                        i.dataid = wvlabels[i.dataid.split()[0]]
-
-            for i in dat:
-                tmp = i.dataid.split()
-                txt = tmp[0]
-
-                if 'Band' not in txt and 'B' in txt:
-                    txt = txt.replace('B', 'Band')
-
-                if 'Band' not in txt and 'LST' not in txt:
-                    continue
-
-                formula = ','.join(rlist)
-                formula = re.sub(r'B(\d+)', r'Band\1', formula)
-
-                if txt in formula:
-                    datsml.append(i)
-
-            dat = lstack(datsml, piter=self.piter, pprint=self.showprocesslog)
-
-            del flist
-            del ifile
-            del datsml
-            # del self.indata['Raster']
-
-            datd = {}
-            newmask = None
-            for i in dat:
-                tmp = i.dataid.split()
-                txt = tmp[0]
-                if txt == 'Band':
-                    txt = tmp[0]+tmp[1]
-
-                if 'Band' not in txt and 'B' in txt and ',' in txt:
-                    txt = txt.replace('B', 'Band')
-                    txt = txt.replace(',', '')
-
-                if 'Band' not in txt and 'B' in txt:
-                    txt = txt.replace('B', 'Band')
-
-                if txt == 'Band3N':
-                    txt = 'Band3'
-
-                datd[txt] = i.data
-
-            datfin = []
-            for i in self.piter(rlist):
-                self.showprocesslog('Calculating '+i)
-                formula = i.split(' ')[0]
-                formula = re.sub(r'B(\d+)', r'Band\1', formula)
-                blist = formula
-                for j in ['/', '*', '+', '-', '(', ')']:
-                    blist = blist.replace(j, ' ')
-                blist = blist.split()
-                blist = list(set(blist))
-                blist = [i for i in blist if 'Band' in i]
-
-                abort = []
-                for j in blist:
-                    if 'B' not in j:
-                        continue
-                    if j not in datd:
-                        abort.append(j)
-                if abort:
-                    self.showprocesslog('Error: '+' '.join(abort)+' missing.')
-                    continue
-
-                newmask = datd[blist[0]].mask
-                for j in blist:
-                    newmask = (newmask | datd[j].mask)
-
-                if len(formula.split(r'/')) == 2:
-                    f1, f2 = formula.split(r'/')
-                    a1 = ne.evaluate(f1, datd)
-                    a1 = a1.astype(np.float32)
-                    a2 = ne.evaluate(f2, datd)
-                    a2 = a2.astype(np.float32)
-
-                    # del datd
-
-                    a2[np.isclose(a2, 0.)] = 0.
-                    ratio = a1/a2
-
-                    del a1
-                    del a2
-                else:
-                    ratio = ne.evaluate(formula, datd)
+            odir = os.path.dirname(dat[0].filename)
 
-                ratio = ratio.astype(np.float32)
-                ratio[newmask] = dat[0].nodata
-                ratio = np.ma.array(ratio, mask=newmask,
-                                    fill_value=dat[0].nodata)
+            datfin = calc_ratios(dat, rlist, showlog=self.showlog,
+                                 piter=self.piter, sensor=sensor)
 
-                ratio = np.ma.fix_invalid(ratio)
+            if datfin:
+                odir = os.path.dirname(data[0].filename)
+                odir = os.path.join(odir, 'ratios')
 
-                rband = copy.deepcopy(dat[0])
-                rband.data = ratio
-                rband.dataid = i.replace(r'/', 'div')
-                datfin.append(rband)
+                os.makedirs(odir, exist_ok=True)
 
-            if datfin:
-                if len(datfin) == 1:
-                    ofile = (ofile.split('.')[0] + '_' +
-                             datfin[0].dataid.partition(' ')[-1] + '.tif')
-                else:
-                    ofile = ofile.split('.')[0] + '_ratio.tif'
+                ofile = set_export_filename(dat, odir, 'ratio')
 
-                self.showprocesslog('Exporting to '+ofile)
-                export_raster(ofile, datfin, 'GTiff', piter=self.piter)
+                self.showlog('Exporting to '+ofile)
+                export_raster(ofile, datfin, 'GTiff', piter=self.piter,
+                              compression='DEFLATE', showlog=self.showlog)
                 self.outdata['Raster'] = datfin
 
         return True
 
     def setratios(self):
         """
         Set the available ratios.
@@ -427,23 +325,28 @@
         # Other
         rlist += [r'B3/B2 Vegetation',
                   r'(B3-B2)/(B3+B2) NDVI',
                   r'(B3-B4)/(B3+B4) NDWI/NDMI water in leaves',
                   r'(B1-B3)/(B1+B3) NDWI water bodies',
                   r'2.5*(B3-B2)/(B3+6.0*B2-7.5*B0+1) EVI',
                   r'0.5*(2*B3+1-sqrt((2*B3+1)**2-8*(B3-B2))) MSAVI2',
-                  r'(B3A-B4+B5)/(B3A+B4-B5) NMDI']
+                  r'(B3A-B4+B5)/(B3A+B4-B5) NMDI',
+                  r'((B4+B2)-(B3+B0))/((B4+B2)+(B3+B0)) BSI']
 
         # Colour composite
 
         rlist += [r'B5/B3 Used in colour composites',
                   r'B4/B0 Used in colour composites',
                   r'B5/B1 Used in colour composites',
                   r'B4/B7 Used in colour composites']
 
+        # Landslides
+
+        rlist += ['B0,B1,B2,B3,B4 Landslide Index']
+
         rlist2 = correct_bands(rlist, sensor)
 
         self.lw_ratios.clear()
         self.lw_ratios.addItems(rlist2)
 
         for i in range(self.lw_ratios.count()):
             item = self.lw_ratios.item(i)
@@ -520,15 +423,15 @@
                                    'MSAVI2'])
 
         self.combo_sensor.addItems(['ASTER',
                                     'Landsat 8 and 9 (OLI)',
                                     'Landsat 7 (ETM+)',
                                     'Landsat 4 and 5 (TM)',
                                     'Landsat (All)',
-                                    'Sentinel-2', 'WorldView'])
+                                    'Sentinel-2', 'WorldView', 'Unknown'])
 
         buttonbox.setOrientation(QtCore.Qt.Horizontal)
         buttonbox.setCenterButtons(True)
         buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
 
         self.setWindowTitle('Condition Indices Calculations')
 
@@ -562,33 +465,43 @@
         -------
         bool
             True if successful, False otherwise.
 
         """
         tmp = []
         if 'RasterFileList' not in self.indata:
-            self.showprocesslog('You need a raster file list as input.')
+            self.showlog('You need a raster file list as input.')
+            return False
+
+        if len(self.indata['RasterFileList']) < 2:
+            self.showlog('You need more than one scene in your raster file '
+                         'list.')
             return False
 
-        bfile = os.path.basename(self.indata['RasterFileList'][0])
+        bfile = os.path.basename(self.indata['RasterFileList'][0].filename)
         self.bfile = bfile[:4]
 
-        if 'AST_' in bfile and 'hdf' in bfile.lower():
+        dat = self.indata['RasterFileList'][0]
+
+        instr = dat.sensor
+
+        if 'ASTER' in instr:
             self.combo_sensor.setCurrentText('ASTER')
-        elif bfile[:4] in ['LC08', 'LC09']:
+        elif 'LC08' in instr or 'LC09' in instr:
             self.combo_sensor.setCurrentText('Landsat 8 and 9 (OLI)')
-        elif bfile[:4] in ['LE07']:
+        elif 'LE07' in instr:
             self.combo_sensor.setCurrentText('Landsat 7 (ETM+)')
-        elif bfile[:4] in ['LT04', 'LT05']:
+        elif 'LT04' in instr or 'LT05' in instr:
             self.combo_sensor.setCurrentText('Landsat 4 and 5 (TM)')
-        elif ('LT04' in bfile or 'LT05' in bfile or 'LE07' in bfile or
-              'LC08' in bfile or 'LC09' in bfile):
-            self.combo_sensor.setCurrentText('Landsat (All)')
-        else:
+        elif 'WorldView' in instr and 'Multi' in instr:
+            self.combo_sensor.setCurrentText('WorldView')
+        elif 'Sentinel-2' in instr:
             self.combo_sensor.setCurrentText('Sentinel-2')
+        else:
+            self.combo_sensor.setCurrentText('Unknown')
 
         self.setratios()
 
         if not nodialog:
             tmp = self.exec_()
         else:
             tmp = 1
@@ -661,16 +574,16 @@
         sensor = self.combo_sensor.currentText()
 
         rlist1 = []
         for i in self.lw_ratios.selectedItems():
             rlist1.append(i.text()[2:])
 
         if not rlist1:
-            self.showprocesslog('You need to select a condition index to '
-                                'calculate.')
+            self.showlog('You need to select a condition index to '
+                         'calculate.')
             return False
 
         rlist2 = []
         if 'VCI' in rlist1 and 'EVI' in index:
             rlist2 += [r'2.5*(B3-B2)/(B3+6.0*B2-7.5*B0+1) EVI']
         elif 'VCI' in rlist1 and 'NDVI' in index:
             rlist2 += [r'(B3-B2)/(B3+B2) NDVI']
@@ -679,57 +592,51 @@
 
         evi = []
         tci = []
         vci = []
         vhi = []
         lst = []
 
-        if 'RasterFileList' in self.indata:
-            flist = self.indata['RasterFileList']
-            if sensor == 'ASTER':
-                flist = get_aster_list(flist)
-            elif 'Landsat' in sensor:
-                flist = get_landsat_list(flist, sensor)
-            elif 'Sentinel-2' in sensor:
-                flist = get_sentinel_list(flist)
-            if not flist:
-                self.showprocesslog('Warning: This might not be ' + sensor +
-                                    ' data. Will attempt to do calculation '
-                                    'anyway.')
-                flist = self.indata['RasterFileList']
+        flist = self.indata['RasterFileList']
+        if sensor == 'ASTER':
+            flist = get_aster_list(flist)
+        elif 'Landsat' in sensor:
+            flist = get_landsat_list(flist, sensor)
+        elif 'Sentinel-2' in sensor:
+            flist = get_sentinel_list(flist)
         else:
-            flist = [self.indata['Raster']]
+            self.showlog('Warning: This might not be ' + sensor +
+                         ' data. Will attempt to do calculation '
+                         'anyway.')
+            flist = self.indata['RasterFileList']
 
         for ifile in flist:
-            if isinstance(ifile, str):
-                dat = iodefs.get_data(ifile,
-                                      showprocesslog=self.showprocesslog,
-                                      piter=self.piter)
-            else:
-                dat = ifile
-                ifile = dat[0].filename
+            dat = get_from_rastermeta(ifile, piter=self.piter,
+                                      showlog=self.showlog)
 
             if dat is None:
                 continue
 
+            ofile = dat[0].filename
+
             # Prepare for layer stacking
             if sensor == 'WorldView':
                 wvlabels = {'CoastalBlue': 'B1',
                             'Blue': 'B2',
                             'Green': 'B3',
                             'Yellow': 'B4',
                             'Red': 'B5',
                             'RedEdge': 'B6',
                             'NIR1': 'B7',
                             'NIR2': 'B8'}
                 for i in dat:
                     if i.dataid.split()[0] in wvlabels:
                         i.dataid = wvlabels[i.dataid.split()[0]]
 
-            bfile = os.path.basename(ifile)
+            bfile = os.path.basename(ifile.filename)
             rlist = correct_bands(rlist2, sensor, bfile)
 
             datsml = []
             for i in dat:
                 txt = i.dataid.split()[0]
 
                 if 'Band' not in txt and 'B' in txt:
@@ -745,18 +652,16 @@
 
                 formula = ','.join(rlist)
                 formula = re.sub(r'B(\d+)', r'Band\1', formula)
 
                 if txt in formula:
                     datsml.append(i)
 
-            dat = lstack(datsml, piter=self.piter, pprint=self.showprocesslog)
+            dat = lstack(datsml, piter=self.piter, showlog=self.showlog)
 
-            # del flist
-            # del ifile
             del datsml
 
             # Correct band names
             datd = {}
             newmask = None
             for i in dat:
                 tmp = i.dataid.split()
@@ -776,19 +681,16 @@
 
                 datd[txt] = i.data
 
                 if 'LST' in txt:
                     lst.append(i)
 
             # Calculate ratios
-            # bfile = os.path.basename(ifile)
             for i in self.piter(rlist):
-                # i = correct_bands([i2], sensor, bfile)[0]
-
-                self.showprocesslog('Calculating '+i)
+                self.showlog('Calculating '+i)
                 formula = i.split(' ')[0]
                 formula = re.sub(r'B(\d+)', r'Band\1', formula)
                 blist = formula
                 for j in ['/', '*', '+', '-', '(', ')']:
                     blist = blist.replace(j, ' ')
                 blist = blist.split()
                 blist = list(set(blist))
@@ -797,15 +699,15 @@
                 abort = []
                 for j in blist:
                     if 'B' not in j:
                         continue
                     if j not in datd:
                         abort.append(j)
                 if abort:
-                    self.showprocesslog('Error: '+' '.join(abort)+' missing.')
+                    self.showlog('Error: '+' '.join(abort)+' missing.')
                     continue
 
                 newmask = datd[blist[0]].mask
                 for j in blist:
                     newmask = (newmask | datd[j].mask)
 
                 if len(formula.split(r'/')) == 2:
@@ -814,34 +716,32 @@
                     a2 = ne.evaluate(f2, datd)
 
                     a2[np.isclose(a2, 0.)] = 0.
                     ratio = a1/a2
                 else:
                     ratio = ne.evaluate(formula, datd)
 
-                # ratio = ne.evaluate(formula, datd)
-
                 newmask = newmask | (ratio < -1) | (ratio > 1)
                 ratio = ratio.astype(np.float32)
                 ratio[newmask] = 1e+20
                 ratio = np.ma.array(ratio, mask=newmask,
                                     fill_value=1e+20)
 
                 ratio = np.ma.fix_invalid(ratio)
 
                 tmp = copy.deepcopy(dat[0])
                 tmp.data = ratio
                 tmp.nodata = 1e+20
                 evi.append(tmp)
 
         if lst:
-            lst = lstack(lst, piter=self.piter, pprint=self.showprocesslog,
+            lst = lstack(lst, piter=self.piter, showlog=self.showlog,
                          commonmask=True)
         if evi:
-            evi = lstack(evi, piter=self.piter, pprint=self.showprocesslog,
+            evi = lstack(evi, piter=self.piter, showlog=self.showlog,
                          commonmask=True)
 
         ofile = ''
         if ('TCI' in rlist1 or 'VHI' in rlist1) and lst:
             tci = get_TCI(lst)
             ofile += '_TCI'
         if ('VCI' in rlist1 or 'VHI' in rlist1) and evi:
@@ -852,16 +752,14 @@
             ofile += '_VHI'
 
         datfin = tci+vci+vhi
 
         for i in datfin:
             i.data = i.data.astype(np.float32)
 
-        ofile = os.path.join(os.path.dirname(ifile), 'CI'+ofile+'.tif')
-
         if datfin:
             self.outdata['Raster'] = datfin
 
         return True
 
     def setratios(self):
         """
@@ -869,16 +767,18 @@
 
         Returns
         -------
         None.
 
         """
         sensor = self.combo_sensor.currentText()
+        rlist = []
 
-        rlist = ['VCI']
+        if 'Unknown' not in sensor:
+            rlist += ['VCI']
 
         if 'Landsat' in sensor:
             rlist += ['TCI', 'VHI']
 
         self.lw_ratios.clear()
         self.lw_ratios.addItems(rlist)
 
@@ -928,14 +828,144 @@
             item = self.lw_ratios.item(i)
             if item.isSelected():
                 item.setText('\u2713' + item.text()[1:])
             else:
                 item.setText(' ' + item.text()[1:])
 
 
+def calc_ratios(dat, rlist, showlog=print, piter=iter, sensor=None):
+    """
+    Calculate Band ratios.
+
+    Note that this routine assumes that the ratio you supply is correct for
+    your data.
+
+    Parameters
+    ----------
+    dat : list
+        List of PyGMI Data.
+    rlist : list
+        List of strings, containing ratios to calculate..
+    showlog : print, optional
+        Display information. The default is print.
+    piter : iter, optional
+        Progress bar iterator. The default is iter.
+
+    Returns
+    -------
+    datfin : list
+        List of PyGMI Data.
+
+    """
+    datsml = []
+
+    for i in dat:
+        tmp = i.dataid.split()
+        txt = tmp[0]
+
+        if 'Band' not in txt and 'B' in txt:
+            txt = txt.replace('B', 'Band')
+
+        if 'Band' not in txt and 'LST' not in txt:
+            continue
+
+        formula = ','.join(rlist)
+        formula = re.sub(r'B(\d+)', r'Band\1', formula)
+
+        if txt == 'Band3N':
+            txt = 'Band3'
+
+        if txt in formula:
+            datsml.append(i)
+
+    dat = lstack(datsml, piter=piter, showlog=showlog)
+
+    del datsml
+
+    datd = {}
+    newmask = None
+    for i in dat:
+        tmp = i.dataid.split()
+        txt = tmp[0]
+        if txt == 'Band':
+            txt = tmp[0]+tmp[1]
+
+        if 'Band' not in txt and 'B' in txt and ',' in txt:
+            txt = txt.replace('B', 'Band')
+            txt = txt.replace(',', '')
+
+        if 'Band' not in txt and 'B' in txt:
+            txt = txt.replace('B', 'Band')
+
+        if txt == 'Band3N':
+            txt = 'Band3'
+
+        datd[txt] = i.data
+
+    datfin = []
+    for i in piter(rlist):
+        showlog('Calculating '+i)
+        if 'Landslide Index' in i:
+            rband = landslide_index(dat, sensor, showlog, piter)
+            datfin += rband
+            continue
+
+        formula = i.split(' ')[0]
+        formula = re.sub(r'B(\d+)', r'Band\1', formula)
+        blist = formula
+        for j in ['/', '*', '+', '-', '(', ')']:
+            blist = blist.replace(j, ' ')
+        blist = blist.split()
+        blist = list(set(blist))
+        blist = [i for i in blist if 'Band' in i]
+
+        abort = []
+        for j in blist:
+            if 'B' not in j:
+                continue
+            if j not in datd:
+                abort.append(j)
+        if abort:
+            showlog('Error: '+' '.join(abort)+' missing.')
+            continue
+
+        newmask = datd[blist[0]].mask
+        for j in blist:
+            newmask = (newmask | datd[j].mask)
+
+        if len(formula.split(r'/')) == 2:
+            f1, f2 = formula.split(r'/')
+            a1 = ne.evaluate(f1, datd)
+            a1 = a1.astype(np.float32)
+            a2 = ne.evaluate(f2, datd)
+            a2 = a2.astype(np.float32)
+
+            a2[np.isclose(a2, 0.)] = 0.
+            ratio = a1/a2
+
+            del a1
+            del a2
+        else:
+            ratio = ne.evaluate(formula, datd)
+
+        ratio = ratio.astype(np.float32)
+        ratio[newmask] = dat[0].nodata
+        ratio = np.ma.array(ratio, mask=newmask,
+                            fill_value=dat[0].nodata)
+
+        ratio = np.ma.fix_invalid(ratio)
+
+        rband = copy.deepcopy(dat[0])
+        rband.data = ratio
+        rband.dataid = i.replace(r'/', 'div')
+        datfin.append(rband)
+
+    return datfin
+
+
 def correct_bands(rlist, sensor, bfile=None):
     """
     Correct the band designations.
 
     Ratio formula are defined in terms of ASTER bands. This converts that to
     the target sensor.
 
@@ -948,31 +978,35 @@
 
     Returns
     -------
     rlist2 : list
         List of converted ratios.
 
     """
+    # custom_indices = ['Landslide Index']
+
     sdict = {}
 
     sdict['ASTER'] = {'B1': 'B1', 'B2': 'B2', 'B3': 'B3', 'B4': 'B4',
+                      'B3A': 'B3',
                       'B5': 'B5', 'B6': 'B6', 'B7': 'B7', 'B8': 'B8',
                       'B9': 'B9', 'B10': 'B10', 'B11': 'B11', 'B12': 'B12',
-                      'B13': 'B13', 'B14': 'B14', 'B3A': 'B3'}
+                      'B13': 'B13', 'B14': 'B14'}
     sdict['Landsat 8 and 9 (OLI)'] = {'B0': 'B2', 'B1': 'B3', 'B2': 'B4',
                                       'B3': 'B5', 'B4': 'B6', 'B5': 'B7',
                                       'B3A': 'B5'}
     sdict['Landsat 7 (ETM+)'] = {'B0': 'B1', 'B1': 'B2', 'B2': 'B3',
                                  'B3': 'B4', 'B4': 'B5', 'B5': 'B7',
                                  'B3A': 'B4'}
     sdict['Landsat 4 and 5 (TM)'] = sdict['Landsat 7 (ETM+)']
     sdict['Sentinel-2'] = {'B0': 'B2', 'B1': 'B3', 'B2': 'B4', 'B3': 'B8',
                            'B4': 'B11', 'B5': 'B12', 'B3A': 'B8A'}
     sdict['WorldView'] = {'B0': 'B2', 'B1': 'B3', 'B2': 'B5', 'B3': 'B7',
                           'B3A': 'B7'}
+    sdict['Unknown'] = {}
 
     if sensor == 'Landsat (All)':
         if 'LC09' in bfile or 'LC08' in bfile:
             sensor = 'Landsat 8 and 9 (OLI)'
         elif 'LE07' in bfile:
             sensor = 'Landsat 7 (ETM+)'
         else:
@@ -986,19 +1020,117 @@
         formula = i.split(' ')[0]
         lbl = i[i.index(' '):]
         bands = set(re.findall(r'B\d+\w?', formula))
         if bands.issubset(svalues):
             tmp = re.sub(r'B(\d+\w?)', r'tmpB\1', formula)
             for j in svalues:
                 tmp = tmp.replace('tmp'+j, bandmap[j])
+
+            # lbl = lbl.strip()
+            # if lbl in custom_indices:
+            #     tmp = ''
+            # else:
+            #     tmp += ' '
             rlist2.append(tmp+lbl)
 
     return rlist2
 
 
+def get_aster_list(flist):
+    """
+    Get ASTER files from a file list.
+
+    Parameters
+    ----------
+    flist : list
+        List of filenames.
+
+    Returns
+    -------
+    flist : list
+        List of filenames.
+
+    """
+    flist2 = []
+    for i in flist:
+        if 'ASTER' not in i.sensor:
+            continue
+        flist2.append(i)
+
+    return flist2
+
+
+def get_landsat_list(flist, sensor=None, allsats=False):
+    """
+    Get Landsat files from a file list.
+
+    Parameters
+    ----------
+    flist : list
+        List of filenames.
+
+    Returns
+    -------
+    flist : list
+        List of filenames.
+
+    """
+    if isinstance(flist[0], list):
+        bfile = os.path.basename(flist[0][0].filename)
+        if bfile[:4] in ['LT04', 'LT05', 'LE07', 'LC08', 'LC09']:
+            return flist
+        return []
+
+    if allsats is True or sensor is None:
+        fid = ['LT04', 'LT05', 'LE07', 'LC08', 'LC09']
+    elif sensor == 'Landsat 8 and 9 (OLI)':
+        fid = ['LC08', 'LC09']
+    elif sensor == 'Landsat 7 (ETM+)':
+        fid = ['LE07']
+    elif sensor == 'Landsat 4 and 5 (TM)':
+        fid = ['LT04', 'LT05']
+    else:
+        return None
+
+    flist2 = []
+    for i in flist:
+        for j in fid:
+            if j not in i.sensor:
+                continue
+            if '.tif' in i.filename:
+                continue
+            flist2.append(i)
+
+    return flist2
+
+
+def get_sentinel_list(flist):
+    """
+    Get Sentinel-2 files from a file list.
+
+    Parameters
+    ----------
+    flist : list
+        List of filenames.
+
+    Returns
+    -------
+    flist : list
+        List of filenames.
+
+    """
+    flist2 = []
+    for i in flist:
+        if 'Sentinel-2' not in i.sensor:
+            continue
+        flist2.append(i)
+
+    return flist2
+
+
 def get_TCI(lst):
     """
     Calculate TCI.
 
     Parameters
     ----------
     lst : list
@@ -1097,253 +1229,142 @@
                 tmp.dataid = os.path.basename(tci1.filename)[:-4]+'_VHI'
 
                 vhi.append(tmp)
 
     return vhi
 
 
-def get_aster_list(flist):
-    """
-    Get ASTER files from a file list.
-
-    Parameters
-    ----------
-    flist : list
-        List of filenames.
-
-    Returns
-    -------
-    flist : list
-        List of filenames.
-
+def landslide_index(dat, sensor=None, showlog=print, piter=iter):
     """
-    if isinstance(flist[0], list):
-        if 'AST_' in flist[0][0].filename:
-            return flist
-        return []
-
-    names = {}
-    for i in flist:
-        if os.path.basename(i)[:3] != 'AST':
-            continue
-
-        adate = os.path.basename(i).split('_')[2]
-        if adate not in names:
-            names[adate] = []
-        names[adate].append(i)
-
-    for adate in names.keys():
-        has_07xt = [True for i in names[adate] if '_07XT_' in i]
-        has_07 = [True for i in names[adate] if '_07_' in i]
-        if len(has_07xt) > 0 and len(has_07) > 0:
-            names[adate] = [i for i in names[adate] if '_07_' not in i]
-
-    flist = []
-    for adate in names:
-        flist.append(names[adate])
-
-    return flist
-
+    Calculate Band ratios.
 
-def get_landsat_list(flist, sensor, allsats=False):
-    """
-    Get Landsat files from a file list.
+    Note that this routine assumes that the ratio you supply is correct for
+    your data.
 
     Parameters
     ----------
-    flist : list
-        List of filenames.
+    dat : list
+        List of PyGMI Data.
+    showlog : print, optional
+        Display information. The default is print.
+    piter : iter, optional
+        Progress bar iterator. The default is iter.
 
     Returns
     -------
-    flist : list
-        List of filenames.
+    datfin : list
+        Red, green and blue PyGMI Data.
 
     """
-    if isinstance(flist[0], list):
-        bfile = os.path.basename(flist[0][0].filename)
-        if bfile[:4] in ['LT04', 'LT05', 'LE07', 'LC08', 'LC09']:
-            return flist
-        return []
+    rlist = [r'(B3-B2)/(B3+B2) NDVI',
+             r'(B1-B3)/(B1+B3) NDWI water bodies',
+             r'B4 SWIR',
+             r'((B4+B2)-(B3+B0))/((B4+B2)+(B3+B0)) BSI']
+
+    if sensor is None:
+        sensor = dat[0].metadata['Raster']['Sensor']
+    rlist = correct_bands(rlist, sensor)
+
+    datfin = calc_ratios(dat, rlist, showlog=showlog, piter=piter)
+
+    for i in datfin:
+        if 'NDVI' in i.dataid:
+            NDVI = i.data
+        elif 'NDWI' in i.dataid:
+            NDWI = i.data
+        elif 'SWIR' in i.dataid:
+            SWIR = i.data
+        elif 'BSI' in i.dataid:
+            BSI = i.data
+
+    red = copy.deepcopy(dat[0])
+    green = copy.deepcopy(dat[0])
+    blue = copy.deepcopy(dat[0])
+
+    red.data[:] = 3.5*BSI
+    green.data[:] = 0.3
+    blue.data[:] = 0.
+
+    filt = ((SWIR > 0.8) | (NDVI < 0.15))
+    red.data[filt] = 1.5
+    green.data[filt] = 0.7
+    blue.data[filt] = -1.
+
+    filt = (NDVI > 0.25)
+    red.data[filt] = 0.
+    green.data[filt] = 0.2*NDVI[filt]
+    blue.data[filt] = 0.
+
+    filt = (NDWI > 0.15)
+    red.data[filt] = 0.
+    green.data[filt] = 0.2
+    blue.data[filt] = NDWI[filt]
+
+    red.dataid = 'Landslide Index Red'
+    green.dataid = 'Landslide Index Green'
+    blue.dataid = 'Landslide Index Blue'
+
+    red.data = np.ma.masked_equal(red.data.filled(1e+20), 1e+20)
+    red.nodata = 1e+20
 
-    if allsats is True:
-        fid = ['LT04', 'LT05', 'LE07', 'LC08', 'LC09']
+    green.data = np.ma.masked_equal(green.data.filled(1e+20), 1e+20)
+    green.nodata = 1e+20
 
-    elif sensor == 'Landsat 8 and 9 (OLI)':
-        fid = ['LC08', 'LC09']
-    elif sensor == 'Landsat 7 (ETM+)':
-        fid = ['LE07']
-    elif sensor == 'Landsat 4 and 5 (TM)':
-        fid = ['LT04', 'LT05']
-    else:
-        return None
-
-    flist2 = []
-    for i in flist:
-        if os.path.basename(i)[:4] not in fid:
-            continue
-        if '.tif' in i:
-            continue
-        flist2.append(i)
-
-    return flist2
-
-
-def get_sentinel_list(flist):
-    """
-    Get Sentinel-2 files from a file list.
-
-    Parameters
-    ----------
-    flist : list
-        List of filenames.
-
-    Returns
-    -------
-    flist : list
-        List of filenames.
-
-    """
-    if isinstance(flist[0], list):
-        if '.SAFE' in flist[0][0].filename:
-            return flist
-        return []
+    blue.data = np.ma.masked_equal(blue.data.filled(1e+20), 1e+20)
+    blue.nodata = 1e+20
 
-    flist2 = []
-    for i in flist:
-        if '.SAFE' not in i or 'S2A' not in i:
-            continue
-        flist2.append(i)
-
-    return flist2
+    return [red, green, blue]
 
 
 def _testfn():
     """Test routine."""
     import matplotlib.pyplot as plt
     import winsound
-
-    extscene = None
+    from pygmi.rsense.iodefs import ImportBatch
 
     ifile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\Sentinel-2\S2A_MSIL2A_20210305T075811_N0214_R035_T35JML_20210305T103519.zip"
     ifile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\Landsat\LC081740432017101901T1-SC20180409064853.tar.gz"
-    ifile =r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\New2016_merge_comp.tif"
-    ifile = r"E:\WorkProjects\ST-2021-1349 NRF\BRICS_NRF\2022-03-29T13-42-10Zcomp.tif"
-
-    dat = iodefs.get_data(ifile, extscene=extscene)
+    ifile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\wv2\014568829030_01_P001_MUL\16MAY28083210-M3DS-014568829030_01_P001.XML"
+    ifile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\ASTER\new\AST_07XT_00308302021082202_20230215122255_9222.zip"
 
-    winsound.PlaySound('SystemQuestion', winsound.SND_ALIAS)
+    idir = r'd:\sentinel2'
+    os.chdir(r'D:\\')
 
     app = QtWidgets.QApplication(sys.argv)
 
+    tmp1 = ImportBatch()
+    tmp1.idir = idir
+    tmp1.get_sfile(True)
+    tmp1.settings()
+
+    tmp1.outdata['RasterFileList'] = [tmp1.outdata['RasterFileList'][0]]
+
     SR = SatRatios()
-    SR.indata['Raster'] = dat
+    SR.indata = tmp1.outdata
     SR.settings()
 
     dat2 = SR.outdata['Raster']
     for i in dat2:
         plt.figure(dpi=150)
         plt.title(i.dataid)
         vmin = i.data.mean()-2*i.data.std()
         vmax = i.data.mean()+2*i.data.std()
         plt.imshow(i.data, vmin=vmin, vmax=vmax)
         plt.colorbar()
         plt.show()
 
-    winsound.PlaySound('SystemQuestion', winsound.SND_ALIAS)
-
-
-def _testfn2():
-    """Test routine."""
-    import glob
-    import matplotlib.pyplot as plt
-
-    ifiles = glob.glob(r'C:\Workdata\PyGMI Test Data\Remote Sensing\ConditionIndex\*.tar')
-
-    app = QtWidgets.QApplication(sys.argv)
-
-    SR = ConditionIndices()
-    SR.indata['RasterFileList'] = ifiles
-    SR.settings()
-
-    dat = SR.outdata["Raster"]
-
-    for i in dat:
-        plt.figure(dpi=200)
-        plt.imshow(i.data, extent=i.extent)
-        plt.colorbar()
-        plt.title(i.dataid)
-        plt.show()
-
-
-def _testfn3():
-    """Test Function."""
-    import matplotlib.pyplot as plt
-
-    ifile = r"C:/Workdata/Remote Sensing/Sentinel-2/S2A_MSIL2A_20210305T075811_N0214_R035_T35JML_20210305T103519.zip"
-    extscene = 'Sentinel-2'
-    dat = iodefs.get_data(ifile, extscene=extscene)
-
-    app = QtWidgets.QApplication(sys.argv)
-
-    SR = SatRatios()
-    SR.indata['Raster'] = dat  # single file only
-
-    SR.settings()
-
-    plt.title(dat[2].dataid)
-    plt.imshow(dat[2].data)
-    plt.colorbar()
-    plt.show()
+    dat = [i.data for i in dat2]
+    dat = np.moveaxis(dat, 0, -1)
 
-    plt.title(dat[0].dataid)
-    plt.imshow(dat[0].data)
-    plt.colorbar()
+    plt.figure(dpi=200)
+    plt.imshow(dat, vmin=0, vmax=1)
     plt.show()
 
-    plt.title(dat[3].dataid)
-    plt.imshow(dat[3].data)
-    plt.colorbar()
-    plt.show()
-
-    dat2 = SR.outdata['Raster']
-
-    plt.title(dat2[0].dataid)
-    plt.imshow(dat2[0].data, vmin=0, vmax=1)
-    plt.colorbar()
+    plt.figure(dpi=200)
+    plt.imshow(dat)
     plt.show()
 
-
-def _testfn4():
-    """Test routine."""
-    import glob
-    import matplotlib.pyplot as plt
-    from pygmi.raster.dataprep import DataMerge
-
-    ifiles = glob.glob(r"C:\WorkProjects\ratios\*.zip")
-
-    app = QtWidgets.QApplication(sys.argv)
-
-    ifiles = glob.glob(r"C:\WorkProjects\ratios\*.tif")
-
-    dat = []
-    for ifile in ifiles:
-        dat += iodefs.get_data(ifile)
-
-    DM = DataMerge()
-    DM.indata['Raster'] = dat
-    DM.settings()
-
-    dat += DM.outdata['Raster']
-
-    vmin = dat[0].data.mean() - dat[0].data.std()
-    vmax = dat[0].data.mean() + dat[0].data.std()
-
-    for i in dat:
-        plt.title(i.dataid)
-        plt.imshow(i.data, extent=i.extent, vmin=vmin, vmax=vmax)
-        plt.colorbar()
-        plt.show()
+    winsound.PlaySound('SystemQuestion', winsound.SND_ALIAS)
 
 
 if __name__ == "__main__":
-    _testfn2()
+    _testfn()
```

### Comparing `pygmi-3.2.6.5/pygmi/rsense/transforms.py` & `pygmi-3.2.7.16/pygmi/rsense/transforms.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,19 +29,21 @@
 
 import numpy as np
 from PyQt5 import QtWidgets, QtCore
 from sklearn.decomposition import IncrementalPCA
 import numexpr as ne
 import matplotlib.pyplot as plt
 
-from pygmi.raster.iodefs import export_raster
-from pygmi.rsense.iodefs import get_data
-from pygmi.raster.dataprep import lstack
 from pygmi.misc import BasicModule
 from pygmi import menu_default
+from pygmi.raster.iodefs import export_raster
+from pygmi.raster.dataprep import lstack
+from pygmi.rsense.iodefs import get_data
+from pygmi.rsense.iodefs import get_from_rastermeta
+from pygmi.rsense.iodefs import set_export_filename
 
 
 class MNF(BasicModule):
     """Perform MNF Transform."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
@@ -114,17 +116,21 @@
         bool
             True if successful, False otherwise.
 
         """
         self.ev = None
         tmp = []
         if 'Raster' not in self.indata and 'RasterFileList' not in self.indata:
-            self.showprocesslog('No Satellite Data')
+            self.showlog('No Satellite Data')
             return False
 
+        if 'RasterFileList' in self.indata:
+            if len(self.indata['RasterFileList'][0].bands) > 5:
+                self.sb_comps.setValue(5)
+
         if 'Raster' in self.indata:
             indata = self.indata['Raster']
             self.sb_comps.setMaximum(len(indata))
             if len(indata) > 5:
                 self.sb_comps.setValue(5)
 
         if not nodialog:
@@ -207,50 +213,54 @@
         Updates self.outdata, which is used as input to other modules.
 
         Returns
         -------
         None.
 
         """
+        if 'RasterFileList' in self.indata:
+            flist = self.indata['RasterFileList']
+
         ncmps = self.sb_comps.value()
         odata = []
 
         if self.rb_noise_diag.isChecked():
             noise = 'diagonal'
         elif self.rb_noise_hv.isChecked():
             noise = 'hv average'
         else:
             noise = 'quad'
 
         if 'RasterFileList' in self.indata:
-            flist = self.indata['RasterFileList']
-            odir = os.path.join(os.path.dirname(flist[0]), 'MNF')
+            filename = flist[0].filename
+            odir = os.path.join(os.path.dirname(filename), 'MNF')
 
             os.makedirs(odir, exist_ok=True)
             for ifile in flist:
-                self.showprocesslog('Processing '+os.path.basename(ifile))
+                filename = ifile.filename
 
-                dat = get_data(ifile, piter=self.piter,
-                               showprocesslog=self.showprocesslog,
-                               extscene='Bands Only')
+                self.showlog('Processing '+os.path.basename(filename))
+
+                dat = get_from_rastermeta(ifile, piter=self.piter,
+                                          showlog=self.showlog)
                 odata, self.ev = mnf_calc(dat, ncmps, piter=self.piter,
-                                          pprint=self.showprocesslog,
+                                          showlog=self.showlog,
                                           noisetxt=noise,
                                           fwdonly=self.cb_fwdonly.isChecked())
 
-                ofile = os.path.basename(ifile).split('.')[0] + '_mnf.tif'
-                ofile = os.path.join(odir, ofile)
+                ofile = set_export_filename(dat, odir, 'mnf')
 
-                self.showprocesslog('Exporting '+os.path.basename(ofile))
-                export_raster(ofile, odata, 'GTiff', piter=self.piter)
+                self.showlog('Exporting '+os.path.basename(ofile))
+                export_raster(ofile, odata, 'GTiff', piter=self.piter,
+                              showlog=self.showlog)
 
         elif 'Raster' in self.indata:
             dat = self.indata['Raster']
             odata, self.ev = mnf_calc(dat, ncmps, piter=self.piter,
-                                      pprint=self.showprocesslog,
+                                      showlog=self.showlog,
                                       noisetxt=noise,
                                       fwdonly=self.cb_fwdonly.isChecked())
 
         self.outdata['Raster'] = odata
         return True
 
 
@@ -321,19 +331,21 @@
         bool
             True if successful, False otherwise.
 
         """
         self.ev = None
         tmp = []
         if 'Raster' not in self.indata and 'RasterFileList' not in self.indata:
-            self.showprocesslog('No Satellite Data')
+            self.showlog('No Satellite Data')
             return False
 
         if 'RasterFileList' in self.indata:
             self.cb_fitlist.setVisible(True)
+            if len(self.indata['RasterFileList'][0].bands) > 5:
+                self.sb_comps.setValue(5)
 
         if 'Raster' in self.indata:
             indata = self.indata['Raster']
             self.sb_comps.setMaximum(len(indata))
             if len(indata) > 5:
                 self.sb_comps.setValue(5)
 
@@ -421,54 +433,66 @@
         None.
 
         """
         ncmps = self.sb_comps.value()
         fitlist = self.cb_fitlist.isChecked()
         fwdonly = self.cb_fwdonly.isChecked()
 
+        if 'RasterFileList' in self.indata:
+            flist = self.indata['RasterFileList']
+
+            sensors = [i.sensor for i in flist]
+            sensors = list(set(sensors))
+
+            if fitlist is True and len(sensors) > 1:
+                self.showlog('Error: You have more than one sensor type in '
+                             'your raster file list directory. Fit list is not'
+                             ' possible.')
+                return False
+
         odata = []
 
         if 'RasterFileList' in self.indata and fitlist is False:
-            flist = self.indata['RasterFileList']
-            odir = os.path.join(os.path.dirname(flist[0]), 'PCA')
+            filename = flist[0].filename
+            odir = os.path.join(os.path.dirname(filename), 'PCA')
 
             os.makedirs(odir, exist_ok=True)
             for ifile in flist:
-                self.showprocesslog('Processing '+os.path.basename(ifile))
+                filename = ifile.filename
+
+                self.showlog('Processing '+os.path.basename(filename))
 
-                dat = get_data(ifile, piter=self.piter,
-                               showprocesslog=self.showprocesslog,
-                               extscene='Bands Only')
+                dat = get_from_rastermeta(ifile, piter=self.piter,
+                                          showlog=self.showlog)
                 odata, self.ev = pca_calc(dat, ncmps, piter=self.piter,
-                                          pprint=self.showprocesslog,
+                                          showlog=self.showlog,
                                           fwdonly=fwdonly)
 
-                ofile = os.path.basename(ifile).split('.')[0] + '_pca.tif'
-                ofile = os.path.join(odir, ofile)
+                ofile = set_export_filename(dat, odir, 'pca')
 
-                self.showprocesslog('Exporting '+os.path.basename(ofile))
-                export_raster(ofile, odata, 'GTiff', piter=self.piter)
+                self.showlog('Exporting '+os.path.basename(ofile))
+                export_raster(ofile, odata, 'GTiff', piter=self.piter,
+                              showlog=self.showlog)
 
         elif 'RasterFileList' in self.indata and fitlist is True:
-            flist = self.indata['RasterFileList']
             odata, self.ev = pca_calc_fitlist(flist, ncmps, piter=self.piter,
-                                              pprint=self.showprocesslog,
+                                              showlog=self.showlog,
                                               fwdonly=fwdonly)
 
         elif 'Raster' in self.indata:
             dat = self.indata['Raster']
             odata, self.ev = pca_calc(dat, ncmps, piter=self.piter,
-                                      pprint=self.showprocesslog,
+                                      showlog=self.showlog,
                                       fwdonly=self.cb_fwdonly.isChecked())
 
         self.outdata['Raster'] = odata
         return True
 
 
-def get_noise(x2d, mask, noise=''):
+def get_noise(x2d, mask, noise='', piter=iter):
     """
     Calculate noise dataset from original data.
 
     Parameters
     ----------
     x2d : numpy array
         Input array, of dimension (MxNxChannels).
@@ -484,14 +508,17 @@
         Noise eigenvalues.
     nevecs : numpy array
         Noise eigenvectors.
 
     """
     mask = ~mask
 
+    pbar = piter([1, 2, 3])
+    next(pbar)
+
     if noise == 'diagonal':
         t1 = x2d[:-1, :-1]
         t2 = x2d[1:, 1:]
         noise = ne.evaluate('t1-t2')
 
         mask2 = mask[:-1, :-1]*mask[1:, 1:]
         noise = noise[mask2]
@@ -527,37 +554,40 @@
         mask2 = (mask[:-2, :-2] * mask[:-2, 1:-1] * mask[:-2, 2:] *
                  mask[1:-1, :-2] * mask[1:-1, 1:-1] * mask[1:-1, 2:] *
                  mask[2:, :-2] * mask[2:, 1:-1] * mask[2:, 2:])
 
         noise = noise[mask2]
         ncov = np.cov(noise.T)/81
 
+    next(pbar)
     # Calculate evecs and evals
     nevals, nevecs = np.linalg.eig(ncov)
 
+    next(pbar)
+
     # return noise, mask2
     return nevals, nevecs
 
 
-def mnf_calc(dat, ncmps=None, noisetxt='hv average', pprint=print, piter=iter,
+def mnf_calc(dat, ncmps=None, noisetxt='hv average', showlog=print, piter=iter,
              fwdonly=True):
     """
     MNF Calculation.
 
     Parameters
     ----------
     dat : List
         List of PyGMI Data.
     ncmps : int or None, optional
         Number of components to use for filtering. The default is None
         (meaning all).
     noisetxt : txt, optional
         Noise type. Can be 'diagonal', 'hv average' or 'quad'. The default is
         'hv average'.
-    pprint : function, optional
+    showlog : function, optional
         Function for printing text. The default is print.
     piter : function, optional
         Iteration function, used for progress bars. The default is iter.
     fwdonly : bool, optional
         Option to perform forward calculation only. The default is True.
 
     Returns
@@ -566,66 +596,66 @@
         Output list of PyGMI Data.Can be forward or inverse transformed data.
     ev : numpy array
         Explained variance, from PCA.
 
     """
     x2d = []
     maskall = []
-    dat = lstack(dat, piter=piter, pprint=pprint, commonmask=True)
+    dat = lstack(dat, piter=piter, showlog=showlog, commonmask=True)
 
     for j in dat:
         x2d.append(j.data)
         maskall.append(j.data.mask)
 
     maskall = np.moveaxis(maskall, 0, -1)
     x2d = np.moveaxis(x2d, 0, -1)
     x2dshape = list(x2d.shape)
 
     mask = maskall[:, :, 0]
 
-    pprint('Calculating noise data...')
-    nevals, nevecs = get_noise(x2d, mask, noisetxt)
+    showlog('Calculating noise data...')
+    nevals, nevecs = get_noise(x2d, mask, noisetxt, piter)
 
-    pprint('Calculating MNF...')
+    showlog('Calculating MNF...')
     Ln = np.power(nevals, -0.5)
     Ln = np.diag(Ln)
 
     W = np.dot(Ln, nevecs.T)
 
     x = x2d[~mask]
     del x2d
 
     Pnorm = np.dot(x, W.T)
 
     pca = IncrementalPCA(n_components=ncmps)
 
     iold = 0
-    pprint('Fitting PCA')
+    showlog('Fitting PCA')
     for i in piter(np.linspace(0, Pnorm.shape[0], 20, dtype=int)):
         if i == 0:
             continue
         pca.partial_fit(Pnorm[iold: i])
         iold = i
 
-    pprint('Calculating PCA transform...')
+    showlog('Calculating PCA transform...')
 
     x2 = np.zeros((Pnorm.shape[0], pca.n_components_))
     iold = 0
     for i in piter(np.linspace(0, Pnorm.shape[0], 20, dtype=int)):
         if i == 0:
             continue
         x2[iold: i] = pca.transform(Pnorm[iold: i])
         iold = i
 
     del Pnorm
     ev = pca.explained_variance_
     evr = pca.explained_variance_ratio_
 
     if fwdonly is False:
-        pprint('Calculating inverse MNF...')
+        showlog('Calculating inverse MNF...')
         Winv = np.linalg.inv(W)
         P = pca.inverse_transform(x2)
         x2 = np.dot(P, Winv.T)
         del P
     else:
         x2dshape[-1] = ncmps
         maskall = maskall[:, :, :ncmps]
@@ -638,34 +668,34 @@
 
     odata = copy.deepcopy(dat)
     if fwdonly:
         odata = odata[:ncmps]
     for j, band in enumerate(odata):
         band.data = datall[:, :, j]
         if fwdonly is True:
-            band.dataid = (f'MNF {j+1} Explained Variance Ratio '
+            band.dataid = (f'MNF{j+1} Explained Variance Ratio '
                            f'{evr[j]*100:.2f}%')
 
     del datall
 
     return odata, ev
 
 
-def pca_calc(dat, ncmps=None,  pprint=print, piter=iter, fwdonly=True):
+def pca_calc(dat, ncmps=None,  showlog=print, piter=iter, fwdonly=True):
     """
     PCA Calculation.
 
     Parameters
     ----------
     dat : List
         List of PyGMI Data.
     ncmps : int or None, optional
         Number of components to use for filtering. The default is None
         (meaning all).
-    pprint : function, optional
+    showlog : function, optional
         Function for printing text. The default is print.
     piter : function, optional
         Iteration function, used for progress bars. The default is iter.
     fwdonly : bool, optional
         Option to perform forward calculation only. The default is True.
 
     Returns
@@ -691,37 +721,37 @@
     mask = maskall[:, :, 0]
 
     x2d = x2d[~mask]
 
     pca = IncrementalPCA(n_components=ncmps)
 
     iold = 0
-    pprint('Fitting PCA')
+    showlog('Fitting PCA')
     for i in piter(np.linspace(0, x2d.shape[0], 20, dtype=int)):
         if i == 0:
             continue
         pca.partial_fit(x2d[iold: i])
         iold = i
 
-    pprint('Calculating PCA transform...')
+    showlog('Calculating PCA transform...')
 
     x2 = np.zeros((x2d.shape[0], pca.n_components_))
     iold = 0
     for i in piter(np.linspace(0, x2d.shape[0], 20, dtype=int)):
         if i == 0:
             continue
         x2[iold: i] = pca.transform(x2d[iold: i])
         iold = i
 
     del x2d
     ev = pca.explained_variance_
     evr = pca.explained_variance_ratio_
 
     if fwdonly is False:
-        pprint('Calculating inverse PCA...')
+        showlog('Calculating inverse PCA...')
         x2 = pca.inverse_transform(x2)
     else:
         x2dshape[-1] = ncmps
         maskall = maskall[:, :, :ncmps]
 
     datall = np.zeros(x2dshape, dtype=np.float32)
 
@@ -732,56 +762,67 @@
 
     odata = copy.deepcopy(dat)
     if fwdonly:
         odata = odata[:ncmps]
     for j, band in enumerate(odata):
         band.data = datall[:, :, j]
         if fwdonly is True:
-            band.dataid = (f'PCA {j+1} Explained Variance Ratio '
+            band.dataid = (f'PCA{j+1} Explained Variance Ratio '
                            f'{evr[j]*100:.2f}%')
     del datall
 
     return odata, ev
 
 
-def pca_calc_fitlist(flist, ncmps=None,  pprint=print, piter=iter,
+def pca_calc_fitlist(flist, ncmps=None,  showlog=print, piter=iter,
                      fwdonly=True):
     """
     PCA Calculation with using list of files in common fit.
 
     Parameters
     ----------
     dat : List
         List of PyGMI Data.
     ncmps : int or None, optional
         Number of components to use for filtering. The default is None
         (meaning all).
-    pprint : function, optional
+    showlog : function, optional
         Function for printing text. The default is print.
     piter : function, optional
         Iteration function, used for progress bars. The default is iter.
     fwdonly : bool, optional
         Option to perform forward calculation only. The default is True.
 
     Returns
     -------
     odata : list
         Output list of PyGMI Data.Can be forward or inverse transformed data.
     ev : numpy array
         Explained variance, from PCA.
 
     """
-    odir = os.path.join(os.path.dirname(flist[0]), 'PCA')
+    if isinstance(flist[0], list):
+        filename = flist[0][0].filename
+    else:
+        filename = flist[0].filename
+
+    odir = os.path.join(os.path.dirname(filename), 'PCA')
     os.makedirs(odir, exist_ok=True)
 
     for ifile in flist:
-        pprint('Fitting '+os.path.basename(ifile))
+        if isinstance(ifile, list):
+            filename = ifile[0].filename
+        else:
+            filename = ifile.filename
 
-        dat = get_data(ifile, piter=piter, showprocesslog=pprint,
-                       extscene='Bands Only')
+        showlog('Fitting '+os.path.basename(filename))
+
+        # dat = get_data(ifile, piter=piter, showlog=showlog)
+
+        dat = get_from_rastermeta(ifile, piter=piter, showlog=showlog)
 
         x2d = []
         maskall = []
         dat = lstack(dat, piter=piter, commonmask=True)
 
         for j in dat:
             x2d.append(j.data)
@@ -801,18 +842,24 @@
         for i in piter(np.linspace(0, x2d.shape[0], 20, dtype=int)):
             if i == 0:
                 continue
             pca.partial_fit(x2d[iold: i])
             iold = i
 
     for ifile in flist:
-        pprint('Transforming '+os.path.basename(ifile))
+        if isinstance(ifile, list):
+            filename = ifile[0].filename
+        else:
+            filename = ifile.filename
+
+        showlog('Transforming '+os.path.basename(filename))
+
+        # dat = get_data(ifile, piter=piter, showlog=showlog)
 
-        dat = get_data(ifile, piter=piter, showprocesslog=pprint,
-                       extscene='Bands Only')
+        dat = get_from_rastermeta(ifile, piter=piter, showlog=showlog)
 
         x2d = []
         maskall = []
         dat = lstack(dat, piter=piter)
 
         for j in dat:
             x2d.append(j.data)
@@ -835,15 +882,15 @@
             iold = i
 
         del x2d
         ev = pca.explained_variance_
         evr = pca.explained_variance_ratio_
 
         if fwdonly is False:
-            pprint('Calculating inverse PCA...')
+            showlog('Calculating inverse PCA...')
             x2 = pca.inverse_transform(x2)
         else:
             x2dshape[-1] = ncmps
             maskall = maskall[:, :, :ncmps]
 
         datall = np.zeros(x2dshape, dtype=np.float32)
 
@@ -854,34 +901,42 @@
 
         odata = copy.deepcopy(dat)
         if fwdonly:
             odata = odata[:ncmps]
         for j, band in enumerate(odata):
             band.data = datall[:, :, j]
             if fwdonly is True:
-                band.dataid = (f'PCA {j+1} Explained Variance Ratio '
+                band.dataid = (f'PCA{j+1} Explained Variance Ratio '
                                f'{evr[j]*100:.2f}%')
         del datall
 
-        ofile = os.path.basename(ifile).split('.')[0] + '_pca.tif'
-        ofile = os.path.join(odir, ofile)
+        # ofile = os.path.basename(filename).split('.')[0] + '_pca.tif'
+        # ofile = os.path.join(odir, ofile)
 
-        pprint('Exporting '+os.path.basename(ofile))
-        export_raster(ofile, odata, 'GTiff', piter=piter, compression='ZSTD')
+        # if 'AST_' in ofile:
+        #     ofile = ofile.replace('_05_', '_')
+        #     ofile = ofile.replace('_07XT_', '_')
+        #     ofile = ofile.replace('_07_', '_')
+
+        ofile = set_export_filename(dat, odir, 'pca')
+
+        showlog('Exporting '+os.path.basename(ofile))
+        export_raster(ofile, odata, 'GTiff', piter=piter, compression='ZSTD',
+                      showlog=showlog)
 
     return odata, ev
 
 
 def _testfn():
     """Test routine."""
     ifile = r"D:\Workdata\PyGMI Test Data\Remote Sensing\Import\hyperion\EO1H1760802013198110KF_1T.ZIP"
 
     ncmps = 10
 
-    dat = get_data(ifile, extscene='Hyperion')
+    dat = get_data(ifile)
 
     pmnf, _ = mnf_calc(dat, ncmps=ncmps, fwdonly=False)
 
     for i, _ in enumerate(dat): #[0, 5, 10, 13, 14, 15, 20, 25]:
         vmax = dat[i].data.max()
         vmin = dat[i].data.min()
 
@@ -902,23 +957,20 @@
 def _testfn2():
     import sys
     from matplotlib import rcParams
 
     rcParams['figure.dpi'] = 150
 
     # ifile = r'C:/Workdata/Remote Sensing/Sentinel-2/S2A_MSIL2A_20210305T075811_N0214_R035_T35JML_20210305T103519.zip'
-    # extscene = 'Sentinel-2 Bands Only'
     ifile = r'C:/Workdata/Remote Sensing/ASTER/PCA Test/AST_05_07XT_20060807_7016_stack.tif'
-    extscene = None
-
     ifile = r'C:/Workdata/Remote Sensing/Landsat/LC09_L1TP_173080_20211110_20220119_02_T1.tar'
     # ifile2 = r'C:/Workdata/Remote Sensing/ASTER/PCA Test/AST_05_07XT_20060807_7016_pca.tif'
 
-    dat = get_data(ifile, extscene=extscene)
-    # dat2 = get_data(ifile2, extscene=extscene)
+    dat = get_data(ifile)
+    # dat2 = get_data(ifile2)
 
     # pmnf, ev = mnf_calc(dat, ncmps=ncmps, noisetxt='', piter=pbar.iter)
 
     app = QtWidgets.QApplication(sys.argv)  # Necessary to test Qt Classes
 
     # tmp = PCA()
     tmp = MNF()
@@ -940,30 +992,28 @@
         # vmax = dat2[i].data.mean()+dat2[i].data.std()*2
         # plt.imshow(dat2[i].data, vmin=vmin, vmax=vmax)
         plt.show()
 
 
 def _testfn3():
     import sys
-    from matplotlib import rcParams
     from pygmi.rsense.iodefs import ImportBatch
 
-    rcParams['figure.dpi'] = 150
-
-    idir = r'e:\WorkProjects\ST-2022-1355 Onshore Mapping\Niger\sentinel_2\full'
+    idir = r'd:\aster'
+    os.chdir(r'D:\\')
 
     app = QtWidgets.QApplication(sys.argv)
 
     tmp1 = ImportBatch()
     tmp1.idir = idir
-    tmp1.settings(True)
+    tmp1.settings()
 
     dat = tmp1.outdata
 
-    tmp2 = PCA()
-    # tmp2 = MNF()
+    # tmp2 = PCA()
+    tmp2 = MNF()
     tmp2.indata = dat
     tmp2.settings()
 
 
 if __name__ == "__main__":
-    _testfn()
+    _testfn3()
```

### Comparing `pygmi-3.2.6.5/pygmi/seis/beachball.py` & `pygmi-3.2.7.16/pygmi/seis/beachball.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,35 +29,37 @@
 at http://www.ceri.memphis.edu/people/olboyd/Software/Software.html
 """
 
 import os
 import numpy as np
 import numexpr as ne
 from PyQt5 import QtWidgets
+import geopandas as gpd
+from shapely.geometry import Polygon
+from shapely.validation import make_valid
 from matplotlib import colormaps
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.backends.backend_qt5 import NavigationToolbar2QT
 from matplotlib import patches
-from osgeo import ogr, osr
 import scipy.spatial.distance as sdist
 
 from pygmi.misc import BasicModule
 
 
 class MyMplCanvas(FigureCanvasQTAgg):
     """Canvas for the actual plot."""
 
     def __init__(self, parent=None):
         fig = Figure()
         super().__init__(fig)
         if parent is None:
-            self.showprocesslog = print
+            self.showlog = print
         else:
-            self.showprocesslog = parent.showprocesslog
+            self.showlog = parent.showlog
 
         # figure stuff
         self.htype = 'Linear'
         self.cbar = colormaps['jet']
         self.data = []
         self.gmode = None
         self.argb = [None, None, None]
@@ -164,15 +166,15 @@
 
         alist = []
         for i in data:
             alist += list(i['F'].keys())
         alist = sorted(set(alist))
 
         if not alist:
-            self.showprocesslog('Error: no Fault Plane Solutions')
+            self.showlog('Error: no Fault Plane Solutions')
             self.nofps = True
             return False
         self.nofps = False
 
         try:
             self.cbox_alg.currentIndexChanged.disconnect()
         except TypeError:
@@ -284,98 +286,62 @@
         if os.path.isfile(ifile_bnd):
             tmp = ifile_bnd[:-4]
             os.remove(tmp+'.shp')
             os.remove(tmp+'.shx')
             os.remove(tmp+'.prj')
             os.remove(tmp+'.dbf')
 
-        driver = ogr.GetDriverByName('ESRI Shapefile')
-        data_source = driver.CreateDataSource(self.ifile)
-        data_source2 = driver.CreateDataSource(ifile_bnd)
-
-        # create the spatial reference, WGS84
-        srs = osr.SpatialReference()
-        srs.ImportFromEPSG(4326)
-        srs.SetAxisMappingStrategy(osr.OAMS_TRADITIONAL_GIS_ORDER)
-
-        # create the layer
-        layer = data_source.CreateLayer('Fault Plane Solution', srs,
-                                        ogr.wkbPolygon)
-        layer.CreateField(ogr.FieldDefn('Strike', ogr.OFTReal))
-        layer.CreateField(ogr.FieldDefn('Dip', ogr.OFTReal))
-        layer.CreateField(ogr.FieldDefn('Rake', ogr.OFTReal))
-        layer.CreateField(ogr.FieldDefn('Magnitude', ogr.OFTReal))
-        layer.CreateField(ogr.FieldDefn('Quadrant', ogr.OFTString))
-        layer.CreateField(ogr.FieldDefn('Depth', ogr.OFTReal))
-
-        layer2 = data_source2.CreateLayer('Fault Plane Solution Boundaries',
-                                          srs, ogr.wkbPolygon)
-
-        layer2.CreateField(ogr.FieldDefn('Strike', ogr.OFTReal))
-        layer2.CreateField(ogr.FieldDefn('Dip', ogr.OFTReal))
-        layer2.CreateField(ogr.FieldDefn('Rake', ogr.OFTReal))
-        layer2.CreateField(ogr.FieldDefn('Magnitude', ogr.OFTReal))
-        layer2.CreateField(ogr.FieldDefn('Quadrant', ogr.OFTString))
-        layer2.CreateField(ogr.FieldDefn('Depth', ogr.OFTReal))
+        layer = {'Event': [],
+                 'Strike': [],
+                 'Dip': [],
+                 'Rake': [],
+                 'Magnitude': [],
+                 'Quadrant': [],
+                 'Depth': [],
+                 'geometry': []}
 
         # Calculate BeachBall
-        for idat in indata:
+        for i, idat in enumerate(indata):
             pxy = idat[:2]
             np1 = idat[3:-1]
             depth = idat[2]
             pwidth = self.mmc.pwidth*idat[-1]
             xxx, yyy, xxx2, yyy2 = beachball(np1, pxy[0], pxy[1], pwidth,
                                              self.mmc.isgeog,
-                                             self.showprocesslog)
+                                             self.showlog)
 
             pvert1 = np.transpose([yyy, xxx])
             pvert0 = np.transpose([xxx2, yyy2])
 
-            # Create Geometry
-            outring = ogr.Geometry(ogr.wkbLinearRing)
-            for i in pvert1:
-                outring.AddPoint(i[0], i[1])
-
-            innerring = ogr.Geometry(ogr.wkbLinearRing)
-            for i in pvert0:
-                innerring.AddPoint(i[0], i[1])
-
-            poly = ogr.Geometry(ogr.wkbPolygon)
-            poly.AddGeometry(outring)
-
-            poly1 = ogr.Geometry(ogr.wkbPolygon)
-            poly1.AddGeometry(innerring)
-
-            feature = ogr.Feature(layer.GetLayerDefn())
-
-            feature.SetField('Strike', np1[0])
-            feature.SetField('Dip', np1[1])
-            feature.SetField('Rake', np1[2])
-            feature.SetField('Magnitude', idat[-1])
-            feature.SetField('Quadrant', 'Compressional')
-            feature.SetField('Depth', depth)
-
-            feature.SetGeometry(poly)
-            # Create the feature in the layer (shapefile)
-            layer.CreateFeature(feature)
-            # Destroy the feature to free resources
-
-            feature2 = ogr.Feature(layer2.GetLayerDefn())
-            feature2.SetField('Quadrant', 'Tensional and Compressional')
-            feature2.SetField('Depth', depth)
-            feature2.SetGeometry(poly1)
-            # Create the feature in the layer (shapefile)
-            layer2.CreateFeature(feature2)
-            layer2.CreateFeature(feature)
-            # Destroy the feature to free resources
-            feature.Destroy()
-            feature2.Destroy()
+            poly1 = make_valid(Polygon(pvert1))
+            poly0 = make_valid(Polygon(pvert0))
+            poly0 = poly0.difference(poly1)
+
+            layer['geometry'].append(poly0)
+            layer['Event'].append(i)
+            layer['Strike'].append(np1[0])
+            layer['Dip'].append(np1[1])
+            layer['Rake'].append(np1[2])
+            layer['Magnitude'].append(idat[-1])
+            layer['Quadrant'].append('Compressional')
+            layer['Depth'].append(depth)
+
+            layer['geometry'].append(poly1)
+            layer['Event'].append(i)
+            layer['Strike'].append(np1[0])
+            layer['Dip'].append(np1[1])
+            layer['Rake'].append(np1[2])
+            layer['Magnitude'].append(idat[-1])
+            layer['Quadrant'].append('Tensional')
+            layer['Depth'].append(depth)
 
-        data_source.Destroy()
-        data_source2.Destroy()
+        gdf = gpd.GeoDataFrame(layer)
+        gdf = gdf.set_crs(4326)
+
+        gdf.to_file(self.ifile)
 
         return True
 
     def change_alg(self):
         """
         Change algorithm.
 
@@ -415,15 +381,15 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         if self.nofps:
-            self.showprocesslog('Error: no Fault Plane Solutions')
+            self.showlog('Error: no Fault Plane Solutions')
             return False
 
         self.show()
         QtWidgets.QApplication.processEvents()
 
         self.mmc.init_graph()
         return True
@@ -456,15 +422,15 @@
 
         """
         projdata = {}
 
         return projdata
 
 
-def beachball(fm, centerx, centery, diam, isgeog, showprocesslog=print):
+def beachball(fm, centerx, centery, diam, isgeog, showlog=print):
     """
     Beachball.
 
     Source code provided here are adopted from MatLab script
     `bb.m` written by Andy Michael and Oliver Boyd.
 
     function bb(fm, centerx, centery, diam, ta, color)
@@ -489,15 +455,15 @@
         place beachball(s) at position centerx
     centery : float
         place beachball(s) at position centery
     diam : float
         draw beachball with this diameter.
     isgeog : bool
         True if in geographic coordinates, False otherwise.
-    showprocesslog : function, optional
+    showlog : function, optional
         Routine to show text messages. The default is print.
 
     Returns
     -------
     X : numpy array
         array of x coordinates for vertices
     Y : numpy array
@@ -580,15 +546,15 @@
     l1 = np.sqrt(d**2/(np.sin(phi)**2 + np.cos(phi)**2 * d**2/m**2))
 
     d = 90 - D2
     m = 90
     l2 = np.sqrt(d**2/(np.sin(phi)**2 + np.cos(phi)**2 * d**2/m**2))
 
     if D == 0:
-        showprocesslog('Enter a diameter for the beachballs!')
+        showlog('Enter a diameter for the beachballs!')
         return None
 
     inc = 1
     X1, Y1 = pol2cart(phi+S1*d2r, l1)
     if P == 1:
         lo = S1 - 180
         hi = S2
```

### Comparing `pygmi-3.2.6.5/pygmi/seis/datatypes.py` & `pygmi-3.2.7.16/pygmi/seis/datatypes.py`

 * *Files identical despite different names*

### Comparing `pygmi-3.2.6.5/pygmi/seis/del_rec.py` & `pygmi-3.2.7.16/pygmi/seis/del_rec.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
-        self.showprocesslog('Delete Rows starting')
+        self.showlog('Delete Rows starting')
 
         ifile, _ = QtWidgets.QFileDialog.getOpenFileName()
         if ifile == '':
             return False
         os.chdir(ifile.rpartition('/')[0])
 
         self.delrec(ifile)
@@ -112,29 +112,29 @@
         Returns
         -------
         None.
 
         """
         ofile = ifile[:-4]+'_new.out'
 
-        self.showprocesslog('Input Filename: '+ifile)
-        self.showprocesslog('Output Filename: '+ofile)
+        self.showlog('Input Filename: '+ifile)
+        self.showlog('Output Filename: '+ofile)
 
         outputf = open(ofile, 'w', encoding='utf-8')
         inputf = open(ifile, encoding='utf-8')
 
         skey = QtWidgets.QInputDialog.getText(
             self.parent, 'Delete Criteria',
             'Please input the terms used to decide on lines to delete',
             QtWidgets.QLineEdit.Normal, 'AML, IAML')[0]
 
         skey = str(skey).upper()
 
-        self.showprocesslog('Delete Criteria: '+skey)
-        self.showprocesslog('Working...')
+        self.showlog('Delete Criteria: '+skey)
+        self.showlog('Working...')
 
         skey = skey.replace(' ', '')
         skey = skey.split(',')
 
         idata = inputf.readlines()
         odata = idata
         for j in skey:
@@ -142,15 +142,15 @@
 
         outputf.writelines(odata)  # Insert a blank line
 
         # Close files
         inputf.close()
         outputf.close()
 
-        self.showprocesslog('Completed!')
+        self.showlog('Completed!')
 
 
 class Quarry(BasicModule):
     """Main form which does the GUI and the program."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
@@ -170,30 +170,30 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
-        self.showprocesslog('Delete quarry events starting')
-        self.showprocesslog('Daytime defined from 9am to 7pm')
-        self.showprocesslog('Events radius: .2 degrees')
+        self.showlog('Delete quarry events starting')
+        self.showlog('Daytime defined from 9am to 7pm')
+        self.showlog('Events radius: .2 degrees')
 
         if 'Seis' not in self.indata:
             return False
 
         data = self.indata['Seis']
 
         alist = []
         for i in data:
             if '1' in i:
                 alist.append(i)
 
         if not alist:
-            self.showprocesslog('Error: no Type 1 records')
+            self.showlog('Error: no Type 1 records')
             return False
 
         self.events = alist
 
         data = self.calcrq2b()
         if data is not None:
             self.outdata['Seis'] = data
@@ -239,15 +239,15 @@
 
         Returns
         -------
         newevents : list
             New events
 
         """
-        self.showprocesslog('Working...')
+        self.showlog('Working...')
 
         hour = []
         lat = []
         lon = []
         newevents = []
 
         for i in self.events:
@@ -279,33 +279,33 @@
         # use DBscan to identify cluster centers and numbers of clusters.
         # eps is max distance between samples
 
         # X = np.transpose([lon, lat])
         # db = DBSCAN(eps=0.01, min_samples=10).fit(X)
         # labels = db.labels_  # noisy samples are -1
 
-        # self.showprocesslog('now calculate means')
+        # self.showlog('now calculate means')
         # clusters = []
         # for i in np.unique(labels):
         #     if i == -1:
         #         continue
         #     lontmp = lon[labels == i].mean()
         #     lattmp = lat[labels == i].mean()
         #     clusters.append([lontmp, lattmp])
 
         # clusters = np.array(clusters)
-        self.showprocesslog('Calculating Rq values')
+        self.showlog('Calculating Rq values')
 
         while stayinloop:
             lls = np.transpose([lat, lon])
             cnt = lls.shape[0]
             nd = []
             rstot = []
-            self.showprocesslog('daylight events left: ' + str(hour.sum()) +
-                                ' of ' + str(hour.size))
+            self.showlog('daylight events left: ' + str(hour.sum()) +
+                         ' of ' + str(hour.size))
 
             # instead of a grid, we are using an actual event location
             # instead of centering on every event, we should use only daytime
             # events
             # also, it must not use an event if it is further than a certain
             # distance
             # also, perhaps if total events less than 50, is that even allowed?
@@ -335,29 +335,29 @@
                 hour = np.delete(hour, rstot[maxel])
                 ehour = np.delete(ehour, rstot[maxel])
                 newevents = np.delete(newevents, rstot[maxel])
             else:
                 stayinloop = False
             stayinloop = False
 
-        self.showprocesslog('Completed!')
+        self.showlog('Completed!')
 
         return newevents
 
     def calcrq2b(self):
         """
         Calculate the Rq value.
 
         Returns
         -------
         newevents : list
             New events
 
         """
-        self.showprocesslog('Working...')
+        self.showlog('Working...')
 
         hour = []
         lat = []
         lon = []
         newevents = []
 
         for i2 in self.events:
@@ -380,38 +380,37 @@
         ln = 24-ld  # number of nightime hours
         rdist = 0.2  # max distance for event to qualify. In degrees
         N = 50
 
         # rperc = self.randrqb(N, day, ehourall.shape[0])
         rperc = 3.0
 
-        self.showprocesslog('Calculating Rq values')
+        self.showlog('Calculating Rq values')
 
         lls = np.transpose([lat, lon])
         cnt = lls.shape[0]
         nd = []
         rstot = []
-        self.showprocesslog('daylight events:'+str(hour.sum())+' of ' +
-                            str(hour.size))
+        self.showlog('daylight events:'+str(hour.sum())+' of ' +
+                     str(hour.size))
 
         for i in range(cnt):  # i is node number, centered on an event
             r = np.sqrt(((lls-lls[i])**2).sum(1))
 
             rs = np.argpartition(r, N)[:N]
 
             if r[rs].max() > rdist:
                 continue
 
             hrs = hour[rs]  # daylight hours for this node
             rstot.append(rs[hrs])
             nd.append(hrs)
 
         if len(nd) == 0:
-            self.showprocesslog('Not enough events within 0.2 degrees. '
-                                'Aborting.')
+            self.showlog('Not enough events within 0.2 degrees. Aborting.')
             return None
         nd = np.sum(nd, 1)
         nn = (N-nd).astype(float)
         nn[nn == 0] = 0.00001
         rq = (nd*ln)/(nn*ld)
 
         rstot = np.array(rstot, dtype=object)
@@ -426,15 +425,15 @@
 
         lat = np.delete(lat, maxel)
         lon = np.delete(lon, maxel)
         hour = np.delete(hour, maxel)
         ehour = np.delete(ehour, maxel)
         newevents = np.delete(newevents, maxel)
 
-        self.showprocesslog('Completed!')
+        self.showlog('Completed!')
 
         return newevents.tolist()
 
     def randrq(self, nmax, nstep, nrange, day):
         """
         Calculate random Rq values.
 
@@ -454,23 +453,23 @@
         rperc : list
             Percentiles
 
         """
         rperc = [1.97435897, 1.64253394, 1.46153846, 1.41025641, 1.35737179,
                  1.3234714, 1.28444936, 1.26923077]
 
-        self.showprocesslog('Calculating random Rq values for calibration')
+        self.showlog('Calculating random Rq values for calibration')
         rperc = []
         nd = 0
         ld = day[1]-day[0]
         ln = 24-ld
 
         nrange = [10]
         for N in nrange:
-            self.showprocesslog(str(N)+' of '+str(nmax), True)
+            self.showlog(str(N)+' of '+str(nmax), True)
             tmp = np.random.rand(1000000, nstep)
             tmp *= 24
 
             tmp = np.logical_and(tmp >= day[0], tmp <= day[1])
 
             nd += tmp.sum(1)
             nn = N-nd
@@ -494,15 +493,15 @@
 
         Returns
         -------
         rperc : list
             Percentiles
 
         """
-        self.showprocesslog('Calculating random Rq values for calibration')
+        self.showlog('Calculating random Rq values for calibration')
         elist = [50, 100, 150, 200]
 
         for N in elist:
             rqmean = []
             for ld in range(1, 24):
                 day = (0, ld)
                 ln = 24-ld
```

### Comparing `pygmi-3.2.6.5/pygmi/seis/graphs.py` & `pygmi-3.2.7.16/pygmi/seis/graphs.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,24 +27,25 @@
 
 This module provides a variety of methods to plot raster data via the context
 menu.
 """
 
 import os
 import numpy as np
-from osgeo import ogr, osr
 from PyQt5 import QtWidgets, QtCore
+import geopandas as gpd
+from shapely.geometry import Polygon
 from scipy.spatial.distance import cdist
 from scipy.stats import linregress
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qt5 import NavigationToolbar2QT
 from matplotlib.patches import Ellipse
-import contextily as ctx
-import pyproj
+# import contextily as ctx
+# import pyproj
 
 from pygmi.misc import ContextModule
 
 
 class MyMplCanvas(FigureCanvasQTAgg):
     """
     Canvas for the actual plot.
@@ -55,15 +56,15 @@
         axes for matplotlib subplot
     parent : parent
         reference to the parent routine
     """
 
     def __init__(self, parent=None):
 
-        fig = Figure()
+        fig = Figure(layout='constrained')
         self.axes = fig.add_subplot(111)
 
         self.ellipses = []
 
         super().__init__(fig)
 
     def update_ellipse(self, datd, dats, nodepth=False):
@@ -152,23 +153,20 @@
                           width=demaj, height=demin,
                           angle=ang, color='black')
             ell.set_facecolor('none')
 
             self.ellipses.append(ell.get_verts())
             self.axes.add_artist(ell)
 
+        # try:
+        #     ctx.add_basemap(self.axes, crs=pyproj.CRS.from_epsg(4326),
+        #                     source=ctx.providers.OpenStreetMap.Mapnik)
+        # except:
+        #     print('No internet')
 
-        try:
-            ctx.add_basemap(self.axes, crs=pyproj.CRS.from_epsg(4326),
-                            source=ctx.providers.OpenStreetMap.Mapnik)
-        except:
-            print('No internet')
-
-
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_hexbin(self, data1, data2, xlbl='Time', ylbl='ML',
                       xbin=None, xrng=None):
         """
         Update the hexbin plot.
 
@@ -232,15 +230,14 @@
 
         for tick in self.axes.get_xticklabels():
             tick.set_rotation(90)
 
         cbar = self.figure.colorbar(hbin[3])
         cbar.set_label('Number of Events')
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_hist(self, data1, xlbl='Data Value',
                     ylbl='Number of Observations', bins='doane', rng=None):
         """
         Update the histogram plot.
 
@@ -283,15 +280,14 @@
         if rng is not None:
             self.axes.set_xlim(rng[0], rng[1])
             self.axes.set_xticks(np.arange(int(rng[0]+1), int(rng[1])+1))
 
         for tick in self.axes.get_xticklabels():
             tick.set_rotation(90)
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_bvalue(self, data1a, bins='doane'):
         """
         Update the b value plot.
 
         Parameters
@@ -357,15 +353,14 @@
         self.axes.plot(xtmp, 10**np.poly1d(abvals)(xtmp), 'k', label=txt)
 
         self.axes.set_xlabel('ML', fontsize=8)
         self.axes.set_ylabel('Number of observations', fontsize=8)
 
         self.axes.legend()
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_pres(self, data1, phase='P'):
         """
         Update the plot.
 
         Parameters
@@ -405,15 +400,14 @@
 
         weights = 100*np.ones_like(ptres)/ptres.size
         self.axes.text(0.75, 0.9, txt, transform=self.axes.transAxes)
         self.axes.hist(ptres, 40, weights=weights, edgecolor='black')
         self.axes.set_xlabel('Time Residual (seconds)')
         self.axes.set_ylabel('Frequency (%)')
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_residual(self, dat, res='ML'):
         """
         Update the residual plot.
 
         Parameters
@@ -486,15 +480,14 @@
         self.axes.set_xticklabels(sname_list, rotation=90)
         self.axes.set_xlabel('Station Name')
         if res != 'ML':
             self.axes.set_ylabel('Travel Time Residual (Seconds)')
         else:
             self.axes.set_ylabel('ML-mean(ML)')
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_wadati(self, dat, min_wad=5, min_vps=1.53,
                       max_vps=1.93):
         """
         Update the wadati plot.
 
@@ -571,15 +564,14 @@
         self.axes.plot(x, np.poly1d([slope, intercept])(x), 'k')
 
         txt = 'Vp/Vs (Ave)='+str(np.around(np.mean(slope), 4))
         self.axes.text(0.1, 0.9, txt, transform=self.axes.transAxes)
         self.axes.set_xlabel('P Time (seconds)')
         self.axes.set_ylabel('S-P Time (seconds)')
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
 
 class GraphWindow(ContextModule):
     """Graph Window - The QDialog window which will contain our image."""
 
     def __init__(self, parent=None):
@@ -731,15 +723,15 @@
 
         """
         self.show()
         data = self.indata['Seis']
         self.datd = import_for_plots(data)
 
         if not self.datd:
-            self.showprocesslog('There is no compatible data in the file')
+            self.showlog('There is no compatible data in the file')
             return
 
         products = ['Hour Histogram',
                     'Month Histogram',
                     'Year Histogram',
                     'Number of Stations',
                     'RMS of time residuals',
@@ -789,47 +781,23 @@
         if os.path.isfile(ifile):
             tmp = ifile[:-4]
             os.remove(tmp+'.shp')
             os.remove(tmp+'.shx')
             os.remove(tmp+'.prj')
             os.remove(tmp+'.dbf')
 
-        driver = ogr.GetDriverByName('ESRI Shapefile')
-        data_source = driver.CreateDataSource(ifile)
-
-        # create the spatial reference, WGS84
-        srs = osr.SpatialReference()
-        srs.ImportFromEPSG(4326)
-        srs.SetAxisMappingStrategy(osr.OAMS_TRADITIONAL_GIS_ORDER)
-
-        # create the layer
-        layer = data_source.CreateLayer('Fault Plane Solution', srs,
-                                        ogr.wkbPolygon)
-
-        # Calculate BeachBall
         indata = self.mmc.ellipses
-        for pvert in indata:
-            # Create Geometry
-            outring = ogr.Geometry(ogr.wkbLinearRing)
-            for i in pvert:
-                outring.AddPoint(i[0], i[1])
+        geom = [Polygon(i) for i in indata]
 
-            poly = ogr.Geometry(ogr.wkbPolygon)
-            poly.AddGeometry(outring)
+        gdict = {'geometry': geom}
 
-            feature = ogr.Feature(layer.GetLayerDefn())
+        gdf = gpd.GeoDataFrame(gdict)
+        gdf = gdf.set_crs(4326)
 
-            feature.SetGeometry(poly)
-            # Create the feature in the layer (shapefile)
-            layer.CreateFeature(feature)
-            # Destroy the feature to free resources
-
-            feature.Destroy()
-
-        data_source.Destroy()
+        gdf.to_file(filename)
 
         return True
 
 
 def import_for_plots(dat):
     """
     Import data to plot.
@@ -920,70 +888,22 @@
 def _testfn():
     """Test routine."""
     import sys
     from pygmi.seis.iodefs import ImportSeisan
 
     app = QtWidgets.QApplication(sys.argv)
     tmp = ImportSeisan()
-    tmp.ifile = r"D:\Workdata\PyGMI Test Data\Sesimology\collect2.out"
+    tmp.ifile = r"D:\Workdata\PyGMI Test Data\Seismology\collect2.out"
     tmp.settings(True)
 
     data = tmp.outdata['Seis']
 
-    dat = import_for_plots(data)
+    # dat = import_for_plots(data)
 
     tmp = PlotQC()
     tmp.indata['Seis'] = data
     tmp.run()
     tmp.exec_()
 
 
-def _testfn2():
-    """Test for wave files."""
-    import sys
-    import matplotlib.pyplot as plt
-    from pygmi.seis.iodefs import ImportSeisan
-
-    ifile = r'D:\Workdata\seismology\april2021\collect.out'
-
-    app = QtWidgets.QApplication(sys.argv)
-    tmp = ImportSeisan()
-    tmp.ifile = ifile
-    tmp.settings(True)
-
-    data = tmp.outdata['Seis']
-
-    ifile = r'D:\Workdata\seismology\april2021\mulplt.wav'
-
-    with open(ifile, encoding='utf-8') as pntfile:
-        ltmp = pntfile.read()
-
-    ltmp = ltmp.split('\n')
-
-    l1 = ltmp.pop(0)
-    l2 = ltmp.pop(0)
-
-    while len(ltmp) > 2:
-        h1 = ltmp.pop(0)
-        h2 = ltmp.pop(0).split()
-
-        samples = int(h2[0])
-        rate = float(h2[1])
-        comp = h2[5]
-        year = h2[6]
-        month = h2[7]
-        day = h2[8]
-
-        lines = samples // 7 + 1
-        y = ''.join(ltmp[:lines]).split()
-        y = np.array(y, dtype=float)
-        x = np.arange(0, samples*rate, rate)
-
-        ltmp = ltmp[lines:]
-
-        plt.title(comp)
-        plt.plot(x, y)
-        plt.show()
-
-
 if __name__ == "__main__":
     _testfn()
```

### Comparing `pygmi-3.2.6.5/pygmi/seis/iodefs.py` & `pygmi-3.2.7.16/pygmi/seis/iodefs.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
         os.chdir(os.path.dirname(self.ifile))
 
         with open(self.ifile, encoding='utf-8') as pntfile:
             ltmp = pntfile.readlines()
 
         if len(ltmp[0]) < 80:
-            self.showprocesslog('Error: Problem with file')
+            self.showlog('Error: Problem with file')
             return False
 
         # This constructs a dictionary of functions
         read_record_type = {}
         read_record_type['1'] = read_record_type_1
         read_record_type['2'] = read_record_type_2
         read_record_type['3'] = read_record_type_3
@@ -299,30 +299,30 @@
                                 'line: '+str(iii+1), i]
                         file_errors.append(errs)
 
         has_errors = any('Error' in s for s in file_errors)
 
         if file_errors:
             if has_errors is False:
-                self.showprocesslog('Warning: Problem with file')
-                self.showprocesslog('Process will continue, but please '
-                                    'see warnings in '+self.ifile+'.log')
+                self.showlog('Warning: Problem with file')
+                self.showlog('Process will continue, but please '
+                             'see warnings in '+self.ifile+'.log')
             else:
-                self.showprocesslog('Error: Problem with file')
-                self.showprocesslog('Process stopping, please see errors '
-                                    'in '+self.ifile+'.log')
-            fout = open(self.ifile+'.log', 'w', encoding='utf-8')
-            for i in file_errors:
-                fout.write(i[0]+'\n')
-                fout.write(i[1]+'\n')
-            fout.close()
+                self.showlog('Error: Problem with file')
+                self.showlog('Process stopping, please see errors '
+                             'in '+self.ifile+'.log')
+            with open(self.ifile+'.log', 'w', encoding='utf-8') as fout:
+                for i in file_errors:
+                    fout.write(i[0]+'\n')
+                    fout.write(i[1]+'\n')
+
             if has_errors is True:
                 return False
         else:
-            self.showprocesslog('No errors in the file')
+            self.showlog('No errors in the file')
 
         if event:
             dat.append(event)
 
         self.outdata['Seis'] = dat
         return True
 
@@ -408,15 +408,14 @@
     tmp.type_of_magnitude_3 = i[75]
     tmp.magnitude_reporting_agency_3 = i[76:79]
 
     # make sure coordinates have the correct range
     tmp.longitude = ((tmp.longitude - 180) % 360) - 180
     tmp.latitude = ((tmp.latitude - 90) % 180) - 90
 
-
     return tmp
 
 
 def read_record_type_2(i):
     """
     Read record type 2.
 
@@ -944,41 +943,44 @@
 
         Returns
         -------
         None.
 
         """
         if 'Seis' not in self.indata:
-            self.showprocesslog(
+            self.showlog(
                 'Error: You need to have a SEISAN data first!')
             return
 
+        self.parent.process_is_active(True)
+
         data = self.indata['Seis']
 
         filename, _ = QtWidgets.QFileDialog.getSaveFileName(self.parent,
                                                             'Save File',
                                                             '.', 'out (*.out)')
 
         if filename == '':
+            self.parent.process_is_active(False)
             return
 
         os.chdir(os.path.dirname(filename))
 
-        self.fobj = open(filename, 'w', encoding='utf-8')
-
-        for i in data:
-            self.write_record_type_1(i)
-            self.write_record_type_f(i)  # This is missing  some #3 recs
-            self.write_record_type_m(i)  # This is missing  some #3 recs
-            self.write_record_type_e(i)
-            self.write_record_type_i(i)  # This is missing  some #3 recs
-            self.write_record_type_4(i)
-            self.fobj.write(' \n')
+        with open(filename, 'w', encoding='utf-8') as self.fobj:
+            for i in self.piter(data):
+                self.write_record_type_1(i)
+                self.write_record_type_f(i)  # This is missing  some #3 recs
+                self.write_record_type_m(i)  # This is missing  some #3 recs
+                self.write_record_type_e(i)
+                self.write_record_type_i(i)  # This is missing  some #3 recs
+                self.write_record_type_4(i)
+                self.fobj.write(' \n')
 
-        self.fobj.close()
+        self.showlog('Export to Seisan Finished!')
+        self.parent.process_is_active(False)
 
     def write_record_type_1(self, data):
         """
         Write record type 1.
 
         Parameters
         ----------
@@ -1446,29 +1448,28 @@
 
         Returns
         -------
         None.
 
         """
         if 'Seis' not in self.indata:
-            self.showprocesslog(
-                'Error: You need to have a SEISAN data first!')
+            self.showlog('Error: You need to have a SEISAN data first!')
             return
+        self.parent.process_is_active(True)
 
         data = self.indata['Seis']
 
         filename, _ = QtWidgets.QFileDialog.getSaveFileName(self.parent,
                                                             'Save File',
                                                             '.', 'csv (*.csv)')
         if filename == '':
+            self.parent.process_is_active(False)
             return
         os.chdir(os.path.dirname(filename))
 
-        self.fobj = open(filename, 'w', encoding='utf-8')
-
         headi = ('last_action_done, date_time_of_last_action, operator, '
                  'status, id, new_id_created, id_locked, ')
 
         head1 = ('year, month, day, fixed_origin_time, hour, minutes, '
                  'seconds, location_model_indicator, distance_indicator, '
                  'event_id, latitude, longitude, depth, depth_indicator, '
                  'locating_indicator, hypocenter_reporting_agency, '
@@ -1485,27 +1486,29 @@
         head4 = ('station_name, instrument_type, dat.component, quality, '
                  'phase_id, weighting_indicator, flag_auto_pick, '
                  'first_motion, hour, minutes, seconds, duration, amplitude, '
                  'period, direction_of_approach, phase_velocity, '
                  'angle_of_incidence, azimuth_residual, travel_time_residual, '
                  'weight, epicentral_distance, azimuth_at_source, ')
 
-        self.fobj.write(headi+head1+heade+head4+'\n')
+        with open(filename, 'w', encoding='utf-8') as self.fobj:
+            self.fobj.write(headi+head1+heade+head4+'\n')
 
-        for i in data:
-            reci = self.write_record_type_i(i)
-            rec1 = self.write_record_type_1(i)
-            rece = self.write_record_type_e(i)
-            rec4 = self.write_record_type_4(i)
-            for j in rec4:
-                jtmp = reci+rec1+rece+j+'\n'
-                jtmp = jtmp.replace('nan', '')
-                self.fobj.write(jtmp)
+            for i in self.piter(data):
+                reci = self.write_record_type_i(i)
+                rec1 = self.write_record_type_1(i)
+                rece = self.write_record_type_e(i)
+                rec4 = self.write_record_type_4(i)
+                for j in rec4:
+                    jtmp = reci+rec1+rece+j+'\n'
+                    jtmp = jtmp.replace('nan', '')
+                    self.fobj.write(jtmp)
 
-        self.fobj.close()
+        self.showlog('Export to csv Finished!')
+        self.parent.process_is_active(False)
 
     def write_record_type_1(self, data):
         """
         Write record type 1.
 
         Parameters
         ----------
@@ -1986,47 +1989,49 @@
 
         Returns
         -------
         None.
 
         """
         if 'Seis' not in self.indata:
-            self.showprocesslog('Error: You need to have a SEISAN data first!')
+            self.showlog('Error: You need to have a SEISAN data first!')
             return
+        self.parent.process_is_active(True)
 
         data = self.indata['Seis']
 
         ext = ('csv (*.csv);;'
                'Excel (*.xlsx);;'
                'Shapefile (*.shp)')
 
         filename, filt = QtWidgets.QFileDialog.getSaveFileName(self.parent,
                                                                'Save File',
                                                                '.', ext)
         if filename == '':
+            self.parent.process_is_active(False)
             return
         os.chdir(os.path.dirname(filename))
 
         head = ["Year", "Month", "Day", "Hour", "Minute", "Second",
                 "Latitude", "Longitude", "Depth", "Ml", "Mw", "Md", "Mb",
                 "Ms", "RMS", "LatitudeError",
-                "LongitudeError", "DepthError", "Mo", "SourceRaduis",
+                "LongitudeError", "DepthError", "Mo", "SourceRadius",
                 "StressDrop", "F0", "StdDeviation", "Mercalli",
                 "Agency", "Description"]
 
         df = pd.DataFrame(columns=head)
 
         mtype = {}
         mtype['L'] = 'Ml'
         mtype['B'] = 'Mb'
         mtype['S'] = 'Ms'
         mtype['C'] = 'Md'
         mtype['W'] = 'Mw'
 
-        for i, idat in enumerate(data):
+        for i, idat in enumerate(self.piter(data)):
             ML = None
             if '1' in idat:
                 dat = idat['1']
                 df.loc[i, 'Year'] = dat.year
                 df.loc[i, 'Month'] = dat.month
                 df.loc[i, 'Day'] = dat.day
                 df.loc[i, 'Hour'] = dat.hour
@@ -2071,14 +2076,17 @@
             df.to_excel(filename, index=False)
         elif filt == 'Shapefile (*.shp)':
             geom = gpd.points_from_xy(df.Longitude, df.Latitude)
             gdf = gpd.GeoDataFrame(df, geometry=geom)
             gdf = gdf.set_crs("EPSG:4326")
             gdf.to_file(filename)
 
+        self.showlog('Export Summary Finished!')
+        self.parent.process_is_active(False)
+
 
 def mercalli(mag):
     """
     Return Mercalli index.
 
     Parameters
     ----------
@@ -2335,15 +2343,15 @@
                                 continue
                             newkey = rectype+'_'+j
                             if newkey not in datd:
                                 datd[newkey] = []
                             datd[newkey].append(tmp[j])
 
         slist = []
-        for event in datd.keys():
+        for event in datd:
             datd[event] = [min(datd[event]), max(datd[event])]
             if isinstance(datd[event][0], str):
                 slist.append(event)
 
         for i in slist:
             del datd[i]
```

### Comparing `pygmi-3.2.6.5/pygmi/seis/utils.py` & `pygmi-3.2.7.16/pygmi/seis/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,20 +188,20 @@
                 continue
             text = i['3'].region
 
             cmatch = difflib.get_close_matches(text, masterlist, 1, cutoff=0.7)
             if cmatch:
                 cmatch = cmatch[0]
             else:
-                # self.showprocesslog('No match found for '+text)
+                # self.showlog('No match found for '+text)
                 nomatch.append(text)
                 continue
 
             if cmatch != text:
-                # self.showprocesslog('Correcting '+text+' to '+cmatch)
+                # self.showlog('Correcting '+text+' to '+cmatch)
                 correction.append(text+' to '+cmatch)
                 i['3'].region = cmatch
 
         self.outdata['Seis'] = data
 
 
 def _testfn():
```

### Comparing `pygmi-3.2.6.5/pygmi/test/test_cluster.py` & `pygmi-3.2.7.16/pygmi/test/test_cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,23 +23,27 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 """
 These are tests. Run pytest on this file from within this directory to do
 the tests.
 """
 
+import os
+import psutil
 import sys
 from PyQt5 import QtWidgets
 import numpy as np
 
 from pygmi.raster.datatypes import Data
 from pygmi.clust import cluster, crisp_clust, fuzzy_clust
 
 APP = QtWidgets.QApplication(sys.argv)  # Necessary to test Qt Classes
 
+os.environ['LOKY_MAX_CPU_COUNT'] = str(psutil.cpu_count(logical=False))
+
 
 def test_cluster():
     """test cluster."""
 
     dat1 = Data()
     dat1.data = np.ma.identity(3)
     dat1.data.mask = np.zeros([3, 3])
@@ -119,8 +123,8 @@
     if datout2[0, 0] == 2:
         datout = np.abs(datout-3)
 
     np.testing.assert_array_equal(datout2, datout)
 
 
 if __name__ == "__main__":
-    test_fuzzy()
+    test_crisp()
```

### Comparing `pygmi-3.2.6.5/pygmi/test/test_gravity.py` & `pygmi-3.2.7.16/pygmi/test/test_gravity.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     IO.settings(True)
 
     # Process Data
     PD = dataprep.ProcessData()
     PD.indata = IO.outdata
     PD.settings(True)
 
-    datout = PD.outdata['Line']
+    datout = PD.outdata['Vector'][0]
 
-    boug = datout['Gravity']['BOUGUER']
+    boug = datout['BOUGUER']
     boug = np.array(boug)
 
     datout2 = np.array([-716.5271207830797, -716.5167383494435,
                         -716.3040775379834, -716.3141448945184,
                         -716.1779168502552, -716.2380602844478,
                         -716.0745685905054, -716.0335678754984,
                         -716.0125048061484, -715.9501174250662,
```

### Comparing `pygmi-3.2.6.5/pygmi/test/test_mag.py` & `pygmi-3.2.7.16/pygmi/test/test_mag.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
            [0.0, 0.0]]
     t22 = [[0.0, 0.0],
            [0.0, 0.0]]
     ta2 = [[1.8572654805528055e-17, 1.8572654805528055e-17],
            [1.8572654805528055e-17, 1.8572654805528055e-17]]
     tdx2 = [[0.30816907111598496, 0.30816907111598496],
             [0.30816907111598496, 0.30816907111598496]]
-    t1, th, t2, ta, tdx = dataprep.tilt1(datin, 90, 0)
+    t1, th, t2, ta, tdx, _ = dataprep.tilt1(datin, 90, 0)
 
     np.testing.assert_array_equal(t1, t12)
     np.testing.assert_array_equal(th, th2)
     np.testing.assert_array_equal(t2, t22)
     np.testing.assert_array_equal(ta, ta2)
     np.testing.assert_array_equal(tdx, tdx2)
 
@@ -115,15 +115,15 @@
                               [1, .5, .1, 0, 0]])
 
     tmp = tiltdepth.TiltDepth(None)
     tmp.indata = {'Raster': [datin]}
     tmp.dsb_dec.setValue(0.)
     tmp.dsb_inc.setValue(90.)
     tmp.settings(True)
-    tmp.change_band1()
+    tmp.calculate()
 
     datout2 = tmp.depths
 
     datout = np.array([[3.93612464, -1.99438548, 1., 0.32962923],
                        [3.49438548, -2.49438548, 1., 0.34958333],
                        [2.99438548, -2.99438548, 1., 0.34958333],
                        [2.49438548, -3.49438548, 1., 0.34958333],
@@ -132,8 +132,8 @@
                        [1.98888969, -1.98888969, 2., 0.36451351],
                        [2.48888969, -1.48759916, 2., 0.36542720]])
 
     np.testing.assert_array_almost_equal(datout2, datout)
 
 
 if __name__ == "__main__":
-    test_IGRF()
+    test_tilt()
```

### Comparing `pygmi-3.2.6.5/pygmi/test/test_pfmod.py` & `pygmi-3.2.7.16/pygmi/test/test_pfmod.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 These are pfmod tests. Run this file from within this directory to do the
 tests.
 """
 
 import numpy as np
 import matplotlib.pyplot as plt
 import PIL
+import PIL.ImageDraw
 
 from pygmi.pfmod.grvmag3d import quick_model
 from pygmi.pfmod.grvmag3d import calc_field
 
 
 def main():
     """
@@ -53,17 +54,17 @@
 
     from IPython import get_ipython
     get_ipython().run_line_magic('matplotlib', 'inline')
 
     print('Testing modelling of gravity and potential field data')
 
     ifile = 'testdata/block'
-    # ifile = 'data/dyke'
+    ifile = 'testdata/dyke'
     samplescale = 1.  # Horizontal scale of the samples.
-    power = 1.  # This parameter changes thinkness of voxels with depth.
+    power = 2.  # This parameter changes thinkness of voxels with depth.
     print('File:', ifile)
     print('Sample Scale:', samplescale)
     print('Power:', power)
 
     with open(ifile+'.ecs', encoding='utf-8') as fnr:
         tmp = fnr.read()
```

### Comparing `pygmi-3.2.6.5/pygmi/test/test_raster.py` & `pygmi-3.2.7.16/pygmi/test/test_raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,15 @@
     np.testing.assert_array_equal(dat, dat2)
 
 
 @pytest.fixture
 def smalldata():
     """Small test dataset."""
     dat = Data()
+    dat.dataid = 'test'
     dat.data = np.ma.array([[29000., 29000.], [29000., 29000.]],
                            mask=[[0, 0], [0, 0]])
     dat.set_transform(1, 25, 1, -27)
     dat.crs = CRS.from_epsg(4326)
 
     return dat
 
@@ -541,8 +542,14 @@
                        [1e+20, 0, 0, 0, 0, 0, 1e+20],
                        [1e+20, 1e+20, 1e+20, 1e+20, 1e+20, 1e+20, 1e+20]])
 
     np.testing.assert_array_almost_equal(datout2, datout)
 
 
 if __name__ == "__main__":
-    test_vertical()
+    dat = Data()
+    dat.data = np.ma.array([[29000., 29000.], [29000., 29000.]],
+                           mask=[[0, 0], [0, 0]])
+    dat.dataid = 'test'
+    dat.set_transform(1, 25, 1, -27)
+    dat.crs = CRS.from_epsg(4326)
+    test_io_ascii(dat)
```

### Comparing `pygmi-3.2.6.5/pygmi/vector/dataprep.py` & `pygmi-3.2.7.16/pygmi/vector/dataprep.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,25 @@
 # -----------------------------------------------------------------------------
 """Data Preparation for Vector Data."""
 
 import os
 import copy
 from PyQt5 import QtWidgets, QtCore, QtGui
 import numpy as np
-import matplotlib.path as mplPath
+# import matplotlib.path as mplPath
 from scipy.interpolate import griddata
 from scipy.ndimage import distance_transform_edt
 import geopandas as gpd
 from pyproj import CRS, Transformer
 
-
 from pygmi import menu_default
 from pygmi.raster.dataprep import GroupProj
 from pygmi.raster.datatypes import Data
 from pygmi.vector.minc import minc
-from pygmi.misc import BasicModule
+from pygmi.misc import BasicModule, ContextModule
 
 
 class PointCut(BasicModule):
     """
     Cut Data using shapefiles.
 
     This class cuts point datasets using a boundary defined by a polygon
@@ -64,20 +63,18 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
-        if 'Line' in self.indata:
-            data = copy.deepcopy(self.indata['Line'])
-            key = list(data.keys())[0]
-            data = data[key]
+        if 'Vector' in self.indata:
+            data = copy.deepcopy(self.indata['Vector'][0])
         else:
-            self.showprocesslog('No point data')
+            self.showlog('No point data')
             return False
 
         # nodialog = False
         if not nodialog:
             ext = 'Shape file (*.shp)'
             self.ifile, _ = QtWidgets.QFileDialog.getOpenFileName(
                 self.parent, 'Open Shape File', '.', ext)
@@ -93,15 +90,15 @@
                    'the shapefile.')
             QtWidgets.QMessageBox.warning(self.parent, 'Error', err,
                                           QtWidgets.QMessageBox.Ok)
             return False
 
         if self.pbar is not None:
             self.pbar.to_max()
-        self.outdata['Line'] = {key: data}
+        self.outdata['Vector'] = [data]
 
         return True
 
     def loadproj(self, projdata):
         """
         Load project data into class.
 
@@ -225,20 +222,18 @@
         """
         txt = str(self.dsb_dxy.text())
         if txt.replace('.', '', 1).isdigit():
             self.dxy = float(self.dsb_dxy.text())
         else:
             return
 
-        key = list(self.indata['Line'].keys())[0]
-        data = self.indata['Line'][key]
-        data = data.dropna()
+        data = self.indata['Vector'][0]
 
-        x = data.pygmiX.values
-        y = data.pygmiY.values
+        x = data.geometry.x.values
+        y = data.geometry.y.values
 
         cols = round(x.ptp()/self.dxy)
         rows = round(y.ptp()/self.dxy)
 
         self.label_rows.setText('Rows: '+str(rows))
         self.label_cols.setText('Columns: '+str(cols))
 
@@ -270,40 +265,40 @@
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
         tmp = []
-        if 'Line' not in self.indata:
-            self.showprocesslog('No Point Data')
+        if 'Vector' not in self.indata:
+            self.showlog('No Point Data')
             return False
 
-        self.dataid.clear()
+        data = self.indata['Vector'][0]
 
-        key = list(self.indata['Line'].keys())[0]
-        data = self.indata['Line'][key]
-        data = data.dropna()
+        if data.geom_type.iloc[0] != 'Point':
+            self.showlog('No Point Data')
+            return False
+
+        self.dataid.clear()
 
         filt = ((data.columns != 'geometry') &
-                (data.columns != 'line') &
-                (data.columns != 'pygmiX') &
-                (data.columns != 'pygmiY'))
+                (data.columns != 'line'))
 
         cols = list(data.columns[filt])
         self.dataid.addItems(cols)
 
         if self.dataid_text is None:
             self.dataid_text = self.dataid.currentText()
         if self.dataid_text in cols:
             self.dataid.setCurrentText(self.dataid_text)
 
         if self.dxy is None:
-            x = data.pygmiX.values
-            y = data.pygmiY.values
+            x = data.geometry.x.values
+            y = data.geometry.y.values
 
             dx = x.ptp()/np.sqrt(x.size)
             dy = y.ptp()/np.sqrt(y.size)
             self.dxy = max(dx, dy)
             self.dxy = min([x.ptp(), y.ptp(), self.dxy])
 
         self.dsb_dxy.setText(f'{self.dxy:.8f}')
@@ -315,15 +310,15 @@
                 return False
 
         try:
             float(self.dsb_dxy.text())
             float(self.dsb_null.text())
             float(self.bdist.text())
         except ValueError:
-            self.showprocesslog('Value Error')
+            self.showlog('Value Error')
             return False
 
         self.acceptall()
 
         return True
 
     def loadproj(self, projdata):
@@ -381,76 +376,37 @@
         None.
 
         """
         dxy = float(self.dsb_dxy.text())
         method = self.grid_method.currentText()
         nullvalue = float(self.dsb_null.text())
         bdist = float(self.bdist.text())
-        key = list(self.indata['Line'].keys())[0]
-        data = self.indata['Line'][key]
-        data = data.dropna()
+        data = self.indata['Vector'][0]
+        dataid = self.dataid.currentText()
         newdat = []
 
         if bdist < 1:
             bdist = None
-            self.showprocesslog('Blanking distance too small.')
+            self.showlog('Blanking distance too small.')
 
-        filt = (data[self.dataid.currentText()] != nullvalue)
-        x = data.pygmiX.values[filt]
-        y = data.pygmiY.values[filt]
-        z = data[self.dataid.currentText()].values[filt]
-
-        if method == 'Minimum Curvature':
-            gdat = minc(x, y, z, dxy, showprocesslog=self.showprocesslog,
-                        bdist=bdist)
-            gdat = np.ma.filled(gdat, fill_value=nullvalue)
-        else:
-            extent = np.array([x.min(), x.max(), y.min(), y.max()])
-
-            rows = int((extent[3] - extent[2])/dxy+1)
-            cols = int((extent[1] - extent[0])/dxy+1)
-
-            xxx = np.linspace(extent[0], extent[1], cols)
-            yyy = np.linspace(extent[2], extent[3], rows)
-            xxx, yyy = np.meshgrid(xxx, yyy)
-
-            points = np.transpose([x.flatten(), y.flatten()])
-
-            if method == 'Nearest Neighbour':
-                gdat = griddata(points, z, (xxx, yyy), method='nearest')
-                gdat = blanking(gdat, x, y, bdist, extent, dxy, nullvalue)
-            elif method == 'Linear':
-                gdat = griddata(points, z, (xxx, yyy), method='linear',
-                                fill_value=nullvalue)
-                gdat = blanking(gdat, x, y, bdist, extent, dxy, nullvalue)
-            elif method == 'Cubic':
-                gdat = griddata(points, z, (xxx, yyy), method='cubic',
-                                fill_value=nullvalue)
-                gdat = blanking(gdat, x, y, bdist, extent, dxy, nullvalue)
-
-            gdat = gdat[::-1]
-        gdat = np.ma.masked_equal(gdat, nullvalue)
-
-        # Create dataset
-        dat = Data()
-        dat.data = gdat
-        dat.nodata = nullvalue
-        dat.dataid = self.dataid.currentText()
+        data2 = data[['geometry', dataid]]
+        data2 = data2.dropna()
 
-        rows, _ = dat.data.shape
+        filt = (data2[dataid] != nullvalue)
+        x = data2.geometry.x.values[filt]
+        y = data2.geometry.y.values[filt]
+        z = data2[dataid].values[filt]
 
-        left = x.min()
-        top = y.min() + dxy*rows
-
-        dat.set_transform(dxy, left, dxy, top)
+        dat = gridxyz(x, y, z, dxy, nullvalue, method, bdist, self.showlog)
+        dat.dataid = dataid
 
         newdat.append(dat)
 
         self.outdata['Raster'] = newdat
-        self.outdata['Line'] = self.indata['Line']
+        self.outdata['Vector'] = self.indata['Vector']
 
 
 class DataReproj(BasicModule):
     """
     Reprojections.
 
     This class reprojects datasets using the rasterio routines.
@@ -507,42 +463,32 @@
 
         Returns
         -------
         None.
 
         """
         if self.in_proj.wkt == 'Unknown' or self.out_proj.wkt == 'Unknown':
-            self.showprocesslog('Could not reproject')
+            self.showlog('Could not reproject')
             return
 
-        key = list(self.indata['Line'].keys())[0]
-        data = self.indata['Line'][key]
+        data = self.indata['Vector'][0]
 
         # Input stuff
         orig_wkt = self.in_proj.wkt
 
         # Output stuff
         targ_wkt = self.out_proj.wkt
 
-        x2, y2 = reprojxy(data.pygmiX, data.pygmiY, orig_wkt, targ_wkt)
-
-        xy = np.transpose([x2, y2])
+        data.set_crs(CRS.from_wkt(orig_wkt), inplace=True)
+        data.to_crs(CRS.from_wkt(targ_wkt), inplace=True)
 
-        if np.inf in xy:
-            self.showprocesslog('Note: inf values in reprojected results. '
-                                'Please check your input and output '
-                                'projections or input x and y data for '
-                                'mistakes.')
-
-        data = data.assign(Xnew=xy[:, 0])
-        data = data.assign(Ynew=xy[:, 1])
-        data.pygmiX = xy[:, 0]
-        data.pygmiY = xy[:, 1]
+        data = data.assign(Xnew=data.geometry.x.values)
+        data = data.assign(Ynew=data.geometry.y.values)
 
-        self.outdata['Line'] = {key: data}
+        self.outdata['Vector'] = [data]
 
     def settings(self, nodialog=False):
         """
         Entry point into item.
 
         Parameters
         ----------
@@ -551,47 +497,46 @@
 
         Returns
         -------
         bool
             True if successful, False otherwise.
 
         """
-        if 'Line' not in self.indata and 'Vector' not in self.indata:
-            self.showprocesslog('No vector data.')
+        if 'Vector' not in self.indata:
+            self.showlog('No vector data.')
             return False
 
-        if 'Vector' in self.indata:
-            firstkey = next(iter(self.indata['Vector'].keys()))
-            self.orig_wkt = self.indata['Vector'][firstkey].crs.to_wkt()
+        if self.indata['Vector'][0].crs is not None:
+            self.orig_wkt = self.indata['Vector'][0].crs.to_wkt()
 
         if self.orig_wkt is None:
             indx = self.in_proj.combodatum.findText(r'WGS 84')
             self.in_proj.combodatum.setCurrentIndex(indx)
             self.orig_wkt = self.in_proj.wkt
         else:
             self.in_proj.set_current(self.orig_wkt)
+
         if self.targ_wkt is None:
             indx = self.in_proj.combodatum.findText(r'WGS 84')
             self.out_proj.combodatum.setCurrentIndex(indx)
             self.targ_wkt = self.out_proj.wkt
         else:
             self.out_proj.set_current(self.targ_wkt)
 
         if not nodialog:
             tmp = self.exec_()
 
             if tmp != 1:
                 return False
 
         if 'Vector' in self.indata:
-            self.outdata['Vector'] = {}
-            for i in self.indata['Vector']:
-                ivec = self.indata['Vector'][i]
-                ivec.set_crs(self.in_proj.wkt)
-                self.outdata['Vector'][i] = ivec.to_crs(self.out_proj.wkt)
+            self.outdata['Vector'] = []
+            for ivec in self.indata['Vector']:
+                ivec = ivec.set_crs(self.in_proj.wkt)
+                self.outdata['Vector'].append(ivec.to_crs(self.out_proj.wkt))
         else:
             self.acceptall()
 
         return True
 
     def loadproj(self, projdata):
         """
@@ -627,14 +572,163 @@
 
         projdata['orig_wkt'] = self.in_proj.wkt
         projdata['targ_wkt'] = self.out_proj.wkt
 
         return projdata
 
 
+class Metadata(ContextModule):
+    """
+    Edit Metadata.
+
+    This class allows the editing of the metadata for a vector dataset using a
+    GUI.
+
+    Attributes
+    ----------
+    banddata : dictionary
+        band data
+    bandid : dictionary
+        dictionary of strings containing band names.
+    """
+
+    def __init__(self, parent=None):
+        super().__init__(parent)
+
+        self.combobox_bandid = QtWidgets.QComboBox()
+        self.proj = GroupProj('Input Projection')
+
+        self.setupui()
+
+    def setupui(self):
+        """
+        Set up UI.
+
+        Returns
+        -------
+        None.
+
+        """
+        gridlayout_main = QtWidgets.QGridLayout(self)
+        buttonbox = QtWidgets.QDialogButtonBox()
+
+        label_bandid = QtWidgets.QLabel('Source:')
+
+        buttonbox.setOrientation(QtCore.Qt.Horizontal)
+        buttonbox.setCenterButtons(True)
+        buttonbox.setStandardButtons(buttonbox.Cancel | buttonbox.Ok)
+
+        self.setWindowTitle('Vector Dataset Metadata')
+
+        gridlayout_main.addWidget(label_bandid, 0, 0, 1, 1)
+        gridlayout_main.addWidget(self.combobox_bandid, 0, 1, 1, 3)
+        gridlayout_main.addWidget(self.proj, 2, 0, 1, 4)
+        gridlayout_main.addWidget(buttonbox, 4, 0, 1, 4)
+
+        buttonbox.accepted.connect(self.accept)
+        buttonbox.rejected.connect(self.reject)
+
+        self.resize(-1, 320)
+
+    def acceptall(self):
+        """
+        Accept option.
+
+        Returns
+        -------
+        None.
+
+        """
+        wkt = self.proj.wkt
+
+        for tmp in self.indata['Vector']:
+            if wkt == 'None':
+                tmp.crs = None
+            else:
+                tmp.crs = CRS.from_wkt(wkt)
+
+    def run(self):
+        """
+        Entry point to start this routine.
+
+        Returns
+        -------
+        tmp : bool
+            True if successful, False otherwise.
+
+        """
+        bandid = []
+        if self.indata['Vector'][0].crs is None:
+            self.proj.set_current('None')
+        else:
+            self.proj.set_current(self.indata['Vector'][0].crs.to_wkt())
+
+        for i in self.indata['Vector']:
+            if 'source' in i.attrs:
+                bandid.append(i.attrs['source'])
+            else:
+                bandid.append('Unknown')
+
+        self.combobox_bandid.addItems(bandid)
+
+        tmp = self.exec_()
+
+        if tmp != 1:
+            return False
+
+        self.acceptall()
+
+        return True
+
+
+def blanking(gdat, x, y, bdist, extent, dxy, nullvalue):
+    """
+    Blanks area further than a defined number of cells from input data.
+
+    Parameters
+    ----------
+    gdat : numpy array
+        grid data to blank.
+    x : numpy array
+        x coordinates.
+    y : numpy array
+        y coordinates.
+    bdist : int
+        Blanking distance in units for cell.
+    extent : list
+        extent of grid.
+    dxy : float
+        Cell size.
+    Nullvalue : float
+        Null or nodata value.
+
+    Returns
+    -------
+    mask : numpy array
+        Mask to be used for blanking.
+
+    """
+    mask = np.zeros_like(gdat)
+
+    points = np.transpose([x, y])
+
+    for xy in points:
+        col = int((xy[0]-extent[0])/dxy)
+        row = int((xy[1]-extent[2])/dxy)
+
+        mask[row, col] = 1
+
+    dist = distance_transform_edt(np.logical_not(mask))
+    mask = (dist > bdist)
+
+    gdat[mask] = nullvalue
+
+    return gdat
+
+
 def cut_point(data, ifile):
     """
     Cuts a point dataset.
 
     Cut a point dataset using a shapefile.
 
     Parameters
@@ -645,62 +739,80 @@
         shapefile used to cut data
 
     Returns
     -------
     data : Data
         PyGMI Dataset
     """
-    # shapef = ogr.Open(ifile)
-    # if shapef is None:
-    #     return None
-    # lyr = shapef.GetLayer()
-    # poly = lyr.GetNextFeature()
-    # if lyr.GetGeomType() is not ogr.wkbPolygon or poly is None:
-    #     shapef = None
-    #     return None
-
-    # points = []
-    # geom = poly.GetGeometryRef()
-
-    # ifin = 0
-    # imax = 0
-    # if geom.GetGeometryName() == 'MULTIPOLYGON':
-    #     for i in range(geom.GetGeometryCount()):
-    #         geom.GetGeometryRef(i)
-    #         itmp = geom.GetGeometryRef(i)
-    #         itmp = itmp.GetGeometryRef(0).GetPointCount()
-    #         if itmp > imax:
-    #             imax = itmp
-    #             ifin = i
-    #     geom = geom.GetGeometryRef(ifin)
-
-    # pts = geom.GetGeometryRef(0)
-    # for pnt in range(pts.GetPointCount()):
-    #     points.append((pts.GetX(pnt), pts.GetY(pnt)))
-
     gdf = gpd.read_file(ifile)
     gdf = gdf[gdf.geometry != None]
 
-    if 'Polygon' in gdf.geom_type.iloc[0]:
-        dat = gdf.geometry.iloc[0]
+    if 'Polygon' not in gdf.geom_type.iloc[0]:
+        return None
 
-    points = list(dat.exterior.coords)
+    data = gpd.clip(data, gdf)
 
-    bbpath = mplPath.Path(points)
+    return data
 
-    chk = bbpath.contains_points(np.transpose([data.pygmiX.values,
-                                               data.pygmiY.values]))
 
-    data = data[chk]
+def gridxyz(x, y, z, dxy, nullvalue=1e+20, method='Nearest Neighbour',
+            bdist=4.0, showlog=print):
+    """Grid data."""
+    if bdist < 1:
+        bdist = None
+        showlog('Blanking distance too small.')
+
+    if method == 'Minimum Curvature':
+        gdat = minc(x, y, z, dxy, showlog=showlog,
+                    bdist=bdist)
+        gdat = np.ma.filled(gdat, fill_value=nullvalue)
+    else:
+        extent = np.array([x.min(), x.max(), y.min(), y.max()])
 
-    # shapef = None
-    return data
+        rows = int((extent[3] - extent[2])/dxy+1)
+        cols = int((extent[1] - extent[0])/dxy+1)
+
+        xxx = np.linspace(extent[0], extent[1], cols)
+        yyy = np.linspace(extent[2], extent[3], rows)
+        xxx, yyy = np.meshgrid(xxx, yyy)
+
+        points = np.transpose([x.flatten(), y.flatten()])
+
+        if method == 'Nearest Neighbour':
+            gdat = griddata(points, z, (xxx, yyy), method='nearest')
+            gdat = blanking(gdat, x, y, bdist, extent, dxy, nullvalue)
+        elif method == 'Linear':
+            gdat = griddata(points, z, (xxx, yyy), method='linear',
+                            fill_value=nullvalue)
+            gdat = blanking(gdat, x, y, bdist, extent, dxy, nullvalue)
+        elif method == 'Cubic':
+            gdat = griddata(points, z, (xxx, yyy), method='cubic',
+                            fill_value=nullvalue)
+            gdat = blanking(gdat, x, y, bdist, extent, dxy, nullvalue)
 
+        gdat = gdat[::-1]
+    gdat = np.ma.masked_equal(gdat, nullvalue)
 
-def quickgrid(x, y, z, dxy, numits=4, showprocesslog=print):
+    # Create dataset
+    dat = Data()
+    dat.data = gdat
+    dat.nodata = nullvalue
+    # dat.dataid = self.dataid.currentText()
+
+    rows, _ = dat.data.shape
+
+    left = x.min()
+    top = y.min() + dxy*rows
+
+    dat.set_transform(dxy, left, dxy, top)
+
+    return dat
+
+
+def quickgrid(x, y, z, dxy, numits=4, showlog=print):
     """
     Do a quick grid.
 
     Parameters
     ----------
     x : numpy array
         array of x coordinates
@@ -709,23 +821,23 @@
     z : numpy array
         array of z values - this is the column being gridded
     dxy : float
         cell size for the grid, in both the x and y direction.
     numits : int
         number of iterations. By default its 4. If this is negative, a maximum
         will be calculated and used.
-    showprocesslog : function, optional
+    showlog : function, optional
         Routine to show text messages. The default is print.
 
     Returns
     -------
     newz : numpy array
         M x N array of z values
     """
-    showprocesslog('Creating Grid')
+    showlog('Creating Grid')
     x = x.flatten()
     y = y.flatten()
     z = z.flatten()
 
     xmin = x.min()
     xmax = x.max()
     ymin = y.min()
@@ -766,68 +878,23 @@
         else:
             xx, yy = newmask.nonzero()
             xx2 = xx//jj
             yy2 = yy//jj
             zfin[xx, yy] = newz[xx2, yy2]
             newmask[xx, yy] = np.logical_not(zdiv[xx2, yy2])
 
-        showprocesslog('Iteration done: '+str(j+1)+' of '+str(numits))
+        showlog('Iteration done: '+str(j+1)+' of '+str(numits))
 
-    showprocesslog('Finished!')
+    showlog('Finished!')
 
     newz = np.ma.array(zfin)
     newz.mask = newmask
     return newz
 
 
-def blanking(gdat, x, y, bdist, extent, dxy, nullvalue):
-    """
-    Blanks area further than a defined number of cells from input data.
-
-    Parameters
-    ----------
-    gdat : numpy array
-        grid data to blank.
-    x : numpy array
-        x coordinates.
-    y : numpy array
-        y coordinates.
-    bdist : int
-        Blanking distance in units for cell.
-    extent : list
-        extent of grid.
-    dxy : float
-        Cell size.
-    Nullvalue : float
-        Null or nodata value.
-
-    Returns
-    -------
-    mask : numpy array
-        Mask to be used for blanking.
-
-    """
-    mask = np.zeros_like(gdat)
-
-    points = np.transpose([x, y])
-
-    for xy in points:
-        col = int((xy[0]-extent[0])/dxy)
-        row = int((xy[1]-extent[2])/dxy)
-
-        mask[row, col] = 1
-
-    dist = distance_transform_edt(np.logical_not(mask))
-    mask = (dist > bdist)
-
-    gdat[mask] = nullvalue
-
-    return gdat
-
-
 def reprojxy(x, y, iwkt, owkt):
     """
     Reproject x and y coordinates.
 
     Parameters
     ----------
     x : numpy array or float
@@ -862,61 +929,46 @@
 
     return xout, yout
 
 
 def _testfn():
     """Test routine."""
     import sys
-    import matplotlib.pyplot as plt
-    from pygmi.vector.iodefs import ImportLineData
+    from pygmi.vector.iodefs import ImportXYZ
 
     app = QtWidgets.QApplication(sys.argv)
 
     ifile = r"D:\Workdata\PyGMI Test Data\Vector\Line Data\SPECARCHIVE.XYZ"
 
-    IO = ImportLineData()
+    IO = ImportXYZ()
     IO.ifile = ifile
     IO.filt = 'Geosoft XYZ (*.xyz)'
     IO.settings(True)
 
-    # DG = DataGrid()
-    # DG.indata = IO.outdata
-    # DG.settings()
-
-    # dat = DG.outdata['Raster'][0].data
-
-    # plt.imshow(dat)
-    # plt.show()
-
-    DR = DataReproj()
-    DR.indata = IO.outdata
-    DR.settings()
-
-    breakpoint()
+    MD = Metadata()
+    MD.indata = IO.outdata
+    MD.run()
 
 
 def _testfn_pointcut():
     """Test routine."""
     import sys
-    from pygmi.vector.iodefs import ImportLineData
+    from pygmi.vector.iodefs import ImportXYZ
 
     app = QtWidgets.QApplication(sys.argv)
 
     ifile = r"D:\Workdata\PyGMI Test Data\Vector\linecut\test2.csv"
     sfile = r"D:\Workdata\PyGMI Test Data\Vector\linecut\test2_cut_outline.shp"
 
-    IO = ImportLineData()
+    IO = ImportXYZ()
     IO.ifile = ifile
     IO.filt = 'Comma Delimited (*.csv)'
     IO.settings(True)
 
     DR = PointCut()
     DR.indata = IO.outdata
     DR.ifile = sfile
     DR.settings(True)
 
-    breakpoint()
-
-
 
 if __name__ == "__main__":
-    _testfn_pointcut()
+    _testfn()
```

### Comparing `pygmi-3.2.6.5/pygmi/vector/graphs.py` & `pygmi-3.2.7.16/pygmi/vector/graphs.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,27 +29,29 @@
 from PyQt5 import QtWidgets, QtCore
 from scipy.stats import median_abs_deviation
 import matplotlib.collections as mc
 from matplotlib import colormaps
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qt5 import NavigationToolbar2QT
-from pandas.api.types import is_numeric_dtype
+# from pandas.api.types import is_numeric_dtype
 
 from pygmi.misc import frm, ContextModule
 
 
 class GraphWindow(ContextModule):
     """Graph Window - Main QT Dialog class for graphs."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.setAttribute(QtCore.Qt.WA_DeleteOnClose)
         self.setWindowTitle('Graph Window')
 
+        self.data = None
+
         vbl = QtWidgets.QVBoxLayout(self)  # self is where layout is assigned
         hbl = QtWidgets.QHBoxLayout()
         self.mmc = MyMplCanvas(self)
         mpl_toolbar = NavigationToolbar2QT(self.mmc, self.parent)
 
         self.combobox1 = QtWidgets.QComboBox()
         self.combobox2 = QtWidgets.QComboBox()
@@ -95,15 +97,15 @@
     """
     MPL Canvas class.
 
     This routine will also allow the picking and movement of nodes of data.
     """
 
     def __init__(self, parent=None):
-        fig = Figure()
+        fig = Figure(layout='constrained')
         self.axes = fig.add_subplot(111)
         self.line = None
         self.ind = None
         self.background = None
         self.pickevents = False
 
         super().__init__(fig)
@@ -242,57 +244,14 @@
 
         self.line, = self.axes.plot(r, data, '.-')
         self.line.set_picker(True)
         self.line.set_pickradius(5)
 
         self.figure.canvas.draw()
 
-    def update_map(self, xdata, ydata, zdata):
-        """
-        Update the map from point data.
-
-        Parameters
-        ----------
-        xdata : numpy array
-            1D x-data array.
-        ydata : numpy array
-            1D y-data array.
-        zdata : numpy array
-            1D z-data array.
-
-        Returns
-        -------
-        None.
-
-        """
-        self.figure.clear()
-
-        ax1 = self.figure.add_subplot(111, label='Map')
-        ax1.ticklabel_format(style='plain')
-
-        self.axes = ax1
-        self.axes.tick_params(axis='x', rotation=90)
-        self.axes.tick_params(axis='y', rotation=0)
-
-        self.figure.canvas.draw()
-        self.background = self.figure.canvas.copy_from_bbox(ax1.bbox)
-
-        if is_numeric_dtype(zdata):
-            scat = ax1.scatter(xdata, ydata, c=zdata, cmap=colormaps['jet'])
-        else:
-            return
-
-        self.figure.colorbar(scat, ax=ax1, format=frm)
-
-        self.axes.xaxis.set_major_formatter(frm)
-        self.axes.yaxis.set_major_formatter(frm)
-
-        self.figure.tight_layout()
-        self.figure.canvas.draw()
-
     def update_lmap(self, data, ival, scale, uselabels):
         """
         Update the plot from line data.
 
         Parameters
         ----------
         data : Pandas dataframe
@@ -315,15 +274,14 @@
         self.axes = ax1
         self.axes.ticklabel_format(useOffset=False, style='plain')
         self.axes.tick_params(axis='x', rotation=90)
         self.axes.tick_params(axis='y', rotation=0)
 
         self.figure.canvas.draw()
         self.background = self.figure.canvas.copy_from_bbox(ax1.bbox)
-        data = data.dropna()
 
         zdata = data[ival]
         med = np.median(zdata)
         std = 2.5 * median_abs_deviation(zdata, axis=None, scale=1/1.4826)
 
         if std == 0:
             std = 1
@@ -332,30 +290,31 @@
         spcing = np.array([])
 
         datagrp = data.groupby('line')
         datagrp = list(datagrp)
 
         for line in datagrp:
             data1 = line[1]
-            x = data1.pygmiX.values
-            y = data1.pygmiY.values
+            data1 = data1.dropna(subset=ival)
+            x = data1.geometry.x.values
+            y = data1.geometry.y.values
             z = data1[ival]
 
             if x.size < 2:
                 continue
 
             spcing = np.append(spcing, np.sqrt(np.diff(x)**2+np.diff(y)**2))
 
         spcing = spcing.mean()
 
         for line in datagrp:
             data1 = line[1]
 
-            x = data1.pygmiX.values
-            y = data1.pygmiY.values
+            x = data1.geometry.x.values
+            y = data1.geometry.y.values
             z = data1[ival]
 
             if x.size < 2:
                 continue
 
             ang = np.arctan2((y[1:]-y[:-1]), (x[1:]-x[:-1]))
             ang = np.append(ang, ang[-1])
@@ -376,15 +335,15 @@
                 ax1.text(x[0], y[0], line[0], rotation=textang)
             ax1.plot(x, y, 'c')
             ax1.plot(qx, qy, 'k')
 
         self.axes.xaxis.set_major_formatter(frm)
         self.axes.yaxis.set_major_formatter(frm)
 
-        self.figure.tight_layout()
+        # self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_vector(self, data, col):
         """
         Update the plot from vector data.
 
         Parameters
@@ -401,62 +360,54 @@
         """
         self.figure.clear()
 
         self.axes = self.figure.add_subplot(111, label='map')
         self.axes.ticklabel_format(style='plain')
         self.axes.tick_params(axis='x', rotation=90)
         self.axes.tick_params(axis='y', rotation=0)
+        self.axes.axis('equal')
 
-        if 'LineString' in data:
-            tmp = []
-            for i in data['LineString'].geometry:
-                if i.type == 'MultiLineString':
-                    for j in i:
-                        tmp.append(np.array(j.coords[:]))
-                else:
-                    tmp.append(np.array(i.coords[:]))
-
-            lcol = mc.LineCollection(tmp)
-            self.axes.add_collection(lcol)
-            self.axes.autoscale()
-            self.axes.axis('equal')
-        elif 'Polygon' in data:
+        if 'LineString' in data.geom_type.iloc[0]:
             tmp = []
-            for i in data['Polygon'].geometry:
-                tmp.append(np.array(i.exterior.coords[:])[:, :2].tolist())
+            for i in data.geometry:
+                tmp.append(np.array(i.coords[:]))
 
             lcol = mc.LineCollection(tmp)
             self.axes.add_collection(lcol)
             self.axes.autoscale()
-            self.axes.axis('equal')
-
-        elif 'MultiPolygon' in data:
+            # self.axes.axis('equal')
+        elif 'Polygon' in data.geom_type.iloc[0]:
             tmp = []
-            for j in data['MultiPolygon'].geometry:
-                for i in list(j.geoms):
-                    tmp.append(np.array(i.exterior.coords[:])[:, :2].tolist())
+            for j in data.geometry:
+                tmp.append(np.array(j.exterior.coords[:])[:, :2].tolist())
 
             lcol = mc.LineCollection(tmp)
             self.axes.add_collection(lcol)
             self.axes.autoscale()
-            self.axes.axis('equal')
+            # self.axes.axis('equal')
 
-        elif 'Point' in data:
+        elif 'Point' in data.geom_type.iloc[0]:
             if col != '':
-                self.axes.scatter(data['Point'].geometry.x,
-                                  data['Point'].geometry.y,
-                                  c=data['Point'][col])
+                dstd = data[col].std()
+                dmean = data[col].mean()
+                vmin = max(dmean-2*dstd, data[col].min())
+                vmax = min(dmean+2*dstd, data[col].max())
+
+                scat = self.axes.scatter(data.geometry.x,
+                                         data.geometry.y,
+                                         c=data[col], vmin=vmin, vmax=vmax)
+                self.figure.colorbar(scat, ax=self.axes, format=frm)
+
             else:
-                self.axes.scatter(data['Point'].geometry.x,
-                                  data['Point'].geometry.y)
+                self.axes.scatter(data.geometry.x,
+                                  data.geometry.y)
 
         self.axes.xaxis.set_major_formatter(frm)
         self.axes.yaxis.set_major_formatter(frm)
 
-        self.figure.tight_layout()
         self.figure.canvas.draw()
 
     def update_rose(self, data, rtype, nbins=8, equal=False):
         """
         Update the rose diagram plot using vector data.
 
         Parameters
@@ -493,16 +444,16 @@
         ax2.yaxis.set_major_formatter(frm)
 
         fangle = []
         fcnt = []
         flen = []
 
         allcrds = []
-        for i in data['LineString'].geometry:
-            if i.type == 'MultiLineString':
+        for i in data.geometry:
+            if i.geom_type == 'MultiLineString':
                 for j in i:
                     allcrds.append(np.array(j.coords[:]))
             else:
                 allcrds.append(np.array(i.coords[:]))
 
         for pnts in allcrds:
             pnts = np.transpose(pnts)
@@ -538,15 +489,15 @@
             bcols2 = bcols[(xtheta/bwidth).astype(int)]
             ax1.bar(xtheta, radii, width=bwidth, color=bcols2)
             ax1.bar(xtheta+np.pi, radii, width=bwidth, color=bcols2)
 
             bcols2 = bcols[(fangle/bwidth).astype(int)]
             lcol = mc.LineCollection(allcrds, color=bcols2)
             ax2.add_collection(lcol)
-            ax2.autoscale(enable=True, tight=True)
+            ax2.autoscale(enable=True)  # , tight=True)
 
         else:
             # Draw rose diagram base on one angle per linear segment, normed
             radii, theta = histogram(fcnt, y=flen, xmin=0., xmax=np.pi,
                                      bins=nbins)
             if equal is True:
                 radii = .01*radii.max()*np.sqrt(100*radii/radii.max())
@@ -555,80 +506,20 @@
             bcols2 = bcols[(xtheta/bwidth).astype(int)]
             ax1.bar(xtheta, radii, width=bwidth, color=bcols2)
             ax1.bar(xtheta+np.pi, radii, width=bwidth, color=bcols2)
 
             bcols2 = bcols[(fcnt/bwidth).astype(int)]
             lcol = mc.LineCollection(allcrds, color=bcols2)
             ax2.add_collection(lcol)
-            ax2.autoscale(enable=True, tight=True)
+            ax2.autoscale(enable=True)  # , tight=True)
 
-        self.figure.tight_layout()
+        # self.figure.tight_layout()
         self.figure.canvas.draw()
 
 
-class PlotPoints(GraphWindow):
-    """Plot Points Class."""
-
-    def __init__(self, parent=None):
-        super().__init__(parent)
-        self.spinbox.hide()
-        self.label3.hide()
-        self.combobox2.hide()
-        self.label2.hide()
-        self.xdata = None
-        self.ydata = None
-
-    def change_band(self):
-        """
-        Combo box to choose band.
-
-        Returns
-        -------
-        None.
-
-        """
-        key = list(self.indata['Line'].keys())[0]
-        data = self.indata['Line'][key]
-        data = data.dropna()
-        i = self.combobox1.currentText()
-
-        self.mmc.update_map(data.pygmiX, data.pygmiY, data[i])
-
-    def run(self):
-        """
-        Entry point to run class.
-
-        Returns
-        -------
-        None.
-
-        """
-        data = self.indata['Line']
-        data = list(data.values())[0]
-
-        filt = ((data.columns != 'geometry') &
-                (data.columns != 'line') &
-                (data.columns != 'pygmiX') &
-                (data.columns != 'pygmiY'))
-
-        cols = list(data.columns[filt])
-
-        if data.pygmiX.isna().min() == True:
-            self.showprocesslog('You do not have coordinates in that point '
-                                'dataset.')
-            return
-
-        self.show()
-
-        self.combobox1.addItems(cols)
-
-        self.label1.setText('Map')
-        self.combobox1.setCurrentIndex(0)
-
-
 class PlotLines(GraphWindow):
     """Plot Lines Class."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.spinbox.hide()
         self.label3.hide()
@@ -650,24 +541,24 @@
         Combo box to choose band.
 
         Returns
         -------
         None.
 
         """
-        key = list(self.indata['Line'].keys())[0]
-        data = self.indata['Line'][key]
-        data = data.dropna()
+        if self.data is None:
+            return
 
         line = self.combobox1.currentText()
         col = self.combobox2.currentText()
 
-        data2 = data[data.line == line]
-        x = data2.pygmiX.values
-        y = data2.pygmiY.values
+        data2 = self.data[self.data.line == line]
+        data2 = data2.dropna(subset=col)
+        x = data2.geometry.x.values
+        y = data2.geometry.y.values
 
         data2 = data2[col].values
 
         r = np.sqrt((x[1:]-x[:-1])**2+(y[1:]-y[:-1])**2)
         r = np.cumsum(r)
         r = np.concatenate(([0.], r))
 
@@ -678,27 +569,33 @@
         Entry point to run class.
 
         Returns
         -------
         None.
 
         """
+        self.data = None
+        for i in self.indata['Vector']:
+            if i.geom_type.iloc[0] == 'Point':
+                self.data = i
+                break
+
+        if self.data is None:
+            self.showlog('No point type data.')
+            return
+
         self.combobox1.currentIndexChanged.disconnect()
         self.combobox2.currentIndexChanged.disconnect()
 
         self.show()
 
-        data = self.indata['Line']
-        data = list(data.values())[0]
-        filt = ((data.columns != 'geometry') &
-                (data.columns != 'line') &
-                (data.columns != 'pygmiX') &
-                (data.columns != 'pygmiY'))
-        cols = list(data.columns[filt])
-        lines = data.line[data.line != 'nan'].unique()
+        filt = ((self.data.columns != 'geometry') &
+                (self.data.columns != 'line'))
+        cols = list(self.data.columns[filt])
+        lines = self.data.line[self.data.line != 'nan'].unique()
 
         self.combobox1.addItems(lines)
         self.combobox2.addItems(cols)
 
         self.label1.setText('Line:')
         self.label2.setText('Column:')
 
@@ -725,43 +622,51 @@
         Combo box to choose band.
 
         Returns
         -------
         None.
 
         """
-        key = list(self.indata['Line'].keys())[0]
-        data = self.indata['Line'][key]
-        data = data.dropna()
+        if self.data is None:
+            return
 
         scale = self.spinbox.value()
         i = self.combobox1.currentText()
+        data = self.data.dropna(subset=i)
+
         self.mmc.update_lmap(data, i, scale, self.checkbox.isChecked())
 
     def run(self):
         """
         Entry point to run class.
 
         Returns
         -------
         None.
 
         """
+        self.data = None
+        for i in self.indata['Vector']:
+            if i.geom_type.iloc[0] == 'Point':
+                self.data = i
+                break
+
+        if self.data is None:
+            self.showlog('No point type data.')
+            return
+
         self.combobox1.currentIndexChanged.disconnect()
         self.spinbox.valueChanged.disconnect()
         self.checkbox.stateChanged.disconnect()
 
         self.show()
 
-        data = self.indata['Line']
-        data = list(data.values())[0]
+        data = self.indata['Vector'][0]
         filt = ((data.columns != 'geometry') &
-                (data.columns != 'line') &
-                (data.columns != 'pygmiX') &
-                (data.columns != 'pygmiY'))
+                (data.columns != 'line'))
         cols = list(data.columns[filt])
         self.combobox1.addItems(cols)
 
         self.checkbox.setText('Show Line Labels:')
         self.label1.setText('Column:')
         self.label3.setText('Scale:')
         self.spinbox.setMinimum(1)
@@ -787,106 +692,119 @@
         self.spinbox.setValue(8)
         self.spinbox.setMinimum(2)
         self.spinbox.setMaximum(360)
         self.checkbox.show()
 
         self.setWindowTitle('Rose Diagram')
         if parent is None:
-            self.showprocesslog = print
+            self.showlog = print
         else:
-            self.showprocesslog = parent.showprocesslog
+            self.showlog = parent.showlog
 
     def change_band(self):
         """
         Combo box to choose band.
 
         Returns
         -------
         None.
 
         """
-        if 'Vector' not in self.indata:
+        if self.data is None:
             return
-        data = self.indata['Vector']
+
         i = self.combobox1.currentIndex()
         equal = self.checkbox.isChecked()
-        if 'LineString' in data:
-            self.mmc.update_rose(data, i, self.spinbox.value(), equal)
-        else:
-            self.showprocesslog('No line type data.')
-            return
+
+        self.mmc.update_rose(self.data, i, self.spinbox.value(), equal)
 
     def run(self):
         """
         Entry point to run class.
 
         Returns
         -------
         None.
 
         """
+        self.data = None
+        if 'Vector' not in self.indata:
+            return
+        for i in self.indata['Vector']:
+            if i.geom_type.iloc[0] == 'LineString':
+                self.data = i
+                break
+
+        if self.data is None:
+            self.showlog('No line type data.')
+            return
+
         self.show()
         self.combobox1.addItem('Average Angle per Feature')
         self.combobox1.addItem('Angle per segment in Feature')
         self.checkbox.setText('Equal Area Rose Diagram')
         self.label1.setText('Rose Diagram Type:')
         self.combobox1.setCurrentIndex(0)
 
 
 class PlotVector(GraphWindow):
     """Plot Vector Class."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
-        self.label1.hide()
+        # self.label1.hide()
         self.combobox2.hide()
         self.label2.hide()
         self.spinbox.hide()
         self.label3.hide()
 
     def change_band(self):
         """
         Combo box to choose band.
 
         Returns
         -------
         None.
 
         """
-        data = self.indata['Vector']
+        if self.data is None:
+            return
+
         i = self.combobox1.currentText()
+        data = self.data.dropna(subset=i)
+        if data.size == 0:
+            i = ''
+            data = self.data
 
         self.mmc.update_vector(data, i)
 
     def run(self):
         """
         Entry point to run class.
 
         Returns
         -------
         None.
 
         """
-        data = self.indata['Vector']
-        key = list(data.keys())[0]
-        data = data[key]
-        data = data.select_dtypes(include='number')
+        self.data = self.indata['Vector'][0]
+        # self.data = self.data.select_dtypes(include='number')
 
-        filt = ((data.columns != 'geometry') &
-                (data.columns != 'line') &
-                (data.columns != 'pygmiX') &
-                (data.columns != 'pygmiY'))
+        # filt = ((self.data.columns != 'geometry') &
+        #         (self.data.columns != 'line'))
 
-        cols = list(data.columns[filt])
+        cols = list(self.data.select_dtypes(include=np.number).columns)
         if len(cols) > 0:
             self.combobox1.addItems(cols)
             self.combobox1.setCurrentIndex(0)
         else:
             self.combobox1.hide()
 
+        self.label1.setText('Channel:')
+
         self.show()
 
         self.change_band()
 
 
 def histogram(x, y=None, xmin=None, xmax=None, bins=10):
     """
```

### Comparing `pygmi-3.2.6.5/pygmi/vector/menu.py` & `pygmi-3.2.7.16/pygmi/vector/menu.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,30 +43,27 @@
     parent : pygmi.main.MainWidget
         Reference to MainWidget class found in main.py
     """
 
     def __init__(self, parent=None):
 
         self.parent = parent
-        self.parent.add_to_context('Line')
         self.parent.add_to_context('Vector')
         context_menu = self.parent.context_menu
 
         self.menufile = QtWidgets.QMenu('Vector')
         parent.menubar.addAction(self.menufile.menuAction())
 
-        self.action_import_shape_data = QtWidgets.QAction('Import Shapefile'
-                                                          ' Data')
-        self.menufile.addAction(self.action_import_shape_data)
-        self.action_import_shape_data.triggered.connect(self.import_shape_data)
-
-        self.action_import_line_data = QtWidgets.QAction('Import Point or Line'
-                                                         ' Data')
-        self.menufile.addAction(self.action_import_line_data)
-        self.action_import_line_data.triggered.connect(self.import_line_data)
+        self.action_import_vector = QtWidgets.QAction('Import Vector Data')
+        self.menufile.addAction(self.action_import_vector)
+        self.action_import_vector.triggered.connect(self.import_vector)
+
+        self.action_import_xyz = QtWidgets.QAction('Import XYZ Data')
+        self.menufile.addAction(self.action_import_xyz)
+        self.action_import_xyz.triggered.connect(self.import_xyz)
 
         self.menufile.addSeparator()
 
         self.action_cut_data = QtWidgets.QAction('Cut Points using Polygon')
         self.menufile.addAction(self.action_cut_data)
         self.action_cut_data.triggered.connect(self.cut_data)
 
@@ -77,81 +74,81 @@
         self.menufile.addSeparator()
 
         self.action_grid = QtWidgets.QAction('Dataset Gridding')
         self.menufile.addAction(self.action_grid)
         self.action_grid.triggered.connect(self.grid)
 
         # Context menus
-        context_menu['Line'].addSeparator()
+        context_menu['Vector'].addSeparator()
+
+        self.action_metadata = QtWidgets.QAction('Display/Edit Vector Metadata')
+        context_menu['Vector'].addAction(self.action_metadata)
+        self.action_metadata.triggered.connect(self.metadata)
 
-        self.action_show_line_data = QtWidgets.QAction('Show Line Data'
-                                                       ' Profile')
-        context_menu['Line'].addAction(self.action_show_line_data)
+        self.action_show_line_data = QtWidgets.QAction('Show Profile Data')
+        context_menu['Vector'].addAction(self.action_show_line_data)
         self.action_show_line_data.triggered.connect(self.show_line_data)
 
-        self.action_show_line_data2 = QtWidgets.QAction('Show Line Data Map')
-        context_menu['Line'].addAction(self.action_show_line_data2)
+        self.action_show_line_data2 = QtWidgets.QAction('Show Profiles on a '
+                                                        'Map')
+        context_menu['Vector'].addAction(self.action_show_line_data2)
         self.action_show_line_data2.triggered.connect(self.show_line_map)
 
-        self.action_show_point_data2 = QtWidgets.QAction('Show Point Data Map')
-        context_menu['Line'].addAction(self.action_show_point_data2)
-        self.action_show_point_data2.triggered.connect(self.show_point_map)
-
-        self.action_export_line = QtWidgets.QAction('Export Line Data')
-        context_menu['Line'].addAction(self.action_export_line)
-        self.action_export_line.triggered.connect(self.export_line)
-
-        context_menu['Vector'].addSeparator()
-
         self.action_show_vector_data = QtWidgets.QAction('Show Vector Data')
         context_menu['Vector'].addAction(self.action_show_vector_data)
         self.action_show_vector_data.triggered.connect(self.show_vector_data)
 
         self.action_show_rose_diagram = QtWidgets.QAction('Show Rose Diagram')
         context_menu['Vector'].addAction(self.action_show_rose_diagram)
         self.action_show_rose_diagram.triggered.connect(self.show_rose_diagram)
 
-        self.action_export_shape = QtWidgets.QAction('Export Shape Data')
-        context_menu['Vector'].addAction(self.action_export_shape)
-        self.action_export_shape.triggered.connect(self.export_shape)
+        context_menu['Vector'].addSeparator()
+
+        self.action_export_xyz = QtWidgets.QAction('Export XYZ Data')
+        context_menu['Vector'].addAction(self.action_export_xyz)
+        self.action_export_xyz.triggered.connect(self.export_xyz)
+
+        self.action_export_vector = QtWidgets.QAction('Export Vector Data')
+        context_menu['Vector'].addAction(self.action_export_vector)
+        self.action_export_vector.triggered.connect(self.export_vector)
 
     def grid(self):
         """Grid datasets."""
         self.parent.item_insert('Step', 'Dataset Gridding', dataprep.DataGrid)
 
     def cut_data(self):
         """Cut point data."""
         self.parent.item_insert('Step', 'Cut Points', dataprep.PointCut)
 
     def reproject(self):
         """Reproject point data."""
         self.parent.item_insert('Step', 'Reproject Vector Data',
                                 dataprep.DataReproj)
 
-    def export_line(self):
-        """Export line data."""
-        self.parent.launch_context_item(iodefs.ExportLine)
+    def export_xyz(self):
+        """Export XYZ data."""
+        self.parent.launch_context_item(iodefs.ExportXYZ)
 
-    def export_shape(self):
+    def export_vector(self):
         """Export line data."""
-        self.parent.launch_context_item(iodefs.ExportShapeData)
+        self.parent.launch_context_item(iodefs.ExportVector)
 
-    def import_line_data(self):
-        """Import line data."""
-        self.parent.item_insert('Io', 'Import Line Data',
-                                iodefs.ImportLineData)
+    def import_xyz(self):
+        """Import XYZ data."""
+        self.parent.item_insert('Io', 'Import XYZ Data',
+                                iodefs.ImportXYZ)
 
-    def import_shape_data(self):
+    def import_vector(self):
         """Import shape data."""
-        self.parent.item_insert('Io', 'Import Shapefile Data',
-                                iodefs.ImportShapeData)
+        self.parent.item_insert('Io', 'Import Vector Data',
+                                iodefs.ImportVector)
 
-    def show_point_map(self):
-        """Show point data."""
-        self.parent.launch_context_item(graphs.PlotPoints)
+    def metadata(self):
+        """Metadata."""
+        self.parent.launch_context_item(dataprep.Metadata)
 
     def show_line_data(self):
         """Show line data."""
         self.parent.launch_context_item(graphs.PlotLines)
 
     def show_line_map(self):
         """Show line map."""
```

### Comparing `pygmi-3.2.6.5/pygmi/vector/minc.py` & `pygmi-3.2.7.16/pygmi/vector/minc.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,30 @@
 from operator import itemgetter
 import numpy as np
 from numba import jit
 from scipy.interpolate import griddata
 from scipy.ndimage import distance_transform_edt
 
 
-def minc(x, y, z, dxy, showprocesslog=print, extent=None, bdist=None,
+def minc(x, y, z, dxy, showlog=print, extent=None, bdist=None,
          maxiters=100):
     """
     Minimum Curvature Gridding.
 
     Parameters
     ----------
     x : numpy array
         1D array with x coordinates.
     y : numpy array
         1D array with y coordinates.
     z : numpy array
         1D array with z coordinates.
     dxy : float
         Cell x and y dimension.
-    showprocesslog : function, optional
+    showlog : function, optional
         Routine to show text messages. The default is print.
     extent : list, optional
         Extent defined as (left, right, bottom, top). The default is None.
     bdist : float, optional
         Blanking distance in units of cell. The default is None.
     maxiters : int, optional
         Maximum number of iterations. The default is 100.
@@ -81,15 +81,15 @@
 
     # Set extent
     if extent is None:
         extent = [x.min(), x.max(), y.min(), y.max()]
 
     extent = np.array(extent)
 
-    showprocesslog('Setting up grid...')
+    showlog('Setting up grid...')
 
     # Add buffer
     extent[0] -= dxy*3
     extent[1] += dxy*3
     extent[2] -= dxy*3
     extent[3] += dxy*3
 
@@ -104,27 +104,27 @@
 
     xxx = np.linspace(extent[0], extent[1], cols)
     yyy = np.linspace(extent[2], extent[3], rows)
     xxx, yyy = np.meshgrid(xxx, yyy)
 
     points = np.transpose([x.flatten(), y.flatten()])
 
-    showprocesslog('Creating nearest neighbour starting value...')
+    showlog('Creating nearest neighbour starting value...')
 
     u = griddata(points, z, (xxx, yyy), method='nearest')
     u = u[::-1]
 
     # define new grid
     ufixed = np.zeros((rows, cols), dtype=bool)
 
     x2 = x.flatten()
     y2 = y.flatten()
     z2 = z.flatten()
 
-    showprocesslog('Organizing input data...')
+    showlog('Organizing input data...')
 
     crds, blist = morg(x2, y2, z2, extent, dxy, rows, cols)
 
     coords = {}
     excludedpnts = 0
     for k, val in enumerate(crds):
         iint, jint, r, zval = val
@@ -141,15 +141,15 @@
             bmax = np.abs(b).max()
 
         if (iint, jint) not in coords:
             coords[iint, jint] = []
         coords[iint, jint].append([bmax, r, zval, b])
 
     if excludedpnts > 0:
-        showprocesslog(str(excludedpnts)+' point(s) excluded.')
+        showlog(str(excludedpnts)+' point(s) excluded.')
     # Choose only the closest coordinate per cell
     ijxyz = []
     for key in coords:
         iint, jint = key
         coords[key].sort(key=itemgetter(1))
         _, r, zval, _ = coords[key][0]
         if r < 0.05:
@@ -157,15 +157,15 @@
             ufixed[iint, jint] = True
             continue
         if 1 < iint < rows-2 and 1 < jint < cols-2:
             coords[key].sort()
             _, _, zval, b = coords[key][0]
             ijxyz.append([iint, jint, zval, b])
 
-    showprocesslog('Creating minimum curvature grid...')
+    showlog('Creating minimum curvature grid...')
     uold = np.zeros((rows, cols))
 
     # mean error per cell
     errdiff1 = np.abs(u-uold)
     errdiff = np.sum(errdiff1)/(rows*cols)
     errold = errdiff*1.1  # Starting 'old' error.
     errstd = errdiff1.std()*2.5
@@ -188,21 +188,21 @@
                     u[i, j] = tmp
 
         u = mcurv(u, ufixed)
 
         errdiff1 = np.abs(u-uold)
         errstd = errdiff1.std()*2.5
         errdiff = np.sum(errdiff1)/(rows*cols)
-        showprocesslog(f'Solution Error: {errdiff:.5f}')
+        showlog(f'Solution Error: {errdiff:.5f}')
 
         if errdiff > errold:
             u = uold
-            showprocesslog('Solution diverging. Stopping...')
+            showlog('Solution diverging. Stopping...')
             break
-    showprocesslog('Finished!')
+    showlog('Finished!')
 
     u = np.ma.array(u)
 
     # Trim buffer
     u = u[3:-3, 3:-3]
     ufixed = ufixed[3:-3, 3:-3]
 
@@ -633,30 +633,30 @@
 
 
 def _testfn():
     """Test routine."""
     import sys
     from PyQt5 import QtWidgets
     import matplotlib.pyplot as plt
-    from pygmi.vector.iodefs import ImportLineData
+    from pygmi.vector.iodefs import ImportXYZ
 
     app = QtWidgets.QApplication(sys.argv)
 
     ifile = r'c:\Workdata\vector\Line Data\MAGARCHIVE.XYZ'
 
-    IO = ImportLineData()
+    IO = ImportXYZ()
     IO.ifile = ifile
     IO.filt = 'Geosoft XYZ (*.xyz)'
     IO.settings(True)
 
-    dat = IO.outdata['Line']
+    dat = IO.outdata['Vector']
 
-    x = dat[ifile]['pygmiX'].to_numpy()
-    y = dat[ifile]['pygmiY'].to_numpy()
-    z = dat[ifile]['Column 8'].to_numpy()
+    x = dat.geometry.x.to_numpy()
+    y = dat.geometry.y.to_numpy()
+    z = dat['Column 8'].to_numpy()
 
     dxy = 125
 
     extent = np.array([x.min(), x.max(), y.min(), y.max()])
 
     odat = minc(x, y, z, dxy, extent=extent, bdist=4)
 
@@ -665,10 +665,9 @@
 
     plt.figure(dpi=150)
     plt.imshow(odat, extent=extent, vmin=vmin, vmax=vmax)
     plt.colorbar()
     plt.show()
 
 
-
 if __name__ == "__main__":
     _testfn()
```

### Comparing `pygmi-3.2.6.5/pygmi.egg-info/PKG-INFO` & `pygmi-3.2.7.16/pygmi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmi
-Version: 3.2.6.5
+Version: 3.2.7.16
 Summary: Python Geoscience Modelling and Interpretation
 Author-email: Patrick Cole <pcole@geoscience.org.za>
 Maintainer-email: Patrick Cole <pcole@geoscience.org.za>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, http://patrick-cole.github.io/pygmi/
 Project-URL: documentation, https://patrick-cole.github.io/pygmi/wiki.html
 Project-URL: repository, https://github.com/Patrick-Cole/pygmi.git
@@ -22,15 +22,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: COPYING
 
 Overview
 ========
 
@@ -57,45 +57,49 @@
 
 You may need to install the `Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019 <https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads>`_.
 
 If you have any comments or queries, you can contact the author either through `GitHub <https://github.com/Patrick-Cole/pygmi>`_ or via email at pcole@geoscience.org.za
 
 Requirements
 ------------
-PyGMI will run on both Windows and Linux. It should be noted that the main development is done in Python 3.10 on Windows.
+PyGMI will run on both Windows and Linux. It should be noted that the main development is done in Python 3.11 on Windows.
 
-PyGMI should still work with Python 3.8 and Python 3.9.
+PyGMI should still work with Python 3.9 and Python 3.10.
 
 PyGMI is developed and has been tested with the following libraries in order to function:
 
-* python 3.10.9
+* python 3.11.4
 * contextily 1.3.0
-* discretize 0.8.3
-* fiona 1.8.22
-* geopandas 0.12.1
-* llvmlite 0.39.1
-* matplotlib 3.7.1
+* discretize 0.9.0
+* fiona 1.9.4.post1
+* gdal 3.7.1
+* geopandas 0.13.2
+* llvmlite 0.40.1
+* matplotlib 3.7.2
 * mtpy 1.1.5
-* natsort 8.2.0
-* numba 0.56.4
+* natsort 8.4.0
+* numba 0.57.1
 * numexpr 2.8.4
-* numpy 1.23.5+mkl
-* pandas 1.5.2
-* pillow 9.3.0
-* psutil 5.9.0
-* pyopengl 3.1.6
-* pyproj 3.4.1
-* PyQt5 5.15.6
-* pytest 7.1.1
-* rasterio 1.3.4
-* scikit-image 0.19.3
-* scikit-learn 1.1.3
-* scipy 1.9.3
-* shapely 1.8.5.post1
-* SimPEG 0.18.1
+* numpy 1.24.4
+* openpyxl 3.1.2
+* pandas 2.0.3
+* pillow 10.0.0
+* psutil 5.9.5
+* pyogrio 0.6.0
+* pyopengl 3.1.7
+* pyproj 3.6.0
+* PyQt5 5.15.9
+* pytest 7.4.0
+* rasterio 1.3.8
+* scikit-image 0.21.0
+* scikit-learn 1.3.0
+* scipy 1.11.1
+* shapely 2.0.1
+* SimPEG 0.19.0
+* utm 0.7.0
 
 Installation
 ------------
 General (Not Anaconda)
 ----------------------
 The easiest way to install pygmi if you are working in a python environment is to use the pip command as follows:
 
@@ -128,15 +132,15 @@
 * numexpr
 * numba
 * llvmlite
 * GDAL
 * discretize
 * fiona
 
-They can be obtained from the `website <http://www.lfd.uci.edu/~gohlke/pythonlibs/>`_ by Christoph Gohlke.
+They can be obtained from the `website <https://www.cgohlke.com/>`_ by Christoph Gohlke.
 
 Linux
 -----
 Linux normally comes with python installed, but the additional libraries will still need to be installed.
 
 Typically, packages can be installed using pip. The process is as follows:
```

### Comparing `pygmi-3.2.6.5/pygmi.egg-info/SOURCES.txt` & `pygmi-3.2.7.16/pygmi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 pygmi/misc.py
 pygmi.egg-info/PKG-INFO
 pygmi.egg-info/SOURCES.txt
 pygmi.egg-info/dependency_links.txt
 pygmi.egg-info/entry_points.txt
 pygmi.egg-info/requires.txt
 pygmi.egg-info/top_level.txt
+pygmi/bholes/__init__.py
+pygmi/bholes/graphs.py
+pygmi/bholes/iodefs.py
+pygmi/bholes/menu.py
 pygmi/clust/__init__.py
 pygmi/clust/cluster.py
 pygmi/clust/crisp_clust.py
 pygmi/clust/fuzzy_clust.py
 pygmi/clust/graphs.py
 pygmi/clust/graphtool.py
 pygmi/clust/menu.py
@@ -69,20 +73,21 @@
 pygmi/helpdocs/pygmi.rsense.iodefs.importsentinel5p.html
 pygmi/helpdocs/pygmi.rsense.landsat_composite.html
 pygmi/helpdocs/pygmi.rsense.mnf.html
 pygmi/helpdocs/pygmi.rsense.pca.html
 pygmi/helpdocs/pygmi.rsense.pfeat.html
 pygmi/helpdocs/pygmi.rsense.ratios.html
 pygmi/helpdocs/pygmi.vector.dataprep.datagrid.html
-pygmi/helpdocs/pygmi.vector.iodefs.importpointdata.html
+pygmi/helpdocs/pygmi.vector.iodefs.importxyzdata.html
 pygmi/images/Help.png
 pygmi/images/bringtofront.png
 pygmi/images/cgslogo.png
 pygmi/images/delete.png
 pygmi/images/linepointer.png
+pygmi/images/load.png
 pygmi/images/logo256.ico
 pygmi/images/play.png
 pygmi/images/pointer.png
 pygmi/images/pygmi.png
 pygmi/images/sendtoback.png
 pygmi/mag/IGRF13.COF
 pygmi/mag/__init__.py
@@ -102,14 +107,15 @@
 pygmi/pfmod/grvmag3d.py
 pygmi/pfmod/iodefs.py
 pygmi/pfmod/menu.py
 pygmi/pfmod/misc.py
 pygmi/pfmod/mvis3d.py
 pygmi/pfmod/pfinvert.py
 pygmi/pfmod/pfmod.py
+pygmi/pfmod/show_table.py
 pygmi/pfmod/tab_mext.py
 pygmi/pfmod/tab_param.py
 pygmi/pfmod/tab_prof.py
 pygmi/raster/__init__.py
 pygmi/raster/anaglyph.py
 pygmi/raster/cooper.py
 pygmi/raster/dataprep.py
@@ -134,14 +140,15 @@
 pygmi/rsense/menu.py
 pygmi/rsense/ratios.py
 pygmi/rsense/transforms.py
 pygmi/seis/__init__.py
 pygmi/seis/beachball.py
 pygmi/seis/datatypes.py
 pygmi/seis/del_rec.py
+pygmi/seis/descriptions.txt
 pygmi/seis/graphs.py
 pygmi/seis/iodefs.py
 pygmi/seis/menu.py
 pygmi/seis/utils.py
 pygmi/test/__init__.py
 pygmi/test/test_cluster.py
 pygmi/test/test_gravity.py
```

### Comparing `pygmi-3.2.6.5/pyproject.toml` & `pygmi-3.2.7.16/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = 'pygmi'
 dynamic = ['version']
 authors = [{name = 'Patrick Cole', email = 'pcole@geoscience.org.za'}]
 maintainers = [{name = 'Patrick Cole', email = 'pcole@geoscience.org.za'}]
 description = 'Python Geoscience Modelling and Interpretation'
 readme = 'README.rst'
-requires-python = '>=3.8'
+requires-python = '>=3.9'
 license = {text = 'GNU General Public License v3 (GPLv3)'}
 keywords=['Geoscience', 'Geophysics', 'Magnetic', 'Gravity', 'Modelling',
           'Interpretation', 'Remote Sensing']
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Win32 (MS Windows)',
     'Environment :: X11 Applications :: Qt',
@@ -35,31 +35,34 @@
 dependencies = ['contextily',
                 'discretize',
                 'fiona',
                 'geopandas',
                 'llvmlite',
                 'matplotlib',
                 'mtpy',
+                'natsort',
                 'numba',
                 'numexpr',
                 'numpy',
-                'natsort',
+                'openpyxl',
                 'pandas',
                 'pillow',
                 'psutil',
+                'pyogrio',
                 'pyopengl',
                 'pyproj',
                 'PyQt5',
                 'pytest',
                 'rasterio',
                 'scikit-image',
                 'scikit-learn',
                 'scipy',
                 'shapely',
-                'SimPEG']
+                'SimPEG',
+                'utm']
 
 [project.urls]
 homepage = 'http://patrick-cole.github.io/pygmi/'
 documentation = 'https://patrick-cole.github.io/pygmi/wiki.html'
 repository =  'https://github.com/Patrick-Cole/pygmi.git'
 changelog = 'https://github.com/Patrick-Cole/pygmi/blob/pygmi3/CHANGES.rst'
```

