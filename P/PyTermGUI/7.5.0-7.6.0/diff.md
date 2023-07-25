# Comparing `tmp/pytermgui-7.5.0.tar.gz` & `tmp/pytermgui-7.6.0.tar.gz`

## Comparing `pytermgui-7.5.0.tar` & `pytermgui-7.6.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    10604 2020-02-02 00:00:00.000000 pytermgui-7.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     7429 2020-02-02 00:00:00.000000 pytermgui-7.5.0/README.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pytermgui-7.5.0/examples/README.md
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/__init__.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/animations.py
--rw-r--r--   0        0        0    19741 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/ansi_interface.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/cell.py
--rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/cmd.py
--rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/color_info.py
--rw-r--r--   0        0        0    26448 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/colors.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/context_managers.py
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/enums.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/exceptions.py
--rw-r--r--   0        0        0    18790 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/exporters.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/fancy_repr.py
--rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/file_loaders.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/helpers.py
--rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/highlighters.py
--rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/input.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/inspector.py
--rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/palettes.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/prettifiers.py
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/pretty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/py.typed
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/regex.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/serialization.py
--rw-r--r--   0        0        0    16868 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/term.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/win32console.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/aliases.py
--rw-r--r--   0        0        0    14551 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/language.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/macros.py
--rw-r--r--   0        0        0    22738 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/parsing.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/style_maps.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/tokens.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/__init__.py
--rw-r--r--   0        0        0    25604 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/base.py
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/boxes.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/button.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/checkbox.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/collapsible.py
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/color_picker.py
--rw-r--r--   0        0        0    33128 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/containers.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/fancy_repr.py
--rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/frames.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/inline.py
--rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/input_field.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/keyboard_button.py
--rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/pixel_matrix.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/slider.py
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/styles.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/toggle.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/window_manager/__init__.py
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/window_manager/compositor.py
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/window_manager/layouts.py
--rw-r--r--   0        0        0    19978 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/window_manager/manager.py
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/window_manager/window.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/__init__.py
--rw-r--r--   0        0        0   138485 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/_exporter_targets.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/colorgrids.py
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/not_test_cell.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test.json
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test.yaml
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_animations.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_auto.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_colors.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_dump_n_load.py
--rw-r--r--   0        0        0    16036 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_exporters.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_fancy_repr.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_helpers.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_highlight_markup_literal.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_layouts.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_parser.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_regex.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_styles.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 pytermgui-7.5.0/.gitignore
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pytermgui-7.5.0/LICENSE
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pyproject.toml
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pytermgui-7.5.0/PKG-INFO
+-rw-r--r--   0        0        0    10841 2020-02-02 00:00:00.000000 pytermgui-7.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     7429 2020-02-02 00:00:00.000000 pytermgui-7.6.0/README.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pytermgui-7.6.0/examples/README.md
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/__init__.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/animations.py
+-rw-r--r--   0        0        0    19743 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/ansi_interface.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/cell.py
+-rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/cmd.py
+-rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/color_info.py
+-rw-r--r--   0        0        0    26448 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/colors.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/context_managers.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/enums.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/exceptions.py
+-rw-r--r--   0        0        0    18846 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/exporters.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/fancy_repr.py
+-rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/file_loaders.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/helpers.py
+-rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/highlighters.py
+-rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/input.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/inspector.py
+-rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/palettes.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/prettifiers.py
+-rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/pretty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/py.typed
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/regex.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/serialization.py
+-rw-r--r--   0        0        0    16868 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/term.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/win32console.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/markup/__init__.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/markup/aliases.py
+-rw-r--r--   0        0        0    14551 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/markup/language.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/markup/macros.py
+-rw-r--r--   0        0        0    22738 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/markup/parsing.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/markup/style_maps.py
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/markup/tokens.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/__init__.py
+-rw-r--r--   0        0        0    25604 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/base.py
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/boxes.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/button.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/checkbox.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/collapsible.py
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/color_picker.py
+-rw-r--r--   0        0        0    33128 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/containers.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/fancy_repr.py
+-rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/frames.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/inline.py
+-rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/input_field.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/keyboard_button.py
+-rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/pixel_matrix.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/slider.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/styles.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/widgets/toggle.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/window_manager/__init__.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/window_manager/compositor.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/window_manager/layouts.py
+-rw-r--r--   0        0        0    19978 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/window_manager/manager.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pytermgui/window_manager/window.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/__init__.py
+-rw-r--r--   0        0        0   138485 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/_exporter_targets.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/colorgrids.py
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/not_test_cell.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test.json
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test.yaml
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_animations.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_auto.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_colors.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_dump_n_load.py
+-rw-r--r--   0        0        0    16036 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_exporters.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_fancy_repr.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_helpers.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_highlight_markup_literal.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_layouts.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_parser.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_regex.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pytermgui-7.6.0/tests/test_styles.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 pytermgui-7.6.0/.gitignore
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pytermgui-7.6.0/LICENSE
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 pytermgui-7.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 pytermgui-7.6.0/PKG-INFO
```

### Comparing `pytermgui-7.5.0/CHANGELOG.md` & `pytermgui-7.6.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## [7.6.0] - 2023-07-25
+
+### Bugfixes
+
+- (temporarily) Fix hyperlinks breaking SVG exports
+
+### Removals
+
+- Remove (undocumented) shortening behaviour from `Button`
+
+<!-- HATCH README END -->
+
 ## [7.5.0] - 2023-07-24
 
 ### Additions
 
 - Add support for Windows' mouse events
 - Add support for feeding input into `getch`
 
