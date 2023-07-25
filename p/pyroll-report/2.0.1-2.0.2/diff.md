# Comparing `tmp/pyroll_report-2.0.1.tar.gz` & `tmp/pyroll_report-2.0.2.tar.gz`

## Comparing `pyroll_report-2.0.1.tar` & `pyroll_report-2.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/__init__.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/cli.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/config.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/hookspecs.py
--rw-r--r--   0        0        0    22453 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/main.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/pluggy.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/report.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/utils.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/unit_display/__init__.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/unit_display/format.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/unit_display/format_guards.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/unit_display/format_special_numbers.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/unit_display/plots.html
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/unit_display/plots.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/unit_display/properties.html
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/unit_display/properties.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyroll/report/unit_display/units.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/.gitignore
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/LICENSE
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/README.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/hatch.toml
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 pyroll_report-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/__init__.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/cli.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/config.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/hookspecs.py
+-rw-r--r--   0        0        0    22453 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/main.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/pluggy.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/report.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/utils.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/unit_display/__init__.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/unit_display/format.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/unit_display/format_guards.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/unit_display/format_special_numbers.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/unit_display/plots.html
+-rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/unit_display/plots.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/unit_display/properties.html
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/unit_display/properties.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyroll/report/unit_display/units.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/LICENSE
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/README.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/hatch.toml
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 pyroll_report-2.0.2/PKG-INFO
```

### Comparing `pyroll_report-2.0.1/pyroll/report/cli.py` & `pyroll_report-2.0.2/pyroll/report/cli.py`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/pyroll/report/config.py` & `pyroll_report-2.0.2/pyroll/report/config.py`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/pyroll/report/hookspecs.py` & `pyroll_report-2.0.2/pyroll/report/hookspecs.py`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/pyroll/report/main.html` & `pyroll_report-2.0.2/pyroll/report/main.html`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/pyroll/report/report.py` & `pyroll_report-2.0.2/pyroll/report/report.py`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/pyroll/report/utils.py` & `pyroll_report-2.0.2/pyroll/report/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,18 @@
 def plot_shapely_geom(geom: shapely.Geometry):
     fig: plt.Figure = plt.figure(figsize=(2, 2))
     ax: plt.Axes = fig.add_subplot()
     ax.axis("off")
     ax.set_aspect("equal")
     fig.patch.set_alpha(0)
 
-    if isinstance(geom, shapely.LineString):
-        ax.plot(*geom.xy, c="k")
-    elif isinstance(geom, shapely.Polygon):
-        ax.fill(*geom.boundary.xy, c="k", alpha=0.5)
-        ax.fill(*geom.boundary.xy, c="k", fill=False)
+    try:
+        if isinstance(geom, shapely.LineString):
+            ax.plot(*geom.xy, c="k")
+        elif isinstance(geom, shapely.Polygon):
+            ax.fill(*geom.boundary.xy, c="k", alpha=0.5)
+            ax.fill(*geom.boundary.xy, c="k", fill=False)
+    except NotImplementedError:
+        return ""
 
-    fig.set_constrained_layout(True)
+    fig.set_layout_engine('constrained')
     return resize_svg_to_100_percent(get_svg_from_figure(fig))
```

### Comparing `pyroll_report-2.0.1/pyroll/report/unit_display/format.py` & `pyroll_report-2.0.2/pyroll/report/unit_display/format.py`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/pyroll/report/unit_display/format_guards.py` & `pyroll_report-2.0.2/pyroll/report/unit_display/format_guards.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,24 @@
 @hookimpl(specname="property_format")
 def do_not_print_points(name: str):
     if "points" in name:
         raise DoNotPrint()
 
 
 @hookimpl(specname="property_format")
+def do_not_print_additional_cross_sections(name: str):
+    if name in [
+        "displaced_cross_section",
+        "reappearing_cross_section"
+    ]:
+        raise DoNotPrint()
+
+
+
+@hookimpl(specname="property_format")
 def do_not_print_roll_surface(name: str):
     if name in [
         "surface_x",
         "surface_y",
         "surface_z"
     ]:
         raise DoNotPrint()
```

### Comparing `pyroll_report-2.0.1/pyroll/report/unit_display/format_special_numbers.py` & `pyroll_report-2.0.2/pyroll/report/unit_display/format_special_numbers.py`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/pyroll/report/unit_display/plots.py` & `pyroll_report-2.0.2/pyroll/report/unit_display/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,10 +161,10 @@
         ipr = ax.fill(*unit.in_profile.equivalent_rectangle.boundary.xy, fill=False, color="red", ls="--",
                       label="in eq. rectangle")
         opr = ax.fill(*unit.out_profile.equivalent_rectangle.boundary.xy, fill=False, color="blue", ls="--",
                       label="out eq. rectangle")
 
         axl.axis("off")
         axl.legend(handles=c + ipp + opp + ipr + opr, ncols=2, loc="lower center")
-        fig.set_constrained_layout(True)
+        fig.set_layout_engine('constrained')
 
         return fig
```

### Comparing `pyroll_report-2.0.1/pyroll/report/unit_display/properties.py` & `pyroll_report-2.0.2/pyroll/report/unit_display/properties.py`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/pyroll/report/unit_display/units.py` & `pyroll_report-2.0.2/pyroll/report/unit_display/units.py`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/.gitignore` & `pyroll_report-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/LICENSE` & `pyroll_report-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/pyproject.toml` & `pyroll_report-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyroll_report-2.0.1/PKG-INFO` & `pyroll_report-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroll-report
-Version: 2.0.1
+Version: 2.0.2
 Summary: PyRoll rolling simulation framework - HTML report generation.
 Project-URL: Homepage, https://pyroll-project.github.io
 Project-URL: Repository, https://github.com/pyroll-project/pyroll-core
 Project-URL: Documentation, https://pyroll.readthedocs.io/en/latest
 Author-email: Max Weiner <max.weiner@imf.tu-freiberg.de>, Christoph Renzing <christoph.renzing@imf.tu-freiberg.de>, Matthias Schmidtchen <matthias.schmidtchen@imf.tu-freiberg.de>, Max Stirl <max.stirl@imf.tu-freiberg.de>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
```

