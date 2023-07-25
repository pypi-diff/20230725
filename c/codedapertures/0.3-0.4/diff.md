# Comparing `tmp/codedapertures-0.3.tar.gz` & `tmp/codedapertures-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedapertures-0.3.tar", last modified: Fri Jul 21 01:51:54 2023, max compression
+gzip compressed data, was "codedapertures-0.4.tar", last modified: Tue Jul 25 00:59:06 2023, max compression
```

## Comparing `codedapertures-0.3.tar` & `codedapertures-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-21 01:51:54.842318 codedapertures-0.3/
--rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.3/LICENSE
--rw-r--r--   0 bbudden    (501) staff       (20)      697 2023-07-21 01:51:54.842213 codedapertures-0.3/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)     1530 2023-07-20 04:15:05.000000 codedapertures-0.3/README.md
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-21 01:51:54.841362 codedapertures-0.3/codedapertures/
--rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.3/codedapertures/__init__.py
--rw-r--r--   0 bbudden    (501) staff       (20)    13570 2023-07-21 01:46:46.000000 codedapertures-0.3/codedapertures/codedapertures.py
-drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-21 01:51:54.842062 codedapertures-0.3/codedapertures.egg-info/
--rw-r--r--   0 bbudden    (501) staff       (20)      697 2023-07-21 01:51:54.000000 codedapertures-0.3/codedapertures.egg-info/PKG-INFO
--rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-21 01:51:54.000000 codedapertures-0.3/codedapertures.egg-info/SOURCES.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-21 01:51:54.000000 codedapertures-0.3/codedapertures.egg-info/dependency_links.txt
--rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.3/codedapertures.egg-info/not-zip-safe
--rw-r--r--   0 bbudden    (501) staff       (20)       26 2023-07-21 01:51:54.000000 codedapertures-0.3/codedapertures.egg-info/requires.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-21 01:51:54.000000 codedapertures-0.3/codedapertures.egg-info/top_level.txt
--rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-21 01:51:54.842347 codedapertures-0.3/setup.cfg
--rw-r--r--   0 bbudden    (501) staff       (20)      868 2023-07-21 01:51:45.000000 codedapertures-0.3/setup.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-25 00:59:06.202970 codedapertures-0.4/
+-rw-r--r--   0 bbudden    (501) staff       (20)     1062 2023-01-26 02:12:38.000000 codedapertures-0.4/LICENSE
+-rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-25 00:59:06.202849 codedapertures-0.4/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)     1743 2023-07-25 00:21:35.000000 codedapertures-0.4/README.md
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-25 00:59:06.201928 codedapertures-0.4/codedapertures/
+-rw-r--r--   0 bbudden    (501) staff       (20)       30 2023-01-26 02:12:38.000000 codedapertures-0.4/codedapertures/__init__.py
+-rw-r--r--   0 bbudden    (501) staff       (20)    16567 2023-07-25 00:54:26.000000 codedapertures-0.4/codedapertures/codedapertures.py
+drwxr-xr-x   0 bbudden    (501) staff       (20)        0 2023-07-25 00:59:06.202687 codedapertures-0.4/codedapertures.egg-info/
+-rw-r--r--   0 bbudden    (501) staff       (20)      720 2023-07-25 00:59:06.000000 codedapertures-0.4/codedapertures.egg-info/PKG-INFO
+-rw-r--r--   0 bbudden    (501) staff       (20)      312 2023-07-25 00:59:06.000000 codedapertures-0.4/codedapertures.egg-info/SOURCES.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-25 00:59:06.000000 codedapertures-0.4/codedapertures.egg-info/dependency_links.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)        1 2023-07-06 00:30:22.000000 codedapertures-0.4/codedapertures.egg-info/not-zip-safe
+-rw-r--r--   0 bbudden    (501) staff       (20)       26 2023-07-25 00:59:06.000000 codedapertures-0.4/codedapertures.egg-info/requires.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       15 2023-07-25 00:59:06.000000 codedapertures-0.4/codedapertures.egg-info/top_level.txt
+-rw-r--r--   0 bbudden    (501) staff       (20)       38 2023-07-25 00:59:06.203002 codedapertures-0.4/setup.cfg
+-rw-r--r--   0 bbudden    (501) staff       (20)      891 2023-07-25 00:57:02.000000 codedapertures-0.4/setup.py
```

### Comparing `codedapertures-0.3/LICENSE` & `codedapertures-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `codedapertures-0.3/PKG-INFO` & `codedapertures-0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.3
-Summary: Coded Aperture Production in PYthon (CAPPY)
-Home-page: https://github.com/bpops/cappy
+Version: 0.4
+Summary: a python package for generating coded apertures
+Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
-CAPPY is a python module that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
+CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.3/README.md` & `codedapertures-0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-# CAPPY
-### Coded Aperture Production in PYthon
+# CodedApertures
+#### a python package for generating coded apertures  
 
 [![Downloads](https://static.pepy.tech/personalized-badge/codedapertures?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/codedapertures)
 
-CAPPY is a python module that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
+CodedApertures is a python module that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
 
 New to coded apertures? Here's a nice article: https://www.paulcarlisle.net/codedaperture/
 
 PyPI URL: https://pypi.org/project/codedapertures/
 
 ### Usage
 
 Install with PIP:
 ```
 pip install codedapertures
 ```
 
-See [demo.ipynb](https://github.com/bpops/cappy/blob/master/demo.ipynb) for examples of use.
-
+See [demo.ipynb](https://github.com/bpops/codedapertures/blob/master/demo.ipynb) for examples of use.
 
 ### Credits
 
 URA pattern: E. E. Fenimore and T. M. Cannon, "Coded aperture imaging with uniformly redundant arrays," Appl. Opt. 17, 337-347 (1978).
 
 MURA pattern:  E.E. Fenimore and S. R. Gottesman, "New family of binary arrays for coded aperture imaging" Appl. Opt. 28 (20): 4344-4352 (1989).
 
 SHURA and HURA pattern: M.H. Finger and T.A. Prince, "Hexagonal Uniformly Redundant Arrays for Coded-Aperture Imaging," Proc. 19th Int. Cosmic Ray Conf., 3: 295-298 (1985).
+
+This package will use an axial coordinate system for the hexagonal grids. It will follow the concept outlined at https://www.redblobgames.com/grids/hexagons/#map-storage.
```

