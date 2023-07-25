# Comparing `tmp/simple_minimizer-1.1.0.tar.gz` & `tmp/simple_minimizer-2.0.0.tar.gz`

## Comparing `simple_minimizer-1.1.0.tar` & `simple_minimizer-2.0.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/make_project.sh
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/src/simple_minimizer/__init__.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/src/simple_minimizer/logistic_constraints.py
--rwxr-xr-x   0        0        0    13572 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/src/simple_minimizer/minimizer.py
--rwxr-xr-x   0        0        0     1843 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/src/simple_minimizer/vertex.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/LICENSE
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 simple_minimizer-1.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/make_project.sh
+-rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/upload_project.sh
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/src/simple_minimizer/__init__.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/src/simple_minimizer/logistic_constraints.py
+-rwxr-xr-x   0        0        0    15765 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/src/simple_minimizer/minimizer.py
+-rwxr-xr-x   0        0        0     1835 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/src/simple_minimizer/vertex.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/src/tests/test1.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 simple_minimizer-2.0.0/PKG-INFO
```

### Comparing `simple_minimizer-1.1.0/src/simple_minimizer/logistic_constraints.py` & `simple_minimizer-2.0.0/src/simple_minimizer/logistic_constraints.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     def __init__(self, fLevel, fScale = 1):
         self.fLevel = fLevel # value to stay above
         self.fScale = fScale
         if fLevel != 0:
             self.fScale = abs(fLevel)
         self.fL = 4*self.fScale # leading factor
         self.fThreshold = fLevel+2*self.fScale # point where constraint kicks in
-        print(self.fLevel, self.fScale, self.fThreshold)
 
     def __call__(self, fX):
         if fX < self.fThreshold:
             fX = (fX-self.fLevel)/self.fScale - 2
             try:
                 fX = self.fLevel+self.fL/(1+math.exp(-fX))
             except OverflowError as e:
@@ -27,15 +26,14 @@
     def __init__(self, fLevel, fScale = 1):
         self.fLevel = fLevel # value to stay above
         self.fScale = fScale
         if fLevel != 0:
             self.fScale = abs(fLevel)
         self.fL = 4*self.fScale # leading factor
         self.fThreshold = fLevel-2*self.fScale # point where constraint kicks in
-        print(self.fLevel, self.fScale, self.fThreshold)
 
     def __call__(self, fX):
         if fX > self.fThreshold:
             fX = (fX-self.fLevel)/self.fScale + 2
             try:
                 fX = self.fLevel-self.fL/(1+math.exp(fX))
             except OverflowError as e:
```

### Comparing `simple_minimizer-1.1.0/src/simple_minimizer/minimizer.py` & `simple_minimizer-2.0.0/src/simple_minimizer/minimizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,41 @@
 import copy
 from math import sqrt
 import random
 
 mapConvergenceReasons = {-1: "Exceeded iteration limit", 1: "Closest points indistinguishable", 
                                                 2: "Met fractional tolerance", 3:"Minimum scale achieved"}
 
+class SimpleMinimum:
+    
+    def __init__(self, nAxis, lowerVertex, middleVertex, upperVertex):
+        self.nAxis = nAxis
+        self.lowerVertex = lowerVertex
+        self.middleVertex = middleVertex
+        self.upperVertex = upperVertex
+        self.fDepth = 0.5*(lowerVertex.fValue+upperVertex.fValue)-middleVertex.fValue
+    
+    def __lt__(self, other):
+        return self.fDepth < other.fDepth
+        
+    def __str__(self):
+        return self.__repr()
+
+    def __repr__(self):
+        return " ".join(map(str, (self.nAxis, self.middleVertex, self.fDepth)))
+
 """ Simple minimizer class applies a simple sequential axial minimization.
 It does a simple bracketing followed by a parabolic interpolation to 
 the minimum along each axis in sequence, repeating with reduced scale
 until the scale is small.  This is a crude but extremely effective way 
 of decoupling parameters during registration.  If you have an objective
 function that goes negative, add a constant to it that is sufficient to
 get the minimum around +1.
 """
-class SimpleMinimizer(object):
+class SimpleMinimizer:
     
     # Constructor sets dimensions of arrays
     def __init__(self, nDimension):
         
         # The dimension of the space we are working in
         self.nDimension = nDimension
 
@@ -139,21 +157,79 @@
     def getMinimum(self):
         return self.lstHistory[-1].getVertex()
 
     # Get reason for convergence
     def getConvergenceReason(self, nReason):
         return mapConvergenceReasons[nReason]
 
