# Comparing `tmp/nicescad-0.0.5.tar.gz` & `tmp/nicescad-0.0.6.tar.gz`

## Comparing `nicescad-0.0.5.tar` & `nicescad-0.0.6.tar`

### file list

```diff
@@ -1,73 +1,78 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.5/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.5/.pydevproject
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.5/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/file_selector.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/local_filepicker.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/nicescad_cmd.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/openscad.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/process.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/profiler.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/version.py
--rw-r--r--   0        0        0    14389 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/webserver.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 nicescad-0.0.5/nicescad/web/static/css/pygments.css
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/intersection.scad
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openjscad_logo.scad
--rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openjscad_logo.stl
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/GEB.scad
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/advance_intersection.scad
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/animation.scad
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/demo_cut.scad
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/difference.scad
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/fractal.scad
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/intersecting.scad
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/iteration.scad
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/module_recursion.scad
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/offset.scad
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/search.scad
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Advanced/translation.scad
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/CSG-modules.scad
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/CSG.scad
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/LetterBlock.scad
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/children.scad
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/children_indexed.scad
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/difference_cube.scad
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/difference_sphere.scad
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/intersection.scad
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/linear_extrude.scad
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/logo.scad
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/logo_and_text.scad
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/projection.scad
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/rotate_extrude.scad
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/surface.scad
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/surface_image.scad
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/text_on_cube.scad
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/translate.scad
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Basics/union.scad
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/cut_view.scad
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/fan_view.scad
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/text.scad
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Functions/functions.scad
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Functions/recursion.scad
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/chopped_blocks.scad
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/fence.scad
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/flat_body.scad
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/polyhedron.scad
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/rounded_box.scad
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/sphere.scad
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 nicescad-0.0.5/scad_examples/openscad_examples/Shapes/tripod.scad
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.5/scripts/doc
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.5/scripts/install
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 nicescad-0.0.5/scripts/openscad_example_scraper.py
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.5/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.5/tests/basetest.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nicescad-0.0.5/tests/test_file_selector.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nicescad-0.0.5/tests/test_openscad.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 nicescad-0.0.5/tests/test_subprocess.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nicescad-0.0.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.5/LICENSE
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 nicescad-0.0.5/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nicescad-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 nicescad-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nicescad-0.0.6/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nicescad-0.0.6/.pydevproject
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nicescad-0.0.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 nicescad-0.0.6/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/__init__.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/axes_helper.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/blockscad_converter.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/file_selector.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/local_filepicker.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/nicescad_cmd.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/openscad.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/process.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/profiler.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/version.py
+-rw-r--r--   0        0        0    16566 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/webserver.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad/web/static/css/pygments.css
+-rw-r--r--   0        0        0     7117 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/blockscad/A10BedLevelKnob.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/blockscad_converted/A10BedLevelKnob.scad
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/intersection.scad
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/openjscad_logo.scad
+-rw-r--r--   0        0        0   495635 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/openjscad_logo.stl
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/GEB.scad
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/advance_intersection.scad
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/animation.scad
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/demo_cut.scad
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/difference.scad
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/fractal.scad
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/intersecting.scad
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/iteration.scad
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/module_recursion.scad
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/offset.scad
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/search.scad
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/translation.scad
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/CSG-modules.scad
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/CSG.scad
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/LetterBlock.scad
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/children.scad
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/children_indexed.scad
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/difference_cube.scad
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/difference_sphere.scad
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/intersection.scad
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/linear_extrude.scad
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/logo.scad
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/logo_and_text.scad
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/projection.scad
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/rotate_extrude.scad
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/surface.scad
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/surface_image.scad
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/text_on_cube.scad
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/translate.scad
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/union.scad
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/cut_view.scad
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/fan_view.scad
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/text.scad
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Functions/functions.scad
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Functions/recursion.scad
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/chopped_blocks.scad
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/fence.scad
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/flat_body.scad
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/polyhedron.scad
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/rounded_box.scad
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/sphere.scad
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/tripod.scad
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 nicescad-0.0.6/scripts/doc
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 nicescad-0.0.6/scripts/install
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 nicescad-0.0.6/scripts/openscad_example_scraper.py
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 nicescad-0.0.6/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/basetest.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/test_blockscad_converter.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/test_file_selector.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/test_openscad.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 nicescad-0.0.6/tests/test_subprocess.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nicescad-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nicescad-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 nicescad-0.0.6/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 nicescad-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 nicescad-0.0.6/PKG-INFO
```