@@ -9,16 +21,14 @@
 
 - Allow immediately halting `WindowManager` programatically by not blocking on `getch` calls
 
 ### Bugfixes
 
 - Fix mouse event handlers not getting cleaned up properly
 
-<!-- HATCH README END -->
-
 ## [7.4.0] - 2023-05-24
 
 ### Additions
 
 - Add meta tokens for saving & restoring styles
 - Add support for alt/ctrl+backspace to remove whole words
 - Add support for word move actions (Ctrl/Alt+<L>/<R>) & Home/End move
@@ -369,14 +379,15 @@
 
 - Fix support for aliasing to an existing tag
 - Fix blocking `getch` call on Windows
 
 
 <!-- HATCH URI DEFINITIONS START -->
 
+[7.6.0]: https://github.com/bczsalba/pytermgui/compare/v7.5.0...v7.6.0
 [7.5.0]: https://github.com/bczsalba/pytermgui/compare/v7.4.0...v7.5.0
 [7.4.0]: https://github.com/bczsalba/pytermgui/compare/v7.3.0...v7.4.0
 [7.3.0]: https://github.com/bczsalba/pytermgui/compare/v7.2.0...v7.3.0
 [7.2.0]: https://github.com/bczsalba/pytermgui/compare/v7.1.0...v7.2.0
 [7.1.0]: https://github.com/bczsalba/pytermgui/compare/v7.0.0...v7.1.0
 [7.0.0]: https://github.com/bczsalba/pytermgui/compare/v6.4.0...v7.0.0
 [6.4.0]: https://github.com/bczsalba/pytermgui/compare/v6.0.0...v6.4.0
```

### Comparing `pytermgui-7.5.0/README.md` & `pytermgui-7.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/examples/README.md` & `pytermgui-7.6.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/__init__.py` & `pytermgui-7.6.0/pytermgui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 # Silence warning if running as standalone module
 if "-m" in sys.argv:  # pragma: no cover
     import warnings
 
     warnings.filterwarnings("ignore")
 
-__version__ = "7.5.0"
+__version__ = "7.6.0"
 
 
 def auto(data: Any, **widget_args: Any) -> Optional[Widget | list[Splitter]]:
     """Creates a widget from specific data structures.
 
     This conversion includes various widget classes, as well as some shorthands for
     more complex objects.  This method is called implicitly whenever a non-widget is
```

### Comparing `pytermgui-7.5.0/pytermgui/animations.py` & `pytermgui-7.6.0/pytermgui/animations.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/ansi_interface.py` & `pytermgui-7.6.0/pytermgui/ansi_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
 def restore_cursor() -> None:
     """Restore cursor position as saved by `save_cursor`."""
 
     get_terminal().write("\x1b[u")
 
 
-def report_cursor() -> Optional[tuple[int, int]]:
+def report_cursor() -> "Optional[tuple[int, int]]":
     """Gets position of cursor.
 
     Returns:
         A tuple of integers, (columns, rows), describing the
         current (printing) cursor's position. Returns None if
         this could not be determined.
