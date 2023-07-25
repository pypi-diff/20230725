# Comparing `tmp/epmwebapi-1.8.74.tar.gz` & `tmp/epmwebapi-1.8.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\epmwebapi-1.8.74.tar", last modified: Mon Apr 17 17:05:34 2023, max compression
+gzip compressed data, was "dist\epmwebapi-1.8.84.tar", last modified: Tue Jul 25 21:05:24 2023, max compression
```

## Comparing `epmwebapi-1.8.74.tar` & `epmwebapi-1.8.84.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/
-drwxrwxrwx   0        0        0        0 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/epmwebapi/
--rw-rw-rw-   0        0        0     5663 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/aggregatedetails.py
--rw-rw-rw-   0        0        0     1160 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/annotationvaluejson.py
--rw-rw-rw-   0        0        0     6391 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/authorizationservice.py
--rw-rw-rw-   0        0        0      677 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/autostarttimer.py
--rw-rw-rw-   0        0        0    17437 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/basicvariable.py
--rw-rw-rw-   0        0        0      655 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/basicvariablepropertymask.py
--rw-rw-rw-   0        0        0      236 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/browsedirection.py
--rw-rw-rw-   0        0        0      892 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/browseitemmodeljson.py
--rw-rw-rw-   0        0        0      580 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/browsemodeljson.py
--rw-rw-rw-   0        0        0      493 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/browseresultitemmodeljson.py
--rw-rw-rw-   0        0        0      541 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/browseresultmodeljson.py
--rw-rw-rw-   0        0        0    10872 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/customtypedefinition.py
--rw-rw-rw-   0        0        0      490 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/dataobjectattributes.py
--rw-rw-rw-   0        0        0     1149 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/dataobjectsfilter.py
--rw-rw-rw-   0        0        0    22528 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/datasetconfig.py
--rw-rw-rw-   0        0        0    12946 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/datasetpen.py
--rw-rw-rw-   0        0        0     1522 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/datavaluejson.py
--rw-rw-rw-   0        0        0      395 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/diagnosticmodeljson.py
-drwxrwxrwx   0        0        0        0 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/epmwebapi/dll_references/
--rw-rw-rw-   0        0        0   103424 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/dll_references/Elipse.Epm.AddressSpaceModel.dll
--rw-rw-rw-   0        0        0   419328 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/dll_references/EpmData.dll
--rw-rw-rw-   0        0        0      317 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/domainfilter.py
--rw-rw-rw-   0        0        0      327 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/downloadtype.py
--rw-rw-rw-   0        0        0    87052 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmconnection.py
--rw-rw-rw-   0        0        0     3567 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmconnectioncontext.py
--rw-rw-rw-   0        0        0    11086 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmdataobject.py
--rw-rw-rw-   0        0        0     1932 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmmodelobject.py
--rw-rw-rw-   0        0        0      545 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmnodeids.py
--rw-rw-rw-   0        0        0     2411 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmobject.py
--rw-rw-rw-   0        0        0      553 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmproperty.py
--rw-rw-rw-   0        0        0     3503 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmutils.py
--rw-rw-rw-   0        0        0     2829 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmvariable.py
--rw-rw-rw-   0        0        0      200 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/epmwebapi.py
--rw-rw-rw-   0        0        0     1039 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/folder.py
--rw-rw-rw-   0        0        0      985 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyprocessedmodeljson.py
--rw-rw-rw-   0        0        0      834 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyrawmodeljson.py
--rw-rw-rw-   0        0        0      434 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyresultitemmodeljson.py
--rw-rw-rw-   0        0        0      412 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyresultmodeljson.py
--rw-rw-rw-   0        0        0      875 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyupdatedataitemmodeljson.py
--rw-rw-rw-   0        0        0      518 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyupdatedatamodeljson.py
--rw-rw-rw-   0        0        0      436 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyupdateresultmodeljson.py
--rw-rw-rw-   0        0        0      338 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/historyupdatetype.py
--rw-rw-rw-   0        0        0      608 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/itempathandcontinuationpointjson.py
--rw-rw-rw-   0        0        0      913 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/itempathjson.py
--rw-rw-rw-   0        0        0     3869 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/mimetype.py
--rw-rw-rw-   0        0        0     2861 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/nodeattributes.py
--rw-rw-rw-   0        0        0     1092 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/nodeclassmask.py
--rw-rw-rw-   0        0        0     5363 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/numpyextras.py
--rw-rw-rw-   0        0        0      336 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/performupdatetype.py
--rw-rw-rw-   0        0        0      430 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/portalresources.py
--rw-rw-rw-   0        0        0      433 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/processorresources.py
--rw-rw-rw-   0        0        0     1281 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/querymodeljson.py
--rw-rw-rw-   0        0        0      639 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/queryperiod.py
--rw-rw-rw-   0        0        0      444 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/queryresultitemmodeljson.py
--rw-rw-rw-   0        0        0      371 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/queryresultmask.py
--rw-rw-rw-   0        0        0      741 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/queryresultmodeljson.py
--rw-rw-rw-   0        0        0      467 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/readitemmodeljson.py
--rw-rw-rw-   0        0        0      558 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/readmodeljson.py
--rw-rw-rw-   0        0        0      475 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/readresultitemmodeljson.py
--rw-rw-rw-   0        0        0      535 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/readresultmodeljson.py
--rw-rw-rw-   0        0        0      792 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/resource.py
--rw-rw-rw-   0        0        0     8938 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/resourcesmanager.py
--rw-rw-rw-   0        0        0    30888 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/statuscodes.py
--rw-rw-rw-   0        0        0      545 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/writeitemmodeljson.py
--rw-rw-rw-   0        0        0      444 2023-04-17 16:51:46.000000 epmwebapi-1.8.74/epmwebapi/writemodeljson.py
--rw-rw-rw-   0        0        0       24 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/_version.py
--rw-rw-rw-   0        0        0     1793 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/epmwebapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/epmwebapi.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-17 17:05:33.000000 epmwebapi-1.8.74/epmwebapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4768 2023-04-17 17:05:33.000000 epmwebapi-1.8.74/epmwebapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-04-17 17:05:33.000000 epmwebapi-1.8.74/epmwebapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0     2229 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/epmwebapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 17:05:33.000000 epmwebapi-1.8.74/epmwebapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/LICENSE.txt
--rw-rw-rw-   0        0        0     4768 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/PKG-INFO
--rw-rw-rw-   0        0        0     3752 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/Readme.md
--rw-rw-rw-   0        0        0      114 2023-04-17 17:05:34.000000 epmwebapi-1.8.74/setup.cfg
--rw-rw-rw-   0        0        0     1497 2023-04-17 16:51:45.000000 epmwebapi-1.8.74/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:05:24.000000 epmwebapi-1.8.84/
+drwxrwxrwx   0        0        0        0 2023-07-25 21:05:24.000000 epmwebapi-1.8.84/epmwebapi/
+-rw-rw-rw-   0        0        0     5663 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/aggregatedetails.py
+-rw-rw-rw-   0        0        0     1160 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/annotationvaluejson.py
+-rw-rw-rw-   0        0        0     7348 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/authorizationservice.py
+-rw-rw-rw-   0        0        0      677 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/autostarttimer.py
+-rw-rw-rw-   0        0        0    17437 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/basicvariable.py
+-rw-rw-rw-   0        0        0      655 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/basicvariablepropertymask.py
+-rw-rw-rw-   0        0        0      236 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/browsedirection.py
+-rw-rw-rw-   0        0        0      892 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/browseitemmodeljson.py
+-rw-rw-rw-   0        0        0      580 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/browsemodeljson.py
+-rw-rw-rw-   0        0        0      493 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/browseresultitemmodeljson.py
+-rw-rw-rw-   0        0        0      541 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/browseresultmodeljson.py
+-rw-rw-rw-   0        0        0    10872 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/customtypedefinition.py
+-rw-rw-rw-   0        0        0      490 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/dataobjectattributes.py
+-rw-rw-rw-   0        0        0     1149 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/dataobjectsfilter.py
+-rw-rw-rw-   0        0        0    22528 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/datasetconfig.py
+-rw-rw-rw-   0        0        0    12946 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/datasetpen.py
+-rw-rw-rw-   0        0        0     1522 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/datavaluejson.py
+-rw-rw-rw-   0        0        0      395 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/diagnosticmodeljson.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:05:24.000000 epmwebapi-1.8.84/epmwebapi/dll_references/
+-rw-rw-rw-   0        0        0   103424 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/dll_references/Elipse.Epm.AddressSpaceModel.dll
+-rw-rw-rw-   0        0        0   419328 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/dll_references/EpmData.dll
+-rw-rw-rw-   0        0        0      317 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/domainfilter.py
+-rw-rw-rw-   0        0        0      327 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/downloadtype.py
+-rw-rw-rw-   0        0        0    89276 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/epmconnection.py
+-rw-rw-rw-   0        0        0     3237 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/epmconnectioncontext.py
+-rw-rw-rw-   0        0        0    11086 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/epmdataobject.py
+-rw-rw-rw-   0        0        0     1932 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/epmmodelobject.py
+-rw-rw-rw-   0        0        0      545 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/epmnodeids.py
+-rw-rw-rw-   0        0        0     2603 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/epmobject.py
+-rw-rw-rw-   0        0        0      553 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/epmproperty.py
+-rw-rw-rw-   0        0        0     1836 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/epmsession.py
+-rw-rw-rw-   0        0        0     3503 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/epmutils.py
+-rw-rw-rw-   0        0        0     2829 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/epmvariable.py
+-rw-rw-rw-   0        0        0      200 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/epmwebapi.py
+-rw-rw-rw-   0        0        0     1039 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/folder.py
+-rw-rw-rw-   0        0        0      985 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/historyprocessedmodeljson.py
+-rw-rw-rw-   0        0        0      834 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/historyrawmodeljson.py
+-rw-rw-rw-   0        0        0      434 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/historyresultitemmodeljson.py
+-rw-rw-rw-   0        0        0      412 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/historyresultmodeljson.py
+-rw-rw-rw-   0        0        0      875 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/historyupdatedataitemmodeljson.py
+-rw-rw-rw-   0        0        0      518 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/historyupdatedatamodeljson.py
+-rw-rw-rw-   0        0        0      436 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/historyupdateresultmodeljson.py
+-rw-rw-rw-   0        0        0      338 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/historyupdatetype.py
+-rw-rw-rw-   0        0        0      608 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/itempathandcontinuationpointjson.py
+-rw-rw-rw-   0        0        0      913 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/itempathjson.py
+-rw-rw-rw-   0        0        0     3869 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/mimetype.py
+-rw-rw-rw-   0        0        0     2861 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/nodeattributes.py
+-rw-rw-rw-   0        0        0     1092 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/nodeclassmask.py
+-rw-rw-rw-   0        0        0     5363 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/numpyextras.py
+-rw-rw-rw-   0        0        0      336 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/performupdatetype.py
+-rw-rw-rw-   0        0        0      430 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/portalresources.py
+-rw-rw-rw-   0        0        0      433 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/processorresources.py
+-rw-rw-rw-   0        0        0     1281 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/querymodeljson.py
+-rw-rw-rw-   0        0        0      639 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/queryperiod.py
+-rw-rw-rw-   0        0        0      444 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/queryresultitemmodeljson.py
+-rw-rw-rw-   0        0        0      371 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/queryresultmask.py
+-rw-rw-rw-   0        0        0      741 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/queryresultmodeljson.py
+-rw-rw-rw-   0        0        0      467 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/readitemmodeljson.py
+-rw-rw-rw-   0        0        0      558 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/readmodeljson.py
+-rw-rw-rw-   0        0        0      475 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/readresultitemmodeljson.py
+-rw-rw-rw-   0        0        0      535 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/readresultmodeljson.py
+-rw-rw-rw-   0        0        0      792 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/resource.py
+-rw-rw-rw-   0        0        0     8938 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/resourcesmanager.py
+-rw-rw-rw-   0        0        0    30888 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/statuscodes.py
+-rw-rw-rw-   0        0        0      545 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/writeitemmodeljson.py
+-rw-rw-rw-   0        0        0      444 2023-07-25 20:50:55.000000 epmwebapi-1.8.84/epmwebapi/writemodeljson.py
+-rw-rw-rw-   0        0        0       24 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/_version.py
+-rw-rw-rw-   0        0        0     1793 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/epmwebapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:05:24.000000 epmwebapi-1.8.84/epmwebapi.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-25 21:05:24.000000 epmwebapi-1.8.84/epmwebapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4768 2023-07-25 21:05:24.000000 epmwebapi-1.8.84/epmwebapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-07-25 21:05:24.000000 epmwebapi-1.8.84/epmwebapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     2253 2023-07-25 21:05:24.000000 epmwebapi-1.8.84/epmwebapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 21:05:24.000000 epmwebapi-1.8.84/epmwebapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/LICENSE.txt
+-rw-rw-rw-   0        0        0     4768 2023-07-25 21:05:24.000000 epmwebapi-1.8.84/PKG-INFO
+-rw-rw-rw-   0        0        0     3752 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/Readme.md
+-rw-rw-rw-   0        0        0      114 2023-07-25 21:05:24.000000 epmwebapi-1.8.84/setup.cfg
+-rw-rw-rw-   0        0        0     1497 2023-07-25 20:50:54.000000 epmwebapi-1.8.84/setup.py
```

### Comparing `epmwebapi-1.8.74/epmwebapi/aggregatedetails.py` & `epmwebapi-1.8.84/epmwebapi/aggregatedetails.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/annotationvaluejson.py` & `epmwebapi-1.8.84/epmwebapi/annotationvaluejson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/authorizationservice.py` & `epmwebapi-1.8.84/epmwebapi/authorizationservice.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,171 +10,197 @@
 import json
 from .autostarttimer import AutoStartTimer
 
 from .epmconnectioncontext import EpmConnectionContext
 
 class AuthorizationService(object):
 
