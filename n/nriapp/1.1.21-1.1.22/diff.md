# Comparing `tmp/nriapp-1.1.21.tar.gz` & `tmp/nriapp-1.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nriapp-1.1.21.tar", last modified: Sat Jul 15 01:38:45 2023, max compression
+gzip compressed data, was "nriapp-1.1.22.tar", last modified: Tue Jul 25 17:49:48 2023, max compression
```

## Comparing `nriapp-1.1.21.tar` & `nriapp-1.1.22.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.206638 nriapp-1.1.21/
--rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.21/LICENSE
--rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.21/MANIFEST.in
--rw-rw-rw-   0        0        0      273 2023-07-15 01:38:45.206638 nriapp-1.1.21/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.21/README
--rw-rw-rw-   0        0        0      344 2023-05-06 05:28:38.000000 nriapp-1.1.21/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-07-15 01:38:45.237838 nriapp-1.1.21/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-07-15 01:38:31.000000 nriapp-1.1.21/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 01:38:44.941438 nriapp-1.1.21/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.003838 nriapp-1.1.21/src/nriapp/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.21/src/nriapp/changelog.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.050638 nriapp-1.1.21/src/nriapp/config/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/config/__init__.py
--rw-rw-rw-   0        0        0       55 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/config/config.py
-drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.128638 nriapp-1.1.21/src/nriapp/core/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/core/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/core/abuseipdbapi.py
--rw-rw-rw-   0        0        0    20773 2023-06-29 05:06:20.000000 nriapp-1.1.21/src/nriapp/core/dataexplorer.py
--rw-rw-rw-   0        0        0    30995 2023-06-21 05:47:59.000000 nriapp-1.1.21/src/nriapp/core/msgraphapi.py
--rw-rw-rw-   0        0        0   105842 2023-06-30 05:29:02.000000 nriapp-1.1.21/src/nriapp/core/mssentinelapi.py
--rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/core/multifactor.py
--rw-rw-rw-   0        0        0      640 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/core/vtquery.py
-drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.206638 nriapp-1.1.21/src/nriapp/helper/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/__init__.py
--rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/doc.py
--rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/excel.py
--rw-rw-rw-   0        0        0     8397 2023-07-12 23:43:13.000000 nriapp-1.1.21/src/nriapp/helper/login.py
--rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/pylog.py
--rw-rw-rw-   0        0        0     1247 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/requestheader.py
--rw-rw-rw-   0        0        0    15815 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.003838 nriapp-1.1.21/src/nriapp/nriapp.egg-info/
--rw-rw-rw-   0        0        0      273 2023-07-15 01:38:44.000000 nriapp-1.1.21/src/nriapp/nriapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2023-07-15 01:38:44.000000 nriapp-1.1.21/src/nriapp/nriapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 01:38:44.000000 nriapp-1.1.21/src/nriapp/nriapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-15 01:38:44.000000 nriapp-1.1.21/src/nriapp/nriapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-15 01:38:44.000000 nriapp-1.1.21/src/nriapp/nriapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    38177 2023-06-12 22:38:37.000000 nriapp-1.1.21/src/nriapp/nriapp.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:49:48.128498 nriapp-1.1.22/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.22/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.22/MANIFEST.in
+-rw-rw-rw-   0        0        0      304 2023-07-25 17:49:48.128498 nriapp-1.1.22/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.22/README
+-rw-rw-rw-   0        0        0      344 2023-05-06 05:28:38.000000 nriapp-1.1.22/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-07-25 17:49:48.128498 nriapp-1.1.22/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2023-07-25 17:49:37.000000 nriapp-1.1.22/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:49:48.088498 nriapp-1.1.22/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 17:49:48.108498 nriapp-1.1.22/src/nriapp/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.22/src/nriapp/__init__.py
+-rw-rw-rw-   0        0        0     4253 2023-07-25 17:48:32.000000 nriapp-1.1.22/src/nriapp/changelog.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 17:49:48.118498 nriapp-1.1.22/src/nriapp/config/
+-rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.22/src/nriapp/config/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.22/src/nriapp/config/config.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:49:48.118498 nriapp-1.1.22/src/nriapp/core/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.1.22/src/nriapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1520 2023-04-19 13:47:32.000000 nriapp-1.1.22/src/nriapp/core/abuseipdbapi.py
+-rw-rw-rw-   0        0        0    20773 2023-06-29 05:06:20.000000 nriapp-1.1.22/src/nriapp/core/dataexplorer.py
+-rw-rw-rw-   0        0        0    30995 2023-06-21 05:47:59.000000 nriapp-1.1.22/src/nriapp/core/msgraphapi.py
+-rw-rw-rw-   0        0        0   106112 2023-07-25 17:38:23.000000 nriapp-1.1.22/src/nriapp/core/mssentinelapi.py
+-rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.22/src/nriapp/core/multifactor.py
+-rw-rw-rw-   0        0        0      640 2023-04-19 13:47:32.000000 nriapp-1.1.22/src/nriapp/core/vtquery.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:49:48.128498 nriapp-1.1.22/src/nriapp/helper/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.22/src/nriapp/helper/__init__.py
+-rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.22/src/nriapp/helper/doc.py
+-rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.1.22/src/nriapp/helper/excel.py
+-rw-rw-rw-   0        0        0     8397 2023-07-12 23:43:13.000000 nriapp-1.1.22/src/nriapp/helper/login.py
+-rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.1.22/src/nriapp/helper/pylog.py
+-rw-rw-rw-   0        0        0     1247 2023-04-19 13:47:32.000000 nriapp-1.1.22/src/nriapp/helper/requestheader.py
+-rw-rw-rw-   0        0        0    15815 2023-04-19 13:47:32.000000 nriapp-1.1.22/src/nriapp/helper/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 17:49:48.108498 nriapp-1.1.22/src/nriapp/nriapp.egg-info/
+-rw-rw-rw-   0        0        0      304 2023-07-25 17:49:47.000000 nriapp-1.1.22/src/nriapp/nriapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-07-25 17:49:47.000000 nriapp-1.1.22/src/nriapp/nriapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 17:49:47.000000 nriapp-1.1.22/src/nriapp/nriapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-25 17:49:47.000000 nriapp-1.1.22/src/nriapp/nriapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-25 17:49:47.000000 nriapp-1.1.22/src/nriapp/nriapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    38173 2023-07-25 16:19:54.000000 nriapp-1.1.22/src/nriapp/nriapp.py
```

### Comparing `nriapp-1.1.21/LICENSE` & `nriapp-1.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.21/setup.py` & `nriapp-1.1.22/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 #with open('requirements.txt') as f:
 #    requirements = f.read().splitlines()
 
 
 setup(
    name='nriapp',
-   version='1.1.21',
-   description='This is an internal tool for crawling MS 365 Defender web with NRI',
+   version='1.1.22',
+   description='This is an internal tool for querying MS 365 Defender using MSGraph and MS Sentinels API with NRI',
     license='MIT',
    author='Llallum Victoria',
    author_email='llallumvictoria@gmail.com',
 #   packages=find_packages('src'),
    package_dir = {'':'src/nriapp'},
     
    packages=['.','config', 'core', 'helper'],  #same as name
```

### Comparing `nriapp-1.1.21/src/nriapp/changelog.txt` & `nriapp-1.1.22/src/nriapp/changelog.txt`

 * *Files 15% similar despite different names*

```diff
@@ -70,14 +70,18 @@
 	- Switched from PyLog to loguru (Open source logging)
 	- Fixes MSGraph
 
 1/27/2023 5:00:48 PM
 	- Fixes MSGraph request with new update on MS 
 	- api/DelegationToken
 
+7/26/2023 
+	- Defender made a major changes in terms of querying the page size of incidents that you can query. 
+	- Before, the maximum number of pagesize is 3000, but now, it is now limited to 50 which makes all the features on querying incidents won't work.	
+	- Fixed in 1.1.22
 
     #10457 -cve 
     #10416 - 7zip 
     #10400-process 
     #10437 zip 
     #6451  ransomware
     #10450 email 
@@ -95,8 +99,25 @@
     #10594 - Skinprogress
     #8642 - Multi-stage incident involving Initial access & Credential access on one endpoint reported by multiple sources
     #8745 - 
     #9613
 	#9985   A user clicked through to a potentially malicious URL​ (No URL)
 
 2/2/2023 8:29:27 AM
-	#12107 Error
+	#12107 Error
+
+3/3/2023 1:43:50 AM
+	Fixed Device Owner where the principal name outputs the admin who enrolls.
+	Includes the Verdict too.
+
+This is  a tmp branch.
+This is an update from tmp branch.
+
+This is for tmp branch only.
+
+This is for mybranch.
+
+Mybranch only.
+
+MyBranch.
+
+My branch Only.
```

### Comparing `nriapp-1.1.21/src/nriapp/core/abuseipdbapi.py` & `nriapp-1.1.22/src/nriapp/core/abuseipdbapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.21/src/nriapp/core/dataexplorer.py` & `nriapp-1.1.22/src/nriapp/core/dataexplorer.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.21/src/nriapp/core/msgraphapi.py` & `nriapp-1.1.22/src/nriapp/core/msgraphapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.21/src/nriapp/core/mssentinelapi.py` & `nriapp-1.1.22/src/nriapp/core/mssentinelapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                     elif response.status_code == 504:
                         dbgPrint.error("Gateway Time-out")
                         sys.exit()      
             except:
                 continue
         return response
 
-    def get_incidents(self, incidentId = [], alertStatus=['New','InProgress', 'Resolved'], severity=[256, 128, 64, 32], pageIndex= 1, lookBackInDays = 60, pageSize = 3000, sourceFilter=[], titleFilter=[], incident_list=[]):
+    def get_incidents(self, incidentId = [], alertStatus=['New','InProgress', 'Resolved'], severity=[256, 128, 64, 32], pageIndex= 1, lookBackInDays = 60, pageSize = 50, sourceFilter=[], titleFilter=[], incident_list=[]):  #July 25, 2023 Changed the PageSize. It seems like the Defender changed the limit from 3000 to 0-50 only.
 
         incident_alerts = 'https://security.microsoft.com/apiproxy/mtp/incidentQueue/incidents/alerts'
         json_data = {
             'pageSize': pageSize,
             'lookBackInDays': str(lookBackInDays),
             'isMultipleIncidents': True,
             'alertStatus': alertStatus,
@@ -136,19 +136,22 @@
             'pageIndex': pageIndex,
             }
         response = self.tryrequest(incident_alerts, json=json_data)
         while(response.status_code != 200):
             if response.status_code == 440:
                 self.load_session()
                 response = self.tryrequest(incident_alerts, json=json_data)
+            elif response.status_code == 400:
+                dbgPrint.error("Error 400: " + response.text)
+                raise("Error 400: ", response.text)
 
         incident_list.extend(json.loads(response.text))
 
         if len(json.loads(response.text)) == pageSize:
-            self.get_incidents(incidentId,pageIndex=pageIndex+1,lookBackInDays = 180, pageSize = 3000, incident_list=incident_list)
+            self.get_incidents(incidentId,pageIndex=pageIndex+1,lookBackInDays = 180, pageSize=pageSize, incident_list=incident_list)
         else:
             incident_list.extend(json.loads(response.text))
 
         return incident_list
```

### Comparing `nriapp-1.1.21/src/nriapp/core/multifactor.py` & `nriapp-1.1.22/src/nriapp/core/multifactor.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.21/src/nriapp/core/vtquery.py` & `nriapp-1.1.22/src/nriapp/core/vtquery.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.21/src/nriapp/helper/doc.py` & `nriapp-1.1.22/src/nriapp/helper/doc.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.21/src/nriapp/helper/login.py` & `nriapp-1.1.22/src/nriapp/helper/login.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.21/src/nriapp/helper/pylog.py` & `nriapp-1.1.22/src/nriapp/helper/pylog.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.21/src/nriapp/helper/requestheader.py` & `nriapp-1.1.22/src/nriapp/helper/requestheader.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.21/src/nriapp/helper/utils.py` & `nriapp-1.1.22/src/nriapp/helper/utils.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.21/src/nriapp/nriapp.egg-info/SOURCES.txt` & `nriapp-1.1.22/src/nriapp/nriapp.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -24,12 +24,8 @@
 src/nriapp/helper/__init__.py
 src/nriapp/helper/doc.py
 src/nriapp/helper/excel.py
 src/nriapp/helper/login.py
 src/nriapp/helper/pylog.py
 src/nriapp/helper/requestheader.py
 src/nriapp/helper/utils.py
-src/nriapp/nriapp.egg-info/PKG-INFO
-src/nriapp/nriapp.egg-info/SOURCES.txt
-src/nriapp/nriapp.egg-info/dependency_links.txt
-src/nriapp/nriapp.egg-info/entry_points.txt
-src/nriapp/nriapp.egg-info/top_level.txt
+src/nriapp/nriapp.egg-info/SOURCES.txt
```

### Comparing `nriapp-1.1.21/src/nriapp/nriapp.py` & `nriapp-1.1.22/src/nriapp/nriapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,15 +518,15 @@
 
             dbgPrint.debug("Fetching incidents data")
             incidents = self.sentinel.get_incidents(incidentId=0, 
                                                     alertStatus=['New','InProgress', 'Resolved'] , 
                                                     severity=[256,128,64,32], 
                                                     pageIndex=1, 
                                                     lookBackInDays=lookBackInDays, 
-                                                    pageSize=3000, 
+                                                    pageSize=50, 
                                                     ) #sourceFilter=[16384, 1048576], titleFilter=["eDiscovery"]      #16384 == MCAS incidents 512 = eDiscovery
             dbgPrint.debug("Ingesting data")
             audit = dataexplorer.ingest_events(data=incidents)
             dbgPrint.debug("Fetching audit logs of incidents")
 
             audit_logs = self.sentinel.get_all_audit_logs(audit)
             dbgPrint.debug("Ingesting data")
@@ -640,15 +640,15 @@
 
         all_data = {}        
         incident_list = self.sentinel.get_incidents(incidentId=id, 
                                                 alertStatus=['New','InProgress', 'Resolved'] , 
                                                 severity=[256,128,64,32], 
                                                 pageIndex=1, 
                                                 lookBackInDays=lookBackInDays, 
-                                                pageSize=3000, 
+                                                pageSize=50, 
                                                 sourceFilter=[16384, 1048576], titleFilter=["eDiscovery"])       #16384 == MCAS incidents 512 = eDiscovery
         if id:
             incidents = []
             for a in id:
                 incident = [i for i in incident_list if i["IncidentId"] == a]
                 if incident:
                     incidents.append(incident[0])
```

