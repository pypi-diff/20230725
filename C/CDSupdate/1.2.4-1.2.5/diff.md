# Comparing `tmp/CDSupdate-1.2.4.tar.gz` & `tmp/CDSupdate-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CDSupdate-1.2.4.tar", last modified: Wed May 31 14:48:35 2023, max compression
+gzip compressed data, was "CDSupdate-1.2.5.tar", last modified: Tue Jul 25 14:59:24 2023, max compression
```

## Comparing `CDSupdate-1.2.4.tar` & `CDSupdate-1.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-31 14:48:35.986013 CDSupdate-1.2.4/
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-31 14:48:35.982017 CDSupdate-1.2.4/CDSupdate/
--rw-r--r--   0 yrobin     (501) staff       (20)     9506 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__CDSUParams.py
--rw-r--r--   0 yrobin     (501) staff       (20)     5145 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__CVarsParams.py
--rw-r--r--   0 yrobin     (501) staff       (20)     2685 2022-08-31 14:53:13.000000 CDSupdate-1.2.4/CDSupdate/__curses_doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)     3744 2023-05-05 06:01:11.000000 CDSupdate-1.2.4/CDSupdate/__doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)      969 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__exceptions.py
--rw-r--r--   0 yrobin     (501) staff       (20)     4471 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__exec.py
--rw-r--r--   0 yrobin     (501) staff       (20)    16235 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__extracvars.py
--rw-r--r--   0 yrobin     (501) staff       (20)      988 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__init__.py
--rw-r--r--   0 yrobin     (501) staff       (20)    14922 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__io.py
--rw-r--r--   0 yrobin     (501) staff       (20)     1983 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/__release.py
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-31 14:48:35.985525 CDSupdate-1.2.4/CDSupdate/data/
--rw-r--r--   0 yrobin     (501) staff       (20)      574 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-dptas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)     1918 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-name.csv
--rw-r--r--   0 yrobin     (501) staff       (20)     1572 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-pr-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      717 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-ps-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      830 2022-08-31 14:53:14.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-psl-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      858 2023-05-05 06:01:11.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-rlds-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)     1280 2023-05-05 06:01:11.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-rsds-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      380 2022-08-31 14:53:14.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-tas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      604 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-uas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      606 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-vas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      842 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/CDSupdate/data/ERA5-zg-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      737 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/CDSupdate/data/__init__.py
--rw-r--r--   0 yrobin     (501) staff       (20)      134 2023-05-03 06:31:49.000000 CDSupdate-1.2.4/CDSupdate/data/areas.csv
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-31 14:48:35.983009 CDSupdate-1.2.4/CDSupdate.egg-info/
--rw-r--r--   0 yrobin     (501) staff       (20)     2552 2023-05-31 14:48:35.000000 CDSupdate-1.2.4/CDSupdate.egg-info/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)      935 2023-05-31 14:48:35.000000 CDSupdate-1.2.4/CDSupdate.egg-info/SOURCES.txt
--rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-31 14:48:35.000000 CDSupdate-1.2.4/CDSupdate.egg-info/dependency_links.txt
--rw-r--r--   0 yrobin     (501) staff       (20)       42 2023-05-31 14:48:35.000000 CDSupdate-1.2.4/CDSupdate.egg-info/requires.txt
--rw-r--r--   0 yrobin     (501) staff       (20)       10 2023-05-31 14:48:35.000000 CDSupdate-1.2.4/CDSupdate.egg-info/top_level.txt
--rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-16 15:22:09.000000 CDSupdate-1.2.4/LICENSE
--rw-r--r--   0 yrobin     (501) staff       (20)       58 2022-08-31 14:53:14.000000 CDSupdate-1.2.4/MANIFEST.in
--rw-r--r--   0 yrobin     (501) staff       (20)     2552 2023-05-31 14:48:35.985859 CDSupdate-1.2.4/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)     1753 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/README.md
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-31 14:48:35.985681 CDSupdate-1.2.4/scripts/
--rwxr-xr-x   0 yrobin     (501) staff       (20)      894 2023-05-02 14:45:32.000000 CDSupdate-1.2.4/scripts/cdsupdate
--rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-31 14:48:35.986050 CDSupdate-1.2.4/setup.cfg
--rwxr-xr-x   0 yrobin     (501) staff       (20)     2431 2023-05-31 14:48:02.000000 CDSupdate-1.2.4/setup.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-07-25 14:59:24.868902 CDSupdate-1.2.5/
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-07-25 14:59:24.863992 CDSupdate-1.2.5/CDSupdate/
+-rw-r--r--   0 yrobin     (501) staff       (20)     9506 2023-05-31 14:48:02.000000 CDSupdate-1.2.5/CDSupdate/__CDSUParams.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     5145 2023-05-31 14:48:02.000000 CDSupdate-1.2.5/CDSupdate/__CVarsParams.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2685 2022-08-31 14:53:13.000000 CDSupdate-1.2.5/CDSupdate/__curses_doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     3744 2023-05-05 06:01:11.000000 CDSupdate-1.2.5/CDSupdate/__doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      969 2023-05-31 14:48:02.000000 CDSupdate-1.2.5/CDSupdate/__exceptions.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     4471 2023-05-31 14:48:02.000000 CDSupdate-1.2.5/CDSupdate/__exec.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    16235 2023-05-31 14:48:02.000000 CDSupdate-1.2.5/CDSupdate/__extracvars.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      988 2023-05-31 14:48:02.000000 CDSupdate-1.2.5/CDSupdate/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    14918 2023-07-25 14:56:42.000000 CDSupdate-1.2.5/CDSupdate/__io.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1983 2023-07-25 14:56:49.000000 CDSupdate-1.2.5/CDSupdate/__release.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-07-25 14:59:24.868120 CDSupdate-1.2.5/CDSupdate/data/
+-rw-r--r--   0 yrobin     (501) staff       (20)      574 2023-05-02 14:45:32.000000 CDSupdate-1.2.5/CDSupdate/data/ERA5-dptas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)     1918 2023-05-31 14:48:02.000000 CDSupdate-1.2.5/CDSupdate/data/ERA5-name.csv
+-rw-r--r--   0 yrobin     (501) staff       (20)     1572 2023-05-02 14:45:32.000000 CDSupdate-1.2.5/CDSupdate/data/ERA5-pr-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      717 2023-05-02 14:45:32.000000 CDSupdate-1.2.5/CDSupdate/data/ERA5-ps-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      830 2022-08-31 14:53:14.000000 CDSupdate-1.2.5/CDSupdate/data/ERA5-psl-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      858 2023-05-05 06:01:11.000000 CDSupdate-1.2.5/CDSupdate/data/ERA5-rlds-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)     1280 2023-05-05 06:01:11.000000 CDSupdate-1.2.5/CDSupdate/data/ERA5-rsds-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      380 2022-08-31 14:53:14.000000 CDSupdate-1.2.5/CDSupdate/data/ERA5-tas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      604 2023-05-02 14:45:32.000000 CDSupdate-1.2.5/CDSupdate/data/ERA5-uas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      606 2023-05-02 14:45:32.000000 CDSupdate-1.2.5/CDSupdate/data/ERA5-vas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      842 2023-05-02 14:45:32.000000 CDSupdate-1.2.5/CDSupdate/data/ERA5-zg-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      737 2023-05-31 14:48:02.000000 CDSupdate-1.2.5/CDSupdate/data/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      134 2023-05-03 06:31:49.000000 CDSupdate-1.2.5/CDSupdate/data/areas.csv
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-07-25 14:59:24.864784 CDSupdate-1.2.5/CDSupdate.egg-info/
+-rw-r--r--   0 yrobin     (501) staff       (20)     2552 2023-07-25 14:59:24.000000 CDSupdate-1.2.5/CDSupdate.egg-info/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)      935 2023-07-25 14:59:24.000000 CDSupdate-1.2.5/CDSupdate.egg-info/SOURCES.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-07-25 14:59:24.000000 CDSupdate-1.2.5/CDSupdate.egg-info/dependency_links.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)       42 2023-07-25 14:59:24.000000 CDSupdate-1.2.5/CDSupdate.egg-info/requires.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)       10 2023-07-25 14:59:24.000000 CDSupdate-1.2.5/CDSupdate.egg-info/top_level.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-16 15:22:09.000000 CDSupdate-1.2.5/LICENSE
+-rw-r--r--   0 yrobin     (501) staff       (20)       58 2022-08-31 14:53:14.000000 CDSupdate-1.2.5/MANIFEST.in
+-rw-r--r--   0 yrobin     (501) staff       (20)     2552 2023-07-25 14:59:24.868732 CDSupdate-1.2.5/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)     1753 2023-05-31 14:48:02.000000 CDSupdate-1.2.5/README.md
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-07-25 14:59:24.868481 CDSupdate-1.2.5/scripts/
+-rwxr-xr-x   0 yrobin     (501) staff       (20)      894 2023-05-02 14:45:32.000000 CDSupdate-1.2.5/scripts/cdsupdate
+-rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-07-25 14:59:24.868954 CDSupdate-1.2.5/setup.cfg
+-rwxr-xr-x   0 yrobin     (501) staff       (20)     2431 2023-05-31 14:48:02.000000 CDSupdate-1.2.5/setup.py
```

### Comparing `CDSupdate-1.2.4/CDSupdate/__CDSUParams.py` & `CDSupdate-1.2.5/CDSupdate/__CDSUParams.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/__CVarsParams.py` & `CDSupdate-1.2.5/CDSupdate/__CVarsParams.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/__curses_doc.py` & `CDSupdate-1.2.5/CDSupdate/__curses_doc.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/__doc.py` & `CDSupdate-1.2.5/CDSupdate/__doc.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/__exceptions.py` & `CDSupdate-1.2.5/CDSupdate/__exceptions.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/__exec.py` & `CDSupdate-1.2.5/CDSupdate/__exec.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/__extracvars.py` & `CDSupdate-1.2.5/CDSupdate/__extracvars.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/__init__.py` & `CDSupdate-1.2.5/CDSupdate/__init__.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/__io.py` & `CDSupdate-1.2.5/CDSupdate/__io.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,18 +408,18 @@
 					idata  = xr.concat( [idataN,idataO] , dim = "version" )
 					idata  = idata.sel( version = 1 ).combine_first( idata.sel( version = 0 ) ).compute()
 					del idataN
 					del idataO
 					os.remove( os.path.join( opath , ifileO ) )
 					
 					if freq == "hr":
