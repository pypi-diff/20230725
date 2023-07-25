# Comparing `tmp/muller-eot-1.3.2.tar.gz` & `tmp/muller-eot-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/muller-eot-1.3.2.tar", last modified: Fri Jan 20 01:29:23 2023, max compression
+gzip compressed data, was "dist/muller-eot-1.4.2.tar", last modified: Tue Jul 25 20:01:47 2023, max compression
```

## Comparing `muller-eot-1.3.2.tar` & `muller-eot-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-20 01:29:23.036808 muller-eot-1.3.2/
--rw-rw-r--   0 user      (1000) user      (1000)    10296 2023-01-20 01:29:23.036808 muller-eot-1.3.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     7702 2023-01-20 01:27:48.000000 muller-eot-1.3.2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-20 01:29:23.032808 muller-eot-1.3.2/muller_eot/
--rw-rw-r--   0 user      (1000) user      (1000)      415 2022-11-25 10:23:47.000000 muller-eot-1.3.2/muller_eot/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6324 2022-12-04 09:14:00.000000 muller-eot-1.3.2/muller_eot/calculate_eot.py
--rw-rw-r--   0 user      (1000) user      (1000)     5802 2023-01-04 00:36:51.000000 muller-eot-1.3.2/muller_eot/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1199 2022-12-01 09:29:28.000000 muller-eot-1.3.2/muller_eot/helper_function.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-20 01:29:23.036808 muller-eot-1.3.2/muller_eot.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    10296 2023-01-20 01:29:22.000000 muller-eot-1.3.2/muller_eot.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      297 2023-01-20 01:29:23.000000 muller-eot-1.3.2/muller_eot.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-01-20 01:29:22.000000 muller-eot-1.3.2/muller_eot.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       32 2023-01-20 01:29:22.000000 muller-eot-1.3.2/muller_eot.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       11 2023-01-20 01:29:22.000000 muller-eot-1.3.2/muller_eot.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-01-20 01:29:23.036808 muller-eot-1.3.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1653 2023-01-20 01:27:21.000000 muller-eot-1.3.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 20:01:47.437437 muller-eot-1.4.2/
+-rw-rw-r--   0 user      (1000) user      (1000)    11162 2023-07-25 20:01:47.437437 muller-eot-1.4.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     8529 2023-07-17 05:20:45.000000 muller-eot-1.4.2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 20:01:47.433437 muller-eot-1.4.2/muller_eot/
+-rw-rw-r--   0 user      (1000) user      (1000)      442 2023-07-16 08:47:15.000000 muller-eot-1.4.2/muller_eot/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6318 2023-07-17 05:16:22.000000 muller-eot-1.4.2/muller_eot/calculate_eot.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1116 2023-07-17 05:20:01.000000 muller-eot-1.4.2/muller_eot/eotClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3708 2023-07-17 04:39:04.000000 muller-eot-1.4.2/muller_eot/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1199 2022-12-01 09:29:28.000000 muller-eot-1.4.2/muller_eot/helper_function.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 20:01:47.437437 muller-eot-1.4.2/muller_eot.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    11162 2023-07-25 20:01:47.000000 muller-eot-1.4.2/muller_eot.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      320 2023-07-25 20:01:47.000000 muller-eot-1.4.2/muller_eot.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 20:01:47.000000 muller-eot-1.4.2/muller_eot.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       32 2023-07-25 20:01:47.000000 muller-eot-1.4.2/muller_eot.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       11 2023-07-25 20:01:47.000000 muller-eot-1.4.2/muller_eot.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 20:01:47.437437 muller-eot-1.4.2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1652 2023-07-25 19:59:23.000000 muller-eot-1.4.2/setup.py
```

### Comparing `muller-eot-1.3.2/PKG-INFO` & `muller-eot-1.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,110 @@
 Metadata-Version: 2.1
 Name: muller-eot
-Version: 1.3.2
+Version: 1.4.2
 Summary: A Python package for M. Müller implementation of the 'Equation of Time - Problem in Astronomy' to calculate EOT and the effect of eccentricity/obliquity
 Home-page: https://github.com/cyschneck/Muller-EOT
