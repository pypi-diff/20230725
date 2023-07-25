# Comparing `tmp/peakrdl-euvm-1.1.tar.gz` & `tmp/peakrdl-euvm-1.2.tar.gz`

## Comparing `peakrdl-euvm-1.1.tar` & `peakrdl-euvm-1.2.tar`

### file list

```diff
@@ -1,44 +1,38 @@
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 11:10:12.000000 peakrdl-euvm-1.1/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/
--rwxrwxr-x   0 kun       (1000) kun       (1000)      888 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/run.sh
--rw-rw-r--   0 kun       (1000) kun       (1000)    18135 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/pylint.rc
--rw-rw-r--   0 kun       (1000) kun       (1000)       21 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/.gitignore
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/testcases/
--rw-rw-r--   0 kun       (1000) kun       (1000)     1320 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/testcases/basic.rdl
--rw-rw-r--   0 kun       (1000) kun       (1000)       11 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/testcases/.gitignore
--rwxrwxr-x   0 kun       (1000) kun       (1000)      366 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/vsim_test.sh
--rwxrwxr-x   0 kun       (1000) kun       (1000)      374 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/rdl_to_uvm.py
--rw-rw-r--   0 kun       (1000) kun       (1000)     4060 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/test/generate_testcase_data.py
--rw-rw-r--   0 kun       (1000) kun       (1000)     2508 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/README.md
--rw-rw-r--   0 kun       (1000) kun       (1000)     1893 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/setup.py
--rw-rw-r--   0 kun       (1000) kun       (1000)       72 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/MANIFEST.in
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 11:03:55.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/
--rw-rw-r--   0 kun       (1000) kun       (1000)     1816 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__peakrdl__.py
--rw-rw-r--   0 kun       (1000) kun       (1000)       20 2023-07-24 11:03:32.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__about__.py
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 10:49:09.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/
--rw-rw-r--   0 kun       (1000) kun       (1000)     3411 2023-07-24 10:48:59.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_reg_block-mem.d
--rw-rw-r--   0 kun       (1000) kun       (1000)     2509 2023-07-24 10:28:39.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_vreg.d
--rw-rw-r--   0 kun       (1000) kun       (1000)      893 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/main.d
--rw-rw-r--   0 kun       (1000) kun       (1000)     5472 2023-07-24 10:49:09.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_reg.d
--rw-rw-r--   0 kun       (1000) kun       (1000)     1369 2023-07-24 10:10:13.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/utils.d
--rw-rw-r--   0 kun       (1000) kun       (1000)      119 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/top_include.d
--rw-rw-r--   0 kun       (1000) kun       (1000)      212 2023-07-24 10:29:29.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/top_pkg.d
--rw-rw-r--   0 kun       (1000) kun       (1000)     3996 2023-07-24 10:48:38.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_reg_block.d
--rw-rw-r--   0 kun       (1000) kun       (1000)       71 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__init__.py
--rw-rw-r--   0 kun       (1000) kun       (1000)     1255 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/pre_export_listener.py
--rw-rw-r--   0 kun       (1000) kun       (1000)    15683 2023-07-24 10:45:31.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/exporter.py
-drwxrwxr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 10:49:45.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/
--rw-rw-r--   0 kun       (1000) kun       (1000)     1908 2023-07-24 10:33:36.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/pre_export_listener.cpython-38.pyc
--rw-rw-r--   0 kun       (1000) kun       (1000)      227 2023-07-24 10:33:36.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 kun       (1000) kun       (1000)    10802 2023-07-24 10:49:45.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/exporter.cpython-38.pyc
--rw-rw-r--   0 kun       (1000) kun       (1000)     1899 2023-07-24 10:33:36.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/__peakrdl__.cpython-38.pyc
--rw-rw-r--   0 kun       (1000) kun       (1000)      157 2023-07-24 10:33:36.000000 peakrdl-euvm-1.1/src/peakrdl_euvm/__pycache__/__about__.cpython-38.pyc
-drwxr-xr-x   0 kun       (1000) kun       (1000)        0 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/
--rw-r--r--   0 kun       (1000) kun       (1000)      752 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/SOURCES.txt
--rw-r--r--   0 kun       (1000) kun       (1000)       13 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/top_level.txt
--rw-r--r--   0 kun       (1000) kun       (1000)        1 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/dependency_links.txt
--rw-r--r--   0 kun       (1000) kun       (1000)     3751 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/PKG-INFO
--rw-r--r--   0 kun       (1000) kun       (1000)       62 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/entry_points.txt
--rw-r--r--   0 kun       (1000) kun       (1000)       34 2023-07-24 11:09:15.000000 peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/requires.txt
--rw-rw-r--   0 kun       (1000) kun       (1000)    35149 2023-07-24 10:07:07.000000 peakrdl-euvm-1.1/LICENSE
+drwxrwxr-x   0 puneet    (1000) puneet    (1000)        0 2023-07-25 06:30:21.000000 peakrdl-euvm-1.2/
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)    35149 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/LICENSE
+drwxrwxr-x   0 puneet    (1000) puneet    (1000)        0 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/test/
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)    18135 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/test/pylint.rc
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)       21 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/test/.gitignore
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     4060 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/test/generate_testcase_data.py
+-rwxrwxr-x   0 puneet    (1000) puneet    (1000)      888 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/test/run.sh
+-rwxrwxr-x   0 puneet    (1000) puneet    (1000)      374 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/test/rdl_to_uvm.py
+-rwxrwxr-x   0 puneet    (1000) puneet    (1000)      366 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/test/vsim_test.sh
+drwxrwxr-x   0 puneet    (1000) puneet    (1000)        0 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/test/testcases/
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)       11 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/test/testcases/.gitignore
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     1320 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/test/testcases/basic.rdl
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     1893 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/setup.py
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)       72 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/MANIFEST.in
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     2508 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/README.md
+drwxrwxr-x   0 puneet    (1000) puneet    (1000)        0 2023-07-25 06:29:53.000000 peakrdl-euvm-1.2/src/
+drwxrwxr-x   0 puneet    (1000) puneet    (1000)        0 2023-07-25 06:29:53.000000 peakrdl-euvm-1.2/src/peakrdl_euvm.egg-info/
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)        1 2023-07-25 06:29:53.000000 peakrdl-euvm-1.2/src/peakrdl_euvm.egg-info/dependency_links.txt
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)       13 2023-07-25 06:29:53.000000 peakrdl-euvm-1.2/src/peakrdl_euvm.egg-info/top_level.txt
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)       34 2023-07-25 06:29:53.000000 peakrdl-euvm-1.2/src/peakrdl_euvm.egg-info/requires.txt
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)      752 2023-07-25 06:29:53.000000 peakrdl-euvm-1.2/src/peakrdl_euvm.egg-info/SOURCES.txt
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     4348 2023-07-25 06:29:53.000000 peakrdl-euvm-1.2/src/peakrdl_euvm.egg-info/PKG-INFO
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)       62 2023-07-25 06:29:53.000000 peakrdl-euvm-1.2/src/peakrdl_euvm.egg-info/entry_points.txt
+drwxrwxr-x   0 puneet    (1000) puneet    (1000)        0 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)    15683 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/exporter.py
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     1255 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/pre_export_listener.py
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)       20 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/__about__.py
+drwxrwxr-x   0 puneet    (1000) puneet    (1000)        0 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/templates/
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     3666 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/templates/uvm_reg_block-mem.d
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     4269 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/templates/uvm_reg_block.d
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)      112 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/templates/top_include.d
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)      200 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/templates/top_pkg.d
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)      893 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/templates/main.d
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     5759 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/templates/uvm_reg.d
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     2453 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/templates/uvm_vreg.d
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     2139 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/templates/utils.d
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)       71 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/__init__.py
+-rw-rw-r--   0 puneet    (1000) puneet    (1000)     1816 2023-07-25 06:29:19.000000 peakrdl-euvm-1.2/src/peakrdl_euvm/__peakrdl__.py
```

