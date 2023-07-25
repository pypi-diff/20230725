# Comparing `tmp/pysolar-0.8.tar.gz` & `tmp/pysolar-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysolar-0.8.tar", last modified: Fri Sep 28 20:12:20 2018, max compression
+gzip compressed data, was "dist/pysolar-0.9.tar", last modified: Sun Oct 18 14:11:26 2020, max compression
```

## Comparing `pysolar-0.8.tar` & `pysolar-0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-09-28 20:12:20.000000 pysolar-0.8/
--rwxrwxrwx   0 root         (0) root         (0)       13 2018-03-30 20:37:16.000000 pysolar-0.8/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)      356 2018-09-28 20:12:20.000000 pysolar-0.8/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-09-28 20:12:20.000000 pysolar-0.8/pysolar/
--rwxrwxrwx   0 root         (0) root         (0)    12794 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/constants.py
--rwxrwxrwx   0 root         (0) root         (0)      793 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/constants.pyi
--rwxrwxrwx   0 root         (0) root         (0)     3035 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/elevation.py
--rwxrwxrwx   0 root         (0) root         (0)      337 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/elevation.pyi
--rwxrwxrwx   0 root         (0) root         (0)     4160 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/numeric.py
--rwxrwxrwx   0 root         (0) root         (0)     1802 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/radiation.py
--rwxrwxrwx   0 root         (0) root         (0)      320 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/radiation.pyi
--rwxrwxrwx   0 root         (0) root         (0)    14878 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/rest.py
--rwxrwxrwx   0 root         (0) root         (0)     2707 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/simulate.py
--rwxrwxrwx   0 root         (0) root         (0)      616 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/simulate.pyi
--rwxrwxrwx   0 root         (0) root         (0)    18677 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/solar.py
--rwxrwxrwx   0 root         (0) root         (0)     3782 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/solar.pyi
--rwxrwxrwx   0 root         (0) root         (0)    20359 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/solartime.py
--rwxrwxrwx   0 root         (0) root         (0)      781 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/solartime.pyi
--rwxrwxrwx   0 root         (0) root         (0)     3188 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/tzinfo_check.py
--rwxrwxrwx   0 root         (0) root         (0)    24117 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/util.py
--rwxrwxrwx   0 root         (0) root         (0)     2791 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/util.pyi
--rwxrwxrwx   0 root         (0) root         (0)      194 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2018-09-28 19:57:35.000000 pysolar-0.8/pysolar/__init__.pyi
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-09-28 20:12:20.000000 pysolar-0.8/pysolar.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)        1 2018-09-28 20:12:19.000000 pysolar-0.8/pysolar.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      356 2018-09-28 20:12:19.000000 pysolar-0.8/pysolar.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      616 2018-09-28 20:12:19.000000 pysolar-0.8/pysolar.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2018-09-28 20:12:19.000000 pysolar-0.8/pysolar.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2018-09-28 20:12:20.000000 pysolar-0.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1127 2018-09-28 20:12:02.000000 pysolar-0.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-09-28 20:12:20.000000 pysolar-0.8/test/
--rwxrwxrwx   0 root         (0) root         (0)    11938 2018-09-28 19:57:35.000000 pysolar-0.8/test/test_datetime_tzinfo.py
--rwxrwxrwx   0 root         (0) root         (0)     2415 2018-03-30 20:37:17.000000 pysolar-0.8/test/test_hour_angle.py
--rwxrwxrwx   0 root         (0) root         (0)     2488 2018-09-28 19:57:35.000000 pysolar-0.8/test/test_numpy.py
--rwxrwxrwx   0 root         (0) root         (0)    10838 2018-09-28 19:57:35.000000 pysolar-0.8/test/test_solar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-18 14:11:26.869771 pysolar-0.9/
+-rw-r--r--   0 root         (0) root         (0)       13 2020-10-16 00:58:11.000000 pysolar-0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      341 2020-10-18 14:11:26.869771 pysolar-0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-18 14:11:26.865771 pysolar-0.9/pysolar/
+-rw-r--r--   0 root         (0) root         (0)      194 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)    12796 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/constants.py
+-rw-r--r--   0 root         (0) root         (0)      793 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/constants.pyi
+-rw-r--r--   0 root         (0) root         (0)     3035 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/elevation.py
+-rw-r--r--   0 root         (0) root         (0)      337 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/elevation.pyi
+-rw-r--r--   0 root         (0) root         (0)     4150 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/numeric.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/radiation.py
+-rw-r--r--   0 root         (0) root         (0)      320 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/radiation.pyi
+-rw-r--r--   0 root         (0) root         (0)    14942 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/rest.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/simulate.py
+-rw-r--r--   0 root         (0) root         (0)      616 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/simulate.pyi
+-rw-r--r--   0 root         (0) root         (0)    18678 2020-10-18 13:25:49.000000 pysolar-0.9/pysolar/solar.py
+-rw-r--r--   0 root         (0) root         (0)     3782 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/solar.pyi
+-rw-r--r--   0 root         (0) root         (0)    20403 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/solartime.py
+-rw-r--r--   0 root         (0) root         (0)      781 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/solartime.pyi
+-rw-r--r--   0 root         (0) root         (0)     3188 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/tzinfo_check.py
+-rw-r--r--   0 root         (0) root         (0)    25564 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/util.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2020-10-16 00:58:11.000000 pysolar-0.9/pysolar/util.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-18 14:11:26.865771 pysolar-0.9/pysolar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      341 2020-10-18 14:11:26.000000 pysolar-0.9/pysolar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      616 2020-10-18 14:11:26.000000 pysolar-0.9/pysolar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-10-18 14:11:26.000000 pysolar-0.9/pysolar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2020-10-18 14:11:26.000000 pysolar-0.9/pysolar.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2020-10-18 14:11:26.869771 pysolar-0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1119 2020-10-18 13:46:32.000000 pysolar-0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-18 14:11:26.869771 pysolar-0.9/test/
+-rw-r--r--   0 root         (0) root         (0)    12103 2020-10-16 00:58:11.000000 pysolar-0.9/test/test_datetime_tzinfo.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2020-10-16 00:58:11.000000 pysolar-0.9/test/test_hour_angle.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2020-10-16 00:58:11.000000 pysolar-0.9/test/test_numpy.py
+-rwxr-xr-x   0 root         (0) root         (0)    10841 2020-10-16 00:58:11.000000 pysolar-0.9/test/test_solar.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pysolar-0.8/pysolar/constants.py` & `pysolar-0.9/pysolar/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,30 +234,30 @@
             (357,2.92,0.067),
             (317,5.849,11790.629),
             (284,1.899,796.298),
             (271,0.315,10977.079),
             (243,0.345,5486.778),
             (206,4.806,2544.314),
             (205,1.869,5573.143),
