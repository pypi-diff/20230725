# Comparing `tmp/pythonbmp-1.0.3.tar.gz` & `tmp/pythonbmp-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonbmp-1.0.3.tar", last modified: Sun Jul 23 15:48:16 2023, max compression
+gzip compressed data, was "pythonbmp-1.0.4.tar", last modified: Tue Jul 25 04:49:51 2023, max compression
```

## Comparing `pythonbmp-1.0.3.tar` & `pythonbmp-1.0.4.tar`

### file list

```diff
@@ -1,41 +1,240 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 15:48:16.037345 pythonbmp-1.0.3/
--rw-rw-rw-   0        0        0     1090 2022-04-13 00:20:29.000000 pythonbmp-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      124 2023-07-23 12:29:53.000000 pythonbmp-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4309 2023-07-23 15:48:16.036344 pythonbmp-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2347 2023-07-23 12:57:58.000000 pythonbmp-1.0.3/README.md
--rw-rw-rw-   0        0        0      896 2023-07-23 15:44:02.000000 pythonbmp-1.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-23 15:48:15.913978 pythonbmp-1.0.3/pythonbmp/
--rw-rw-rw-   0        0        0   449728 2023-03-06 17:05:20.000000 pythonbmp-1.0.3/pythonbmp/BITMAPlib.py
--rw-rw-rw-   0        0        0    66015 2022-06-25 10:49:24.000000 pythonbmp-1.0.3/pythonbmp/X11colordict.py
--rw-rw-rw-   0        0        0    91943 2022-05-29 23:32:29.000000 pythonbmp-1.0.3/pythonbmp/XKCDcolordict.py
--rw-rw-rw-   0        0        0        0 2022-04-13 00:20:29.000000 pythonbmp-1.0.3/pythonbmp/__init__.py
--rw-rw-rw-   0        0        0      783 2022-09-04 13:43:04.000000 pythonbmp-1.0.3/pythonbmp/bmpconstants.py
--rw-rw-rw-   0        0        0     8335 2022-05-29 18:00:32.000000 pythonbmp-1.0.3/pythonbmp/bmppal.py
--rw-rw-rw-   0        0        0     1885 2022-05-29 18:03:32.000000 pythonbmp-1.0.3/pythonbmp/bufferflip.py
--rw-rw-rw-   0        0        0     1877 2022-05-31 12:10:53.000000 pythonbmp-1.0.3/pythonbmp/buffersplit.py
--rw-rw-rw-   0        0        0     6634 2022-05-31 12:10:53.000000 pythonbmp-1.0.3/pythonbmp/bufresize.py
--rw-rw-rw-   0        0        0     1401 2022-05-31 12:10:53.000000 pythonbmp-1.0.3/pythonbmp/chartools.py
--rw-rw-rw-   0        0        0     1422 2022-05-31 12:10:53.000000 pythonbmp-1.0.3/pythonbmp/charts.py
--rw-rw-rw-   0        0        0     4603 2022-05-29 22:58:36.000000 pythonbmp-1.0.3/pythonbmp/colordict.py
--rw-rw-rw-   0        0        0    28282 2022-09-19 08:21:23.000000 pythonbmp-1.0.3/pythonbmp/colors.py
--rw-rw-rw-   0        0        0     1575 2022-05-29 19:14:32.000000 pythonbmp-1.0.3/pythonbmp/conditionaltools.py
--rw-rw-rw-   0        0        0      853 2022-05-31 12:10:53.000000 pythonbmp-1.0.3/pythonbmp/dicttools.py
--rw-rw-rw-   0        0        0     1637 2022-06-05 11:41:44.000000 pythonbmp-1.0.3/pythonbmp/fileutils.py
--rw-rw-rw-   0        0        0   113333 2023-02-21 07:03:50.000000 pythonbmp-1.0.3/pythonbmp/fonts.py
--rw-rw-rw-   0        0        0    57313 2023-07-12 05:53:17.000000 pythonbmp-1.0.3/pythonbmp/fractals.py
--rw-rw-rw-   0        0        0      346 2022-06-09 11:01:53.000000 pythonbmp-1.0.3/pythonbmp/funcmeta.py
--rw-rw-rw-   0        0        0     2380 2022-08-27 08:50:11.000000 pythonbmp-1.0.3/pythonbmp/inttools.py
--rw-rw-rw-   0        0        0    44529 2022-10-04 08:21:21.000000 pythonbmp-1.0.3/pythonbmp/mathlib.py
--rw-rw-rw-   0        0        0     2498 2022-09-14 06:02:31.000000 pythonbmp-1.0.3/pythonbmp/messages.py
--rw-rw-rw-   0        0        0     9821 2022-08-30 02:29:48.000000 pythonbmp-1.0.3/pythonbmp/paramchecks.py
--rw-rw-rw-   0        0        0    40078 2022-09-07 22:46:41.000000 pythonbmp-1.0.3/pythonbmp/primitives2D.py
--rw-rw-rw-   0        0        0     1860 2022-06-05 03:55:11.000000 pythonbmp-1.0.3/pythonbmp/proctimer.py
--rw-rw-rw-   0        0        0      818 2022-08-30 12:38:45.000000 pythonbmp-1.0.3/pythonbmp/shims.py
--rw-rw-rw-   0        0        0    19674 2022-09-07 20:14:18.000000 pythonbmp-1.0.3/pythonbmp/solids3D.py
--rw-rw-rw-   0        0        0     1869 2022-07-21 16:34:56.000000 pythonbmp-1.0.3/pythonbmp/textgraphics.py
-drwxrwxrwx   0        0        0        0 2023-07-23 15:48:16.006351 pythonbmp-1.0.3/pythonbmp.egg-info/
--rw-rw-rw-   0        0        0     4309 2023-07-23 15:48:14.000000 pythonbmp-1.0.3/pythonbmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      823 2023-07-23 15:48:15.000000 pythonbmp-1.0.3/pythonbmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 15:48:14.000000 pythonbmp-1.0.3/pythonbmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-23 15:48:14.000000 pythonbmp-1.0.3/pythonbmp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 15:48:16.038350 pythonbmp-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:51.364934 pythonbmp-1.0.4/
+-rw-rw-rw-   0        0        0     1090 2022-04-13 00:20:29.000000 pythonbmp-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      139 2023-07-25 04:30:25.000000 pythonbmp-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4149 2023-07-25 04:49:51.362948 pythonbmp-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2187 2023-07-25 04:47:21.000000 pythonbmp-1.0.4/README.md
+-rw-rw-rw-   0        0        0      896 2023-07-25 04:31:47.000000 pythonbmp-1.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.186403 pythonbmp-1.0.4/pythonbmp/
+-rw-rw-rw-   0        0        0   449728 2023-03-06 17:05:20.000000 pythonbmp-1.0.4/pythonbmp/BITMAPlib.py
+-rw-rw-rw-   0        0        0    66015 2022-06-25 10:49:24.000000 pythonbmp-1.0.4/pythonbmp/X11colordict.py
+-rw-rw-rw-   0        0        0    91943 2022-05-29 23:32:29.000000 pythonbmp-1.0.4/pythonbmp/XKCDcolordict.py
+-rw-rw-rw-   0        0        0        0 2022-04-13 00:20:29.000000 pythonbmp-1.0.4/pythonbmp/__init__.py
+-rw-rw-rw-   0        0        0      783 2022-09-04 13:43:04.000000 pythonbmp-1.0.4/pythonbmp/bmpconstants.py
+-rw-rw-rw-   0        0        0     8335 2022-05-29 18:00:32.000000 pythonbmp-1.0.4/pythonbmp/bmppal.py
+-rw-rw-rw-   0        0        0     1885 2022-05-29 18:03:32.000000 pythonbmp-1.0.4/pythonbmp/bufferflip.py
+-rw-rw-rw-   0        0        0     1877 2022-05-31 12:10:53.000000 pythonbmp-1.0.4/pythonbmp/buffersplit.py
+-rw-rw-rw-   0        0        0     6634 2022-05-31 12:10:53.000000 pythonbmp-1.0.4/pythonbmp/bufresize.py
+-rw-rw-rw-   0        0        0     1401 2022-05-31 12:10:53.000000 pythonbmp-1.0.4/pythonbmp/chartools.py
+-rw-rw-rw-   0        0        0     1422 2022-05-31 12:10:53.000000 pythonbmp-1.0.4/pythonbmp/charts.py
+-rw-rw-rw-   0        0        0     4603 2022-05-29 22:58:36.000000 pythonbmp-1.0.4/pythonbmp/colordict.py
+-rw-rw-rw-   0        0        0    28282 2022-09-19 08:21:23.000000 pythonbmp-1.0.4/pythonbmp/colors.py
+-rw-rw-rw-   0        0        0     1575 2022-05-29 19:14:32.000000 pythonbmp-1.0.4/pythonbmp/conditionaltools.py
+-rw-rw-rw-   0        0        0      853 2022-05-31 12:10:53.000000 pythonbmp-1.0.4/pythonbmp/dicttools.py
+-rw-rw-rw-   0        0        0     1637 2022-06-05 11:41:44.000000 pythonbmp-1.0.4/pythonbmp/fileutils.py
+-rw-rw-rw-   0        0        0   113333 2023-02-21 07:03:50.000000 pythonbmp-1.0.4/pythonbmp/fonts.py
+-rw-rw-rw-   0        0        0    57313 2023-07-12 05:53:17.000000 pythonbmp-1.0.4/pythonbmp/fractals.py
+-rw-rw-rw-   0        0        0      346 2022-06-09 11:01:53.000000 pythonbmp-1.0.4/pythonbmp/funcmeta.py
+-rw-rw-rw-   0        0        0     2380 2022-08-27 08:50:11.000000 pythonbmp-1.0.4/pythonbmp/inttools.py
+-rw-rw-rw-   0        0        0    44529 2022-10-04 08:21:21.000000 pythonbmp-1.0.4/pythonbmp/mathlib.py
+-rw-rw-rw-   0        0        0     2498 2022-09-14 06:02:31.000000 pythonbmp-1.0.4/pythonbmp/messages.py
+-rw-rw-rw-   0        0        0     9821 2022-08-30 02:29:48.000000 pythonbmp-1.0.4/pythonbmp/paramchecks.py
+-rw-rw-rw-   0        0        0    40078 2022-09-07 22:46:41.000000 pythonbmp-1.0.4/pythonbmp/primitives2D.py
+-rw-rw-rw-   0        0        0     1860 2022-06-05 03:55:11.000000 pythonbmp-1.0.4/pythonbmp/proctimer.py
+-rw-rw-rw-   0        0        0      818 2022-08-30 12:38:45.000000 pythonbmp-1.0.4/pythonbmp/shims.py
+-rw-rw-rw-   0        0        0    19674 2022-09-07 20:14:18.000000 pythonbmp-1.0.4/pythonbmp/solids3D.py
+-rw-rw-rw-   0        0        0     1869 2022-07-21 16:34:56.000000 pythonbmp-1.0.4/pythonbmp/textgraphics.py
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.217405 pythonbmp-1.0.4/pythonbmp.egg-info/
+-rw-rw-rw-   0        0        0     4149 2023-07-25 04:49:49.000000 pythonbmp-1.0.4/pythonbmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9494 2023-07-25 04:49:49.000000 pythonbmp-1.0.4/pythonbmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 04:49:49.000000 pythonbmp-1.0.4/pythonbmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 04:49:49.000000 pythonbmp-1.0.4/pythonbmp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.236406 pythonbmp-1.0.4/samples/
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.333403 pythonbmp-1.0.4/samples/3d/
+-rw-rw-rw-   0        0        0     4170 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_3D.py
+-rw-rw-rw-   0        0        0     1853 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_3D_surfaceplot.py
+-rw-rw-rw-   0        0        0     1898 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Benzene.py
+-rw-rw-rw-   0        0        0     2350 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Coin.py
+-rw-rw-rw-   0        0        0     2298 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Cone.py
+-rw-rw-rw-   0        0        0     2105 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Cube.py
+-rw-rw-rw-   0        0        0     2033 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Decahedron.py
+-rw-rw-rw-   0        0        0     2046 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_DiscoBall.py
+-rw-rw-rw-   0        0        0     1793 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Globe.py
+-rw-rw-rw-   0        0        0     1886 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Icosahedron.py
+-rw-rw-rw-   0        0        0     2006 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Icosahedron_Outline.py
+-rw-rw-rw-   0        0        0     2348 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/3d/Hello_Octahedron.py
+-rw-rw-rw-   0        0        0     1497 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/3d/Hello_Sphere.py
+-rw-rw-rw-   0        0        0     2330 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/3d/Hello_Tetrahedron.py
+-rw-rw-rw-   0        0        0     3679 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/Hello_APP_Github_ID.py
+-rw-rw-rw-   0        0        0     1210 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/Hello_Darkness.py
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.570497 pythonbmp-1.0.4/samples/colorgradients/
+-rw-rw-rw-   0        0        0     1603 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Circular_Gradient.py
+-rw-rw-rw-   0        0        0     1467 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Dichromic_Circular_Gradient.py
+-rw-rw-rw-   0        0        0     1507 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Dichromic_Circular_Gradient_smoothstep.py
+-rw-rw-rw-   0        0        0     1539 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Elliptical_Gradient.py
+-rw-rw-rw-   0        0        0     1514 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRect.py
+-rw-rw-rw-   0        0        0     1562 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootherstep.py
+-rw-rw-rw-   0        0        0     1565 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmootheststep.py
+-rw-rw-rw-   0        0        0     1556 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromatichoriGradRectsmoothstep.py
+-rw-rw-rw-   0        0        0     1510 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRect.py
+-rw-rw-rw-   0        0        0     1558 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmootherstep.py
+-rw-rw-rw-   0        0        0     1561 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmootheststep.py
+-rw-rw-rw-   0        0        0     1552 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilleddichromaticvertGradRectsmoothstep.py
+-rw-rw-rw-   0        0        0     1480 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRect.py
+-rw-rw-rw-   0        0        0     1531 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRectsmootherstep.py
+-rw-rw-rw-   0        0        0     1534 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRectsmootheststep.py
+-rw-rw-rw-   0        0        0     1525 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledhoriGradRectsmoothstep.py
+-rw-rw-rw-   0        0        0     1476 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRect.py
+-rw-rw-rw-   0        0        0     1527 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRectsmootherstep.py
+-rw-rw-rw-   0        0        0     1530 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRectsmootheststep.py
+-rw-rw-rw-   0        0        0     1521 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_FilledvertGradRectsmoothstep.py
+-rw-rw-rw-   0        0        0     1401 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Linear_Gradient.py
+-rw-rw-rw-   0        0        0     1856 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_NonLinearRadialMultichannel_Gradients.py
+-rw-rw-rw-   0        0        0     1758 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_NonLinearRadial_Gradients.py
+-rw-rw-rw-   0        0        0     1466 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Orb.py
+-rw-rw-rw-   0        0        0     1870 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_RadialMultichannel_Gradients.py
+-rw-rw-rw-   0        0        0     1884 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Radial_Gradients.py
+-rw-rw-rw-   0        0        0     1530 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic.py
+-rw-rw-rw-   0        0        0     1578 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic_smootherstep.py
+-rw-rw-rw-   0        0        0     1581 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic_smootheststep.py
+-rw-rw-rw-   0        0        0     1573 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_dichromic_smoothstep.py
+-rw-rw-rw-   0        0        0     1524 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_smootherstep.py
+-rw-rw-rw-   0        0        0     1527 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_smootheststep.py
+-rw-rw-rw-   0        0        0     1519 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colorgradients/Hello_Sphere_smoothstep.py
+-rw-rw-rw-   0        0        0  1440054 2023-07-25 04:28:42.000000 pythonbmp-1.0.4/samples/colorgradients/HellodistcentercoordplotRGBxybit1.bmp
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.598510 pythonbmp-1.0.4/samples/colornames/
+-rw-rw-rw-   0        0        0     1701 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/colornames/Hello_ColorNames.py
+-rw-rw-rw-   0        0        0     1710 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colornames/Hello_X11ColorNames.py
+-rw-rw-rw-   0        0        0     1754 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/colornames/Hello_XKCDColorNames.py
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.681495 pythonbmp-1.0.4/samples/curves/
+-rw-rw-rw-   0        0        0     1645 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_Cardioid.py
+-rw-rw-rw-   0        0        0     1456 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_CornuSpiral.py
+-rw-rw-rw-   0        0        0     1506 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_EggCurve.py
+-rw-rw-rw-   0        0        0     1760 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_Epicycloid.py
+-rw-rw-rw-   0        0        0     1679 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_Flower.py
+-rw-rw-rw-   0        0        0     1551 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_GearCurve.py
+-rw-rw-rw-   0        0        0     1475 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_HeartCurve.py
+-rw-rw-rw-   0        0        0     1807 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_Hypotrochoid.py
+-rw-rw-rw-   0        0        0     1658 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_InvoluteofaCircle.py
+-rw-rw-rw-   0        0        0     1621 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/curves/Hello_Octopetala.py
+-rw-rw-rw-   0        0        0     1688 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/curves/Hello_SquareSpiral.py
+-rw-rw-rw-   0        0        0     1542 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/curves/Hello_Squircles.py
+-rw-rw-rw-   0        0        0     1672 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/curves/Hello_Superellipse.py
+-rw-rw-rw-   0        0        0     2133 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/curves/Hello_Thick_Exponential_Spiral_Gradient.py
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:50.854116 pythonbmp-1.0.4/samples/fonts/
+-rw-rw-rw-   0        0        0     1760 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_WorId_Italic_RainbowSideway.py
+-rw-rw-rw-   0        0        0     1505 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World.py
+-rw-rw-rw-   0        0        0     1558 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots.py
+-rw-rw-rw-   0        0        0     1580 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_Italicupsidedown.py
+-rw-rw-rw-   0        0        0     1779 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_Rainbow_vertical.py
+-rw-rw-rw-   0        0        0     1775 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italic_rainbowsideway.py
+-rw-rw-rw-   0        0        0     1577 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italicsideway.py
+-rw-rw-rw-   0        0        0     1575 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italicvertical.py
+-rw-rw-rw-   0        0        0     1777 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_italicvertical_rainbow.py
+-rw-rw-rw-   0        0        0     1788 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowItalicupsidedown.py
+-rw-rw-rw-   0        0        0     1792 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowreversedItalic.py
+-rw-rw-rw-   0        0        0     1779 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowsideway.py
+-rw-rw-rw-   0        0        0     1785 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_rainbowupsidedown.py
+-rw-rw-rw-   0        0        0     1569 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_reversed.py
+-rw-rw-rw-   0        0        0     1578 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_reversedItalic.py
+-rw-rw-rw-   0        0        0     1563 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_sideway.py
+-rw-rw-rw-   0        0        0     1572 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_upsidedown.py
+-rw-rw-rw-   0        0        0     1569 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Dots_vertical.py
+-rw-rw-rw-   0        0        0     1414 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Italic.py
+-rw-rw-rw-   0        0        0     1417 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Italicdots.py
+-rw-rw-rw-   0        0        0     1572 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Italicupsidedown.py
+-rw-rw-rw-   0        0        0     1768 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_Dots.py
+-rw-rw-rw-   0        0        0     1584 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_Italic.py
+-rw-rw-rw-   0        0        0     1773 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_Italic_Dots.py
+-rw-rw-rw-   0        0        0     1770 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_Rainbow_vertical.py
+-rw-rw-rw-   0        0        0     1568 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_italicsideway.py
+-rw-rw-rw-   0        0        0     1568 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_italicvertical.py
+-rw-rw-rw-   0        0        0     1774 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_italicvertical_rainbow.py
+-rw-rw-rw-   0        0        0     1771 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowItalicupsidedown.py
+-rw-rw-rw-   0        0        0     1766 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowreversedItalic.py
+-rw-rw-rw-   0        0        0     1770 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowsideway.py
+-rw-rw-rw-   0        0        0     1761 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_rainbowupsidedown.py
+-rw-rw-rw-   0        0        0     1514 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fonts/Hello_World_reversedItalic.py
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:51.222936 pythonbmp-1.0.4/samples/fractals/
+-rw-rw-rw-   0        0        0     1307 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Astroidfractal.py
+-rw-rw-rw-   0        0        0     1466 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_BarnsleyTree.py
+-rw-rw-rw-   0        0        0     1431 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_CatPaws.py
+-rw-rw-rw-   0        0        0     1262 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_CliffordAttractor.py
+-rw-rw-rw-   0        0        0     1474 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_CosJulia_Set.py
+-rw-rw-rw-   0        0        0     1259 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_DuffingAttractor.py
+-rw-rw-rw-   0        0        0     1238 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Fern.py
+-rw-rw-rw-   0        0        0     1287 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_FractalDreamAttractor.py
+-rw-rw-rw-   0        0        0     1267 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Gumowski-Mira_attractor.py
+-rw-rw-rw-   0        0        0     1266 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Gumowski-Mira_attractor_1.py
+-rw-rw-rw-   0        0        0     1161 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_HilbertCurve.py
+-rw-rw-rw-   0        0        0     1260 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_HopalongAttractor.py
+-rw-rw-rw-   0        0        0     1261 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Ikedaattractor.py
+-rw-rw-rw-   0        0        0     1497 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Julia_Set.py
+-rw-rw-rw-   0        0        0     1585 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_KochCurve.py
+-rw-rw-rw-   0        0        0     1627 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_KochSnowflake.py
+-rw-rw-rw-   0        0        0     1379 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Lambdafractal.py
+-rw-rw-rw-   0        0        0     1308 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Lemniscatefractal.py
+-rw-rw-rw-   0        0        0     1732 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_LissajousCurve.py
+-rw-rw-rw-   0        0        0     1354 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Mandelbrot_Set.py
+-rw-rw-rw-   0        0        0     1388 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Mandelbrot_Set_dichromatic.py
+-rw-rw-rw-   0        0        0     1431 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MarekDragon.py
+-rw-rw-rw-   0        0        0     1437 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MarekDragon_4bit.py
+-rw-rw-rw-   0        0        0     1504 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multi2ndtetrationBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1523 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1554 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphphasevariantfractal.py
+-rw-rw-rw-   0        0        0     1498 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphvariantfractal.py
+-rw-rw-rw-   0        0        0     1501 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiBiomorphvariantfractal1.py
+-rw-rw-rw-   0        0        0     1531 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiCosBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1504 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiCoshBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1494 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiSinBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1508 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiSinhBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1502 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiTanBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1531 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiTanBiomorphfractal_dichromatic.py
+-rw-rw-rw-   0        0        0     1504 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiTanhBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1433 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multibrot_Set.py
+-rw-rw-rw-   0        0        0     1426 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multicircle.py
+-rw-rw-rw-   0        0        0     1461 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multicircle_dichromatic.py
+-rw-rw-rw-   0        0        0     1413 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multicorn_Set.py
+-rw-rw-rw-   0        0        0     1494 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultiexpBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1414 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multihyperbola.py
+-rw-rw-rw-   0        0        0     1497 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multijulia_Set.py
+-rw-rw-rw-   0        0        0     1315 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Multisuperellipse.py
+-rw-rw-rw-   0        0        0     1501 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_MultizconjugateBiomorphfractal.py
+-rw-rw-rw-   0        0        0     1528 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal.py
+-rw-rw-rw-   0        0        0     1551 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal4.py
+-rw-rw-rw-   0        0        0     1552 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal4_1.py
+-rw-rw-rw-   0        0        0     1575 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal5.py
+-rw-rw-rw-   0        0        0     1577 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal5_1.py
+-rw-rw-rw-   0        0        0     1578 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal5_3.py
+-rw-rw-rw-   0        0        0     1627 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal6.py
+-rw-rw-rw-   0        0        0     1629 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_Newtons_fractal6_3.py
+-rw-rw-rw-   0        0        0     1272 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_PeterdeJongAttractor.py
+-rw-rw-rw-   0        0        0     1474 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_SinJulia_Set.py
+-rw-rw-rw-   0        0        0     1472 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_SinJulia_Set_1bit.py
+-rw-rw-rw-   0        0        0     1487 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_SinJulia_Set_4bit.py
+-rw-rw-rw-   0        0        0     1489 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_SpiralJulia_Set.py
+-rw-rw-rw-   0        0        0     1314 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_Symmetric_Icon_Attractor.py
+-rw-rw-rw-   0        0        0     1294 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_Tetration_Fractal.py
+-rw-rw-rw-   0        0        0     1783 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_ThickGradHilbertCurve.py
+-rw-rw-rw-   0        0        0     1279 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_ThickHilbertCurve.py
+-rw-rw-rw-   0        0        0     1401 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_Tricorn_Set.py
+-rw-rw-rw-   0        0        0     1416 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_Xordivfractal.py
+-rw-rw-rw-   0        0        0     1329 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/fractals/Hello_Xorfractal.py
+-rw-rw-rw-   0        0        0     1262 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_nattractor.py
+-rw-rw-rw-   0        0        0     1472 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/fractals/Hello_ngonfractal.py
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:51.228931 pythonbmp-1.0.4/samples/graphs/
+-rw-rw-rw-   0        0        0     2230 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/graphs/Hello_XYScatterplot.py
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:51.336931 pythonbmp-1.0.4/samples/primitives2d/
+-rw-rw-rw-   0        0        0     1711 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_BezierCurve.py
+-rw-rw-rw-   0        0        0     1943 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Bspline.py
+-rw-rw-rw-   0        0        0     1544 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Circles.py
+-rw-rw-rw-   0        0        0     1415 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Ellipse.py
+-rw-rw-rw-   0        0        0     1713 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_FilledCircle.py
+-rw-rw-rw-   0        0        0     1677 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_FilledEllipse.py
+-rw-rw-rw-   0        0        0     1679 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_FilledRectangle.py
+-rw-rw-rw-   0        0        0     1868 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Gradient_Thick_Regular_Polygon.py
+-rw-rw-rw-   0        0        0     1485 2023-07-21 14:08:49.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Lines.py
+-rw-rw-rw-   0        0        0     1550 2023-07-21 14:08:45.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Rectangle.py
+-rw-rw-rw-   0        0        0     1672 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Regular_Polygon.py
+-rw-rw-rw-   0        0        0     1699 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Circle.py
+-rw-rw-rw-   0        0        0     1709 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Gradient_Circle.py
+-rw-rw-rw-   0        0        0     1721 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Gradient_Ellipse_Rotated.py
+-rw-rw-rw-   0        0        0     1479 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Regular_Polygon.py
+-rw-rw-rw-   0        0        0     1665 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Round_Gradient_Line.py
+-rw-rw-rw-   0        0        0     1772 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Thick_Round_Line.py
+-rw-rw-rw-   0        0        0     1461 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/primitives2d/Hello_Vector.py
+drwxrwxrwx   0        0        0        0 2023-07-25 04:49:51.356930 pythonbmp-1.0.4/samples/spirographs/
+-rw-rw-rw-   0        0        0     1759 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph.py
+-rw-rw-rw-   0        0        0     1856 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph_1.py
+-rw-rw-rw-   0        0        0     1772 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph_2.py
+-rw-rw-rw-   0        0        0     1639 2023-07-21 14:08:42.000000 pythonbmp-1.0.4/samples/spirographs/Hello_Spirograph_Record.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 04:49:51.365930 pythonbmp-1.0.4/setup.cfg
```

### Comparing `pythonbmp-1.0.3/LICENSE` & `pythonbmp-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/PKG-INFO` & `pythonbmp-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonbmp
-Version: 1.0.3
+Version: 1.0.4
 Summary: A pure Python 2D/3D graphics library that outputs to windows bitmap format
 Author-email: Joel Alcarez <joelalcarez1975@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 TechnoTanuki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Project-URL: Bug Tracker, https://github.com/TechnoTanuki/Python_BMP/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![AppID](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/Hello_GithubID.png)](https://github.com/TechnoTanuki/Python_BMP/blob/main/Hello_APP_Github_ID.py)