### Comparing `peakrdl-euvm-1.1/test/run.sh` & `peakrdl-euvm-1.2/test/run.sh`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.1/test/pylint.rc` & `peakrdl-euvm-1.2/test/pylint.rc`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.1/test/testcases/basic.rdl` & `peakrdl-euvm-1.2/test/testcases/basic.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.1/test/generate_testcase_data.py` & `peakrdl-euvm-1.2/test/generate_testcase_data.py`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.1/README.md` & `peakrdl-euvm-1.2/README.md`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.1/setup.py` & `peakrdl-euvm-1.2/setup.py`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.1/src/peakrdl_euvm/__peakrdl__.py` & `peakrdl-euvm-1.2/src/peakrdl_euvm/__peakrdl__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.1/src/peakrdl_euvm/templates/main.d` & `peakrdl-euvm-1.2/src/peakrdl_euvm/templates/main.d`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.1/src/peakrdl_euvm/templates/uvm_reg.d` & `peakrdl-euvm-1.2/src/peakrdl_euvm/templates/uvm_reg.d`

 * *Files 13% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 {%- endmacro %}
 
 
 //------------------------------------------------------------------------------
 // new() function
 //------------------------------------------------------------------------------
 {% macro function_new(node) -%}
-this(string name = "{{get_class_name(node)}}"){
+this(string name = "{{get_class_name(node)}}") {
     super(name, {{node.get_property('regwidth')}}, UVM_NO_COVERAGE);
 }
 {%- endmacro %}
 
 
 //------------------------------------------------------------------------------
 // build() function
@@ -57,24 +57,27 @@
 
 
 //------------------------------------------------------------------------------
 // build() actions for uvm_reg instance (called by parent)
 //------------------------------------------------------------------------------
 {% macro build_instance(node) -%}
 {%- if node.is_array %}
-foreach (uint {{utils.array_iterator_list(node)}}, ref inst; this.{{get_inst_name(node)}}) {
-    {%- if use_uvm_factory %}
-    inst = {{get_class_name(node)}}.type_id.create(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
-    {%- else %}
-    inst = new {{get_class_name(node)}}(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
-    {%- endif %}
-    inst.configure(this);
-    {{add_hdl_path_slices(node, get_inst_name(node) + utils.array_iterator_suffix(node))|trim|indent}}
-    inst.build();
-    this.default_map.add_reg(inst, {{get_array_address_offset_expr(node)}});
+  {%- for dim in node.array_dimensions %}
+foreach (uint {{utils.array_iterator(loop.index0)}}, ref {{utils.array_element(node, loop.index0)}}; {{utils.array_subarray(node, loop.index0)}})
+  {%- if loop.last %} { {% endif -%}
+  {%- endfor -%}
+  {%- if use_uvm_factory %}
+  {{utils.array_elements_leaf(node)}} = {{get_class_name(node)}}.type_id.create(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
+  {%- else %}
+  {{utils.array_elements_leaf(node)}} = new {{get_class_name(node)}}(format("{{get_inst_name(node)}}{{utils.array_suffix_format(node)}}", {{utils.array_iterator_list(node)}}));
+  {%- endif %}
+  {{utils.array_elements_leaf(node)}}.configure(this);
+  {{add_hdl_path_slices(node, get_inst_name(node) + utils.array_iterator_suffix(node))|trim|indent}}
+  {{utils.array_elements_leaf(node)}}.build();
+  this.default_map.add_reg({{utils.array_elements_leaf(node)}}, {{get_array_address_offset_expr(node)}});
 }
 {%- else %}
 {%- if use_uvm_factory %}
 this.{{get_inst_name(node)}} = {{get_class_name(node)}}.type_id.create("{{get_inst_name(node)}}");
 {%- else %}
 this.{{get_inst_name(node)}} = new {{get_class_name(node)}}("{{get_inst_name(node)}}");
 {%- endif %}
```

### Comparing `peakrdl-euvm-1.1/src/peakrdl_euvm/pre_export_listener.py` & `peakrdl-euvm-1.2/src/peakrdl_euvm/pre_export_listener.py`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.1/src/peakrdl_euvm/exporter.py` & `peakrdl-euvm-1.2/src/peakrdl_euvm/exporter.py`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/SOURCES.txt` & `peakrdl-euvm-1.2/src/peakrdl_euvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peakrdl-euvm-1.1/src/peakrdl_euvm.egg-info/PKG-INFO` & `peakrdl-euvm-1.2/src/peakrdl_euvm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,93 @@
 Metadata-Version: 2.1
 Name: peakrdl-euvm
-Version: 1.1
+Version: 1.2
 Summary: Generate eUVM register model from compiled SystemRDL input
 Home-page: https://github.com/coverify/PeakRDL-euvm
 Author: Alex Mykyta, Jude Zhang
 License: UNKNOWN
 Project-URL: Source, https://github.com/coverify/PeakRDL-euvm
 Project-URL: Tracker, https://github.com/coverify/PeakRDL-euvm/issues
+Description: [![build](https://github.com/coverify/PeakRDL-euvm/workflows/build/badge.svg)](https://github.com/coverify/PeakRDL-euvm/actions?query=workflow%3Abuild+branch%3Amain)
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peakrdl-uvm.svg)](https://pypi.org/project/peakrdl-uvm)
+        
+        # PeakRDL-euvm
+        Generate eUVM register model from compiled SystemRDL input.
+        
+        For the command line tool, see the [PeakRDL project](https://peakrdl.readthedocs.io).
+        
+        ## Installing
+        Install from [PyPi](https://pypi.org/project/peakrdl-uvm) using pip:
+        
+            python3 -m pip install peakrdl-euvm
+        
+        --------------------------------------------------------------------------------
+        
+        ## Exporter Usage
+        Pass the elaborated output of the [SystemRDL Compiler](http://systemrdl-compiler.readthedocs.io)
+        to the exporter.
+        
+        ```python
+        import sys
+        from systemrdl import RDLCompiler, RDLCompileError
+        from peakrdl_euvm import eUVMExporter
+        
+        rdlc = RDLCompiler()
+        
+        try:
+            rdlc.compile_file("path/to/my.rdl")
+            root = rdlc.elaborate()
+        except RDLCompileError:
+            sys.exit(1)
+        
+        exporter = eUVMExporter()
+        exporter.export(root, "test.sv")
+        ```
+        --------------------------------------------------------------------------------
+        
+        ## Reference
+        
+        ### `eUVMExporter(**kwargs)`
+        Constructor for the eUVM Exporter class
+        
+        **Optional Parameters**
+        
+        * `user_template_dir`
+            * Path to a directory where user-defined template overrides are stored.
+        * `user_template_context`
+            * Additional context variables to load into the template namespace.
+        
+        ### `eUVMExporter.export(node, path, **kwargs)`
+        Perform the export!
+        
+        **Parameters**
+        
+        * `node`
+            * Top-level node to export. Can be the top-level `RootNode` or any internal `AddrmapNode`.
+        * `path`
+            * Output file.
+        
+        **Optional Parameters**
+        
+        * `export_as_package`
+            * If True (Default), eUVM register model is exported as a SystemVerilog
+              package. Package name is based on the output file name.
+            * If False, register model is exported as an includable header.
+        * `reuse_class_definitions`
+            * If True (Default), exporter attempts to re-use class definitions
+              where possible. Class names are based on the lexical scope of the
+              original SystemRDL definitions.
+            * If False, class definitions are not reused. Class names are based on
+              the instance's hierarchical path.
+        * `use_uvm_factory`
+            * If True, class definitions and class instances are created using the
+              UVM factory.
+            * If False (Default), UVM factory is disabled. Classes are created
+              directly via new() constructors.
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -20,87 +97,7 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![build](https://github.com/coverify/PeakRDL-euvm/workflows/build/badge.svg)](https://github.com/coverify/PeakRDL-euvm/actions?query=workflow%3Abuild+branch%3Amain)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peakrdl-uvm.svg)](https://pypi.org/project/peakrdl-uvm)
-
-# PeakRDL-euvm
-Generate eUVM register model from compiled SystemRDL input.
-
-For the command line tool, see the [PeakRDL project](https://peakrdl.readthedocs.io).
-
-## Installing
-Install from [PyPi](https://pypi.org/project/peakrdl-uvm) using pip:
-
-    python3 -m pip install peakrdl-euvm
-
---------------------------------------------------------------------------------
-
-## Exporter Usage
-Pass the elaborated output of the [SystemRDL Compiler](http://systemrdl-compiler.readthedocs.io)
-to the exporter.
-
-```python
-import sys
-from systemrdl import RDLCompiler, RDLCompileError
-from peakrdl_euvm import eUVMExporter
-
-rdlc = RDLCompiler()
-
-try:
-    rdlc.compile_file("path/to/my.rdl")
-    root = rdlc.elaborate()
-except RDLCompileError:
-    sys.exit(1)
-
-exporter = eUVMExporter()
-exporter.export(root, "test.sv")
-```
---------------------------------------------------------------------------------
-
-## Reference
-
-### `eUVMExporter(**kwargs)`
-Constructor for the eUVM Exporter class
-
-**Optional Parameters**
-
-* `user_template_dir`
-    * Path to a directory where user-defined template overrides are stored.
-* `user_template_context`
-    * Additional context variables to load into the template namespace.
-
-### `eUVMExporter.export(node, path, **kwargs)`
-Perform the export!
-
-**Parameters**
-
-* `node`
-    * Top-level node to export. Can be the top-level `RootNode` or any internal `AddrmapNode`.
-* `path`
-    * Output file.
-
-**Optional Parameters**
-
-* `export_as_package`
-    * If True (Default), eUVM register model is exported as a SystemVerilog
-      package. Package name is based on the output file name.
-    * If False, register model is exported as an includable header.
-* `reuse_class_definitions`
-    * If True (Default), exporter attempts to re-use class definitions
-      where possible. Class names are based on the lexical scope of the
-      original SystemRDL definitions.
-    * If False, class definitions are not reused. Class names are based on
-      the instance's hierarchical path.
-* `use_uvm_factory`
-    * If True, class definitions and class instances are created using the
-      UVM factory.
-    * If False (Default), UVM factory is disabled. Classes are created
-      directly via new() constructors.
-
-
```

### Comparing `peakrdl-euvm-1.1/LICENSE` & `peakrdl-euvm-1.2/LICENSE`

 * *Files identical despite different names*

