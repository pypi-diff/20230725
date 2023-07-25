# Comparing `tmp/audiostack-0.0.7.tar.gz` & `tmp/audiostack-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostack-0.0.7.tar", last modified: Thu Jun  1 13:44:18 2023, max compression
+gzip compressed data, was "audiostack-0.0.9.tar", last modified: Fri Jul  7 13:16:44 2023, max compression
```

## Comparing `audiostack-0.0.7.tar` & `audiostack-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.496035 audiostack-0.0.7/
--rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-06-01 13:44:18.495875 audiostack-0.0.7/PKG-INFO
--rw-r--r--   0 hackerman   (501) staff       (20)    26796 2022-12-13 14:01:40.000000 audiostack-0.0.7/README.md
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.486341 audiostack-0.0.7/audiostack/
--rw-r--r--   0 hackerman   (501) staff       (20)      555 2023-06-01 13:43:58.000000 audiostack-0.0.7/audiostack/__init__.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.488871 audiostack-0.0.7/audiostack/content/
--rw-r--r--   0 hackerman   (501) staff       (20)      459 2023-03-16 15:15:23.000000 audiostack-0.0.7/audiostack/content/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     2270 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/content/media.py
--rw-r--r--   0 hackerman   (501) staff       (20)      947 2023-03-16 15:15:23.000000 audiostack-0.0.7/audiostack/content/root_functions.py
--rw-r--r--   0 hackerman   (501) staff       (20)     3528 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/content/script.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.489482 audiostack-0.0.7/audiostack/delivery/
--rw-r--r--   0 hackerman   (501) staff       (20)       48 2022-12-06 15:30:00.000000 audiostack-0.0.7/audiostack/delivery/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     2313 2023-05-04 12:16:31.000000 audiostack-0.0.7/audiostack/delivery/encoder.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.490214 audiostack-0.0.7/audiostack/docs/
--rw-r--r--   0 hackerman   (501) staff       (20)       47 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/docs/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      631 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/docs/docs.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.492062 audiostack-0.0.7/audiostack/helpers/
--rw-r--r--   0 hackerman   (501) staff       (20)        0 2022-12-06 15:30:00.000000 audiostack-0.0.7/audiostack/helpers/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      716 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/helpers/api_item.py
--rw-r--r--   0 hackerman   (501) staff       (20)      972 2023-06-01 13:43:58.000000 audiostack-0.0.7/audiostack/helpers/api_list.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4322 2023-05-22 09:42:33.000000 audiostack-0.0.7/audiostack/helpers/request_interface.py
--rw-r--r--   0 hackerman   (501) staff       (20)      163 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/helpers/request_types.py
--rw-r--r--   0 hackerman   (501) staff       (20)      338 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/helpers/response.py
--rw-r--r--   0 hackerman   (501) staff       (20)      227 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/helpers/util.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.492255 audiostack-0.0.7/audiostack/orchestrator/
--rw-r--r--   0 hackerman   (501) staff       (20)       58 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/orchestrator/__init__.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.493282 audiostack-0.0.7/audiostack/production/
--rw-r--r--   0 hackerman   (501) staff       (20)       88 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/production/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4149 2023-06-01 13:43:58.000000 audiostack-0.0.7/audiostack/production/mix.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4349 2023-04-17 07:55:11.000000 audiostack-0.0.7/audiostack/production/sound.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.494550 audiostack-0.0.7/audiostack/speech/
--rw-r--r--   0 hackerman   (501) staff       (20)      126 2022-12-08 09:57:07.000000 audiostack-0.0.7/audiostack/speech/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     2979 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/speech/diction.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4621 2023-06-01 13:43:58.000000 audiostack-0.0.7/audiostack/speech/tts.py
--rw-r--r--   0 hackerman   (501) staff       (20)     1215 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/speech/voice.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.487224 audiostack-0.0.7/audiostack.egg-info/
--rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-06-01 13:44:18.000000 audiostack-0.0.7/audiostack.egg-info/PKG-INFO
--rw-r--r--   0 hackerman   (501) staff       (20)      959 2023-06-01 13:44:18.000000 audiostack-0.0.7/audiostack.egg-info/SOURCES.txt
--rw-r--r--   0 hackerman   (501) staff       (20)        1 2023-06-01 13:44:18.000000 audiostack-0.0.7/audiostack.egg-info/dependency_links.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       45 2023-06-01 13:44:18.000000 audiostack-0.0.7/audiostack.egg-info/requires.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       17 2023-06-01 13:44:18.000000 audiostack-0.0.7/audiostack.egg-info/top_level.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       38 2023-06-01 13:44:18.496093 audiostack-0.0.7/setup.cfg
--rw-r--r--   0 hackerman   (501) staff       (20)     1039 2023-02-20 16:12:26.000000 audiostack-0.0.7/setup.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.495171 audiostack-0.0.7/tests/
--rw-r--r--   0 hackerman   (501) staff       (20)      173 2023-02-20 16:03:10.000000 audiostack-0.0.7/tests/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      659 2023-02-20 16:41:55.000000 audiostack-0.0.7/tests/test_audience.py
+drwxr-xr-x   0 guillempeeters   (501) staff       (20)        0 2023-07-07 13:16:44.514264 audiostack-0.0.9/
+-rw-r--r--   0 guillempeeters   (501) staff       (20)     1061 2022-12-12 09:47:00.000000 audiostack-0.0.9/LICENSE
+-rw-r--r--   0 guillempeeters   (501) staff       (20)    27644 2023-07-07 13:16:44.514085 audiostack-0.0.9/PKG-INFO
+-rw-r--r--   0 guillempeeters   (501) staff       (20)    27169 2023-07-07 13:13:10.000000 audiostack-0.0.9/README.md
+drwxr-xr-x   0 guillempeeters   (501) staff       (20)        0 2023-07-07 13:16:44.510355 audiostack-0.0.9/audiostack/
+-rw-r--r--   0 guillempeeters   (501) staff       (20)      555 2023-07-07 13:16:21.000000 audiostack-0.0.9/audiostack/__init__.py
+drwxr-xr-x   0 guillempeeters   (501) staff       (20)        0 2023-07-07 13:16:44.511812 audiostack-0.0.9/audiostack/content/
+-rw-r--r--   0 guillempeeters   (501) staff       (20)      459 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/content/__init__.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)     2270 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/content/media.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)      947 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/content/root_functions.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)     3528 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/content/script.py
+drwxr-xr-x   0 guillempeeters   (501) staff       (20)        0 2023-07-07 13:16:44.512020 audiostack-0.0.9/audiostack/delivery/
+-rw-r--r--   0 guillempeeters   (501) staff       (20)       48 2022-12-12 09:47:00.000000 audiostack-0.0.9/audiostack/delivery/__init__.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)     3223 2023-07-07 13:13:10.000000 audiostack-0.0.9/audiostack/delivery/encoder.py
+drwxr-xr-x   0 guillempeeters   (501) staff       (20)        0 2023-07-07 13:16:44.512233 audiostack-0.0.9/audiostack/docs/
+-rw-r--r--   0 guillempeeters   (501) staff       (20)       47 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/docs/__init__.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)      631 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/docs/docs.py
+drwxr-xr-x   0 guillempeeters   (501) staff       (20)        0 2023-07-07 13:16:44.513030 audiostack-0.0.9/audiostack/helpers/
+-rw-r--r--   0 guillempeeters   (501) staff       (20)        0 2022-12-12 09:47:00.000000 audiostack-0.0.9/audiostack/helpers/__init__.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)      809 2023-06-29 08:15:00.000000 audiostack-0.0.9/audiostack/helpers/api_item.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)      972 2023-06-29 08:15:00.000000 audiostack-0.0.9/audiostack/helpers/api_list.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)     4597 2023-07-07 13:13:10.000000 audiostack-0.0.9/audiostack/helpers/request_interface.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)      163 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/helpers/request_types.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)      338 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/helpers/response.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)      227 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/helpers/util.py
+drwxr-xr-x   0 guillempeeters   (501) staff       (20)        0 2023-07-07 13:16:44.513128 audiostack-0.0.9/audiostack/orchestrator/
+-rw-r--r--   0 guillempeeters   (501) staff       (20)       58 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/orchestrator/__init__.py
+drwxr-xr-x   0 guillempeeters   (501) staff       (20)        0 2023-07-07 13:16:44.513433 audiostack-0.0.9/audiostack/production/
+-rw-r--r--   0 guillempeeters   (501) staff       (20)       88 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/production/__init__.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)     4628 2023-07-07 13:13:10.000000 audiostack-0.0.9/audiostack/production/mix.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)     4349 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/production/sound.py
+drwxr-xr-x   0 guillempeeters   (501) staff       (20)        0 2023-07-07 13:16:44.513849 audiostack-0.0.9/audiostack/speech/
+-rw-r--r--   0 guillempeeters   (501) staff       (20)      126 2022-12-12 09:47:00.000000 audiostack-0.0.9/audiostack/speech/__init__.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)     2979 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/speech/diction.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)     5870 2023-06-29 08:15:00.000000 audiostack-0.0.9/audiostack/speech/tts.py
+-rw-r--r--   0 guillempeeters   (501) staff       (20)     1215 2023-04-21 14:37:45.000000 audiostack-0.0.9/audiostack/speech/voice.py
+drwxr-xr-x   0 guillempeeters   (501) staff       (20)        0 2023-07-07 13:16:44.511354 audiostack-0.0.9/audiostack.egg-info/
+-rw-r--r--   0 guillempeeters   (501) staff       (20)    27644 2023-07-07 13:16:44.000000 audiostack-0.0.9/audiostack.egg-info/PKG-INFO
+-rw-r--r--   0 guillempeeters   (501) staff       (20)      926 2023-07-07 13:16:44.000000 audiostack-0.0.9/audiostack.egg-info/SOURCES.txt
+-rw-r--r--   0 guillempeeters   (501) staff       (20)        1 2023-07-07 13:16:44.000000 audiostack-0.0.9/audiostack.egg-info/dependency_links.txt
+-rw-r--r--   0 guillempeeters   (501) staff       (20)       45 2023-07-07 13:16:44.000000 audiostack-0.0.9/audiostack.egg-info/requires.txt
+-rw-r--r--   0 guillempeeters   (501) staff       (20)       11 2023-07-07 13:16:44.000000 audiostack-0.0.9/audiostack.egg-info/top_level.txt
+-rw-r--r--   0 guillempeeters   (501) staff       (20)       38 2023-07-07 13:16:44.514304 audiostack-0.0.9/setup.cfg
+-rw-r--r--   0 guillempeeters   (501) staff       (20)     1039 2023-04-21 14:37:45.000000 audiostack-0.0.9/setup.py
```

### Comparing `audiostack-0.0.7/README.md` & `audiostack-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -670,18 +670,18 @@
 
 	``` audiostack.Production.Mix.delete(<args>)```
 
 	- Parameters:
 		 - `productionId` *[required] (string) - 
 
 ---
