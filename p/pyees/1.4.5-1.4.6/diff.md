# Comparing `tmp/pyees-1.4.5.tar.gz` & `tmp/pyees-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.4.5.tar", last modified: Fri Jul 21 11:21:45 2023, max compression
+gzip compressed data, was "pyees-1.4.6.tar", last modified: Tue Jul 25 18:04:40 2023, max compression
```

## Comparing `pyees-1.4.5.tar` & `pyees-1.4.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 11:21:45.316561 pyees-1.4.5/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.5/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-07-21 11:21:45.322544 pyees-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 11:21:45.125074 pyees-1.4.5/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.5/pyees/__init__.py
--rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.5/pyees/fit.py
--rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.5/pyees/profileFit.py
--rw-rw-rw-   0        0        0      812 2023-07-21 11:13:10.000000 pyees-1.4.5/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.5/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.5/pyees/sheet.py
--rw-rw-rw-   0        0        0    10180 2023-07-21 06:44:16.000000 pyees-1.4.5/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.5/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7387 2023-07-17 06:54:59.000000 pyees-1.4.5/pyees/testFit.py
--rw-rw-rw-   0        0        0    13364 2023-07-21 06:43:40.000000 pyees-1.4.5/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-07-21 10:48:22.000000 pyees-1.4.5/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.5/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.5/pyees/testSolve.py
--rw-rw-rw-   0        0        0    10768 2023-07-21 11:19:40.000000 pyees-1.4.5/pyees/testUnit.py
--rw-rw-rw-   0        0        0    84469 2023-07-21 08:40:30.000000 pyees-1.4.5/pyees/testVariable.py
--rw-rw-rw-   0        0        0    37325 2023-07-21 11:18:44.000000 pyees-1.4.5/pyees/unit.py
--rw-rw-rw-   0        0        0    36151 2023-07-21 09:10:18.000000 pyees-1.4.5/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-07-21 11:21:45.294620 pyees-1.4.5/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-21 11:21:44.000000 pyees-1.4.5/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-07-21 11:21:44.000000 pyees-1.4.5/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 11:21:44.000000 pyees-1.4.5/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-21 11:21:44.000000 pyees-1.4.5/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-21 11:21:44.000000 pyees-1.4.5/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-21 11:21:45.350469 pyees-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-07-21 11:21:38.000000 pyees-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:04:40.859134 pyees-1.4.6/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-07-25 18:04:40.864120 pyees-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 18:04:40.678614 pyees-1.4.6/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.6/pyees/__init__.py
+-rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.6/pyees/fit.py
+-rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.6/pyees/profileFit.py
+-rw-rw-rw-   0        0        0      818 2023-07-24 09:58:21.000000 pyees-1.4.6/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.6/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.6/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10180 2023-07-21 06:44:16.000000 pyees-1.4.6/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.6/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7387 2023-07-17 06:54:59.000000 pyees-1.4.6/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13344 2023-07-25 17:57:15.000000 pyees-1.4.6/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-07-25 13:15:40.000000 pyees-1.4.6/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.6/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.6/pyees/testSolve.py
+-rw-rw-rw-   0        0        0    10768 2023-07-21 11:19:40.000000 pyees-1.4.6/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    84469 2023-07-21 08:40:30.000000 pyees-1.4.6/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    39220 2023-07-25 18:03:03.000000 pyees-1.4.6/pyees/unit.py
+-rw-rw-rw-   0        0        0    35531 2023-07-25 17:53:28.000000 pyees-1.4.6/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:04:40.838190 pyees-1.4.6/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-25 18:04:39.000000 pyees-1.4.6/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-07-25 18:04:39.000000 pyees-1.4.6/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:04:39.000000 pyees-1.4.6/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-25 18:04:39.000000 pyees-1.4.6/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-25 18:04:39.000000 pyees-1.4.6/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-25 18:04:40.891048 pyees-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-07-25 18:04:33.000000 pyees-1.4.6/setup.py
```

### Comparing `pyees-1.4.5/LICENSE.txt` & `pyees-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/PKG-INFO` & `pyees-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.5
+Version: 1.4.6
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.5/README.md` & `pyees-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/fit.py` & `pyees-1.4.6/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/profileFit.py` & `pyees-1.4.6/pyees/profileFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/profilePyees.py` & `pyees-1.4.6/pyees/profilePyees.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,25 +5,24 @@
     from variable import variable
 except ImportError:
     from pyees.variable import variable
     
 pr = cProfile.Profile()
 pr.enable()
 
-for _ in range(50_000):
-
+for _ in range(50_000):    
     c = variable(4.182, 'J/kg-K', 0.130)
     rho = variable(1000, 'kg/m3', 0.01)
     t_in = variable(50, 'C', 1.2)
     t_out = variable([10, 15, 20, 25, 30, 35, 40], 'C', [0.9, 1.1, 1.0, 0.8, 0.9, 1.3, 1.1])
     v_dot = variable(300, 'L/min', 3)
     air_speed = variable([6.5, 6, 5.5, 5, 4.5, 4, 3.5], 'm/s', [0.1, 0.15, 0.12, 0.13, 0.9, 1.1, 1.0])
     q = c * rho * v_dot * (t_in - t_out)
     q.convert('kW')
-
+    
 pr.disable()
 s = io.StringIO()
 ps = pstats.Stats(pr, stream=s).sort_stats('tottime')
 ps.print_stats()
 
 with open('profile.txt', 'w+') as f:
     f.write(s.getvalue())