### Comparing `nicescad-0.0.5/.github/workflows/build.yml` & `nicescad-0.0.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/.github/workflows/upload-to-pypi.yml` & `nicescad-0.0.6/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/nicescad/file_selector.py` & `nicescad-0.0.6/nicescad/file_selector.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/nicescad/local_filepicker.py` & `nicescad-0.0.6/nicescad/local_filepicker.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/nicescad/nicescad_cmd.py` & `nicescad-0.0.6/nicescad/nicescad_cmd.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/nicescad/openscad.py` & `nicescad-0.0.6/nicescad/openscad.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/nicescad/process.py` & `nicescad-0.0.6/nicescad/process.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/nicescad/profiler.py` & `nicescad-0.0.6/nicescad/profiler.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/nicescad/version.py` & `nicescad-0.0.6/nicescad/version.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/nicescad/webserver.py` & `nicescad-0.0.6/nicescad/webserver.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Created on 2023-06-19
 
 @author: wf
 """
 from typing import Optional
 from nicescad.version import Version
 from nicescad.openscad import OpenScad
+from nicescad.axes_helper import AxesHelper
 from nicescad.file_selector import FileSelector
 from nicescad.local_filepicker import LocalFilePicker
 from nicegui import ui, app
 from pathlib import Path
 
 import os
 import sys
@@ -43,31 +44,32 @@
         self.stl_name="result.stl"
         self.stl_object=None
         self.is_local=False
         app.add_static_files('/stl', self.oscad.tmp_dir)
         self.log_view=None
         self.do_trace=True
         self.html_view=None
+        self.axes_view=None
  
         @ui.page('/')
         async def home():
             await self.home()
             
         @ui.page('/settings')
         def settings():
             self.settings()
             
             
     @classmethod
     def examples_path(cls)->str:
         # the root directory (default: examples)
-        path = os.path.join(os.path.dirname(__file__), '../scad_examples')
+        path = os.path.join(os.path.dirname(__file__), '../nicescad_examples')
+        path = os.path.abspath(path)
         return path
  
- 
     def handle_exception(self, e: BaseException, trace: Optional[bool] = False):
         """Handles an exception by creating an error message.
 
         Args:
             e (BaseException): The exception to handle.
             trace (bool, optional): Whether to include the traceback in the error message. Default is False.
         """
@@ -172,32 +174,33 @@
                 await self.read_and_optionally_render(input_file)
     pass
 
     async def reload_file(self):
         """
         reload the input file
         """
+        input_str=self.input
+        if os.path.exists(input_str):
+            input_str=os.path.abspath(input_str)
         allowed_urls=[
             "https://raw.githubusercontent.com/WolfgangFahl/nicescad/main/examples/",
-            "https://raw.githubusercontent.com/openscad/openscad/master/examples/"
+            "https://raw.githubusercontent.com/openscad/openscad/master/examples/",
+            self.examples_path(),
+            self.root_path
         ]
         if not self.is_local:
             allowed=False
             for allowed_url in allowed_urls:
-                if self.input.startswith(allowed_url):
+                if input_str.startswith(allowed_url):
                     allowed=True
         if not allowed:
-            ui.notify("only white listed URLs are allowed")
+            ui.notify("only white listed URLs and Path inputs are allowed")
         else:    
             await self.read_and_optionally_render(self.input)
             
-    def select_example(self,ts):
-        """
-        """
-        pass
     
     def link_button(self, name: str, target: str, icon_name: str):
         """
         Creates a button with a specified icon that opens a target URL upon being clicked.
     
         Args:
             name (str): The name to be displayed on the button.
@@ -207,31 +210,34 @@
         Returns:
             The button object.
         """
         with ui.button(name,icon=icon_name) as button:
             button.on("click",lambda: (ui.open(target)))
         return button
     
-    def tool_button(self,name:str,icon:str,handler:callable):
+    
+    def tool_button(self,tooltip:str,icon:str,handler:callable=None,toggle_icon:str=None)->ui.button:
         """
-        Creates an icon button that triggers a specified function upon being clicked.
+        Creates an  button with icon that triggers a specified function upon being clicked.
     
         Args:
-            name (str): The name of the button (not displayed, but could be used for identification).
+            tooltip (str): The tooltip to be displayed.
             icon (str): The name of the icon to be displayed on the button.
             handler (function): The function to be called when the button is clicked.
+            toggle_icon (str): The name of an alternative icon to be displayed when the button is clicked.
     
         Returns:
-            The icon button object.
+            ui.button: The icon button object.
             
         valid icons may be found at:    
             https://fonts.google.com/icons
         """
-        icon=ui.icon(icon, color='primary').classes('text-4xl').tooltip(name).on("click",handler=handler)  
-        return icon   
+        icon_button=ui.button("",icon=icon, color='primary').tooltip(tooltip).on("click",handler=handler)  
+        icon_button.toggle_icon=toggle_icon
+        return icon_button   
     
     def setup_pygments(self):
         """
         prepare pygments syntax highlighting by loading style
         """
         pygments_css_file=(Path(__file__).parent / 'web'/'static' / 'css'/ 'pygments.css')
         pygments_css= pygments_css_file.read_text()
@@ -265,27 +271,43 @@
     def code_changed(self,cargs):
         """
         react on changed code
         """
         self.code=cargs.value
         pass
     
-    def highlight_code(self,_cargs):
+    def toggle_icon(self,button:ui.button):
+        """
+        toggle the icon of the given button
+        
+        Args:
+            ui.button: the button that needs the icon to be toggled
+        """
+        if hasattr(button,"toggle_icon"):
+            # exchange icon with toggle icon
+            toggle_icon=button._props["icon"]
+            icon=button.toggle_icon
+            button._props["icon"]=icon
+            button.toggle_icon=toggle_icon
+        button.update()
+    
+    async def highlight_code(self,_cargs):
         """
         highlight the code and show the html 
         """
         try:
             if self.code_area.visible:
                 self.code_area.visible=False
                 code_html=self.oscad.highlight_code(self.code)
                 self.html_view.content=code_html
                 self.html_view.visible=True
             else:
                 self.html_view.visible=False
                 self.code_area.visible=True
+            self.toggle_icon(self.highlight_button)  
         except BaseException as ex:
             self.handle_exception(ex, self.do_trace)
         
     async def pick_color(self,e:ColorPickEventArguments):
         """
         Asynchronously picks a color based on provided event arguments.
     