-- `list()` Lists available encoder presets.
+- `list()` Lists available mix presets.
 
 
-	``` audiostack.Production.Mix.get(<args>)```
+	``` audiostack.Production.Mix.list_presets(<args>)```
 
 	- Parameters:
 		 - (none) 
 
 ---
 ### `Mixes` resource <a name = "mixes"> </a>
 
@@ -708,24 +708,33 @@
 Out Delivery endpoints put the finishing touches on your mixed audio assets. Our encoder can be used to convert your file into a different format i.e. `mp3`. Our connector endpoints allow you to publish these assets onwards.
 
 
 ---
 - `create()` Changes the audio encoding of a mixed audio file
 
 
-	``` audiostack.Delivery.Encoder.create(<args>)```
+	``` audiostack.Delivery.Encoder.encode_mix(<args>)```
 
 
 	For most use cases, the preset can be either `custom` or one of the values returned from the `/encoder/presets` list. When using `custom` the other fields can be supplied. Please note not all fields are supported in conjunction with one another. For example `sampleRate` cannot be used in conjunction with `bitRateType`.
 	- Parameters:
 		 - `productionId` *[required] (string) - Reference to the productionId that is to be encoded
 		 - `preset` (string) - named preset to use or 'custom'
 		 - `public` (boolean) - Make the output a publicly available URL 
 		 - `bitRateType` (string) - Supplied value must be either 'constant' or 'variable
 		 - `bitRate` (string) - Can be between 0-9 for variable bit rates, or between 32 and 320 for constant bit rates
 		 - `sampleRate` (int) - Sample rate, should be between 24000 and 96000
 		 - `format` (string) - Can be wav, mp3, flac or ogg
 		 - `bitDepth` (int) - Can be 16, 24, or 32
 		 - `channels` (int) - Supply 1 for mono or 2 for stereo