```

### Comparing `pyees-1.4.5/pyees/prop.py` & `pyees-1.4.6/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/sheet.py` & `pyees-1.4.6/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/solve.py` & `pyees-1.4.6/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/stackOverflowODR.py` & `pyees-1.4.6/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/testFit.py` & `pyees-1.4.6/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/testProp.py` & `pyees-1.4.6/pyees/testProp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import unittest
-import numpy as np
 import openpyxl
 try:
     from prop import prop
     from variable import variable
 except ImportError:
     from pyees.prop import prop
     from pyees.variable import variable
```

### Comparing `pyees-1.4.5/pyees/testPyees.py` & `pyees-1.4.6/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/testSheet.py` & `pyees-1.4.6/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/testSolve.py` & `pyees-1.4.6/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/testUnit.py` & `pyees-1.4.6/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/testVariable.py` & `pyees-1.4.6/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.5/pyees/unit.py` & `pyees-1.4.6/pyees/unit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 import numpy as np
 from fractions import Fraction
 
-
 class _unitConversion():
     def __init__(self, scale, offset=0) -> None:
         self.scale, self.offset = scale, offset
      
     @staticmethod
     def staticMul(selfScale, selfOffset, otherScale, otherOffset = 0):
         scale = selfScale * otherScale
         offset = selfScale * otherOffset + selfOffset
         return scale, offset
     
     @staticmethod
     def staticPow(scale, offset, pow):
         if pow == 1: return scale, offset
-                
-        pos = pow > 0
-        scale, offset = (scale, offset) * pos + _unitConversion.staticTruediv(1,0,scale, offset) * (not pos)
-        pow = pow * pos - pow * (not pos)
         
+        ## invert the scale and the offset if the power is negative
+        positivePower = pow > 0
+        if not positivePower:
+            scale, offset = _unitConversion.staticTruediv(1,0,scale, offset) * (not positivePower)
+            pow =  - pow 
+        
+        ## raise the scale and the offset to the power
+        offset = offset * sum([scale ** (i) for i in range(pow)])
         scale = scale ** pow
-        offset = offset * sum([scale ** (pow - i) for i in range(pow)])
         return scale, offset
        
     @staticmethod
     def staticTruediv(selfScale, selfOffset, otherScale, otherOffset = 0):
         return _unitConversion.staticMul(1 / otherScale, - otherOffset / otherScale, selfScale, selfOffset)
 
     def convert(self, value, useOffset=True):
         return self.scale * value + useOffset * self.offset
 
-class neperConversion():
+class _neperConversion():
             
     @staticmethod
     def convertToSignal(var):
         var._uncert = 2*np.exp(2*var.value) * var.uncert
         var._uncertSI = 2*np.exp(2*var.value) * var._uncertSI
         var._value = np.exp(2*var.value)
         
     @staticmethod
     def convertFromSignal(var):
         var._uncert = 1 / (2*var.value) * var.uncert
         var._uncertSI = 1 / (2*var.value) * var._uncertSI
         var._value = 1/2 * np.log(var.value)
 
-class bellConversion():
+class _bellConversion():
         
     @staticmethod
     def convertToSignal(var):
         var._uncert = 10**var.value * np.log(10) * var.uncert
         var._uncertSI = 10**var.value * np.log(10) * var._uncertSI
         var._value = 10**var.value
         
     @staticmethod
     def convertFromSignal(var):
         var._uncert = 1 / (var.value * np.log(10)) * var.uncert
         var._uncertSI = 1 / (var.value * np.log(10)) * var._uncertSI
         var._value = np.log10(var.value)
 
-class octaveConversion():
+class _octaveConversion():
         
     @staticmethod
     def convertToSignal(var):
         var._uncert = 2**var.value * np.log(2) * var.uncert
         var._uncertSI = 2**var.value * np.log(2) * var._uncertSI
         var._value = 2**var.value
         
@@ -71,144 +73,152 @@
     def convertFromSignal(var):
         var._uncert = 1 / (var.value * np.log(2)) * var.uncert
         var._uncertSI = 1 / (var.value * np.log(2)) * var._uncertSI
         var._value = np.log2(var.value)
 
     
     