-  def __init__(self, connectionContext, forceConnection = True):
+  def __init__(self, connectionContext:EpmConnectionContext, forceConnection = True):
     import copy
     self._context = copy.deepcopy(connectionContext)
-    self._context += self.changedToken
     self._error = ''
     self._expireIn = 0
     self._session = None
-    self._timer = None
-    if forceConnection:
-      self._context.setToken(self.renewToken())
-      self._timer = AutoStartTimer(60, self.reloadToken)
+    if self._context.hasToken():
+      self.changedToken(self._context.getToken())
 
   def reloadToken(self):
     try:
-      self._context.setToken(self.renewToken())
+      token = self.renewToken()
+      self._context.setToken(token)
+      self.changedToken(token)
       self._error = ''
     except Exception as ex:
-      self._context.setToken('')
+      self._context.setToken(None)
       self._error = str(ex)
+      raise
     
   def renewToken(self):
     from datetime import datetime, timedelta
 
     import logging
     try:
       if (self._context.hasToken()):
        return self.refreshToken()
+    except TokenOldException:
+      logging.info('The token is old and were closed! Trying to create a new one.')
     except Exception as ex:
-      logging.error('Refresh failed! Trying to connect again. Error: ' + str(ex))
+      import traceback
+      details = traceback.format_exc()
+      logging.error('Refresh failed! Trying to connect again. Error: ' + str(ex) + '. Details: ' + details)
 
     client_auth = requests.auth.HTTPBasicAuth(self._context.getClientId(), self._context.getProgramId())
     post_data = {"grant_type": "password", 
                   "username": self._context.getUserName(),
                   "password": self._context.getPassword(),
                   "scope": "offline_access openid profile email opcua_browse opcua_read opcua_write opcua_subscription opcua_history EpmWebApi portal_files portal_upload"} #EpmProcessor #openid profile email opcua_browse opcua_read opcua_subscription 
     auth_url = self._context.getAuthServer() + '/connect/token'
 