-		 - `masteringPreset` (string) - Mastering preset to use, for example heavyDucking.
+		 - `loudnessPreset` (string) - Loudness standard to use, for example spotify or podcast.
+
+---
+
+- `list()` Lists available encoder presets.
+
+
+	``` audiostack.Delivery.Encoder.list_presets(<args>)```
+
+	Returns a list of encoding presets, for example mp3, wav for alexa, wav 48kHz and a description of these. In addition, returns a list of loudness presets which match the loudness specifications for apple podcasting, spotify advertising and other.
 
 ---
```

#### html2text {}

```diff
@@ -292,34 +292,38 @@
 `sectionProperties` (object) - todo - `acousticSpace` (string) - Applies an
 acoustic reverb to the speech track - `masteringPreset` (string) - Mastering
 preset to use, for example heavyDucking. - `public` (boolean) - Makes returned
 URLs publicly available --- - `get()` Retrieve a mixed resource. ```
 audiostack.Production.Mix.get()``` - Parameters: - `productionId` *[required]
 (string) - --- - `delete()` Deletes a mixed resource ```
 audiostack.Production.Mix.delete()``` - Parameters: - `productionId` *
-[required] (string) - --- - `list()` Lists available encoder presets. ```
-audiostack.Production.Mix.get()``` - Parameters: - (none) --- ### `Mixes`
-resource  --- - `list()` Lists multiple mixed resources. ```
+[required] (string) - --- - `list()` Lists available mix presets. ```
+audiostack.Production.Mix.list_presets()``` - Parameters: - (none) --- ###
+`Mixes` resource  --- - `list()` Lists multiple mixed resources. ```
 audiostack.Production.Mixes.get()``` Returns a list of mixed files that have
 been created. Can be filtered by `projectName`, `moduleName`, `scriptName` and
 `scriptId`. - Parameters: - `projectName` (string) - - `moduleName` (string) -
 - `scriptName` (string) - - `scriptId` (string) - - `paginationToken` (string)
 - - `verbose` (boolean) - --- ### `Encoder` resource  #### Product Description
 Out Delivery endpoints put the finishing touches on your mixed audio assets.
 Our encoder can be used to convert your file into a different format i.e.
 `mp3`. Our connector endpoints allow you to publish these assets onwards. --- -
 `create()` Changes the audio encoding of a mixed audio file ```
