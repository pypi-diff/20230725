# Comparing `tmp/EASYPLOT_TOOLBOX-2023.6.tar.gz` & `tmp/EASYPLOT_TOOLBOX-2023.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EASYPLOT_TOOLBOX-2023.6.tar", last modified: Sun Jul 16 00:00:51 2023, max compression
+gzip compressed data, was "EASYPLOT_TOOLBOX-2023.7.tar", last modified: Tue Jul 25 14:26:32 2023, max compression
```

## Comparing `EASYPLOT_TOOLBOX-2023.6.tar` & `EASYPLOT_TOOLBOX-2023.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 00:00:51.775308 EASYPLOT_TOOLBOX-2023.6/
-drwxrwxrwx   0        0        0        0 2023-07-16 00:00:51.741302 EASYPLOT_TOOLBOX-2023.6/EASYPLOT_TOOLBOX/
--rw-rw-rw-   0        0        0    13229 2023-07-15 23:26:17.000000 EASYPLOT_TOOLBOX-2023.6/EASYPLOT_TOOLBOX/EASYPLOT.py
--rw-rw-rw-   0        0        0       23 2023-02-18 15:01:30.000000 EASYPLOT_TOOLBOX-2023.6/EASYPLOT_TOOLBOX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 00:00:51.771303 EASYPLOT_TOOLBOX-2023.6/EASYPLOT_TOOLBOX.egg-info/
--rw-rw-rw-   0        0        0     1571 2023-07-16 00:00:51.000000 EASYPLOT_TOOLBOX-2023.6/EASYPLOT_TOOLBOX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-16 00:00:51.000000 EASYPLOT_TOOLBOX-2023.6/EASYPLOT_TOOLBOX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 00:00:51.000000 EASYPLOT_TOOLBOX-2023.6/EASYPLOT_TOOLBOX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-16 00:00:51.000000 EASYPLOT_TOOLBOX-2023.6/EASYPLOT_TOOLBOX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-16 00:00:51.000000 EASYPLOT_TOOLBOX-2023.6/EASYPLOT_TOOLBOX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1571 2023-07-16 00:00:51.774305 EASYPLOT_TOOLBOX-2023.6/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2023-07-15 23:52:16.000000 EASYPLOT_TOOLBOX-2023.6/license.md
--rw-rw-rw-   0        0        0       42 2023-07-16 00:00:51.775308 EASYPLOT_TOOLBOX-2023.6/setup.cfg
--rw-rw-rw-   0        0        0     1481 2023-07-16 00:00:46.000000 EASYPLOT_TOOLBOX-2023.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:26:32.456637 EASYPLOT_TOOLBOX-2023.7/
+drwxrwxrwx   0        0        0        0 2023-07-25 14:26:32.433630 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX/
+-rw-rw-rw-   0        0        0    13687 2023-07-25 14:25:53.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX/EASYPLOT.py
+-rw-rw-rw-   0        0        0       23 2023-03-09 15:47:42.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:26:32.454635 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/
+-rw-rw-rw-   0        0        0      618 2023-07-25 14:26:32.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-25 14:26:32.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:26:32.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-25 14:26:32.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-25 14:26:32.000000 EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      618 2023-07-25 14:26:32.455635 EASYPLOT_TOOLBOX-2023.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2023-07-25 14:25:53.000000 EASYPLOT_TOOLBOX-2023.7/license.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:26:32.456637 EASYPLOT_TOOLBOX-2023.7/setup.cfg
+-rw-rw-rw-   0        0        0     1467 2023-07-25 14:26:29.000000 EASYPLOT_TOOLBOX-2023.7/setup.py
```

### Comparing `EASYPLOT_TOOLBOX-2023.6/EASYPLOT_TOOLBOX/EASYPLOT.py` & `EASYPLOT_TOOLBOX-2023.7/EASYPLOT_TOOLBOX/EASYPLOT.py`

 * *Files 10% similar despite different names*

```diff
@@ -303,63 +303,73 @@
 
     # Setup
     DATASET = kwargs.get('DATASET')
     PLOT_SETUP = kwargs.get('PLOT_SETUP')
     NAME = PLOT_SETUP['NAME']
     W = PLOT_SETUP['WIDTH']
     H = PLOT_SETUP['HEIGHT']