+[![AppID](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/Hello_GithubID.png)](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Hello_APP_Github_ID.py)
 ___________
 # pythonbmp
 ___________
 A pure Python 2D/3D graphics library that outputs to windows bitmap format
 * Developed and tested using Python 3.8 / 3.10.4 / 3.11
 * No dependencies required
 
@@ -47,15 +47,15 @@
 
 # Instructions
 
 Run Hello_somestring_here.py
 
 This will show minimum code to accomplish certain tasks
 
-* ![Hello_Darkness.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/Hello_Darkness.py) (my old friend) is a minimum template
+* ![Hello_Darkness.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Hello_Darkness.py) (my old friend) is a minimum template
 
 Run ![Features_Speedtest.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/Features_Speedtest.py)
 
 * It should generate a bitmap and open MS Paint under windows to show output...
 * Close the MS Paint window to execute another script
 
 # Unit tests (images are links to test)
@@ -64,18 +64,14 @@
 
 [![Fractals](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/fractals/multijulia.bmp)](https://github.com/TechnoTanuki/Python_BMP/blob/main/test_fractals.py)
 
 [![Text](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/fonts/8x8x4px1cs024bitplotitalicstring2filebc0cmulti.bmp)](https://github.com/TechnoTanuki/Python_BMP/blob/main/test_fonts.py)
 
 * Will generate images (one per function under test) then compare it with previously generated images generated with the function under test (this might take a while)
 
-# VS Code Users
-
-See: https://k0nze.dev/posts/python-relative-imports-vscode/
-* (Module Relative imports dont work in VS Code but code as-is runs fine in terminal or IDLE)
 
 # Moar docs
 
 * ![Hello Graphics](https://github.com/TechnoTanuki/Python_BMP/blob/main/docs/Hello_Graphics.md)
 
 * ![Hello Text](https://github.com/TechnoTanuki/Python_BMP/blob/main/docs/Hello_Text.md)
```

### Comparing `pythonbmp-1.0.3/README.md` & `pythonbmp-1.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![AppID](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/Hello_GithubID.png)](https://github.com/TechnoTanuki/Python_BMP/blob/main/Hello_APP_Github_ID.py)
+[![AppID](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/Hello_GithubID.png)](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Hello_APP_Github_ID.py)
 ___________
 # pythonbmp
 ___________
 A pure Python 2D/3D graphics library that outputs to windows bitmap format
 * Developed and tested using Python 3.8 / 3.10.4 / 3.11
 * No dependencies required
 
@@ -10,15 +10,15 @@
 
 # Instructions
 
 Run Hello_somestring_here.py
 
 This will show minimum code to accomplish certain tasks
 
-* ![Hello_Darkness.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/Hello_Darkness.py) (my old friend) is a minimum template
+* ![Hello_Darkness.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Hello_Darkness.py) (my old friend) is a minimum template
 
 Run ![Features_Speedtest.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/Features_Speedtest.py)
 
 * It should generate a bitmap and open MS Paint under windows to show output...
 * Close the MS Paint window to execute another script
 
 # Unit tests (images are links to test)
@@ -27,18 +27,14 @@
 
 [![Fractals](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/fractals/multijulia.bmp)](https://github.com/TechnoTanuki/Python_BMP/blob/main/test_fractals.py)
 
 [![Text](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/fonts/8x8x4px1cs024bitplotitalicstring2filebc0cmulti.bmp)](https://github.com/TechnoTanuki/Python_BMP/blob/main/test_fonts.py)
 
 * Will generate images (one per function under test) then compare it with previously generated images generated with the function under test (this might take a while)
 
-# VS Code Users
-
-See: https://k0nze.dev/posts/python-relative-imports-vscode/
-* (Module Relative imports dont work in VS Code but code as-is runs fine in terminal or IDLE)
 
 # Moar docs
 
 * ![Hello Graphics](https://github.com/TechnoTanuki/Python_BMP/blob/main/docs/Hello_Graphics.md)
 
 * ![Hello Text](https://github.com/TechnoTanuki/Python_BMP/blob/main/docs/Hello_Text.md)
```

### Comparing `pythonbmp-1.0.3/pyproject.toml` & `pythonbmp-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pythonbmp"
 description = "A pure Python 2D/3D graphics library that outputs to windows bitmap format"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     { name = "Joel Alcarez", email = "joelalcarez1975@gmail.com" }
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
```

### Comparing `pythonbmp-1.0.3/pythonbmp/BITMAPlib.py` & `pythonbmp-1.0.4/pythonbmp/BITMAPlib.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/X11colordict.py` & `pythonbmp-1.0.4/pythonbmp/X11colordict.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/XKCDcolordict.py` & `pythonbmp-1.0.4/pythonbmp/XKCDcolordict.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/bmpconstants.py` & `pythonbmp-1.0.4/pythonbmp/bmpconstants.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/bmppal.py` & `pythonbmp-1.0.4/pythonbmp/bmppal.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/bufferflip.py` & `pythonbmp-1.0.4/pythonbmp/bufferflip.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/buffersplit.py` & `pythonbmp-1.0.4/pythonbmp/buffersplit.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/bufresize.py` & `pythonbmp-1.0.4/pythonbmp/bufresize.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/chartools.py` & `pythonbmp-1.0.4/pythonbmp/chartools.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/charts.py` & `pythonbmp-1.0.4/pythonbmp/charts.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/colordict.py` & `pythonbmp-1.0.4/pythonbmp/colordict.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/colors.py` & `pythonbmp-1.0.4/pythonbmp/colors.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/conditionaltools.py` & `pythonbmp-1.0.4/pythonbmp/conditionaltools.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/dicttools.py` & `pythonbmp-1.0.4/pythonbmp/dicttools.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/fileutils.py` & `pythonbmp-1.0.4/pythonbmp/fileutils.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/fonts.py` & `pythonbmp-1.0.4/pythonbmp/fonts.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/fractals.py` & `pythonbmp-1.0.4/pythonbmp/fractals.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/inttools.py` & `pythonbmp-1.0.4/pythonbmp/inttools.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/mathlib.py` & `pythonbmp-1.0.4/pythonbmp/mathlib.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/messages.py` & `pythonbmp-1.0.4/pythonbmp/messages.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/paramchecks.py` & `pythonbmp-1.0.4/pythonbmp/paramchecks.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/primitives2D.py` & `pythonbmp-1.0.4/pythonbmp/primitives2D.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/proctimer.py` & `pythonbmp-1.0.4/pythonbmp/proctimer.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/shims.py` & `pythonbmp-1.0.4/pythonbmp/shims.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/solids3D.py` & `pythonbmp-1.0.4/pythonbmp/solids3D.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp/textgraphics.py` & `pythonbmp-1.0.4/pythonbmp/textgraphics.py`

 * *Files identical despite different names*

### Comparing `pythonbmp-1.0.3/pythonbmp.egg-info/PKG-INFO` & `pythonbmp-1.0.4/pythonbmp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonbmp
-Version: 1.0.3
+Version: 1.0.4
 Summary: A pure Python 2D/3D graphics library that outputs to windows bitmap format
 Author-email: Joel Alcarez <joelalcarez1975@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 TechnoTanuki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Project-URL: Bug Tracker, https://github.com/TechnoTanuki/Python_BMP/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![AppID](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/Hello_GithubID.png)](https://github.com/TechnoTanuki/Python_BMP/blob/main/Hello_APP_Github_ID.py)
+[![AppID](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/Hello_GithubID.png)](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Hello_APP_Github_ID.py)
 ___________
 # pythonbmp
 ___________
 A pure Python 2D/3D graphics library that outputs to windows bitmap format
 * Developed and tested using Python 3.8 / 3.10.4 / 3.11
 * No dependencies required
 
@@ -47,15 +47,15 @@
 
 # Instructions
 
 Run Hello_somestring_here.py
 
 This will show minimum code to accomplish certain tasks
 
-* ![Hello_Darkness.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/Hello_Darkness.py) (my old friend) is a minimum template
+* ![Hello_Darkness.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/samples/Hello_Darkness.py) (my old friend) is a minimum template
 
 Run ![Features_Speedtest.py](https://github.com/TechnoTanuki/Python_BMP/blob/main/Features_Speedtest.py)
 
 * It should generate a bitmap and open MS Paint under windows to show output...
 * Close the MS Paint window to execute another script
 
 # Unit tests (images are links to test)
@@ -64,18 +64,14 @@
 
 [![Fractals](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/fractals/multijulia.bmp)](https://github.com/TechnoTanuki/Python_BMP/blob/main/test_fractals.py)
 
 [![Text](https://github.com/TechnoTanuki/Python_BMP/blob/main/assets/fonts/8x8x4px1cs024bitplotitalicstring2filebc0cmulti.bmp)](https://github.com/TechnoTanuki/Python_BMP/blob/main/test_fonts.py)
 
 * Will generate images (one per function under test) then compare it with previously generated images generated with the function under test (this might take a while)
 
-# VS Code Users
-
-See: https://k0nze.dev/posts/python-relative-imports-vscode/
-* (Module Relative imports dont work in VS Code but code as-is runs fine in terminal or IDLE)
 
 # Moar docs
 
 * ![Hello Graphics](https://github.com/TechnoTanuki/Python_BMP/blob/main/docs/Hello_Graphics.md)
 
 * ![Hello Text](https://github.com/TechnoTanuki/Python_BMP/blob/main/docs/Hello_Text.md)
```