-audiostack.Delivery.Encoder.create()``` For most use cases, the preset can be
-either `custom` or one of the values returned from the `/encoder/presets` list.
-When using `custom` the other fields can be supplied. Please note not all
+audiostack.Delivery.Encoder.encode_mix()``` For most use cases, the preset can
+be either `custom` or one of the values returned from the `/encoder/presets`
+list. When using `custom` the other fields can be supplied. Please note not all
 fields are supported in conjunction with one another. For example `sampleRate`
 cannot be used in conjunction with `bitRateType`. - Parameters: -
 `productionId` *[required] (string) - Reference to the productionId that is to
 be encoded - `preset` (string) - named preset to use or 'custom' - `public`
 (boolean) - Make the output a publicly available URL - `bitRateType` (string) -
 Supplied value must be either 'constant' or 'variable - `bitRate` (string) -
 Can be between 0-9 for variable bit rates, or between 32 and 320 for constant
 bit rates - `sampleRate` (int) - Sample rate, should be between 24000 and 96000
 - `format` (string) - Can be wav, mp3, flac or ogg - `bitDepth` (int) - Can be
 16, 24, or 32 - `channels` (int) - Supply 1 for mono or 2 for stereo -
-`masteringPreset` (string) - Mastering preset to use, for example heavyDucking.
----
+`loudnessPreset` (string) - Loudness standard to use, for example spotify or
+podcast. --- - `list()` Lists available encoder presets. ```
+audiostack.Delivery.Encoder.list_presets()``` Returns a list of encoding
+presets, for example mp3, wav for alexa, wav 48kHz and a description of these.
+In addition, returns a list of loudness presets which match the loudness
+specifications for apple podcasting, spotify advertising and other. ---
```

### Comparing `audiostack-0.0.7/audiostack/content/media.py` & `audiostack-0.0.9/audiostack/content/media.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.7/audiostack/content/root_functions.py` & `audiostack-0.0.9/audiostack/content/root_functions.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.7/audiostack/content/script.py` & `audiostack-0.0.9/audiostack/content/script.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.7/audiostack/docs/docs.py` & `audiostack-0.0.9/audiostack/docs/docs.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.7/audiostack/helpers/api_item.py` & `audiostack-0.0.9/audiostack/helpers/api_item.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import json
 
 
 class APIResponseItem:
     def __init__(self, response):
         self.response = response