-baseUnit = {
+_baseUnit = {
     '1': (1,0),
     '': (1,0),
     '%': (1e-2,0)
 }
 
-force = {
+_force = {
     'N': (1,0)
 }
 
-mass = {
+_mass = {
     'g': (1 / 1000,0)
 }
 
-energy = {
+_energy = {
     'J': (1,0),
 }
 
-power = {
+_power = {
     'W': (1,0)
 }
 
-pressure = {
+_pressure = {
     'Pa': (1,0),
     'bar': (1e5,0)
 }
 
-temperature = {
+_temperature = {
     'K': (1,0),
     'C': (1, 273.15),
     'F': (5 / 9, 273.15 - 32 * 5 / 9)
 }
 
-temperatureDifference = {
+_temperatureDifference = {
     'DELTAK': (1,0),
     'DELTAC': (1,0),
     'DELTAF': (5 / 9,0)
 }
 
-time = {
+_time = {
     's': (1,0),
     'min': (60,0),
     'h': (60 * 60,0),
     'yr': (60 * 60 * 24 * 365,0)
 }
 
-volume = {
+_volume = {
     'm3': (1,0),
     'L': (1 / 1000,0)
 }
 
-length = {
+_length = {
     'm': (1,0),
     'Å': (1e-10,0),
     'ly': (9460730472580800,0)
 }
 
-angle = {
+_angle = {
     'rad': (1,0),
     'deg': (np.pi / 180,0)
 }
 
-current = {
+_current = {
     'A': (1,0)
 }
 
-voltage = {
+_voltage = {
     'V': (1,0)
 }
 
-frequency = {
+_frequency = {
     'Hz': (1,0)
 }
 
-resistance = {
+_resistance = {
     'ohm': (1,0)
 }
 
-kinematicViscosity = {
+_kinematicViscosity = {
     'St': (1e-4,0)
 }
 
-logrithmicUnits = {
+_logrithmicUnits = {
     'Np' : (1,0),
     'B': (1,0),
     'oct': (1,0),
     'dec': (1,0)
 }
 
-def siUnitForce():                      return {'g':{'k':1}, 'm':{'':1}, 's':{'':-2}} 
-def siUnitPressure():                   return {'g':{'k':1}, 'm':{'':-1}, 's':{'':-2}}
-def siUnitTime():                       return {'s':{'':1}}
-def siUnitTemperature():                return {'K':{'':1}}
-def siUnitVolume():                     return {'m':{'':3}}
-def siUnitLength():                     return {'m':{'':1}}
-def siUnitEnergy():                     return {'g':{'k':1}, 'm':{'':2}, 's':{'':-2}}
-def siUnitPower():                      return {'g':{'k':1}, 'm':{'':2}, 's':{'':-3}}
-def siUnitMass():                       return {'g':{'k':1}}
-def siUnitCurrent():                    return {'A':{'':1}}
-def siUnitVoltage():                    return {'g':{'k':1}, 'm':{'':2}, 's':{'':-3}, 'A':{'':-1}}
-def siUnitBaseUnit():                   return {'1':{'':1}}
-def siUnitFreqeuncy():                  return {'s':{'':-1}}
-def siUnitAngle():                      return {'rad':{'':1}}
-def siUnitResistance():                 return {'g':{'k':1}, 'm':{'':2}, 's':{'':-3}, 'A':{'':-2}}
-def siUnitKinematicViscosity():         return {'m':{'':2},'s':{'':-1}}
-def siUnitLogarithmicUnit():            return {'Np':{'':1}}
-def siUnitTemperatureDifference():      return {'DELTAK':{'':1}}
-
-knownUnitsDict = {
-    siUnitForce:                        force,
-    siUnitPressure:                     pressure,
-    siUnitTime:                         time,
-    siUnitTemperature:                  temperature,
-    siUnitVolume:                       volume,
-    siUnitLength:                       length,
-    siUnitEnergy :                      energy,
-    siUnitPower :                       power,
-    siUnitMass:                         mass,
-    siUnitCurrent:                      current,
-    siUnitVoltage :                     voltage,
-    siUnitBaseUnit:                     baseUnit,
-    siUnitFreqeuncy:                    frequency,
-    siUnitAngle:                        angle,
-    siUnitResistance:                   resistance,
-    siUnitKinematicViscosity:           kinematicViscosity,
-    siUnitLogarithmicUnit:              logrithmicUnits,
-    siUnitTemperatureDifference:        temperatureDifference
+
+## Create a dictionary of all the si base units of each different type of measurement
+## the value of this dictionary is the dictionary representation of the si units
+_SIBaseUnits = {
+    'Force'                     : {'g':{'k':1}, 'm':{'':1}, 's':{'':-2}}, 
+    'Pressure'                  : {'g':{'k':1}, 'm':{'':-1}, 's':{'':-2}},
+    'Time'                      : {'s':{'':1}},
+    'Temperature'               : {'K':{'':1}},
+    'Volume'                    : {'m':{'':3}},
+    'Length'                    : {'m':{'':1}},
+    'Energy'                    : {'g':{'k':1}, 'm':{'':2}, 's':{'':-2}},
+    'Power'                     : {'g':{'k':1}, 'm':{'':2}, 's':{'':-3}},
+    'Mass'                      : {'g':{'k':1}},
+    'Current'                   : {'A':{'':1}},
+    'Voltage'                   : {'g':{'k':1}, 'm':{'':2}, 's':{'':-3}, 'A':{'':-1}},
+    'BaseUnit'                  : {'1':{'':1}},
+    'Freqeuncy'                 : {'s':{'':-1}},
+    'Angle'                     : {'rad':{'':1}},
+    'Resistance'                : {'g':{'k':1}, 'm':{'':2}, 's':{'':-3}, 'A':{'':-2}},
+    'KinematicViscosity'        : {'m':{'':2},'s':{'':-1}},
+    'LogarithmicUnit'           : {'Np':{'':1}},
+    'TemperatureDifference'     : {'DELTAK':{'':1}},
+}
+
+## create a dictionary of all units for each type of measurement.
+## the values of this dictionary is itself a dictionary of (string, conversion) pairs
+_knownUnitsDict = {
+    'Force':                        _force,
+    'Pressure':                     _pressure,
+    'Time':                         _time,
+    'Temperature':                  _temperature,
+    'Volume':                       _volume,
+    'Length':                       _length,
+    'Energy' :                      _energy,
+    'Power' :                       _power,
+    'Mass':                         _mass,
+    'Current':                      _current,
+    'Voltage' :                     _voltage,
+    'BaseUnit':                     _baseUnit,
+    'Freqeuncy':                    _frequency,
+    'Angle':                        _angle,
+    'Resistance':                   _resistance,
+    'KinematicViscosity':           _kinematicViscosity,
+    'LogarithmicUnit':              _logrithmicUnits,
+    'TemperatureDifference':        _temperatureDifference
 }
 
-knownPrefixes = {
+## create a dictionary of the known prefixes
+_knownPrefixes = {
     'T':10**12,
     'G':10**9,
     'M':10**6,
     'k':10**3,
     'h':10**2,
     'da':10**1,
     '': 1,
@@ -216,108 +226,140 @@
     'c':10**-2,
     'm':10**-3,
     'mu':10**-6,
     'n':10**-9,
     'p':10**-12
 }
 
-
-knownUnits = {}
-for key, d in knownUnitsDict.items():
-    for item, _ in d.items():
-        if item not in knownUnits:
-            knownUnits[item] = [key, knownUnitsDict[key][item]]
+## create a dictionary of all known units
+## the keys of this dictionary is the stringrepresenation of the unit
+## the values is a list of two elements:
+## the first element is the dictionary representation of the corresponding si unit
+## the second element is the conversion from the unit to the corresponding si unit
+_knownUnits = {}
+for key in _SIBaseUnits.keys():
+    sibaseunit = _SIBaseUnits[key]
+    for kkey, conversion in _knownUnitsDict[key].items():
+        if kkey not in _knownUnits:
+            _knownUnits[kkey] = [sibaseunit, conversion]
         else:
-            raise Warning(f'The unit {item} known in more than one unit system')
+            raise Warning(f'The unit {kkey} is known in more than one unit system')
+    
 
 
 # determine the known characters within the unit system
-knownCharacters = list(knownUnits.keys()) + list(knownPrefixes.keys())
-knownCharacters = ''.join(knownCharacters)
-knownCharacters += '-/ '
-knownCharacters += '0123456789'
-knownCharacters += '()'
-knownCharacters = set(knownCharacters)
+_knownCharacters = list(_knownUnits.keys()) + list(_knownPrefixes.keys())
+_knownCharacters = ''.join(_knownCharacters)
+_knownCharacters += '-/ '
+_knownCharacters += '0123456789'
+_knownCharacters += '()'
+_knownCharacters = set(_knownCharacters)
 
 # check if all unit and prefix combinations can be distiguished
-unitPrefixCombinations = []
-for u in knownUnits:
-    unitPrefixCombinations += [u]
-    if u not in baseUnit or u == "%":
-        for p in knownPrefixes:
+_unitPrefixCombinations = []
+for u in _knownUnits:
+    _unitPrefixCombinations += [u]
+    if u not in _baseUnit or u == "%":
+        for p in _knownPrefixes:
             if p == '':continue
+            _unitPrefixCombinations.append(p+u)
+
+
+
+
+def _checkForAmbiguityInTheUnits():
+    for elem in _unitPrefixCombinations:
+        count = sum([1 if u == elem else 0 for u in _unitPrefixCombinations])
+        if count > 1:
             
-            unitPrefixCombinations.append(p+u)
+            def splitPrefixAndUnit(unit):
+                
+                # The unit was not found. This must be because the unit has a prefix
+                found = False
+                
+                for p in _knownPrefixes:
+                    if p != unit[0:len(p)]: continue
+                    u = unit[len(p):]
+                    if not u in _knownUnits: continue
+                    found = True
+                    prefix, unit = p,u
+                    break 
+
+                if not found:
+                    raise ValueError(f'The unit ({unit}) was not found. Therefore it was interpreted as a prefix and a unit. However a combination of prefix and unit which matches {unit} was not found')
+                
+                if unit in _baseUnit and unit != "%":
+                    unit = "1"
+                    raise ValueError(f'The unit ({prefix}) was not found. Therefore it was interpreted as a prefix and a unit. The prefix was identified as "{p}" and the unit was identified as "{unit}". However, the unit "1" cannot have a prefix')
+
+                # look for the unit without the prefix
+                if not unit in _knownUnits:
+                    raise ValueError(f'The unit ({prefix}{unit}) was not found. Therefore it was interpreted as a prefix and a unit. However the unit ({unit}) was not found')
+                return unit, prefix
+
+            unit, prefix = splitPrefixAndUnit(elem)
+
+            unitType1 = ''
+            for key, item in _knownUnitsDict.items():
+                if elem in item:
+                    unitType1 = key
+            if unitType1 == '':
+                raise ValueError(f'The unit {elem} was not found.')
 
-for elem in unitPrefixCombinations:
-    count = sum([1 if u == elem else 0 for u in unitPrefixCombinations])
-    if count > 1:
-        prefix = elem[0:1]
-        unit = elem[1:]
-
-        unitType1 = ''
-        for key, item in knownUnitsDict.items():
-            if elem in item:
-                unitType1 = [key for key, a in locals().items() if a == item][0]
-        if unitType1 == '':
-            raise ValueError(f'The unit {elem} was not found.')
-
-        unitType2 = ''
-        for key, item in knownUnitsDict.items():
-            if unit in item:
-                unitType2 = [key for key, a in locals().items() if a == item][0]
-        if unitType2 == '':
-            raise ValueError(f'The unit {unit} was not found.')
+            unitType2 = ''
+            for key, item in _knownUnitsDict.items():
+                if unit in item:
+                    unitType2 = key
+            if unitType2 == '':
+                raise ValueError(f'The unit {unit} was not found.')
+
+            raise ValueError(f'The unit {elem} can be interpreted as a {unitType1} ({elem}) or a {unitType2} in the unit "{unit}" with the prefix "{prefix}". This cannot be distiguished.')
 
-        raise ValueError(f'The unit {elem} can be interpreted as a {unitType1} or a {unitType2} with the prefix {prefix}. The cannot be distiguished.')
 
 
 def addNewUnit(newUnit: str, scale: float, existingUnit: str, offset : float = 0):
-        
-    if newUnit in unitPrefixCombinations:
-        raise ValueError(f'The unit {newUnit} is already known within the unit system')
-    unitPrefixCombinations.append(newUnit)
-    for p in knownPrefixes:
+    
+    ## add the newUnit to the unitPrefix combinations
+    _unitPrefixCombinations.append(newUnit)
+    for p in _knownPrefixes:
         if p == '': continue
-        if p+newUnit in unitPrefixCombinations:
-            raise ValueError(f'The unit {p+newUnit} is already known within the unit system')
-        unitPrefixCombinations.append(newUnit)
+        _unitPrefixCombinations.append(p+newUnit)
 
+    ## create a unitObject from the existing unit string
+    existingUnit = unit(existingUnit)
     
-    existingUnitDict = unit._getUnitDict(existingUnit)
-    existingUnitDictSI = unit._getUnitDictSI(existingUnitDict)
-    def existingUnitDictSIMethod(): return existingUnitDictSI
-
+    ## the SI unit of the existing unit must be the same as that of the new unit
+    newUnitDictSI = existingUnit.unitDictSI
     
-    for u, item in existingUnitDict.items():
-        for pre, exp in item.items():
-            convScale, convOffset = knownUnits[u][1]
-            convScale = convScale * knownPrefixes[pre]
-            if convScale == 1 and convOffset == 0: continue
-            isUpper = exp > 0
-            if not isUpper: exp = -exp 
-            convScale, convOffset = _unitConversion.staticPow(convScale, convOffset, exp)
-            ## i have no idea why the order of the inputs has to be swapped when comparing _unitConversion.staticMul and _unitConversion.staticTruediv
-            if isUpper:
-                scale, offset = _unitConversion.staticMul(convScale, convOffset, scale, offset)
-            else:
-                scale, offset = _unitConversion.staticTruediv(scale, offset, convScale, convOffset)      
+    ## determine the scale and the offset from the new unit to the si unit using the scale and the offset from the existing unit
+    scale, offset = _unitConversion.staticMul(existingUnit._converterToSI.scale, existingUnit._converterToSI.offset, scale, offset)
+   
+    ## add the new unit to the knownUnits
+    _knownUnits[newUnit] = [newUnitDictSI, (scale, offset)]
     
-    knownUnits[newUnit] = [existingUnitDictSIMethod, (scale, offset)]
-        
-    global knownCharacters
+    ## add the newunit to the values of knownUnitsDict. This is used to check for ambiguity in the unit system
+    for item in _knownUnitsDict.values():
+        if existingUnit in item:
+            item[newUnit] = (scale,offset)
+    
+    ## add the characters of the new unit to the knownCharacters
     for s in newUnit:
-        knownCharacters.add(s)
+        _knownCharacters.add(s)
+        
+    ## check for ambiguity in the unit system
+    _checkForAmbiguityInTheUnits()
 
     
+
 hyphen = '-'
 slash = '/'
 integers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
 
 
+
 class unit():
 
     def __init__(self, unitStr = None, unitDict = None, unitDictSI = None, selfUnitStr = None, selfUnitStrSI = None, converterToSI = None):
         if unitStr is None:
             unitStr = ''
         
         if unitDict is None:
@@ -348,20 +390,20 @@
     @staticmethod
     def _getUnitStrFromDict(unitDict):
         upper, lower = [], []
         
         for u, item in unitDict.items():    
             for p, exp in item.items():
                 isUpper = exp > 0
-                if not isUpper: exp = -exp
-                if exp == 1: s = p+u
-                else: s = p+u+str(exp)
+                if not isUpper: exp = - exp
+                exp = str(exp) if exp != 1 else ''
+                s = p+u+str(exp)
                 if isUpper: upper.append(s)
                 else: lower.append(s)
-                            
+        
         out = '-'.join(upper)
         if lower: out = out + '/' + '-'.join(lower)
         return out
       
     def getUnitWithoutPrefix(self):
         
         upper, lower = [],[]
@@ -381,91 +423,92 @@
         if lower:
             out += '/' + '-'.joing(lower)
             
         return out
         
     @ staticmethod
     def _splitCompositeUnit(compositeUnit):
-        lower = []
         if not slash in compositeUnit:
             upper = compositeUnit.split(hyphen)
-            return upper, lower
+            return upper, []
     
         compositeUnit = compositeUnit.split(slash)
 
         if len(compositeUnit) > 2:
-            raise ValueError('A unit can only have a single slash (/)')
+            raise ValueError(f'A unit can only have a single slash ({slash})')
 
         upper = compositeUnit[0].split(hyphen)
-        lower = compositeUnit[1].split(hyphen) if len(compositeUnit) > 1 else []
+        lower = compositeUnit[1].split(hyphen) if len(compositeUnit) == 2 else []
 
         return upper, lower
 
     @staticmethod
     def _splitUnitExponentAndPrefix(unitStr):
         prefixUnit, exponent = unit._removeExponentFromUnit(unitStr)
         u, prefix = unit._removePrefixFromUnit(prefixUnit)
         return u, prefix, exponent
-
+   
     @staticmethod
     def _reduceDict(unitDict):
         
         ## loop over all units, and remove any prefixes, which has an exponenet of 0
         for key, item in unitDict.items():
             prefixesToRemove = []
             for pre, exp in item.items():
                 if exp == 0:  prefixesToRemove.append(pre)
             for pre in prefixesToRemove: item.pop(pre)
-    
+
         ## remove the units, which has no items in their dictionary
         keysToRemove = []
+        n = len(unitDict)
         for key, item in unitDict.items():
-            if not item: keysToRemove.append(key)
+            if not item:
+                keysToRemove.append(key)
+                n -= 1
+                
+        ## if all the keys in unitDict has to be removed, then return the unit '1'
+        if n == 0:
+            ## return '1' if there are not other units
+            return {'1': {'': 1}}
+        
+        ## remove the keys
         for key in keysToRemove: unitDict.pop(key)
         
-        ## remove the unit '1' above the fraction line, if there are any other units above the fraction line
-        if len(unitDict) > 1 and '1' in unitDict:
-            otherUpper = False
-            for key, item in unitDict.items():
-                if key == '1':
-                    continue
-                for exp in item.values():
-                    if exp > 0:
-                        otherUpper = True
-                        break
+        ## check if 1 is in the unit
+        if '1' in unitDict:
+            if n > 1:
+                ## determine if there are any other units than '1' above the fraction line
+                otherUpper = sum([sum([1 if exp > 0 else 0 for exp in item.values()]) if (key != '1') else 0 for key, item in unitDict.items()])
+                            
+                ## if there are any other upper units, then remove 1
+                ## else set the exponent of the unit '1' to 1
                 if otherUpper:
-                    break
-            if otherUpper:
-                unitDict.pop('1')
-                
-        ## return '1' if there are not other units
-        if not unitDict:
-            return {'1': {'': 1}}
+                    unitDict.pop('1')
+                    n -= 1
+                else: unitDict['1'][''] = 1
+            else:
+                unitDict['1'][''] = 1
                 
-        ## set the exponent of the unit '1' to 1
-        if '1' in unitDict:
-            unitDict['1'][''] = 1
-        
         ## make temperature units in to temperature differences, if there are any other units in the dict
-        if len(unitDict) > 1:
+        if n > 1:
             keysToChange = []
-            for key in unitDict.keys():
-                if key in temperature: keysToChange.append(key)
+            for key in _temperature.keys():
+                if key in unitDict: keysToChange.append(key)
             for key in keysToChange: 
                 unitDict['DELTA' + key] = unitDict[key]
-                unitDict.pop(key)       
+                unitDict.pop(key)
             
         return unitDict
     
     @staticmethod
     def _getUnitDictSI(unitDict):
         out = {}
         for key, item in unitDict.items():
             exp = sum(item.values())
-            unitSI = knownUnits[key][0]()
+            unitSI = _knownUnits[key][0]
             for kkey, iitem in unitSI.items():
                 if kkey in out:
                     for p,e in iitem.items():
                         e = e * exp
                         if p in out[kkey]:
                             out[kkey][p] += e
                         else:
@@ -504,15 +547,15 @@
     def _formatUnitStr(unitStr):
         
         ## remove spaces
         unitStr = unitStr.replace(' ', '')
         
         # check for any illegal symbols
         for s in unitStr:
-            if s not in knownCharacters:
+            if s not in _knownCharacters:
                 raise ValueError(f'The character {s} is not used within the unitsystem')
         
         ## return the unity        
         if unitStr is None or unitStr == '':
             return '1'
 
         ## find start parenthesis is the unit string
@@ -654,41 +697,37 @@
                 raise ValueError(f'The unit {u} was stripped of all integers which left no symbols in the unit. This is normally due to the integers removed being equal to 1, as the unit is THE unit. Howver, the intergers removed was not equal to 1. The unit is therefore not known.')
             u = '1'
         return u, exponent
 
     @staticmethod
     def _removePrefixFromUnit(unit):
         
-        if unit in knownUnits:
+        if unit in _knownUnits:
             return unit, ''
 
         # The unit was not found. This must be because the unit has a prefix
         found = False
         
-        for p in knownPrefixes.keys():
-            index = unit.find(p)
-            if index != 0:
-                continue
+        for p in _knownPrefixes:
+            if p != unit[0:len(p)]: continue
             u = unit[len(p):]
-            if not u in knownUnits:
-                continue
+            if not u in _knownUnits: continue
             found = True
             prefix, unit = p,u
-            break
-        
+            break 
 
         if not found:
             raise ValueError(f'The unit ({unit}) was not found. Therefore it was interpreted as a prefix and a unit. However a combination of prefix and unit which matches {unit} was not found')
         
-        if unit in baseUnit and unit != "%":
+        if unit in _baseUnit and unit != "%":
             unit = "1"
             raise ValueError(f'The unit ({prefix}) was not found. Therefore it was interpreted as a prefix and a unit. The prefix was identified as "{p}" and the unit was identified as "{unit}". However, the unit "1" cannot have a prefix')
 
         # look for the unit without the prefix
-        if not unit in knownUnits:
+        if not unit in _knownUnits:
             raise ValueError(f'The unit ({prefix}{unit}) was not found. Therefore it was interpreted as a prefix and a unit. However the unit ({unit}) was not found')
         return unit, prefix
 
     def __str__(self, pretty=False):
         
         if not pretty:
             return self.unitStr
@@ -713,22 +752,22 @@
         # a fraction is needed
         out = rf'\frac{{'
         out += '\cdot'.join(upper)
         out += rf'}}{{'
         out += '\cdot'.join(lower)
         out += rf'}}'
         return out
-
+    
     def __eq__(self, other):
         return self.unitDict == other.unitDict
 
     def isLogarithmicUnit(self):
         upper, lower = unit._splitCompositeUnit(self.unitStr)
         if lower or len(upper) != 1: return False
-        return unit._splitUnitExponentAndPrefix(upper[0])[0] in logrithmicUnits
+        return unit._splitUnitExponentAndPrefix(upper[0])[0] in _logrithmicUnits
 
     def __add__(self, other):
         ## determine the units of self without any prefixes and convert this to a string
         selfUnitDictWithoutPrefixes = {}
         for key, item in self.unitDict.items():
             selfUnitDictWithoutPrefixes[key] = {}
             selfUnitDictWithoutPrefixes[key][''] = 0
@@ -845,15 +884,14 @@
         
         return unit(unitDict = unitDict, converterToSI = converterToSI)
     
     def __truediv__(self, other):
         unitDict = unit.staticTruediv(self.unitDict, other.unitDict)
         converterToSI = _unitConversion(*_unitConversion.staticTruediv(self._converterToSI.scale, self._converterToSI.offset, other._converterToSI.scale, other._converterToSI.offset))
         return unit(unitDict = unitDict, converterToSI = converterToSI)
-   
     
     @staticmethod
     def staticTruediv(a, b):
        
         unitDict = {}
         for key, item in a.items():
             unitDict[key]= {}
@@ -930,16 +968,16 @@
     def getConverterToSI(self):
         # initialize the scale and offset
         outScale, outOffset = 1,0
         
         ## loop over self.unitDict
         for u, item in self.unitDict.items():
             for pre, exp in item.items():
-                convScale, convOffset = knownUnits[u][1]
-                convScale = convScale * knownPrefixes[pre]
+                convScale, convOffset = _knownUnits[u][1]
+                convScale = convScale * _knownPrefixes[pre]
                 if convScale == 1 and convOffset == 0: continue
                 convScale, convOffset = _unitConversion.staticPow(convScale, convOffset, exp)
                 outScale, outOffset = _unitConversion.staticMul(outScale, outOffset, convScale, convOffset)
      
         self._converterToSI = _unitConversion(outScale, outOffset)
 
     def getConverter(self, newUnitStr):  
@@ -953,32 +991,32 @@
             raise ValueError(f'You tried to convert from {self} to {newUnitStr}. But these do not have the same base units')
         
         outScale, outOffset = self._converterToSI.scale, self._converterToSI.offset
         
         ## loop over newUnitDict
         for u, item in newUnitDict.items():
             for pre, exp in item.items():
-                convScale, convOffset = knownUnits[u][1]
-                convScale = convScale * knownPrefixes[pre]
+                convScale, convOffset = _knownUnits[u][1]
+                convScale = convScale * _knownPrefixes[pre]
                 if convScale == 1 and convOffset == 0: continue
                 convScale, convOffset = _unitConversion.staticPow(convScale, convOffset, exp)
                 outScale, outOffset = _unitConversion.staticTruediv(outScale, outOffset, convScale, convOffset)      
             
         return _unitConversion(outScale, outOffset)
 
     def isCombinationUnit(self):
         return len(list(self.unitDict.keys())) > 1
 
     def getLogarithmicConverter(self):
         u, _ = self._removePrefixFromUnit(self.unitStr)
         
         if u == 'B':
-            return bellConversion()
+            return _bellConversion()
         if u == 'Np':
-            return neperConversion()
+            return _neperConversion()
         if u == 'oct':
-            return octaveConversion()
-        return bellConversion()
+            return _octaveConversion()
+        return _bellConversion()
 
+    def __hash__(self):
+        return id(self)
 
-    
-
```

### Comparing `pyees-1.4.5/pyees/variable.py` & `pyees-1.4.6/pyees/variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from copy import copy
+
 import numpy as np
 try:
     from unit import unit
 except ImportError:
     from pyees.unit import unit
      
     
@@ -94,26 +94,23 @@
     def __init__(self, value, unitObject : str | unit, uncert, nDigits) -> None:
         
         self._value = value
         self._uncert = uncert
 
         # create a unit object
         self._unitObject = unitObject if isinstance(unitObject, unit) else unit(unitObject)
-        self._uncertSI = self._unitObject._converterToSI.convert(self._uncert, useOffset=False)
+        self._uncertSI = self.uncert * self._unitObject._converterToSI.scale
 
         # number of digits to show
         self.nDigits = nDigits
 
         # uncertanty
         self.dependsOn = {}
         self.covariance = {}
 
-    @property
-    def _converterToSI(self):
-        return self._unitObject._converterToSI
 
     @property
     def value(self):
         return self._value
 
     @property
     def unit(self):
@@ -122,15 +119,15 @@
     @property
     def uncert(self):
         return self._uncert
 
     def convert(self, newUnit):
         converter = self._unitObject.getConverter(newUnit)
         self._value = converter.convert(self._value, useOffset=not self._unitObject.isCombinationUnit())
-        self._uncert = converter.convert(self._uncert, useOffset=False)
+        self._uncert = self._uncert * converter.scale
         self._unitObject = unit(newUnit)
  
     def printUncertanty(self, value, uncert):
         # function to print number
         if uncert == 0 or uncert is None or np.isnan(uncert):
             return f'{value:.{self.nDigits}g}', None
 
@@ -195,15 +192,15 @@
             return rf'{value}{space}{unitStr}'
         else:
                 return rf'{value} {pm} {uncert}{space}{unitStr}'
 
     def _addDependent(self, var, grad):
                                 
         # scale the gradient to SI units. This is necessary if one of the variables are converted after the dependency has been noted
-        grad *= self._converterToSI.convert(1, useOffset=False) / var._converterToSI.convert(1, useOffset=False)
+        grad *= self._unitObject._converterToSI.scale / var._unitObject._converterToSI.scale
         self.__addDependent(var, grad)
         
     def __addDependent(self, var, grad):
         
         if not var.dependsOn:
             ## the variable does not depend on other variables
             ## add the variable to the dependencies of self
@@ -245,55 +242,55 @@
             raise ValueError(f'You tried to set the covariance between {self} and {var} with a non scalar value')
         
         covUnit = unit(unitStr)
         selfVarUnit = self._unitObject * var._unitObject
         if not covUnit.unitDictSI ==  selfVarUnit.unitDictSI:
             raise ValueError(f'The covariance of {covariance} [{unitStr}] does not match the units of {self} and {var}')
         
-        covariance = covUnit._converterToSI.convert(covariance, useOffset=False)
+        covariance = covariance * covUnit._converterToSI.scale
         
         self.covariance[var] = covariance        
         var.covariance[self] = covariance
         
     def _calculateUncertanty(self):
         
         variance = 0
         for var, grad in self.dependsOn.items():
             ## variance from the measurements     
             variance += (var._uncertSI * grad)**2
-           
+        
             # variance from the corralation between measurements
             ## covariance = dict(var: covariance)
             ## the gradients can be found in self.dependsOn
             ## loop over all variables that are in var.covariance and also self.dependsOn
             if not var.covariance: continue
             for var2 in filter(lambda x: x in self.dependsOn, var.covariance):
                 variance += grad * self.dependsOn[var2] * var.covariance[var2]
         
         ## all variances are determined in the SI unit system.
         ## these has to be converted back in the the unit of self
         self._uncertSI = np.sqrt(variance)
-        self._uncert = self._uncertSI / self._converterToSI.convert(1, useOffset=False)
+        self._uncert = self._uncertSI / self._unitObject._converterToSI.scale
         
     def __add__(self, other):
         
         if not isinstance(other, scalarVariable):
             return self + variable(other, self.unit)
 
         # determine if the two variable can be added
         outputUnit = self._unitObject + other._unitObject
         
         ## handle logarithmic addition seperately
         if outputUnit.isLogarithmicUnit():
             return logarithmicVariables.__add__(self, other)
 
         # convert self and other
-        selfUnit = copy(self._unitObject)
-        otherUnit = copy(other._unitObject)
-        
+        selfUnit = self._unitObject
+        otherUnit = other._unitObject
+    
         ## convert the units if the SI unit is identical to that of the output unit and the unit is not equal to the output unit
         if self._unitObject.unitDictSI == outputUnit.unitDictSI and not self._unitObject == outputUnit:
             self.convert(str(outputUnit))
         if other._unitObject.unitDictSI == outputUnit.unitDictSI and not other._unitObject == outputUnit:
             other.convert(str(outputUnit))
 
         # determine the value
@@ -334,16 +331,16 @@
         outputUnit = self._unitObject - other._unitObject
     
         ## handle logarithmic unit seperately
         if outputUnit.isLogarithmicUnit():
             return logarithmicVariables.__sub__(self, other)
         
         # convert self and other
-        selfUnit = copy(self._unitObject)
-        otherUnit = copy(other._unitObject)
+        selfUnit = self._unitObject
+        otherUnit = other._unitObject
         
         ## convert the units if the SI unit is identical to that of the output unit and the unit is not equal to the output unit
         if self._unitObject.unitDictSI == outputUnit.unitDictSI and not self._unitObject == outputUnit:
             self.convert(str(outputUnit))
         if other._unitObject.unitDictSI == outputUnit.unitDictSI and not other._unitObject == outputUnit:
             other.convert(str(outputUnit))
        
@@ -413,15 +410,15 @@
         ## determine the output unit
         outputUnit = self._unitObject ** other.value
         
         ## if self._unitObject has the same keys, as the output unit
         ## then self does not have to be scaled to the SI unit system in order for the unit to be raised to the power
         hasToBeScaledToSI = self._unitObject.unitDict.keys() != outputUnit.unitDict.keys()
         if hasToBeScaledToSI:
-            selfUnit = copy(self.unit)
+            selfUnit = self.unit
             self.convert(self._unitObject.unitStrSI)
         
         ## dertermine the value
         val = self.value ** other.value
 
         ## determine the gradients of the output with respoect to self and other
         def gradSelf(valSelf, valOTher):
@@ -614,16 +611,16 @@
             
             if a.unit == b.unit:
                 return func(a,b)
             
             if not a._unitObject.unitDictSI == b._unitObject.unitDictSI:
                 raise ValueError(f'You cannot compare {a} and {b} as they do not have the same SI base unit')
         
-            aUnit = copy(a.unit)
-            bUnit = copy(b.unit)
+            aUnit = a.unit
+            bUnit = b.unit
             
             a.convert(a._unitObject.unitStrSI)
             b.convert(b._unitObject.unitStrSI)
             
             res = func(a,b)
             
             a.convert(aUnit)
@@ -737,15 +734,15 @@
         for elem, varElem, gradElem in zip(self.scalarVariables, var, grad):
             elem.addCovariance(varElem, gradElem, unitStr)
     
     def _addDependent(self, var, grad):
         isArrayVariable = isinstance(var, arrayVariable)
         isArrayGradient = isinstance(grad, list) or isinstance(grad, np.ndarray)
         
-        grad *= self._converterToSI.convert(1, useOffset=False) / var._converterToSI.convert(1, useOffset=False)
+        grad *= self._unitObject._converterToSI.scale / var._unitObject._converterToSI.scale
         
         for i, elem in enumerate(self.scalarVariables):
             v = var[i] if isArrayVariable else var
             g = grad[i] if isArrayGradient else grad
             elem._scalarVariable__addDependent(v, g)
                         
     def __len__(self):
@@ -999,17 +996,7 @@
                 raise ValueError('The lenght of the value has to be equal to the lenght of the uncertanty')      
     
     if isinstance(value, np.ndarray):
         return arrayVariable(value = value, unitStr = unit, uncert = uncert, nDigits = nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
 
-    
-if __name__ == "__main__":
-    a = variable(11,'dB', 0.1)
-    b = variable(19,'dB', 1.2)
-    print(a._uncertSI)
-    print(b._uncertSI)
-    c = a + b
-    gradA = (10**(11/10)) / (10**(19/10) + 10**(11/10))
-    gradB = (10**(19/10)) / (10**(19/10) + 10**(11/10))
-    print(c.uncert, np.sqrt( (gradA * a.uncert)**2 + (gradB * b.uncert)**2))
```

### Comparing `pyees-1.4.5/pyees.egg-info/PKG-INFO` & `pyees-1.4.6/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.5
+Version: 1.4.6
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.5/setup.py` & `pyees-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.4.5',
+    version='1.4.6',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

