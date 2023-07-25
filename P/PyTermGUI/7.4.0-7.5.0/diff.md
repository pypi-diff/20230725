# Comparing `tmp/pytermgui-7.4.0.tar.gz` & `tmp/pytermgui-7.5.0.tar.gz`

## Comparing `pytermgui-7.4.0.tar` & `pytermgui-7.5.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 pytermgui-7.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     7429 2020-02-02 00:00:00.000000 pytermgui-7.4.0/README.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pytermgui-7.4.0/examples/README.md
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/__init__.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/animations.py
--rw-r--r--   0        0        0    19812 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/ansi_interface.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/cell.py
--rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/cmd.py
--rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/color_info.py
--rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/colors.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/context_managers.py
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/enums.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/exceptions.py
--rw-r--r--   0        0        0    18790 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/exporters.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/fancy_repr.py
--rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/file_loaders.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/helpers.py
--rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/highlighters.py
--rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/input.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/inspector.py
--rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/palettes.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/prettifiers.py
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/pretty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/py.typed
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/regex.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/serialization.py
--rw-r--r--   0        0        0    16868 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/term.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/aliases.py
--rw-r--r--   0        0        0    14551 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/language.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/macros.py
--rw-r--r--   0        0        0    22738 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/parsing.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/style_maps.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/tokens.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/__init__.py
--rw-r--r--   0        0        0    25604 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/base.py
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/boxes.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/button.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/checkbox.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/collapsible.py
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/color_picker.py
--rw-r--r--   0        0        0    33128 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/containers.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/fancy_repr.py
--rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/frames.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/inline.py
--rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/input_field.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/keyboard_button.py
--rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/pixel_matrix.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/slider.py
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/styles.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/toggle.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/window_manager/__init__.py
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/window_manager/compositor.py
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/window_manager/layouts.py
--rw-r--r--   0        0        0    19429 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/window_manager/manager.py
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/window_manager/window.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/__init__.py
--rw-r--r--   0        0        0   138485 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/_exporter_targets.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/colorgrids.py
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/not_test_cell.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test.json
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test.yaml
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_animations.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_auto.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_colors.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_dump_n_load.py
--rw-r--r--   0        0        0    16036 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_exporters.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_fancy_repr.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_helpers.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_highlight_markup_literal.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_layouts.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_parser.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_regex.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_styles.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 pytermgui-7.4.0/.gitignore
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pytermgui-7.4.0/LICENSE
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pyproject.toml
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 pytermgui-7.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10604 2020-02-02 00:00:00.000000 pytermgui-7.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     7429 2020-02-02 00:00:00.000000 pytermgui-7.5.0/README.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pytermgui-7.5.0/examples/README.md
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/__init__.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/animations.py
+-rw-r--r--   0        0        0    19741 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/ansi_interface.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/cell.py
+-rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/cmd.py
+-rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/color_info.py
+-rw-r--r--   0        0        0    26448 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/colors.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/context_managers.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/enums.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/exceptions.py
+-rw-r--r--   0        0        0    18790 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/exporters.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/fancy_repr.py
+-rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/file_loaders.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/helpers.py
+-rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/highlighters.py
+-rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/input.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/inspector.py
+-rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/palettes.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/prettifiers.py
+-rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/pretty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/py.typed
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/regex.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/serialization.py
+-rw-r--r--   0        0        0    16868 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/term.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/win32console.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/__init__.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/aliases.py
+-rw-r--r--   0        0        0    14551 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/language.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/macros.py
+-rw-r--r--   0        0        0    22738 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/parsing.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/style_maps.py
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/markup/tokens.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/__init__.py
+-rw-r--r--   0        0        0    25604 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/base.py
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/boxes.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/button.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/checkbox.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/collapsible.py
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/color_picker.py
+-rw-r--r--   0        0        0    33128 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/containers.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/fancy_repr.py
+-rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/frames.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/inline.py
+-rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/input_field.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/keyboard_button.py
+-rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/pixel_matrix.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/slider.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/styles.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/widgets/toggle.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/window_manager/__init__.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/window_manager/compositor.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/window_manager/layouts.py
+-rw-r--r--   0        0        0    19978 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/window_manager/manager.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pytermgui/window_manager/window.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/__init__.py
+-rw-r--r--   0        0        0   138485 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/_exporter_targets.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/colorgrids.py
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/not_test_cell.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test.json
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test.yaml
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_animations.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_auto.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_colors.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_dump_n_load.py
+-rw-r--r--   0        0        0    16036 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_exporters.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_fancy_repr.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_helpers.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_highlight_markup_literal.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_layouts.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_parser.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_regex.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pytermgui-7.5.0/tests/test_styles.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 pytermgui-7.5.0/.gitignore
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pytermgui-7.5.0/LICENSE
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 pytermgui-7.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pytermgui-7.5.0/PKG-INFO
```

### Comparing `pytermgui-7.4.0/CHANGELOG.md` & `pytermgui-7.5.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+## [7.5.0] - 2023-07-24
+
+### Additions
+
+- Add support for Windows' mouse events
+- Add support for feeding input into `getch`
+
+### Refactor
+
+- Allow immediately halting `WindowManager` programatically by not blocking on `getch` calls
+
+### Bugfixes
+
+- Fix mouse event handlers not getting cleaned up properly
+
+<!-- HATCH README END -->
+
+## [7.4.0] - 2023-05-24
+
+### Additions
+
+- Add meta tokens for saving & restoring styles
+- Add support for alt/ctrl+backspace to remove whole words
+- Add support for word move actions (Ctrl/Alt+<L>/<R>) & Home/End move
+
+### Bugfixes
+
+- Fix multiline Label widget to incorrectly display message with hyperlink
+- Fix input errors when alert is open (@qoft, #115)
+
 ## [7.3.0] - 2022-11-17
 
 ### Additions
 
 - Add support for `SHIFT+` scroll events
 - Add shade number indicators to `Palette.print`
 - Add `inline` widget runner
@@ -19,16 +49,14 @@
 - Improve pseudo token behaviour by parsing it as a new token type
 - Start generating semantic colors (success, warning, error) by blending with the primary
 
 ### Removals
 
 - Remove `is_bindable` widget attribute
 
-<!-- HATCH README END -->
-
 ## [7.2.0] - 2022-08-05
 
 ### Additions
 
 - Add various color manipulation utilities
 - Add `#auto` TIM pseudo-tag that always gives properly contrasted foreground text
 - Add `palettes` module for framework-wide color generation & configuration
@@ -341,14 +369,16 @@
 
 - Fix support for aliasing to an existing tag
 - Fix blocking `getch` call on Windows
 
 
 <!-- HATCH URI DEFINITIONS START -->
 
+[7.5.0]: https://github.com/bczsalba/pytermgui/compare/v7.4.0...v7.5.0
+[7.4.0]: https://github.com/bczsalba/pytermgui/compare/v7.3.0...v7.4.0
 [7.3.0]: https://github.com/bczsalba/pytermgui/compare/v7.2.0...v7.3.0
 [7.2.0]: https://github.com/bczsalba/pytermgui/compare/v7.1.0...v7.2.0
 [7.1.0]: https://github.com/bczsalba/pytermgui/compare/v7.0.0...v7.1.0
 [7.0.0]: https://github.com/bczsalba/pytermgui/compare/v6.4.0...v7.0.0
 [6.4.0]: https://github.com/bczsalba/pytermgui/compare/v6.0.0...v6.4.0
 [6.3.0]: https://github.com/bczsalba/pytermgui/compare/v6.2.2...v6.3.0
 [6.2.2]: https://github.com/bczsalba/pytermgui/compare/v6.2.1...v6.2.2
```

### Comparing `pytermgui-7.4.0/README.md` & `pytermgui-7.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/examples/README.md` & `pytermgui-7.5.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/__init__.py` & `pytermgui-7.5.0/pytermgui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .enums import *
 from .exceptions import *
 from .exporters import *
 from .fancy_repr import *
 from .file_loaders import *
 from .helpers import *
 from .highlighters import *
-from .input import getch, keys
+from .input import *
 from .inspector import *
 from .markup import *
 from .palettes import *
 from .prettifiers import *
 from .regex import *
 from .serialization import *
 from .term import *
@@ -36,15 +36,15 @@
 
 # Silence warning if running as standalone module
 if "-m" in sys.argv:  # pragma: no cover
     import warnings
 
     warnings.filterwarnings("ignore")
 
-__version__ = "7.4.0"
+__version__ = "7.5.0"
 
 
 def auto(data: Any, **widget_args: Any) -> Optional[Widget | list[Splitter]]:
     """Creates a widget from specific data structures.
 
     This conversion includes various widget classes, as well as some shorthands for
     more complex objects.  This method is called implicitly whenever a non-widget is
```

### Comparing `pytermgui-7.4.0/pytermgui/animations.py` & `pytermgui-7.5.0/pytermgui/animations.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/ansi_interface.py` & `pytermgui-7.5.0/pytermgui/ansi_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,59 +489,60 @@
         events, gives a translator method and handles exceptions.
 
     Possible events:
         - **press**: Report when the mouse is clicked, left or right button.
         - **highlight**: Report highlighting.
         - **press_hold**: Report with a left or right click, as well as both
             left & right drag and release.
-        - **hover**: Report even when no active action is done, only the mouse
-          is moved.
+        - **all**: Report every event, even hover.
 
     Methods:
         - **None**: Non-decimal xterm method. Limited in coordinates.
         - **decimal_xterm**: The default setting. Most universally supported.
         - **decimal_urxvt**: Older, less compatible, but useful on some systems.
         - **decimal_utf8**:  Apparently not too stable.
 
     More information <a href='https://stackoverflow.com/a/5970472'>here</a>.
     """
 
+    terminal = get_terminal()
+
     if event == "press":
-        get_terminal().write("\x1b[?1000")
+        terminal.write("\x1b[?1000")
 
     elif event == "highlight":
-        get_terminal().write("\x1b[?1001")
+        terminal.write("\x1b[?1001")
 
     elif event == "press_hold":
-        get_terminal().write("\x1b[?1002")
+        terminal.write("\x1b[?1002")
 
-    elif event == "hover":
-        get_terminal().write("\x1b[?1003")
+    elif event == "all":
+        terminal.write("\x1b[?1003")
 
     else:
-        raise NotImplementedError(f"Mouse report event {event} is not supported!")
+        raise NotImplementedError(f"Mouse report event {event!r} is not supported!")
 
-    get_terminal().write("l" if stop else "h")
+    terminal.write("l" if stop else "h")
 
     if method == "decimal_utf8":
-        get_terminal().write("\x1b[?1005")
+        terminal.write("\x1b[?1005")
 
     elif method == "decimal_xterm":
-        get_terminal().write("\x1b[?1006")
+        terminal.write("\x1b[?1006")
 
     elif method == "decimal_urxvt":
-        get_terminal().write("\x1b[?1015")
+        terminal.write("\x1b[?1015")
 
     elif method is None:
         return
 
     else:
         raise NotImplementedError(f"Mouse report method {method} is not supported!")
 
-    get_terminal().write("l" if stop else "h", flush=True)
+    terminal.write("l" if stop else "h", flush=True)
 
 
 def translate_mouse(code: str, method: str) -> list[MouseEvent | None] | None:
     """Translates the output of produced by setting `report_mouse` into MouseEvents.
 
     This method currently only supports `decimal_xterm` and `decimal_urxvt`.
```

### Comparing `pytermgui-7.4.0/pytermgui/cell.py` & `pytermgui-7.5.0/pytermgui/cell.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/cmd.py` & `pytermgui-7.5.0/pytermgui/cmd.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/color_info.py` & `pytermgui-7.5.0/pytermgui/color_info.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/colors.py` & `pytermgui-7.5.0/pytermgui/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -827,17 +827,17 @@
     redmean = (red1 + red2) // 2
 
     delta_red = red1 - red2
     delta_green = green1 - green2
     delta_blue = blue1 - blue2
 
     return sqrt(
-        (2 + (redmean / 256)) * (delta_red ** 2)
-        + 4 * (delta_green ** 2)
-        + (2 + (255 - redmean) / 256) * (delta_blue ** 2)
+        (2 + (redmean / 256)) * (delta_red**2)
+        + 4 * (delta_green**2)
+        + (2 + (255 - redmean) / 256) * (delta_blue**2)
     )
 
 
 @lru_cache(maxsize=1024)
 def str_to_color(
     text: str,
     is_background: bool = False,
```

### Comparing `pytermgui-7.4.0/pytermgui/context_managers.py` & `pytermgui-7.5.0/pytermgui/context_managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,18 +133,16 @@
     'pytermgui.ansi_interface.MouseEvent'
     'pytermgui.ansi_interface.MouseAction.LEFT_CLICK'
     (33, 55)
     ```
 
     """
 
-    event = None
     try:
         for event in events:
             report_mouse(event, method=method)
 
         yield lambda code: translate_mouse(code, method=method)
 
     finally:
-        input(event)
-        if event is not None:
+        for event in events:
             report_mouse(event, method=method, stop=True)
```

### Comparing `pytermgui-7.4.0/pytermgui/enums.py` & `pytermgui-7.5.0/pytermgui/enums.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/exceptions.py` & `pytermgui-7.5.0/pytermgui/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/exporters.py` & `pytermgui-7.5.0/pytermgui/exporters.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/fancy_repr.py` & `pytermgui-7.5.0/pytermgui/fancy_repr.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/file_loaders.py` & `pytermgui-7.5.0/pytermgui/file_loaders.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/helpers.py` & `pytermgui-7.5.0/pytermgui/helpers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/highlighters.py` & `pytermgui-7.5.0/pytermgui/highlighters.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/input.py` & `pytermgui-7.5.0/pytermgui/input.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # pylint: disable=c-extension-no-member, no-name-in-module, used-before-assignment
 
 from __future__ import annotations
 
 import os
 import signal
 import sys
+from io import StringIO
 from codecs import getincrementaldecoder
 from contextlib import contextmanager
 from select import select
 from typing import (
     IO,
     Any,
     AnyStr,
@@ -32,15 +33,17 @@
     Optional,
     Union,
     ValuesView,
 )
 
 from .exceptions import TimeoutException
 
-__all__ = ["Keys", "getch", "getch_timeout", "keys"]
+__all__ = ["Keys", "getch", "getch_timeout", "keys", "feed"]
+
+feeder_stream = StringIO()
 
 
 @contextmanager
 def timeout(duration: float) -> Generator[None, None, None]:
     """Allows context to run for a certain amount of time, quits it once it's up.
 
     Note that this should never be run on Windows, as the required signals are not
@@ -75,14 +78,25 @@
         content.
     """
 
     result = select([file], [], [], 0.0)
     return len(result[0]) > 0
 
 
+def feed(text: str) -> None:
+    """Manually feeds some text to be read by `getch`.
+
+    This can be used to emulate input, as well as to "interrupt" a blocking `getch`
+    call (though `getch_timeout` works better for that scenario).
+    """
+
+    feeder_stream.write(text)
+    feeder_stream.seek(0)
+
+
 class _GetchUnix:
     """Getch implementation for UNIX systems."""
 
     def __init__(self) -> None:
         """Initializes object."""
 
         if sys.stdin.encoding is not None:
@@ -163,18 +177,16 @@
 
         Returns:
             All read characters.
         """
 
         # We need to type: ignore these on non-windows machines,
         # as the library does not exist.
-
-        # Return empty string if there is no input to get
         if not msvcrt.kbhit():  # type: ignore
-            return ""
+            raise TimeoutException("No input available.")
 
         char = msvcrt.getch()  # type: ignore
         if char == b"\xe0":
             char = "\x1b"
 
         buff = self._ensure_str(char)
 
@@ -395,23 +407,36 @@
         "F12": "\x1b[24~",
     }
 
     _getch = _GetchUnix()
     keys = Keys(_platform_keys, "posix")
 
 
-def getch(printable: bool = False, interrupts: bool = True) -> Any:
+def getch(
+    printable: bool = False,
+    interrupts: bool = True,
+    windows_raise_timeout: bool = False,
+) -> str:
     """Wrapper to call the platform-appropriate character getter.
 
     Args:
         printable: When set, printable versions of the input are returned.
-        interrupts: If not set, `KeyboardInterrupt` is silenced and `chr(3)`
-            (`CTRL_C`) is returned.
+        interrupts: If not set, `KeyboardInterrupt` is silenced and `chr(3)` (`CTRL_C`)
+            is returned.
+        windows_raise_timeout: If set, `TimeoutException` (raised by Windows' getch when
+            no input is available) isn't silenced.
     """
 
+    fed_text = feeder_stream.getvalue()
+
+    if fed_text != "":
+        feeder_stream.seek(0)
+        feeder_stream.truncate(0)
+        return fed_text
+
     try:
         key = _getch()
 
         # msvcrt.getch returns CTRL_C as a character, unlike UNIX systems
         # where an interrupt is raised. Thus, we need to manually raise
         # the interrupt.
         if key == chr(3):
@@ -419,32 +444,44 @@
 
     except KeyboardInterrupt as error:
         if interrupts:
             raise KeyboardInterrupt("Unhandled interrupt") from error
 
         key = chr(3)
 
+    except TimeoutException:
+        if windows_raise_timeout:
+            raise
+
+        key = ""
+
     if printable:
         key = key.encode("unicode_escape").decode("utf-8")
 
     return key
 
 
 def getch_timeout(
     duration: float, default: str = "", printable: bool = False, interrupts: bool = True
 ) -> Any:
     """Calls `getch`, returns `default` if timeout passes before getting input.
 
-    No timeout is applied on Windows systems, as there is no support for `SIGALRM`.
+    No timeout is applied on Windows systems, as there is no support for
+    `SIGALRM`. Instead, it will return immediately if no input is provided, since the
+    Windows APIs expose a way to detect that case.
 
     Args:
         duration: How long the call should wait for input.
         default: The value to return if timeout occured.
     """
 
     if isinstance(_getch, _GetchWindows):
-        return getch()
+        try:
+            return getch(windows_raise_timeout=True)
+
+        except TimeoutException:
+            return default
 
     with timeout(duration):
         return getch(printable=printable, interrupts=interrupts)
 
     return default
```

### Comparing `pytermgui-7.4.0/pytermgui/inspector.py` & `pytermgui-7.5.0/pytermgui/inspector.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/palettes.py` & `pytermgui-7.5.0/pytermgui/palettes.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/prettifiers.py` & `pytermgui-7.5.0/pytermgui/prettifiers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/pretty.py` & `pytermgui-7.5.0/pytermgui/pretty.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/regex.py` & `pytermgui-7.5.0/pytermgui/regex.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/serialization.py` & `pytermgui-7.5.0/pytermgui/serialization.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/term.py` & `pytermgui-7.5.0/pytermgui/term.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/markup/aliases.py` & `pytermgui-7.5.0/pytermgui/markup/aliases.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/markup/language.py` & `pytermgui-7.5.0/pytermgui/markup/language.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/markup/macros.py` & `pytermgui-7.5.0/pytermgui/markup/macros.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/markup/parsing.py` & `pytermgui-7.5.0/pytermgui/markup/parsing.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/markup/style_maps.py` & `pytermgui-7.5.0/pytermgui/markup/style_maps.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/markup/tokens.py` & `pytermgui-7.5.0/pytermgui/markup/tokens.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/__init__.py` & `pytermgui-7.5.0/pytermgui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/base.py` & `pytermgui-7.5.0/pytermgui/widgets/base.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/boxes.py` & `pytermgui-7.5.0/pytermgui/widgets/boxes.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/button.py` & `pytermgui-7.5.0/pytermgui/widgets/button.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/checkbox.py` & `pytermgui-7.5.0/pytermgui/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/collapsible.py` & `pytermgui-7.5.0/pytermgui/widgets/collapsible.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/color_picker.py` & `pytermgui-7.5.0/pytermgui/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/containers.py` & `pytermgui-7.5.0/pytermgui/widgets/containers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/fancy_repr.py` & `pytermgui-7.5.0/pytermgui/widgets/fancy_repr.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/frames.py` & `pytermgui-7.5.0/pytermgui/widgets/frames.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/inline.py` & `pytermgui-7.5.0/pytermgui/widgets/inline.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/input_field.py` & `pytermgui-7.5.0/pytermgui/widgets/input_field.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/keyboard_button.py` & `pytermgui-7.5.0/pytermgui/widgets/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/pixel_matrix.py` & `pytermgui-7.5.0/pytermgui/widgets/pixel_matrix.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/slider.py` & `pytermgui-7.5.0/pytermgui/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/styles.py` & `pytermgui-7.5.0/pytermgui/widgets/styles.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/widgets/toggle.py` & `pytermgui-7.5.0/pytermgui/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/window_manager/__init__.py` & `pytermgui-7.5.0/pytermgui/window_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/window_manager/compositor.py` & `pytermgui-7.5.0/pytermgui/window_manager/compositor.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/window_manager/layouts.py` & `pytermgui-7.5.0/pytermgui/window_manager/layouts.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pytermgui/window_manager/manager.py` & `pytermgui-7.5.0/pytermgui/window_manager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 from typing import Any, Iterator, Type
 
 from ..animations import Animation, AttrAnimation, FloatAnimation, animator
 from ..ansi_interface import MouseAction, MouseEvent
 from ..colors import str_to_color
 from ..context_managers import MouseTranslator, alt_buffer, mouse_handler
 from ..enums import Overflow
-from ..input import getch
+from ..input import getch, getch_timeout
 from ..regex import real_length
 from ..term import terminal
 from ..widgets import Container, Widget
 from ..widgets.base import BoundCallback
+from ..win32console import enable_virtual_processing
 from .compositor import Compositor
 from .layouts import Layout
 from .window import Window
 
 
 def _center_during_animation(animation: AttrAnimation) -> None:
     """Centers a window, when applicable, while animating."""
@@ -111,39 +112,45 @@
     def __exit__(self, _: Any, exception: Exception, __: Any) -> bool:
         """Ends context manager."""
 
         # Run the manager if it hasnt been run before.
         if self.autorun and exception is None and self.mouse_translator is None:
             self.run()
 
-        self.stop()
-
         if exception is not None:
+            self.stop()
             raise exception
 
         return True
 
     def __iter__(self) -> Iterator[Window]:
         """Iterates this manager's windows."""
 
         return iter(self._windows)
 
     def _run_input_loop(self) -> None:
         """The main input loop of the WindowManager."""
 
-        while self._is_running:
-            key = getch(interrupts=False)
-
-            if key == chr(3):
-                break
+        with enable_virtual_processing():
+            while self._is_running:
+                # This stops us from blocking during input:
+                #   On POSIX it only reads from 0.01s before returning the empty string
+                #   On Windows it doesn't do a timeout, but since the Windows' getch
+                #     setup immediately returns when no input is available something
+                #     similar ends up happening as well.
+                key = getch_timeout(1 / 100, interrupts=False)
+
+                if key == chr(3):
+                    self.stop()
+                    break
 
-            if self.handle_key(key):
-                continue
+                if self.handle_key(key):
+                    continue
 
-            self.process_mouse(key)
+                self.process_mouse(key)
 
     def get_lines(self) -> list[str]:
         """Gets the empty list."""
 
         # TODO: Allow using WindowManager as a widget.
 
         return []
@@ -182,15 +189,15 @@
         Returns:
             The WindowManager's compositor instance.
         """
 
         self._is_running = True
 
         if mouse_events is None:
-            mouse_events = ["press_hold", "hover"]
+            mouse_events = ["all"]
 
         with alt_buffer(cursor=False, echo=False):
             with mouse_handler(mouse_events, "decimal_xterm") as translate:
                 self.mouse_translator = translate
                 self.compositor.run()
 
                 self._run_input_loop()
```

### Comparing `pytermgui-7.4.0/pytermgui/window_manager/window.py` & `pytermgui-7.5.0/pytermgui/window_manager/window.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/_exporter_targets.py` & `pytermgui-7.5.0/tests/_exporter_targets.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/colorgrids.py` & `pytermgui-7.5.0/tests/colorgrids.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/not_test_cell.py` & `pytermgui-7.5.0/tests/not_test_cell.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test.json` & `pytermgui-7.5.0/tests/test.json`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test.yaml` & `pytermgui-7.5.0/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test_animations.py` & `pytermgui-7.5.0/tests/test_animations.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test_auto.py` & `pytermgui-7.5.0/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test_colors.py` & `pytermgui-7.5.0/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test_dump_n_load.py` & `pytermgui-7.5.0/tests/test_dump_n_load.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test_exporters.py` & `pytermgui-7.5.0/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test_fancy_repr.py` & `pytermgui-7.5.0/tests/test_fancy_repr.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test_helpers.py` & `pytermgui-7.5.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test_layouts.py` & `pytermgui-7.5.0/tests/test_layouts.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test_parser.py` & `pytermgui-7.5.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test_regex.py` & `pytermgui-7.5.0/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/tests/test_styles.py` & `pytermgui-7.5.0/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/.gitignore` & `pytermgui-7.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/LICENSE` & `pytermgui-7.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/pyproject.toml` & `pytermgui-7.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytermgui-7.4.0/PKG-INFO` & `pytermgui-7.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTermGUI
-Version: 7.4.0
+Version: 7.5.0
 Summary: Python TUI framework with mouse support, modular widget system, customizable and rapid terminal markup language and more!
 Project-URL: homepage, https://github.com/bczsalba/PyTermGUI
 Project-URL: repository, https://github.com/bczsalba/PyTermGUI
 Project-URL: documentation, https://ptg.bczsalba.com
 Author-email: Balázs Cene <bczsalba@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -97,44 +97,36 @@
 
 - An inspection utility
 - A pretty printer for both the REPL and IPython
 - A way to create SVG and HTML screenshots of your terminal
 
 ## Latest release
 
-### [7.3.0] - 2022-11-17
+### [7.5.0] - 2023-07-24
 
 ### Additions
 
-- Add support for `SHIFT+` scroll events
-- Add shade number indicators to `Palette.print`
-- Add `inline` widget runner
+- Add support for Windows' mouse events
+- Add support for feeding input into `getch`
 
-### Bugfixes
-
-- Fix incorrect macro caching behaviour
-- Fix various issues and misbehaviours with SVG exports
-- Fix incorrect placement of `InputField` cursor
+### Refactor
 
-### Refactors
+- Allow immediately halting `WindowManager` programatically by not blocking on `getch` calls
 
-- New `MkDocs` based documentation
-- Change `terminal.py` -> `term.py` and `serializer.py` -> `serialization.py` to avoid naming conflicts
-- Improve pseudo token behaviour by parsing it as a new token type
-- Start generating semantic colors (success, warning, error) by blending with the primary
-
-### Removals
+### Bugfixes
 
-- Remove `is_bindable` widget attribute
+- Fix mouse event handlers not getting cleaned up properly
 
 
 Read the full changelog [here](https://github.com/bczsalba/pytermgui/blob/master/CHANGELOG.md).
 
 
 
+[7.5.0]: https://github.com/bczsalba/pytermgui/compare/v7.4.0...v7.5.0
+[7.4.0]: https://github.com/bczsalba/pytermgui/compare/v7.3.0...v7.4.0
 [7.3.0]: https://github.com/bczsalba/pytermgui/compare/v7.2.0...v7.3.0
 [7.2.0]: https://github.com/bczsalba/pytermgui/compare/v7.1.0...v7.2.0
 [7.1.0]: https://github.com/bczsalba/pytermgui/compare/v7.0.0...v7.1.0
 [7.0.0]: https://github.com/bczsalba/pytermgui/compare/v6.4.0...v7.0.0
 [6.4.0]: https://github.com/bczsalba/pytermgui/compare/v6.0.0...v6.4.0
 [6.3.0]: https://github.com/bczsalba/pytermgui/compare/v6.2.2...v6.3.0
 [6.2.2]: https://github.com/bczsalba/pytermgui/compare/v6.2.1...v6.2.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyTermGUI Version: 7.4.0 Summary: Python TUI
+Metadata-Version: 2.1 Name: PyTermGUI Version: 7.5.0 Summary: Python TUI
 framework with mouse support, modular widget system, customizable and rapid
 terminal markup language and more! Project-URL: homepage, https://github.com/
 bczsalba/PyTermGUI Project-URL: repository, https://github.com/bczsalba/
 PyTermGUI Project-URL: documentation, https://ptg.bczsalba.com Author-email:
 BalÃ¡zs Cene
 gmail.com> License: MIT License-File: LICENSE Keywords:
 ANSI,TUI,UI,framework,markup,terminal,user-interface,xterm Classifier:
@@ -36,38 +36,36 @@
 window manager system with modals and completely customizable windows - Mouse
 support out of the box with **0** configuration - YAML (or Python) based
 styling engines - TIM, our markup language for creating styled terminal text
 with expressive text, including systems for aliases & macros - A bunch of
 things I can't think of right now :slightly_smiling_face: Additionally, there
 are a couple of neat tools to make your general Python development easier: - An
 inspection utility - A pretty printer for both the REPL and IPython - A way to
-create SVG and HTML screenshots of your terminal ## Latest release ### [7.3.0]
-- 2022-11-17 ### Additions - Add support for `SHIFT+` scroll events - Add shade
-number indicators to `Palette.print` - Add `inline` widget runner ### Bugfixes
-- Fix incorrect macro caching behaviour - Fix various issues and misbehaviours
-with SVG exports - Fix incorrect placement of `InputField` cursor ### Refactors
-- New `MkDocs` based documentation - Change `terminal.py` -> `term.py` and
-`serializer.py` -> `serialization.py` to avoid naming conflicts - Improve
-pseudo token behaviour by parsing it as a new token type - Start generating
-semantic colors (success, warning, error) by blending with the primary ###
-Removals - Remove `is_bindable` widget attribute Read the full changelog [here]
-(https://github.com/bczsalba/pytermgui/blob/master/CHANGELOG.md). [7.3.0]:
-https://github.com/bczsalba/pytermgui/compare/v7.2.0...v7.3.0 [7.2.0]: https://
-github.com/bczsalba/pytermgui/compare/v7.1.0...v7.2.0 [7.1.0]: https://
-github.com/bczsalba/pytermgui/compare/v7.0.0...v7.1.0 [7.0.0]: https://
-github.com/bczsalba/pytermgui/compare/v6.4.0...v7.0.0 [6.4.0]: https://
-github.com/bczsalba/pytermgui/compare/v6.0.0...v6.4.0 [6.3.0]: https://
-github.com/bczsalba/pytermgui/compare/v6.2.2...v6.3.0 [6.2.2]: https://
-github.com/bczsalba/pytermgui/compare/v6.2.1...v6.2.2 [6.2.1]: https://
-github.com/bczsalba/pytermgui/compare/v6.2.0...v6.2.1 [6.2.0]: https://
-github.com/bczsalba/pytermgui/compare/v6.1.0...v6.2.0 [6.1.0]: https://
-github.com/bczsalba/pytermgui/compare/v6.0.0...v6.1.0 [6.0.0]: https://
-github.com/bczsalba/pytermgui/compare/v5.0.0...v6.0.0 [5.0.0]: https://
-github.com/bczsalba/pytermgui/compare/v4.3.2...v5.0.0 [4.3.2]: https://
-github.com/bczsalba/pytermgui/compare/v4.3.1...v4.3.2 [4.3.1]: https://
-github.com/bczsalba/pytermgui/compare/v4.3.0...v4.3.1 [4.3.0]: https://
-github.com/bczsalba/pytermgui/compare/v4.2.0...v4.3.0 [4.2.1]: https://
-github.com/bczsalba/pytermgui/compare/v4.2.0...v4.2.1 [4.2.0]: https://
-github.com/bczsalba/pytermgui/compare/v4.1.0...v4.2.0 [4.1.0]: https://
-github.com/bczsalba/pytermgui/compare/v4.0.0...v4.1.0 [4.0.1]: https://
-github.com/bczsalba/pytermgui/compare/v4.0.0...v4.0.1 [4.0.0]: https://
-github.com/bczsalba/pytermgui/compare/v3.2.1...v4.0.0
+create SVG and HTML screenshots of your terminal ## Latest release ### [7.5.0]
+- 2023-07-24 ### Additions - Add support for Windows' mouse events - Add
+support for feeding input into `getch` ### Refactor - Allow immediately halting
+`WindowManager` programatically by not blocking on `getch` calls ### Bugfixes -
+Fix mouse event handlers not getting cleaned up properly Read the full
+changelog [here](https://github.com/bczsalba/pytermgui/blob/master/
+CHANGELOG.md). [7.5.0]: https://github.com/bczsalba/pytermgui/compare/
+v7.4.0...v7.5.0 [7.4.0]: https://github.com/bczsalba/pytermgui/compare/
+v7.3.0...v7.4.0 [7.3.0]: https://github.com/bczsalba/pytermgui/compare/
+v7.2.0...v7.3.0 [7.2.0]: https://github.com/bczsalba/pytermgui/compare/
+v7.1.0...v7.2.0 [7.1.0]: https://github.com/bczsalba/pytermgui/compare/
+v7.0.0...v7.1.0 [7.0.0]: https://github.com/bczsalba/pytermgui/compare/
+v6.4.0...v7.0.0 [6.4.0]: https://github.com/bczsalba/pytermgui/compare/
+v6.0.0...v6.4.0 [6.3.0]: https://github.com/bczsalba/pytermgui/compare/
+v6.2.2...v6.3.0 [6.2.2]: https://github.com/bczsalba/pytermgui/compare/
+v6.2.1...v6.2.2 [6.2.1]: https://github.com/bczsalba/pytermgui/compare/
+v6.2.0...v6.2.1 [6.2.0]: https://github.com/bczsalba/pytermgui/compare/
+v6.1.0...v6.2.0 [6.1.0]: https://github.com/bczsalba/pytermgui/compare/
+v6.0.0...v6.1.0 [6.0.0]: https://github.com/bczsalba/pytermgui/compare/
+v5.0.0...v6.0.0 [5.0.0]: https://github.com/bczsalba/pytermgui/compare/
+v4.3.2...v5.0.0 [4.3.2]: https://github.com/bczsalba/pytermgui/compare/
+v4.3.1...v4.3.2 [4.3.1]: https://github.com/bczsalba/pytermgui/compare/
+v4.3.0...v4.3.1 [4.3.0]: https://github.com/bczsalba/pytermgui/compare/
+v4.2.0...v4.3.0 [4.2.1]: https://github.com/bczsalba/pytermgui/compare/
+v4.2.0...v4.2.1 [4.2.0]: https://github.com/bczsalba/pytermgui/compare/
+v4.1.0...v4.2.0 [4.1.0]: https://github.com/bczsalba/pytermgui/compare/
+v4.0.0...v4.1.0 [4.0.1]: https://github.com/bczsalba/pytermgui/compare/
+v4.0.0...v4.0.1 [4.0.0]: https://github.com/bczsalba/pytermgui/compare/
+v3.2.1...v4.0.0
```