-    session = self.getSession()
+    session = self._getSession()
     response = session.post(auth_url,
                              auth=client_auth,
                              data=post_data, verify=False)
     respose_json = response.json()
 
     if response.status_code != 200:
         raise Exception("GetToken() call http error '" +  str(response.status_code) + "'. Reason: " + respose_json["error"])
     
-    self._expireIn = respose_json["expires_in"]
+    expireIn = respose_json["expires_in"]
+    if expireIn is None or expireIn < 60 or expireIn > 180:
+      expireIn = 180
+
+    self._expireIn = expireIn
 
     from datetime import datetime, timedelta
     self._context.setExpiration(datetime.utcnow() + timedelta(seconds=self._expireIn))
     self._context.setRefreshToken(respose_json["refresh_token"])
 
     return respose_json["access_token"]
 
   def changedToken(self, token):
-    session = self.getSession()
+    session = self._getSession()
     if token != None:
       header = {'Authorization': 'Bearer {}'.format(token)}
       session.headers.update(header)
     else:
       header = {}
       session.headers.update(header)
 
+  def getContext(self) -> EpmConnectionContext:
+    return self._context
+
   def getToken(self):
     if self._error == '':
       return self._context.getToken()
     else:
       raise Exception(self._error)
 
-  def getSession(self):
+  def getEpmSession(self):
+    from .epmsession import EpmSession
+    return EpmSession(self)
+
+  def _getSession(self):
     if self._session == None:
       self._session = requests.session()
     return self._session
 
   def refreshToken(self):
 
     import logging
     from datetime import datetime, timedelta
     # agora sempre faz um refresh pra verificar a conexão
     #if (self._tokenExpiration != None and self._tokenExpiration  > (datetime.utcnow() + timedelta(seconds=60))):
     #  return self._token
     if (self._context.hasExpiration() and self._context.getExpiration() < (datetime.utcnow() + timedelta(seconds=30))):
       # tenta fechar o token
-      self.close()
-      raise Exception('refresh Token expired!') 
+      logging.debug('Token is old. Logging out to create a new one.')
+      self.logout()
+      raise TokenOldException()
 
     client_auth = requests.auth.HTTPBasicAuth(self._context.getClientId(), self._context.getProgramId())
     post_data = {"grant_type": "refresh_token", 
-                 "refresh_token": "%s"%(self._context.getRefreshToken()) }
+                 "refresh_token": "%s"%(str(self._context.getRefreshToken())) }
     auth_url = self._context.getAuthServer() + '/connect/token'
 
-    session = self.getSession()
+    session = self._getSession()
     response = session.post(auth_url,
                               auth=client_auth,
                               data=post_data, verify=False) 
     respose_json = response.json()
 
     if response.status_code != 200:
       raise Exception("RefreshToken() call http error '" +  str(response.status_code) + "'.")
 
     from datetime import datetime, timedelta
 
     expireIn = self._expireIn
-    if expireIn is None or expireIn < 60:
-      expireIn = 300
+    if expireIn is None or expireIn < 60 or expireIn > 180:
+      expireIn = 180
 
     self._context.setRefreshToken(respose_json["refresh_token"])
     self._context.setExpiration(datetime.utcnow() + timedelta(seconds=expireIn))
 
     return respose_json["access_token"]
 
   def logout(self):
     if (not self._context.hasToken()):
       return
-    post_data = { "token" : self._context.getToken() }
-    client_auth = requests.auth.HTTPBasicAuth(self._context.getClientId(), self._context.getProgramId())
-    auth_url = self._context.getAuthServer() + '/connect/revocation'
-    session = self.getSession()
-    response = session.post(auth_url,
-                              auth=client_auth,
-                              data=post_data, verify=False)
-    if (not self._context.hasRefreshToken()):
-      return
-    post_data = { "token" : self._context.getRefreshToken(), "token_type_hint" : "refresh_token" }
-    client_auth = requests.auth.HTTPBasicAuth(self._context.getClientId(), self._context.getProgramId())
-    auth_url = self._context.getAuthServer() + '/connect/revocation'
-    session = self.getSession()
-    response = session.post(auth_url,
-                              auth=client_auth,
-                              data=post_data, verify=False)
-
-  def detach(self):
+    
     try:
-      if not self._timer is None:
-        self._timer.cancel()
-    except Exception as ex:
-      import logging
-      logging.exception(ex)
+      post_data = { "token" : self._context.getToken() }
+      client_auth = requests.auth.HTTPBasicAuth(self._context.getClientId(), self._context.getProgramId())
+      auth_url = self._context.getAuthServer() + '/connect/revocation'
+      session = self._getSession()
+      try:
+        response = session.post(auth_url,
+                                  auth=client_auth,
+                                  data=post_data, verify=False)
+      except Exception as ex:
+        import traceback
+        details = traceback.format_exc()
+        import logging
+        logging.error('Trying to revoke token failed! Error: ' + str(ex) + '. Details: ' + details)
+
+      if (not self._context.hasRefreshToken()):
+        return
+      post_data = { "token" : self._context.getRefreshToken(), "token_type_hint" : "refresh_token" }
+      client_auth = requests.auth.HTTPBasicAuth(self._context.getClientId(), self._context.getProgramId())
+      auth_url = self._context.getAuthServer() + '/connect/revocation'
+      session = self._getSession()
+
+      try:
+        response = session.post(auth_url,
+                                  auth=client_auth,
+                                  data=post_data, verify=False)
+      except Exception as ex:
+        import traceback
+        details = traceback.format_exc()
+        import logging
+        logging.error('Trying to revoke refreshToken failed! Error: ' + str(ex) + '. Details: ' + details)
+
+    finally:
+      self._context.setRefreshToken(None)
+      self._context.setExpiration(None)
+      self._context.setToken(None)
 
+  def detach(self):
     import copy
     context = copy.deepcopy(self._context)
     self._context.reset()
     return context
 
 
   def close(self):
-    try:
-      if self._timer != None:
-        self._timer.cancel()
-    except Exception as ex:
-      import logging
-      logging.exception(ex)
-    self._context -= self.changedToken
     self.logout()
 
   def restart(self):
     self._context.setRefreshToken(None)
     self._context.setExpiration(None)
     self._context.setToken(None)
     self._context.setToken(self.renewToken())
-    self._timer = AutoStartTimer(60, self.reloadToken)
 
 
+class TokenOldException(Exception):
+    def __init__(self):
+        msg = 'The token is old.'
+        super().__init__(msg)
```

### Comparing `epmwebapi-1.8.74/epmwebapi/autostarttimer.py` & `epmwebapi-1.8.84/epmwebapi/autostarttimer.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/basicvariable.py` & `epmwebapi-1.8.84/epmwebapi/basicvariable.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/basicvariablepropertymask.py` & `epmwebapi-1.8.84/epmwebapi/basicvariablepropertymask.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/browseitemmodeljson.py` & `epmwebapi-1.8.84/epmwebapi/browseitemmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/browsemodeljson.py` & `epmwebapi-1.8.84/epmwebapi/browsemodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/browseresultmodeljson.py` & `epmwebapi-1.8.84/epmwebapi/browseresultmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/customtypedefinition.py` & `epmwebapi-1.8.84/epmwebapi/customtypedefinition.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/dataobjectsfilter.py` & `epmwebapi-1.8.84/epmwebapi/dataobjectsfilter.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/datasetconfig.py` & `epmwebapi-1.8.84/epmwebapi/datasetconfig.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/datasetpen.py` & `epmwebapi-1.8.84/epmwebapi/datasetpen.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/datavaluejson.py` & `epmwebapi-1.8.84/epmwebapi/datavaluejson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/dll_references/Elipse.Epm.AddressSpaceModel.dll` & `epmwebapi-1.8.84/epmwebapi/dll_references/Elipse.Epm.AddressSpaceModel.dll`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/dll_references/EpmData.dll` & `epmwebapi-1.8.84/epmwebapi/dll_references/EpmData.dll`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/epmconnection.py` & `epmwebapi-1.8.84/epmwebapi/epmconnection.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                                   'discrete': discrete, 'interface': interface, 'ioTagAddress': ioTagAddress,
                                   'processingEnabled': processingEnabled,
                                   'isRecording': isRecording, 'isCompressing': isCompressing,
                                   'storeMillisecondsEnabled': storeMillisecondsEnabled,
                                   'storageSet': storageSet, 'deadBandFilter': deadBandFilter,
                                   'deadBandUnit': deadBandUnit}]}
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.post(url, json=jsonRequest, verify=False)
         if response.status_code != 200:
             if response.status_code == 400:
                 if 'EpmErrorTagAlreadyExists' in response.text:
                     raise BasicVariableAlreadyExistsException('BasicVariable ' + name + ' already exists')
                 if 'Invalid format Name' in response.text:
                     raise BasicVariableInvalidNameException('BasicVariable ' + name + ' has an invalid format')
@@ -198,15 +198,15 @@
                                   'discrete': discrete, 'interface': interface, 'ioTagAddress': ioTagAddress,
                                   'processingEnabled': processingEnabled,
                                   'isRecording': isRecording, 'isCompressing': isCompressing,
                                   'storeMillisecondsEnabled': storeMillisecondsEnabled,
                                   'storageSet': storageSet, 'deadBandFilter': deadBandFilter,
                                   'deadBandUnit': deadBandUnit}]}
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.patch(url, json=jsonRequest, verify=False)
         if response.status_code != 200:
             if response.status_code == 400:
                 if 'EpmErrorTagAlreadyExists' in response.text:
                     raise BasicVariableAlreadyExistsException('BasicVariable ' + name + ' already exists')
                 if 'Invalid format Name' in response.text:
                     raise BasicVariableInvalidNameException('BasicVariable ' + name + ' has an invalid format')
@@ -219,15 +219,15 @@
 
     def deleteBasicVariable(self, names):
 
         url = self._webApi + '/epm/v1/BV'
 
         jsonRequest = {'Items': names}
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.delete(url, json=jsonRequest, verify=False)
         if response.status_code != 200:
             raise Exception(
                 "DeleteBasicVariable call error + '" + str(response.status_code) + "'. Reason: " + response.reason)
 
         json_result = json.loads(response.text)
 