```

### Comparing `pytermgui-7.5.0/pytermgui/cell.py` & `pytermgui-7.6.0/pytermgui/cell.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/cmd.py` & `pytermgui-7.6.0/pytermgui/cmd.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/color_info.py` & `pytermgui-7.6.0/pytermgui/color_info.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/colors.py` & `pytermgui-7.6.0/pytermgui/colors.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/context_managers.py` & `pytermgui-7.6.0/pytermgui/context_managers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/enums.py` & `pytermgui-7.6.0/pytermgui/enums.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/exceptions.py` & `pytermgui-7.6.0/pytermgui/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/exporters.py` & `pytermgui-7.6.0/pytermgui/exporters.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,14 +499,17 @@
     if isinstance(obj, Widget):
         obj = "\n".join(obj.get_lines())
 
     elif isinstance(obj, StyledText):
         obj = str(obj)
 
     for plain in tim.group_styles(obj):
+        if "\x1b" in plain.plain:
+            continue
+
         should_newline = False
 
         pos, back, styles = _handle_tokens_svg(plain, default_fore, default_back)
 
         index = _generate_index_in(document_styles, styles)
 
         if index == len(document_styles):
```

### Comparing `pytermgui-7.5.0/pytermgui/fancy_repr.py` & `pytermgui-7.6.0/pytermgui/fancy_repr.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/file_loaders.py` & `pytermgui-7.6.0/pytermgui/file_loaders.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/helpers.py` & `pytermgui-7.6.0/pytermgui/helpers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/highlighters.py` & `pytermgui-7.6.0/pytermgui/highlighters.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/input.py` & `pytermgui-7.6.0/pytermgui/input.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/inspector.py` & `pytermgui-7.6.0/pytermgui/inspector.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/palettes.py` & `pytermgui-7.6.0/pytermgui/palettes.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/prettifiers.py` & `pytermgui-7.6.0/pytermgui/prettifiers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/pretty.py` & `pytermgui-7.6.0/pytermgui/pretty.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/regex.py` & `pytermgui-7.6.0/pytermgui/regex.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/serialization.py` & `pytermgui-7.6.0/pytermgui/serialization.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/term.py` & `pytermgui-7.6.0/pytermgui/term.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/win32console.py` & `pytermgui-7.6.0/pytermgui/win32console.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/markup/aliases.py` & `pytermgui-7.6.0/pytermgui/markup/aliases.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/markup/language.py` & `pytermgui-7.6.0/pytermgui/markup/language.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/markup/macros.py` & `pytermgui-7.6.0/pytermgui/markup/macros.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/markup/parsing.py` & `pytermgui-7.6.0/pytermgui/markup/parsing.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/markup/style_maps.py` & `pytermgui-7.6.0/pytermgui/markup/style_maps.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/markup/tokens.py` & `pytermgui-7.6.0/pytermgui/markup/tokens.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/__init__.py` & `pytermgui-7.6.0/pytermgui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/base.py` & `pytermgui-7.6.0/pytermgui/widgets/base.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/boxes.py` & `pytermgui-7.6.0/pytermgui/widgets/boxes.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/button.py` & `pytermgui-7.6.0/pytermgui/widgets/button.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from __future__ import annotations
 
 from typing import Any, Callable, Optional
 
 from ..ansi_interface import MouseAction, MouseEvent
 from ..input import keys
-from ..regex import real_length
 from . import styles as w_styles
 from .base import Widget
 
 
 class Button(Widget):
     """A simple Widget representing a mouse-clickable button"""
 
@@ -90,25 +89,16 @@
         """Get object lines"""
 
         delimiters = self._get_char("delimiter")
         assert isinstance(delimiters, list) and len(delimiters) == 2
 
         left, right = delimiters
         left = left.replace("[", r"\[")
-        delim_len = real_length(left + right)
-
-        label = self.label
-        if len(self.label) > self.width:
-            sli = max(self.width - delim_len - 3 - self.padding, 0)
-            label = self.label[:sli] + "..."
-
-        elif self.centered:
-            label = self.label.center(self.width)
 
         if self.selected_index is None:
             style = self.styles["_current"]
         else:
             style = self.styles.highlight
 