-    X_AXIS_SIZE = PLOT_SETUP['X AXIS SIZE']
-    AXISES_COLOR = PLOT_SETUP['AXISES COLOR']
-    LEGEND_SIZE = PLOT_SETUP['LEGEND SIZE']
-    LINE_WIDTH = PLOT_SETUP['LINE WIDTH']
-    GRID = PLOT_SETUP['ON GRID?']
+    RADAR_DIV_SIZE = PLOT_SETUP['TEXT SIZE']
+    RADAR_DIV_COLOR = PLOT_SETUP['DIV COLOR']
+    RADAR_COLOR = PLOT_SETUP['RADAR COLOR']
+    OPACITY = PLOT_SETUP['OPACITY']
+    POLAR_COLOR = PLOT_SETUP['BACKGROUND']
+    SIZE_LEGEND = PLOT_SETUP['LEGEND SIZE']
     DPI = PLOT_SETUP['DPI']
     EXT = PLOT_SETUP['EXTENSION']
     
-    #Dataset
-    CATEGORIAS = DATASET['CATEGORIES']
-    VALORES = DATASET['VALUES']
-    CORES = DATASET['COLORS']
-    LEGENDAS = DATASET['LEGENDS']
-
-    # Calcular os ângulos para cada categoria
-    num_categorias = len(CATEGORIAS)
-    angulos = np.linspace(0, 2 * np.pi, num_categorias, endpoint=False).tolist()
+    # Dataset
+    DATA = DATASET['COMPLETE DATA']
+    RADAR_DIV = DATASET['DIVS']
+    RADAR_LABEL = DATASET['DIV LABELS']
 
+    # Plot
     W, H = CONVERT_SI_TO_INCHES(W, H)
-    fig, AX = plt.subplots(1, 1, figsize=(W, H),subplot_kw={'projection': 'polar'})
-    
-    maximo = 0
-    
-    legendas = []
-    for valor, cor, legenda in zip(VALORES, CORES, LEGENDAS):
-        max_local = max(valor)
-        if max_local > maximo:
-            maximo = max_local
-        # Plotar as linhas do gráfico de radar
-        linha, = AX.plot(angulos, valor, color=cor, linewidth=LINE_WIDTH, label=legenda)
-        # Preencher as áreas entre as linhas
-        AX.fill(angulos, valor, cor, alpha=0.25)
-        # Criar as legendas
-        legendas.append(Line2D([0], [0], color=cor, linewidth=LINE_WIDTH, label=legenda)) 
-    
-    # Configurar os rótulos das categorias
-    AX.set_xticks(angulos)
-    AX.set_xticklabels(CATEGORIAS,position=(-0.2, -0.05, 0.3))
-    AX.tick_params(axis = 'x', labelsize = X_AXIS_SIZE, colors = AXISES_COLOR, labelrotation = 0, direction = 'out', which = 'both', length = 10)
-
-    # Configurar os limites dos eixos
-    AX.set_ylim(0, maximo)
-
-    # Adicionar as legendas ao gráfico
-    legenda = AX.legend(handles=legendas, loc='upper right', bbox_to_anchor=(1.3, 1),fontsize=LEGEND_SIZE)
+    FIG, AX = plt.subplots(1, 1, figsize = (W, H), subplot_kw = {'projection': 'polar'})
+    CATEGORIES = list(DATA)[1:]
+    N = len(CATEGORIES)
+    print(N)
+    angles = [n / float(N) * 2 * np.pi for n in range(N)]
+    angles += angles[:1]
+    AX.set_theta_offset(np.pi / 2)
+    AX.set_theta_direction(-1)  
+    plt.xticks(angles[:-1], CATEGORIES, size = RADAR_DIV_SIZE)  
+    AX.set_rlabel_position(180 / N)
+    angless = np.linspace(0, 2 * np.pi, N, endpoint = False).tolist()
+    for label, anglee in zip(AX.get_xticklabels(), angless):
+        if anglee in (0, np.pi):
+            label.set_horizontalalignment('center')
+        elif 0 < anglee < np.pi:
+            label.set_horizontalalignment('left')
+        else:
+            label.set_horizontalalignment('right')
+    plt.yticks(RADAR_DIV, RADAR_LABEL, color = RADAR_DIV_COLOR, size = RADAR_DIV_SIZE)
+    max_value = max(list(DATA.max())[1:])
+    plt.ylim(0, max_value)
+    for I in range(len(list(DATA['group']))):
+        GROUP = list(DATA['group'])
+        values=DATA.loc[I].drop('group').values.flatten().tolist()
+        values += values[:1]
+        AX.plot(angles, values, linewidth = 2, linestyle = '--', label = GROUP[I], c = RADAR_COLOR[I])
+        AX.fill(angles, values, RADAR_COLOR[I], alpha = OPACITY)
+    AX.set_facecolor(POLAR_COLOR)
+    plt.legend(loc = 'upper right', bbox_to_anchor = (0.1, 0.1), prop = {'size': SIZE_LEGEND})
 
