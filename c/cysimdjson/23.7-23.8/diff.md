# Comparing `tmp/cysimdjson-23.7.tar.gz` & `tmp/cysimdjson-23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cysimdjson-23.7.tar", last modified: Thu Jul 20 10:41:23 2023, max compression
+gzip compressed data, was "cysimdjson-23.8.tar", last modified: Tue Jul 25 09:27:22 2023, max compression
```

## Comparing `cysimdjson-23.7.tar` & `cysimdjson-23.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:41:23.000000 cysimdjson-23.7/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-07-20 09:13:36.000000 cysimdjson-23.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7803 2023-07-20 10:41:23.000000 cysimdjson-23.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6835 2023-07-20 10:34:30.000000 cysimdjson-23.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:41:23.000000 cysimdjson-23.7/cysimdjson/
--rw-r--r--   0 root         (0) root         (0)      801 2023-07-20 09:13:36.000000 cysimdjson-23.7/cysimdjson/__init__.py
--rw-r--r--   0 root         (0) root         (0)   761904 2023-07-20 10:41:22.000000 cysimdjson-23.7/cysimdjson/cysimdjson.cpp
--rw-r--r--   0 root         (0) root         (0)     2174 2023-07-20 10:41:22.000000 cysimdjson-23.7/cysimdjson/cysimdjson.h
--rw-r--r--   0 root         (0) root         (0)    11759 2023-07-20 10:34:30.000000 cysimdjson-23.7/cysimdjson/cysimdjson.pyx
--rw-r--r--   0 root         (0) root         (0)     5210 2023-07-20 09:13:36.000000 cysimdjson-23.7/cysimdjson/cysimdjsonc.cpp
--rw-r--r--   0 root         (0) root         (0)     1303 2023-07-20 09:13:36.000000 cysimdjson-23.7/cysimdjson/cysimdjsonc.h
--rw-r--r--   0 root         (0) root         (0)     1044 2023-07-20 09:51:03.000000 cysimdjson-23.7/cysimdjson/jsoninter.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:41:23.000000 cysimdjson-23.7/cysimdjson/pysimdjson/
--rw-r--r--   0 root         (0) root         (0)     2783 2023-07-20 09:13:36.000000 cysimdjson-23.7/cysimdjson/pysimdjson/errors.cpp
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-20 09:13:36.000000 cysimdjson-23.7/cysimdjson/pysimdjson/errors.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:41:23.000000 cysimdjson-23.7/cysimdjson/simdjson/
--rw-r--r--   0 root         (0) root         (0)   690133 2023-07-20 09:51:03.000000 cysimdjson-23.7/cysimdjson/simdjson/simdjson.cpp
--rw-r--r--   0 root         (0) root         (0)  1295372 2023-07-20 09:51:03.000000 cysimdjson-23.7/cysimdjson/simdjson/simdjson.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 10:41:23.000000 cysimdjson-23.7/cysimdjson.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7803 2023-07-20 10:41:22.000000 cysimdjson-23.7/cysimdjson.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      489 2023-07-20 10:41:22.000000 cysimdjson-23.7/cysimdjson.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 10:41:22.000000 cysimdjson-23.7/cysimdjson.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-20 10:41:22.000000 cysimdjson-23.7/cysimdjson.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-20 09:13:36.000000 cysimdjson-23.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-20 10:41:23.000000 cysimdjson-23.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2143 2023-07-20 10:34:30.000000 cysimdjson-23.7/setup.py
+drwxr-xr-x   0 ateska     (501) staff       (20)        0 2023-07-25 09:27:22.178354 cysimdjson-23.8/
+-rw-r--r--   0 ateska     (501) staff       (20)    11343 2023-07-20 09:13:36.000000 cysimdjson-23.8/LICENSE
+-rw-r--r--   0 ateska     (501) staff       (20)     7803 2023-07-25 09:27:22.178479 cysimdjson-23.8/PKG-INFO
+-rw-r--r--   0 ateska     (501) staff       (20)     6835 2023-07-20 10:34:30.000000 cysimdjson-23.8/README.md
+drwxr-xr-x   0 ateska     (501) staff       (20)        0 2023-07-25 09:27:22.166879 cysimdjson-23.8/cysimdjson/
+-rw-r--r--   0 ateska     (501) staff       (20)      801 2023-07-20 09:13:36.000000 cysimdjson-23.8/cysimdjson/__init__.py
+-rw-r--r--   0 ateska     (501) staff       (20)   761904 2023-07-20 10:44:55.000000 cysimdjson-23.8/cysimdjson/cysimdjson.cpp
+-rw-r--r--   0 ateska     (501) staff       (20)     2174 2023-07-20 10:44:55.000000 cysimdjson-23.8/cysimdjson/cysimdjson.h
+-rw-r--r--   0 ateska     (501) staff       (20)    11759 2023-07-20 10:34:30.000000 cysimdjson-23.8/cysimdjson/cysimdjson.pyx
+-rw-r--r--   0 ateska     (501) staff       (20)     5590 2023-07-23 20:50:02.000000 cysimdjson-23.8/cysimdjson/cysimdjsonc.cpp
+-rw-r--r--   0 ateska     (501) staff       (20)     1514 2023-07-23 20:50:29.000000 cysimdjson-23.8/cysimdjson/cysimdjsonc.h
+-rw-r--r--   0 ateska     (501) staff       (20)     1044 2023-07-20 09:51:03.000000 cysimdjson-23.8/cysimdjson/jsoninter.h
+drwxr-xr-x   0 ateska     (501) staff       (20)        0 2023-07-25 09:27:22.169855 cysimdjson-23.8/cysimdjson/pysimdjson/
+-rw-r--r--   0 ateska     (501) staff       (20)     2783 2023-07-20 09:13:36.000000 cysimdjson-23.8/cysimdjson/pysimdjson/errors.cpp
+-rw-r--r--   0 ateska     (501) staff       (20)      178 2023-07-20 09:13:36.000000 cysimdjson-23.8/cysimdjson/pysimdjson/errors.h
+drwxr-xr-x   0 ateska     (501) staff       (20)        0 2023-07-25 09:27:22.174395 cysimdjson-23.8/cysimdjson/simdjson/
+-rw-r--r--   0 ateska     (501) staff       (20)   690133 2023-07-20 09:51:03.000000 cysimdjson-23.8/cysimdjson/simdjson/simdjson.cpp
+-rw-r--r--   0 ateska     (501) staff       (20)  1295372 2023-07-20 09:51:03.000000 cysimdjson-23.8/cysimdjson/simdjson/simdjson.h
+drwxr-xr-x   0 ateska     (501) staff       (20)        0 2023-07-25 09:27:22.168692 cysimdjson-23.8/cysimdjson.egg-info/
+-rw-r--r--   0 ateska     (501) staff       (20)     7803 2023-07-25 09:27:22.000000 cysimdjson-23.8/cysimdjson.egg-info/PKG-INFO
+-rw-r--r--   0 ateska     (501) staff       (20)      489 2023-07-25 09:27:22.000000 cysimdjson-23.8/cysimdjson.egg-info/SOURCES.txt
+-rw-r--r--   0 ateska     (501) staff       (20)        1 2023-07-25 09:27:22.000000 cysimdjson-23.8/cysimdjson.egg-info/dependency_links.txt
+-rw-r--r--   0 ateska     (501) staff       (20)       11 2023-07-25 09:27:22.000000 cysimdjson-23.8/cysimdjson.egg-info/top_level.txt
+-rw-r--r--   0 ateska     (501) staff       (20)       60 2023-07-20 09:13:36.000000 cysimdjson-23.8/pyproject.toml
+-rw-r--r--   0 ateska     (501) staff       (20)       82 2023-07-25 09:27:22.179048 cysimdjson-23.8/setup.cfg
+-rw-r--r--   0 ateska     (501) staff       (20)     2140 2023-07-25 09:17:23.000000 cysimdjson-23.8/setup.py
```

### Comparing `cysimdjson-23.7/LICENSE` & `cysimdjson-23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cysimdjson-23.7/PKG-INFO` & `cysimdjson-23.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cysimdjson
-Version: 23.7
+Version: 23.8
 Summary: High-speed JSON parser
 Home-page: https://github.com/TeskaLabs/cysimdjson
 Author: TeskaLabs Ltd
 Author-email: info@teskalabs.com
 Project-URL: Source, https://github.com/TeskaLabs/cysimdjson
 Project-URL: Tracker, https://github.com/TeskaLabs/cysimdjson/issues
 Platform: any