-						t0    = str(idataN.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
-						t1    = str(idataN.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
+						t0    = str(idata.time[ 0].values)[:13].replace("-","").replace(" ","").replace("T","")
+						t1    = str(idata.time[-1].values)[:13].replace("-","").replace(" ","").replace("T","")
 					else:
-						t0    = str(idataN.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
-						t1    = str(idataN.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
+						t0    = str(idata.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
+						t1    = str(idata.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
 					ofile  = f"ERA5_{cvar}_{freq}_{area_name}_{t0}-{t1}.nc"
 					logger.info( f" * Save '{ofile}'" )
 					save_netcdf( idata , cvar , freq , os.path.join( opath , ofile ) )
 ##}}}
```

### Comparing `CDSupdate-1.2.4/CDSupdate/__release.py` & `CDSupdate-1.2.5/CDSupdate/__release.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ## 
 ## You should have received a copy of the GNU General Public License
 ## along with CDSupdate.  If not, see <https://www.gnu.org/licenses/>.
 
 
 version_major = "1"
 version_minor = "2"
-version_patch = "4"
+version_patch = "5"
 version_extra = ""
 version       = f"{version_major}.{version_minor}.{version_patch}{version_extra}"
 
 name = "CDSupdate"
 
 description = "Auto-updater of data from the Climate Data Store"
```

### Comparing `CDSupdate-1.2.4/CDSupdate/data/ERA5-dptas-description.txt` & `CDSupdate-1.2.5/CDSupdate/data/ERA5-dptas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/data/ERA5-name.csv` & `CDSupdate-1.2.5/CDSupdate/data/ERA5-name.csv`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/data/ERA5-pr-description.txt` & `CDSupdate-1.2.5/CDSupdate/data/ERA5-pr-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/data/ERA5-ps-description.txt` & `CDSupdate-1.2.5/CDSupdate/data/ERA5-ps-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/data/ERA5-psl-description.txt` & `CDSupdate-1.2.5/CDSupdate/data/ERA5-psl-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/data/ERA5-rlds-description.txt` & `CDSupdate-1.2.5/CDSupdate/data/ERA5-rlds-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/data/ERA5-rsds-description.txt` & `CDSupdate-1.2.5/CDSupdate/data/ERA5-rsds-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/data/ERA5-uas-description.txt` & `CDSupdate-1.2.5/CDSupdate/data/ERA5-uas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/data/ERA5-vas-description.txt` & `CDSupdate-1.2.5/CDSupdate/data/ERA5-vas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/data/ERA5-zg-description.txt` & `CDSupdate-1.2.5/CDSupdate/data/ERA5-zg-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate/data/__init__.py` & `CDSupdate-1.2.5/CDSupdate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/CDSupdate.egg-info/PKG-INFO` & `CDSupdate-1.2.5/CDSupdate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CDSupdate
-Version: 1.2.4
+Version: 1.2.5
 Summary: Auto-updater of data from the Climate Data Store
 Home-page: https://github.com/yrobink/CDSupdate
 Author: Yoann Robin, Andreia Hisi
 Author-email: yoann.robin.k@gmail.com, andreia.hisi@lsce.ipsl.fr
 License: GNU-GPL3
 Keywords: Climate Data Store,Auto update
 Platform: linux
```

### Comparing `CDSupdate-1.2.4/CDSupdate.egg-info/SOURCES.txt` & `CDSupdate-1.2.5/CDSupdate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/LICENSE` & `CDSupdate-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/PKG-INFO` & `CDSupdate-1.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CDSupdate
-Version: 1.2.4
+Version: 1.2.5
 Summary: Auto-updater of data from the Climate Data Store
 Home-page: https://github.com/yrobink/CDSupdate
 Author: Yoann Robin, Andreia Hisi
 Author-email: yoann.robin.k@gmail.com, andreia.hisi@lsce.ipsl.fr
 License: GNU-GPL3
 Keywords: Climate Data Store,Auto update
 Platform: linux
```

### Comparing `CDSupdate-1.2.4/README.md` & `CDSupdate-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/scripts/cdsupdate` & `CDSupdate-1.2.5/scripts/cdsupdate`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.2.4/setup.py` & `CDSupdate-1.2.5/setup.py`

 * *Files identical despite different names*