-            (202,2.4458,6069.777),
+            (202,2.458,6069.777),
             (156,0.833,213.299),
             (132,3.411,2942.463),
             (126,1.083,20.775),
             (115,0.645,0.98),
             (103,0.636,4694.003),
             (102,0.976,15720.839),
             (102,4.267,7.114),
             (99,6.21,2146.17),
             (98,0.68,155.42),
             (86,5.98,161000.69),
             (85,1.3,6275.96),
             (85,3.67,71430.7),
             (80,1.81,17260.15),
             (79,3.04,12036.46),
-            (71,1.76,5088.63),
+            (75,1.76,5088.63),
             (74,3.5,3154.69),
             (74,4.68,801.82),
             (70,0.83,9437.76),
             (62,3.98,8827.39),
             (61,1.82,7084.9),
             (57,2.78,6286.6),
             (56,4.39,14143.5),
@@ -302,15 +302,15 @@
             (16,1.43,2146.17),
             (15,1.21,10977.08),
             (12,2.83,1748.02),
             (12,3.26,5088.63),
             (12,5.27,1194.45),
             (12,2.08,4694),
             (11,0.77,553.57),
-            (10,1.3,3286.6),
+            (10,1.3,6286.6),
             (10,4.24,1349.87),
             (9,2.7,242.73),
             (9,5.64,951.72),
             (8,5.3,2352.87),
             (6,2.65,9437.76),
             (6,4.67,4690.48)
         ],
@@ -389,15 +389,15 @@
             (212.0,5.847,1577.344),
             (186.0,5.022,10977.079),
             (175.0,3.012,18849.228),
             (110.0,5.055,5486.778),
             (98,0.89,6069.78),
             (86,5.69,15720.84),
             (86,1.27,161000.69),
-            (85,0.27,17260.15),
+            (65,0.27,17260.15),
             (63,0.92,529.69),
             (57,2.01,83996.85),
             (56,5.24,71430.7),
             (49,3.25,2544.31),
             (47,2.58,775.52),
             (45,5.54,9437.76),
             (43,6.01,6275.96),
