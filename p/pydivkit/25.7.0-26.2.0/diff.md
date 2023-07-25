# Comparing `tmp/pydivkit-25.7.0.tar.gz` & `tmp/pydivkit-26.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydivkit-25.7.0.tar", max compression
+gzip compressed data, was "pydivkit-26.2.0.tar", max compression
```

## Comparing `pydivkit-25.7.0.tar` & `pydivkit-26.2.0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     9446 2023-06-30 11:32:05.700599 pydivkit-25.7.0/README.md
--rw-r--r--   0        0        0      700 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/__init__.py
--rw-r--r--   0        0        0      164 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/__init__.py
--rw-r--r--   0        0        0      445 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/compat.py
--rw-r--r--   0        0        0    28631 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/entities.py
--rw-r--r--   0        0        0     3039 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/fields.py
--rw-r--r--   0        0        0        0 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/types/__init__.py
--rw-r--r--   0        0        0      728 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/core/types/union.py
--rw-r--r--   0        0        0    13901 2023-06-30 11:32:46.030344 pydivkit-25.7.0/pydivkit/div/__init__.py
--rw-r--r--   0        0        0      884 2023-06-30 11:32:45.781249 pydivkit-25.7.0/pydivkit/div/boolean_variable.py
--rw-r--r--   0        0        0      898 2023-06-30 11:32:45.781447 pydivkit-25.7.0/pydivkit/div/color_variable.py
--rw-r--r--   0        0        0      879 2023-06-30 11:32:45.781901 pydivkit-25.7.0/pydivkit/div/dict_variable.py
--rw-r--r--   0        0        0      863 2023-06-30 11:32:45.768330 pydivkit-25.7.0/pydivkit/div/div.py
--rw-r--r--   0        0        0     1209 2023-06-30 11:32:45.773659 pydivkit-25.7.0/pydivkit/div/div_absolute_edge_insets.py
--rw-r--r--   0        0        0     3285 2023-06-30 11:32:45.782394 pydivkit-25.7.0/pydivkit/div/div_accessibility.py
--rw-r--r--   0        0        0     3671 2023-06-30 11:32:45.783346 pydivkit-25.7.0/pydivkit/div/div_action.py
--rw-r--r--   0        0        0      285 2023-06-30 11:32:45.782543 pydivkit-25.7.0/pydivkit/div/div_alignment_horizontal.py
--rw-r--r--   0        0        0      309 2023-06-30 11:32:45.788687 pydivkit-25.7.0/pydivkit/div/div_alignment_vertical.py
--rw-r--r--   0        0        0     3038 2023-06-30 11:32:45.797990 pydivkit-25.7.0/pydivkit/div/div_animation.py
--rw-r--r--   0        0        0      371 2023-06-30 11:32:45.789016 pydivkit-25.7.0/pydivkit/div/div_animation_interpolator.py
--rw-r--r--   0        0        0      879 2023-06-30 11:32:45.791548 pydivkit-25.7.0/pydivkit/div/div_appearance_set_transition.py
--rw-r--r--   0        0        0      557 2023-06-30 11:32:45.788125 pydivkit-25.7.0/pydivkit/div/div_appearance_transition.py
--rw-r--r--   0        0        0      671 2023-06-30 11:32:45.790196 pydivkit-25.7.0/pydivkit/div/div_aspect.py
--rw-r--r--   0        0        0      599 2023-06-30 11:32:45.790066 pydivkit-25.7.0/pydivkit/div/div_background.py
--rw-r--r--   0        0        0     9833 2023-06-30 11:32:45.809339 pydivkit-25.7.0/pydivkit/div/div_base.py
--rw-r--r--   0        0        0      369 2023-06-30 11:32:45.796876 pydivkit-25.7.0/pydivkit/div/div_blend_mode.py
--rw-r--r--   0        0        0      764 2023-06-30 11:32:45.799481 pydivkit-25.7.0/pydivkit/div/div_blur.py
--rw-r--r--   0        0        0     1697 2023-06-30 11:32:45.798774 pydivkit-25.7.0/pydivkit/div/div_border.py
--rw-r--r--   0        0        0     1403 2023-06-30 11:32:45.802893 pydivkit-25.7.0/pydivkit/div/div_change_bounds_transition.py
--rw-r--r--   0        0        0      809 2023-06-30 11:32:45.801312 pydivkit-25.7.0/pydivkit/div/div_change_set_transition.py
--rw-r--r--   0        0        0      420 2023-06-30 11:32:45.797743 pydivkit-25.7.0/pydivkit/div/div_change_transition.py
--rw-r--r--   0        0        0     1176 2023-06-30 11:32:45.808208 pydivkit-25.7.0/pydivkit/div/div_circle_shape.py
--rw-r--r--   0        0        0    17693 2023-06-30 11:32:45.856440 pydivkit-25.7.0/pydivkit/div/div_container.py
--rw-r--r--   0        0        0      396 2023-06-30 11:32:45.806978 pydivkit-25.7.0/pydivkit/div/div_content_alignment_horizontal.py
--rw-r--r--   0        0        0      420 2023-06-30 11:32:45.807227 pydivkit-25.7.0/pydivkit/div/div_content_alignment_vertical.py
--rw-r--r--   0        0        0     1861 2023-06-30 11:32:45.813508 pydivkit-25.7.0/pydivkit/div/div_corners_radius.py
--rw-r--r--   0        0        0      351 2023-06-30 11:32:45.806726 pydivkit-25.7.0/pydivkit/div/div_count.py
--rw-r--r--   0        0        0     1292 2023-06-30 11:32:45.813258 pydivkit-25.7.0/pydivkit/div/div_currency_input_mask.py
--rw-r--r--   0        0        0    10752 2023-06-30 11:32:45.851666 pydivkit-25.7.0/pydivkit/div/div_custom.py
--rw-r--r--   0        0        0     2915 2023-06-30 11:32:45.818082 pydivkit-25.7.0/pydivkit/div/div_data.py
--rw-r--r--   0        0        0      872 2023-06-30 11:32:45.817813 pydivkit-25.7.0/pydivkit/div/div_default_indicator_item_placement.py
--rw-r--r--   0        0        0      802 2023-06-30 11:32:45.815439 pydivkit-25.7.0/pydivkit/div/div_dimension.py
--rw-r--r--   0        0        0     2970 2023-06-30 11:32:45.823213 pydivkit-25.7.0/pydivkit/div/div_disappear_action.py
--rw-r--r--   0        0        0     1228 2023-06-30 11:32:45.821063 pydivkit-25.7.0/pydivkit/div/div_download_callbacks.py
--rw-r--r--   0        0        0      302 2023-06-30 11:32:45.821876 pydivkit-25.7.0/pydivkit/div/div_drawable.py
--rw-r--r--   0        0        0     1385 2023-06-30 11:32:45.827364 pydivkit-25.7.0/pydivkit/div/div_edge_insets.py
--rw-r--r--   0        0        0      827 2023-06-30 11:32:45.828612 pydivkit-25.7.0/pydivkit/div/div_extension.py
--rw-r--r--   0        0        0     1675 2023-06-30 11:32:45.835158 pydivkit-25.7.0/pydivkit/div/div_fade_transition.py
--rw-r--r--   0        0        0      271 2023-06-30 11:32:45.829825 pydivkit-25.7.0/pydivkit/div/div_filter.py
--rw-r--r--   0        0        0      686 2023-06-30 11:32:45.832012 pydivkit-25.7.0/pydivkit/div/div_fixed_count.py
--rw-r--r--   0        0        0     3313 2023-06-30 11:32:45.841142 pydivkit-25.7.0/pydivkit/div/div_fixed_length_input_mask.py
--rw-r--r--   0        0        0     1090 2023-06-30 11:32:45.841686 pydivkit-25.7.0/pydivkit/div/div_fixed_size.py
--rw-r--r--   0        0        0     3026 2023-06-30 11:32:45.842834 pydivkit-25.7.0/pydivkit/div/div_focus.py
--rw-r--r--   0        0        0      300 2023-06-30 11:32:45.838220 pydivkit-25.7.0/pydivkit/div/div_font_weight.py
--rw-r--r--   0        0        0    14582 2023-06-30 11:32:45.876045 pydivkit-25.7.0/pydivkit/div/div_gallery.py
--rw-r--r--   0        0        0    14431 2023-06-30 11:32:45.879042 pydivkit-25.7.0/pydivkit/div/div_gif_image.py
--rw-r--r--   0        0        0    12886 2023-06-30 11:32:45.877903 pydivkit-25.7.0/pydivkit/div/div_grid.py
--rw-r--r--   0        0        0    16177 2023-06-30 11:32:45.886837 pydivkit-25.7.0/pydivkit/div/div_image.py
--rw-r--r--   0        0        0     2552 2023-06-30 11:32:45.857177 pydivkit-25.7.0/pydivkit/div/div_image_background.py
--rw-r--r--   0        0        0      300 2023-06-30 11:32:45.853746 pydivkit-25.7.0/pydivkit/div/div_image_scale.py
--rw-r--r--   0        0        0    13998 2023-06-30 11:32:45.890014 pydivkit-25.7.0/pydivkit/div/div_indicator.py
--rw-r--r--   0        0        0      490 2023-06-30 11:32:45.860161 pydivkit-25.7.0/pydivkit/div/div_indicator_item_placement.py
--rw-r--r--   0        0        0      516 2023-06-30 11:32:45.865772 pydivkit-25.7.0/pydivkit/div/div_infinity_count.py
--rw-r--r--   0        0        0    16458 2023-06-30 11:32:45.930319 pydivkit-25.7.0/pydivkit/div/div_input.py
--rw-r--r--   0        0        0      403 2023-06-30 11:32:45.867781 pydivkit-25.7.0/pydivkit/div/div_input_mask.py
--rw-r--r--   0        0        0      671 2023-06-30 11:32:45.872367 pydivkit-25.7.0/pydivkit/div/div_input_mask_base.py
--rw-r--r--   0        0        0      424 2023-06-30 11:32:45.874811 pydivkit-25.7.0/pydivkit/div/div_input_validator.py
--rw-r--r--   0        0        0     1323 2023-06-30 11:32:45.882317 pydivkit-25.7.0/pydivkit/div/div_input_validator_base.py
--rw-r--r--   0        0        0     1765 2023-06-30 11:32:45.888107 pydivkit-25.7.0/pydivkit/div/div_input_validator_expression.py
--rw-r--r--   0        0        0     1697 2023-06-30 11:32:45.888091 pydivkit-25.7.0/pydivkit/div/div_input_validator_regex.py
--rw-r--r--   0        0        0      255 2023-06-30 11:32:45.885163 pydivkit-25.7.0/pydivkit/div/div_line_style.py
--rw-r--r--   0        0        0     1046 2023-06-30 11:32:45.888410 pydivkit-25.7.0/pydivkit/div/div_linear_gradient.py
--rw-r--r--   0        0        0      974 2023-06-30 11:32:45.894475 pydivkit-25.7.0/pydivkit/div/div_match_parent_size.py
--rw-r--r--   0        0        0      858 2023-06-30 11:32:45.895232 pydivkit-25.7.0/pydivkit/div/div_neighbour_page_size.py
--rw-r--r--   0        0        0     1297 2023-06-30 11:32:45.897606 pydivkit-25.7.0/pydivkit/div/div_nine_patch_background.py
--rw-r--r--   0        0        0      795 2023-06-30 11:32:45.898273 pydivkit-25.7.0/pydivkit/div/div_page_size.py
--rw-r--r--   0        0        0    13014 2023-06-30 11:32:45.924238 pydivkit-25.7.0/pydivkit/div/div_pager.py
--rw-r--r--   0        0        0      369 2023-06-30 11:32:45.893109 pydivkit-25.7.0/pydivkit/div/div_pager_layout_mode.py
--rw-r--r--   0        0        0     1950 2023-06-30 11:32:45.905630 pydivkit-25.7.0/pydivkit/div/div_patch.py
--rw-r--r--   0        0        0      694 2023-06-30 11:32:45.904332 pydivkit-25.7.0/pydivkit/div/div_percentage_size.py
--rw-r--r--   0        0        0      357 2023-06-30 11:32:45.899756 pydivkit-25.7.0/pydivkit/div/div_pivot.py
--rw-r--r--   0        0        0     1136 2023-06-30 11:32:45.904950 pydivkit-25.7.0/pydivkit/div/div_pivot_fixed.py
--rw-r--r--   0        0        0      800 2023-06-30 11:32:45.907253 pydivkit-25.7.0/pydivkit/div/div_pivot_percentage.py
--rw-r--r--   0        0        0      768 2023-06-30 11:32:45.904791 pydivkit-25.7.0/pydivkit/div/div_point.py
--rw-r--r--   0        0        0     1933 2023-06-30 11:32:45.913307 pydivkit-25.7.0/pydivkit/div/div_radial_gradient.py
--rw-r--r--   0        0        0      473 2023-06-30 11:32:45.910337 pydivkit-25.7.0/pydivkit/div/div_radial_gradient_center.py
--rw-r--r--   0        0        0     1156 2023-06-30 11:32:45.916966 pydivkit-25.7.0/pydivkit/div/div_radial_gradient_fixed_center.py
--rw-r--r--   0        0        0      412 2023-06-30 11:32:45.912141 pydivkit-25.7.0/pydivkit/div/div_radial_gradient_radius.py
--rw-r--r--   0        0        0      800 2023-06-30 11:32:45.915905 pydivkit-25.7.0/pydivkit/div/div_radial_gradient_relative_center.py
--rw-r--r--   0        0        0     1052 2023-06-30 11:32:45.917465 pydivkit-25.7.0/pydivkit/div/div_radial_gradient_relative_radius.py
--rw-r--r--   0        0        0     1721 2023-06-30 11:32:45.923814 pydivkit-25.7.0/pydivkit/div/div_rounded_rectangle_shape.py
--rw-r--r--   0        0        0     2300 2023-06-30 11:32:45.930929 pydivkit-25.7.0/pydivkit/div/div_scale_transition.py
--rw-r--r--   0        0        0    13890 2023-06-30 11:32:45.956362 pydivkit-25.7.0/pydivkit/div/div_select.py
--rw-r--r--   0        0        0    13054 2023-06-30 11:32:45.952789 pydivkit-25.7.0/pydivkit/div/div_separator.py
--rw-r--r--   0        0        0     1198 2023-06-30 11:32:45.924609 pydivkit-25.7.0/pydivkit/div/div_shadow.py
--rw-r--r--   0        0        0      380 2023-06-30 11:32:45.922132 pydivkit-25.7.0/pydivkit/div/div_shape.py
--rw-r--r--   0        0        0     1144 2023-06-30 11:32:45.934871 pydivkit-25.7.0/pydivkit/div/div_shape_drawable.py
--rw-r--r--   0        0        0     2165 2023-06-30 11:32:45.936122 pydivkit-25.7.0/pydivkit/div/div_sight_action.py
--rw-r--r--   0        0        0      424 2023-06-30 11:32:45.930235 pydivkit-25.7.0/pydivkit/div/div_size.py
--rw-r--r--   0        0        0      256 2023-06-30 11:32:45.933138 pydivkit-25.7.0/pydivkit/div/div_size_unit.py
--rw-r--r--   0        0        0     2360 2023-06-30 11:32:45.943727 pydivkit-25.7.0/pydivkit/div/div_slide_transition.py
--rw-r--r--   0        0        0    15030 2023-06-30 11:32:45.980307 pydivkit-25.7.0/pydivkit/div/div_slider.py
--rw-r--r--   0        0        0      700 2023-06-30 11:32:45.940072 pydivkit-25.7.0/pydivkit/div/div_solid_background.py
--rw-r--r--   0        0        0    13360 2023-06-30 11:32:45.981759 pydivkit-25.7.0/pydivkit/div/div_state.py
--rw-r--r--   0        0        0     1101 2023-06-30 11:32:45.945288 pydivkit-25.7.0/pydivkit/div/div_stretch_indicator_item_placement.py
--rw-r--r--   0        0        0     1000 2023-06-30 11:32:45.948881 pydivkit-25.7.0/pydivkit/div/div_stroke.py
--rw-r--r--   0        0        0    20553 2023-06-30 11:32:46.013984 pydivkit-25.7.0/pydivkit/div/div_tabs.py
--rw-r--r--   0        0        0    25644 2023-06-30 11:32:46.018547 pydivkit-25.7.0/pydivkit/div/div_text.py
--rw-r--r--   0        0        0      373 2023-06-30 11:32:45.950652 pydivkit-25.7.0/pydivkit/div/div_text_gradient.py
--rw-r--r--   0        0        0      319 2023-06-30 11:32:45.956329 pydivkit-25.7.0/pydivkit/div/div_text_range_background.py
--rw-r--r--   0        0        0      975 2023-06-30 11:32:45.960020 pydivkit-25.7.0/pydivkit/div/div_text_range_border.py
--rw-r--r--   0        0        0     2796 2023-06-30 11:32:45.963845 pydivkit-25.7.0/pydivkit/div/div_timer.py
--rw-r--r--   0        0        0     2923 2023-06-30 11:32:45.974324 pydivkit-25.7.0/pydivkit/div/div_tooltip.py
--rw-r--r--   0        0        0     1171 2023-06-30 11:32:45.966110 pydivkit-25.7.0/pydivkit/div/div_transform.py
--rw-r--r--   0        0        0     1234 2023-06-30 11:32:45.969969 pydivkit-25.7.0/pydivkit/div/div_transition_base.py
--rw-r--r--   0        0        0      338 2023-06-30 11:32:45.975480 pydivkit-25.7.0/pydivkit/div/div_transition_selector.py
--rw-r--r--   0        0        0      333 2023-06-30 11:32:45.976638 pydivkit-25.7.0/pydivkit/div/div_transition_trigger.py
--rw-r--r--   0        0        0     1581 2023-06-30 11:32:45.984727 pydivkit-25.7.0/pydivkit/div/div_trigger.py
--rw-r--r--   0        0        0      613 2023-06-30 11:32:45.980644 pydivkit-25.7.0/pydivkit/div/div_variable.py
--rw-r--r--   0        0        0    13675 2023-06-30 11:32:46.027816 pydivkit-25.7.0/pydivkit/div/div_video.py
--rw-r--r--   0        0        0     2331 2023-06-30 11:32:45.990717 pydivkit-25.7.0/pydivkit/div/div_video_source.py
--rw-r--r--   0        0        0      286 2023-06-30 11:32:45.987531 pydivkit-25.7.0/pydivkit/div/div_visibility.py
--rw-r--r--   0        0        0     2956 2023-06-30 11:32:45.992519 pydivkit-25.7.0/pydivkit/div/div_visibility_action.py
--rw-r--r--   0        0        0     2298 2023-06-30 11:32:45.995316 pydivkit-25.7.0/pydivkit/div/div_wrap_content_size.py
--rw-r--r--   0        0        0      866 2023-06-30 11:32:45.996831 pydivkit-25.7.0/pydivkit/div/integer_variable.py
--rw-r--r--   0        0        0      872 2023-06-30 11:32:45.998793 pydivkit-25.7.0/pydivkit/div/number_variable.py
--rw-r--r--   0        0        0      860 2023-06-30 11:32:46.001820 pydivkit-25.7.0/pydivkit/div/string_variable.py
--rw-r--r--   0        0        0      882 2023-06-30 11:32:46.005354 pydivkit-25.7.0/pydivkit/div/url_variable.py
--rw-r--r--   0        0        0        0 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pydivkit/py.typed
--rw-r--r--   0        0        0     1697 2023-06-30 11:32:05.700599 pydivkit-25.7.0/pyproject.toml
--rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-25.7.0/PKG-INFO
+-rw-r--r--   0        0        0     9446 2023-07-25 09:26:49.579098 pydivkit-26.2.0/README.md
+-rw-r--r--   0        0        0      700 2023-07-25 09:26:49.579098 pydivkit-26.2.0/pydivkit/__init__.py
+-rw-r--r--   0        0        0      164 2023-07-25 09:26:49.579098 pydivkit-26.2.0/pydivkit/core/__init__.py
+-rw-r--r--   0        0        0      445 2023-07-25 09:26:49.579098 pydivkit-26.2.0/pydivkit/core/compat.py
+-rw-r--r--   0        0        0    28631 2023-07-25 09:26:49.579098 pydivkit-26.2.0/pydivkit/core/entities.py
+-rw-r--r--   0        0        0     3039 2023-07-25 09:26:49.579098 pydivkit-26.2.0/pydivkit/core/fields.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:26:49.579098 pydivkit-26.2.0/pydivkit/core/types/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-25 09:26:49.579098 pydivkit-26.2.0/pydivkit/core/types/union.py
+-rw-r--r--   0        0        0    13901 2023-07-25 09:27:30.430096 pydivkit-26.2.0/pydivkit/div/__init__.py
+-rw-r--r--   0        0        0      884 2023-07-25 09:27:30.186199 pydivkit-26.2.0/pydivkit/div/boolean_variable.py
+-rw-r--r--   0        0        0      898 2023-07-25 09:27:30.186140 pydivkit-26.2.0/pydivkit/div/color_variable.py
+-rw-r--r--   0        0        0      879 2023-07-25 09:27:30.186139 pydivkit-26.2.0/pydivkit/div/dict_variable.py
+-rw-r--r--   0        0        0      863 2023-07-25 09:27:30.162254 pydivkit-26.2.0/pydivkit/div/div.py
+-rw-r--r--   0        0        0     1209 2023-07-25 09:27:30.162255 pydivkit-26.2.0/pydivkit/div/div_absolute_edge_insets.py
+-rw-r--r--   0        0        0     3285 2023-07-25 09:27:30.187306 pydivkit-26.2.0/pydivkit/div/div_accessibility.py
+-rw-r--r--   0        0        0     3671 2023-07-25 09:27:30.187930 pydivkit-26.2.0/pydivkit/div/div_action.py
+-rw-r--r--   0        0        0      321 2023-07-25 09:27:30.185795 pydivkit-26.2.0/pydivkit/div/div_alignment_horizontal.py
+-rw-r--r--   0        0        0      309 2023-07-25 09:27:30.190345 pydivkit-26.2.0/pydivkit/div/div_alignment_vertical.py
+-rw-r--r--   0        0        0     3038 2023-07-25 09:27:30.197098 pydivkit-26.2.0/pydivkit/div/div_animation.py
+-rw-r--r--   0        0        0      371 2023-07-25 09:27:30.191453 pydivkit-26.2.0/pydivkit/div/div_animation_interpolator.py
+-rw-r--r--   0        0        0      879 2023-07-25 09:27:30.193298 pydivkit-26.2.0/pydivkit/div/div_appearance_set_transition.py
+-rw-r--r--   0        0        0      557 2023-07-25 09:27:30.190846 pydivkit-26.2.0/pydivkit/div/div_appearance_transition.py
+-rw-r--r--   0        0        0      671 2023-07-25 09:27:30.192321 pydivkit-26.2.0/pydivkit/div/div_aspect.py
+-rw-r--r--   0        0        0      599 2023-07-25 09:27:30.191753 pydivkit-26.2.0/pydivkit/div/div_background.py
+-rw-r--r--   0        0        0     9833 2023-07-25 09:27:30.222691 pydivkit-26.2.0/pydivkit/div/div_base.py
+-rw-r--r--   0        0        0      369 2023-07-25 09:27:30.195246 pydivkit-26.2.0/pydivkit/div/div_blend_mode.py
+-rw-r--r--   0        0        0      764 2023-07-25 09:27:30.197107 pydivkit-26.2.0/pydivkit/div/div_blur.py
+-rw-r--r--   0        0        0     1697 2023-07-25 09:27:30.197589 pydivkit-26.2.0/pydivkit/div/div_border.py
+-rw-r--r--   0        0        0     1403 2023-07-25 09:27:30.200143 pydivkit-26.2.0/pydivkit/div/div_change_bounds_transition.py
+-rw-r--r--   0        0        0      809 2023-07-25 09:27:30.199301 pydivkit-26.2.0/pydivkit/div/div_change_set_transition.py
+-rw-r--r--   0        0        0      420 2023-07-25 09:27:30.197593 pydivkit-26.2.0/pydivkit/div/div_change_transition.py
+-rw-r--r--   0        0        0     1176 2023-07-25 09:27:30.228491 pydivkit-26.2.0/pydivkit/div/div_circle_shape.py
+-rw-r--r--   0        0        0    17693 2023-07-25 09:27:30.243759 pydivkit-26.2.0/pydivkit/div/div_container.py
+-rw-r--r--   0        0        0      432 2023-07-25 09:27:30.223601 pydivkit-26.2.0/pydivkit/div/div_content_alignment_horizontal.py
+-rw-r--r--   0        0        0      420 2023-07-25 09:27:30.228311 pydivkit-26.2.0/pydivkit/div/div_content_alignment_vertical.py
+-rw-r--r--   0        0        0     1861 2023-07-25 09:27:30.230321 pydivkit-26.2.0/pydivkit/div/div_corners_radius.py
+-rw-r--r--   0        0        0      351 2023-07-25 09:27:30.223735 pydivkit-26.2.0/pydivkit/div/div_count.py
+-rw-r--r--   0        0        0     1292 2023-07-25 09:27:30.229919 pydivkit-26.2.0/pydivkit/div/div_currency_input_mask.py
+-rw-r--r--   0        0        0    10752 2023-07-25 09:27:30.250991 pydivkit-26.2.0/pydivkit/div/div_custom.py
+-rw-r--r--   0        0        0     2915 2023-07-25 09:27:30.239230 pydivkit-26.2.0/pydivkit/div/div_data.py
+-rw-r--r--   0        0        0      872 2023-07-25 09:27:30.243746 pydivkit-26.2.0/pydivkit/div/div_default_indicator_item_placement.py
+-rw-r--r--   0        0        0      802 2023-07-25 09:27:30.239361 pydivkit-26.2.0/pydivkit/div/div_dimension.py
+-rw-r--r--   0        0        0     2970 2023-07-25 09:27:30.243462 pydivkit-26.2.0/pydivkit/div/div_disappear_action.py
+-rw-r--r--   0        0        0     1228 2023-07-25 09:27:30.243463 pydivkit-26.2.0/pydivkit/div/div_download_callbacks.py
+-rw-r--r--   0        0        0      302 2023-07-25 09:27:30.239230 pydivkit-26.2.0/pydivkit/div/div_drawable.py
+-rw-r--r--   0        0        0     2081 2023-07-25 09:27:30.252462 pydivkit-26.2.0/pydivkit/div/div_edge_insets.py
+-rw-r--r--   0        0        0      827 2023-07-25 09:27:30.252468 pydivkit-26.2.0/pydivkit/div/div_extension.py
+-rw-r--r--   0        0        0     1675 2023-07-25 09:27:30.258427 pydivkit-26.2.0/pydivkit/div/div_fade_transition.py
+-rw-r--r--   0        0        0      271 2023-07-25 09:27:30.250816 pydivkit-26.2.0/pydivkit/div/div_filter.py
+-rw-r--r--   0        0        0      686 2023-07-25 09:27:30.257832 pydivkit-26.2.0/pydivkit/div/div_fixed_count.py
+-rw-r--r--   0        0        0     3313 2023-07-25 09:27:30.260515 pydivkit-26.2.0/pydivkit/div/div_fixed_length_input_mask.py
+-rw-r--r--   0        0        0     1090 2023-07-25 09:27:30.258231 pydivkit-26.2.0/pydivkit/div/div_fixed_size.py
+-rw-r--r--   0        0        0     3026 2023-07-25 09:27:30.259568 pydivkit-26.2.0/pydivkit/div/div_focus.py
+-rw-r--r--   0        0        0      300 2023-07-25 09:27:30.258954 pydivkit-26.2.0/pydivkit/div/div_font_weight.py
+-rw-r--r--   0        0        0    14582 2023-07-25 09:27:30.300538 pydivkit-26.2.0/pydivkit/div/div_gallery.py
+-rw-r--r--   0        0        0    14431 2023-07-25 09:27:30.300550 pydivkit-26.2.0/pydivkit/div/div_gif_image.py
+-rw-r--r--   0        0        0    12886 2023-07-25 09:27:30.300241 pydivkit-26.2.0/pydivkit/div/div_grid.py
+-rw-r--r--   0        0        0    16177 2023-07-25 09:27:30.300547 pydivkit-26.2.0/pydivkit/div/div_image.py
+-rw-r--r--   0        0        0     2552 2023-07-25 09:27:30.281043 pydivkit-26.2.0/pydivkit/div/div_image_background.py
+-rw-r--r--   0        0        0      300 2023-07-25 09:27:30.272307 pydivkit-26.2.0/pydivkit/div/div_image_scale.py
+-rw-r--r--   0        0        0    13998 2023-07-25 09:27:30.300533 pydivkit-26.2.0/pydivkit/div/div_indicator.py
+-rw-r--r--   0        0        0      490 2023-07-25 09:27:30.272980 pydivkit-26.2.0/pydivkit/div/div_indicator_item_placement.py
+-rw-r--r--   0        0        0      516 2023-07-25 09:27:30.282207 pydivkit-26.2.0/pydivkit/div/div_infinity_count.py
+-rw-r--r--   0        0        0    16458 2023-07-25 09:27:30.324885 pydivkit-26.2.0/pydivkit/div/div_input.py
+-rw-r--r--   0        0        0      403 2023-07-25 09:27:30.284402 pydivkit-26.2.0/pydivkit/div/div_input_mask.py
+-rw-r--r--   0        0        0      671 2023-07-25 09:27:30.286187 pydivkit-26.2.0/pydivkit/div/div_input_mask_base.py
+-rw-r--r--   0        0        0      424 2023-07-25 09:27:30.289458 pydivkit-26.2.0/pydivkit/div/div_input_validator.py
+-rw-r--r--   0        0        0     1323 2023-07-25 09:27:30.304252 pydivkit-26.2.0/pydivkit/div/div_input_validator_base.py
+-rw-r--r--   0        0        0     1765 2023-07-25 09:27:30.308112 pydivkit-26.2.0/pydivkit/div/div_input_validator_expression.py
+-rw-r--r--   0        0        0     1697 2023-07-25 09:27:30.308116 pydivkit-26.2.0/pydivkit/div/div_input_validator_regex.py
+-rw-r--r--   0        0        0      255 2023-07-25 09:27:30.304918 pydivkit-26.2.0/pydivkit/div/div_line_style.py
+-rw-r--r--   0        0        0     1046 2023-07-25 09:27:30.307446 pydivkit-26.2.0/pydivkit/div/div_linear_gradient.py
+-rw-r--r--   0        0        0      974 2023-07-25 09:27:30.306755 pydivkit-26.2.0/pydivkit/div/div_match_parent_size.py
+-rw-r--r--   0        0        0      858 2023-07-25 09:27:30.306732 pydivkit-26.2.0/pydivkit/div/div_neighbour_page_size.py
+-rw-r--r--   0        0        0     1297 2023-07-25 09:27:30.310932 pydivkit-26.2.0/pydivkit/div/div_nine_patch_background.py
+-rw-r--r--   0        0        0      795 2023-07-25 09:27:30.311661 pydivkit-26.2.0/pydivkit/div/div_page_size.py
+-rw-r--r--   0        0        0    13014 2023-07-25 09:27:30.337403 pydivkit-26.2.0/pydivkit/div/div_pager.py
+-rw-r--r--   0        0        0      369 2023-07-25 09:27:30.310674 pydivkit-26.2.0/pydivkit/div/div_pager_layout_mode.py
+-rw-r--r--   0        0        0     1950 2023-07-25 09:27:30.328820 pydivkit-26.2.0/pydivkit/div/div_patch.py
+-rw-r--r--   0        0        0      694 2023-07-25 09:27:30.326348 pydivkit-26.2.0/pydivkit/div/div_percentage_size.py
+-rw-r--r--   0        0        0      357 2023-07-25 09:27:30.324596 pydivkit-26.2.0/pydivkit/div/div_pivot.py
+-rw-r--r--   0        0        0     1136 2023-07-25 09:27:30.329898 pydivkit-26.2.0/pydivkit/div/div_pivot_fixed.py
+-rw-r--r--   0        0        0      800 2023-07-25 09:27:30.329658 pydivkit-26.2.0/pydivkit/div/div_pivot_percentage.py
+-rw-r--r--   0        0        0      768 2023-07-25 09:27:30.328470 pydivkit-26.2.0/pydivkit/div/div_point.py
+-rw-r--r--   0        0        0     1933 2023-07-25 09:27:30.333466 pydivkit-26.2.0/pydivkit/div/div_radial_gradient.py
+-rw-r--r--   0        0        0      473 2023-07-25 09:27:30.330155 pydivkit-26.2.0/pydivkit/div/div_radial_gradient_center.py
+-rw-r--r--   0        0        0     1156 2023-07-25 09:27:30.333546 pydivkit-26.2.0/pydivkit/div/div_radial_gradient_fixed_center.py
+-rw-r--r--   0        0        0      412 2023-07-25 09:27:30.333066 pydivkit-26.2.0/pydivkit/div/div_radial_gradient_radius.py
+-rw-r--r--   0        0        0      800 2023-07-25 09:27:30.335394 pydivkit-26.2.0/pydivkit/div/div_radial_gradient_relative_center.py
+-rw-r--r--   0        0        0     1052 2023-07-25 09:27:30.335760 pydivkit-26.2.0/pydivkit/div/div_radial_gradient_relative_radius.py
+-rw-r--r--   0        0        0     1721 2023-07-25 09:27:30.337523 pydivkit-26.2.0/pydivkit/div/div_rounded_rectangle_shape.py
+-rw-r--r--   0        0        0     2300 2023-07-25 09:27:30.339600 pydivkit-26.2.0/pydivkit/div/div_scale_transition.py
+-rw-r--r--   0        0        0    13890 2023-07-25 09:27:30.374759 pydivkit-26.2.0/pydivkit/div/div_select.py
+-rw-r--r--   0        0        0    13054 2023-07-25 09:27:30.373866 pydivkit-26.2.0/pydivkit/div/div_separator.py
+-rw-r--r--   0        0        0     1198 2023-07-25 09:27:30.338864 pydivkit-26.2.0/pydivkit/div/div_shadow.py
+-rw-r--r--   0        0        0      380 2023-07-25 09:27:30.338485 pydivkit-26.2.0/pydivkit/div/div_shape.py
+-rw-r--r--   0        0        0     1144 2023-07-25 09:27:30.342484 pydivkit-26.2.0/pydivkit/div/div_shape_drawable.py
+-rw-r--r--   0        0        0     2165 2023-07-25 09:27:30.343815 pydivkit-26.2.0/pydivkit/div/div_sight_action.py
+-rw-r--r--   0        0        0      424 2023-07-25 09:27:30.340811 pydivkit-26.2.0/pydivkit/div/div_size.py
+-rw-r--r--   0        0        0      256 2023-07-25 09:27:30.343146 pydivkit-26.2.0/pydivkit/div/div_size_unit.py
+-rw-r--r--   0        0        0     2360 2023-07-25 09:27:30.347643 pydivkit-26.2.0/pydivkit/div/div_slide_transition.py
+-rw-r--r--   0        0        0    15030 2023-07-25 09:27:30.380533 pydivkit-26.2.0/pydivkit/div/div_slider.py
+-rw-r--r--   0        0        0      700 2023-07-25 09:27:30.347001 pydivkit-26.2.0/pydivkit/div/div_solid_background.py
+-rw-r--r--   0        0        0    13360 2023-07-25 09:27:30.379404 pydivkit-26.2.0/pydivkit/div/div_state.py
+-rw-r--r--   0        0        0     1101 2023-07-25 09:27:30.349641 pydivkit-26.2.0/pydivkit/div/div_stretch_indicator_item_placement.py
+-rw-r--r--   0        0        0     1000 2023-07-25 09:27:30.350692 pydivkit-26.2.0/pydivkit/div/div_stroke.py
+-rw-r--r--   0        0        0    20553 2023-07-25 09:27:30.388612 pydivkit-26.2.0/pydivkit/div/div_tabs.py
+-rw-r--r--   0        0        0    25644 2023-07-25 09:27:30.412469 pydivkit-26.2.0/pydivkit/div/div_text.py
+-rw-r--r--   0        0        0      373 2023-07-25 09:27:30.353354 pydivkit-26.2.0/pydivkit/div/div_text_gradient.py
+-rw-r--r--   0        0        0      319 2023-07-25 09:27:30.367924 pydivkit-26.2.0/pydivkit/div/div_text_range_background.py
+-rw-r--r--   0        0        0      975 2023-07-25 09:27:30.372053 pydivkit-26.2.0/pydivkit/div/div_text_range_border.py
+-rw-r--r--   0        0        0     2796 2023-07-25 09:27:30.375723 pydivkit-26.2.0/pydivkit/div/div_timer.py
+-rw-r--r--   0        0        0     2923 2023-07-25 09:27:30.383726 pydivkit-26.2.0/pydivkit/div/div_tooltip.py
+-rw-r--r--   0        0        0     1171 2023-07-25 09:27:30.379247 pydivkit-26.2.0/pydivkit/div/div_transform.py
+-rw-r--r--   0        0        0     1234 2023-07-25 09:27:30.380280 pydivkit-26.2.0/pydivkit/div/div_transition_base.py
+-rw-r--r--   0        0        0      338 2023-07-25 09:27:30.382441 pydivkit-26.2.0/pydivkit/div/div_transition_selector.py
+-rw-r--r--   0        0        0      333 2023-07-25 09:27:30.384089 pydivkit-26.2.0/pydivkit/div/div_transition_trigger.py
+-rw-r--r--   0        0        0     1581 2023-07-25 09:27:30.387770 pydivkit-26.2.0/pydivkit/div/div_trigger.py
+-rw-r--r--   0        0        0      613 2023-07-25 09:27:30.384774 pydivkit-26.2.0/pydivkit/div/div_variable.py
+-rw-r--r--   0        0        0    13675 2023-07-25 09:27:30.429259 pydivkit-26.2.0/pydivkit/div/div_video.py
+-rw-r--r--   0        0        0     2331 2023-07-25 09:27:30.392165 pydivkit-26.2.0/pydivkit/div/div_video_source.py
+-rw-r--r--   0        0        0      286 2023-07-25 09:27:30.388724 pydivkit-26.2.0/pydivkit/div/div_visibility.py
+-rw-r--r--   0        0        0     2956 2023-07-25 09:27:30.391502 pydivkit-26.2.0/pydivkit/div/div_visibility_action.py
+-rw-r--r--   0        0        0     2298 2023-07-25 09:27:30.402754 pydivkit-26.2.0/pydivkit/div/div_wrap_content_size.py
+-rw-r--r--   0        0        0      866 2023-07-25 09:27:30.402771 pydivkit-26.2.0/pydivkit/div/integer_variable.py
+-rw-r--r--   0        0        0      872 2023-07-25 09:27:30.418265 pydivkit-26.2.0/pydivkit/div/number_variable.py
+-rw-r--r--   0        0        0      860 2023-07-25 09:27:30.418274 pydivkit-26.2.0/pydivkit/div/string_variable.py
+-rw-r--r--   0        0        0      882 2023-07-25 09:27:30.419864 pydivkit-26.2.0/pydivkit/div/url_variable.py
+-rw-r--r--   0        0        0        0 2023-07-25 09:26:49.579098 pydivkit-26.2.0/pydivkit/py.typed
+-rw-r--r--   0        0        0     1697 2023-07-25 09:26:49.579098 pydivkit-26.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10885 1970-01-01 00:00:00.000000 pydivkit-26.2.0/PKG-INFO
```

### Comparing `pydivkit-25.7.0/README.md` & `pydivkit-26.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/__init__.py` & `pydivkit-26.2.0/pydivkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/core/entities.py` & `pydivkit-26.2.0/pydivkit/core/entities.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/core/fields.py` & `pydivkit-26.2.0/pydivkit/core/fields.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/core/types/union.py` & `pydivkit-26.2.0/pydivkit/core/types/union.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/__init__.py` & `pydivkit-26.2.0/pydivkit/div/__init__.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/boolean_variable.py` & `pydivkit-26.2.0/pydivkit/div/boolean_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/color_variable.py` & `pydivkit-26.2.0/pydivkit/div/color_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/dict_variable.py` & `pydivkit-26.2.0/pydivkit/div/dict_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div.py` & `pydivkit-26.2.0/pydivkit/div/div.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_absolute_edge_insets.py` & `pydivkit-26.2.0/pydivkit/div/div_absolute_edge_insets.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_accessibility.py` & `pydivkit-26.2.0/pydivkit/div/div_accessibility.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_action.py` & `pydivkit-26.2.0/pydivkit/div/div_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_animation.py` & `pydivkit-26.2.0/pydivkit/div/div_animation.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_appearance_set_transition.py` & `pydivkit-26.2.0/pydivkit/div/div_appearance_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_appearance_transition.py` & `pydivkit-26.2.0/pydivkit/div/div_appearance_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_aspect.py` & `pydivkit-26.2.0/pydivkit/div/div_aspect.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_background.py` & `pydivkit-26.2.0/pydivkit/div/div_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_base.py` & `pydivkit-26.2.0/pydivkit/div/div_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_blur.py` & `pydivkit-26.2.0/pydivkit/div/div_blur.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_border.py` & `pydivkit-26.2.0/pydivkit/div/div_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_change_bounds_transition.py` & `pydivkit-26.2.0/pydivkit/div/div_change_bounds_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_change_set_transition.py` & `pydivkit-26.2.0/pydivkit/div/div_change_set_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_circle_shape.py` & `pydivkit-26.2.0/pydivkit/div/div_circle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_container.py` & `pydivkit-26.2.0/pydivkit/div/div_container.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_corners_radius.py` & `pydivkit-26.2.0/pydivkit/div/div_corners_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_currency_input_mask.py` & `pydivkit-26.2.0/pydivkit/div/div_currency_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_custom.py` & `pydivkit-26.2.0/pydivkit/div/div_custom.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_data.py` & `pydivkit-26.2.0/pydivkit/div/div_data.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_default_indicator_item_placement.py` & `pydivkit-26.2.0/pydivkit/div/div_default_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_dimension.py` & `pydivkit-26.2.0/pydivkit/div/div_dimension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_disappear_action.py` & `pydivkit-26.2.0/pydivkit/div/div_disappear_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_download_callbacks.py` & `pydivkit-26.2.0/pydivkit/div/div_download_callbacks.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_edge_insets.py` & `pydivkit-26.2.0/pydivkit/div/div_shadow.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,48 +4,45 @@
 from __future__ import annotations
 
 import enum
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_size_unit
+from . import div_point
 
 
-# It sets margins.
-class DivEdgeInsets(BaseDiv):
+# Element shadow.
+class DivShadow(BaseDiv):
 
     def __init__(
         self, *,
-        bottom: typing.Optional[typing.Union[Expr, int]] = None,
-        left: typing.Optional[typing.Union[Expr, int]] = None,
-        right: typing.Optional[typing.Union[Expr, int]] = None,
-        top: typing.Optional[typing.Union[Expr, int]] = None,
-        unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = None,
+        alpha: typing.Optional[typing.Union[Expr, float]] = None,
+        blur: typing.Optional[typing.Union[Expr, int]] = None,
+        color: typing.Optional[typing.Union[Expr, str]] = None,
+        offset: typing.Optional[div_point.DivPoint] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
-            bottom=bottom,
-            left=left,
-            right=right,
-            top=top,
-            unit=unit,
+            alpha=alpha,
+            blur=blur,
+            color=color,
+            offset=offset,
             **kwargs,
         )
 