-
+        self.status_code = response["statusCode"]
+        
         if "data" in response:
             self.data = self.response["data"]
         if "message" in response:
             self.message = self.response["message"]
         if "meta" in response:
             self.meta = self.response["meta"]
-
-            # for key in self.data:
-            #     assert key != "data"
-            #     self.__dict__[key] = self.data["key"]
+        if "bytes" in response:
+            self.bytes = self.response["bytes"]
 
     def print_response(self, indent=0):
         if indent:
             return json.dumps(self.response, indent=indent)
         else:
             return self.response
 
     def __str__(self) -> str:
-        return json.dumps(self.response)
+        if hasattr(self, "bytes"):
+            return "bytes object"
+        else:
+            return json.dumps(self.response)
```

### Comparing `audiostack-0.0.7/audiostack/helpers/api_list.py` & `audiostack-0.0.9/audiostack/helpers/api_list.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.7/audiostack/helpers/request_interface.py` & `audiostack-0.0.9/audiostack/helpers/request_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,33 +40,41 @@
             # "x-assume-org": audiostack.assume_org_id,
         }
 
     def resolve_response(self, r):
         if r.status_code >= 500:
             print(r)
             raise Exception("Internal server error - aborting")
-
-        if self.DEBUG_PRINT:
-            print(json.dumps(r.json(), indent=4))
-
-        if "meta" in r.json():
-            if "creditsUsed" in r.json()["meta"]:
-                audiostack.billing_session += r.json()["meta"]["creditsUsed"]
-
+        
         if r.status_code == 403:
             raise Exception("Not authorised - check API key is valid")
 
         if r.status_code >= 400:
             msg = (
                 r.json()["message"]
                 + ". Errors listed as follows: \n\t"
                 + "\t".join(r.json()["errors"])
             )
             raise Exception(msg)
 
+        # if isinstance(r.content, bytes):
+        #     if self.DEBUG_PRINT:
+        #         print("Is bytes")
+        #     return {
+        #         "bytes" : r.content,
+        #         "statusCode" : r.status_code
+        #     }
+            
+        # else:
+        if self.DEBUG_PRINT:
+            print(json.dumps(r.json(), indent=4))
+        if "meta" in r.json():
+            if "creditsUsed" in r.json()["meta"]:
+                audiostack.billing_session += r.json()["meta"]["creditsUsed"]
+
         return {**r.json(), **{"statusCode": r.status_code}}
 
     def send_upload_request(self, local_path, upload_url):
         with open(local_path, "rb") as data:
             r = requests.put(url=upload_url, data=data)
 
             if r.status_code >= 400:
```

### Comparing `audiostack-0.0.7/audiostack/production/mix.py` & `audiostack-0.0.9/audiostack/production/mix.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     class List(APIResponseList):
         def __init__(self, response, list_type) -> None:
             super().__init__(response, list_type)
 
         def resolve_item(self, list_type, item):
             if list_type == "productionIds":
                 return Mix.Item({"data": item})
+            elif list_type == "presets":
+                return
+
             else:
                 raise Exception()
 
     @staticmethod
     def create(
         speechId="",
         speechItem=None,
@@ -48,15 +51,16 @@
         mediaFiles: dict = {},
         fxFiles: dict = {},
         sectionProperties: dict = {},
         timelineProperties: dict = {},
         masteringPreset: str = "",
         public: bool = False,
         exportSettings: dict = {},
-        strictValidation: bool = True
+        strictValidation: bool = True,
+        validate: bool = False
     ) -> Item:
         if speechId and speechItem:
             raise Exception("speechId or scriptItem should be supplied not both")
         if not (speechId or speechItem):
             raise Exception("speechId or scriptItem should be supplied")
         if speechItem:
             speechId = speechItem.speechId
@@ -75,16 +79,19 @@
             "sectionProperties": sectionProperties,
             "timelineProperties": timelineProperties,
             "masteringPreset": masteringPreset,
             "public": public,
             "exportSettings" : exportSettings,
             "strictValidation" : strictValidation
         }
