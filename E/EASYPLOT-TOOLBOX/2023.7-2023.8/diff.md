# Comparing `tmp/EASYPLOT_TOOLBOX-2023.7.tar.gz` & `tmp/EASYPLOT_TOOLBOX-2023.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EASYPLOT_TOOLBOX-2023.7.tar", last modified: Tue Jul 25 14:26:32 2023, max compression
+gzip compressed data, was "EASYPLOT_TOOLBOX-2023.8.tar", last modified: Tue Jul 25 18:45:46 2023, max compression
```

## Comparing `EASYPLOT_TOOLBOX-2023.7.tar` & `EASYPLOT_TOOLBOX-2023.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:26:32.456637 EASYPLOT_TOOLBOX-2023.7/
-drwxrwxrwx   0        0        0        0 2023-07-25 14:26:32.433630 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX/
--rw-rw-rw-   0        0        0    13687 2023-07-25 14:25:53.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX/EASYPLOT.py
--rw-rw-rw-   0        0        0       23 2023-03-09 15:47:42.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:26:32.454635 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/
--rw-rw-rw-   0        0        0      618 2023-07-25 14:26:32.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-25 14:26:32.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:26:32.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-25 14:26:32.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-25 14:26:32.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      618 2023-07-25 14:26:32.455635 EASYPLOT_TOOLBOX-2023.7/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2023-07-25 14:25:53.000000 EASYPLOT_TOOLBOX-2023.7/license.md
--rw-rw-rw-   0        0        0       42 2023-07-25 14:26:32.456637 EASYPLOT_TOOLBOX-2023.7/setup.cfg
--rw-rw-rw-   0        0        0     1467 2023-07-25 14:26:29.000000 EASYPLOT_TOOLBOX-2023.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:45:46.273626 EASYPLOT_TOOLBOX-2023.8/
+drwxrwxrwx   0        0        0        0 2023-07-25 18:45:46.251621 EASYPLOT_TOOLBOX-2023.8/EASYPLOT_TOOLBOX/
+-rw-rw-rw-   0        0        0    13846 2023-07-25 18:14:10.000000 EASYPLOT_TOOLBOX-2023.8/EASYPLOT_TOOLBOX/EASYPLOT.py
+-rw-rw-rw-   0        0        0       23 2023-03-09 15:47:42.000000 EASYPLOT_TOOLBOX-2023.8/EASYPLOT_TOOLBOX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:45:46.272627 EASYPLOT_TOOLBOX-2023.8/EASYPLOT_TOOLBOX.egg-info/
+-rw-rw-rw-   0        0        0      618 2023-07-25 18:45:46.000000 EASYPLOT_TOOLBOX-2023.8/EASYPLOT_TOOLBOX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-25 18:45:46.000000 EASYPLOT_TOOLBOX-2023.8/EASYPLOT_TOOLBOX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:45:46.000000 EASYPLOT_TOOLBOX-2023.8/EASYPLOT_TOOLBOX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-25 18:45:46.000000 EASYPLOT_TOOLBOX-2023.8/EASYPLOT_TOOLBOX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-25 18:45:46.000000 EASYPLOT_TOOLBOX-2023.8/EASYPLOT_TOOLBOX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      618 2023-07-25 18:45:46.273626 EASYPLOT_TOOLBOX-2023.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2023-07-25 14:25:53.000000 EASYPLOT_TOOLBOX-2023.8/license.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 18:45:46.274626 EASYPLOT_TOOLBOX-2023.8/setup.cfg
+-rw-rw-rw-   0        0        0     1467 2023-07-25 18:45:30.000000 EASYPLOT_TOOLBOX-2023.8/setup.py
```

### Comparing `EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX/EASYPLOT.py` & `EASYPLOT_TOOLBOX-2023.8/EASYPLOT_TOOLBOX/EASYPLOT.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,42 +222,50 @@
     X_AXIS_LABEL = PLOT_SETUP['X AXIS LABEL']
     X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
     Y_AXIS_SIZE = PLOT_SETUP['Y AXIS SIZE']
     AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
     LABELS_SIZE = PLOT_SETUP['LABELS SIZE']
     LABELS_COLOR = PLOT_SETUP['LABELS COLOR']
     COLORS = PLOT_SETUP['COLORS']