+    def adaptiveMinimize(self, lstStart = None):
+        """This is still an axial minimizer, but it figures out the order of
+        the axes to minimize along rather than requiring the user to do it.
+        As always, efficiency is not an option."""
+        if lstStart:
+            self.setStarts(lstStart)
+        
+        self.fBest = 1.e8;   # not close to any likely value
+
+        # evaluate starting point
+        nCount = 0
+        self.lstHistory[-1].setValue(self.pObjective(self.lstHistory[-1].getVertex()))
+
+        # generate collection of minima along each axis
+        while True:
+            self.fSecondBest = self.fBest;    # record old best value
+            lstMinima = []
+            lstStart = self.lstHistory[-1]
+            for nAxis in range(self.nDimension):            
+                lower = EmptyVertex(self.nDimension)
+                middle = EmptyVertex(self.nDimension)
+                CopyVertex(middle, lstStart)
+                upper = EmptyVertex(self.nDimension)
+                bFound = self.bracket(nAxis,lower,middle,upper)
+                if bFound:
+                    lstMinima.append(SimpleMinimum(nAxis, lower, middle, upper))
+                # skip axis of not able to bracket
+            
+            lstMinima.sort()
+            lstMinima.reverse()
+            for pMinimum in lstMinima:
+                nAxis = pMinimum.nAxis
+                self.fBest = self.parabolic(nAxis, pMinimum.lowerVertex, pMinimum.middleVertex, pMinimum.upperVertex)        
+
+            self.fRadialScale *= 0.3183098861; # ~1/pi (any ~irrational will do)
+            nCount += 1
+            if self.nMaxIterations < nCount:   # bail out if we are stuck
+                nReason = -1
+                break;
+                
+            # Various reasons for quiting:
+            if (self.fBest+self.fSecondBest) == 0:
+                nReason = 1
+                break
+            elif (abs(self.fBest-self.fSecondBest)/(self.fBest+self.fSecondBest) <= self.fFractionalTolerance):
+                nReason = 2
+                break
+            elif (self.fRadialScale <= self.fMinimumScale):
+                nReason = 3
+                break
+
+        return (nCount, self.lstHistory[-1], nReason);
+
     # Axial minimization
     def minimize(self, lstStart = None):
         """
         Minimize by minimizations along successive axes.  This is the same
         techinque used in the original pseudo-correlation work, and it has the
         advantage of decoupling the rotation from the translation as much as
-        possible.
+        possible. This is really intended for "anatomical" cases where there are
+        well-defined axes that are largely independent of each other. The ordering
+        of axial minimizations can be controlled using lstOrder, and the 
+        system still works pretty well for cases where the axes aren't all
+        that independent, but for a lot of cases adaptiveMinimize() may
+        work better, as it figures out the optimal ordering of axes as it goes.
         """
         if lstStart:
             self.setStarts(lstStart)
         
         self.fBest = 1.e8;   # not close to any likely value
 
         # evaluate starting point
@@ -173,15 +249,15 @@
 
             self.fRadialScale *= 0.3183098861; # ~1/pi (any ~irrational will do)
             nCount += 1
             if self.nMaxIterations < nCount:   # bail out if we are stuck
                 nReason = -1
                 break;
                 
-            # for floating-point minimiation 0.001 is a reasonable tolerance
+            # Various reasons for quiting:
             if (self.fBest+self.fSecondBest) == 0:
                 nReason = 1
                 break
             elif (abs(self.fBest-self.fSecondBest)/(self.fBest+self.fSecondBest) <= self.fFractionalTolerance):
                 nReason = 2
                 break
             elif (self.fRadialScale <= self.fMinimumScale):
@@ -211,43 +287,50 @@
         bFound = self.bracket(nAxis,lower,middle,upper)
         
         if (bFound):
             # at this point we have a triple with the current point the lowest
             # and two higher points on either side.  We do a single parabolic
             # step to try to improve things
 
