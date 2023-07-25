# Comparing `tmp/spatialdata_plot-0.0.2.tar.gz` & `tmp/spatialdata_plot-0.0.3.tar.gz`

## Comparing `spatialdata_plot-0.0.2.tar` & `spatialdata_plot-0.0.3.tar`

### file list

```diff
@@ -1,59 +1,95 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.bumpversion.cfg
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.codecov.yaml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.cruft.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.editorconfig
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.flake8
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.mypy.ini
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/_version.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/test_sandbox_data.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.github/codecov.yml
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.github/workflows/sync.yaml
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.github/workflows/test_and_deploy.yaml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/Makefile
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/changelog.md
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/conf.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/contributing.md
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/index.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/make.bat
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/plotting.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/preprocessing.rst
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/references.md
--rw-r--r--   0        0        0  1810880 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/spatialdata-plot.png
--rw-r--r--   0        0        0    17907 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/template_usage.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0   215590 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/notebooks/demo.ipynb
--rw-r--r--   0        0        0    15163 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/docs/notebooks/preprocessing.ipynb
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/src/spatialdata_plot/__init__.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/src/spatialdata_plot/_accessor.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/src/spatialdata_plot/pl/__init__.py
--rw-r--r--   0        0        0    26135 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/src/spatialdata_plot/pl/basic.py
--rw-r--r--   0        0        0    17025 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/src/spatialdata_plot/pl/render.py
--rw-r--r--   0        0        0    36230 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/src/spatialdata_plot/pl/utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/src/spatialdata_plot/pp/__init__.py
--rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/src/spatialdata_plot/pp/basic.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/src/spatialdata_plot/pp/basic.py.rej
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/src/spatialdata_plot/pp/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0    16875 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/tests/test_basic.py.rej
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/tests/test_image.py
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/tests/test_pp.py
--rw-r--r--   0        0        0    38467 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/tests/_images/Images_images.png
--rw-r--r--   0        0        0    14512 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/tests/_images/Labels_labels.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/tests/pl/__init__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/tests/pl/test_plot.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/tests/pl/test_render.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/tests/pp/test_basic.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/LICENSE
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/README.md
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.bumpversion.cfg
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.codecov.yaml
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.cruft.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.editorconfig
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.flake8
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.mypy.ini
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/_version.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.github/codecov.yml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/Makefile
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/changelog.md
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/conf.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/contributing.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/index.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/make.bat
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/plotting.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/preprocessing.rst
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/references.md
+-rw-r--r--   0        0        0  1810880 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/spatialdata-plot.png
+-rw-r--r--   0        0        0    17907 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/template_usage.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0    15163 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/docs/notebooks/preprocessing.ipynb
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/src/spatialdata_plot/__init__.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/src/spatialdata_plot/_accessor.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/src/spatialdata_plot/_logging.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/src/spatialdata_plot/pl/__init__.py
+-rw-r--r--   0        0        0    29116 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/src/spatialdata_plot/pl/basic.py
+-rw-r--r--   0        0        0    22889 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/src/spatialdata_plot/pl/render.py
+-rw-r--r--   0        0        0    43201 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/src/spatialdata_plot/pl/utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/src/spatialdata_plot/pp/__init__.py
+-rw-r--r--   0        0        0    12992 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/src/spatialdata_plot/pp/basic.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/src/spatialdata_plot/pp/basic.py.rej
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/src/spatialdata_plot/pp/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0    16961 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/test_basic.py.rej
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/test_image.py
+-rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/test_pp.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Extent_extent_calculation_respects_element_selection_circles.png
+-rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Extent_extent_calculation_respects_element_selection_circles_and_polygons.png
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Extent_extent_calculation_respects_element_selection_polygons.png
+-rw-r--r--   0        0        0    38467 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Extent_extent_of_img_full_canvas.png
+-rw-r--r--   0        0        0    32359 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Extent_extent_of_img_is_correct_after_spatial_query.png
+-rw-r--r--   0        0        0    39864 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Extent_extent_of_partial_canvas_on_full_canvas.png
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Extent_extent_of_points_partial_canvas.png
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Extent_extent_of_polygons_is_correct_after_spatial_query.png
+-rw-r--r--   0        0        0    33264 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Extent_extent_of_polygons_on_img_is_correct_after_spatial_query.png
+-rw-r--r--   0        0        0    32435 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Images_can_pass_cmap_to_each_channel.png
+-rw-r--r--   0        0        0    38467 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Images_can_pass_cmap_to_render_images.png
+-rw-r--r--   0        0        0    27365 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Images_can_pass_cmap_to_single_channel.png
+-rw-r--r--   0        0        0    36294 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Images_can_pass_color_to_each_channel.png
+-rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Images_can_pass_color_to_single_channel.png
+-rw-r--r--   0        0        0    26641 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Images_can_render_a_single_channel_from_image.png
+-rw-r--r--   0        0        0    38467 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Images_can_render_image.png
+-rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Images_can_render_two_channels_from_image.png
+-rw-r--r--   0        0        0    14410 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Labels_can_render_labels.png
+-rw-r--r--   0        0        0    40469 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_mapaxis.png
+-rw-r--r--   0        0        0    36658 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_overlay.png
+-rw-r--r--   0        0        0    20205 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_scale.png
+-rw-r--r--   0        0        0    45253 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/NotebooksTransformations_can_render_transformations_raccoon_split.png
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Points_can_render_points.png
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Shapes_can_render_circles.png
+-rw-r--r--   0        0        0     8802 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Shapes_can_render_circles_with_colored_outline.png
+-rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Shapes_can_render_circles_with_outline.png
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Shapes_can_render_polygons.png
+-rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Shapes_can_render_polygons_with_outline.png
+-rw-r--r--   0        0        0     7857 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Shapes_can_render_polygons_with_rgb_colored_outline.png
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Shapes_can_render_polygons_with_rgba_colored_outline.png
+-rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Shapes_can_render_polygons_with_str_colored_outline.png
+-rw-r--r--   0        0        0    22662 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/_images/Show_pad_extent_adds_padding.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/pl/__init__.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/pl/test_get_extent.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/pl/test_render.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/pl/test_render_images.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/pl/test_render_labels.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/pl/test_render_points.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/pl/test_render_shapes.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/pl/test_show.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/pl/test_upstream_plots.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/pl/test_utils.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/tests/pp/test_basic.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/README.md
+-rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 spatialdata_plot-0.0.3/PKG-INFO
```

### Comparing `spatialdata_plot-0.0.2/.cruft.json` & `spatialdata_plot-0.0.3/.cruft.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'checkout'": "'v0.2.9'", "'commit'": "'1929d97848fd6a62fe2916dec21d6c3de99cd0a2'"}*

```diff
@@ -1,10 +1,10 @@
 {
-    "checkout": "main",
-    "commit": "c21b82bf134f3a0f13db7482d4fb04ca1f562d59",
+    "checkout": "v0.2.9",
+    "commit": "1929d97848fd6a62fe2916dec21d6c3de99cd0a2",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 ".github/workflows/**.yaml",
                 "docs/_templates/autosummary/**.rst"
             ],
             "_template": "https://github.com/scverse/cookiecutter-scverse",
```

### Comparing `spatialdata_plot-0.0.2/.flake8` & `spatialdata_plot-0.0.3/.flake8`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/.mypy.ini` & `spatialdata_plot-0.0.3/.mypy.ini`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/.pre-commit-config.yaml` & `spatialdata_plot-0.0.3/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -9,25 +9,25 @@
     skip: []
 repos:
     - repo: https://github.com/psf/black
       rev: 23.3.0
       hooks:
           - id: black
     - repo: https://github.com/pre-commit/mirrors-prettier
-      rev: v3.0.0-alpha.6
+      rev: v3.0.0-alpha.9-for-vscode
       hooks:
           - id: prettier
     - repo: https://github.com/asottile/blacken-docs
       rev: 1.13.0
       hooks:
           - id: blacken-docs
     - repo: https://github.com/pre-commit/mirrors-mypy
-      rev: v1.2.0
+      rev: v1.3.0
       hooks:
           - id: mypy
             additional_dependencies: [numpy, types-requests]
             exclude: tests/|docs/
     - repo: https://github.com/charliermarsh/ruff-pre-commit
-      rev: v0.0.261
+      rev: v0.0.272
       hooks:
           - id: ruff
             args: [--fix, --exit-non-zero-on-fix]
```

### Comparing `spatialdata_plot-0.0.2/.github/workflows/build.yaml` & `spatialdata_plot-0.0.3/.github/workflows/build.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -2,28 +2,22 @@
 
 on:
     push:
         branches: [main]
     pull_request:
         branches: [main]
 
-concurrency:
-    group: ${{ github.workflow }}-${{ github.ref }}
-    cancel-in-progress: true
-
 jobs:
     package:
         runs-on: ubuntu-latest
         steps:
-            - uses: actions/checkout@v3
+            - uses: actions/checkout@v2
             - name: Set up Python 3.10
-              uses: actions/setup-python@v4
+              uses: actions/setup-python@v2
               with:
                   python-version: "3.10"
-                  cache: "pip"
-                  cache-dependency-path: "**/pyproject.toml"
             - name: Install build dependencies
               run: python -m pip install --upgrade pip wheel twine build
             - name: Build package
               run: python -m build
             - name: Check package
               run: twine check --strict dist/*.whl
```

### Comparing `spatialdata_plot-0.0.2/.github/workflows/test_and_deploy.yaml` & `spatialdata_plot-0.0.3/.github/workflows/test_and_deploy.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,14 @@
     push:
         branches: [main]
         tags:
             - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
     pull_request:
         branches: [main]
 
-concurrency:
-    group: ${{ github.workflow }}-${{ github.ref }}
-    cancel-in-progress: true
-
 jobs:
     test:
         runs-on: ${{ matrix.os }}
         defaults:
             run:
                 shell: bash -e {0} # -e to fail on error
 
@@ -26,26 +22,26 @@
                 os: [ubuntu-latest]
 
         env:
             OS: ${{ matrix.os }}
             PYTHON: ${{ matrix.python }}
 
         steps:
-            - uses: actions/checkout@v2
+            - uses: actions/checkout@v3
             - name: Set up Python ${{ matrix.python }}
-              uses: actions/setup-python@v2
+              uses: actions/setup-python@v3
               with:
                   python-version: ${{ matrix.python }}
 
             - name: Get pip cache dir
               id: pip-cache-dir
               run: |
                   echo "::set-output name=dir::$(pip cache dir)"
             - name: Restore pip cache
-              uses: actions/cache@v2
+              uses: actions/cache@v3
               with:
                   path: ${{ steps.pip-cache-dir.outputs.dir }}
                   key: pip-${{ runner.os }}-${{ env.pythonLocation }}-${{ hashFiles('**/pyproject.toml') }}
                   restore-keys: |
                       pip-${{ runner.os }}-${{ env.pythonLocation }}-
             - name: Install test dependencies
               run: |