-    # Adicionar título
-    plt.title(NAME)
+    SAVE_GRAPHIC(NAME, EXT, DPI)
 
-    # Ajustar o layout para evitar sobreposição
-    plt.tight_layout()
+"""
+def TREEMAP_CHART(**kwargs):
     
-    if GRID == True:
-        AX.grid(color = 'grey', linestyle = '-.', linewidth = 1, alpha = 0.20)
-        
-    SAVE_GRAPHIC(NAME, EXT, DPI)
+    libraries
+    #!pip install squarify
+    import matplotlib.pyplot as plt
+    import squarify    # pip install squarify (algorithm for treemap)
+    import pandas as pd
+
+    # Create a data frame with fake data
+    df = pd.DataFrame({'nb_people':[8,3,4,2], 'group':["group A", "group B", "group C", "group D"] })
+
+    # plot it
+    colors = ["red", "black", "green","violet"]
+    squarify.plot(sizes=df['nb_people'], label=df['group'], alpha=.2, color=colors)
+    plt.axis('off')
+    plt.show()
+"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `EASYPLOT_TOOLBOX-2023.6/license.md` & `EASYPLOT_TOOLBOX-2023.7/license.md`

 * *Files identical despite different names*

### Comparing `EASYPLOT_TOOLBOX-2023.6/setup.py` & `EASYPLOT_TOOLBOX-2023.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from setuptools import setup, find_packages
-from pathlib import Path
-this_directory = Path(__file__).parent
-this_directory = Path(__file__).resolve().parent
-readme_path = this_directory / "readme.md"
-long_description = readme_path.read_text(encoding='utf-8')
+# from pathlib import Path
+# this_directory = Path(__file__).resolve().parent
+# readme_path = this_directory / "readme.md"
+# long_description = readme_path.read_text(encoding = 'utf-8')
 
 setup(
     	name = 'EASYPLOT_TOOLBOX',
-    	version = '2023.6',
+    	version = '2023.7',
 		url = 'https://wmpjrufg.github.io/EASYPLOTPY/',
     	description = 'The Easyplotpy toolboox is an algorithm that aims to facilitate the plotting of charts for use in articles and lectures.',
-		long_description = long_description,
-		long_description_content_type='text/markdown',        
+		# long_description = long_description,
+		# long_description_content_type='text/markdown',        
 		keywords = ["Plot", "Learning"],
 		license = 'MIT License',
         readme = 'readme.md',
 		authors = ['Wanderlei Malaquias Pereira Junior', 'Sergio Francisco da Silva', 'Nilson Jorge Leão Junior', 'Mateus Pereira da Silva'],
 		author_email = 'wanderlei_junior@ufcat.edu.br',
     	maintainers = ['Wanderlei Malaquias Pereira Junior', 'Mateus Pereira da Silva'],
-    	install_requires = ["matplotlib", "seaborn"],
+    	install_requires = ["matplotlib", "seaborn", "squarify"],
 		classifiers = [	
             			'Development Status :: 4 - Beta',
             			'Topic :: Education',
                         'Topic :: Multimedia :: Graphics',
                         'License :: OSI Approved :: MIT License',
                   		'Framework :: Matplotlib', 
 						'Programming Language :: Python',
```