### Comparing `codedapertures-0.3/codedapertures/codedapertures.py` & `codedapertures-0.4/codedapertures/codedapertures.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-#                                                                                 
-#            _|_|_|    _|_|    _|_|_|    _|_|_|    _|      _|                
-#          _|        _|    _|  _|    _|  _|    _|    _|  _|                  
-#          _|        _|_|_|_|  _|_|_|    _|_|_|        _|                    
-#          _|        _|    _|  _|        _|            _|                    
-#            _|_|_|  _|    _|  _|        _|            _|                    
-#                                                                                 
-#                Coded Aperture Production in PYthon                                                                              
 #
-#                           MIT license
-#                  https://github.com/bpops/cappy
+#       _____       _       _ _____             _                            
+#      |     |___ _| |___ _| |  _  |___ ___ ___| |_ _ _ ___ ___ ___          
+#      |   --| . | . | -_| . |     | . | -_|  _|  _| | |  _| -_|_ -|         
+#      |_____|___|___|___|___|__|__|  _|___|_| |_| |___|_| |___|___|         
+#                                  |_|                                       
+#
+#            a python package for generating coded apertures                                                                        
+#
+#                             MIT license
+#                    https://github.com/bpops/cappy
 #
 
+#import copy
 import numpy              as     np
 import matplotlib.pyplot  as     plt
 from   matplotlib.patches import RegularPolygon
 import pyprimes
 import random
 
 
@@ -454,24 +455,24 @@
         ax.set_aspect('equal')
 
         # closed pixels
         for x, y in zip (x_closed, y_closed):
 
             # determine patch origin
             x += y * 0.5
-            y *= np.sqrt(3)/2
+            y *= 1/hex_vert
 
             # recenter
             x -= (self.mask.shape[0] + self.mask.shape[1]/2.0)/2.0
             y -= (self.mask.shape[1] * 1/hex_vert)/2.0
 
             # add hexagon
             hex = RegularPolygon((x, y), numVertices=6, radius=hex_radius, 
                                     orientation=np.radians(60), 
-                                    facecolor='k', alpha=0.5, edgecolor='k')
+                                    facecolor='k', alpha=0.6, edgecolor='k')
             ax.add_patch(hex)
 
         # open pixels
         for x, y in zip (x_opened, y_opened):
 
             # determine patch origin
             x += y * 0.5
@@ -486,7 +487,93 @@
                                     orientation=np.radians(60), 
                                     facecolor='w', alpha=0.2, edgecolor='k')
             ax.add_patch(hex)
 
         plt.xlim(-self.mask.shape[0]/3.0,self.mask.shape[0]/3.0)
         plt.ylim(-self.mask.shape[0]/3.0,self.mask.shape[1]/3.0)
         plt.title(f"SHURA [o:{self.v}, r:{self.r}, x:{self.mult}]")