-Author: cyschneck (C. Y. Schneck)
+Author: Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/Muller-EOT/archive/refs/tags/v1.3.2.tar.gz
+Download-URL: https://github.com/cyschneck/Muller-EOT/archive/refs/tags/v1.4.2.tar.gz
 Description: # Muller-EOT
         ![PyPi](https://img.shields.io/pypi/v/muller-eot)
         ![license](https://img.shields.io/github/license/cyschneck/Muller-EOT)
         
         A Python package for [M. Müller implementation of the "Equation of Time - Problem in Astronomy"](http://info.ifpan.edu.pl/firststep/aw-works/fsII/mul/mueller.pdf) to calculate the Equation of Time based on the individual effect of eccentricity and obliquity
         
+        ## Quickstart: muller-eot
+        
+        Get a list of differences in time for each day of the Earth's orbit and then plot it as a function of days in orbit
+        
+        ```
+        import muller_eot
+        
+        earth_eot = muller_eot.EOT(eccentricity=0.0167, obliquity=23.45, orbit_period=365.25)
+        earth_eot.plotEOT()
+        ```
+        ![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_quickstart.png)
+        
+        ## Install
+        PyPi pip install at [pypi.org/project/muller-eot/](https://pypi.org/project/muller-eot/)
+        
+        ```
+        pip install muller-eot
+        ```
+        ## Dependencies
+        Python 3.7+
+        ```
+        pip install -r requirements.txt
+        ```
+        Requirements will also be downloaded as part of the pip download
+        
+        ## Functions
         The combined effect of eccentricity and obliquity create the Equation of Time components.
         
         | Effect of Eccentricity | Effect of Obliquity |
         | ------------- | ------------- |
-        | ![effect_eccentricity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eccentricity_testing.png) | ![effect_obliquity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_obliquity_testing.png) |
+        | ![effect_eccentricity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eccentricity.png) | ![effect_obliquity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_obliquity.png) |
         
         Combined Effect of the Eccentricity and Obliquity = Equation of Time
-        ![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eot_testing.png)
+        ![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eot.png)
+        
+        ### EOT Object
+        All Equation of Time calculations are done as a part of the EOT class object. First, create an EOT object for a specific eccentricity, obliquity, and orbit period (in days)
+        ```python
+        import muller_eot
+        muller_eot.EOT(eccentricity=None,
+        		obliquity=None,
+        		orbit_period=None)
+        ```
+        - **[REQUIRED]** eccentricity (float/int): eccentricity of the planet's orbit
+        - **[REQUIRED]** obliquity (float/int): obliquity/axial tilt of the planet
+        - **[REQUIRED]** orbit_period (float/int): days in a solar year
+        
+        
+        ### EOT Class Attributes and Functions
+        
+        **eotDayAndMinutes**
+        Returns a dictionary for the difference in time for each day in a year {number_day: time difference}
+        ```python
+        EOT.eotDayAndMinutes
+        ```
+        
+        **plotEOT**
+        Plot the differences in time for the EOT as well as the individual effect of obliquity and eccentricity
+        ```python
+        EOT.plotEOT(plot_title=None,
+        		plot_x_title=None,
+        		plot_y_title=None,
+        		show_plot=True,
+        		fig_plot_color="cornflowerblue",
+        		figsize_n=12,
+        		figsize_dpi=100,
+        		save_plot_name=None)
+        ```
+        - *[OPTIONAL]* plot_title (string): Title of plot, defaults to `EOT Minute Difference (Min = <negative minutes>, Max = <postive minutes>)`
+        - *[OPTIONAL]* plot_x_title (string): X-axis title, defaults to `Days in the Sidereal Year`
+        - *[OPTIONAL]* plot_y_title (string): Y-axis title, defaults to `Time Difference (Minutes)`
+        - *[OPTIONAL]* show_plot (boolean): Show plot (triggers plt.show()), useful when generating multiple plots at once in the background, defaults to True
+        - *[OPTIONAL]* fig_plot_color (string): Scatter plot color, defaults to `cornflowerblue` blue
+        - *[OPTIONAL]* figsize_n (int/float): Figure size nxn, defaults to 12x12
+        - *[OPTIONAL]* figsize_dpi (int/lfoat): Figure DPI, defaults to 100
+        - *[OPTIONAL]* save_plot_name (boolean): Save plot as output, defaults to None (does not save)
         
-        ## Overview
+        ## Background
         
         The length of a day on Earth is only close to being 24 hours four times a year. For the rest of the year when the sun is at its highest point (solar noon), a clock can run as much as 16 minutes ahead (12:16pm) or 13 minutes behind (11:47am). This discrepancy is the result of the combined effect of a planet's obliquity (axial tilt) and its eccentricity (as well as other smaller gravitational forces like moons that are ignored here). Both of these features form two sine curves that oscillate throughout the year. The combined sum
         of these two curves form the Equation of Time, a non-uniform change in time to fix to a clock.
         A planet with an obliquity of 0° and perfectly circular orbit (zero eccentricity) would have
         no difference in the Expected Solar Noon and the Actual Solar Noon.
         
+        To calculate the difference in time for an individual day:
+        <p align="center">
+          <img src="https://user-images.githubusercontent.com/22159116/203877814-c2d710f3-0681-4f72-8607-0f96e2a33256.png" />
+        </p>
+        
         Equation of Time = (Apparent Solar Time) - (Mean Solar Time) 
         
         **Effect of Eccentricity:**
         <p align="center">
           <img src="https://user-images.githubusercontent.com/22159116/203484492-bf0f6098-fe13-44d3-b372-bcb8cc4120f8.png" />
         </p>
         
@@ -92,89 +165,21 @@
         compensate each other in winter whereas the negative value in summer begins to dominate." (Müller, 1995)
         
         Equation of Time is the combination of the effect of eccentricity and obliquity
         <p align="center">
           <img src="https://user-images.githubusercontent.com/22159116/203484851-c96be35a-2d4a-44df-a2ee-a9d88974aa9e.png" />
         </p>
         
-        To calculate the difference in time for an individual day:
-        <p align="center">
-          <img src="https://user-images.githubusercontent.com/22159116/203877814-c2d710f3-0681-4f72-8607-0f96e2a33256.png" />
-        </p>
-        
-        ## Documentation
-        **calculateDifferenceEOTMinutes**
-        Calculate the difference in time (in minutes) based on orbital period, eccentricity, and obliquity. Returns a list of differences in time for each day in the orbital year
-        ```
-        calculateDifferenceEOTMinutes(eccentricity=None,
-        				obliquity_deg=None,
-        				orbit_period=None)
-        ```
-        Returns a dictionary for the difference in time for each day in a year {day: time difference}
-        
-        **plotEOT**
-        Plot the differences in time for the EOT as well as the individual effect of obliquity and eccentricity
-        ```
-        plotEOT(planet_name=None,
-        	eot_dict={},
-        	effect_title_str=None,
-        	plot_title=None,
-        	plot_x_title=None,
-        	plot_y_title=None,
-        	showPlot=True,
-        	fig_plot_color="C0",
-        	figsize_n=12,
-        	figsize_dpi=100,
-        	save_plot_name=None)
-        ```
-        ## Dependencies
-        Python 3.7+
-        ```
-        pip3 install -r requirements.txt
-        ```
-        ## Install
-        PyPi pip install at [pypi.org/project/muller-eot/](https://pypi.org/project/muller-eot/)
-        
-        ```
-        pip install muller-eot
-        ```
-        ## Examples
-        
-        Get a list of differences in time for each day of the Earth's orbit and then plot it as a function of days in orbit
-        
-        ```
-        import muller_eot
-        
-        # Get a list of time differences for each day
-        eot_combined_dict = muller_eot.calculateDifferenceEOTMinutes(eccentricity=0.0167,
-        							obliquity_deg=23.45,
-        							orbit_period=365.25)
-        
-        # Plot differences in time as a function of days
-        muller_eot.plotEOT(planet_name="Earth",
-        		eot_dict=eot_combined_dict,
-        		effect_title_str="Eccentricity (0.0167) and Obliquity (23.45)")
-        ```
-        ![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eot_testing.png)
-        
-        ## Tests
-        
-        TODO
-        
-        ## TODO:
-        
-        calculateOrbitalPeriod(semimajor_axis) function
-        
-        calculateDistanceBetweenSolisticePerhelion() function
-        
-        calculatePerihelionDay() function
-        
-        calculateWinterSolsticeDay() function
-        
-        calculateEccentricity() function
+        ### TODO:
+        - Pytests
+        - calculateOrbitalPeriod(semimajor_axis)
+        - calculateDistanceBetweenSolisticePerhelion()
+        - calculatePerihelionDay()
+        - calculateWinterSolsticeDay()
+        - calculateEccentricity()
         
 Keywords: astronomy,python,eot,equation of time,eccentricity,obliquity,orbital dynamics
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `muller-eot-1.3.2/README.md` & `muller-eot-1.4.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,102 @@
 # Muller-EOT
 ![PyPi](https://img.shields.io/pypi/v/muller-eot)
 ![license](https://img.shields.io/github/license/cyschneck/Muller-EOT)
 
 A Python package for [M. Müller implementation of the "Equation of Time - Problem in Astronomy"](http://info.ifpan.edu.pl/firststep/aw-works/fsII/mul/mueller.pdf) to calculate the Equation of Time based on the individual effect of eccentricity and obliquity
 
+## Quickstart: muller-eot
+
+Get a list of differences in time for each day of the Earth's orbit and then plot it as a function of days in orbit
+
+```
+import muller_eot
+
+earth_eot = muller_eot.EOT(eccentricity=0.0167, obliquity=23.45, orbit_period=365.25)
+earth_eot.plotEOT()
+```
+![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_quickstart.png)
+
+## Install
+PyPi pip install at [pypi.org/project/muller-eot/](https://pypi.org/project/muller-eot/)
+
+```
+pip install muller-eot
+```
+## Dependencies
+Python 3.7+
+```
+pip install -r requirements.txt
+```
+Requirements will also be downloaded as part of the pip download
+
+## Functions
 The combined effect of eccentricity and obliquity create the Equation of Time components.
 
 | Effect of Eccentricity | Effect of Obliquity |
 | ------------- | ------------- |
-| ![effect_eccentricity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eccentricity_testing.png) | ![effect_obliquity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_obliquity_testing.png) |
+| ![effect_eccentricity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eccentricity.png) | ![effect_obliquity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_obliquity.png) |
 
 Combined Effect of the Eccentricity and Obliquity = Equation of Time
-![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eot_testing.png)
+![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eot.png)
+
+### EOT Object
+All Equation of Time calculations are done as a part of the EOT class object. First, create an EOT object for a specific eccentricity, obliquity, and orbit period (in days)
+```python
+import muller_eot
+muller_eot.EOT(eccentricity=None,
+		obliquity=None,
+		orbit_period=None)
+```
+- **[REQUIRED]** eccentricity (float/int): eccentricity of the planet's orbit
+- **[REQUIRED]** obliquity (float/int): obliquity/axial tilt of the planet
+- **[REQUIRED]** orbit_period (float/int): days in a solar year
+
+
+### EOT Class Attributes and Functions
+
+**eotDayAndMinutes**
+Returns a dictionary for the difference in time for each day in a year {number_day: time difference}
+```python
+EOT.eotDayAndMinutes
+```
+
+**plotEOT**
+Plot the differences in time for the EOT as well as the individual effect of obliquity and eccentricity
+```python
+EOT.plotEOT(plot_title=None,
+		plot_x_title=None,
+		plot_y_title=None,
+		show_plot=True,
+		fig_plot_color="cornflowerblue",
+		figsize_n=12,
+		figsize_dpi=100,
+		save_plot_name=None)
+```
+- *[OPTIONAL]* plot_title (string): Title of plot, defaults to `EOT Minute Difference (Min = <negative minutes>, Max = <postive minutes>)`
+- *[OPTIONAL]* plot_x_title (string): X-axis title, defaults to `Days in the Sidereal Year`
+- *[OPTIONAL]* plot_y_title (string): Y-axis title, defaults to `Time Difference (Minutes)`
+- *[OPTIONAL]* show_plot (boolean): Show plot (triggers plt.show()), useful when generating multiple plots at once in the background, defaults to True
+- *[OPTIONAL]* fig_plot_color (string): Scatter plot color, defaults to `cornflowerblue` blue
+- *[OPTIONAL]* figsize_n (int/float): Figure size nxn, defaults to 12x12
+- *[OPTIONAL]* figsize_dpi (int/lfoat): Figure DPI, defaults to 100
+- *[OPTIONAL]* save_plot_name (boolean): Save plot as output, defaults to None (does not save)
 
-## Overview
+## Background
 
 The length of a day on Earth is only close to being 24 hours four times a year. For the rest of the year when the sun is at its highest point (solar noon), a clock can run as much as 16 minutes ahead (12:16pm) or 13 minutes behind (11:47am). This discrepancy is the result of the combined effect of a planet's obliquity (axial tilt) and its eccentricity (as well as other smaller gravitational forces like moons that are ignored here). Both of these features form two sine curves that oscillate throughout the year. The combined sum
 of these two curves form the Equation of Time, a non-uniform change in time to fix to a clock.
 A planet with an obliquity of 0° and perfectly circular orbit (zero eccentricity) would have
 no difference in the Expected Solar Noon and the Actual Solar Noon.
 
+To calculate the difference in time for an individual day:
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/22159116/203877814-c2d710f3-0681-4f72-8607-0f96e2a33256.png" />
+</p>
+
 Equation of Time = (Apparent Solar Time) - (Mean Solar Time) 
 
 **Effect of Eccentricity:**
 <p align="center">
   <img src="https://user-images.githubusercontent.com/22159116/203484492-bf0f6098-fe13-44d3-b372-bcb8cc4120f8.png" />
 </p>
 
@@ -84,82 +157,14 @@
 compensate each other in winter whereas the negative value in summer begins to dominate." (Müller, 1995)
 
 Equation of Time is the combination of the effect of eccentricity and obliquity
 <p align="center">
   <img src="https://user-images.githubusercontent.com/22159116/203484851-c96be35a-2d4a-44df-a2ee-a9d88974aa9e.png" />
 </p>
 
-To calculate the difference in time for an individual day:
-<p align="center">
-  <img src="https://user-images.githubusercontent.com/22159116/203877814-c2d710f3-0681-4f72-8607-0f96e2a33256.png" />
-</p>
-
-## Documentation
-**calculateDifferenceEOTMinutes**
-Calculate the difference in time (in minutes) based on orbital period, eccentricity, and obliquity. Returns a list of differences in time for each day in the orbital year
-```
-calculateDifferenceEOTMinutes(eccentricity=None,
-				obliquity_deg=None,
-				orbit_period=None)
-```
-Returns a dictionary for the difference in time for each day in a year {day: time difference}
-
-**plotEOT**
-Plot the differences in time for the EOT as well as the individual effect of obliquity and eccentricity
-```
-plotEOT(planet_name=None,
-	eot_dict={},
-	effect_title_str=None,
-	plot_title=None,
-	plot_x_title=None,
-	plot_y_title=None,
-	showPlot=True,
-	fig_plot_color="C0",
-	figsize_n=12,
-	figsize_dpi=100,
-	save_plot_name=None)
-```
-## Dependencies
-Python 3.7+
-```
-pip3 install -r requirements.txt
-```
-## Install
-PyPi pip install at [pypi.org/project/muller-eot/](https://pypi.org/project/muller-eot/)
-
-```
-pip install muller-eot
-```
-## Examples
-
-Get a list of differences in time for each day of the Earth's orbit and then plot it as a function of days in orbit
-
-```
-import muller_eot
-
-# Get a list of time differences for each day
-eot_combined_dict = muller_eot.calculateDifferenceEOTMinutes(eccentricity=0.0167,
-							obliquity_deg=23.45,
-							orbit_period=365.25)
-
-# Plot differences in time as a function of days
-muller_eot.plotEOT(planet_name="Earth",
-		eot_dict=eot_combined_dict,
-		effect_title_str="Eccentricity (0.0167) and Obliquity (23.45)")
-```
-![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eot_testing.png)
-
-## Tests
-
-TODO
-
-## TODO:
-
-calculateOrbitalPeriod(semimajor_axis) function
-
-calculateDistanceBetweenSolisticePerhelion() function
-
-calculatePerihelionDay() function
-
-calculateWinterSolsticeDay() function
-
-calculateEccentricity() function
+### TODO:
+- Pytests
+- calculateOrbitalPeriod(semimajor_axis)
+- calculateDistanceBetweenSolisticePerhelion()
+- calculatePerihelionDay()
+- calculateWinterSolsticeDay()
+- calculateEccentricity()
```

### Comparing `muller-eot-1.3.2/muller_eot/calculate_eot.py` & `muller-eot-1.4.2/muller_eot/calculate_eot.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 # t = time span after passaage through the perihelion
 # M = 2pi * (t/T) ==> mean anomaly = (time span since perhelion / total time) in radians
 # E = (angle) eccentric anomaly: used to calculate the area of elliptic sectors
 # e = eccentricity of Earth = 0.0167
 # ε = obliquity of Earth = 23.45◦
 
 def calculateDifferenceEOTMinutes(eccentricity=None,
-								obliquity_deg=None,
+								obliquity=None,
 								orbit_period=None):
 	# Calculate the time difference (in minutes) for the Equation of Time
 
-	muller_eot.errorHandlingEOT(eccentricity,
-								obliquity_deg,
-								orbit_period) # Verify argument behavior
+	muller_eot.errorHandlingEOT(eccentricity=eccentricity,
+								obliquity=obliquity,
+								orbit_period=orbit_period)
 
 	distance_between_solistice_perhelion_deg = muller_eot.calculateDistanceBetweenSolisticePerhelion()
 	distance_between_solistice_perhelion_rad = np.deg2rad(distance_between_solistice_perhelion_deg)
 
-	obliquity_rad = np.deg2rad(obliquity_deg)
+	obliquity_rad = np.deg2rad(obliquity)
 
 	minutes_conversion = (24 * 60) / (2 * math.pi)
 	perihelion_day = muller_eot.calculatePerihelionDay()
 
 	eot_dict = {} # { day : eot_min_difference }
 	orbit_days_x = np.arange(1, round(orbit_period)+1, 1)
 
@@ -85,38 +85,33 @@
 		sin6_m_p = math.sin(6 * (mean_anomaly + distance_between_solistice_perhelion_rad)) # sin6(M + P)
 		line_five = tan6_1_3 * sin6_m_p
 
 		eot_min_difference = -( line_one + line_two + line_three + line_four + line_five)*minutes_conversion
 		eot_dict[day] = eot_min_difference
 	return eot_dict
 
-def plotEOT(planet_name=None,
-			eot_dict={},
-			effect_title_str=None,
+def plotEOT(eot_dict=None,
 			plot_title=None,
 			plot_x_title=None,
 			plot_y_title=None,
-			showPlot=True,
-			fig_plot_color="C0",
-			figsize_n=12,
-			figsize_dpi=100,
+			show_plot=None,
+			fig_plot_color=None,
+			figsize_n=None,
+			figsize_dpi=None,
 			save_plot_name=None):
 	# Plot EOT Time Differences
-
-	muller_eot.errorHandlingPlotEOT(planet_name,
-									eot_dict,
-									effect_title_str,
-									plot_title,
-									plot_x_title,
-									plot_y_title,
-									showPlot,
-									fig_plot_color,
-									figsize_n,
-									figsize_dpi,
-									save_plot_name) # Verify argument behavior
+	muller_eot.errorHandlingPlotEOT(eot_dict=eot_dict,
+									plot_title=plot_title,
+									plot_x_title=plot_x_title,
+									plot_y_title=plot_y_title,
+									show_plot=show_plot,
+									fig_plot_color=fig_plot_color,
+									figsize_n=figsize_n,
+									figsize_dpi=figsize_dpi,
+									save_plot_name=save_plot_name) # Verify argument behavior
 
 	fig = plt.figure(figsize=(figsize_n,figsize_n), dpi=figsize_dpi)
 
 	# X Axis = orbital days in year, Y Axis = minute differences for EOT
 	orbit_days_x = eot_dict.keys()
 	eot_y = eot_dict.values()
 
@@ -125,21 +120,23 @@
 	for i, value in enumerate(date_range_split_into_months): date_range_split_into_months[i] = math.floor(value) # round all values
 
 	plt.xticks(date_range_split_into_months)
 	plt.xlim([min(date_range_split_into_months), max(date_range_split_into_months)])
 	plt.scatter(orbit_days_x, eot_y, c=fig_plot_color)
 	plt.grid()
 
-	if plot_title is None: plt.title("{0}: Effect of {1} (Min = {2:.4f}, Max = {3:.4f})".format(planet_name, effect_title_str, min(eot_y), max(eot_y)))
-	else: plt.title(plot_title)
+	if plot_title is None: 
+		plt.title("EOT Minute Difference (Min = {0:.4f}, Max = {1:.4f})".format(min(eot_y), max(eot_y)))
+	else: 
+		plt.title(plot_title)
 
 	if plot_x_title is None: plt.xlabel("Days in the Sidereal Year")
 	else: plt.xlabel(plot_x_title)
 
 	if plot_y_title is None: plt.ylabel("Time Difference (Minutes)")
 	else: plt.ylabel(plot_y_title)
 
-	if showPlot:
+	if show_plot:
 		plt.show()
 
 	if save_plot_name:
 		fig.savefig(save_plot_name)
```

### Comparing `muller-eot-1.3.2/muller_eot/error_handling.py` & `muller-eot-1.4.2/muller_eot/error_handling.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,126 +5,85 @@
 
 ## Logging set up for .INFO
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.CRITICAL)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
-def errorHandlingEOT(eccentricity,
-					obliquity_deg,
-					orbit_period):
+def errorHandlingEOT(eccentricity=None,
+					obliquity=None,
+					orbit_period=None):
 
 	# Ensure that eccentricity is a float or int
+	if eccentricity is None:
+		logger.critical("\nCRITICAL ERROR, [eccentricity]: eccentricity is required")
+		exit()
 	if eccentricity is not None and type(eccentricity) != int and type(eccentricity) != float:
 		logger.critical("\nCRITICAL ERROR, [eccentricity]: Must be a int or float, current type = '{0}'".format(type(eccentricity)))
 		exit()
-	if eccentricity is None:
-		logger.critical("\nCRITICAL ERROR, [eccentricity]: Must be a int or float, currently is 'None'")
-		exit()
-	logger.debug("eccentricity = '{0}'".format(eccentricity))
 
-	# Ensure that obliquity_deg is a float or int
-	if obliquity_deg is not None and type(obliquity_deg) != int and type(obliquity_deg) != float:
-		logger.critical("\nCRITICAL ERROR, [obliquity_deg]: Must be a int or float, current type = '{0}'".format(type(obliquity_deg)))
+	# Ensure that obliquity is a float or int
+	if obliquity is None:
+		logger.critical("\nCRITICAL ERROR, [obliquity]: obliquity is required")
 		exit()
-	if obliquity_deg is None:
-		logger.critical("\nCRITICAL ERROR, [obliquity_deg]: Must be a int or float, currently is 'None'")
+	if obliquity is not None and type(obliquity) != int and type(obliquity) != float:
+		logger.critical("\nCRITICAL ERROR, [obliquity]: Must be a int or float, current type = '{0}'".format(type(obliquity)))
 		exit()
-	logger.debug("obliquity_deg = '{0}'".format(obliquity_deg))
 
 	# Ensure that orbit_period is a float or int
-	if orbit_period is not None and type(orbit_period) != int and type(orbit_period) != float:
-		logger.critical("\nCRITICAL ERROR, [orbit_period]: Must be a int or float, current type = '{0}'".format(type(orbit_period)))
-		exit()
 	if orbit_period is None:
-		logger.critical("\nCRITICAL ERROR, [orbit_period]: Must be a int or float, currently is 'None'")
+		logger.critical("\nCRITICAL ERROR, [orbit_period]: orbit_period is required")
 		exit()
-	logger.debug("orbit_period = '{0}'".format(orbit_period))
-
-def errorHandlingPlotEOT(planet_name,
-						eot_dict,
-						effect_title_str,
-						plot_title,
-						plot_x_title,
-						plot_y_title,
-						showPlot,
-						fig_plot_color,
-						figsize_n,
-						figsize_dpi,
-						save_plot_name):
-
-	# Ensure that planet_name is a string
-	if type(planet_name) != str:
-		logger.critical("\nCRITICAL ERROR, [planet_name]: Must be a str, current type = '{0}'".format(type(planet_name)))
-		exit()
-	if planet_name is None:
-		logger.critical("\nCRITICAL ERROR, [planet_name]: Must be a int or float, currently is 'None'")
-		exit()
-	logger.debug("planet_name = '{0}'".format(planet_name))
-
-	# Ensure that all values in eot_dict for minute differences is a float or int
-	if type(eot_dict) is not dict:
-		logger.critical("\nCRITICAL ERROR, [eot_y]: Must be a dict, currently is '{0}'".format(type(eot_dict)))
-		exit()
-	for minute_dif in eot_dict.values():
-		if type(minute_dif) != int and type(minute_dif) != float:
-			logger.critical("\nCRITICAL ERROR, [eot_dict.values()]: Must be a int or float, current type = '{0}'".format(type(minute_dif)))
-			exit()
-	if len(eot_dict.values()) < 1:
-		logger.critical("\nCRITICAL ERROR, [eot_dict.values()]: Must have a length greater than zero")
+	if orbit_period is not None and type(orbit_period) != int and type(orbit_period) != float:
+		logger.critical("\nCRITICAL ERROR, [orbit_period]: Must be a int or float, current type = '{0}'".format(type(orbit_period)))
 		exit()
-	logger.debug("eot_dict = '{0}'".format(eot_dict))
+	
 
-	# Ensure that the effect title type is a string
-	if type(effect_title_str) != str:
-		logger.critical("\nCRITICAL ERROR, [effect_title_str]: Must be a str, current type = '{0}'".format(type(effect_title_str)))
-		exit()
-	if effect_title_str is None:
-		logger.critical("\nCRITICAL ERROR, [effect_title_str]: Must be a str, currently is 'None'")
+def errorHandlingPlotEOT(eot_dict=None,
+						plot_title=None,
+						plot_x_title=None,
+						plot_y_title=None,
+						show_plot=None,
+						fig_plot_color=None,
+						figsize_n=None,
+						figsize_dpi=None,
+						save_plot_name=None):
 
 	# Ensure that plot_title is a string
 	if plot_title is not None and type(plot_title) != str:
 		logger.critical("\nCRITICAL ERROR, [plot_title]: Must be a str, current type = '{0}'".format(type(plot_title)))
 		exit()
-	logger.debug("plot_title = '{0}'".format(plot_title))
 
 	# Ensure that plot_x_title is a string
 	if plot_x_title is not None and type(plot_x_title) != str:
 		logger.critical("\nCRITICAL ERROR, [plot_x_title]: Must be a str, current type = '{0}'".format(type(plot_x_title)))
 		exit()
-	logger.debug("plot_x_title = '{0}'".format(plot_x_title))
 
 	# Ensure that plot_y_title is a string
 	if plot_y_title is not None and type(plot_y_title) != str:
 		logger.critical("\nCRITICAL ERROR, [plot_y_title]: Must be a str, current type = '{0}'".format(type(plot_y_title)))
 		exit()
-	logger.debug("plot_y_title = '{0}'".format(plot_y_title))
 
-	# Ensure that all showPlot is a boolean ["True", "False"]
-	if type(showPlot) != bool:
-		logger.critical("\nCRITICAL ERROR, [showPlot]: Must be a bool, current type = '{0}'".format(type(showPlot)))
+	# Ensure that all show_plot is a boolean ["True", "False"]
+	if type(show_plot) != bool:
+		logger.critical("\nCRITICAL ERROR, [show_plot]: Must be a bool, current type = '{0}'".format(type(show_plot)))
 		exit()
-	logger.debug("showPlot = '{0}'".format(showPlot))
 
 	# Ensure that the color given is a string (matplotlib has error checking for invalid color options)
 	if type(fig_plot_color) != str:
 		logger.critical("\nCRITICAL ERROR, [fig_plot_color]: Must be a string, current type = '{0}'".format(type(fig_plot_color)))
 		exit()
-	logger.debug("fig_plot_color = '{0}'".format(fig_plot_color))
 
 	# Ensure that all figsize_n is a float or int
 	if type(figsize_n) != int and type(figsize_n) != float:
 		logger.critical("\nCRITICAL ERROR, [figsize_n]: Must be a int or float, current type = '{0}'".format(type(figsize_n)))
 		exit()
-	logger.debug("figsize_n = '{0}'".format(figsize_n))
 
 	# Ensure that all figsize_dpi is a float or int
 	if type(figsize_dpi) != int and type(figsize_dpi) != float:
 		logger.critical("\nCRITICAL ERROR, [figsize_dpi]: Must be a int or float, current type = '{0}'".format(type(figsize_dpi)))
 		exit()
-	logger.debug("figsize_dpi = '{0}'".format(figsize_dpi))
 
 	# Ensure that the effect title type is a string
 	if save_plot_name!= None and type(save_plot_name) != str:
 		logger.critical("\nCRITICAL ERROR, [save_plot_name]: Must be a str, current type = '{0}'".format(type(save_plot_name)))
 		exit()
-	logger.debug("save_plot_name = '{0}'".format(save_plot_name))
```

### Comparing `muller-eot-1.3.2/muller_eot/helper_function.py` & `muller-eot-1.4.2/muller_eot/helper_function.py`

 * *Files identical despite different names*

### Comparing `muller-eot-1.3.2/muller_eot.egg-info/PKG-INFO` & `muller-eot-1.4.2/muller_eot.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,110 @@
 Metadata-Version: 2.1
 Name: muller-eot
-Version: 1.3.2
+Version: 1.4.2
 Summary: A Python package for M. Müller implementation of the 'Equation of Time - Problem in Astronomy' to calculate EOT and the effect of eccentricity/obliquity
 Home-page: https://github.com/cyschneck/Muller-EOT
-Author: cyschneck (C. Y. Schneck)
+Author: Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/Muller-EOT/archive/refs/tags/v1.3.2.tar.gz
+Download-URL: https://github.com/cyschneck/Muller-EOT/archive/refs/tags/v1.4.2.tar.gz
 Description: # Muller-EOT
         ![PyPi](https://img.shields.io/pypi/v/muller-eot)
         ![license](https://img.shields.io/github/license/cyschneck/Muller-EOT)
         
         A Python package for [M. Müller implementation of the "Equation of Time - Problem in Astronomy"](http://info.ifpan.edu.pl/firststep/aw-works/fsII/mul/mueller.pdf) to calculate the Equation of Time based on the individual effect of eccentricity and obliquity
         
+        ## Quickstart: muller-eot
+        
+        Get a list of differences in time for each day of the Earth's orbit and then plot it as a function of days in orbit
+        
+        ```
+        import muller_eot
+        
+        earth_eot = muller_eot.EOT(eccentricity=0.0167, obliquity=23.45, orbit_period=365.25)
+        earth_eot.plotEOT()
+        ```
+        ![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_quickstart.png)
+        
+        ## Install
+        PyPi pip install at [pypi.org/project/muller-eot/](https://pypi.org/project/muller-eot/)
+        
+        ```
+        pip install muller-eot
+        ```
+        ## Dependencies
+        Python 3.7+
+        ```
+        pip install -r requirements.txt
+        ```
+        Requirements will also be downloaded as part of the pip download
+        
+        ## Functions
         The combined effect of eccentricity and obliquity create the Equation of Time components.
         
         | Effect of Eccentricity | Effect of Obliquity |
         | ------------- | ------------- |
-        | ![effect_eccentricity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eccentricity_testing.png) | ![effect_obliquity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_obliquity_testing.png) |
+        | ![effect_eccentricity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eccentricity.png) | ![effect_obliquity](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_obliquity.png) |
         
         Combined Effect of the Eccentricity and Obliquity = Equation of Time
-        ![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eot_testing.png)
+        ![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eot.png)
+        
+        ### EOT Object
+        All Equation of Time calculations are done as a part of the EOT class object. First, create an EOT object for a specific eccentricity, obliquity, and orbit period (in days)
+        ```python
+        import muller_eot
+        muller_eot.EOT(eccentricity=None,
+        		obliquity=None,
+        		orbit_period=None)
+        ```
+        - **[REQUIRED]** eccentricity (float/int): eccentricity of the planet's orbit
+        - **[REQUIRED]** obliquity (float/int): obliquity/axial tilt of the planet
+        - **[REQUIRED]** orbit_period (float/int): days in a solar year
+        
+        
+        ### EOT Class Attributes and Functions
+        
+        **eotDayAndMinutes**
+        Returns a dictionary for the difference in time for each day in a year {number_day: time difference}
+        ```python
+        EOT.eotDayAndMinutes
+        ```
+        
+        **plotEOT**
+        Plot the differences in time for the EOT as well as the individual effect of obliquity and eccentricity
+        ```python
+        EOT.plotEOT(plot_title=None,
+        		plot_x_title=None,
+        		plot_y_title=None,
+        		show_plot=True,
+        		fig_plot_color="cornflowerblue",
+        		figsize_n=12,
+        		figsize_dpi=100,
+        		save_plot_name=None)
+        ```
+        - *[OPTIONAL]* plot_title (string): Title of plot, defaults to `EOT Minute Difference (Min = <negative minutes>, Max = <postive minutes>)`
+        - *[OPTIONAL]* plot_x_title (string): X-axis title, defaults to `Days in the Sidereal Year`
+        - *[OPTIONAL]* plot_y_title (string): Y-axis title, defaults to `Time Difference (Minutes)`
+        - *[OPTIONAL]* show_plot (boolean): Show plot (triggers plt.show()), useful when generating multiple plots at once in the background, defaults to True
+        - *[OPTIONAL]* fig_plot_color (string): Scatter plot color, defaults to `cornflowerblue` blue
+        - *[OPTIONAL]* figsize_n (int/float): Figure size nxn, defaults to 12x12
+        - *[OPTIONAL]* figsize_dpi (int/lfoat): Figure DPI, defaults to 100
+        - *[OPTIONAL]* save_plot_name (boolean): Save plot as output, defaults to None (does not save)
         
-        ## Overview
+        ## Background
         
         The length of a day on Earth is only close to being 24 hours four times a year. For the rest of the year when the sun is at its highest point (solar noon), a clock can run as much as 16 minutes ahead (12:16pm) or 13 minutes behind (11:47am). This discrepancy is the result of the combined effect of a planet's obliquity (axial tilt) and its eccentricity (as well as other smaller gravitational forces like moons that are ignored here). Both of these features form two sine curves that oscillate throughout the year. The combined sum
         of these two curves form the Equation of Time, a non-uniform change in time to fix to a clock.
         A planet with an obliquity of 0° and perfectly circular orbit (zero eccentricity) would have
         no difference in the Expected Solar Noon and the Actual Solar Noon.
         
+        To calculate the difference in time for an individual day:
+        <p align="center">
+          <img src="https://user-images.githubusercontent.com/22159116/203877814-c2d710f3-0681-4f72-8607-0f96e2a33256.png" />
+        </p>
+        
         Equation of Time = (Apparent Solar Time) - (Mean Solar Time) 
         
         **Effect of Eccentricity:**
         <p align="center">
           <img src="https://user-images.githubusercontent.com/22159116/203484492-bf0f6098-fe13-44d3-b372-bcb8cc4120f8.png" />
         </p>
         
@@ -92,89 +165,21 @@
         compensate each other in winter whereas the negative value in summer begins to dominate." (Müller, 1995)
         
         Equation of Time is the combination of the effect of eccentricity and obliquity
         <p align="center">
           <img src="https://user-images.githubusercontent.com/22159116/203484851-c96be35a-2d4a-44df-a2ee-a9d88974aa9e.png" />
         </p>
         
-        To calculate the difference in time for an individual day:
-        <p align="center">
-          <img src="https://user-images.githubusercontent.com/22159116/203877814-c2d710f3-0681-4f72-8607-0f96e2a33256.png" />
-        </p>
-        
-        ## Documentation
-        **calculateDifferenceEOTMinutes**
-        Calculate the difference in time (in minutes) based on orbital period, eccentricity, and obliquity. Returns a list of differences in time for each day in the orbital year
-        ```
-        calculateDifferenceEOTMinutes(eccentricity=None,
-        				obliquity_deg=None,
-        				orbit_period=None)
-        ```
-        Returns a dictionary for the difference in time for each day in a year {day: time difference}
-        
-        **plotEOT**
-        Plot the differences in time for the EOT as well as the individual effect of obliquity and eccentricity
-        ```
-        plotEOT(planet_name=None,
-        	eot_dict={},
-        	effect_title_str=None,
-        	plot_title=None,
-        	plot_x_title=None,
-        	plot_y_title=None,
-        	showPlot=True,
-        	fig_plot_color="C0",
-        	figsize_n=12,
-        	figsize_dpi=100,
-        	save_plot_name=None)
-        ```
-        ## Dependencies
-        Python 3.7+
-        ```
-        pip3 install -r requirements.txt
-        ```
-        ## Install
-        PyPi pip install at [pypi.org/project/muller-eot/](https://pypi.org/project/muller-eot/)
-        
-        ```
-        pip install muller-eot
-        ```
-        ## Examples
-        
-        Get a list of differences in time for each day of the Earth's orbit and then plot it as a function of days in orbit
-        
-        ```
-        import muller_eot
-        
-        # Get a list of time differences for each day
-        eot_combined_dict = muller_eot.calculateDifferenceEOTMinutes(eccentricity=0.0167,
-        							obliquity_deg=23.45,
-        							orbit_period=365.25)
-        
-        # Plot differences in time as a function of days
-        muller_eot.plotEOT(planet_name="Earth",
-        		eot_dict=eot_combined_dict,
-        		effect_title_str="Eccentricity (0.0167) and Obliquity (23.45)")
-        ```
-        ![effect_eot](https://raw.githubusercontent.com/cyschneck/Muller-EOT/main/examples/earth_eot_testing.png)
-        
-        ## Tests
-        
-        TODO
-        
-        ## TODO:
-        
-        calculateOrbitalPeriod(semimajor_axis) function
-        
-        calculateDistanceBetweenSolisticePerhelion() function
-        
-        calculatePerihelionDay() function
-        
-        calculateWinterSolsticeDay() function
-        
-        calculateEccentricity() function
+        ### TODO:
+        - Pytests
+        - calculateOrbitalPeriod(semimajor_axis)
+        - calculateDistanceBetweenSolisticePerhelion()
+        - calculatePerihelionDay()
+        - calculateWinterSolsticeDay()
+        - calculateEccentricity()
         
 Keywords: astronomy,python,eot,equation of time,eccentricity,obliquity,orbital dynamics
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `muller-eot-1.3.2/setup.py` & `muller-eot-1.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="1.3.2"
+VERSION="1.4.2"
 DESCRIPTION="A Python package for M. Müller implementation of the 'Equation of Time - Problem in Astronomy' to calculate EOT and the effect of eccentricity/obliquity"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="muller-eot",
 	version=VERSION,
 	description=DESCRIPTION,
 	long_description=long_description_readme,
 	long_description_content_type='text/markdown',
 	url="https://github.com/cyschneck/Muller-EOT",
 	download_url="https://github.com/cyschneck/Muller-EOT/archive/refs/tags/v{0}.tar.gz".format(VERSION),
-	author="cyschneck (C. Y. Schneck)",
+	author="Cora Schneck (cyschneck)",
 	keywords=["astronomy", "python", "eot", "equation of time", "eccentricity", "obliquity", "orbital dynamics"],
 	license="MIT",
 	classifiers=[
 		"Development Status :: 4 - Beta",
 		"Intended Audience :: Developers",
 		"Intended Audience :: Education",
 		"Intended Audience :: Science/Research",
```