@@ -300,41 +322,74 @@
             If 'stl_object' is None, the function will only change the color of 'color_picker_button'.
             Otherwise, it changes the color of both 'color_picker_button' and 'stl_object'.
         """
         self.color_picker_button.style(f'background-color:{e.color}!important')
         if self.stl_object:
             self.stl_object.material(f'{e.color}')
         pass
+    
+    async def toggle_axes(self):
+        """
+        toggle the axes of my scene
+        """
+        self.toggle_icon(self.axes_button)
+        if self.axes_view is None:
+            self.axes_view=AxesHelper(self.scene)
+        else:
+            self.axes_view.toggle_axes()
+        pass
+    
+    async def toggle_grid(self,_ea):
+        """
+        toogle the grid of my scene
+        """
+        try:
+            grid=self.scene._props["grid"]
+            grid_str="off" if grid else "on"
+            # try toggling grid
+            ui.notify(f"setting grid to {grid_str}")
+            grid=not grid
+            self.scene._props["grid"]=grid
+            self.scene.update()
+            # try toggling icon
+            self.toggle_icon(self.grid_button)
+        except BaseException as ex:
+            self.handleExeption(ex)
+        pass
         
     async def home(self):
         """Generates the home page with a 3D viewer and a code editor."""
         self.setup_pygments()
         self.setup_menu()
         with ui.column():
             with ui.splitter() as splitter:
                 with splitter.before:
-                    self.color_picker = ui.color_picker(on_pick=self.pick_color)
-                    self.color_picker_button=ui.button(on_click=self.color_picker.open, icon='colorize')      
+                    self.grid_button=self.tool_button("toggle grid",handler=self.toggle_grid,icon='grid_off',toggle_icon='grid_on')
+                    self.axes_button=self.tool_button("toggle axes",icon="polyline",toggle_icon="square",handler=self.toggle_axes)
+                    self.color_picker_button=ui.button(icon='colorize')     
+                    with self.color_picker_button: 
+                        self.color_picker = ui.color_picker(on_pick=self.pick_color)
                     self.color_picker_button.disable()
+                    
                     with ui.scene(width=1024, height=768).classes("w-full") as scene:
                         self.scene = scene
                         scene.spot_light(distance=100, intensity=0.2).move(-10, 0, 10)
                     with splitter.after:
                         with ui.element("div").classes("w-full"):
                             self.example_selector=FileSelector(path=self.root_path,extension=".scad",handler=self.read_and_optionally_render)
                             self.input_input=ui.input(
                                 value=self.input,
                                 on_change=self.input_changed).props("size=100")
-                            self.tool_button(name="highlight", icon="html", handler=self.highlight_code)    
+                            self.highlight_button=self.tool_button(tooltip="highlight", icon="html", toggle_icon="code",handler=self.highlight_code)    
                             if self.is_local:
-                                self.tool_button(name="save",icon="save",handler=self.save_file)
-                            self.tool_button(name="reload",icon="refresh",handler=self.reload_file)
+                                self.tool_button(tooltip="save",icon="save",handler=self.save_file)
+                            self.tool_button(tooltip="reload",icon="refresh",handler=self.reload_file)
                             if self.is_local:
-                                self.tool_button(name="open",icon="file_open",handler=self.open_file)
-                            self.tool_button(name="render",icon="play_circle",handler=self.render)
+                                self.tool_button(tooltip="open",icon="file_open",handler=self.open_file)
+                            self.tool_button(tooltip="render",icon="play_circle",handler=self.render)
                             self.stl_link=ui.link("stl result",f"/stl/{self.stl_name}",new_tab=True)
                             self.stl_link.visible=False
                             self.progress_view = ui.spinner('dots', size='lg', color='blue')
                             self.progress_view.visible = False
                             self.code_area = ui.textarea(value=self.code,on_change=self.code_changed).props('clearable').props("rows=25")
                             self.html_view = ui.html()
                             self.html_view.visible=False
@@ -356,10 +411,10 @@
         """Runs the UI of the web server.
 
         Args:
             args (list): The command line arguments.
         """
         self.args=args
         self.is_local=args.local
-        self.root_path=args.root_path 
+        self.root_path=os.path.abspath(args.root_path) 
         self.render_on_load=args.render_on_load
         ui.run(title=Version.name, host=args.host, port=args.port, show=args.client,reload=False)
```

### Comparing `nicescad-0.0.5/nicescad/web/static/css/pygments.css` & `nicescad-0.0.6/nicescad/web/static/css/pygments.css`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/intersection.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openjscad_logo.stl` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/openjscad_logo.stl`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/GEB.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/GEB.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/advance_intersection.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/advance_intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/animation.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/animation.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/demo_cut.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/demo_cut.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/difference.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/difference.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/fractal.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/fractal.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/intersecting.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/intersecting.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/iteration.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/iteration.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/module_recursion.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/module_recursion.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/offset.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/offset.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/search.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/search.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Advanced/translation.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Advanced/translation.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/CSG-modules.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/CSG-modules.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/CSG.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/CSG.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/LetterBlock.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/LetterBlock.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/children.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/children.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/children_indexed.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/children_indexed.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/difference_cube.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/difference_cube.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/difference_sphere.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/difference_sphere.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/intersection.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/intersection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/linear_extrude.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/linear_extrude.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/logo.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/logo.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/logo_and_text.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/logo_and_text.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/projection.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/projection.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/rotate_extrude.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/rotate_extrude.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/surface.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/surface.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/surface_image.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/surface_image.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/text_on_cube.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/text_on_cube.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/translate.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/translate.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Basics/union.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Basics/union.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/cut_view.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/cut_view.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/fan_view.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/fan_view.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Extrusion/text.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Extrusion/text.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Functions/functions.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Functions/functions.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Functions/recursion.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Functions/recursion.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/chopped_blocks.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/chopped_blocks.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/fence.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/fence.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/flat_body.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/flat_body.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/polyhedron.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/polyhedron.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/rounded_box.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/rounded_box.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/sphere.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/sphere.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scad_examples/openscad_examples/Shapes/tripod.scad` & `nicescad-0.0.6/nicescad_examples/scad/openscad_examples/Shapes/tripod.scad`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scripts/doc` & `nicescad-0.0.6/scripts/doc`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/scripts/openscad_example_scraper.py` & `nicescad-0.0.6/scripts/openscad_example_scraper.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/tests/basetest.py` & `nicescad-0.0.6/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/tests/test_openscad.py` & `nicescad-0.0.6/tests/test_openscad.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/tests/test_subprocess.py` & `nicescad-0.0.6/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/.gitignore` & `nicescad-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/LICENSE` & `nicescad-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/README.md` & `nicescad-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nicescad-0.0.5/pyproject.toml` & `nicescad-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 [project.optional-dependencies]
 test = [
   "green",
 ]
 
 [tool.hatch.build.targets.wheel]
-only-include = ["nicescad","scad_examples"]
+only-include = ["nicescad","nicescad_examples"]
 
 [tool.hatch.build.targets.wheel.sources]
 "nicescad" = "nicescad"
-"scad_examples" = "scad_examples"
+"nicescad_examples" = "nicescad_examples"
 
 [project.scripts]
 nicescad = "nicescad.nicescad_cmd:main"
```

### Comparing `nicescad-0.0.5/PKG-INFO` & `nicescad-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicescad
-Version: 0.0.5
+Version: 0.0.6
 Project-URL: Home, https://github.com/WolfgangFahl/nicescad
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/nicescad
 Project-URL: Source, https://github.com/WolfgangFahl/nicescad
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