@@ -70,18 +66,19 @@
             - name: Archive figures generated during testing
               if: always()
               uses: actions/upload-artifact@v3
               with:
                   name: plotting-results
                   path: /home/runner/work/spatialdata-plot/spatialdata-plot/tests/figures/*
             - name: Upload coverage to Codecov
-              uses: codecov/codecov-action@v3.1.1
+              uses: codecov/codecov-action@v3
               with:
-                  name: coverage
-                  verbose: true
+                  token: ${{ secrets.CODECOV_TOKEN }}
+                  fail_ci_if_error: true # optional (default = false)
+                  verbose: true # optional (default = false)
     deploy:
         # this will run when you have tagged a commit, starting with "v*"
         # and requires that you have put your twine API key in your
         # github secrets (see readme for details)
         needs: [test]
         runs-on: ubuntu-latest
         if: contains(github.ref, 'tags')
```

### Comparing `spatialdata_plot-0.0.2/docs/Makefile` & `spatialdata_plot-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/docs/conf.py` & `spatialdata_plot-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/docs/contributing.md` & `spatialdata_plot-0.0.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/docs/make.bat` & `spatialdata_plot-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/docs/references.bib` & `spatialdata_plot-0.0.3/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/docs/spatialdata-plot.png` & `spatialdata_plot-0.0.3/docs/spatialdata-plot.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/docs/template_usage.md` & `spatialdata_plot-0.0.3/docs/template_usage.md`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/docs/_templates/autosummary/class.rst` & `spatialdata_plot-0.0.3/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/docs/extensions/typed_returns.py` & `spatialdata_plot-0.0.3/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/docs/notebooks/preprocessing.ipynb` & `spatialdata_plot-0.0.3/docs/notebooks/preprocessing.ipynb`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/src/spatialdata_plot/_accessor.py` & `spatialdata_plot-0.0.3/src/spatialdata_plot/_accessor.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/src/spatialdata_plot/pl/basic.py` & `spatialdata_plot-0.0.3/src/spatialdata_plot/pl/basic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from __future__ import annotations
 
 import sys
 from collections import OrderedDict
 from collections.abc import Sequence
 from pathlib import Path
-from typing import Any, Optional, Union
+from typing import Any
 
 import matplotlib.pyplot as plt
+import numpy as np
 import scanpy as sc
 import spatialdata as sd
 from anndata import AnnData
 from dask.dataframe.core import DataFrame as DaskDataFrame
 from geopandas import GeoDataFrame
 from matplotlib.axes import Axes
-from matplotlib.colors import Colormap, Normalize
+from matplotlib.colors import Colormap, ListedColormap, Normalize
 from matplotlib.figure import Figure
 from multiscale_spatial_image.multiscale_spatial_image import MultiscaleSpatialImage
 from pandas.api.types import is_categorical_dtype
 from spatial_image import SpatialImage
-from spatialdata import transform
 from spatialdata._logging import logger as logg
-from spatialdata.transformations import get_transformation
 
 from spatialdata_plot._accessor import register_spatial_data_accessor
 from spatialdata_plot.pl.render import (
     ImageRenderParams,
     LabelsRenderParams,
     PointsRenderParams,
     ShapesRenderParams,
     _render_images,
     _render_labels,
     _render_points,
     _render_shapes,
 )
 from spatialdata_plot.pl.utils import (
+    CmapParams,
     LegendParams,
-    Palette_t,
     _FontSize,
     _FontWeight,
     _get_cs_contents,
     _get_extent,
     _maybe_set_colors,
+    _mpl_ax_contains_elements,
     _multiscale_to_image,
     _prepare_cmap_norm,
     _prepare_params_plot,
+    _robust_transform,
     _set_outline,
-    _translate_image,
     save_fig,
 )
 from spatialdata_plot.pp.utils import _verify_plotting_tree
 
 
 @register_spatial_data_accessor("pl")
 class PlotAccessor:
@@ -80,19 +80,19 @@
         self._sdata = sdata
 
     def __init__(self, sdata: sd.SpatialData) -> None:
         self._sdata = sdata
 
     def _copy(
         self,
-        images: Union[None, dict[str, Union[SpatialImage, MultiscaleSpatialImage]]] = None,
-        labels: Union[None, dict[str, Union[SpatialImage, MultiscaleSpatialImage]]] = None,
-        points: Union[None, dict[str, DaskDataFrame]] = None,
-        shapes: Union[None, dict[str, GeoDataFrame]] = None,
-        table: Union[None, AnnData] = None,
+        images: None | dict[str, SpatialImage | MultiscaleSpatialImage] = None,
+        labels: None | dict[str, SpatialImage | MultiscaleSpatialImage] = None,
+        points: None | dict[str, DaskDataFrame] = None,
+        shapes: None | dict[str, GeoDataFrame] = None,
+        table: None | AnnData = None,
     ) -> sd.SpatialData:
         """Copy the current `SpatialData` object, optionally modifying some of its attributes.
 
         Parameters
         ----------
         images :
             A dictionary containing image data to replace the images in the
@@ -137,37 +137,38 @@
         )
         sdata.plotting_tree = self._sdata.plotting_tree if hasattr(self._sdata, "plotting_tree") else OrderedDict()
 
         return sdata
 
     def render_shapes(
         self,
-        element: str | None = None,
+        elements: str | list[str] | None = None,
         color: str | None = None,
         groups: str | Sequence[str] | None = None,
         size: float = 1.0,
         outline: bool = False,
         outline_width: tuple[float, float] = (0.3, 0.05),
-        outline_color: tuple[str, str] = ("black", "white"),
+        outline_color: str | list[float] = "#000000ff",
         alt_var: str | None = None,
         layer: str | None = None,
-        palette: Palette_t = None,
+        palette: ListedColormap | str | None = None,
         cmap: Colormap | str | None = None,
-        norm: Optional[Normalize] = None,
+        norm: None | Normalize = None,
         na_color: str | tuple[float, ...] | None = "lightgrey",
-        alpha: float = 1.0,
+        outline_alpha: float = 1.0,
+        fill_alpha: float = 1.0,
         **kwargs: Any,
     ) -> sd.SpatialData:
         """
         Render shapes elements in SpatialData.
 
         Parameters
         ----------
-        element
-            The name of the shapes element to render. If `None`, the first
+        elements
+            The name of the shapes element(s) to render. If `None`, all
             shapes element in the `SpatialData` object will be used.
         color
             Key for annotations in :attr:`anndata.AnnData.obs` or variables/genes.
         groups
             For discrete annotation in ``color``, select which values
             to plot (other values are set to NAs).
         size
@@ -206,47 +207,49 @@
             cmap=cmap,
             norm=norm,
             na_color=na_color,  # type: ignore[arg-type]
             **kwargs,
         )
         outline_params = _set_outline(size, outline, outline_width, outline_color)
         sdata.plotting_tree[f"{n_steps+1}_render_shapes"] = ShapesRenderParams(
-            element=element,
+            elements=elements,
             color=color,
             groups=groups,
             outline_params=outline_params,
             alt_var=alt_var,
             layer=layer,
             cmap_params=cmap_params,
             palette=palette,
-            alpha=alpha,
+            outline_alpha=outline_alpha,
+            fill_alpha=fill_alpha,
+            transfunc=kwargs.get("transfunc", None),
         )
 
         return sdata
 
     def render_points(
         self,
-        element: str | None = None,
+        elements: str | list[str] | None = None,
         color: str | None = None,
         groups: str | Sequence[str] | None = None,
         size: float = 1.0,
-        palette: Palette_t = None,
+        palette: ListedColormap | str | None = None,
         cmap: Colormap | str | None = None,
-        norm: Optional[Normalize] = None,
+        norm: None | Normalize = None,
         na_color: str | tuple[float, ...] | None = (0.0, 0.0, 0.0, 0.0),
         alpha: float = 1.0,
         **kwargs: Any,
     ) -> sd.SpatialData:
         """
         Render points elements in SpatialData.
 
         Parameters
         ----------
-        element
-            The name of the points element to render. If `None`, the first
+        elements
+            The name of the points element(s) to render. If `None`, all
             shapes element in the `SpatialData` object will be used.
         color
             Key for annotations in :attr:`anndata.AnnData.obs` or variables/genes.
         groups
             For discrete annotation in ``color``, select which values
             to plot (other values are set to NAs).
         size
@@ -274,105 +277,128 @@
         cmap_params = _prepare_cmap_norm(
             cmap=cmap,
             norm=norm,
             na_color=na_color,  # type: ignore[arg-type]
             **kwargs,
         )
         sdata.plotting_tree[f"{n_steps+1}_render_points"] = PointsRenderParams(
-            element=element,
+            elements=elements,
             color=color,
             groups=groups,
             cmap_params=cmap_params,
             palette=palette,
             alpha=alpha,
+            transfunc=kwargs.get("transfunc", None),
+            size=size,
         )
 
         return sdata
 
     def render_images(
         self,
-        element: str | None = None,
+        elements: str | list[str] | None = None,
         channel: list[str] | list[int] | int | str | None = None,
-        cmap: Colormap | str | None = None,
-        norm: Optional[Normalize] = None,
+        cmap: list[Colormap] | list[str] | Colormap | str | None = None,
+        norm: None | Normalize = None,
         na_color: str | tuple[float, ...] | None = (0.0, 0.0, 0.0, 0.0),
-        palette: Palette_t = None,
+        palette: ListedColormap | str | None = None,
         alpha: float = 1.0,
+        quantiles_for_norm: tuple[float | None, float | None] = (3.0, 99.8),  # defaults from CSBDeep
         **kwargs: Any,
     ) -> sd.SpatialData:
         """
         Render image elements in SpatialData.
 
         Parameters
         ----------
-        element
-            The name of the image element to render. If `None`, the first
-            shapes element in the `SpatialData` object will be used.
+        elements
+            The name of the image element(s) to render. If `None`, all
+            shapes elements in the `SpatialData` object will be used.
         channel
             To select which channel to plot (all by default).
         cmap
             Colormap for continuous annotations, see :class:`matplotlib.colors.Colormap`.
         norm
             Colormap normalization for continuous annotations, see :class:`matplotlib.colors.Normalize`.
         na_color
             Color to be used for NAs values, if present.
         alpha
             Alpha value for the shapes.
+        quantiles_for_norm
+            Tuple of (pmin, pmax) which will be used for quantile normalization.
         kwargs
             Additional arguments to be passed to cmap and norm.
 
         Returns
         -------
         None
         """
         sdata = self._copy()
         sdata = _verify_plotting_tree(sdata)
         n_steps = len(sdata.plotting_tree.keys())
 
-        cmap_params = _prepare_cmap_norm(
-            cmap=cmap,
-            norm=norm,
-            na_color=na_color,  # type: ignore[arg-type]
-            **kwargs,
-        )
+        if channel is None and cmap is None:
+            cmap = "brg"
+
+        cmap_params: list[CmapParams] | CmapParams
+        if isinstance(cmap, list):
+            cmap_params = [
+                _prepare_cmap_norm(
+                    cmap=c,
+                    norm=norm,
+                    na_color=na_color,  # type: ignore[arg-type]
+                    **kwargs,
+                )
+                for c in cmap
+            ]
+
+        else:
+            cmap_params = _prepare_cmap_norm(
+                cmap=cmap,
+                norm=norm,
+                na_color=na_color,  # type: ignore[arg-type]
+                **kwargs,
+            )
+
         sdata.plotting_tree[f"{n_steps+1}_render_images"] = ImageRenderParams(
-            element=element,
+            elements=elements,
             channel=channel,
             cmap_params=cmap_params,
             palette=palette,
             alpha=alpha,
+            quantiles_for_norm=quantiles_for_norm,
         )
 
         return sdata
 
     def render_labels(
         self,
-        element: str | None = None,
+        elements: str | list[str] | None = None,
         color: str | None = None,
         groups: str | Sequence[str] | None = None,
         contour_px: int = 3,
         outline: bool = False,
         alt_var: str | None = None,
         layer: str | None = None,
-        palette: Palette_t = None,
+        palette: ListedColormap | str | None = None,
         cmap: Colormap | str | None = None,
-        norm: Optional[Normalize] = None,
+        norm: None | Normalize = None,
         na_color: str | tuple[float, ...] | None = (0.0, 0.0, 0.0, 0.0),
         outline_alpha: float = 1.0,
         fill_alpha: float = 0.3,
         **kwargs: Any,
     ) -> sd.SpatialData:
         """
         Render labels elements in SpatialData.
 
         Parameters
         ----------
-        element
-            The name of the labels element to render. If `None`, the first
-            labels element in the `SpatialData` object will be used.
+        elements
+            The name of the labels element(s) to render. If `None`, all
+            labels elements in the `SpatialData` object will be used.
         color
             Key for annotations in :attr:`anndata.AnnData.obs` or variables/genes.
         groups
             For discrete annotation in ``color``, select which values
             to plot (other values are set to NAs).
         contour_px
             Draw contour of specified width for each segment. If `None`, fills
@@ -413,25 +439,26 @@
         cmap_params = _prepare_cmap_norm(
             cmap=cmap,
             norm=norm,
             na_color=na_color,  # type: ignore[arg-type]
             **kwargs,
         )
         sdata.plotting_tree[f"{n_steps+1}_render_labels"] = LabelsRenderParams(
-            element=element,
+            elements=elements,
             color=color,
             groups=groups,
             contour_px=contour_px,
             outline=outline,
             alt_var=alt_var,
             layer=layer,
             cmap_params=cmap_params,
             palette=palette,
             outline_alpha=outline_alpha,
             fill_alpha=fill_alpha,
+            transfunc=kwargs.get("transfunc", None),
         )
 
         return sdata
 
     def show(
         self,
         coordinate_systems: str | Sequence[str] | None = None,
@@ -444,17 +471,20 @@
         wspace: float | None = None,
         hspace: float = 0.25,
         ncols: int = 4,
         frameon: bool | None = None,
         figsize: tuple[float, float] | None = None,
         dpi: int | None = None,
         fig: Figure | None = None,
+        title: None | str | Sequence[str] = None,
+        share_extent: bool = True,
+        pad_extent: int = 0,
         ax: Axes | Sequence[Axes] | None = None,
         return_ax: bool = False,
-        save: Optional[Union[str, Path]] = None,
+        save: None | str | Path = None,
     ) -> sd.SpatialData:
         """
         Plot the images in the SpatialData object.
 
         Parameters
         ----------
         ax :
@@ -503,82 +533,97 @@
             if "render" in cmd:
                 # verify that rendering commands have been called before
                 render_cmds[cmd] = params
 
         if len(render_cmds.keys()) == 0:
             raise TypeError("Please specify what to plot using the 'render_*' functions before calling 'imshow().")
 
-        # Simplicstic solution: If the images are multiscale, just use the first
-        sdata = _multiscale_to_image(sdata)
-
-        img_transformations: dict[str, dict[str, sd.transformations.transformations.BaseTransformation]] = {}
-        # transform all elements
-        for cmd, _ in render_cmds.items():
-            if cmd == "render_images" or cmd == "render_channels":
-                for key in sdata.images:
-                    img_transformations[key] = {}
-                    all_transformations = get_transformation(sdata.images[key], get_all=True)
+        if title is not None:
+            if isinstance(title, str):
+                title = [title]
 
-                    for cs, transformation in all_transformations.items():
-                        img_transformations[key][cs] = transformation
+            if not all(isinstance(t, str) for t in title):
+                raise TypeError("All titles must be strings.")
 
-                        if isinstance(transformation, sd.transformations.transformations.Translation):
-                            sdata.images[key] = _translate_image(image=sdata.images[key], translation=transformation)
+        # Simplicstic solution: If the images are multiscale, just use the first
+        sdata = _multiscale_to_image(sdata)
 
-                        elif isinstance(transformation, sd.transformations.transformations.Sequence):
-                            # we have more than one transformation, let's find the translation(s)
-                            for t in list(transformation.transformations):
-                                if isinstance(t, sd.transformations.transformations.Translation):
-                                    sdata.images[key] = _translate_image(image=sdata.images[key], translation=t)
+        # get original axis extent for later comparison
+        x_min_orig, x_max_orig = (np.inf, -np.inf)
+        y_min_orig, y_max_orig = (np.inf, -np.inf)
+
+        if isinstance(ax, Axes) and _mpl_ax_contains_elements(ax):
+            x_min_orig, x_max_orig = ax.get_xlim()
+            y_max_orig, y_min_orig = ax.get_ylim()  # (0, 0) is top-left
 
-                                else:
-                                    sdata.images[key] = transform(sdata.images[key], t)
+        # handle coordinate system
+        coordinate_systems = sdata.coordinate_systems if coordinate_systems is None else coordinate_systems
+        if isinstance(coordinate_systems, str):
+            coordinate_systems = [coordinate_systems]
 
-            elif cmd == "render_shapes":
-                for key in sdata.shapes:
-                    shape_transformation = get_transformation(sdata.shapes[key], get_all=True)
-                    shape_transformation = list(shape_transformation.values())[0]
-                    sdata.shapes[key] = transform(sdata.shapes[key], shape_transformation)
+        for cs in coordinate_systems:
+            if cs not in sdata.coordinate_systems:
+                raise ValueError(f"Unknown coordinate system '{cs}', valid choices are: {sdata.coordinate_systems}")
 
-            elif cmd == "render_labels":
-                for key in sdata.labels:
-                    label_transformation = get_transformation(sdata.labels[key], get_all=True)
-                    label_transformation = list(label_transformation.values())[0]
-                    sdata.labels[key] = transform(sdata.labels[key], label_transformation)
+        # Check if user specified only certain elements to be plotted
+        cs_contents = _get_cs_contents(sdata)
+        elements_to_be_rendered = []
+        for cmd, params in render_cmds.items():
+            if cmd == "render_images" and cs_contents.query(f"cs == '{cs}'")["has_images"][0]:  # noqa: SIM114
+                if params.elements is not None:
+                    elements_to_be_rendered += (
+                        [params.elements] if isinstance(params.elements, str) else params.elements
+                    )
+            elif cmd == "render_shapes" and cs_contents.query(f"cs == '{cs}'")["has_shapes"][0]:  # noqa: SIM114
+                if params.elements is not None:
+                    elements_to_be_rendered += (
+                        [params.elements] if isinstance(params.elements, str) else params.elements
+                    )
+            elif cmd == "render_points" and cs_contents.query(f"cs == '{cs}'")["has_points"][0]:  # noqa: SIM114
+                if params.elements is not None:
+                    elements_to_be_rendered += (
+                        [params.elements] if isinstance(params.elements, str) else params.elements
+                    )
+            elif cmd == "render_labels" and cs_contents.query(f"cs == '{cs}'")["has_labels"][0]:  # noqa: SIM102
+                if params.elements is not None:
+                    elements_to_be_rendered += (
+                        [params.elements] if isinstance(params.elements, str) else params.elements
+                    )
 
         extent = _get_extent(
             sdata=sdata,
-            images="render_images" in render_cmds,
-            labels="render_labels" in render_cmds,
-            points="render_points" in render_cmds,
-            shapes="render_shapes" in render_cmds,
-            img_transformations=img_transformations if len(img_transformations) > 0 else None,
+            has_images="render_images" in render_cmds,
+            has_labels="render_labels" in render_cmds,
+            has_points="render_points" in render_cmds,
+            has_shapes="render_shapes" in render_cmds,
+            elements=elements_to_be_rendered,
+            coordinate_systems=coordinate_systems,
         )
 
-        # handle coordinate system
-        coordinate_systems = sdata.coordinate_systems if coordinate_systems is None else coordinate_systems
-        if isinstance(coordinate_systems, str):
-            coordinate_systems = [coordinate_systems]
-
         # Use extent to filter out coordinate system without the relevant elements
         valid_cs = []
         for cs in coordinate_systems:
             if cs in extent:
                 valid_cs.append(cs)
             else:
                 logg.info(f"Dropping coordinate system '{cs}' since it doesn't have relevant elements.")
         coordinate_systems = valid_cs
 
+        # print(coordinate_systems)
+        # cs_mapping = _get_coordinate_system_mapping(sdata)
+        # print(cs_mapping)
+
         # check that coordinate system and elements to be rendered match
-        for cmd, params in render_cmds.items():
-            if params.element is not None and len([params.element]) != len(coordinate_systems):
-                raise ValueError(
-                    f"Number of coordinate systems ({len(coordinate_systems)}) does not match number of elements "
-                    f"({len(params.element)}) in command {cmd}."
-                )
+        # for cmd, params in render_cmds.items():
+        #     if params.elements is not None and len([params.elements]) != len(coordinate_systems):
+        #         print(params.elements)
+        #         raise ValueError(
+        #             f"Number of coordinate systems ({len(coordinate_systems)}) does not match number of elements "
+        #             f"({len(params.elements)}) in command {cmd}."
+        #         )
 
         # set up canvas
         fig_params, scalebar_params = _prepare_params_plot(
             num_panels=len(coordinate_systems),
             figsize=figsize,
             dpi=dpi,
             fig=fig,
@@ -594,27 +639,48 @@
             legend_loc=legend_loc,
             legend_fontoutline=legend_fontoutline,
             na_in_legend=na_in_legend,
             colorbar=colorbar,
         )
 
         # go through tree
-        cs_contents = _get_cs_contents(sdata)
         for i, cs in enumerate(coordinate_systems):
+            sdata = self._copy()
+            # properly transform all elements to the current coordinate system
+            members = cs_contents.query(f"cs == '{cs}'")
+
+            if members["has_images"].values[0]:
+                for key in sdata.images:
+                    sdata.images[key] = _robust_transform(sdata.images[key], cs)
+
+            if members["has_labels"].values[0]:
+                for key in sdata.labels:
+                    sdata.labels[key] = _robust_transform(sdata.labels[key], cs)
+
+            if members["has_points"].values[0]:
+                for key in sdata.points:
+                    sdata.points[key] = _robust_transform(sdata.points[key], cs)
+
+            if members["has_shapes"].values[0]:
+                for key in sdata.shapes:
+                    sdata.shapes[key] = _robust_transform(sdata.shapes[key], cs)
+
             ax = fig_params.ax if fig_params.axs is None else fig_params.axs[i]
+
             for cmd, params in render_cmds.items():
                 if cmd == "render_images" and cs_contents.query(f"cs == '{cs}'")["has_images"][0]:
                     _render_images(
                         sdata=sdata,
                         render_params=params,
                         coordinate_system=cs,
                         ax=ax,
                         fig_params=fig_params,
                         scalebar_params=scalebar_params,
                         legend_params=legend_params,
+                        # extent=extent[cs],
                     )
                 elif cmd == "render_shapes" and cs_contents.query(f"cs == '{cs}'")["has_shapes"][0]:
                     if sdata.table is not None and isinstance(params.color, str):
                         colors = sc.get.obs_df(sdata.table, params.color)
                         if is_categorical_dtype(colors):
                             _maybe_set_colors(
                                 source=sdata.table,
@@ -640,19 +706,15 @@
                         ax=ax,
                         fig_params=fig_params,
                         scalebar_params=scalebar_params,
                         legend_params=legend_params,
                     )
 
                 elif cmd == "render_labels" and cs_contents.query(f"cs == '{cs}'")["has_labels"][0]:
-                    if (
-                        sdata.table is not None
-                        # and isinstance(params["instance_key"], str)
-                        and isinstance(params.color, str)
-                    ):
+                    if sdata.table is not None and isinstance(params.color, str):
                         colors = sc.get.obs_df(sdata.table, params.color)
                         if is_categorical_dtype(colors):
                             _maybe_set_colors(
                                 source=sdata.table,
                                 target=sdata.table,
                                 key=params.color,
                                 palette=params.palette,
@@ -663,25 +725,41 @@
                         coordinate_system=cs,
                         ax=ax,
                         fig_params=fig_params,
                         scalebar_params=scalebar_params,
                         legend_params=legend_params,
                     )
 
-                ax.set_title(cs)
-                if any(
-                    [
-                        cs_contents.query(f"cs == '{cs}'")["has_images"][0],
-                        cs_contents.query(f"cs == '{cs}'")["has_labels"][0],
-                        cs_contents.query(f"cs == '{cs}'")["has_points"][0],
-                        cs_contents.query(f"cs == '{cs}'")["has_shapes"][0],
-                    ]
-                ):
-                    ax.set_xlim(extent[cs][0], extent[cs][1])
-                    ax.set_ylim(extent[cs][3], extent[cs][2])  # (0, 0) is top-left
+                if title is not None:
+                    if len(title) == 1:
+                        t = title[0]
+                    else:
+                        try:
+                            t = title[i]
+                        except IndexError as e:
+                            raise IndexError("The number of titles must match the number of coordinate systems.") from e
+                else:
+                    t = cs
+                ax.set_title(t)
+
+            if any(
+                [
+                    cs_contents.query(f"cs == '{cs}'")["has_images"][0],
+                    cs_contents.query(f"cs == '{cs}'")["has_labels"][0],
+                    cs_contents.query(f"cs == '{cs}'")["has_points"][0],
+                    cs_contents.query(f"cs == '{cs}'")["has_shapes"][0],
+                ]
+            ):
+                # If the axis already has limits, only expand them but not overwrite
+                x_min = min(x_min_orig, extent[cs][0]) - pad_extent
+                x_max = max(x_max_orig, extent[cs][1]) + pad_extent
+                y_min = min(y_min_orig, extent[cs][2]) - pad_extent
+                y_max = max(y_max_orig, extent[cs][3]) + pad_extent
+                ax.set_xlim(x_min, x_max)
+                ax.set_ylim(y_max, y_min)  # (0, 0) is top-left
 
         if fig_params.fig is not None and save is not None:
             save_fig(fig_params.fig, path=save)
 
         # Manually show plot if we're not in interactive mode
         # https://stackoverflow.com/a/64523765
         if not hasattr(sys, "ps1"):
```

### Comparing `spatialdata_plot-0.0.2/src/spatialdata_plot/pl/utils.py` & `spatialdata_plot-0.0.3/src/spatialdata_plot/pl/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,54 +3,53 @@
 import os
 from collections.abc import Iterable, Mapping, Sequence
 from copy import copy
 from dataclasses import dataclass
 from functools import partial
 from pathlib import Path
 from types import MappingProxyType
-from typing import Any, Literal, Optional, Union
+from typing import Any, Literal
 
+import matplotlib
 import matplotlib.pyplot as plt
 import multiscale_spatial_image as msi
 import numpy as np
 import pandas as pd
 import spatial_image
 import spatialdata as sd
 import xarray as xr
 from anndata import AnnData
 from cycler import Cycler, cycler
 from matplotlib import colors, patheffects, rcParams
 from matplotlib.axes import Axes
-from matplotlib.cm import get_cmap
 from matplotlib.collections import PatchCollection
 from matplotlib.colors import Colormap, LinearSegmentedColormap, ListedColormap, Normalize, TwoSlopeNorm, to_rgba
 from matplotlib.figure import Figure
 from matplotlib.gridspec import GridSpec
 from matplotlib_scalebar.scalebar import ScaleBar
 from numpy.random import default_rng
 from pandas.api.types import CategoricalDtype, is_categorical_dtype
 from scanpy import settings
 from scanpy.plotting._tools.scatterplots import _add_categorical_legend
 from scanpy.plotting.palettes import default_20, default_28, default_102
-from shapely.geometry import Point
+from shapely.geometry import LineString, Point, Polygon
 from skimage.color import label2rgb
 from skimage.morphology import erosion, square
 from skimage.segmentation import find_boundaries
 from skimage.util import map_array
+from spatialdata import transform
 from spatialdata._logging import logger as logging
 from spatialdata._types import ArrayLike
 from spatialdata.models import (
     Image2DModel,
 )
+from spatialdata.transformations import get_transformation
 
 from spatialdata_plot.pp.utils import _get_coordinate_system_mapping
 
-Palette_t = Optional[Union[str, ListedColormap]]
-_Normalize = Union[Normalize, Sequence[Normalize]]
-_SeqStr = Union[str, Sequence[str]]
 _FontWeight = Literal["light", "normal", "medium", "semibold", "bold", "heavy", "black"]
 _FontSize = Literal["xx-small", "x-small", "small", "medium", "large", "x-large", "xx-large"]
 
 to_hex = partial(colors.to_hex, keep_alpha=True)
 
 
 @dataclass
@@ -84,15 +83,15 @@
     ax: Axes | Sequence[Axes] | None = None,
     wspace: float | None = None,
     hspace: float = 0.25,
     ncols: int = 4,
     frameon: bool | None = None,
     # this is passed at `render_*`
     cmap: Colormap | str | None = None,
-    norm: _Normalize | None = None,
+    norm: Normalize | Sequence[Normalize] | None = None,
     na_color: str | tuple[float, ...] | None = (0.0, 0.0, 0.0, 0.0),
     vmin: float | None = None,
     vmax: float | None = None,
     vcenter: float | None = None,
     # this args will be inferred from coordinate system
     scalebar_dx: float | Sequence[float] | None = None,
     scalebar_units: str | Sequence[str] | None = None,
@@ -103,15 +102,15 @@
     wspace = 0.75 / rcParams["figure.figsize"][0] + 0.02 if wspace is None else wspace
     figsize = rcParams["figure.figsize"] if figsize is None else figsize
     dpi = rcParams["figure.dpi"] if dpi is None else dpi
     if num_panels > 1 and ax is None:
         fig, grid = _panel_grid(
             num_panels=num_panels, hspace=hspace, wspace=wspace, ncols=ncols, dpi=dpi, figsize=figsize
         )
-        axs: Union[Sequence[Axes], None] = [plt.subplot(grid[c]) for c in range(num_panels)]
+        axs: None | Sequence[Axes] = [plt.subplot(grid[c]) for c in range(num_panels)]
     elif num_panels > 1 and ax is not None:
         if len(ax) != num_panels:
             raise ValueError(f"Len of `ax`: {len(ax)} is not equal to number of panels: {num_panels}.")
         if fig is None:
             raise ValueError(
                 f"Invalid value of `fig`: {fig}. If a list of `Axes` is passed, a `Figure` must also be specified."
             )
@@ -142,18 +141,18 @@
     """Check which coordinate systems contain which elements and return that info."""
     cs_mapping = _get_coordinate_system_mapping(sdata)
     content_flags = ["has_images", "has_labels", "has_points", "has_shapes"]
     cs_contents = pd.DataFrame(columns=["cs"] + content_flags)
 
     for cs_name, element_ids in cs_mapping.items():
         # determine if coordinate system has the respective elements
-        cs_has_images = bool(any([(e in sdata.images) for e in element_ids]))
-        cs_has_labels = bool(any([(e in sdata.labels) for e in element_ids]))
-        cs_has_points = bool(any([(e in sdata.points) for e in element_ids]))
-        cs_has_shapes = bool(any([(e in sdata.shapes) for e in element_ids]))
+        cs_has_images = bool(any((e in sdata.images) for e in element_ids))
+        cs_has_labels = bool(any((e in sdata.labels) for e in element_ids))
+        cs_has_points = bool(any((e in sdata.points) for e in element_ids))
+        cs_has_shapes = bool(any((e in sdata.shapes) for e in element_ids))
 
         cs_contents = pd.concat(
             [
                 cs_contents,
                 pd.DataFrame(
                     {
                         "cs": cs_name,
@@ -172,171 +171,237 @@
         cs_contents["has_shapes"] = cs_contents["has_shapes"].astype("bool")
 
     return cs_contents
 
 
 def _get_extent(
     sdata: sd.SpatialData,
-    coordinate_systems: Union[str, Sequence[str]] = "all",
-    images: bool = True,
-    labels: bool = True,
-    points: bool = True,
-    shapes: bool = True,
-    img_transformations: Optional[dict[str, dict[str, sd.transformations.transformations.BaseTransformation]]] = None,
+    coordinate_systems: Sequence[str] | str | None = None,
+    has_images: bool = True,
+    has_labels: bool = True,
+    has_points: bool = True,
+    has_shapes: bool = True,
+    elements: Iterable[Any] | None = None,
+    share_extent: bool = False,
 ) -> dict[str, tuple[int, int, int, int]]:
-    """Return the extent of the elements contained in the SpatialData object.
+    """Return the extent of all elements in their respective coordinate systems.
 
     Parameters
     ----------
     sdata
         The sd.SpatialData object to retrieve the extent from
-    images
+    has_images
         Flag indicating whether to consider images when calculating the extent
-    labels
+    has_labels
         Flag indicating whether to consider labels when calculating the extent
-    points
+    has_points
         Flag indicating whether to consider points when calculating the extent
-    shapes
-        Flag indicating whether to consider shaoes when calculating the extent
-    img_transformations
-        List of transformations already applied to the images
+    has_shapes
+        Flag indicating whether to consider shapes when calculating the extent
+    elements
+        Optional list of element names to be considered. When None, all are used.
+    share_extent
+        Flag indicating whether to use the same extent for all coordinate systems
 
     Returns
     -------
     A dict of tuples with the shape (xmin, xmax, ymin, ymax). The keys of the
         dict are the coordinate_system keys.
 
     """
-    extent: dict[str, tuple[int, int, int, int]] = {}
+    extent: dict[str, dict[str, Sequence[int]]] = {}
     cs_mapping = _get_coordinate_system_mapping(sdata)
     cs_contents = _get_cs_contents(sdata)
 
+    if elements is None:  # to shut up ruff
+        elements = []
+
+    if not isinstance(elements, list):
+        raise ValueError(f"Invalid type of `elements`: {type(elements)}, expected `list`.")
+
+    if coordinate_systems is not None:
+        if isinstance(coordinate_systems, str):
+            coordinate_systems = [coordinate_systems]
+        cs_contents = cs_contents[cs_contents["cs"].isin(coordinate_systems)]
+        cs_mapping = {k: v for k, v in cs_mapping.items() if k in coordinate_systems}
+
     for cs_name, element_ids in cs_mapping.items():
-        x_dims = []
-        y_dims = []
+        extent[cs_name] = {}
+        if len(elements) > 0:
+            element_ids = [e for e in element_ids if e in elements]
+
+        def _get_extent_after_transformations(element: Any, cs_name: str) -> Sequence[int]:
+            tmp = element.copy()
+            if len(tmp.shape) == 3:
+                x_idx = 2
+                y_idx = 1
+            elif len(tmp.shape) == 2:
+                x_idx = 1
+                y_idx = 0
+
+            transformations = get_transformation(tmp, to_coordinate_system=cs_name)
+            transformations = _flatten_transformation_sequence(transformations)
+
+            if len(transformations) == 1 and isinstance(
+                transformations[0], sd.transformations.transformations.Identity
+            ):
+                result = (0, tmp.shape[x_idx], 0, tmp.shape[y_idx])
 
-        # Using two for-loops in the following code to avoid partial matches
-        # since "aa" in ["aaa", "bbb"] would return true
+            else:
+                origin = {
+                    "x": 0,
+                    "y": 0,
+                }
+                for t in transformations:
+                    if isinstance(t, sd.transformations.transformations.Translation):
+                        tmp = _translate_image(image=tmp, translation=t)
+
+                        for idx, ax in enumerate(t.axes):
+                            origin["x"] += t.translation[idx] if ax == "x" else 0
+                            origin["y"] += t.translation[idx] if ax == "y" else 0
+
+                    else:
+                        tmp = transform(tmp, t)
+
+                        if isinstance(t, sd.transformations.transformations.Scale):
+                            for idx, ax in enumerate(t.axes):
+                                origin["x"] *= t.scale[idx] if ax == "x" else 1
+                                origin["y"] *= t.scale[idx] if ax == "y" else 1
+
+                        elif isinstance(t, sd.transformations.transformations.Affine):
+                            pass
 
-        if images and cs_contents.query(f"cs == '{cs_name}'")["has_images"][0]:
-            for images_key in sdata.images:
-                for element_id in element_ids:
-                    if images_key == element_id:
-                        tmp = sdata.images[element_id]
-
-                        # calculate original image extent
-                        if img_transformations is not None:
-                            shifts: dict[str, float] = {}
-                            shifts["c"] = tmp.shape[0]
-                            shifts["y"] = tmp.shape[1]
-                            shifts["x"] = tmp.shape[2]
-
-                            if isinstance(
-                                img_transformations[images_key][cs_name], sd.transformations.transformations.Sequence
-                            ):
-                                transformations = list(img_transformations[images_key][cs_name].transformations)
+                result = (origin["x"], tmp.shape[x_idx], origin["y"], tmp.shape[y_idx])
 
-                            else:
-                                transformations = [img_transformations[images_key][cs_name]]
+            del tmp
+            return result
 
-                            # First reverse all scaling
-                            for transformation in transformations:
-                                if isinstance(transformation, sd.transformations.transformations.Scale):
-                                    for idx, ax in enumerate(transformation.axes):
-                                        shifts["c"] /= transformation.scale[idx] if ax == "c" else 1
-                                        shifts["x"] /= transformation.scale[idx] if ax == "x" else 1
-                                        shifts["y"] /= transformation.scale[idx] if ax == "y" else 1
-
-                            # Then the shift
-                            for transformation in transformations:
-                                if isinstance(transformation, sd.transformations.transformations.Translation):
-                                    for idx, ax in enumerate(transformation.axes):
-                                        shifts["c"] -= transformation.translation[idx] if ax == "c" else 0
-                                        shifts["x"] -= transformation.translation[idx] if ax == "x" else 0
-                                        shifts["y"] -= transformation.translation[idx] if ax == "y" else 0
-
-                                for ax in ["c", "x", "y"]:
-                                    shifts[ax] = int(shifts[ax])
-
-                        y_dims += [(tmp.shape[1] - shifts["y"], tmp.shape[1])]  # img is cyx, so we skip 0
-                        x_dims += [(tmp.shape[2] - shifts["x"], tmp.shape[2])]
-                        del tmp
+        if has_images and cs_contents.query(f"cs == '{cs_name}'")["has_images"][0]:
+            for images_key in sdata.images:
+                for e_id in element_ids:
+                    if images_key == e_id:
+                        if not isinstance(sdata.images[e_id], msi.multiscale_spatial_image.MultiscaleSpatialImage):
+                            extent[cs_name][e_id] = _get_extent_after_transformations(sdata.images[e_id], cs_name)
+                        else:
+                            pass
 
-        if labels and cs_contents.query(f"cs == '{cs_name}'")["has_labels"][0]:
+        if has_labels and cs_contents.query(f"cs == '{cs_name}'")["has_labels"][0]:
             for labels_key in sdata.labels:
-                for element_id in element_ids:
-                    if labels_key == element_id:
-                        tmp = sdata.labels[element_id]
-                        y_dims += [(0, tmp.shape[0])]
-                        x_dims += [(0, tmp.shape[1])]
-                        del tmp
+                for e_id in element_ids:
+                    if labels_key == e_id:
+                        if not isinstance(sdata.labels[e_id], msi.multiscale_spatial_image.MultiscaleSpatialImage):
+                            extent[cs_name][e_id] = _get_extent_after_transformations(sdata.labels[e_id], cs_name)
+                        else:
+                            pass
 
-        if points and cs_contents.query(f"cs == '{cs_name}'")["has_points"][0]:
-            for points_key in sdata.points:
-                for element_id in element_ids:
-                    if points_key == element_id:
-                        tmp = sdata.points[element_id]
-                        y_dims += [(tmp.y.min().compute(), tmp.y.max().compute())]
-                        x_dims += [(tmp.x.min().compute(), tmp.x.max().compute())]
-                        del tmp
-
-        if shapes and cs_contents.query(f"cs == '{cs_name}'")["has_shapes"][0]:
+        if has_shapes and cs_contents.query(f"cs == '{cs_name}'")["has_shapes"][0]:
             for shapes_key in sdata.shapes:
-                for element_id in element_ids:
-                    if shapes_key == element_id:
+                for e_id in element_ids:
+                    if shapes_key == e_id:
 
                         def get_point_bb(
                             point: Point, radius: int, method: Literal["topleft", "bottomright"], buffer: int = 1
                         ) -> Point:
                             x, y = point.coords[0]
                             if method == "topleft":
                                 point_bb = Point(x - radius - buffer, y - radius - buffer)
                             else:
                                 point_bb = Point(x + radius + buffer, y + radius + buffer)
 
                             return point_bb
 
+                        y_dims = []
+                        x_dims = []
+
                         # Split by Point and Polygon:
-                        tmp_points = sdata.shapes[element_id][
-                            sdata.shapes[element_id]["geometry"].apply(lambda geom: geom.geom_type == "Point")
+                        tmp_points = sdata.shapes[e_id][
+                            sdata.shapes[e_id]["geometry"].apply(lambda geom: geom.geom_type == "Point")
                         ]
-                        tmp_polygons = sdata.shapes[element_id][
-                            sdata.shapes[element_id]["geometry"].apply(lambda geom: geom.geom_type == "Polygon")
+                        tmp_polygons = sdata.shapes[e_id][
+                            sdata.shapes[e_id]["geometry"].apply(
+                                lambda geom: geom.geom_type in ["Polygon", "MultiPolygon"]
+                            )
                         ]
 
                         if not tmp_points.empty:
                             tmp_points["point_topleft"] = tmp_points.apply(
                                 lambda row: get_point_bb(row["geometry"], row["radius"], "topleft"),
                                 axis=1,
                             )
                             tmp_points["point_bottomright"] = tmp_points.apply(
                                 lambda row: get_point_bb(row["geometry"], row["radius"], "bottomright"),
                                 axis=1,
                             )
                             xmin_tl, ymin_tl, xmax_tl, ymax_tl = tmp_points["point_topleft"].total_bounds
                             xmin_br, ymin_br, xmax_br, ymax_br = tmp_points["point_bottomright"].total_bounds
-                            y_dims += [(min(ymin_tl, ymin_br), max(ymax_tl, ymax_br))]
-                            x_dims += [(min(xmin_tl, xmin_br), max(xmax_tl, xmax_br))]
+                            y_dims += [min(ymin_tl, ymin_br), max(ymax_tl, ymax_br)]
+                            x_dims += [min(xmin_tl, xmin_br), max(xmax_tl, xmax_br)]
 
                         if not tmp_polygons.empty:
                             xmin, ymin, xmax, ymax = tmp_polygons.total_bounds
-                            y_dims += [(ymin, ymax)]
-                            x_dims += [(xmin, xmax)]
+                            y_dims += [ymin, ymax]
+                            x_dims += [xmin, xmax]
 
                         del tmp_points
                         del tmp_polygons
 
-        if len(x_dims) > 0 and len(y_dims) > 0:
-            xmax = max(list(sum(x_dims, ())))
-            xmin = min(list(sum(x_dims, ())))
-            ymax = max(list(sum(y_dims, ())))
-            ymin = min(list(sum(y_dims, ())))
-            extent[cs_name] = (xmin, xmax, ymin, ymax)
+                        extent[cs_name][e_id] = x_dims + y_dims
+
+                        transformations = get_transformation(sdata.shapes[e_id], to_coordinate_system=cs_name)
+                        transformations = _flatten_transformation_sequence(transformations)
+
+                        for t in transformations:
+                            if isinstance(t, sd.transformations.transformations.Translation):
+                                for idx, ax in enumerate(t.axes):
+                                    extent[cs_name][e_id][0] += t.translation[idx] if ax == "x" else 0  # type: ignore
+                                    extent[cs_name][e_id][1] += t.translation[idx] if ax == "x" else 0  # type: ignore
+                                    extent[cs_name][e_id][2] += t.translation[idx] if ax == "y" else 0  # type: ignore
+                                    extent[cs_name][e_id][3] += t.translation[idx] if ax == "y" else 0  # type: ignore
 
-    return extent
+                            else:
+                                if isinstance(t, sd.transformations.transformations.Scale):
+                                    for idx, ax in enumerate(t.axes):
+                                        extent[cs_name][e_id][1] *= t.scale[idx] if ax == "x" else 1  # type: ignore
+                                        extent[cs_name][e_id][3] *= t.scale[idx] if ax == "y" else 1  # type: ignore
+
+                                elif isinstance(t, sd.transformations.transformations.Affine):
+                                    pass
+
+        if has_points and cs_contents.query(f"cs == '{cs_name}'")["has_points"][0]:
+            for points_key in sdata.points:
+                for e_id in element_ids:
+                    if points_key == e_id:
+                        tmp = sdata.points[points_key]
+                        xmin = tmp["x"].min().compute()
+                        xmax = tmp["x"].max().compute()
+                        ymin = tmp["y"].min().compute()
+                        ymax = tmp["y"].max().compute()
+                        extent[cs_name][e_id] = [xmin, xmax, ymin, ymax]
+
+    cswise_extent = {}
+    for cs_name, cs_contents in extent.items():
+        if len(cs_contents) > 0:
+            xmin = min([v[0] for v in cs_contents.values()])
+            xmax = max([v[1] for v in cs_contents.values()])
+            ymin = min([v[2] for v in cs_contents.values()])
+            ymax = max([v[3] for v in cs_contents.values()])
+            cswise_extent[cs_name] = (xmin, xmax, ymin, ymax)
+
+    if share_extent:
+        global_extent = {}
+        if len(cs_contents) > 0:
+            xmin = min([v[0] for v in cswise_extent.values()])
+            xmax = max([v[1] for v in cswise_extent.values()])
+            ymin = min([v[2] for v in cswise_extent.values()])
+            ymax = max([v[3] for v in cswise_extent.values()])
+            for cs_name in cswise_extent:
+                global_extent[cs_name] = (xmin, xmax, ymin, ymax)
+        return global_extent
+
+    return cswise_extent
 
 
 def _panel_grid(
     num_panels: int,
     hspace: float,
     wspace: float,
     ncols: int,
@@ -388,21 +453,22 @@
     cmap: Colormap
     norm: Normalize
     na_color: str | tuple[float, ...] = (0.0, 0.0, 0.0, 0.0)
 
 
 def _prepare_cmap_norm(
     cmap: Colormap | str | None = None,
-    norm: _Normalize | None = None,
+    norm: Normalize | Sequence[Normalize] | None = None,
     na_color: str | tuple[float, ...] = (0.0, 0.0, 0.0, 0.0),
     vmin: float | None = None,
     vmax: float | None = None,
     vcenter: float | None = None,
+    **kwargs: Any,
 ) -> CmapParams:
-    cmap = copy(get_cmap(cmap))
+    cmap = copy(matplotlib.colormaps[rcParams["image.cmap"] if cmap is None else cmap])
     cmap.set_bad("lightgray" if na_color is None else na_color)
 
     if isinstance(norm, Normalize):
         pass  # TODO
     elif vcenter is None:
         norm = Normalize(vmin=vmin, vmax=vmax)
     else:
@@ -412,42 +478,43 @@
 
 
 @dataclass
 class OutlineParams:
     """Cmap params."""
 
     outline: bool
+    outline_color: str | list[float]
     gap_size: float
-    gap_color: str
     bg_size: float
-    bg_color: str
 
 
 def _set_outline(
     size: float,
     outline: bool = False,
     outline_width: tuple[float, float] = (0.3, 0.05),
-    outline_color: tuple[str, str] = ("black", "white"),
+    outline_color: str | list[float] = "#0000000ff",  # black, white
     **kwargs: Any,
 ) -> OutlineParams:
     bg_width, gap_width = outline_width
     point = np.sqrt(size)
     gap_size = (point + (point * gap_width) * 2) ** 2
     bg_size = (np.sqrt(gap_size) + (point * bg_width) * 2) ** 2
     # the default black and white colors can be changes using the contour_config parameter
-    bg_color, gap_color = outline_color
+
+    if (len(outline_color) == 3 or len(outline_color) == 4) and all(isinstance(c, float) for c in outline_color):
+        outline_color = matplotlib.colors.to_hex(outline_color)
 
     if outline:
         kwargs.pop("edgecolor", None)  # remove edge from kwargs if present
         kwargs.pop("alpha", None)  # remove alpha from kwargs if present
 
-    return OutlineParams(outline, gap_size, gap_color, bg_size, bg_color)
+    return OutlineParams(outline, outline_color, gap_size, bg_size)
 
 
-def _get_subplots(num_images: int, ncols: int = 4, width: int = 4, height: int = 3) -> Union[plt.Figure, plt.Axes]:
+def _get_subplots(num_images: int, ncols: int = 4, width: int = 4, height: int = 3) -> plt.Figure | plt.Axes:
     """Set up the axs objects.
 
     Parameters
     ----------
     num_images
         Number of images to plot. Must be greater than 1.
     ncols
@@ -527,53 +594,60 @@
     colors = cmap(norm(values))
 
     return [colors.to_hex(color) for color in colors]
 
 
 def _normalize(
     img: xr.DataArray,
-    pmin: float = 3.0,
-    pmax: float = 99.8,
+    pmin: float | None = 3.0,
+    pmax: float | None = 99.8,
     eps: float = 1e-20,
     clip: bool = False,
     name: str = "normed",
 ) -> xr.DataArray:
     """Perform a min max normalisation on the xr.DataArray.
 
     This function was adapted from the csbdeep package.
 
     Parameters
     ----------
     dataarray
         A xarray DataArray with an image field.
     pmin
-        Lower quantile (min value) used to perform qunatile normalization.
+        Lower quantile (min value) used to perform quantile normalization.
     pmax
-        Upper quantile (max value) used to perform qunatile normalization.
+        Upper quantile (max value) used to perform quantile normalization.
     eps
         Epsilon float added to prevent 0 division.
     clip
         Ensures that normed image array contains no values greater than 1.
 
     Returns
     -------
     xr.DataArray
         A min-max normalized image.
     """
-    perc = np.percentile(img, [pmin, pmax], axis=(1, 2)).T
+    pmin = pmin or 0.0
+    pmax = pmax or 100.0
 
-    norm = (img - np.expand_dims(perc[:, 0], (1, 2))) / (np.expand_dims(perc[:, 1] - perc[:, 0], (1, 2)) + eps)
+    perc = np.percentile(img, [pmin, pmax])
+
+    norm = (img - perc[0]) / (perc[1] - perc[0] + eps)
 
     if clip:
         norm = np.clip(norm, 0, 1)
 
     return norm
 
 
-def _get_colors_for_categorical_obs(categories: Sequence[Union[str, int]], palette: Palette_t = None) -> list[str]:
+def _get_colors_for_categorical_obs(
+    categories: Sequence[str | int],
+    palette: ListedColormap | str | None = None,
+    alpha: float = 1.0,
+) -> list[str]:
     """
     Return a list of colors for a categorical observation.
 
     Parameters
     ----------
     adata
         AnnData object
@@ -582,45 +656,60 @@
     categories
         categories of the categorical observation.
 
     Returns
     -------
     None
     """
-    length = len(categories)
+    len_cat = len(categories)
 
     # check if default matplotlib palette has enough colors
     if palette is None:
-        if len(rcParams["axes.prop_cycle"].by_key()["color"]) >= length:
+        if len(rcParams["axes.prop_cycle"].by_key()["color"]) >= len_cat:
             cc = rcParams["axes.prop_cycle"]()
-            palette = [next(cc)["color"] for _ in range(length)]
+            palette = [next(cc)["color"] for _ in range(len_cat)]
         else:
-            if length <= 20:
+            if len_cat <= 20:
                 palette = default_20
-            elif length <= 28:
+            elif len_cat <= 28:
                 palette = default_28
-            elif length <= len(default_102):  # 103 colors
+            elif len_cat <= len(default_102):  # 103 colors
                 palette = default_102
             else:
-                palette = ["grey" for _ in range(length)]
+                palette = ["grey" for _ in range(len_cat)]
                 logging.info(
                     "input has more than 103 categories. Uniform " "'grey' color will be used for all categories."
                 )
 
-    return palette[:length]  # type: ignore[return-value]
+    # otherwise, single chanels turn out grey
+    color_idx = np.linspace(0, 1, len_cat) if len_cat > 1 else [0.7]
+
+    if isinstance(palette, str):
+        cmap = plt.get_cmap(palette)
+        palette = [to_hex(x) for x in cmap(color_idx, alpha=alpha)]
+    elif isinstance(palette, list):
+        palette = [to_hex(x) for x in palette]
+    elif isinstance(palette, ListedColormap):
+        palette = [to_hex(x) for x in palette(color_idx, alpha=alpha)]
+    elif isinstance(palette, LinearSegmentedColormap):
+        palette = [to_hex(palette(x, alpha=alpha)) for x in color_idx]  # type: ignore[attr-defined]
+    else:
+        raise TypeError(f"Palette is {type(palette)} but should be string or `ListedColormap`.")
+
+    return palette[:len_cat]  # type: ignore[return-value]
 
 
 def _set_color_source_vec(
     adata: AnnData,
     value_to_plot: str | None,
     use_raw: bool | None = None,
     alt_var: str | None = None,
     layer: str | None = None,
-    groups: _SeqStr | None = None,
-    palette: Palette_t = None,
+    groups: Sequence[str] | str | None = None,
+    palette: ListedColormap | str | None = None,
     na_color: str | tuple[float, ...] | None = None,
     alpha: float = 1.0,
 ) -> tuple[ArrayLike | pd.Series | None, ArrayLike, bool]:
     if value_to_plot is None:
         color = np.full(adata.n_obs, to_hex(na_color))
         return color, color, False
 
@@ -632,20 +721,22 @@
         color_source_vector = adata.obs_vector(value_to_plot, layer=layer)
 
     if not is_categorical_dtype(color_source_vector):
         return None, color_source_vector, False
 
     color_source_vector = pd.Categorical(color_source_vector)  # convert, e.g., `pd.Series`
     categories = color_source_vector.categories
+
     if groups is not None:
         color_source_vector = color_source_vector.remove_categories(categories.difference(groups))
 
-    color_map = _get_palette(
-        adata=adata, cluster_key=value_to_plot, categories=categories, palette=palette, alpha=alpha
-    )
+    color_map = dict(zip(categories, _get_colors_for_categorical_obs(categories)))
+    # color_map = _get_palette(
+    #     adata=adata, cluster_key=value_to_plot, categories=categories, palette=palette, alpha=alpha
+    # )
     if color_map is None:
         raise ValueError("Unable to create color palette.")
 
     # do not rename categories, as colors need not be unique
     color_vector = color_source_vector.map(color_map)
     if color_vector.isna().any():
         color_vector = color_vector.add_categories([to_hex(na_color)])
@@ -704,16 +795,16 @@
 
     return np.dstack((seg_im, np.where(val_im > 0, 1, 0)))
 
 
 def _get_palette(
     categories: Sequence[Any],
     adata: AnnData | None = None,
-    cluster_key: Optional[str] | None = None,
-    palette: Palette_t = None,
+    cluster_key: None | str = None,
+    palette: ListedColormap | str | None = None,
     alpha: float = 1.0,
 ) -> Mapping[str, str] | None:
     if adata is not None and palette is None:
         try:
             palette = adata.uns[f"{cluster_key}_colors"]  # type: ignore[arg-type]
             if len(palette) != len(categories):
                 raise ValueError(
@@ -781,33 +872,27 @@
 def _decorate_axs(
     ax: Axes,
     cax: PatchCollection,
     fig_params: FigParams,
     adata: AnnData,
     value_to_plot: str | None,
     color_source_vector: pd.Series[CategoricalDtype],
-    palette: Palette_t = None,
+    palette: ListedColormap | str | None = None,
     alpha: float = 1.0,
     na_color: str | tuple[float, ...] = (0.0, 0.0, 0.0, 0.0),
     legend_fontsize: int | float | _FontSize | None = None,
     legend_fontweight: int | _FontWeight = "bold",
     legend_loc: str | None = "right margin",
     legend_fontoutline: int | None = None,
     na_in_legend: bool = True,
     colorbar: bool = True,
     scalebar_dx: Sequence[float] | None = None,
     scalebar_units: Sequence[str] | None = None,
     scalebar_kwargs: Mapping[str, Any] = MappingProxyType({}),
 ) -> Axes:
-    # ax.set_yticks([])
-    # ax.set_xticks([])
-    # ax.set_xlabel(fig_params.ax_labels[0])
-    # ax.set_ylabel(fig_params.ax_labels[1])
-    # ax.autoscale_view()  # needed when plotting points but no image
-
     if value_to_plot is not None:
         # if only dots were plotted without an associated value
         # there is not need to plot a legend or a colorbar
 
         if legend_fontoutline is not None:
             path_effect = [patheffects.withStroke(linewidth=legend_fontoutline, foreground="w")]
         else:
@@ -1005,7 +1090,85 @@
             shifted_channels.append(channel)
 
     return Image2DModel.parse(
         np.array(shifted_channels),
         dims=["c", "y", "x"],
         transformations=image.attrs["transform"],
     )
+
+
+def _convert_polygon_to_linestrings(polygon: Polygon) -> list[LineString]:
+    b = polygon.boundary.coords
+    linestrings = [LineString(b[k : k + 2]) for k in range(len(b) - 1)]
+
+    return [list(ls.coords) for ls in linestrings]
+
+
+def _flatten_transformation_sequence(
+    transformation_sequence: list[sd.transformations.transformations.Sequence],
+) -> list[sd.transformations.transformations.Sequence]:
+    if isinstance(transformation_sequence, sd.transformations.transformations.Sequence):
+        transformations = list(transformation_sequence.transformations)
+        found_bottom_of_tree = False
+        while not found_bottom_of_tree:
+            if all(not isinstance(t, sd.transformations.transformations.Sequence) for t in transformations):
+                found_bottom_of_tree = True
+            else:
+                for idx, t in enumerate(transformations):
+                    if isinstance(t, sd.transformations.transformations.Sequence):
+                        transformations.pop(idx)
+                        transformations += t.transformations
+
+        return transformations
+
+    if isinstance(transformation_sequence, sd.transformations.transformations.BaseTransformation):
+        return [transformation_sequence]
+
+    raise TypeError("Parameter 'transformation_sequence' must be a Sequence.")
+
+
+def _robust_transform(element: Any, cs: str) -> Any:
+    try:
+        transformations = get_transformation(element, get_all=True)
+        if cs not in transformations:
+            return element
+        transformations = transformations[cs]
+        transformations = _flatten_transformation_sequence(transformations)
+        for _, t in enumerate(transformations):
+            if isinstance(t, sd.transformations.transformations.Translation):
+                element = _translate_image(image=element, translation=t)
+
+            elif isinstance(t, sd.transformations.transformations.Affine):
+                # edge case, waiting for Luca to decompose affine into components
+                # element = transform(element, t)
+                # new_transformations = get_transformation(element, get_all=True)
+                # new_transformations = new_transformations[cs]
+                # new_transformations = _flatten_transformation_sequence(new_transformations)
+                # seq = new_transformations[:len(new_transformations) - len(transformations)]
+                # seq = sd.transformations.Sequence(seq)
+                # set_transformation(element, seq, to_coordinate_system=cs)
+                # element = _robust_transform(element, cs)
+                # print(element.shape)
+                pass
+
+            else:
+                element = transform(element, t)
+
+    except ValueError as e:
+        # hack, talk to Luca
+        raise ValueError("Unable to transform element.") from e
+
+    return element
+
+
+def _mpl_ax_contains_elements(ax: Axes) -> bool:
+    """Check if any objects have been plotted on the axes object.
+
+    While extracting the extent, we need to know if the axes object has just been
+    initialised and therefore has extent (0, 1), (0,1) or if it has been plotted on
+    and therefore has a different extent.
+
+    Based on: https://stackoverflow.com/a/71966295
+    """
+    return (
+        len(ax.lines) > 0 or len(ax.collections) > 0 or len(ax.images) > 0 or len(ax.patches) > 0 or len(ax.tables) > 0
+    )
```

### Comparing `spatialdata_plot-0.0.2/src/spatialdata_plot/pp/basic.py` & `spatialdata_plot-0.0.3/src/spatialdata_plot/pp/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         If the original spatial data object has no table, or if `elements` does
         not include label keys, the returned spatialdata object will have no
         table.
         """
         if not isinstance(elements, (str, list)):
             raise TypeError("Parameter 'elements' must be a string or a list of strings.")
 
-        if not all([isinstance(e, str) for e in elements]):
+        if not all(isinstance(e, str) for e in elements):
             raise TypeError("When parameter 'elements' is a list, all elements must be strings.")
 
         if isinstance(elements, str):
             elements = [elements]
 
         coord_keys = []
         image_keys = []
```

### Comparing `spatialdata_plot-0.0.2/src/spatialdata_plot/pp/utils.py` & `spatialdata_plot-0.0.3/src/spatialdata_plot/pp/utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/tests/conftest.py` & `spatialdata_plot-0.0.3/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from geopandas import GeoDataFrame
 from matplotlib.testing.compare import compare_images
 from multiscale_spatial_image import MultiscaleSpatialImage
 from numpy.random import default_rng
 from shapely.geometry import MultiPolygon, Polygon
 from spatial_image import SpatialImage
 from spatialdata import SpatialData
-from spatialdata.datasets import blobs
+from spatialdata.datasets import blobs, raccoon
 from spatialdata.models import (
     Image2DModel,
     Image3DModel,
     Labels2DModel,
     Labels3DModel,
     PointsModel,
     ShapesModel,
@@ -52,14 +52,19 @@
 
 
 @pytest.fixture()
 def sdata_blobs() -> SpatialData:
     return blobs()
 
 
+@pytest.fixture()
+def sdata_raccoon() -> SpatialData:
+    return raccoon()
+
+
 @pytest.fixture
 def test_sdata_single_image():
     """Creates a simple sdata object."""
     images = {
         "data1_image": sd.models.Image2DModel.parse(
             np.zeros((1, 10, 10)), dims=("c", "y", "x"), transformations={"data1": sd.transformations.Identity()}
         )
```

### Comparing `spatialdata_plot-0.0.2/tests/test_pp.py` & `spatialdata_plot-0.0.3/tests/test_pp.py`

 * *Files 8% similar despite different names*

```diff
@@ -146,28 +146,7 @@
         sdata.pp.get_bb((0, 5, 1), (0, 5))
 
     with pytest.raises(ValueError, match="Parameter 'y' must be of length 2."):
         sdata.pp.get_bb([0, 5], [0, 5, 5])
 
     with pytest.raises(ValueError, match="Parameter 'y' must be of length 2."):
         sdata.pp.get_bb((0, 5), (0, 5, 2))
-
-
-# @pytest.mark.parametrize(
-#     "sdata, keys, nrows ",
-#     [
-#         ("full_sdata", "data1", 3),
-#         ("full_sdata", ["data1", "data3"], 23),
-#     ],
-# )
-# def test_table_gets_subset_when_images_are_subset(sdata, keys, nrows, request):
-#     """Tests wether the images inside sdata can be clipped to a bounding box."""
-
-#     sdata = request.getfixturevalue(sdata)
-
-#     assert sdata.table.n_obs == 30
-
-#     new_sdata = sdata.pp.get_elements(keys)
-
-#     print(new_sdata.table)
-
-#     assert len(new_sdata.table.obs) == nrows
```

### Comparing `spatialdata_plot-0.0.2/tests/_images/Images_images.png` & `spatialdata_plot-0.0.3/tests/_images/Extent_extent_of_img_full_canvas.png`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/tests/pl/test_plot.py` & `spatialdata_plot-0.0.3/tests/pl/test_show.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,20 @@
 from spatialdata import SpatialData
 
 from tests.conftest import PlotTester, PlotTesterMeta
 
 sc.pl.set_rcParams_defaults()
 sc.set_figure_params(dpi=40, color_map="viridis")
 matplotlib.use("agg")  # same as GitHub action runner
+_ = spatialdata_plot
 
 # WARNING:
 # 1. all classes must both subclass PlotTester and use metaclass=PlotTesterMeta
 # 2. tests which produce a plot must be prefixed with `test_plot_`
 # 3. if the tolerance needs to be changed, don't prefix the function with `test_plot_`, but with something else
 #    the comp. function can be accessed as `self.compare(<your_filename>, tolerance=<your_tolerance>)`
 #    ".png" is appended to <your_filename>, no need to set it
 
 
-class TestLabels(PlotTester, metaclass=PlotTesterMeta):
-    def test_plot_labels(self, sdata_blobs: SpatialData):
-        sdata_blobs.pl.render_labels(color="channel_2_mean").pl.show()
-
-
-class TestImages(PlotTester, metaclass=PlotTesterMeta):
-    def test_plot_images(self, sdata_blobs: SpatialData):
-        sdata_blobs.pl.render_images().pl.show()
+class TestShow(PlotTester, metaclass=PlotTesterMeta):
+    def test_plot_pad_extent_adds_padding(self, sdata_blobs: SpatialData):
+        sdata_blobs.pl.render_images(elements="blobs_image").pl.show(pad_extent=100)
```

### Comparing `spatialdata_plot-0.0.2/tests/pl/test_render.py` & `spatialdata_plot-0.0.3/tests/pl/test_render.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,12 +25,12 @@
     sdata = fun(share_coordinate_system)
     sdata.pl.render_images().pl.show()
     axs = plt.gcf().get_axes()
 
     if share_coordinate_system == "all":
         assert len(axs) == 1
 
-    elif share_coordinate_system == "two":
+    if share_coordinate_system == "two":
         assert len(axs) == 2
 
-    elif share_coordinate_system == "none":
+    if share_coordinate_system == "none":
         assert len(axs) == 3
```

### Comparing `spatialdata_plot-0.0.2/tests/pp/test_basic.py` & `spatialdata_plot-0.0.3/tests/pp/test_basic.py`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/LICENSE` & `spatialdata_plot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata_plot-0.0.2/README.md` & `spatialdata_plot-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# spatialdata-plot
+![SpatialData banner](https://github.com/scverse/spatialdata/blob/main/docs/_static/img/spatialdata_horizontal.png?raw=true)
+
+# spatialdata-plot: rich static plotting from SpatialData objects
 
 [![Tests][badge-tests]][link-tests]
 [![Documentation][badge-docs]][link-docs]
 [![Codecov][badge-codecov]][link-codecov]
 
-[badge-tests]: https://img.shields.io/github/actions/workflow/status/scverse/spatialdata-plot/test.yaml?branch=main
+[badge-tests]: https://img.shields.io/github/actions/workflow/status/scverse/spatialdata-plot/test_and_deploy.yaml?branch=main
 [link-tests]: https://github.com/scverse/spatialdata-plot/actions/workflows/test.yml
 [badge-docs]: https://img.shields.io/readthedocs/spatialdata-plot
 [badge-codecov]: https://codecov.io/gh/scverse/spatialdata-plot/branch/main/graph/badge.svg?token=C45F3ATSVI
 [link-codecov]: https://app.codecov.io/gh/scverse/spatialdata-plot
 
 The `spatialdata-plot` package extends `spatialdata` with a declarative plotting API that enables to quickly visualize `spatialdata` objects and their respective elements (i.e. `images`, `labels`, `points` and `shapes`).
 
 SpatialData’s plotting capabilities allow to quickly visualise all contained modalities. The user can specify which elements should be rendered (images, labels, points, shapes) and specify certain parameters for each layer, such as for example the intent to color shapes by a gene’s expression profile or which color to use for which image channel. When the plot is then eventually displayed, all transformations, alignments and coordinate systems are internally processed to form the final visualisation. In concordance with the general SpatialData philosophy, all modalities of the major spatial technologies are supported out of the box.
 
 <img src='https://raw.githubusercontent.com/scverse/spatialdata-plot/main/docs/spatialdata-plot.png'/>
 
 ## Getting started
 
-For more information on the `spatialdata` format, please refer to the [documentation](https://spatialdata.scverse.org/en/latest/). In particular, the
+For more information on the `spatialdata-plot` library, please refer to the [documentation](https://spatialdata.scverse.org/projects/plot/en/latest/index.html). In particular, the
 
 -   [API documentation][link-api].
--   [Design doc][link-design-doc].
--   [Example notebooks][link-notebooks].
-
-For usage examples, please refer to the ["Visualizations"](https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks.html#visualizations) section of `spatialdata`.
+-   [Example notebooks][link-notebooks] (section "Visiualizations")
 
 ## Installation
 
 You need to have Python 3.8 or newer installed on your system. If you don't have
 Python installed, we recommend installing [Mambaforge](https://github.com/conda-forge/miniforge#mambaforge).
 
 There are several alternative options to install spatialdata-plot:
@@ -50,16 +49,22 @@
 ## Contact
 
 For questions and help requests, you can reach out in the [scverse discourse][scverse-discourse].
 If you found a bug, please use the [issue tracker][issue-tracker].
 
 ## Citation
 
-> t.b.a
+If you use `spatialdata` in your work, please cite the `spatialdata` publication as follows:
+
+> SpatialData: an open and universal data framework for spatial omics
+>
+> Luca Marconato, Giovanni Palla, Kevin A. Yamauchi, Isaac Virshup, Elyas Heidari, Tim Treis, Marcella Toth, Rahul Shrestha, Harald Vöhringer, Wolfgang Huber, Moritz Gerstung, Josh Moore, Fabian J. Theis, Oliver Stegle
+>
+> bioRxiv 2023.05.05.539647; doi: https://doi.org/10.1101/2023.05.05.539647
 
 [scverse-discourse]: https://discourse.scverse.org/
 [issue-tracker]: https://github.com/scverse/spatialdata-plot/issues
 [changelog]: https://spatialdata-plot.readthedocs.io/latest/changelog.html
 [link-docs]: https://spatialdata-plot.readthedocs.io
-[link-api]: https://spatialdata.scverse.org/projects/plot/en/latest
+[link-api]: https://spatialdata.scverse.org/projects/plot/en/latest/api.html
 [link-design-doc]: https://spatialdata.scverse.org/en/latest/design_doc.html
 [link-notebooks]: https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks.html
```

### Comparing `spatialdata_plot-0.0.2/pyproject.toml` & `spatialdata_plot-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling", "hatch-vcs"]
 
-
 [project]
 name = "spatialdata-plot"
-description = "Static plotting for SpatialData."
+description = "Static plotting for spatial data."
 authors = [
     {name = "scverse"},
 ]
 maintainers = [
     {name = "scverse", email = "tim.treis@helmholtz-munich.de"},
 ]
-urls.Documentation = "https://spatialdata.scverse.org/projects/plot/en/latest/"
+urls.Documentation = "https://spatialdata.readthedocs.io/"
 urls.Source = "https://github.com/scverse/spatialdata-plot.git"
 urls.Home-page = "https://github.com/scverse/spatialdata-plot.git"
+requires-python = ">=3.9"
 dynamic= [
   "version" # allow version to be set by git tags
 ]
-requires-python = ">=3.9"
 license = {file = "LICENSE"}
 readme = "README.md"
 dependencies = [
     "spatialdata",
     "matplotlib",
     "scikit-learn",
     "scanpy",
@@ -47,22 +46,17 @@
     "ipython>=8.6.0",
     "sphinx-copybutton",
 ]
 test = [
     "pytest",
     "pytest-cov",
 ]
-torch = [
-    "torch"
-]
-extra  = [
-]
 
 [tool.coverage.run]
-source = ["spatialdata-plot"]
+source = ["spatialdata_plot"]
 omit = [
     "**/test_*.py",
 ]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 xfail_strict = true