-
-        r = Mix.interface.send_request(rtype=RequestTypes.POST, route="mix", json=body)
+        if validate:
+            r = Mix.interface.send_request(rtype=RequestTypes.POST, route="validate", json=body)
+        else:
+            r = Mix.interface.send_request(rtype=RequestTypes.POST, route="mix", json=body)
+            
         while r["statusCode"] == 202:
             print("Response in progress please wait...")
             r = Mix.interface.send_request(
                 rtype=RequestTypes.GET, route="mix", path_parameters=r["data"]["productionId"]
             )
         
         return Mix.Item(r)
@@ -114,7 +121,14 @@
             "scriptId": scriptId,
         }
 
         r = Mix.interface.send_request(
             rtype=RequestTypes.GET, route="mixes", query_parameters=query_params
         )
         return Mix.List(r, list_type="productionIds")
+
+    @staticmethod
+    def list_presets() -> Item:
+        r = Mix.interface.send_request(
+            rtype=RequestTypes.GET, route="mix/presets", path_parameters=""
+        )
+        return Mix.List(response=r, list_type="presets")
```

### Comparing `audiostack-0.0.7/audiostack/production/sound.py` & `audiostack-0.0.9/audiostack/production/sound.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.7/audiostack/speech/diction.py` & `audiostack-0.0.9/audiostack/speech/diction.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.7/audiostack/speech/tts.py` & `audiostack-0.0.9/audiostack/speech/tts.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from audiostack.helpers.request_types import RequestTypes
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.helpers.api_list import APIResponseList
 
 
 class TTS:
     interface = RequestInterface(family="speech")
-
+    
     class Item(APIResponseItem):
         def __init__(self, response) -> None:
             super().__init__(response)
             self.speechId = self.data["speechId"]
 
         def download(self, autoName=False, fileName="", path="./") -> None:
             sections = self.data["sections"]
@@ -29,80 +29,83 @@
                 RequestInterface.download_url(
                     s["url"], destination=path, name=full_name
                 )
 
         def delete(self):
             return TTS.delete(self.speechId)
 
+    class BytesItem(APIResponseItem):
+        def __init__(self, response) -> None:
+            super().__init__(response)
+            self.bytes = response["bytes"]
+        # def download(self, autoName=False, fileName="default", path="./") -> None:
+        #     with open("")
+
+
+
     class List(APIResponseList):
         def __init__(self, response, list_type) -> None:
             super().__init__(response, list_type)
 
         def resolve_item(self, list_type, item):
             if list_type == "speechIds":
                 return TTS.Item({"data": item})
             else:
                 raise Exception()
 
+    class Section:
+        @staticmethod    
+        def create(
+            sectionToProduce,
+            scriptId="",
+            scriptItem=None,
+            voice: str = "",
+            speed: float = 1.0,
+            silencePadding: str = "",
+            audience: dict = {},
+            sections: dict = {},
+            voiceIntelligence: bool = False,
+            public: bool = False,
+            sync: bool = True,
+        ):
+            # (start) no modify
+            route = "tts/section"
+            return TTS._create(**locals())
+            # (end) modify
+
+    @staticmethod
+    def preview(text: str, voice: str):
+        body = {
+            "text" : text,
+            "voice" : voice
+        }
+        r = TTS.interface.send_request(
+            rtype=RequestTypes.POST, route="tts/preview", json=body
+        )
+        return TTS.BytesItem(r)
+
     @staticmethod
     def create(
         scriptId="",
         scriptItem=None,
         voice: str = "",
         speed: float = 1.0,
         silencePadding: str = "",
-        effect: str = "",
         audience: dict = {},
         sections: dict = {},
-        useDictionary: bool = False,
-        useTextNormalizer: bool = False,
+        voiceIntelligence: bool = False,
         public: bool = False,
         sync: bool = True,
     ) -> Item:
-        if scriptId and scriptItem:
-            raise Exception("scriptId or scriptItem should be supplied not both")
-        if not (scriptId or scriptItem):
-            raise Exception("scriptId or scriptItem should be supplied")
+        # (start) no modify
+        route = "tts"
+        return TTS._create(**locals())
+        # (end) modify
+        
 