-        line = style(left + label + right + self.padding * " ")
+        line = style(left + self.label + right + self.padding * " ")
 
         return [line]
```

### Comparing `pytermgui-7.5.0/pytermgui/widgets/checkbox.py` & `pytermgui-7.6.0/pytermgui/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/collapsible.py` & `pytermgui-7.6.0/pytermgui/widgets/collapsible.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/color_picker.py` & `pytermgui-7.6.0/pytermgui/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/containers.py` & `pytermgui-7.6.0/pytermgui/widgets/containers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/fancy_repr.py` & `pytermgui-7.6.0/pytermgui/widgets/fancy_repr.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/frames.py` & `pytermgui-7.6.0/pytermgui/widgets/frames.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/inline.py` & `pytermgui-7.6.0/pytermgui/widgets/inline.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/input_field.py` & `pytermgui-7.6.0/pytermgui/widgets/input_field.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/keyboard_button.py` & `pytermgui-7.6.0/pytermgui/widgets/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/pixel_matrix.py` & `pytermgui-7.6.0/pytermgui/widgets/pixel_matrix.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/slider.py` & `pytermgui-7.6.0/pytermgui/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/styles.py` & `pytermgui-7.6.0/pytermgui/widgets/styles.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/widgets/toggle.py` & `pytermgui-7.6.0/pytermgui/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/window_manager/__init__.py` & `pytermgui-7.6.0/pytermgui/window_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/window_manager/compositor.py` & `pytermgui-7.6.0/pytermgui/window_manager/compositor.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/window_manager/layouts.py` & `pytermgui-7.6.0/pytermgui/window_manager/layouts.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/window_manager/manager.py` & `pytermgui-7.6.0/pytermgui/window_manager/manager.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pytermgui/window_manager/window.py` & `pytermgui-7.6.0/pytermgui/window_manager/window.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/_exporter_targets.py` & `pytermgui-7.6.0/tests/_exporter_targets.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/colorgrids.py` & `pytermgui-7.6.0/tests/colorgrids.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/not_test_cell.py` & `pytermgui-7.6.0/tests/not_test_cell.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test.json` & `pytermgui-7.6.0/tests/test.json`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test.yaml` & `pytermgui-7.6.0/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test_animations.py` & `pytermgui-7.6.0/tests/test_animations.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test_auto.py` & `pytermgui-7.6.0/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test_colors.py` & `pytermgui-7.6.0/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test_dump_n_load.py` & `pytermgui-7.6.0/tests/test_dump_n_load.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test_exporters.py` & `pytermgui-7.6.0/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test_fancy_repr.py` & `pytermgui-7.6.0/tests/test_fancy_repr.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test_helpers.py` & `pytermgui-7.6.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test_layouts.py` & `pytermgui-7.6.0/tests/test_layouts.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test_parser.py` & `pytermgui-7.6.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test_regex.py` & `pytermgui-7.6.0/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/tests/test_styles.py` & `pytermgui-7.6.0/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/.gitignore` & `pytermgui-7.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/LICENSE` & `pytermgui-7.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/pyproject.toml` & `pytermgui-7.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytermgui-7.5.0/PKG-INFO` & `pytermgui-7.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTermGUI
-Version: 7.5.0
+Version: 7.6.0
 Summary: Python TUI framework with mouse support, modular widget system, customizable and rapid terminal markup language and more!
 Project-URL: homepage, https://github.com/bczsalba/PyTermGUI
 Project-URL: repository, https://github.com/bczsalba/PyTermGUI
 Project-URL: documentation, https://ptg.bczsalba.com
 Author-email: Balázs Cene <bczsalba@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -97,34 +97,30 @@
 
 - An inspection utility
 - A pretty printer for both the REPL and IPython
 - A way to create SVG and HTML screenshots of your terminal
 
 ## Latest release
 
-### [7.5.0] - 2023-07-24
+### [7.6.0] - 2023-07-25
 
-### Additions
-
-- Add support for Windows' mouse events
-- Add support for feeding input into `getch`
-
-### Refactor
+### Bugfixes
 
-- Allow immediately halting `WindowManager` programatically by not blocking on `getch` calls
+- (temporarily) Fix hyperlinks breaking SVG exports
 
-### Bugfixes
+### Removals
 
-- Fix mouse event handlers not getting cleaned up properly
+- Remove (undocumented) shortening behaviour from `Button`
 
 
 Read the full changelog [here](https://github.com/bczsalba/pytermgui/blob/master/CHANGELOG.md).
 
 
 
+[7.6.0]: https://github.com/bczsalba/pytermgui/compare/v7.5.0...v7.6.0
 [7.5.0]: https://github.com/bczsalba/pytermgui/compare/v7.4.0...v7.5.0
 [7.4.0]: https://github.com/bczsalba/pytermgui/compare/v7.3.0...v7.4.0
 [7.3.0]: https://github.com/bczsalba/pytermgui/compare/v7.2.0...v7.3.0
 [7.2.0]: https://github.com/bczsalba/pytermgui/compare/v7.1.0...v7.2.0
 [7.1.0]: https://github.com/bczsalba/pytermgui/compare/v7.0.0...v7.1.0
 [7.0.0]: https://github.com/bczsalba/pytermgui/compare/v6.4.0...v7.0.0
 [6.4.0]: https://github.com/bczsalba/pytermgui/compare/v6.0.0...v6.4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyTermGUI Version: 7.5.0 Summary: Python TUI
+Metadata-Version: 2.1 Name: PyTermGUI Version: 7.6.0 Summary: Python TUI
 framework with mouse support, modular widget system, customizable and rapid
 terminal markup language and more! Project-URL: homepage, https://github.com/
 bczsalba/PyTermGUI Project-URL: repository, https://github.com/bczsalba/
 PyTermGUI Project-URL: documentation, https://ptg.bczsalba.com Author-email:
 BalÃ¡zs Cene
 gmail.com> License: MIT License-File: LICENSE Keywords:
 ANSI,TUI,UI,framework,markup,terminal,user-interface,xterm Classifier:
@@ -36,21 +36,20 @@
 window manager system with modals and completely customizable windows - Mouse
 support out of the box with **0** configuration - YAML (or Python) based
 styling engines - TIM, our markup language for creating styled terminal text
 with expressive text, including systems for aliases & macros - A bunch of
 things I can't think of right now :slightly_smiling_face: Additionally, there
 are a couple of neat tools to make your general Python development easier: - An
 inspection utility - A pretty printer for both the REPL and IPython - A way to
-create SVG and HTML screenshots of your terminal ## Latest release ### [7.5.0]
-- 2023-07-24 ### Additions - Add support for Windows' mouse events - Add
-support for feeding input into `getch` ### Refactor - Allow immediately halting
-`WindowManager` programatically by not blocking on `getch` calls ### Bugfixes -
-Fix mouse event handlers not getting cleaned up properly Read the full
-changelog [here](https://github.com/bczsalba/pytermgui/blob/master/
-CHANGELOG.md). [7.5.0]: https://github.com/bczsalba/pytermgui/compare/
+create SVG and HTML screenshots of your terminal ## Latest release ### [7.6.0]
+- 2023-07-25 ### Bugfixes - (temporarily) Fix hyperlinks breaking SVG exports
+### Removals - Remove (undocumented) shortening behaviour from `Button` Read
+the full changelog [here](https://github.com/bczsalba/pytermgui/blob/master/
+CHANGELOG.md). [7.6.0]: https://github.com/bczsalba/pytermgui/compare/
+v7.5.0...v7.6.0 [7.5.0]: https://github.com/bczsalba/pytermgui/compare/
 v7.4.0...v7.5.0 [7.4.0]: https://github.com/bczsalba/pytermgui/compare/
 v7.3.0...v7.4.0 [7.3.0]: https://github.com/bczsalba/pytermgui/compare/
 v7.2.0...v7.3.0 [7.2.0]: https://github.com/bczsalba/pytermgui/compare/
 v7.1.0...v7.2.0 [7.1.0]: https://github.com/bczsalba/pytermgui/compare/
 v7.0.0...v7.1.0 [7.0.0]: https://github.com/bczsalba/pytermgui/compare/
 v6.4.0...v7.0.0 [6.4.0]: https://github.com/bczsalba/pytermgui/compare/
 v6.0.0...v6.4.0 [6.3.0]: https://github.com/bczsalba/pytermgui/compare/
```