@@ -236,29 +236,29 @@
             return [True if item == 1 else False for item in json_result['diagnostics']]
         else:
             return True
 
     def getAllCustomTypes(self):
         url = self._webApi + '/epm/v1/usertypes'
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.get(url, verify=False)
 
         if response.status_code != 200:
             raise Exception("GetAllCustomTypes call error + '" + str(response.status_code) + "'. Reason: " +
                             response.reason + ". Text: " + response.text)
 
         types_list = json.loads(response.text)
 
         return types_list
 
     def getCustomType(self, name):
         url = self._webApi + '/epm/v1/usertypes/' + name
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.get(url, verify=False)
 
         if response.status_code == 200:
             responseCode = response.json()['diagnostic']['code']
             if responseCode != 0:
                 if responseCode == 2158690304:
                     raise InvalidCustomTypeNameException('Custom type ' + name + ' not found')
@@ -318,15 +318,15 @@
 
             jsonRequest = {'name': name, 'icon': properties['icon'],
                            'aliasProperties': properties['aliasProperties'],
                            'simpleProperties': properties['simpleProperties'],
                            'objectProperties': properties['objectProperties'],
                            'placeHolderProperties': properties['placeHolderProperties']}
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.post(url, json=jsonRequest, verify=False)
 
         if response.status_code == 200:
             responseCode = response.json()['code']
             if responseCode != 0:
                 if responseCode == 2153840640:
                     if 'There is already a type with the same name!' in response.json()["message"]:
@@ -358,15 +358,15 @@
         return self.getCustomType(name)
 
     def updateCustomType(self, propertiesJson):
         url = self._webApi + '/epm/v1/usertypes'
 
         jsonRequest = propertiesJson
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.patch(url, json=jsonRequest, verify=False)
 
         if response.status_code == 200:
             responseCode = response.json()['code']
             if responseCode != 0:
                 if responseCode == 2158690304:
                     if 'Unknown type name' in response.json()["message"]:
@@ -391,15 +391,15 @@
         else:
             raise Exception("UpdateCustomType call error + '" + str(response.status_code) + "'. Reason: " +
                             response.reason + ". Text: " + response.text)
 
     def deleteCustomType(self, name):
         url = self._webApi + '/epm/v1/usertypes/' + name
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.delete(url, verify=False)
 
         if response.status_code == 200:
             responseCode = response.json()['code']
             if responseCode != 0:
                 if responseCode == 2158690304:
                     raise InvalidCustomTypeNameException('Custom type ' + name + ' not found')
@@ -528,14 +528,47 @@
             for index in range(0, len(identities)):
                 path = ''
                 if discoverInstancePaths:
                     path = self._getObjectPath(identities[index], names[index])
                 objs.append(EpmObject(self, identities[index], path, names[index], typeName))
         return objs
 
+    def _getObjectsFromItemPaths(self, browsePaths, paths):
+        # Verifica se todos os itens existem
+        readRequest = self._read(browsePaths, [NodeAttributes.NodeId.value] * len(browsePaths)).items()
+
+        objs = collections.OrderedDict()
+
+        existentPaths = []
+        identities = []
+
+        index = 0
+        for item in readRequest:
+            if item[1].code != 0:
+                objs[paths[index]] = None
+            else:
+                existentPaths.append(paths[index])
+                identities.append(ItemPathJSON('OPCUA.NodeId', None, item[0]._identity))
+            index = index + 1
+
+        if len(identities) < 1:
+            return objs
+
+        typesResults = self._browse(identities, EpmNodeIds.HasTypeDefinition.value).references()
+     
+        for index in range(0, len(existentPaths)):
+            if typesResults[index][0]._displayName == "PropertyType":
+                objs[existentPaths[index]] = EpmProperty(self, existentPaths[index].split('/')[-1], existentPaths[index],
+                                                        identities[index])
+            else:
+                objs[existentPaths[index]] = EpmModelObject(self, identities[index], existentPaths[index],
+                                                            existentPaths[index].split('/')[-1],
+                                                            typesResults[index][0]._displayName)
+
+        return objs
 
     def getObjects(self, objectsPaths):
         paths = []
         browsePaths = []
 
         if type(objectsPaths) is str:
             paths.append(objectsPaths)
@@ -640,48 +673,68 @@
                                                             typesResults[index][0]._displayName)
 
         return objs
 
     def getElipseDataModelObjects(self, objectsPaths):
         paths = []
         browsePaths = []
+        resultPaths = []
 
         if type(objectsPaths) is str:
-            objectsPaths = '/Models/ElipseDataModel/' + objectsPaths
+            resultPaths.append(objectsPaths)
+            if objectsPaths == '' or objectsPaths[0] == '/':
+                objectsPaths = '/Models/ElipseDataModel' + objectsPaths
+            else:
+                objectsPaths = '/Models/ElipseDataModel/' + objectsPaths
             paths.append(objectsPaths)
             browsePath = self._translatePathToBrowsePath(objectsPaths)
             browsePaths.append(ItemPathJSON('OPCUA.BrowsePath', '', browsePath))
         else:
             for path in objectsPaths:
-                path = '/Models/ElipseDataModel/' + path
+                resultPaths.append(path)
+                if path == '' or path[0] == '/':
+                    path = '/Models/ElipseDataModel' + path
+                else:
+                    path = '/Models/ElipseDataModel/' + path
                 paths.append(path)
                 browsePath = self._translatePathToBrowsePath(path)
                 browsePaths.append(ItemPathJSON('OPCUA.BrowsePath', '', browsePath))
 
         # Verifica se todos os itens existem
         readRequest = self._read(browsePaths, [NodeAttributes.NodeId.value] * len(browsePaths)).items()
 
-        identities = [ItemPathJSON('OPCUA.NodeId', None, item[0]._identity) for item in readRequest]
-        diagnosticResults = [item[1].code for item in readRequest]
+        objs = collections.OrderedDict()
 
-        typesResults = self._browse(identities, EpmNodeIds.HasTypeDefinition.value).references()
+        existentPaths = []
+        opcUaPaths = []
+        identities = []
 
-        objs = collections.OrderedDict()
-        for index in range(0, len(paths)):
-            if diagnosticResults[index] == 0:
-                if typesResults[index][0]._displayName == "PropertyType":
-                    objs[objectsPaths[index]] = EpmProperty(self, paths[index].split('/')[-1], paths[index],
-                                                            identities[index])
-                else:
-                    objs[objectsPaths[index]] = EpmObject(self, identities[index], paths[index],
-                                                          paths[index].split('/')[-1],
-                                                          typesResults[index][0]._displayName)
+        index = 0
+        for item in readRequest:
+            if item[1].code != 0:
+                objs[resultPaths[index]] = None
             else:
-                objs[paths[index]] = None
+                existentPaths.append(resultPaths[index])
+                opcUaPaths.append(paths[index])
+                identities.append(ItemPathJSON('OPCUA.NodeId', None, item[0]._identity))
+            index = index + 1
+
+        if len(identities) < 1:
+            return objs
+        
+        typesResults = self._browse(identities, EpmNodeIds.HasTypeDefinition.value).references()
 
+        for index in range(0, len(existentPaths)):
+            if typesResults[index][0]._displayName == "PropertyType":
+                objs[resultPaths[index]] = EpmProperty(self, opcUaPaths[index].split('/')[-1], opcUaPaths[index],
+                                                        identities[index])
+            else:
+                objs[resultPaths[index]] = EpmModelObject(self, identities[index], opcUaPaths[index],
+                                                            opcUaPaths[index].split('/')[-1],
+                                                            typesResults[index][0]._displayName)
         return objs
 
     def addInstancesEpmModel(self, path, names, objTypes):
         url = self._webApi + '/epm/v1/epmmodel/' + path
         paths = []
         objs = {}
 
@@ -702,15 +755,15 @@
                     raise BadArgumentException("Names and ObjTypes must have the same size")
                 requestList = []
                 for (name, objType) in zip(names, objTypes):
                     requestList.append({'name': name, 'type': objType})
                     paths.append(path + "/" + name)
                 jsonRequest = {'items': requestList}
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.post(url, json=jsonRequest, verify=False)
 
         if response.status_code == 200:
             responseCode = response.json()['code']
             if responseCode != 0:
                 if responseCode == 2153840640:
                     raise InstanceNameDuplicatedException('Instance name duplicated')
@@ -730,15 +783,15 @@
             objs[obj.name] = obj
 
         return objs
 
     def removeInstanceEpmModel(self, path):
         url = self._webApi + '/epm/v1/epmmodel/' + path
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.delete(url, verify=False)
 
         if response.status_code == 200:
             responseCode = response.json()['code']
             if responseCode != 0:
                 if responseCode == 2154758144:
                     raise InvalidObjectNameException('EPM Model object not found')
@@ -750,15 +803,15 @@
 
     def setBindedVariables(self, objectPath, aliasProperties, variablesNames, isEpmModel=True):
         if isEpmModel:
             url = self._webApi + '/epm/v1/epmmodel/' + objectPath
         else:
             raise BadArgumentException('Invalid isEpmModel argument')
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.get(url, verify=False)
 
         if response.status_code == 200:
             responseCode = response.json()['diagnostic']['code']
             if responseCode != 0:
                 if responseCode == 2154758144:
                     raise InvalidObjectNameException('Object not found')
@@ -829,15 +882,15 @@
 
         self._jsonToEpmModelInstances(jsonRead['items'], '', importMode)
 
 
     def _epmModelInstancesToJson(self, path):
         url = self._webApi + '/epm/v1/epmmodel/' + path
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.get(url, verify=False)
 
         if response.status_code == 200:
             responseCode = response.json()['diagnostic']['code']
             if responseCode != 0:
                 if responseCode == 2154758144:
                     raise InvalidObjectNameException('Object ' + path + ' not found')
@@ -864,15 +917,15 @@
             itemsList.append(dic)
 
         return itemsList
 
     def _jsonToEpmModelInstances(self, items, path, importMode):
         url = self._webApi + '/epm/v1/epmmodel/' + path
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.get(url, verify=False)
 
         if response.status_code == 200:
             responseCode = response.json()['diagnostic']['code']
             if responseCode != 0:
                 if responseCode == 2154758144:
                     raise InvalidObjectNameException('Object ' + path + ' not found')
@@ -1025,15 +1078,15 @@
 
     def loadDatasetServer(self, name):
         url = self._webApi + '/epm/v1/resource'
         datasetAddress = "1:Datasets/1:" + name
         itemPath = ItemPathJSON("OPCUA.BrowsePath", None, datasetAddress)
         continuationPoint = None
         jsonRequest = {"continuationPoint": continuationPoint, "paths": [itemPath.toDict()]}
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.post(url, json=jsonRequest, verify=False)
         jsonResponse = json.loads(response.text)
         content = jsonResponse['items'][0]['content']
         description = jsonResponse['items'][0]['description']
 
         return DatasetConfigServer(self, name, description, content)
 
@@ -1048,15 +1101,15 @@
 
     def _saveDatasetServer(self, name, description, content, overwrite = False, oldName = None):
         exists = False
         for datasetName in self.listDatasetServer():
             if str.lower(name) == str.lower(datasetName):
                 exists = True
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
 
         if exists is False:
             if oldName is None:
                 identity = None
             else:
                 url = self._webApi + '/epm/v1/resource'
                 datasetAddress = "1:Datasets/1:" + oldName
@@ -1101,15 +1154,15 @@
             if str.lower(name) == str.lower(datasetName):
                 exists = True
         if exists is True:
             url = self._webApi + '/epm/v1/resource/remove'
             datasetAddress = "1:Datasets/1:" + name
             itemPath = ItemPathJSON("OPCUA.BrowsePath", None, datasetAddress)
             jsonRequest = {"paths": [itemPath.toDict()]}
-            session = self._authorizationService.getSession()
+            session = self._authorizationService.getEpmSession()
             response = session.post(url, json=jsonRequest, verify=False)
             jsonResponse = json.loads(response.text)
             errorCode = jsonResponse['diagnostics'][0]['code']
             if errorCode != 0:
                 raise Exception("Dataset delete did not succeed")
         else:
             raise BadArgumentException("Dataset does not exist")
@@ -1130,15 +1183,15 @@
         return datasetNames
 
     def listDatasetServer(self):
         url = self._webApi + '/epm/v1/resource/list'
         continuationPoint = None
         datasetTypeId = "{041582AB-CD7B-4313-8477-1D3AC4A43256}"
         jsonRequest = {"continuationPoint": continuationPoint, "types": [datasetTypeId]}
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.post(url, json=jsonRequest, verify=False)
         jsonResponse = json.loads(response.text)
         datasetNames = []
         for item in jsonResponse['items']:
             datasetNames.append(item['name'])
 
         return datasetNames
@@ -1222,15 +1275,15 @@
         return
 
     def _historyUpdateCall(self, historyUpdateRequest):
         url = self._webApi + '/opcua/v1/history/update/data'
 
         jsonRequest = historyUpdateRequest.toDict()
 
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.post(url, json=jsonRequest, verify=False)
         if response.status_code != 200:
             raise Exception(
                 "HistoryUpdate call error + '" + str(response.status_code) + "'. Reason: " + response.reason)
 
         json_result = json.loads(response.text)
         if json_result['diagnostics'][0]['code'] != 0:
@@ -1269,15 +1322,15 @@
 
         writeItems = []
         for x in range(0, len(paths)):
             writeItems.append(WriteItemModelJSON(paths[x], attributeIds[x], values[x]))
 
         request = WriteModelJSON(writeItems)
         jsonRequest = request.toDict()
-        session = self._authorizationService.getSession()
+        session = self._authorizationService.getEpmSession()
         response = session.post(url, json=jsonRequest, verify=False)
         if response.status_code != 200:
             print(response.reason)
             raise Exception(
                 "Write service call http error '" + str(response.status_code) + "'. Reason: " + response.reason + ". Message: " + response.text)
         json_result = json.loads(response.text)
         if json_result is None:
@@ -1302,15 +1355,15 @@
 
         resultItems = []
         diagnostics = []
 
         while True:
             request = ReadModelJSON(readItems, continuationPoint)
             jsonRequest = request.toDict()
-            session = self._authorizationService.getSession()
+            session = self._authorizationService.getEpmSession()
             response = session.post(url, json=jsonRequest, verify=False)
             if response.status_code != 200:
                 print(response.reason)
                 raise Exception(
                     "Read service call http error '" + str(response.status_code) + "'. Reason: " + response.reason)
             json_result = json.loads(response.text)
             if json_result is None:
@@ -1352,15 +1405,15 @@
 
         requestResults = []
         diagnostics = []
 
         while True:
             request = BrowseModelJSON(itemsModels, continuationPoint)
             jsonRequest = request.toDict()
-            session = self._authorizationService.getSession()
+            session = self._authorizationService.getEpmSession()
             response = session.post(url, json=jsonRequest, verify=False)
             if response.status_code != 200:
                 print(response.reason)
                 raise Exception(
                     "Browse service call http error '" + str(response.status_code) + "'. Reason: " + response.reason)
             json_result = json.loads(response.text)
             if json_result is None:
@@ -1404,15 +1457,15 @@
         processingInterval = aggregateType.interval.total_seconds() * 1000
 
         while True:
             itemPathAndCP = ItemPathAndContinuationPointJSON(itemPath, continuationPoint, False)
             historyReadRequest = HistoryProcessedModelJSON(aggregatePath, processingInterval, queryPeriod.start,
                                                            queryPeriod.end, [itemPathAndCP])
             jsonRequest = historyReadRequest.toDict()
-            session = self._authorizationService.getSession()
+            session = self._authorizationService.getEpmSession()
             response = session.post(url, json=jsonRequest, verify=False)
             if response.status_code != 200:
                 print(response.reason)
                 raise Exception(
                     "Service call http error '" + str(response.status_code) + "'. Reason: " + response.reason)
             json_result = json.loads(response.text)
             if json_result is None:
@@ -1440,15 +1493,15 @@
 
         import dateutil.parser
 
         while True:
             itemPathAndCP = ItemPathAndContinuationPointJSON(annotationPath, continuationPoint, False)
             historyReadRequest = HistoryRawModelJSON(queryPeriod.start, queryPeriod.end, False, [itemPathAndCP])
             jsonRequest = historyReadRequest.toDict()
-            session = self._authorizationService.getSession()
+            session = self._authorizationService.getEpmSession()
             response = session.post(url, json=jsonRequest, verify=False)
             if response.status_code != 200:
                 print(response.reason)
                 raise Exception(
                     "Service call http error '" + str(response.status_code) + "'. Reason: " + response.reason)
             json_result = json.loads(response.text)
             if json_result is None:
@@ -1481,15 +1534,15 @@
         continuationPoint = None
         dataValues = []
 
         while True:
             itemPathAndCP = ItemPathAndContinuationPointJSON(itemPath, continuationPoint, False)
             historyReadRequest = HistoryRawModelJSON(queryPeriod.start, queryPeriod.end, bounds, [itemPathAndCP])
             jsonRequest = historyReadRequest.toDict()
-            session = self._authorizationService.getSession()
+            session = self._authorizationService.getEpmSession()
             response = session.post(url, json=jsonRequest, verify=False)
             if response.status_code != 200:
                 print(response.reason)
                 raise Exception(
                     "Service call http error '" + str(response.status_code) + "'. Reason: " + response.reason)
             json_result = json.loads(response.text)
             if json_result is None:
@@ -1518,15 +1571,15 @@
         items = collections.OrderedDict()
 
         while True:
             model = QueryModelJSON(continuationPoint, False,
                                    QueryResultMask.Name.value | QueryResultMask.Identity.value, browseNameFilter,
                                    descriptionFilter, euNameFilter, typeFilter, domainFilter.value)
             jsonRequest = model.toDict()
-            session = self._authorizationService.getSession()
+            session = self._authorizationService.getEpmSession()
             response = session.post(url, json=jsonRequest, verify=False)
             if response.status_code != 200:
                 print(response.reason)
                 raise Exception(
                     "Service call http error '" + str(response.status_code) + "'. Reason: " + response.reason)
             json_result = json.loads(response.text)
             if json_result is None:
```

### Comparing `epmwebapi-1.8.74/epmwebapi/epmconnectioncontext.py` & `epmwebapi-1.8.84/epmwebapi/epmconnectioncontext.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,26 +13,14 @@
       self._eventhandler = []
 
     def __deepcopy__(self, memodict={}):
         cpyobj = EpmConnectionContext(self._authServer, self._webapi, self._clientId, self._programId, self._userName, 
                                       self._password, self._token, self._refreshToken, self._expiration) # shallow copy of whole object 
         return cpyobj
 
-    def __iadd__(self, ehandler):
-      self._eventhandler.append(ehandler) 
-      return self
-
-    def __isub__(self, ehandler):
-      self._eventhandler.remove(ehandler) 
-      return self
-
-    def onchangeToken(self, token): 
-      for eventhandler in self._eventhandler: 
-        eventhandler(token)
-
     def set(self, authServer, webapi, clientId, programId, userName, password, token, refreshToken, expiration):
       self._authServer = authServer
       self._webapi = webapi
       self._clientId = clientId
       self._programId = programId
       self._userName = userName
       self._password = password
@@ -48,17 +36,17 @@
       self._userName = None
       self._password = None
       self._token = None
       self._refreshToken = None
       self._expiration = None
 
     def isValidToken(self):
-      if self.hasExpiration():
+      if self.hasToken() and self.hasExpiration():
         from datetime import datetime, timedelta
-        return self._expiration < datetime.utcnow() + timedelta(seconds=10) 
+        return self._expiration > datetime.utcnow() + timedelta(seconds=30) 
       return False
 
     def hasToken(self):
       return self._token != None
 
     def hasRefreshToken(self):
       return self._refreshToken != None