+
+
+class rand_hex():
+    """
+    Random Hexagonal Array
+
+    Parameters
+    ----------
+    radius: int
+        vertex-to-vertex radius of the array, minus half the pixel width
+    fill: float
+        fraction fill
+    quiet : bool
+        if True, will print information about the array upon creation
+    """
+    def __init__(self, radius=3, fill=0.5, quiet=False):
+
+        # get/determine mask properties
+        self.radius       = radius
+        self.diam         = self.radius*2+1
+        self.side_width   = radius + 1
+        self.axial_matrix = np.zeros((self.diam,self.diam))
+        self.loc_matrix   = np.zeros((2,self.diam,self.diam))
+        self.fill         = fill
+
+        # generate mask pattern
+        for i in range(self.diam):
+            for j in range(self.diam):
+                if (i+j > (self.radius-1)) and (i+j < (self.diam+self.radius)):
+                    if random.random() < self.fill:
+                        self.axial_matrix[i,j] = 1
+                else:
+                    self.axial_matrix[i,j] = np.nan
+
+        # determine actual fill factor
+        self.actual_fill = np.sum(self.axial_matrix == 1) / np.sum(~np.isnan(self.axial_matrix))
+
+        # generate locations
+        for i in range(self.diam):
+            for j in range(self.diam):
+                if not np.isnan(self.axial_matrix[i,j]):
+                    self.loc_matrix[0,i,j] = i*np.sqrt(3) - abs(j-self.radius)/2.0
+                    self.loc_matrix[1,i,j] = -i + j
+
+        if not quiet: self.report()
+
+    def report(self):
+        """
+        Report the array info
+        """
+        print("Random Hexagonal Array")
+        print(f"radius: {self.radius}")
+        print(f"diameter: {self.diam}")
+        print(f"side_width: {self.side_width}")
+        print(f"desired fill factor: {self.fill:.2f}")
+        print(f"actual  fill factor: {self.actual_fill:.2f}")
+
+    def show(self):
+        """
+        Plot the mask
+        """
+
+        # set up plot parameters
+        fig, ax = plt.subplots(1)
+        ax.set_aspect('equal')
+        hex_width = 1.0 # face-to-face distance
+        hex_vert  = (hex_width)*(2.0/np.sqrt(3))
+
+        # draw hexagon array
+        for y in range(self.diam):
+            row_width = self.diam - abs(self.radius-y)
+            start_i   = np.max((self.radius-y,0))
+            for x in range(row_width):
+                facecolor = 'k' if self.axial_matrix[x+start_i,y] == 1 else 'w'
+                alpha     = 0.6 if self.axial_matrix[x+start_i,y] == 1 else 0.3
+                hex = RegularPolygon((x+0.5*abs(y-self.radius)-self.radius,
+                                      ((y-self.radius)*((3/2)*hex_vert/2.0))),
+                                     numVertices=6, radius=hex_vert/2.0, 
+                                     orientation=np.radians(60), 
+                                     facecolor=facecolor, alpha=alpha, edgecolor='k')
+                ax.add_patch(hex)
+
+        # set axis limits
+        plt.xlim(-self.radius*hex_vert,self.radius*hex_vert)
+        plt.ylim(-self.radius,self.radius)
+        plt.title(f"Random Hex Array [diam: {self.diam}, fill: {self.actual_fill:.2f}]")
```

### Comparing `codedapertures-0.3/codedapertures.egg-info/PKG-INFO` & `codedapertures-0.4/codedapertures.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedapertures
-Version: 0.3
-Summary: Coded Aperture Production in PYthon (CAPPY)
-Home-page: https://github.com/bpops/cappy
+Version: 0.4
+Summary: a python package for generating coded apertures
+Home-page: https://github.com/bpops/codedapertures
 Author: bpops
 License: MIT
 License-File: LICENSE
 
-CAPPY is a python module that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
+CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.
```

### Comparing `codedapertures-0.3/setup.py` & `codedapertures-0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(name='codedapertures',
-      version='0.3',
-      description='Coded Aperture Production in PYthon (CAPPY)',
-      long_description='CAPPY is a python module that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.',
-      url='https://github.com/bpops/cappy',
+      version='0.4',
+      description='a python package for generating coded apertures',
+      long_description='CodedApertures is a python package that allows one to easily generate and display common coded aperture patterns. Coded apertures are a spatial encoding technique for straight-line optics, wherein traditional lensing (e.g., visible light) is not possible. Even wherein tradiational lensing is possible, there may be other advantages (infinite depth of field). Coded apertures may therefore be used for hard x-ray and gamma-ray imaging for astrophysics, medical imaging, and homeland security applications.',
+      url='https://github.com/bpops/codedapertures',
       author='bpops',
       license='MIT',
       install_requires=['pyprimes',
                 'numpy',
                 'matplotlib'],
       zip_safe=False)
```