@@ -96,26 +90,26 @@
   )/
 )
 '''
 
 [tool.jupytext]
 formats = "ipynb,md"
 
-[tool.hatch.metadata]
-allow-direct-references = true
-
 [tool.hatch.build.targets.wheel]
 packages = ['src/spatialdata_plot']
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "_version.py"
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [tool.ruff]
 exclude = [
     ".git",
     ".tox",
     "__pycache__",
     "build",
     "docs/_build",
@@ -167,10 +161,7 @@
     "*/__init__.py" = ["F401", "D104", "D107", "E402"]
     "docs/*" = ["D","B","E","A"]
     # "src/spatialdata/transformations/transformations.py" = ["D101","D102", "D106", "B024", "T201", "RET504"]
     "tests/conftest.py"= ["E402", "RET504"]
     "src/spatialdata_plot/pl/utils.py"= ["PGH003"]
 [tool.ruff.pydocstyle]
 convention = "numpy"
-[tool.ruff.pyupgrade]
-# Preserve types, even if a file imports `from __future__ import annotations`.
-keep-runtime-typing = true
```

### Comparing `spatialdata_plot-0.0.2/PKG-INFO` & `spatialdata_plot-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: spatialdata-plot
-Version: 0.0.2
-Summary: Static plotting for SpatialData.
-Project-URL: Documentation, https://spatialdata.scverse.org/projects/plot/en/latest/
+Version: 0.0.3
+Summary: Static plotting for spatial data.
+Project-URL: Documentation, https://spatialdata.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/spatialdata-plot.git
 Project-URL: Home-page, https://github.com/scverse/spatialdata-plot.git
 Author: scverse
 Maintainer-email: scverse <tim.treis@helmholtz-munich.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, scverse
@@ -53,49 +53,45 @@
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-book-theme>=1.0.0; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-design; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Requires-Dist: sphinx>=4.5; extra == 'docs'
 Requires-Dist: sphinxcontrib-bibtex>=1.0.0; extra == 'docs'
-Provides-Extra: extra
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
-Provides-Extra: torch
-Requires-Dist: torch; extra == 'torch'
 Description-Content-Type: text/markdown
 
-# spatialdata-plot
+![SpatialData banner](https://github.com/scverse/spatialdata/blob/main/docs/_static/img/spatialdata_horizontal.png?raw=true)
+
+# spatialdata-plot: rich static plotting from SpatialData objects
 
 [![Tests][badge-tests]][link-tests]
 [![Documentation][badge-docs]][link-docs]
 [![Codecov][badge-codecov]][link-codecov]
 
-[badge-tests]: https://img.shields.io/github/actions/workflow/status/scverse/spatialdata-plot/test.yaml?branch=main
+[badge-tests]: https://img.shields.io/github/actions/workflow/status/scverse/spatialdata-plot/test_and_deploy.yaml?branch=main
 [link-tests]: https://github.com/scverse/spatialdata-plot/actions/workflows/test.yml
 [badge-docs]: https://img.shields.io/readthedocs/spatialdata-plot
 [badge-codecov]: https://codecov.io/gh/scverse/spatialdata-plot/branch/main/graph/badge.svg?token=C45F3ATSVI
 [link-codecov]: https://app.codecov.io/gh/scverse/spatialdata-plot
 
 The `spatialdata-plot` package extends `spatialdata` with a declarative plotting API that enables to quickly visualize `spatialdata` objects and their respective elements (i.e. `images`, `labels`, `points` and `shapes`).
 
 SpatialData’s plotting capabilities allow to quickly visualise all contained modalities. The user can specify which elements should be rendered (images, labels, points, shapes) and specify certain parameters for each layer, such as for example the intent to color shapes by a gene’s expression profile or which color to use for which image channel. When the plot is then eventually displayed, all transformations, alignments and coordinate systems are internally processed to form the final visualisation. In concordance with the general SpatialData philosophy, all modalities of the major spatial technologies are supported out of the box.
 
 <img src='https://raw.githubusercontent.com/scverse/spatialdata-plot/main/docs/spatialdata-plot.png'/>
 
 ## Getting started
 
-For more information on the `spatialdata` format, please refer to the [documentation](https://spatialdata.scverse.org/en/latest/). In particular, the
+For more information on the `spatialdata-plot` library, please refer to the [documentation](https://spatialdata.scverse.org/projects/plot/en/latest/index.html). In particular, the
 
 -   [API documentation][link-api].
--   [Design doc][link-design-doc].
--   [Example notebooks][link-notebooks].
-
-For usage examples, please refer to the ["Visualizations"](https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks.html#visualizations) section of `spatialdata`.
+-   [Example notebooks][link-notebooks] (section "Visiualizations")
 
 ## Installation
 
 You need to have Python 3.8 or newer installed on your system. If you don't have
 Python installed, we recommend installing [Mambaforge](https://github.com/conda-forge/miniforge#mambaforge).
 
 There are several alternative options to install spatialdata-plot:
@@ -117,16 +113,22 @@
 ## Contact
 
 For questions and help requests, you can reach out in the [scverse discourse][scverse-discourse].
 If you found a bug, please use the [issue tracker][issue-tracker].
 
 ## Citation
 
-> t.b.a
+If you use `spatialdata` in your work, please cite the `spatialdata` publication as follows:
+
+> SpatialData: an open and universal data framework for spatial omics
+>
+> Luca Marconato, Giovanni Palla, Kevin A. Yamauchi, Isaac Virshup, Elyas Heidari, Tim Treis, Marcella Toth, Rahul Shrestha, Harald Vöhringer, Wolfgang Huber, Moritz Gerstung, Josh Moore, Fabian J. Theis, Oliver Stegle
+>
+> bioRxiv 2023.05.05.539647; doi: https://doi.org/10.1101/2023.05.05.539647
 
 [scverse-discourse]: https://discourse.scverse.org/
 [issue-tracker]: https://github.com/scverse/spatialdata-plot/issues
 [changelog]: https://spatialdata-plot.readthedocs.io/latest/changelog.html
 [link-docs]: https://spatialdata-plot.readthedocs.io
-[link-api]: https://spatialdata.scverse.org/projects/plot/en/latest
+[link-api]: https://spatialdata.scverse.org/projects/plot/en/latest/api.html
 [link-design-doc]: https://spatialdata.scverse.org/en/latest/design_doc.html
 [link-notebooks]: https://spatialdata.scverse.org/en/latest/tutorials/notebooks/notebooks.html
```