@@ -428,15 +428,15 @@
         ],
         [  # R2
             (4359.0,5.7846,6283.0758),
             (124.0,5.579,12566.152),
             (12,3.14,0),
             (9,3.63,77713.77),
             (6,1.87,5573.14),
-            (3,5.47,18849)
+            (3,5.47,18849.23)
         ],
         [  # R3
             (145.0,4.273,6283.076),
             (7,3.92,12566.15),
         ],
         [  # R4
             (4,2.56,6283.08)
```

### Comparing `pysolar-0.8/pysolar/constants.pyi` & `pysolar-0.9/pysolar/constants.pyi`

 * *Files identical despite different names*

### Comparing `pysolar-0.8/pysolar/elevation.py` & `pysolar-0.9/pysolar/elevation.py`

 * *Files identical despite different names*

### Comparing `pysolar-0.8/pysolar/numeric.py` & `pysolar-0.9/pysolar/numeric.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,10 +133,9 @@
     globals()['tm_min'] = tm_min_math
     globals()['current_mod'] = 'math'
 
 
 try:
     import numpy
     use_numpy()
-except ModuleNotFoundError:
+except ImportError:
     pass
-
```

### Comparing `pysolar-0.8/pysolar/radiation.py` & `pysolar-0.9/pysolar/radiation.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 def get_optical_depth(day):
     # from Masters, p. 412
     return 0.174 + (0.035 * math.sin(2 * math.pi / 365 * (day - 100)))
 #end get_optical_depth
 
 def get_radiation_direct(when, altitude_deg):
     # from Masters, p. 412
-    if int(altitude_deg) <= 0:
-        return 0.0
-    day = when.utctimetuple().tm_yday
+    is_daytime = (altitude_deg > 0)
+    day = math.tm_yday(when)
     flux = get_apparent_extraterrestrial_flux(day)
     optical_depth = get_optical_depth(day)
     air_mass_ratio = get_air_mass_ratio(altitude_deg)
-    return flux * math.exp(-1 * optical_depth * air_mass_ratio)
+    return flux * math.exp(-1 * optical_depth * air_mass_ratio) * is_daytime
 #end get_radiation_direct
```

### Comparing `pysolar-0.8/pysolar/rest.py` & `pysolar-0.9/pysolar/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License along
 #    with Pysolar. If not, see <http://www.gnu.org/licenses/>.
 
+# Disable linting as this is a work in progress
+# flake8: noqa
+
 from . import numeric as math
 from .constants import standard_pressure
 
 # single-scattering albedo used to calculate aerosol scattering transmittance;
 # not used for sky or ground albedo for backscattering estimate
 albedo = {}
```

### Comparing `pysolar-0.8/pysolar/simulate.py` & `pysolar-0.9/pysolar/simulate.py`

 * *Files identical despite different names*

### Comparing `pysolar-0.8/pysolar/simulate.pyi` & `pysolar-0.9/pysolar/simulate.pyi`

 * *Files identical despite different names*

### Comparing `pysolar-0.8/pysolar/solar.py` & `pysolar-0.9/pysolar/solar.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,20 @@
 """
 from . import numeric as math
 import datetime
 from . import constants
 from . import solartime as stime
 from . import radiation
 from .tzinfo_check import check_aware_dt
-import pytz
 
 
 def solar_test():
     latitude_deg = 42.364908
     longitude_deg = -71.112828
-    d = datetime.datetime.now(tz=pytz.UTC)
+    d = datetime.datetime.now(tz=datetime.timezone.utc)
     thirty_minutes = datetime.timedelta(hours = 0.5)
     for _ in range(48):
         timestamp = d.ctime()
         altitude_deg = get_altitude(latitude_deg, longitude_deg, d)
         azimuth_deg = get_azimuth(latitude_deg, longitude_deg, d)
         power = radiation.get_radiation_direct(d, altitude_deg)
         if (altitude_deg > 0):
```

### Comparing `pysolar-0.8/pysolar/solar.pyi` & `pysolar-0.9/pysolar/solar.pyi`

 * *Files identical despite different names*

### Comparing `pysolar-0.8/pysolar/solartime.py` & `pysolar-0.9/pysolar/solartime.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,16 @@
       (+1, 0), # 2012
       (0, 0), # 2013
       (0, 0), # 2014
       (+1, 0), # 2015
       (0, +1), # 2016
       (0, 0),  # 2017
       (0, 0),  # 2018
+      (0, 0),  # 2019
+      (0, 0),  # 2020
     ]
 
 @check_aware_dt('when')
 def get_leap_seconds(when) :
     "returns adjustment to be added to UTC at the specified datetime to produce TAI."
     when = when.utctimetuple()
     adj = 10 # as decreed from 1972
```

### Comparing `pysolar-0.8/pysolar/solartime.pyi` & `pysolar-0.9/pysolar/solartime.pyi`

 * *Files identical despite different names*

### Comparing `pysolar-0.8/pysolar/tzinfo_check.py` & `pysolar-0.9/pysolar/tzinfo_check.py`

 * *Files identical despite different names*

### Comparing `pysolar-0.8/pysolar/util.py` & `pysolar-0.9/pysolar/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 SC_default = 1367.0          # Solar constant in W/m^2 is 1367.0. Note that this value could vary by +/-4 W/m^2
 TY_default = 365             # Total year number from 1 to 365 days
 elevation_default = 0.0      # Default elevation is 0.0
 
 # Useful equations for analysis
 
 @check_aware_dt('when')
-def get_sunrise_sunset(latitude_deg, longitude_deg, when):
-    """This function calculates the astronomical sunrise and sunset times in local time.
+def get_sunrise_sunset_transit(latitude_deg, longitude_deg, when):
+    """This function calculates the astronomical sunrise, sunset and sun transit times in local time.
 
     Parameters
     ----------
     latitude_deg : float
         latitude in decimal degree. A geographical term denoting
         the north/south angular location of a place on a sphere.
     longitude_deg : float
@@ -61,40 +61,63 @@
 
     Returns
     -------
     sunrise_time_dt : datetime.datetime
         Sunrise time in local time.
     sunset_time_dt : datetime.datetime
         Sunset time in local time.
+    transit_time_dt:
+        Sun transit time in local time.
 
     References
     ----------
-    .. [1] http://www.skypowerinternational.com/pdf/Radiation/7.1415.01.121_cm121_bed-anleitung_engl.pdf
+    .. [1] http://www.skypowerinternational.com/uploads/documents/7.1415.01.121_cm121_bed-anleitung_engl.pdf
     .. [2] http://pysolar.org/
+    .. [3] https://www.esrl.noaa.gov/gmd/grad/solcalc/solareqns.PDF
+    .. [4] https://www.sciencedirect.com/science/article/pii/S0038092X11004592
+    .. [5] https://iris.unipa.it/retrieve/handle/10447/55143/28818/Articolo.pdf
 
     Examples
     --------
     >>> lat = 50.111512
     >>> lon = 8.680506
-    >>> timezone_local = pytz.timezone('Europe/Berlin')
+    >>> timezone_local = dateutil.tz.gettz('Europe/Berlin')
     >>> now = datetime.now(timezone_local)
-    >>> sr, ss = sb.get_sunrise_sunset(lat, lon, now)
+    >>> sr, ss, tr = sb.get_sunrise_sunset_transit(lat, lon, now)
     >>> print('sunrise: ', sr)
     >>> print('sunset:', ss)
+    >>> print('transit:', tr)
 
     """
 
     utc_offset = when.utcoffset()
     if utc_offset != None :
         utc_offset = utc_offset.total_seconds()
     else :
         utc_offset = 0
     #end if
     day = when.utctimetuple().tm_yday # Day of the year
     SHA = utc_offset / 3600 * 15.0 - longitude_deg # Solar hour angle
+    TT = 2 * math.pi * day / 366
+    decl = \
+        (
+            0.322003
+        -
+            22.971 * math.cos(TT)
+        -
+            0.357898 * math.cos(2 * TT)
+        -
+            0.14398 * math.cos(3 * TT)
+        +
+            3.94638 * math.sin(TT)
+        +
+            0.019334 * math.sin(2 * TT)
+        +
+            0.05928 * math.sin(3 * TT)
+        ) # solar declination in degrees
     TT = math.radians(279.134 + 0.985647 * day) # Time adjustment angle
     time_adst = \
         (
                 (
                     5.0323
                 -
                     100.976 * math.sin(TT)
@@ -111,44 +134,61 @@
                 +
                     18.25 * math.cos(3 * TT)
                 )
             /
                 3600
         ) # Time adjustment in hours
     TON = 12 + SHA / 15.0 - time_adst # Time of noon
-    sunn = \
+    ha = \
         (
-            (
-                math.pi / 2
-            -
-                    math.radians(constants.earth_axis_inclination)
-                *
-                    math.tan(math.radians(latitude_deg))
+            math.acos(
+                math.cos(math.radians(90.833))
+            /
+                (
+                    math.cos(math.radians(latitude_deg))
                 *
-                    math.cos(2 * math.pi * day / 365.25)
+                    math.cos(math.radians(decl))
+                )
+            -
+                math.tan(math.radians(latitude_deg))
+            *
+                math.tan(math.radians(decl))
             )
         *
             (12 / math.pi)
         )
     same_day = datetime(year = when.year, month = when.month, day = when.day, tzinfo = when.tzinfo)
-    sunrise_time = same_day + timedelta(hours = TON - sunn + time_adst)
-    sunset_time = same_day + timedelta(hours = TON + sunn - time_adst)
-    return sunrise_time, sunset_time
+    sunrise_time = same_day + timedelta(hours = TON - ha)
+    sunset_time = same_day + timedelta(hours = TON + ha)
+    transit_time = same_day + timedelta(hours = TON)
+    return sunrise_time, sunset_time, transit_time
+
+@check_aware_dt('when')
+def get_sunrise_sunset(latitude_deg, longitude_deg, when):
+    "Wrapper for get_sunrise_sunset_transit that returns just the sunrise and the sunset time."
+    return \
+        get_sunrise_sunset_transit(latitude_deg, longitude_deg, when)[0:2]
 
 @check_aware_dt('when')
 def get_sunrise_time(latitude_deg, longitude_deg, when):
-    "Wrapper for get_sunrise_sunset that returns just the sunrise time."
+    "Wrapper for get_sunrise_sunset_transit that returns just the sunrise time."
     return \
-        get_sunrise_sunset(latitude_deg, longitude_deg, when)[0]
+        get_sunrise_sunset_transit(latitude_deg, longitude_deg, when)[0]
 
 @check_aware_dt('when')
 def get_sunset_time(latitude_deg, longitude_deg, when):
-    "Wrapper for get_sunrise_sunset that returns just the sunset time."
+    "Wrapper for get_sunrise_sunset_transit that returns just the sunset time."
+    return \
+        get_sunrise_sunset_transit(latitude_deg, longitude_deg, when)[1]
+
+@check_aware_dt('when')
+def get_transit_time(latitude_deg, longitude_deg, when):
+    "Wrapper for get_sunrise_sunset_transit that returns just the transit time."
     return \
-        get_sunrise_sunset(latitude_deg, longitude_deg, when)[1]
+        get_sunrise_sunset_transit(latitude_deg, longitude_deg, when)[2]
 
 @check_aware_dt('when')
 def mean_earth_sun_distance(when):
     """Mean Earth-Sun distance is the arithmetical mean of the maximum and minimum distances
     between a planet (Earth) and the object about which it revolves (Sun). However,
     the function is used to  calculate the Mean earth sun distance.
```

### Comparing `pysolar-0.8/pysolar/util.pyi` & `pysolar-0.9/pysolar/util.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 
 AM_default: float
 TL_default: float
 SC_default: float
 TY_default: float
 elevation_default: float
 
+def get_sunrise_sunset_transit(latitude_deg:float, longitude_deg:float, when:datetime.datetime) -> Tuple[datetime.datetime, datetime.datetime, datetime.datetime]: ...
 def get_sunrise_sunset(latitude_deg:float, longitude_deg:float, when:datetime.datetime) -> Tuple[datetime.datetime, datetime.datetime]: ...
 def get_sunrise_time(latitude_deg:float, longitude_deg:float, when:datetime.datetime) -> datetime.datetime: ...
 def get_sunset_time(latitude_deg:float, longitude_deg:float, when:datetime.datetime) -> datetime.datetime: ...
+def get_transit_time(latitude_deg:float, longitude_deg:float, when:datetime.datetime) -> datetime.datetime: ...
 def mean_earth_sun_distance(when:datetime.datetime) -> float: ...
 def extraterrestrial_irrad(when:datetime.datetime, latitude_deg:float, longitude_deg:float, SC:float = ...) -> float: ...
 def declination_degree(when:datetime.datetime, TY:float = ...) -> float: ...
 def solarelevation_function_clear(latitude_deg:float, longitude_deg:float, when:datetime.datetime, temperature:float = ..., pressure:float = ..., elevation:float = ...) -> float: ...
 def solarelevation_function_overcast(latitude_deg:float, longitude_deg:float, when:datetime.datetime, elevation:float = ..., temperature:float = ..., pressure:float = ...) -> float: ...
 def diffuse_transmittance(TL:float = ...) -> float: ...
 def diffuse_underclear(latitude_deg:float, longitude_deg:float, when:datetime.datetime, elevation:float = ..., temperature:float = ..., pressure:float = ..., TL:float = ...) -> float: ...
```

### Comparing `pysolar-0.8/pysolar.egg-info/SOURCES.txt` & `pysolar-0.9/pysolar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysolar-0.8/setup.py` & `pysolar-0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     'Topic :: Scientific/Engineering :: Atmospheric Science',
     'Topic :: Scientific/Engineering :: Mathematics',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Programming Language :: Python :: 3']
 
 
 setup(name='pysolar',
-    version='0.8',
+    version='0.9',
     description='Collection of Python libraries for simulating the irradiation of any point on earth by the sun',
     author='Brandon Stafford',
     author_email='brandon@pingswept.org',
     license = 'GNU General Public License (GPL)',
     url='http://pysolar.org',
     packages=['pysolar'],
     package_data = {"pysolar": ["*.pyi"]},  # *.py is included in any case
-    requires = ['numpy', 'pytz'],
+    requires = ['numpy'],
     )
```

### Comparing `pysolar-0.8/test/test_datetime_tzinfo.py` & `pysolar-0.9/test/test_datetime_tzinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 receives only timezone-aware ones.
 """
 
 from pysolar import solar
 from pysolar import solartime
 from pysolar import util
 import datetime
-import pytz
 import unittest
 from pysolar.tzinfo_check import NoTimeZoneInfoError
 import numpy as np
 
 
 class TestErrorTimeZoneIsNone(unittest.TestCase):
   unaware = datetime.datetime(2000, 1, 1)
@@ -92,14 +91,18 @@
     with self.assertRaises(NoTimeZoneInfoError):
       util.get_sunrise_time(self.lat, self.lon, self.unaware)
 
   def test_util_get_sunset_time_raise_error(self):
     with self.assertRaises(NoTimeZoneInfoError):
       util.get_sunset_time(self.lat, self.lon, self.unaware)
 
+  def test_util_get_transit_time_raise_error(self):
+    with self.assertRaises(NoTimeZoneInfoError):
+      util.get_transit_time(self.lat, self.lon, self.unaware)
+
   def test_util_mean_earth_sun_distance_raise_error(self):
     with self.assertRaises(NoTimeZoneInfoError):
       util.mean_earth_sun_distance(self.unaware)
 
   def test_util_extraterrestrial_irrad_raise_error(self):
     with self.assertRaises(NoTimeZoneInfoError):
       util.extraterrestrial_irrad(self.lat, self.lon, self.unaware)
@@ -136,15 +139,15 @@
     with self.assertRaises(NoTimeZoneInfoError):
       ghi_data = np.asarray([0, 0]) # Don't know what ghi_data is supposed to be
       util.clear_index(ghi_data, self.lat, self.lon, self.unaware)
 
 
 
 class TestTimeZoneNotNone(unittest.TestCase):
-  aware = datetime.datetime(2000, 1, 1, tzinfo=pytz.utc)
+  aware = datetime.datetime(2000, 1, 1, tzinfo=datetime.timezone.utc)
 
   lat = 1.0
   lon = 1.0
 
   def test_solar_topocentric_position_no_error(self):
     try:
       solar.get_topocentric_position(self.lat, self.lon, self.aware)
```

### Comparing `pysolar-0.8/test/test_hour_angle.py` & `pysolar-0.9/test/test_hour_angle.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Created on Aug 13, 2015
 
 @author: rene
 '''
 import unittest
 import datetime
 from pysolar.solar import *
-import pytz
 from pysolar.solartime import *
 
 
 class Test(unittest.TestCase):
 
     def setUp(self):
         pass
@@ -22,21 +21,16 @@
 
         '''
         Example 1.6.1 from Book "Solar Engineering of Thermal Processes by Duffie and Beckman, fourth edition, Wiley 2013"
 
         hour angle should be -22.5. (-22.5 % 360.0 = 337.5)
         '''
 
-        tz = pytz.timezone('US/Central')
-        when = tz.localize(datetime.datetime(
-            2008,
-            2,
-            13,
-            10,
-            42))
+        tz = datetime.timezone(datetime.timedelta(hours=-6))
+        when = datetime.datetime(2008, 2, 13, 10, 42, tzinfo=tz)
 
         latitude_deg = 43.076342
         longitude_deg = -89.384448
 
         '''
         Hour angle from get_hour_angle
         '''
```

### Comparing `pysolar-0.8/test/test_numpy.py` & `pysolar-0.9/test/test_numpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 import pysolar
-from pysolar import solar
+from pysolar import radiation, solar
 from pysolar import numeric as math
-from datetime import datetime
-import pytz
+import datetime
 import numpy as np
 from nose.tools import raises, assert_equal
 
 
 @raises(TypeError)
 def test_fail_with_math():
     pysolar.use_math()
     lat = np.array([45., 40.])
     lon = np.array([3., 4.])
-    time = datetime(2018, 5, 8, 12, 0, 0, tzinfo=pytz.UTC)
+    time = datetime.datetime(2018, 5, 8, 12, 0, 0, tzinfo=datetime.timezone.utc)
 
     solar.get_altitude(lat, lon, time)
 
 
 def test_scalar_with_math():
     pysolar.use_math()
 
     lat = 45.
     lon = 3.
-    time = datetime(2018, 5, 8, 12, 0, 0, tzinfo=pytz.UTC)
+    time = datetime.datetime(2018, 5, 8, 12, 0, 0, tzinfo=datetime.timezone.utc)
 
     print(solar.get_altitude(lat, lon, time))
     print(solar.get_azimuth(lat, lon, time))
 
 
 def test_scalar_with_numpy():
     pysolar.use_numpy()
 
     lat = 50.63
     lon = 3.05
-    time = datetime(2018, 5, 8, 12, 0, 0, tzinfo=pytz.UTC)
+    time = datetime.datetime(2018, 5, 8, 12, 0, 0, tzinfo=datetime.timezone.utc)
     print(solar.get_altitude(lat, lon, time))
     print(solar.get_azimuth(lat, lon, time))
 
 
 def test_with_fixed_time():
     """ get_altitude and get_azimuth, with scalar date """
     pysolar.use_numpy()
 
     lat = np.array([45., 40.])
     lon = np.array([3., 4.])
 
-    time = datetime(2018, 5, 8, 12, 0, 0, tzinfo=pytz.UTC)
+    time = datetime.datetime(2018, 5, 8, 12, 0, 0, tzinfo=datetime.timezone.utc)
 
     print(solar.get_altitude(lat, lon, time))
     print(solar.get_azimuth(lat, lon, time))
     print(solar.get_altitude_fast(lat, lon, time))
     print(solar.get_azimuth_fast(lat, lon, time))
 
 
@@ -64,15 +63,15 @@
                      '2018-05-08T15:00:00'], dtype='datetime64')
 
     print(solar.get_altitude_fast(lat, lon, time))
     print(solar.get_azimuth_fast(lat, lon, time))
 
 def test_datetime_operations():
 
-    d0 = datetime(2018,5,8,12,0,0)
+    d0 = datetime.datetime(2018,5,8,12,0,0)
     d1 = np.array(d0)
 
     assert_equal(math.tm_yday_math(d0),
                  math.tm_yday_numpy(d1))
 
     assert_equal(math.tm_hour_math(d0),
                  math.tm_hour_numpy(d1))
@@ -88,8 +87,29 @@
     lat = np.array([45., 40.])
     lon = np.array([3., 4.])
 
     time = np.array(['2018-05-08T12:15:00',
                      '2018-05-08T15:00:00'], dtype='datetime64')
 
     print(solar.get_altitude_fast(lat, lon, time))
-    print(solar.get_azimuth_fast(lat, lon, time))
+    print(solar.get_azimuth_fast(lat, lon, time))
+
+
+def test_numpy_radiation():
+    """
+    get_radiation_direct with lat, lon, and date as arrays
+    """
+    pysolar.use_numpy()
+
+    lat = np.array([45., 40., 40.])
+    lon = np.array([3., 4., 3.])
+
+    time = np.array([
+        '2018-05-08T12:15:00',
+        '2018-05-08T15:00:00',
+        '2018-05-08T03:00:00',
+    ], dtype='datetime64')
+
+    altitude = solar.get_altitude_fast(lat, lon, time)
+    rad_results = radiation.get_radiation_direct(time, altitude)
+    assert rad_results[2] == 0
+    print(rad_results)
```

### Comparing `pysolar-0.8/test/test_solar.py` & `pysolar-0.9/test/test_solar.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,21 +94,21 @@
 		self.assertAlmostEqual(0.0001011219, self.geocentric_latitude, 8) # above fails with more accurate Julian Ephemeris correction
 
 	def test_get_nutation(self):
 		self.assertAlmostEqual(0.00166657, self.nutation['obliquity'], 8) # value from Reda and Andreas (2005)
 		self.assertAlmostEqual(-0.00399840, self.nutation['longitude'], 8) # value from Reda and Andreas (2005)
 
 	def test_get_sun_earth_distance(self):
-		self.assertAlmostEqual(0.9965421031, self.sun_earth_distance, 7) # value from Reda and Andreas (2005)
+		self.assertAlmostEqual(0.9965421031, self.sun_earth_distance, 6) # value from Reda and Andreas (2005)
 
 	def test_get_true_ecliptic_obliquity(self):
 		self.assertAlmostEqual(23.440465, self.true_ecliptic_obliquity, 6) # value from Reda and Andreas (2005)
 
 	def test_get_aberration_correction(self):
-		self.assertAlmostEqual(-0.0057113603, self.aberration_correction, 9) # value not validated
+		self.assertAlmostEqual(-0.005711359, self.aberration_correction, 9) # value not validated
 
 	def test_get_apparent_sun_longitude(self):
 		# self.assertAlmostEqual(204.0085537528, self.apparent_sun_longitude, 10) # value from Reda and Andreas (2005)
 		self.assertAlmostEqual(204.0085537528, self.apparent_sun_longitude, 4) # above fails with more accurate Julian Ephemeris correction
 
 	def test_get_apparent_sidereal_time(self):
 		self.assertAlmostEqual(318.5119, self.apparent_sidereal_time, 2) # value derived from Reda and Andreas (2005)
@@ -125,15 +125,15 @@
 	def test_get_projected_radial_distance(self):
 		self.assertAlmostEqual(0.7702006, self.projected_radial_distance, 6) # value not validated
 
 	def test_get_topocentric_sun_right_ascension(self):
 		self.assertAlmostEqual(202.22741, self.topocentric_sun_right_ascension, 3) # value from Reda and Andreas (2005)
 
 	def test_get_parallax_sun_right_ascension(self):
-		self.assertAlmostEqual(-0.0003659911495454668, self.parallax_sun_right_ascension, 12) # value not validated
+		self.assertAlmostEqual(-0.0003659912761437859, self.parallax_sun_right_ascension, 12) # value not validated
 		
 	def test_get_topocentric_sun_declination(self):
 		self.assertAlmostEqual(-9.316179, self.topocentric_sun_declination, 3) # value from Reda and Andreas (2005)
 
 	def test_get_topocentric_local_hour_angle(self):
 		self.assertAlmostEqual(11.10629, self.topocentric_local_hour_angle, 4) # value from Reda and Andreas (2005)
 
@@ -155,33 +155,33 @@
 
 
 class TestApi(unittest.TestCase):
 	test_when = datetime.datetime(2016, 12, 19, 23, 0, 0, tzinfo=datetime.timezone.utc)
 
 	def testGetPosition(self):
 		az, al = solar.get_position(59.6365662,12.5350953, TestApi.test_when)
-		self.assertAlmostEqual(az, 357.1431475)
-		self.assertAlmostEqual(al, -53.7672218)
+		self.assertAlmostEqual(az, 357.1431414)
+		self.assertAlmostEqual(al, -53.7672217)
 
 		az, al = solar.get_position(-43, 172, TestApi.test_when)
-		self.assertAlmostEqual(az, 50.5003507)
-		self.assertAlmostEqual(al, 63.0922058)
+		self.assertAlmostEqual(az, 50.50035708)
+		self.assertAlmostEqual(al, 63.0922036)
 
 		# From Greenwich
 		az, al = solar.get_position(51.4826, 0, TestApi.test_when)
-		self.assertAlmostEqual(az, 333.0403866)
-		self.assertAlmostEqual(al, -59.8372445)
+		self.assertAlmostEqual(az, 333.04037976)
+		self.assertAlmostEqual(al, -59.83724345)
 
 	def testGetAltitude(self):
 		al = solar.get_altitude(-43, 172, TestApi.test_when)
-		self.assertAlmostEqual(al, 63.0922058)
+		self.assertAlmostEqual(al, 63.0922036)
 
 	def testGetAzimuth(self):
 		az = solar.get_azimuth(-43, 172, TestApi.test_when)
-		self.assertAlmostEqual(az, 50.5003507)
+		self.assertAlmostEqual(az, 50.50035708)
 
 	def testGetAltitudeFast(self):
 		# location is in NZ, use relevant timezone
 		day = datetime.datetime(
 		    2016, 12, 19, 0, 0,
 		    tzinfo=datetime.timezone(datetime.timedelta(hours=12)))
 		for hour in range(7, 19):
```