```

### Comparing `cysimdjson-23.7/README.md` & `cysimdjson-23.8/README.md`

 * *Files identical despite different names*

### Comparing `cysimdjson-23.7/cysimdjson/__init__.py` & `cysimdjson-23.8/cysimdjson/__init__.py`

 * *Files identical despite different names*

### Comparing `cysimdjson-23.7/cysimdjson/cysimdjson.cpp` & `cysimdjson-23.8/cysimdjson/cysimdjson.cpp`

 * *Files identical despite different names*

### Comparing `cysimdjson-23.7/cysimdjson/cysimdjson.h` & `cysimdjson-23.8/cysimdjson/cysimdjson.h`

 * *Files identical despite different names*

### Comparing `cysimdjson-23.7/cysimdjson/cysimdjson.pyx` & `cysimdjson-23.8/cysimdjson/cysimdjson.pyx`

 * *Files identical despite different names*

### Comparing `cysimdjson-23.7/cysimdjson/cysimdjsonc.cpp` & `cysimdjson-23.8/cysimdjson/cysimdjsonc.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -182,7 +182,20 @@
 	auto error = parser.parse(jsond, jsond_len).get(object);
 	if (error) {
 		return -1;
 	}
 	
 	return 0;
 }
+
+
+size_t cysimdjson_minify(void * e, char * buffer, size_t buffer_size) {
+	simdjson::dom::element * element = static_cast<simdjson::dom::element *>(e);
+	std::string json_string = simdjson::minify(*element);
+
+	if (json_string.size() < buffer_size) {
+		std::strcpy(buffer, json_string.c_str());
+		return json_string.size();
+	} else {
+		return 0; // The output JSON doesn't fit
+	}
+}
```

### Comparing `cysimdjson-23.7/cysimdjson/cysimdjsonc.h` & `cysimdjson-23.8/cysimdjson/cysimdjsonc.h`

 * *Files 17% similar despite different names*

```diff
@@ -23,8 +23,12 @@
 bool cysimdjson_element_get_double(const char * attrname, size_t attrlen, void * element, double * output);
 
 char cysimdjson_element_get_type(const char * attrname, size_t attrlen, void * element);
 bool cysimdjson_element_get(const char * attrname, size_t attrlen, void * element, void * output_element);
 
 int cysimdjson_parser_test(void);
 