@@ -104,15 +92,14 @@
       self._password = password
 
     def getToken(self):
       return self._token
 
     def setToken(self, token):
       self._token = token
-      self.onchangeToken(token)
 
     def getRefreshToken(self):
       return self._refreshToken
 
     def setRefreshToken(self, refreshToken):
       self._refreshToken = refreshToken
```

### Comparing `epmwebapi-1.8.74/epmwebapi/epmdataobject.py` & `epmwebapi-1.8.84/epmwebapi/epmdataobject.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/epmmodelobject.py` & `epmwebapi-1.8.84/epmwebapi/epmmodelobject.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/epmnodeids.py` & `epmwebapi-1.8.84/epmwebapi/epmnodeids.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/epmobject.py` & `epmwebapi-1.8.84/epmwebapi/epmobject.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,17 @@
         self._path = path
         self._type = type
         self._name = name
 
     # Public Methods
     def enumObjects(self):
         childObjects = collections.OrderedDict()
-        result = self._epmConnection._browse([self._itemPath], EpmNodeIds.HasComponent.value).references()[0]
+        hasComponentElements = self._epmConnection._browse([self._itemPath], EpmNodeIds.HasComponent.value).references()[0]
+        organizesElements = self._epmConnection._browse([self._itemPath], EpmNodeIds.Organizes.value).references()[0]
+        result = hasComponentElements + organizesElements
         if len(result) < 1:
             return childObjects
         
         identities = [ItemPathJSON('OPCUA.NodeId', '', item._identity) for item in result]
         typesResults = self._epmConnection._browse(identities, EpmNodeIds.HasTypeDefinition.value).references()
 
         for index in range(0, len(result)):
```

### Comparing `epmwebapi-1.8.74/epmwebapi/epmproperty.py` & `epmwebapi-1.8.84/epmwebapi/epmproperty.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/epmutils.py` & `epmwebapi-1.8.84/epmwebapi/epmutils.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/epmvariable.py` & `epmwebapi-1.8.84/epmwebapi/epmvariable.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/folder.py` & `epmwebapi-1.8.84/epmwebapi/folder.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/historyprocessedmodeljson.py` & `epmwebapi-1.8.84/epmwebapi/historyprocessedmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/historyrawmodeljson.py` & `epmwebapi-1.8.84/epmwebapi/historyrawmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/historyupdatedataitemmodeljson.py` & `epmwebapi-1.8.84/epmwebapi/historyupdatedataitemmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/historyupdatedatamodeljson.py` & `epmwebapi-1.8.84/epmwebapi/historyupdatedatamodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/itempathandcontinuationpointjson.py` & `epmwebapi-1.8.84/epmwebapi/itempathandcontinuationpointjson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/itempathjson.py` & `epmwebapi-1.8.84/epmwebapi/itempathjson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/mimetype.py` & `epmwebapi-1.8.84/epmwebapi/mimetype.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/nodeattributes.py` & `epmwebapi-1.8.84/epmwebapi/nodeattributes.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/nodeclassmask.py` & `epmwebapi-1.8.84/epmwebapi/nodeclassmask.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/numpyextras.py` & `epmwebapi-1.8.84/epmwebapi/numpyextras.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/querymodeljson.py` & `epmwebapi-1.8.84/epmwebapi/querymodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/queryperiod.py` & `epmwebapi-1.8.84/epmwebapi/queryperiod.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/queryresultmodeljson.py` & `epmwebapi-1.8.84/epmwebapi/queryresultmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/readmodeljson.py` & `epmwebapi-1.8.84/epmwebapi/readmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/readresultmodeljson.py` & `epmwebapi-1.8.84/epmwebapi/readresultmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/resource.py` & `epmwebapi-1.8.84/epmwebapi/resource.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/resourcesmanager.py` & `epmwebapi-1.8.84/epmwebapi/resourcesmanager.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/statuscodes.py` & `epmwebapi-1.8.84/epmwebapi/statuscodes.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/writeitemmodeljson.py` & `epmwebapi-1.8.84/epmwebapi/writeitemmodeljson.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi/__init__.py` & `epmwebapi-1.8.84/epmwebapi/__init__.py`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/epmwebapi.egg-info/PKG-INFO` & `epmwebapi-1.8.84/epmwebapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epmwebapi
-Version: 1.8.74
+Version: 1.8.84
 Summary: UNKNOWN
 Home-page: https://github.com/elipsesoftware/epmwebapi
 Author: Elipse Software Ltda
 License: UNKNOWN
 Description: # epmwebapi
         
         A biblioteca **Epmwebapi** desenvolvida pela **Elipse Software**, permite a interação com os dados da sua plataforma
```

### Comparing `epmwebapi-1.8.74/epmwebapi.egg-info/SOURCES.txt` & `epmwebapi-1.8.84/epmwebapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 epmwebapi/epmconnection.py
 epmwebapi/epmconnectioncontext.py
 epmwebapi/epmdataobject.py
 epmwebapi/epmmodelobject.py
 epmwebapi/epmnodeids.py
 epmwebapi/epmobject.py
 epmwebapi/epmproperty.py
+epmwebapi/epmsession.py
 epmwebapi/epmutils.py
 epmwebapi/epmvariable.py
 epmwebapi/epmwebapi.py
 epmwebapi/folder.py
 epmwebapi/historyprocessedmodeljson.py
 epmwebapi/historyrawmodeljson.py
 epmwebapi/historyresultitemmodeljson.py
```

### Comparing `epmwebapi-1.8.74/LICENSE.txt` & `epmwebapi-1.8.84/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/PKG-INFO` & `epmwebapi-1.8.84/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epmwebapi
-Version: 1.8.74
+Version: 1.8.84
 Summary: UNKNOWN
 Home-page: https://github.com/elipsesoftware/epmwebapi
 Author: Elipse Software Ltda
 License: UNKNOWN
 Description: # epmwebapi
         
         A biblioteca **Epmwebapi** desenvolvida pela **Elipse Software**, permite a interação com os dados da sua plataforma
```

### Comparing `epmwebapi-1.8.74/Readme.md` & `epmwebapi-1.8.84/Readme.md`

 * *Files identical despite different names*

### Comparing `epmwebapi-1.8.74/setup.py` & `epmwebapi-1.8.84/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name = 'epmwebapi', 
-      version = '1.8.74', 
+      version = '1.8.84', 
       author = 'Elipse Software Ltda', 
       packages = ['epmwebapi'], 
       include_package_data=True,
       description = '', 
       long_description = long_description, 
       long_description_content_type='text/markdown',
       url = 'https://github.com/elipsesoftware/epmwebapi',
```