-    bottom: typing.Optional[typing.Union[Expr, int]] = Field(
-        description="Bottom margin.",
+    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
+        description="Shadow transparency.",
     )
-    left: typing.Optional[typing.Union[Expr, int]] = Field(
-        description="Left margin.",
+    blur: typing.Optional[typing.Union[Expr, int]] = Field(
+        description="Blur intensity.",
     )
-    right: typing.Optional[typing.Union[Expr, int]] = Field(
-        description="Right margin.",
+    color: typing.Optional[typing.Union[Expr, str]] = Field(
+        format="color", 
+        description="Shadow color.",
     )
-    top: typing.Optional[typing.Union[Expr, int]] = Field(
-        description="Top margin.",
-    )
-    unit: typing.Optional[typing.Union[Expr, div_size_unit.DivSizeUnit]] = Field(
+    offset: div_point.DivPoint = Field(
+        description="Shadow offset.",
     )
 
 
-DivEdgeInsets.update_forward_refs()
+DivShadow.update_forward_refs()
```

### Comparing `pydivkit-25.7.0/pydivkit/div/div_extension.py` & `pydivkit-26.2.0/pydivkit/div/div_extension.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_fade_transition.py` & `pydivkit-26.2.0/pydivkit/div/div_fade_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_fixed_count.py` & `pydivkit-26.2.0/pydivkit/div/div_fixed_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_fixed_length_input_mask.py` & `pydivkit-26.2.0/pydivkit/div/div_fixed_length_input_mask.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_fixed_size.py` & `pydivkit-26.2.0/pydivkit/div/div_fixed_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_focus.py` & `pydivkit-26.2.0/pydivkit/div/div_focus.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_gallery.py` & `pydivkit-26.2.0/pydivkit/div/div_gallery.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_gif_image.py` & `pydivkit-26.2.0/pydivkit/div/div_gif_image.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_grid.py` & `pydivkit-26.2.0/pydivkit/div/div_grid.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_image.py` & `pydivkit-26.2.0/pydivkit/div/div_image.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_image_background.py` & `pydivkit-26.2.0/pydivkit/div/div_image_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_indicator.py` & `pydivkit-26.2.0/pydivkit/div/div_indicator.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_infinity_count.py` & `pydivkit-26.2.0/pydivkit/div/div_infinity_count.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_input.py` & `pydivkit-26.2.0/pydivkit/div/div_input.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_input_mask_base.py` & `pydivkit-26.2.0/pydivkit/div/div_input_mask_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_input_validator_base.py` & `pydivkit-26.2.0/pydivkit/div/div_input_validator_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_input_validator_expression.py` & `pydivkit-26.2.0/pydivkit/div/div_input_validator_expression.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_input_validator_regex.py` & `pydivkit-26.2.0/pydivkit/div/div_input_validator_regex.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_linear_gradient.py` & `pydivkit-26.2.0/pydivkit/div/div_linear_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_match_parent_size.py` & `pydivkit-26.2.0/pydivkit/div/div_match_parent_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_neighbour_page_size.py` & `pydivkit-26.2.0/pydivkit/div/div_neighbour_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_nine_patch_background.py` & `pydivkit-26.2.0/pydivkit/div/div_nine_patch_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_page_size.py` & `pydivkit-26.2.0/pydivkit/div/div_page_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_pager.py` & `pydivkit-26.2.0/pydivkit/div/div_pager.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_patch.py` & `pydivkit-26.2.0/pydivkit/div/div_patch.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_percentage_size.py` & `pydivkit-26.2.0/pydivkit/div/div_percentage_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_pivot_fixed.py` & `pydivkit-26.2.0/pydivkit/div/div_pivot_fixed.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_pivot_percentage.py` & `pydivkit-26.2.0/pydivkit/div/div_pivot_percentage.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_point.py` & `pydivkit-26.2.0/pydivkit/div/div_point.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_radial_gradient.py` & `pydivkit-26.2.0/pydivkit/div/div_radial_gradient.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_radial_gradient_fixed_center.py` & `pydivkit-26.2.0/pydivkit/div/div_radial_gradient_fixed_center.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_radial_gradient_relative_center.py` & `pydivkit-26.2.0/pydivkit/div/div_radial_gradient_relative_center.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_radial_gradient_relative_radius.py` & `pydivkit-26.2.0/pydivkit/div/div_radial_gradient_relative_radius.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_rounded_rectangle_shape.py` & `pydivkit-26.2.0/pydivkit/div/div_rounded_rectangle_shape.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_scale_transition.py` & `pydivkit-26.2.0/pydivkit/div/div_scale_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_select.py` & `pydivkit-26.2.0/pydivkit/div/div_select.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_separator.py` & `pydivkit-26.2.0/pydivkit/div/div_separator.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_shadow.py` & `pydivkit-26.2.0/pydivkit/div/number_variable.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,45 +4,36 @@
 from __future__ import annotations
 
 import enum
 import typing
 
 from pydivkit.core import BaseDiv, Expr, Field
 
-from . import div_point
 
-
-# Element shadow.
-class DivShadow(BaseDiv):
+# A floating-point variable.
+class NumberVariable(BaseDiv):
 
     def __init__(
         self, *,
-        alpha: typing.Optional[typing.Union[Expr, float]] = None,
-        blur: typing.Optional[typing.Union[Expr, int]] = None,
-        color: typing.Optional[typing.Union[Expr, str]] = None,
-        offset: typing.Optional[div_point.DivPoint] = None,
+        type: str = "number",
+        name: typing.Optional[typing.Union[Expr, str]] = None,
+        value: typing.Optional[typing.Union[Expr, float]] = None,
         **kwargs: typing.Any,
     ):
         super().__init__(
-            alpha=alpha,
-            blur=blur,
-            color=color,
-            offset=offset,
+            type=type,
+            name=name,
+            value=value,
             **kwargs,
         )
 
-    alpha: typing.Optional[typing.Union[Expr, float]] = Field(
-        description="Shadow transparency.",
-    )
-    blur: typing.Optional[typing.Union[Expr, int]] = Field(
-        description="Blur intensity.",
-    )
-    color: typing.Optional[typing.Union[Expr, str]] = Field(
-        format="color", 
-        description="Shadow color.",
+    type: str = Field(default="number")
+    name: typing.Union[Expr, str] = Field(
+        min_length=1, 
+        description="Variable name.",
     )
-    offset: div_point.DivPoint = Field(
-        description="Shadow offset.",
+    value: typing.Union[Expr, float] = Field(
+        description="Value.",
     )
 
 
-DivShadow.update_forward_refs()
+NumberVariable.update_forward_refs()
```

### Comparing `pydivkit-25.7.0/pydivkit/div/div_shape_drawable.py` & `pydivkit-26.2.0/pydivkit/div/div_shape_drawable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_sight_action.py` & `pydivkit-26.2.0/pydivkit/div/div_sight_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_slide_transition.py` & `pydivkit-26.2.0/pydivkit/div/div_slide_transition.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_slider.py` & `pydivkit-26.2.0/pydivkit/div/div_slider.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_solid_background.py` & `pydivkit-26.2.0/pydivkit/div/div_solid_background.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_state.py` & `pydivkit-26.2.0/pydivkit/div/div_state.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_stretch_indicator_item_placement.py` & `pydivkit-26.2.0/pydivkit/div/div_stretch_indicator_item_placement.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_stroke.py` & `pydivkit-26.2.0/pydivkit/div/div_stroke.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_tabs.py` & `pydivkit-26.2.0/pydivkit/div/div_tabs.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_text.py` & `pydivkit-26.2.0/pydivkit/div/div_text.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_text_range_border.py` & `pydivkit-26.2.0/pydivkit/div/div_text_range_border.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_timer.py` & `pydivkit-26.2.0/pydivkit/div/div_timer.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_tooltip.py` & `pydivkit-26.2.0/pydivkit/div/div_tooltip.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_transform.py` & `pydivkit-26.2.0/pydivkit/div/div_transform.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_transition_base.py` & `pydivkit-26.2.0/pydivkit/div/div_transition_base.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_trigger.py` & `pydivkit-26.2.0/pydivkit/div/div_trigger.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_variable.py` & `pydivkit-26.2.0/pydivkit/div/div_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_video.py` & `pydivkit-26.2.0/pydivkit/div/div_video.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_video_source.py` & `pydivkit-26.2.0/pydivkit/div/div_video_source.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_visibility_action.py` & `pydivkit-26.2.0/pydivkit/div/div_visibility_action.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/div_wrap_content_size.py` & `pydivkit-26.2.0/pydivkit/div/div_wrap_content_size.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/integer_variable.py` & `pydivkit-26.2.0/pydivkit/div/integer_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/string_variable.py` & `pydivkit-26.2.0/pydivkit/div/string_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pydivkit/div/url_variable.py` & `pydivkit-26.2.0/pydivkit/div/url_variable.py`

 * *Files identical despite different names*

### Comparing `pydivkit-25.7.0/pyproject.toml` & `pydivkit-26.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydivkit"
-version = "25.7.0"
+version = "26.2.0"
 description = "DivKit python library"
 readme = "README.md"
 repository = "https://github.com/divkit/divkit/tree/main/json-builder/python"
 keywords = ["divkit", "sdk"]
 authors = [
     "Vladislav Bakaev <bakaev-vlad@yandex-team.ru>",
     "Pavel Mosein <p-mosein@yandex-team.ru>",
```

### Comparing `pydivkit-25.7.0/PKG-INFO` & `pydivkit-26.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydivkit
-Version: 25.7.0
+Version: 26.2.0
 Summary: DivKit python library
 Home-page: https://github.com/divkit/divkit/tree/main/json-builder/python
 Keywords: divkit,sdk
 Author: Vladislav Bakaev
 Author-email: bakaev-vlad@yandex-team.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