+// Export element `e` as JSON into the "buffer" and returns the exported JSON size.
+// If the "buffer_size" is too small, returns 0;
+size_t cysimdjson_minify(void * element, char * buffer, size_t buffer_size);
+
 #endif
```

### Comparing `cysimdjson-23.7/cysimdjson/jsoninter.h` & `cysimdjson-23.8/cysimdjson/jsoninter.h`

 * *Files identical despite different names*

### Comparing `cysimdjson-23.7/cysimdjson/pysimdjson/errors.cpp` & `cysimdjson-23.8/cysimdjson/pysimdjson/errors.cpp`

 * *Files identical despite different names*

### Comparing `cysimdjson-23.7/cysimdjson/simdjson/simdjson.cpp` & `cysimdjson-23.8/cysimdjson/simdjson/simdjson.cpp`

 * *Files identical despite different names*

### Comparing `cysimdjson-23.7/cysimdjson/simdjson/simdjson.h` & `cysimdjson-23.8/cysimdjson/simdjson/simdjson.h`

 * *Files identical despite different names*

### Comparing `cysimdjson-23.7/cysimdjson.egg-info/PKG-INFO` & `cysimdjson-23.8/cysimdjson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cysimdjson
-Version: 23.7
+Version: 23.8
 Summary: High-speed JSON parser
 Home-page: https://github.com/TeskaLabs/cysimdjson
 Author: TeskaLabs Ltd
 Author-email: info@teskalabs.com
 Project-URL: Source, https://github.com/TeskaLabs/cysimdjson
 Project-URL: Tracker, https://github.com/TeskaLabs/cysimdjson/issues
 Platform: any
```

### Comparing `cysimdjson-23.7/setup.py` & `cysimdjson-23.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,24 @@
 			'cysimdjson/pysimdjson/errors.cpp',
 			'cysimdjson/cysimdjsonc.cpp',
 		],
 		language="c++",
 		extra_compile_args=[
 			"-std=c++17",  # for std::string_view class that became standard in C++17
 			"-Wno-deprecated",
-		# NOTE Windows doesn't know how to handle "-Wno-deprecated"		
-		] if sys.platform != "win32" else [
+		] if sys.platform != "win32" else [  # NOTE Windows doesn't know how to handle "-Wno-deprecated"
 			"/std:c++17",
 		],
 		define_macros=[("CYTHON_EXTERN_C", 'extern "C"')],  # https://cython.readthedocs.io/en/latest/src/userguide/external_C_code.html#c-public-declarations
 	)
 ]
 
 setup(
 	name='cysimdjson',
-	version="23.07",
+	version="23.08",
 	description='High-speed JSON parser',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	author='TeskaLabs Ltd',
 	author_email='info@teskalabs.com',
 	platforms='any',
 	classifiers=[
```