-    GRID = PLOT_SETUP['ON GRID?']    
+    GRID = PLOT_SETUP['ON GRID?']  
+    YLOGSCALE = PLOT_SETUP['Y LOG']
     EXT = PLOT_SETUP['EXTENSION']
     DPI = PLOT_SETUP['DPI']
     
     # Data
     X = DATASET['X']
     Y = DATASET['Y']
     LEGEND = DATASET['LEGEND']
    
     # Plot
     [W, H] = CONVERT_SI_TO_INCHES(W, H)
     FIG, AX = plt.subplots(1, 1, figsize = (W, H))
-    #error_config = {'ecolor': '0.3'}
+    
     # Create the bar chart for each category
+    POS1 = range(len(X))
+    
     for I, CATEGORY in enumerate(LEGEND):
-        X_VALUES = [CAT + I * BAR_WIDTH for CAT in X]
-        AX.bar(X_VALUES, Y[I], BAR_WIDTH, alpha = OPACITY, color = COLORS[I], label = CATEGORY) #, error_kw = error_config)
+        if I == 0 and I <= len(X) - 1: 
+            POS = POS1
+        else:
+            POS = [aux + BAR_WIDTH * I for aux in POS1]
+        AX.bar(POS, Y[I], width = BAR_WIDTH, alpha = OPACITY, color = COLORS[I],  align = 'center', label = CATEGORY) #, error_kw = error_config)
     FONT = {'fontname': 'DejaVu Sans',
             'color':  LABELS_COLOR,
             'weight': 'normal',
             'size': LABELS_SIZE}
     AX.set_ylabel(Y_AXIS_LABEL, fontdict = FONT)
     AX.set_xlabel(X_AXIS_LABEL, fontdict = FONT)
     AX.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR)
     AX.tick_params(axis = 'y', labelsize = Y_AXIS_SIZE, colors = AXISES_COLOR)
-    AX.set_xticks([CAT + (len(LEGEND) - 1) * BAR_WIDTH / 2 for CAT in X])
+    AX.set_xticks([AUX + BAR_WIDTH for AUX in POS1])
     AX.set_xticklabels(X)
     AX.legend()
+    if YLOGSCALE:
+        AX.semilogy()
 
     if GRID == True:
         AX.grid(color = 'grey', linestyle = '-', linewidth = 1, alpha = 0.20, axis = 'y')
     plt.tight_layout()
     SAVE_GRAPHIC(NAME, EXT, DPI)
 
 def PIZZA_CHART(**kwargs):
```

### Comparing `EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/PKG-INFO` & `EASYPLOT_TOOLBOX-2023.8/EASYPLOT_TOOLBOX.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EASYPLOT-TOOLBOX
-Version: 2023.7
+Version: 2023.8
 Summary: The Easyplotpy toolboox is an algorithm that aims to facilitate the plotting of charts for use in articles and lectures.
 Home-page: https://wmpjrufg.github.io/EASYPLOTPY/
 Author-email: wanderlei_junior@ufcat.edu.br
 License: MIT License
 Keywords: Plot,Learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Education
```

### Comparing `EASYPLOT_TOOLBOX-2023.7/PKG-INFO` & `EASYPLOT_TOOLBOX-2023.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EASYPLOT_TOOLBOX
-Version: 2023.7
+Version: 2023.8
 Summary: The Easyplotpy toolboox is an algorithm that aims to facilitate the plotting of charts for use in articles and lectures.
 Home-page: https://wmpjrufg.github.io/EASYPLOTPY/
 Author-email: wanderlei_junior@ufcat.edu.br
 License: MIT License
 Keywords: Plot,Learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Education
```

### Comparing `EASYPLOT_TOOLBOX-2023.7/license.md` & `EASYPLOT_TOOLBOX-2023.8/license.md`

 * *Files identical despite different names*

### Comparing `EASYPLOT_TOOLBOX-2023.7/setup.py` & `EASYPLOT_TOOLBOX-2023.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # from pathlib import Path
 # this_directory = Path(__file__).resolve().parent
 # readme_path = this_directory / "readme.md"
 # long_description = readme_path.read_text(encoding = 'utf-8')
 
 setup(
     	name = 'EASYPLOT_TOOLBOX',
-    	version = '2023.7',
+    	version = '2023.8',
 		url = 'https://wmpjrufg.github.io/EASYPLOTPY/',
     	description = 'The Easyplotpy toolboox is an algorithm that aims to facilitate the plotting of charts for use in articles and lectures.',
 		# long_description = long_description,
 		# long_description_content_type='text/markdown',        
 		keywords = ["Plot", "Learning"],
 		license = 'MIT License',
         readme = 'readme.md',
```