-        if scriptItem:
-            scriptId = scriptItem.scriptId
-
-        if not isinstance(voice, str):
-            raise Exception("voice argument should be a string")
-        if not isinstance(effect, str):
-            raise Exception("effect argument should be a string")
-        if not isinstance(silencePadding, str):
-            raise Exception("silencePadding argument should be a string")
-        if not isinstance(useDictionary, bool):
-            raise Exception("useDictionary argument should be a boolean")
-        if not isinstance(useTextNormalizer, bool):
-            raise Exception("useTextNormaliser argument should be a boolean")
-
-        body = {
-            "scriptId": scriptId,
-            "voice": voice,
-            "speed": speed,
-            "silencePadding": silencePadding,
-            "effect": effect,
-            "audience": audience,
-            "sections": sections,
-            "useDictionary": useDictionary,
-            "useTextNormalizer": useTextNormalizer,
-            "public": public,
-            "sync": sync,
-        }
-
-        r = TTS.interface.send_request(rtype=RequestTypes.POST, route="tts", json=body)
-        while r["statusCode"] == 202:
-            print("Response in progress please wait...")
-            r = TTS.interface.send_request(
-                rtype=RequestTypes.GET, route="tts", path_parameters=r["data"]["speechId"]   
-            )
-            
-        return TTS.Item(r)
 
     @staticmethod
     def get(speechId: str) -> Item:
         r = TTS.interface.send_request(
             rtype=RequestTypes.GET, route="tts", path_parameters=speechId
         )
         return TTS.Item(r)
@@ -124,7 +127,60 @@
             "scriptName": scriptName,
             "scriptId": scriptId,
         }
         r = TTS.interface.send_request(
             rtype=RequestTypes.GET, route="tts", query_parameters=query_params
         )
         return TTS.List(r, list_type="speechIds")
+
+
+    @staticmethod
+    def _create(
+        route: str,
+        scriptId="",
+        scriptItem=None,
+        voice: str = "",
+        speed: float = 1.0,
+        silencePadding: str = "",
+        audience: dict = {},
+        sections: dict = {},
+        voiceIntelligence: bool = False,
+        public: bool = False,
+        sync: bool = True,
+        sectionToProduce: str = ""
+    ):
+        if scriptId and scriptItem:
+            raise Exception("scriptId or scriptItem should be supplied not both")
+        if not (scriptId or scriptItem):
+            raise Exception("scriptId or scriptItem should be supplied")
+
+        if scriptItem:
+            scriptId = scriptItem.scriptId
+
+        if not isinstance(voice, str):
+            raise Exception("voice argument should be a string")
+        if not isinstance(silencePadding, str):
+            raise Exception("silencePadding argument should be a string")
+
+
+        body = {
+            "scriptId": scriptId,
+            "voice": voice,
+            "speed": speed,
+            "silencePadding": silencePadding,
+            "audience": audience,
+            "sections": sections,
+            "voiceIntelligence": voiceIntelligence,
+            "public": public,
+            "sync": sync,
+        }
+        if sectionToProduce:
+            body["sectionToProduce"] = sectionToProduce
+
+        r = TTS.interface.send_request(rtype=RequestTypes.POST, route="tts", json=body)
+        while r["statusCode"] == 202:
+            print("Response in progress please wait...")
+            r = TTS.interface.send_request(
+                rtype=RequestTypes.GET, route=route, path_parameters=r["data"]["speechId"]   
+            )
+            
+        return TTS.Item(r)
```

### Comparing `audiostack-0.0.7/audiostack/speech/voice.py` & `audiostack-0.0.9/audiostack/speech/voice.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.7/audiostack.egg-info/SOURCES.txt` & `audiostack-0.0.9/audiostack.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 audiostack/__init__.py
 audiostack.egg-info/PKG-INFO
 audiostack.egg-info/SOURCES.txt
 audiostack.egg-info/dependency_links.txt
 audiostack.egg-info/requires.txt
@@ -24,10 +25,8 @@
 audiostack/orchestrator/__init__.py
 audiostack/production/__init__.py
 audiostack/production/mix.py
 audiostack/production/sound.py
 audiostack/speech/__init__.py
 audiostack/speech/diction.py
 audiostack/speech/tts.py
-audiostack/speech/voice.py
-tests/__init__.py
-tests/test_audience.py
+audiostack/speech/voice.py
```

### Comparing `audiostack-0.0.7/setup.py` & `audiostack-0.0.9/setup.py`

 * *Files identical despite different names*