-            fA = lower.getVertex()[nAxis]     # do parabolic fit
-            fB = middle.getVertex()[nAxis] 
-            fC = upper.getVertex()[nAxis]  
-            fFa = lower.getValue() 
-            fFb = middle.getValue() 
-            fFc = upper.getValue() 
-
-            fBA = fB - fA
-            fBC = fB - fC
-            fTop = fBA*fBA*(fFb-fFc)-fBC*fBC*(fFb-fFa);
-            fBot = fBA*(fFb-fFc)-fBC*(fFb-fFa);
-
-            fDistance = 0.0
-            if (0 == fBot):  # NO DIFFERENCE--RETURN EARLY
-                self.lstHistory.append(self.lstHistory[-1])
-                self.traceOut()  # trace progress if requested
-                return self.lstHistory[-1].getValue() 
-            else:
-                fDistance = -0.5*fTop/fBot     # distance from middle
-
-            middle.incrementVertex(nAxis, fDistance)
-            fValue = self.pObjective(middle.getVertex())
-            if (fValue > self.lstHistory[-1].getValue()): # no improvement
-                fValue = self.lstHistory[-1].getValue()
-                self.traceOut() # trace progress if requested
-            else:
-                middle.setValue(fValue) 
-                self.lstHistory.append(middle) 
-                self.traceOut()  # trace progress if requested
+            fValue = self.parabolic(nAxis, lower, middle, upper)
+        
+        return fValue
+            
+    def parabolic(self, nAxis, lower, middle, upper):
+        """Take a single parabolic step"""
+        
+        fA = lower.getVertex()[nAxis]     # do parabolic fit
+        fB = middle.getVertex()[nAxis] 
+        fC = upper.getVertex()[nAxis]  
+        fFa = lower.getValue() 
+        fFb = middle.getValue() 
+        fFc = upper.getValue() 
+
+        fBA = fB - fA
+        fBC = fB - fC
+        fTop = fBA*fBA*(fFb-fFc)-fBC*fBC*(fFb-fFa);
+        fBot = fBA*(fFb-fFc)-fBC*(fFb-fFa);
+
+        fDistance = 0.0
+        if (0 == fBot):  # NO DIFFERENCE--RETURN EARLY
+            self.lstHistory.append(self.lstHistory[-1])
+            self.traceOut()  # trace progress if requested
+            return self.lstHistory[-1].getValue() 
+        else:
+            fDistance = -0.5*fTop/fBot     # distance from middle
+
+        middle.incrementVertex(nAxis, fDistance)
+        fValue = self.pObjective(middle.getVertex())
+        if (fValue > self.lstHistory[-1].getValue()): # no improvement
+            fValue = self.lstHistory[-1].getValue()
+            self.traceOut() # trace progress if requested
+        else:
+            middle.setValue(fValue) 
+            self.lstHistory.append(middle) 
+            self.traceOut()  # trace progress if requested
 
         return fValue
 
     # Bracket the minimum along a given axis
     def bracket(self, nAxis, lower, middle, upper):
         """
         Bracket the minimum along an axis using golden section algorithm.  If
@@ -321,43 +404,7 @@
     def traceOut(self):
         if self.pOutStream:
             self.pOutStream.write(str(self.lstHistory[-1].getValue())+" "+str(self.lstHistory[-1].getVertex())+"\n")
         
     # Close the trace file
     def traceClose(self):
         self.pOutStream = None
-
-if __name__ == "__main__":
-    
-    nDimension = 3
-    
-    class Test(object):
-        def __init__(self):
-            self.lstOrigin = [nI for nI in range(0,nDimension)]
-                
-        def __call__(self, lstVertex):
-            fSum = 0.0
-            for nI in range(0, nDimension):
-                fSum += (self.lstOrigin[nI]-lstVertex[nI])**2
-                
-            fSum += 1.0
-            
-            return sqrt(fSum/nDimension)
-    
-    minimizer = SimpleMinimizer(nDimension)
-    test = Test()
-    minimizer.setObjective(test)
-
-    # test bracketing.  We are starting at [0,0,0] and the minimum
-    # is at [0, 1, 2]
-    
-    lower = EmptyVertex(nDimension)
-    middle = EmptyVertex(nDimension)
-    upper = EmptyVertex(nDimension)
-    bFound = minimizer.bracket(0,lower,middle,upper)
-    print(((lower.getValue() > middle.getValue()) and (upper.getValue() > middle.getValue())))
-
-    (nCount, vertex) = minimizer.minimize()
-    lstVertex = vertex.getVertex()
-    fError = sqrt(sum([(nI-lstVertex[nI])**2 for nI in range(0,nDimension)])/nDimension)
-    print(fError < 0.001)
-    print(nCount < 10)
```

### Comparing `simple_minimizer-1.1.0/src/simple_minimizer/vertex.py` & `simple_minimizer-2.0.0/src/simple_minimizer/vertex.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def CopyVertex(v1, v2):
     v1.lstVertex = [v2.lstVertex[nI] for nI in range(0, len(v2.lstVertex))]
     v1.fValue = v2.fValue
     v1.fDistance = v2.fDistance
 
 # Helper class to hold vertex data
-class SimpleVertex(object):
+class SimpleVertex:
     
     def __init__(self, lstVertex, fValue, fDistance):
         
         # The position of the vertex
         self.lstVertex = [lstVertex[nI] for nI in range(0,len(lstVertex))]
 
         # The value at the vertex
```

### Comparing `simple_minimizer-1.1.0/.gitignore` & `simple_minimizer-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `simple_minimizer-1.1.0/LICENSE` & `simple_minimizer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_minimizer-1.1.0/README.md` & `simple_minimizer-2.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # Simple Minimizer
 
 This minimizer was designed to be brutally simple and extremely
 robust. The original aim was primarily multi-model image registration
 during the development of the pseudo-correlation image registration
-algorithm for online portal imaging and other applications.
+algorithm for online portal imaging and other applications. This means
+it works best on systems with clearly defined ("anatomical") axes
+that are largely independent of each other.
 
 It uses a combination of bracketing and parabolic interpolation to
 get the job done. It is not designed for speed.
 
 An understanding of the shape of your objective function is
 desirable. It is useful to map it on various sets of axes. 
 
 The axes you use to represent your problem are not in general 
 independent: your objective will have diagonal "troughs"
 due to the ability of one axis to trade off against another.
 
 In general you are not minimizing in a vector space, and if you are the
-scales on different axes are often wildly different.
+scales on different axes are often wildly different. Scales on each
+axis can be set via setScale(nAxis, fScale) prior to minimization.
 
 The value of the objective function should be strictly positive over the
 domain, and ideally around 1.0 near the minimum, where "around"
 means 1E-4 => 1E4 or so.
 
 If local minima are a problem call `.reseed()` on your minimizer object
 after recording the current minimum, set new starting points (or use
@@ -28,14 +31,19 @@
 lot of local minimia I've sometimes run this three or five times and looked
 for a majority vote on the true minimum or a lowest value (which works
 best depends on the scale of the noise on the objective function: if the
 noise is smooth on the scale of the minimum lowest value works well, if
 the noise is rough on the scale of the minimum majority of minima within
 a small region works well.)
 
+Version 2 has an alternative algorithm implemented in the adaptiveMinimize()
+method, which will try to work out what is the best ordering of axes to 
+minimize on by looking at the depth of the bracketed minimum. It is still
+largely experimental.
+
 Simple usage example:
 
 ```
 from math import sqrt
 
 from simple_minimizer import *
```

### Comparing `simple_minimizer-1.1.0/pyproject.toml` & `simple_minimizer-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simple-minimizer"
-version = "1.1.0"
+version = "2.0.0"
 authors = [
   { name="TJ Radcliffe", email="tj@tjradcliffe.com" },
 ]
 description = "A brutally simple, extremely robust minimizer"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `simple_minimizer-1.1.0/PKG-INFO` & `simple_minimizer-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-minimizer
-Version: 1.1.0
+Version: 2.0.0
 Summary: A brutally simple, extremely robust minimizer
 Project-URL: Homepage, https://github.com/tjradcliffe/simple-minimizer
 Project-URL: Bug Tracker, https://github.com/tjradcliffe/simple-minimizer/issues
 Author-email: TJ Radcliffe <tj@tjradcliffe.com>
 License: Copyright (c) 2022 Thomas J. Radcliffe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,28 +32,31 @@
 Description-Content-Type: text/markdown
 
 # Simple Minimizer
 
 This minimizer was designed to be brutally simple and extremely
 robust. The original aim was primarily multi-model image registration
 during the development of the pseudo-correlation image registration
-algorithm for online portal imaging and other applications.
+algorithm for online portal imaging and other applications. This means
+it works best on systems with clearly defined ("anatomical") axes
+that are largely independent of each other.
 
 It uses a combination of bracketing and parabolic interpolation to
 get the job done. It is not designed for speed.
 
 An understanding of the shape of your objective function is
 desirable. It is useful to map it on various sets of axes. 
 
 The axes you use to represent your problem are not in general 
 independent: your objective will have diagonal "troughs"
 due to the ability of one axis to trade off against another.
 
 In general you are not minimizing in a vector space, and if you are the
-scales on different axes are often wildly different.
+scales on different axes are often wildly different. Scales on each
+axis can be set via setScale(nAxis, fScale) prior to minimization.
 
 The value of the objective function should be strictly positive over the
 domain, and ideally around 1.0 near the minimum, where "around"
 means 1E-4 => 1E4 or so.
 
 If local minima are a problem call `.reseed()` on your minimizer object
 after recording the current minimum, set new starting points (or use
@@ -61,14 +64,19 @@
 lot of local minimia I've sometimes run this three or five times and looked
 for a majority vote on the true minimum or a lowest value (which works
 best depends on the scale of the noise on the objective function: if the
 noise is smooth on the scale of the minimum lowest value works well, if
 the noise is rough on the scale of the minimum majority of minima within
 a small region works well.)
 
+Version 2 has an alternative algorithm implemented in the adaptiveMinimize()
+method, which will try to work out what is the best ordering of axes to 
+minimize on by looking at the depth of the bracketed minimum. It is still
+largely experimental.
+
 Simple usage example:
 
 ```
 from math import sqrt
 
 from simple_minimizer import *
```

