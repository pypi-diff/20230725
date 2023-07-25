# Comparing `tmp/reflex-0.2.3a1.tar.gz` & `tmp/reflex-0.2.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.2.3a1.tar", max compression
+gzip compressed data, was "reflex-0.2.3a2.tar", max compression
```

## Comparing `reflex-0.2.3a1.tar` & `reflex-0.2.3a2.tar`

### file list

```diff
@@ -1,178 +1,178 @@
--rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.3a1/LICENSE
--rw-r--r--   0        0        0     7766 2023-07-17 23:29:33.625723 reflex-0.2.3a1/README.md
--rw-r--r--   0        0        0     2002 2023-07-22 03:09:53.833732 reflex-0.2.3a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.3a1/reflex/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1337 2023-07-19 01:58:23.983993 reflex-0.2.3a1/reflex/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.3a1/reflex/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.3a1/reflex/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.3a1/reflex/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.3a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.3a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.3a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.3a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.3a1/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.3a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.3a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.3a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.3a1/reflex/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.3a1/reflex/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.3a1/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       65 2023-07-21 22:05:26.060616 reflex-0.2.3a1/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0     1287 2023-07-20 20:03:35.347093 reflex-0.2.3a1/reflex/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-07-21 22:29:32.048334 reflex-0.2.3a1/reflex/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.3a1/reflex/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.3a1/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.3a1/reflex/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.3a1/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0    10127 2023-07-21 18:51:53.047150 reflex-0.2.3a1/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1965 2023-07-19 01:58:26.538410 reflex-0.2.3a1/reflex/__init__.py
--rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.3a1/reflex/admin.py
--rw-r--r--   0        0        0    24459 2023-07-21 20:03:39.530167 reflex-0.2.3a1/reflex/app.py
--rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.3a1/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.3a1/reflex/compiler/__init__.py
--rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.3a1/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     2725 2023-07-22 03:01:43.547546 reflex-0.2.3a1/reflex/compiler/templates.py
--rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.3a1/reflex/compiler/utils.py
--rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.3a1/reflex/components/__init__.py
--rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.3a1/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.3a1/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.3a1/reflex/components/base/body.py
--rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.3a1/reflex/components/base/document.py
--rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.3a1/reflex/components/base/head.py
--rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.3a1/reflex/components/base/link.py
--rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.3a1/reflex/components/base/meta.py
--rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.3a1/reflex/components/base/script.py
--rw-r--r--   0        0        0    24321 2023-07-22 03:01:43.547958 reflex-0.2.3a1/reflex/components/component.py
--rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.3a1/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.3a1/reflex/components/datadisplay/badge.py
--rw-r--r--   0        0        0     3495 2023-07-22 03:01:43.548095 reflex-0.2.3a1/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0     3951 2023-07-21 18:51:53.047714 reflex-0.2.3a1/reflex/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.3a1/reflex/components/datadisplay/divider.py
--rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.3a1/reflex/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.3a1/reflex/components/datadisplay/list.py
--rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.3a1/reflex/components/datadisplay/stat.py
--rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.3a1/reflex/components/datadisplay/table.py
--rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.3a1/reflex/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.3a1/reflex/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.3a1/reflex/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.3a1/reflex/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.3a1/reflex/components/disclosure/transition.py
--rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.3a1/reflex/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.3a1/reflex/components/feedback/__init__.py
--rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.3a1/reflex/components/feedback/alert.py
--rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.3a1/reflex/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.3a1/reflex/components/feedback/progress.py
--rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.3a1/reflex/components/feedback/skeleton.py
--rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.3a1/reflex/components/feedback/spinner.py
--rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.3a1/reflex/components/forms/__init__.py
--rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.3a1/reflex/components/forms/button.py
--rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.3a1/reflex/components/forms/checkbox.py
--rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.3a1/reflex/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.3a1/reflex/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.3a1/reflex/components/forms/date_picker.py
--rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.3a1/reflex/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.3a1/reflex/components/forms/debounce.py
--rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.3a1/reflex/components/forms/editable.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.3a1/reflex/components/forms/email.py
--rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.3a1/reflex/components/forms/form.py
--rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.3a1/reflex/components/forms/iconbutton.py
--rw-r--r--   0        0        0     3246 2023-07-21 23:52:40.428089 reflex-0.2.3a1/reflex/components/forms/input.py
--rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.3a1/reflex/components/forms/multiselect.py
--rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.3a1/reflex/components/forms/numberinput.py
--rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.3a1/reflex/components/forms/password.py
--rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.3a1/reflex/components/forms/pininput.py
--rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.3a1/reflex/components/forms/radio.py
--rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.3a1/reflex/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.3a1/reflex/components/forms/select.py
--rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.3a1/reflex/components/forms/slider.py
--rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.3a1/reflex/components/forms/switch.py
--rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.3a1/reflex/components/forms/textarea.py
--rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.3a1/reflex/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.3a1/reflex/components/graphing/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.3a1/reflex/components/graphing/plotly.py
--rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.3a1/reflex/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.3a1/reflex/components/layout/__init__.py
--rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.3a1/reflex/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.3a1/reflex/components/layout/box.py
--rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.3a1/reflex/components/layout/card.py
--rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.3a1/reflex/components/layout/center.py
--rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.3a1/reflex/components/layout/cond.py
--rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.3a1/reflex/components/layout/container.py
--rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.3a1/reflex/components/layout/flex.py
--rw-r--r--   0        0        0     3159 2023-07-22 02:58:05.741564 reflex-0.2.3a1/reflex/components/layout/foreach.py
--rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.3a1/reflex/components/layout/fragment.py
--rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.3a1/reflex/components/layout/grid.py
--rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.3a1/reflex/components/layout/html.py
--rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.3a1/reflex/components/layout/responsive.py
--rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.3a1/reflex/components/layout/spacer.py
--rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.3a1/reflex/components/layout/stack.py
--rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.3a1/reflex/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.3a1/reflex/components/libs/__init__.py
--rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.3a1/reflex/components/libs/chakra.py
--rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.3a1/reflex/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.3a1/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.3a1/reflex/components/media/audio.py
--rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.3a1/reflex/components/media/avatar.py
--rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.3a1/reflex/components/media/icon.py
--rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.3a1/reflex/components/media/image.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.3a1/reflex/components/media/video.py
--rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.3a1/reflex/components/navigation/__init__.py
--rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.3a1/reflex/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.3a1/reflex/components/navigation/link.py
--rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.3a1/reflex/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.3a1/reflex/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.3a1/reflex/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.3a1/reflex/components/overlay/__init__.py
--rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.3a1/reflex/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.3a1/reflex/components/overlay/banner.py
--rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.3a1/reflex/components/overlay/drawer.py
--rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.3a1/reflex/components/overlay/menu.py
--rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.3a1/reflex/components/overlay/modal.py
--rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.3a1/reflex/components/overlay/popover.py
--rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.3a1/reflex/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.3a1/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.3a1/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-07-22 03:09:31.906614 reflex-0.2.3a1/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5008 2023-07-22 03:01:43.548457 reflex-0.2.3a1/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.3a1/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.3a1/reflex/components/typography/__init__.py
--rw-r--r--   0        0        0      278 2023-07-14 23:13:37.779315 reflex-0.2.3a1/reflex/components/typography/heading.py
--rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.3a1/reflex/components/typography/highlight.py
--rw-r--r--   0        0        0     3593 2023-07-22 03:01:43.548609 reflex-0.2.3a1/reflex/components/typography/markdown.py
--rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.3a1/reflex/components/typography/span.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.3a1/reflex/components/typography/text.py
--rw-r--r--   0        0        0     7692 2023-07-20 20:03:35.349661 reflex-0.2.3a1/reflex/config.py
--rw-r--r--   0        0        0    11209 2023-07-21 18:51:53.047891 reflex-0.2.3a1/reflex/constants.py
--rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.3a1/reflex/el/__init__.py
--rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.3a1/reflex/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.3a1/reflex/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.3a1/reflex/el/constants/react.py
--rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.3a1/reflex/el/constants/reflex.py
--rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.3a1/reflex/el/element.py
--rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.3a1/reflex/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.3a1/reflex/el/precompile.py
--rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.3a1/reflex/event.py
--rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.3a1/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.3a1/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.3a1/reflex/middleware/middleware.py
--rw-r--r--   0        0        0     9604 2023-07-19 23:09:19.472388 reflex-0.2.3a1/reflex/model.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.3a1/reflex/py.typed
--rw-r--r--   0        0        0    11041 2023-07-21 22:29:32.048533 reflex-0.2.3a1/reflex/reflex.py
--rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.3a1/reflex/route.py
--rw-r--r--   0        0        0    32118 2023-07-21 18:51:53.048117 reflex-0.2.3a1/reflex/state.py
--rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.3a1/reflex/style.py
--rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.3a1/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.3a1/reflex/utils/__init__.py
--rw-r--r--   0        0        0     7971 2023-07-20 20:03:35.350159 reflex-0.2.3a1/reflex/utils/build.py
--rw-r--r--   0        0        0     1692 2023-07-19 01:58:26.541439 reflex-0.2.3a1/reflex/utils/console.py
--rw-r--r--   0        0        0     4225 2023-07-17 23:29:33.628283 reflex-0.2.3a1/reflex/utils/exec.py
--rw-r--r--   0        0        0    11845 2023-07-21 23:46:28.128377 reflex-0.2.3a1/reflex/utils/format.py
--rw-r--r--   0        0        0      585 2023-07-14 23:13:37.782125 reflex-0.2.3a1/reflex/utils/imports.py
--rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.3a1/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    14208 2023-07-21 18:51:53.048319 reflex-0.2.3a1/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     4105 2023-07-17 23:29:33.628618 reflex-0.2.3a1/reflex/utils/processes.py
--rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.3a1/reflex/utils/telemetry.py
--rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.3a1/reflex/utils/types.py
--rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.3a1/reflex/utils/watch.py
--rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.3a1/reflex/vars.py
--rw-r--r--   0        0        0     9586 1970-01-01 00:00:00.000000 reflex-0.2.3a1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.3a2/LICENSE
+-rw-r--r--   0        0        0     7905 2023-07-25 18:50:56.099599 reflex-0.2.3a2/README.md
+-rw-r--r--   0        0        0     2002 2023-07-25 20:27:30.669223 reflex-0.2.3a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.3a2/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1337 2023-07-19 01:58:23.983993 reflex-0.2.3a2/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.3a2/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.3a2/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.3a2/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.3a2/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.3a2/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.3a2/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.3a2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.3a2/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.3a2/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.3a2/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.3a2/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.3a2/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.3a2/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.3a2/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       65 2023-07-21 22:05:26.060616 reflex-0.2.3a2/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1287 2023-07-23 00:56:20.970158 reflex-0.2.3a2/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-07-21 22:29:32.048334 reflex-0.2.3a2/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.3a2/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.3a2/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.3a2/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.3a2/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0    10127 2023-07-21 18:51:53.047150 reflex-0.2.3a2/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1965 2023-07-19 01:58:26.538410 reflex-0.2.3a2/reflex/__init__.py
+-rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.3a2/reflex/admin.py
+-rw-r--r--   0        0        0    24459 2023-07-21 20:03:39.530167 reflex-0.2.3a2/reflex/app.py
+-rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.3a2/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.3a2/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.3a2/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-07-25 18:39:55.667575 reflex-0.2.3a2/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.3a2/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.3a2/reflex/components/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.3a2/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.3a2/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.3a2/reflex/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.3a2/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.3a2/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.3a2/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.3a2/reflex/components/base/meta.py
+-rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.3a2/reflex/components/base/script.py
+-rw-r--r--   0        0        0    24321 2023-07-25 18:39:55.676277 reflex-0.2.3a2/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.3a2/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.3a2/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     3495 2023-07-25 18:39:55.680665 reflex-0.2.3a2/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     3951 2023-07-21 18:51:53.047714 reflex-0.2.3a2/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.3a2/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.3a2/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.3a2/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.3a2/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.3a2/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.3a2/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.3a2/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.3a2/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.3a2/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.3a2/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.3a2/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.3a2/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.3a2/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.3a2/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.3a2/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.3a2/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.3a2/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.3a2/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.3a2/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.3a2/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.3a2/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.3a2/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.3a2/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.3a2/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.3a2/reflex/components/forms/debounce.py
+-rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.3a2/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.3a2/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.3a2/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.3a2/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     3246 2023-07-21 23:52:40.428089 reflex-0.2.3a2/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.3a2/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.3a2/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.3a2/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.3a2/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.3a2/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.3a2/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.3a2/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.3a2/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.3a2/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.3a2/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.3a2/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.3a2/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.3a2/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.3a2/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.3a2/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.3a2/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.3a2/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.3a2/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.3a2/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.3a2/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.3a2/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.3a2/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-07-22 02:58:05.741564 reflex-0.2.3a2/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.3a2/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.3a2/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.3a2/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.3a2/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.3a2/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.3a2/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.3a2/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.3a2/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.3a2/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.3a2/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.3a2/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.3a2/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.3a2/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.3a2/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.3a2/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.3a2/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.3a2/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.3a2/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.3a2/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.3a2/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.3a2/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.3a2/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.3a2/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.3a2/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.3a2/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.3a2/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.3a2/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.3a2/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.3a2/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.3a2/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.3a2/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.3a2/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-07-24 16:26:04.843847 reflex-0.2.3a2/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5008 2023-07-25 18:50:56.099830 reflex-0.2.3a2/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.3a2/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.3a2/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      278 2023-07-25 18:50:56.099969 reflex-0.2.3a2/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.3a2/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     3593 2023-07-25 18:50:56.100332 reflex-0.2.3a2/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.3a2/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.3a2/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7564 2023-07-25 20:26:59.826284 reflex-0.2.3a2/reflex/config.py
+-rw-r--r--   0        0        0    11900 2023-07-25 20:07:33.016303 reflex-0.2.3a2/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.3a2/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.3a2/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.3a2/reflex/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.3a2/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.3a2/reflex/el/constants/reflex.py
+-rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.3a2/reflex/el/element.py
+-rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.3a2/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.3a2/reflex/el/precompile.py
+-rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.3a2/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.3a2/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.3a2/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.3a2/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     9604 2023-07-19 23:09:19.472388 reflex-0.2.3a2/reflex/model.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.3a2/reflex/py.typed
+-rw-r--r--   0        0        0    10559 2023-07-25 19:40:15.401052 reflex-0.2.3a2/reflex/reflex.py
+-rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.3a2/reflex/route.py
+-rw-r--r--   0        0        0    32118 2023-07-21 18:51:53.048117 reflex-0.2.3a2/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.3a2/reflex/style.py
+-rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.3a2/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.3a2/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     7868 2023-07-25 19:38:10.257733 reflex-0.2.3a2/reflex/utils/build.py
+-rw-r--r--   0        0        0     1692 2023-07-19 01:58:26.541439 reflex-0.2.3a2/reflex/utils/console.py
+-rw-r--r--   0        0        0     4181 2023-07-25 18:50:56.101998 reflex-0.2.3a2/reflex/utils/exec.py
+-rw-r--r--   0        0        0    11845 2023-07-21 23:46:28.128377 reflex-0.2.3a2/reflex/utils/format.py
+-rw-r--r--   0        0        0      585 2023-07-14 23:13:37.782125 reflex-0.2.3a2/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.3a2/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    14196 2023-07-25 20:26:59.823656 reflex-0.2.3a2/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     4200 2023-07-25 20:22:27.923152 reflex-0.2.3a2/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.3a2/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.3a2/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.3a2/reflex/utils/watch.py
+-rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.3a2/reflex/vars.py
+-rw-r--r--   0        0        0     9725 1970-01-01 00:00:00.000000 reflex-0.2.3a2/PKG-INFO
```

### Comparing `reflex-0.2.3a1/LICENSE` & `reflex-0.2.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/README.md` & `reflex-0.2.3a2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -52,435 +52,444 @@
 00000330: 3f63 6f6c 6f72 3d25 3233 3732 3839 6461  ?color=%237289da
 00000340: 266c 6162 656c 3d44 6973 636f 7264 295d  &label=Discord)]
 00000350: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
 00000360: 2e67 672f 5435 5753 6243 3259 7451 290a  .gg/T5WSbC2YtQ).
 00000370: 0a3c 2f64 6976 3e0a 0a23 2323 2052 4541  .</div>..### REA
 00000380: 444d 4520 696e 2064 6966 6665 7265 6e74  DME in different
 00000390: 206c 616e 6775 6167 650a 0a2d 2d2d 0a0a   language..---..
-000003a0: 5b45 6e67 6c69 7368 5d28 5245 4144 4d45  [English](README
-000003b0: 2e6d 6429 207c 205b e7ae 80e4 bd93 e4b8  .md) | [........
-000003c0: ade6 9687 5d28 2f64 6f63 732f 7a68 2f7a  ....](/docs/zh/z
-000003d0: 685f 636e 2f52 4541 444d 452e 6d64 2920  h_cn/README.md) 
-000003e0: 7c20 5be7 b981 e9ab 94e4 b8ad e696 875d  | [............]
-000003f0: 282f 646f 6373 2f7a 682f 7a68 5f74 772f  (/docs/zh/zh_tw/
-00000400: 5245 4144 4d45 2e6d 6429 0a0a 2d2d 2d0a  README.md)..---.
-00000410: 0a23 2320 f09f 93a6 2031 2e20 496e 7374  .## .... 1. Inst
-00000420: 616c 6c0a 0a52 6566 6c65 7820 7265 7175  all..Reflex requ
-00000430: 6972 6573 2074 6865 2066 6f6c 6c6f 7769  ires the followi
-00000440: 6e67 2074 6f20 6765 7420 7374 6172 7465  ng to get starte
-00000450: 643a 0a0a 2d20 2020 5079 7468 6f6e 2033  d:..-   Python 3
-00000460: 2e37 2b0a 2d20 2020 5b4e 6f64 652e 6a73  .7+.-   [Node.js
-00000470: 2031 362e 382e 302b 5d28 6874 7470 733a   16.8.0+](https:
-00000480: 2f2f 6e6f 6465 6a73 2e6f 7267 2f65 6e2f  //nodejs.org/en/
-00000490: 2920 2844 6f6e 2774 2077 6f72 7279 2c20  ) (Don't worry, 
-000004a0: 796f 7520 776f 6ee2 8099 7420 6861 7665  you won...t have
-000004b0: 2074 6f20 7772 6974 6520 616e 7920 4a61   to write any Ja
-000004c0: 7661 5363 7269 7074 2129 0a0a 6060 600a  vaScript!)..```.
-000004d0: 7069 7020 696e 7374 616c 6c20 7265 666c  pip install refl
-000004e0: 6578 0a60 6060 0a0a 2323 20f0 9fa5 b320  ex.```..## .... 
-000004f0: 322e 2043 7265 6174 6520 796f 7572 2066  2. Create your f
-00000500: 6972 7374 2061 7070 0a0a 496e 7374 616c  irst app..Instal
-00000510: 6c69 6e67 2060 7265 666c 6578 6020 616c  ling `reflex` al
-00000520: 736f 2069 6e73 7461 6c6c 7320 7468 6520  so installs the 
-00000530: 6072 6566 6c65 7860 2063 6f6d 6d61 6e64  `reflex` command
-00000540: 206c 696e 6520 746f 6f6c 2e20 5465 7374   line tool. Test
-00000550: 2074 6861 7420 7468 6520 696e 7374 616c   that the instal
-00000560: 6c20 7761 7320 7375 6363 6573 7366 756c  l was successful
-00000570: 2062 7920 6372 6561 7469 6e67 2061 206e   by creating a n
-00000580: 6577 2070 726f 6a65 6374 2e0a 0a52 6570  ew project...Rep
-00000590: 6c61 6365 206d 795f 6170 705f 6e61 6d65  lace my_app_name
-000005a0: 2077 6974 6820 796f 7572 2070 726f 6a65   with your proje
-000005b0: 6374 206e 616d 653a 0a0a 6060 600a 6d6b  ct name:..```.mk
-000005c0: 6469 7220 6d79 5f61 7070 5f6e 616d 650a  dir my_app_name.
-000005d0: 6364 206d 795f 6170 705f 6e61 6d65 0a72  cd my_app_name.r
-000005e0: 6566 6c65 7820 696e 6974 0a60 6060 0a0a  eflex init.```..
-000005f0: 5768 656e 2079 6f75 2072 756e 2074 6869  When you run thi
-00000600: 7320 636f 6d6d 616e 6420 666f 7220 7468  s command for th
-00000610: 6520 6669 7273 7420 7469 6d65 2c20 7765  e first time, we
-00000620: 2077 696c 6c20 646f 776e 6c6f 6164 2061   will download a
-00000630: 6e64 2069 6e73 7461 6c6c 205b 6275 6e5d  nd install [bun]
-00000640: 2868 7474 7073 3a2f 2f62 756e 2e73 682f  (https://bun.sh/
-00000650: 2920 6175 746f 6d61 7469 6361 6c6c 792e  ) automatically.
-00000660: 0a0a 5468 6973 2063 6f6d 6d61 6e64 2069  ..This command i
-00000670: 6e69 7469 616c 697a 6573 2061 2074 656d  nitializes a tem
-00000680: 706c 6174 6520 6170 7020 696e 2079 6f75  plate app in you
-00000690: 7220 6e65 7720 6469 7265 6374 6f72 792e  r new directory.
-000006a0: 0a0a 2323 20f0 9f8f 8320 332e 2052 756e  ..## .... 3. Run
-000006b0: 2079 6f75 7220 6170 700a 0a59 6f75 2063   your app..You c
-000006c0: 616e 2072 756e 2074 6869 7320 6170 7020  an run this app 
-000006d0: 696e 2064 6576 656c 6f70 6d65 6e74 206d  in development m
-000006e0: 6f64 653a 0a0a 6060 600a 7265 666c 6578  ode:..```.reflex
-000006f0: 2072 756e 0a60 6060 0a0a 596f 7520 7368   run.```..You sh
-00000700: 6f75 6c64 2073 6565 2079 6f75 7220 6170  ould see your ap
-00000710: 7020 7275 6e6e 696e 6720 6174 2068 7474  p running at htt
-00000720: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
-00000730: 3030 2e0a 0a4e 6f77 2079 6f75 2063 616e  00...Now you can
-00000740: 206d 6f64 6966 7920 7468 6520 736f 7572   modify the sour
-00000750: 6365 2063 6f64 6520 696e 2060 6d79 5f61  ce code in `my_a
-00000760: 7070 5f6e 616d 652f 6d79 5f61 7070 5f6e  pp_name/my_app_n
-00000770: 616d 652e 7079 602e 2052 6566 6c65 7820  ame.py`. Reflex 
-00000780: 6861 7320 6661 7374 2072 6566 7265 7368  has fast refresh
-00000790: 6573 2073 6f20 796f 7520 6361 6e20 7365  es so you can se
-000007a0: 6520 796f 7572 2063 6861 6e67 6573 2069  e your changes i
-000007b0: 6e73 7461 6e74 6c79 2077 6865 6e20 796f  nstantly when yo
-000007c0: 7520 7361 7665 2079 6f75 7220 636f 6465  u save your code
-000007d0: 2e0a 0a23 2320 f09f aba7 2045 7861 6d70  ...## .... Examp
-000007e0: 6c65 0a0a 4c65 7427 7320 676f 206f 7665  le..Let's go ove
-000007f0: 7220 616e 2065 7861 6d70 6c65 3a20 6372  r an example: cr
-00000800: 6561 7469 6e67 2061 6e20 696d 6167 6520  eating an image 
-00000810: 6765 6e65 7261 7469 6f6e 2055 4920 6172  generation UI ar
-00000820: 6f75 6e64 2044 414c 4cc2 b745 2e20 466f  ound DALL..E. Fo
-00000830: 7220 7369 6d70 6c69 6369 7479 2c20 7765  r simplicity, we
-00000840: 206a 7573 7420 6361 6c6c 2074 6865 204f   just call the O
-00000850: 7065 6e41 4920 4150 492c 2062 7574 2079  penAI API, but y
-00000860: 6f75 2063 6f75 6c64 2072 6570 6c61 6365  ou could replace
-00000870: 2074 6869 7320 7769 7468 2061 6e20 4d4c   this with an ML
-00000880: 206d 6f64 656c 2072 756e 206c 6f63 616c   model run local
-00000890: 6c79 2e0a 0a26 6e62 7370 3b0a 0a3c 6469  ly...&nbsp;..<di
-000008a0: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-000008b0: 3e0a 3c69 6d67 2073 7263 3d22 646f 6373  >.<img src="docs
-000008c0: 2f69 6d61 6765 732f 6461 6c6c 652e 6769  /images/dalle.gi
-000008d0: 6622 2061 6c74 3d22 4120 6672 6f6e 7465  f" alt="A fronte
-000008e0: 6e64 2077 7261 7070 6572 2066 6f72 2044  nd wrapper for D
-000008f0: 414c 4cc2 b745 2c20 7368 6f77 6e20 696e  ALL..E, shown in
-00000900: 2074 6865 2070 726f 6365 7373 206f 6620   the process of 
-00000910: 6765 6e65 7261 7469 6e67 2061 6e20 696d  generating an im
-00000920: 6167 652e 2220 7769 6474 683d 2235 3530  age." width="550
-00000930: 2220 2f3e 0a3c 2f64 6976 3e0a 0a26 6e62  " />.</div>..&nb
-00000940: 7370 3b0a 0a48 6572 6520 6973 2074 6865  sp;..Here is the
-00000950: 2063 6f6d 706c 6574 6520 636f 6465 2074   complete code t
-00000960: 6f20 6372 6561 7465 2074 6869 732e 2054  o create this. T
-00000970: 6869 7320 6973 2061 6c6c 2064 6f6e 6520  his is all done 
-00000980: 696e 206f 6e65 2050 7974 686f 6e20 6669  in one Python fi
-00000990: 6c65 210a 0a60 6060 7079 7468 6f6e 0a69  le!..```python.i
-000009a0: 6d70 6f72 7420 7265 666c 6578 2061 7320  mport reflex as 
-000009b0: 7278 0a69 6d70 6f72 7420 6f70 656e 6169  rx.import openai
-000009c0: 0a0a 6f70 656e 6169 2e61 7069 5f6b 6579  ..openai.api_key
-000009d0: 203d 2022 594f 5552 5f41 5049 5f4b 4559   = "YOUR_API_KEY
-000009e0: 220a 0a63 6c61 7373 2053 7461 7465 2872  "..class State(r
-000009f0: 782e 5374 6174 6529 3a0a 2020 2020 2222  x.State):.    ""
-00000a00: 2254 6865 2061 7070 2073 7461 7465 2e22  "The app state."
-00000a10: 2222 0a20 2020 2070 726f 6d70 7420 3d20  "".    prompt = 
-00000a20: 2222 0a20 2020 2069 6d61 6765 5f75 726c  "".    image_url
-00000a30: 203d 2022 220a 2020 2020 7072 6f63 6573   = "".    proces
-00000a40: 7369 6e67 203d 2046 616c 7365 0a20 2020  sing = False.   
-00000a50: 2063 6f6d 706c 6574 6520 3d20 4661 6c73   complete = Fals
-00000a60: 650a 0a20 2020 2064 6566 2067 6574 5f69  e..    def get_i
-00000a70: 6d61 6765 2873 656c 6629 3a0a 2020 2020  mage(self):.    
-00000a80: 2020 2020 2222 2247 6574 2074 6865 2069      """Get the i
-00000a90: 6d61 6765 2066 726f 6d20 7468 6520 7072  mage from the pr
-00000aa0: 6f6d 7074 2e22 2222 0a20 2020 2020 2020  ompt.""".       
-00000ab0: 2069 6620 7365 6c66 2e70 726f 6d70 7420   if self.prompt 
-00000ac0: 3d3d 2022 223a 0a20 2020 2020 2020 2020  == "":.         
-00000ad0: 2020 2072 6574 7572 6e20 7278 2e77 696e     return rx.win
-00000ae0: 646f 775f 616c 6572 7428 2250 726f 6d70  dow_alert("Promp
-00000af0: 7420 456d 7074 7922 290a 0a20 2020 2020  t Empty")..     
-00000b00: 2020 2073 656c 662e 7072 6f63 6573 7369     self.processi
-00000b10: 6e67 2c20 7365 6c66 2e63 6f6d 706c 6574  ng, self.complet
-00000b20: 6520 3d20 5472 7565 2c20 4661 6c73 650a  e = True, False.
-00000b30: 2020 2020 2020 2020 7969 656c 640a 2020          yield.  
-00000b40: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00000b50: 206f 7065 6e61 692e 496d 6167 652e 6372   openai.Image.cr
-00000b60: 6561 7465 2870 726f 6d70 743d 7365 6c66  eate(prompt=self
-00000b70: 2e70 726f 6d70 742c 206e 3d31 2c20 7369  .prompt, n=1, si
-00000b80: 7a65 3d22 3130 3234 7831 3032 3422 290a  ze="1024x1024").
-00000b90: 2020 2020 2020 2020 7365 6c66 2e69 6d61          self.ima
-00000ba0: 6765 5f75 726c 203d 2072 6573 706f 6e73  ge_url = respons
-00000bb0: 655b 2264 6174 6122 5d5b 305d 5b22 7572  e["data"][0]["ur
-00000bc0: 6c22 5d0a 2020 2020 2020 2020 7365 6c66  l"].        self
-00000bd0: 2e70 726f 6365 7373 696e 672c 2073 656c  .processing, sel
-00000be0: 662e 636f 6d70 6c65 7465 203d 2046 616c  f.complete = Fal
-00000bf0: 7365 2c20 5472 7565 0a20 2020 2020 2020  se, True.       
-00000c00: 200a 0a64 6566 2069 6e64 6578 2829 3a0a   ..def index():.
-00000c10: 2020 2020 7265 7475 726e 2072 782e 6365      return rx.ce
-00000c20: 6e74 6572 280a 2020 2020 2020 2020 7278  nter(.        rx
-00000c30: 2e76 7374 6163 6b28 0a20 2020 2020 2020  .vstack(.       
-00000c40: 2020 2020 2072 782e 6865 6164 696e 6728       rx.heading(
-00000c50: 2244 414c 4cc2 b745 2229 2c0a 2020 2020  "DALL..E"),.    
-00000c60: 2020 2020 2020 2020 7278 2e69 6e70 7574          rx.input
-00000c70: 2870 6c61 6365 686f 6c64 6572 3d22 456e  (placeholder="En
-00000c80: 7465 7220 6120 7072 6f6d 7074 222c 206f  ter a prompt", o
-00000c90: 6e5f 626c 7572 3d53 7461 7465 2e73 6574  n_blur=State.set
-00000ca0: 5f70 726f 6d70 7429 2c0a 2020 2020 2020  _prompt),.      
-00000cb0: 2020 2020 2020 7278 2e62 7574 746f 6e28        rx.button(
-00000cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000cd0: 2022 4765 6e65 7261 7465 2049 6d61 6765   "Generate Image
-00000ce0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000cf0: 2020 206f 6e5f 636c 6963 6b3d 5374 6174     on_click=Stat
-00000d00: 652e 6765 745f 696d 6167 652c 0a20 2020  e.get_image,.   
-00000d10: 2020 2020 2020 2020 2020 2020 2069 735f               is_
-00000d20: 6c6f 6164 696e 673d 5374 6174 652e 7072  loading=State.pr
-00000d30: 6f63 6573 7369 6e67 2c0a 2020 2020 2020  ocessing,.      
-00000d40: 2020 2020 2020 2020 2020 7769 6474 683d            width=
-00000d50: 2231 3030 2522 2c0a 2020 2020 2020 2020  "100%",.        
-00000d60: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00000d70: 2020 2072 782e 636f 6e64 280a 2020 2020     rx.cond(.    
-00000d80: 2020 2020 2020 2020 2020 2020 5374 6174              Stat
-00000d90: 652e 636f 6d70 6c65 7465 2c0a 2020 2020  e.complete,.    
-00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000db0: 2072 782e 696d 6167 6528 0a20 2020 2020   rx.image(.     
-00000dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dd0: 2020 2020 7372 633d 5374 6174 652e 696d      src=State.im
-00000de0: 6167 655f 7572 6c2c 0a20 2020 2020 2020  age_url,.       
-00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e00: 2020 6865 6967 6874 3d22 3235 656d 222c    height="25em",
-00000e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e20: 2020 2020 2020 2020 2020 7769 6474 683d            width=
-00000e30: 2232 3565 6d22 2c0a 2020 2020 2020 2020  "25em",.        
-00000e40: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00000e50: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00000e60: 2020 2020 2020 2020 2070 6164 6469 6e67           padding
-00000e70: 3d22 3265 6d22 2c0a 2020 2020 2020 2020  ="2em",.        
-00000e80: 2020 2020 7368 6164 6f77 3d22 6c67 222c      shadow="lg",
-00000e90: 0a20 2020 2020 2020 2020 2020 2062 6f72  .            bor
-00000ea0: 6465 725f 7261 6469 7573 3d22 6c67 222c  der_radius="lg",
-00000eb0: 0a20 2020 2020 2020 2029 2c0a 2020 2020  .        ),.    
-00000ec0: 2020 2020 7769 6474 683d 2231 3030 2522      width="100%"
-00000ed0: 2c0a 2020 2020 2020 2020 6865 6967 6874  ,.        height
-00000ee0: 3d22 3130 3076 6822 2c0a 2020 2020 290a  ="100vh",.    ).
-00000ef0: 0a23 2041 6464 2073 7461 7465 2061 6e64  .# Add state and
-00000f00: 2070 6167 6520 746f 2074 6865 2061 7070   page to the app
-00000f10: 2e0a 6170 7020 3d20 7278 2e41 7070 2873  ..app = rx.App(s
-00000f20: 7461 7465 3d53 7461 7465 290a 6170 702e  tate=State).app.
-00000f30: 6164 645f 7061 6765 2869 6e64 6578 2c20  add_page(index, 
-00000f40: 7469 746c 653d 2272 6566 6c65 783a 4441  title="reflex:DA
-00000f50: 4c4c c2b7 4522 290a 6170 702e 636f 6d70  LL..E").app.comp
-00000f60: 696c 6528 290a 6060 600a 0a4c 6574 2773  ile().```..Let's
-00000f70: 2062 7265 616b 2074 6869 7320 646f 776e   break this down
-00000f80: 2e0a 0a23 2323 202a 2a55 4920 496e 2052  ...### **UI In R
-00000f90: 6566 6c65 782a 2a0a 0a4c 6574 2773 2073  eflex**..Let's s
-00000fa0: 7461 7274 2077 6974 6820 7468 6520 5549  tart with the UI
-00000fb0: 2e0a 0a60 6060 7079 7468 6f6e 0a64 6566  ...```python.def
-00000fc0: 2069 6e64 6578 2829 3a0a 2020 2020 7265   index():.    re
-00000fd0: 7475 726e 2072 782e 6365 6e74 6572 280a  turn rx.center(.
-00000fe0: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
-00000ff0: 290a 6060 600a 0a54 6869 7320 6069 6e64  ).```..This `ind
-00001000: 6578 6020 6675 6e63 7469 6f6e 2064 6566  ex` function def
-00001010: 696e 6573 2074 6865 2066 726f 6e74 656e  ines the fronten
-00001020: 6420 6f66 2074 6865 2061 7070 2e0a 0a57  d of the app...W
-00001030: 6520 7573 6520 6469 6666 6572 656e 7420  e use different 
-00001040: 636f 6d70 6f6e 656e 7473 2073 7563 6820  components such 
-00001050: 6173 2060 6365 6e74 6572 602c 2060 7673  as `center`, `vs
-00001060: 7461 636b 602c 2060 696e 7075 7460 2c20  tack`, `input`, 
-00001070: 616e 6420 6062 7574 746f 6e60 2074 6f20  and `button` to 
-00001080: 6275 696c 6420 7468 6520 6672 6f6e 7465  build the fronte
-00001090: 6e64 2e20 436f 6d70 6f6e 656e 7473 2063  nd. Components c
-000010a0: 616e 2062 6520 6e65 7374 6564 2077 6974  an be nested wit
-000010b0: 6869 6e20 6561 6368 206f 7468 6572 0a74  hin each other.t
-000010c0: 6f20 6372 6561 7465 2063 6f6d 706c 6578  o create complex
-000010d0: 206c 6179 6f75 7473 2e20 416e 6420 796f   layouts. And yo
-000010e0: 7520 6361 6e20 7573 6520 6b65 7977 6f72  u can use keywor
-000010f0: 6420 6172 6773 2074 6f20 7374 796c 6520  d args to style 
-00001100: 7468 656d 2077 6974 6820 7468 6520 6675  them with the fu
-00001110: 6c6c 2070 6f77 6572 206f 6620 4353 532e  ll power of CSS.
-00001120: 0a0a 5265 666c 6578 2063 6f6d 6573 2077  ..Reflex comes w
-00001130: 6974 6820 5b36 302b 2062 7569 6c74 2d69  ith [60+ built-i
-00001140: 6e20 636f 6d70 6f6e 656e 7473 5d28 6874  n components](ht
-00001150: 7470 733a 2f2f 7265 666c 6578 2e64 6576  tps://reflex.dev
-00001160: 2f64 6f63 732f 6c69 6272 6172 7929 2074  /docs/library) t
-00001170: 6f20 6865 6c70 2079 6f75 2067 6574 2073  o help you get s
-00001180: 7461 7274 6564 2e20 5765 2061 7265 2061  tarted. We are a
-00001190: 6374 6976 656c 7920 6164 6469 6e67 206d  ctively adding m
-000011a0: 6f72 6520 636f 6d70 6f6e 656e 7473 2c20  ore components, 
-000011b0: 616e 6420 6974 2773 2065 6173 7920 746f  and it's easy to
-000011c0: 205b 6372 6561 7465 2079 6f75 7220 6f77   [create your ow
-000011d0: 6e20 636f 6d70 6f6e 656e 7473 5d28 6874  n components](ht
-000011e0: 7470 733a 2f2f 7265 666c 6578 2e64 6576  tps://reflex.dev
-000011f0: 2f64 6f63 732f 6164 7661 6e63 6564 2d67  /docs/advanced-g
-00001200: 7569 6465 2f77 7261 7070 696e 672d 7265  uide/wrapping-re
-00001210: 6163 7429 2e0a 0a23 2323 202a 2a53 7461  act)...### **Sta
-00001220: 7465 2a2a 0a0a 5265 666c 6578 2072 6570  te**..Reflex rep
-00001230: 7265 7365 6e74 7320 796f 7572 2055 4920  resents your UI 
-00001240: 6173 2061 2066 756e 6374 696f 6e20 6f66  as a function of
-00001250: 2079 6f75 7220 7374 6174 652e 0a0a 6060   your state...``
-00001260: 6070 7974 686f 6e0a 636c 6173 7320 5374  `python.class St
-00001270: 6174 6528 7278 2e53 7461 7465 293a 0a20  ate(rx.State):. 
-00001280: 2020 2022 2222 5468 6520 6170 7020 7374     """The app st
-00001290: 6174 652e 2222 220a 2020 2020 7072 6f6d  ate.""".    prom
-000012a0: 7074 203d 2022 220a 2020 2020 696d 6167  pt = "".    imag
-000012b0: 655f 7572 6c20 3d20 2222 0a20 2020 2070  e_url = "".    p
-000012c0: 726f 6365 7373 696e 6720 3d20 4661 6c73  rocessing = Fals
-000012d0: 650a 2020 2020 636f 6d70 6c65 7465 203d  e.    complete =
-000012e0: 2046 616c 7365 0a60 6060 0a0a 5468 6520   False.```..The 
-000012f0: 7374 6174 6520 6465 6669 6e65 7320 616c  state defines al
-00001300: 6c20 7468 6520 7661 7269 6162 6c65 7320  l the variables 
-00001310: 2863 616c 6c65 6420 7661 7273 2920 696e  (called vars) in
-00001320: 2061 6e20 6170 7020 7468 6174 2063 616e   an app that can
-00001330: 2063 6861 6e67 6520 616e 6420 7468 6520   change and the 
-00001340: 6675 6e63 7469 6f6e 7320 7468 6174 2063  functions that c
-00001350: 6861 6e67 6520 7468 656d 2e0a 0a48 6572  hange them...Her
-00001360: 6520 7468 6520 7374 6174 6520 6973 2063  e the state is c
-00001370: 6f6d 7072 6973 6564 206f 6620 6120 6070  omprised of a `p
-00001380: 726f 6d70 7460 2061 6e64 2060 696d 6167  rompt` and `imag
-00001390: 655f 7572 6c60 2e20 5468 6572 6520 6172  e_url`. There ar
-000013a0: 6520 616c 736f 2074 6865 2062 6f6f 6c65  e also the boole
-000013b0: 616e 7320 6070 726f 6365 7373 696e 6760  ans `processing`
-000013c0: 2061 6e64 2060 636f 6d70 6c65 7465 6020   and `complete` 
-000013d0: 746f 2069 6e64 6963 6174 6520 7768 656e  to indicate when
-000013e0: 2074 6f20 7368 6f77 2074 6865 2063 6972   to show the cir
-000013f0: 6375 6c61 7220 7072 6f67 7265 7373 2061  cular progress a
-00001400: 6e64 2069 6d61 6765 2e0a 0a23 2323 202a  nd image...### *
-00001410: 2a45 7665 6e74 2048 616e 646c 6572 732a  *Event Handlers*
-00001420: 2a0a 0a60 6060 7079 7468 6f6e 0a64 6566  *..```python.def
-00001430: 2067 6574 5f69 6d61 6765 2873 656c 6629   get_image(self)
-00001440: 3a0a 2020 2020 2222 2247 6574 2074 6865  :.    """Get the
-00001450: 2069 6d61 6765 2066 726f 6d20 7468 6520   image from the 
-00001460: 7072 6f6d 7074 2e22 2222 0a20 2020 2069  prompt.""".    i
-00001470: 6620 7365 6c66 2e70 726f 6d70 7420 3d3d  f self.prompt ==
-00001480: 2022 223a 0a20 2020 2020 2020 2072 6574   "":.        ret
-00001490: 7572 6e20 7278 2e77 696e 646f 775f 616c  urn rx.window_al
-000014a0: 6572 7428 2250 726f 6d70 7420 456d 7074  ert("Prompt Empt
-000014b0: 7922 290a 0a20 2020 2073 656c 662e 7072  y")..    self.pr
-000014c0: 6f63 6573 7369 6e67 2c20 7365 6c66 2e63  ocessing, self.c
-000014d0: 6f6d 706c 6574 6520 3d20 5472 7565 2c20  omplete = True, 
-000014e0: 4661 6c73 650a 2020 2020 7969 656c 640a  False.    yield.
-000014f0: 2020 2020 7265 7370 6f6e 7365 203d 206f      response = o
-00001500: 7065 6e61 692e 496d 6167 652e 6372 6561  penai.Image.crea
-00001510: 7465 2870 726f 6d70 743d 7365 6c66 2e70  te(prompt=self.p
-00001520: 726f 6d70 742c 206e 3d31 2c20 7369 7a65  rompt, n=1, size
-00001530: 3d22 3130 3234 7831 3032 3422 290a 2020  ="1024x1024").  
-00001540: 2020 7365 6c66 2e69 6d61 6765 5f75 726c    self.image_url
-00001550: 203d 2072 6573 706f 6e73 655b 2264 6174   = response["dat
-00001560: 6122 5d5b 305d 5b22 7572 6c22 5d0a 2020  a"][0]["url"].  
-00001570: 2020 7365 6c66 2e70 726f 6365 7373 696e    self.processin
-00001580: 672c 2073 656c 662e 636f 6d70 6c65 7465  g, self.complete
-00001590: 203d 2046 616c 7365 2c20 5472 7565 0a60   = False, True.`
-000015a0: 6060 0a0a 5769 7468 696e 2074 6865 2073  ``..Within the s
-000015b0: 7461 7465 2c20 7765 2064 6566 696e 6520  tate, we define 
-000015c0: 6675 6e63 7469 6f6e 7320 6361 6c6c 6564  functions called
-000015d0: 2065 7665 6e74 2068 616e 646c 6572 7320   event handlers 
-000015e0: 7468 6174 2063 6861 6e67 6520 7468 6520  that change the 
-000015f0: 7374 6174 6520 7661 7273 2e20 4576 656e  state vars. Even
-00001600: 7420 6861 6e64 6c65 7273 2061 7265 2074  t handlers are t
-00001610: 6865 2077 6179 2074 6861 7420 7765 2063  he way that we c
-00001620: 616e 206d 6f64 6966 7920 7468 6520 7374  an modify the st
-00001630: 6174 6520 696e 2052 6566 6c65 782e 2054  ate in Reflex. T
-00001640: 6865 7920 6361 6e20 6265 2063 616c 6c65  hey can be calle
-00001650: 6420 696e 2072 6573 706f 6e73 6520 746f  d in response to
-00001660: 2075 7365 7220 6163 7469 6f6e 732c 2073   user actions, s
-00001670: 7563 6820 6173 2063 6c69 636b 696e 6720  uch as clicking 
-00001680: 6120 6275 7474 6f6e 206f 7220 7479 7069  a button or typi
-00001690: 6e67 2069 6e20 6120 7465 7874 2062 6f78  ng in a text box
-000016a0: 2e20 5468 6573 6520 6163 7469 6f6e 7320  . These actions 
-000016b0: 6172 6520 6361 6c6c 6564 2065 7665 6e74  are called event
-000016c0: 732e 0a0a 4f75 7220 4441 4c4c c2b7 452e  s...Our DALL..E.
-000016d0: 2061 7070 2068 6173 2061 6e20 6576 656e   app has an even
-000016e0: 7420 6861 6e64 6c65 722c 2060 6765 745f  t handler, `get_
-000016f0: 696d 6167 6560 2074 6f20 7768 6963 6820  image` to which 
-00001700: 6765 7420 7468 6973 2069 6d61 6765 2066  get this image f
-00001710: 726f 6d20 7468 6520 4f70 656e 4149 2041  rom the OpenAI A
-00001720: 5049 2e20 5573 696e 6720 6079 6965 6c64  PI. Using `yield
-00001730: 6020 696e 2074 6865 206d 6964 646c 6520  ` in the middle 
-00001740: 6f66 2061 6e20 6576 656e 7420 6861 6e64  of an event hand
-00001750: 6c65 7220 7769 6c6c 2063 6175 7365 2074  ler will cause t
-00001760: 6865 2055 4920 746f 2075 7064 6174 652e  he UI to update.
-00001770: 204f 7468 6572 7769 7365 2074 6865 2055   Otherwise the U
-00001780: 4920 7769 6c6c 2075 7064 6174 6520 6174  I will update at
-00001790: 2074 6865 2065 6e64 206f 6620 7468 6520   the end of the 
-000017a0: 6576 656e 7420 6861 6e64 6c65 722e 0a0a  event handler...
-000017b0: 2323 2320 2a2a 526f 7574 696e 672a 2a0a  ### **Routing**.
-000017c0: 0a46 696e 616c 6c79 2c20 7765 2064 6566  .Finally, we def
-000017d0: 696e 6520 6f75 7220 6170 7020 616e 6420  ine our app and 
-000017e0: 7061 7373 2069 7420 6f75 7220 7374 6174  pass it our stat
-000017f0: 652e 0a0a 6060 6070 7974 686f 6e0a 6170  e...```python.ap
-00001800: 7020 3d20 7278 2e41 7070 2873 7461 7465  p = rx.App(state
-00001810: 3d53 7461 7465 290a 6060 600a 0a57 6520  =State).```..We 
-00001820: 6164 6420 6120 726f 7574 6520 6672 6f6d  add a route from
-00001830: 2074 6865 2072 6f6f 7420 6f66 2074 6865   the root of the
-00001840: 2061 7070 2074 6f20 7468 6520 696e 6465   app to the inde
-00001850: 7820 636f 6d70 6f6e 656e 742e 2057 6520  x component. We 
-00001860: 616c 736f 2061 6464 2061 2074 6974 6c65  also add a title
-00001870: 2074 6861 7420 7769 6c6c 2073 686f 7720   that will show 
-00001880: 7570 2069 6e20 7468 6520 7061 6765 2070  up in the page p
-00001890: 7265 7669 6577 2f62 726f 7773 6572 2074  review/browser t
-000018a0: 6162 2e0a 0a60 6060 7079 7468 6f6e 0a61  ab...```python.a
-000018b0: 7070 2e61 6464 5f70 6167 6528 696e 6465  pp.add_page(inde
-000018c0: 782c 2074 6974 6c65 3d22 4441 4c4c 2d45  x, title="DALL-E
-000018d0: 2229 0a61 7070 2e63 6f6d 7069 6c65 2829  ").app.compile()
-000018e0: 0a60 6060 0a0a 596f 7520 6361 6e20 6372  .```..You can cr
-000018f0: 6561 7465 2061 206d 756c 7469 2d70 6167  eate a multi-pag
-00001900: 6520 6170 7020 6279 2061 6464 696e 6720  e app by adding 
-00001910: 6d6f 7265 2072 6f75 7465 732e 0a0a 2323  more routes...##
-00001920: 2053 7461 7475 730a 0a52 6566 6c65 7820   Status..Reflex 
-00001930: 6c61 756e 6368 6564 2069 6e20 4465 6365  launched in Dece
-00001940: 6d62 6572 2032 3032 3220 7769 7468 2074  mber 2022 with t
-00001950: 6865 206e 616d 6520 5079 6e65 636f 6e65  he name Pynecone
-00001960: 2e0a 0a41 7320 6f66 204a 756e 6520 3230  ...As of June 20
-00001970: 3233 2c20 7765 2061 7265 2069 6e20 7468  23, we are in th
-00001980: 6520 2a2a 5075 626c 6963 2042 6574 612a  e **Public Beta*
-00001990: 2a20 7374 6167 652e 0a0a 2d20 2020 3a77  * stage...-   :w
-000019a0: 6869 7465 5f63 6865 636b 5f6d 6172 6b3a  hite_check_mark:
-000019b0: 202a 2a50 7562 6c69 6320 416c 7068 612a   **Public Alpha*
-000019c0: 2a3a 2041 6e79 6f6e 6520 6361 6e20 696e  *: Anyone can in
-000019d0: 7374 616c 6c20 616e 6420 7573 6520 5265  stall and use Re
-000019e0: 666c 6578 2e20 5468 6572 6520 6d61 7920  flex. There may 
-000019f0: 6265 2069 7373 7565 732c 2062 7574 2077  be issues, but w
-00001a00: 6520 6172 6520 776f 726b 696e 6720 746f  e are working to
-00001a10: 2072 6573 6f6c 7665 2074 6865 6d20 6163   resolve them ac
-00001a20: 7469 7665 6c79 2e0a 2d20 2020 3a6c 6172  tively..-   :lar
-00001a30: 6765 5f6f 7261 6e67 655f 6469 616d 6f6e  ge_orange_diamon
-00001a40: 643a 202a 2a50 7562 6c69 6320 4265 7461  d: **Public Beta
-00001a50: 2a2a 3a20 5374 6162 6c65 2065 6e6f 7567  **: Stable enoug
-00001a60: 6820 666f 7220 6e6f 6e2d 656e 7465 7270  h for non-enterp
-00001a70: 7269 7365 2075 7365 2d63 6173 6573 2e0a  rise use-cases..
-00001a80: 2d20 2020 2a2a 5075 626c 6963 2048 6f73  -   **Public Hos
-00001a90: 7469 6e67 2042 6574 612a 2a3a 205f 4f70  ting Beta**: _Op
-00001aa0: 7469 6f6e 616c 6c79 5f2c 2064 6570 6c6f  tionally_, deplo
-00001ab0: 7920 616e 6420 686f 7374 2079 6f75 7220  y and host your 
-00001ac0: 6170 7073 206f 6e20 5265 666c 6578 210a  apps on Reflex!.
-00001ad0: 2d20 2020 2a2a 5075 626c 6963 2a2a 3a20  -   **Public**: 
-00001ae0: 5265 666c 6578 2069 7320 7072 6f64 7563  Reflex is produc
-00001af0: 7469 6f6e 2072 6561 6479 2e0a 0a52 6566  tion ready...Ref
-00001b00: 6c65 7820 6861 7320 6e65 7720 7265 6c65  lex has new rele
-00001b10: 6173 6573 2061 6e64 2066 6561 7475 7265  ases and feature
-00001b20: 7320 636f 6d69 6e67 2065 7665 7279 2077  s coming every w
-00001b30: 6565 6b21 204d 616b 6520 7375 7265 2074  eek! Make sure t
-00001b40: 6f20 3a73 7461 723a 2073 7461 7220 616e  o :star: star an
-00001b50: 6420 3a65 7965 733a 2077 6174 6368 2074  d :eyes: watch t
-00001b60: 6869 7320 7265 706f 7369 746f 7279 2074  his repository t
-00001b70: 6f20 7374 6179 2075 7020 746f 2064 6174  o stay up to dat
-00001b80: 652e 0a0a 2323 2043 6f6e 7472 6962 7574  e...## Contribut
-00001b90: 696e 670a 0a57 6520 7765 6c63 6f6d 6520  ing..We welcome 
-00001ba0: 636f 6e74 7269 6275 7469 6f6e 7320 6f66  contributions of
-00001bb0: 2061 6e79 2073 697a 6521 2042 656c 6f77   any size! Below
-00001bc0: 2061 7265 2073 6f6d 6520 676f 6f64 2077   are some good w
-00001bd0: 6179 7320 746f 2067 6574 2073 7461 7274  ays to get start
-00001be0: 6564 2069 6e20 7468 6520 5265 666c 6578  ed in the Reflex
-00001bf0: 2063 6f6d 6d75 6e69 7479 2e0a 0a2d 2020   community...-  
-00001c00: 202a 2a4a 6f69 6e20 4f75 7220 4469 7363   **Join Our Disc
-00001c10: 6f72 642a 2a3a 204f 7572 205b 4469 7363  ord**: Our [Disc
-00001c20: 6f72 645d 2868 7474 7073 3a2f 2f64 6973  ord](https://dis
-00001c30: 636f 7264 2e67 672f 5435 5753 6243 3259  cord.gg/T5WSbC2Y
-00001c40: 7451 2920 6973 2074 6865 2062 6573 7420  tQ) is the best 
-00001c50: 706c 6163 6520 746f 2067 6574 2068 656c  place to get hel
-00001c60: 7020 6f6e 2079 6f75 7220 5265 666c 6578  p on your Reflex
-00001c70: 2070 726f 6a65 6374 2061 6e64 2074 6f20   project and to 
-00001c80: 6469 7363 7573 7320 686f 7720 796f 7520  discuss how you 
-00001c90: 6361 6e20 636f 6e74 7269 6275 7465 2e0a  can contribute..
-00001ca0: 2d20 2020 2a2a 4769 7448 7562 2044 6973  -   **GitHub Dis
-00001cb0: 6375 7373 696f 6e73 2a2a 3a20 4120 6772  cussions**: A gr
-00001cc0: 6561 7420 7761 7920 746f 2074 616c 6b20  eat way to talk 
-00001cd0: 6162 6f75 7420 6665 6174 7572 6573 2079  about features y
-00001ce0: 6f75 2077 616e 7420 6164 6465 6420 6f72  ou want added or
-00001cf0: 2074 6869 6e67 7320 7468 6174 2061 7265   things that are
-00001d00: 2063 6f6e 6675 7369 6e67 2f6e 6565 6420   confusing/need 
-00001d10: 636c 6172 6966 6963 6174 696f 6e2e 0a2d  clarification..-
-00001d20: 2020 202a 2a47 6974 4875 6220 4973 7375     **GitHub Issu
-00001d30: 6573 2a2a 3a20 5468 6573 6520 6172 6520  es**: These are 
-00001d40: 616e 2065 7863 656c 6c65 6e74 2077 6179  an excellent way
-00001d50: 2074 6f20 7265 706f 7274 2062 7567 732e   to report bugs.
-00001d60: 2041 6464 6974 696f 6e61 6c6c 792c 2079   Additionally, y
-00001d70: 6f75 2063 616e 2074 7279 2061 6e64 2073  ou can try and s
-00001d80: 6f6c 7665 2061 6e20 6578 6973 7469 6e67  olve an existing
-00001d90: 2069 7373 7565 2061 6e64 2073 7562 6d69   issue and submi
-00001da0: 7420 6120 5052 2e0a 0a57 6520 6172 6520  t a PR...We are 
-00001db0: 6163 7469 7665 6c79 206c 6f6f 6b69 6e67  actively looking
-00001dc0: 2066 6f72 2063 6f6e 7472 6962 7574 6f72   for contributor
-00001dd0: 732c 206e 6f20 6d61 7474 6572 2079 6f75  s, no matter you
-00001de0: 7220 736b 696c 6c20 6c65 7665 6c20 6f72  r skill level or
-00001df0: 2065 7870 6572 6965 6e63 652e 0a0a 2323   experience...##
-00001e00: 204c 6963 656e 7365 0a0a 5265 666c 6578   License..Reflex
-00001e10: 2069 7320 6f70 656e 2d73 6f75 7263 6520   is open-source 
-00001e20: 616e 6420 6c69 6365 6e73 6564 2075 6e64  and licensed und
-00001e30: 6572 2074 6865 205b 4170 6163 6865 204c  er the [Apache L
-00001e40: 6963 656e 7365 2032 2e30 5d28 4c49 4345  icense 2.0](LICE
-00001e50: 4e53 4529 2e0a                           NSE)..
+000003a0: 5b45 6e67 6c69 7368 5d28 6874 7470 733a  [English](https:
+000003b0: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6566  //github.com/ref
+000003c0: 6c65 782d 6465 762f 7265 666c 6578 2f62  lex-dev/reflex/b
+000003d0: 6c6f 622f 6d61 696e 2f52 4541 444d 452e  lob/main/README.
+000003e0: 6d64 2920 7c20 5be7 ae80 e4bd 93e4 b8ad  md) | [.........
+000003f0: e696 875d 2868 7474 7073 3a2f 2f67 6974  ...](https://git
+00000400: 6875 622e 636f 6d2f 7265 666c 6578 2d64  hub.com/reflex-d
+00000410: 6576 2f72 6566 6c65 782f 626c 6f62 2f6d  ev/reflex/blob/m
+00000420: 6169 6e2f 646f 6373 2f7a 682f 7a68 5f63  ain/docs/zh/zh_c
+00000430: 6e2f 5245 4144 4d45 2e6d 6429 207c 205b  n/README.md) | [
+00000440: e7b9 81e9 ab94 e4b8 ade6 9687 5d28 6874  ............](ht
+00000450: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000460: 2f72 6566 6c65 782d 6465 762f 7265 666c  /reflex-dev/refl
+00000470: 6578 2f62 6c6f 622f 6d61 696e 2f64 6f63  ex/blob/main/doc
+00000480: 732f 7a68 2f7a 685f 7477 2f52 4541 444d  s/zh/zh_tw/READM
+00000490: 452e 6d64 290a 0a2d 2d2d 0a0a 2323 20f0  E.md)..---..## .
+000004a0: 9f93 a620 312e 2049 6e73 7461 6c6c 0a0a  ... 1. Install..
+000004b0: 5265 666c 6578 2072 6571 7569 7265 7320  Reflex requires 
+000004c0: 7468 6520 666f 6c6c 6f77 696e 6720 746f  the following to
+000004d0: 2067 6574 2073 7461 7274 6564 3a0a 0a2d   get started:..-
+000004e0: 2020 2050 7974 686f 6e20 332e 372b 0a2d     Python 3.7+.-
+000004f0: 2020 205b 4e6f 6465 2e6a 7320 3136 2e38     [Node.js 16.8
+00000500: 2e30 2b5d 2868 7474 7073 3a2f 2f6e 6f64  .0+](https://nod
+00000510: 656a 732e 6f72 672f 656e 2f29 2028 446f  ejs.org/en/) (Do
+00000520: 6e27 7420 776f 7272 792c 2079 6f75 2077  n't worry, you w
+00000530: 6f6e e280 9974 2068 6176 6520 746f 2077  on...t have to w
+00000540: 7269 7465 2061 6e79 204a 6176 6153 6372  rite any JavaScr
+00000550: 6970 7421 290a 0a60 6060 0a70 6970 2069  ipt!)..```.pip i
+00000560: 6e73 7461 6c6c 2072 6566 6c65 780a 6060  nstall reflex.``
+00000570: 600a 0a23 2320 f09f a5b3 2032 2e20 4372  `..## .... 2. Cr
+00000580: 6561 7465 2079 6f75 7220 6669 7273 7420  eate your first 
+00000590: 6170 700a 0a49 6e73 7461 6c6c 696e 6720  app..Installing 
+000005a0: 6072 6566 6c65 7860 2061 6c73 6f20 696e  `reflex` also in
+000005b0: 7374 616c 6c73 2074 6865 2060 7265 666c  stalls the `refl
+000005c0: 6578 6020 636f 6d6d 616e 6420 6c69 6e65  ex` command line
+000005d0: 2074 6f6f 6c2e 2054 6573 7420 7468 6174   tool. Test that
+000005e0: 2074 6865 2069 6e73 7461 6c6c 2077 6173   the install was
+000005f0: 2073 7563 6365 7373 6675 6c20 6279 2063   successful by c
+00000600: 7265 6174 696e 6720 6120 6e65 7720 7072  reating a new pr
+00000610: 6f6a 6563 742e 0a0a 5265 706c 6163 6520  oject...Replace 
+00000620: 6d79 5f61 7070 5f6e 616d 6520 7769 7468  my_app_name with
+00000630: 2079 6f75 7220 7072 6f6a 6563 7420 6e61   your project na
+00000640: 6d65 3a0a 0a60 6060 0a6d 6b64 6972 206d  me:..```.mkdir m
+00000650: 795f 6170 705f 6e61 6d65 0a63 6420 6d79  y_app_name.cd my
+00000660: 5f61 7070 5f6e 616d 650a 7265 666c 6578  _app_name.reflex
+00000670: 2069 6e69 740a 6060 600a 0a57 6865 6e20   init.```..When 
+00000680: 796f 7520 7275 6e20 7468 6973 2063 6f6d  you run this com
+00000690: 6d61 6e64 2066 6f72 2074 6865 2066 6972  mand for the fir
+000006a0: 7374 2074 696d 652c 2077 6520 7769 6c6c  st time, we will
+000006b0: 2064 6f77 6e6c 6f61 6420 616e 6420 696e   download and in
+000006c0: 7374 616c 6c20 5b62 756e 5d28 6874 7470  stall [bun](http
+000006d0: 733a 2f2f 6275 6e2e 7368 2f29 2061 7574  s://bun.sh/) aut
+000006e0: 6f6d 6174 6963 616c 6c79 2e0a 0a54 6869  omatically...Thi
+000006f0: 7320 636f 6d6d 616e 6420 696e 6974 6961  s command initia
+00000700: 6c69 7a65 7320 6120 7465 6d70 6c61 7465  lizes a template
+00000710: 2061 7070 2069 6e20 796f 7572 206e 6577   app in your new
+00000720: 2064 6972 6563 746f 7279 2e0a 0a23 2320   directory...## 
+00000730: f09f 8f83 2033 2e20 5275 6e20 796f 7572  .... 3. Run your
+00000740: 2061 7070 0a0a 596f 7520 6361 6e20 7275   app..You can ru
+00000750: 6e20 7468 6973 2061 7070 2069 6e20 6465  n this app in de
+00000760: 7665 6c6f 706d 656e 7420 6d6f 6465 3a0a  velopment mode:.
+00000770: 0a60 6060 0a72 6566 6c65 7820 7275 6e0a  .```.reflex run.
+00000780: 6060 600a 0a59 6f75 2073 686f 756c 6420  ```..You should 
+00000790: 7365 6520 796f 7572 2061 7070 2072 756e  see your app run
+000007a0: 6e69 6e67 2061 7420 6874 7470 3a2f 2f6c  ning at http://l
+000007b0: 6f63 616c 686f 7374 3a33 3030 302e 0a0a  ocalhost:3000...
+000007c0: 4e6f 7720 796f 7520 6361 6e20 6d6f 6469  Now you can modi
+000007d0: 6679 2074 6865 2073 6f75 7263 6520 636f  fy the source co
+000007e0: 6465 2069 6e20 606d 795f 6170 705f 6e61  de in `my_app_na
+000007f0: 6d65 2f6d 795f 6170 705f 6e61 6d65 2e70  me/my_app_name.p
+00000800: 7960 2e20 5265 666c 6578 2068 6173 2066  y`. Reflex has f
+00000810: 6173 7420 7265 6672 6573 6865 7320 736f  ast refreshes so
+00000820: 2079 6f75 2063 616e 2073 6565 2079 6f75   you can see you
+00000830: 7220 6368 616e 6765 7320 696e 7374 616e  r changes instan
+00000840: 746c 7920 7768 656e 2079 6f75 2073 6176  tly when you sav
+00000850: 6520 796f 7572 2063 6f64 652e 0a0a 2323  e your code...##
+00000860: 20f0 9fab a720 4578 616d 706c 650a 0a4c   .... Example..L
+00000870: 6574 2773 2067 6f20 6f76 6572 2061 6e20  et's go over an 
+00000880: 6578 616d 706c 653a 2063 7265 6174 696e  example: creatin
+00000890: 6720 616e 2069 6d61 6765 2067 656e 6572  g an image gener
+000008a0: 6174 696f 6e20 5549 2061 726f 756e 6420  ation UI around 
+000008b0: 4441 4c4c c2b7 452e 2046 6f72 2073 696d  DALL..E. For sim
+000008c0: 706c 6963 6974 792c 2077 6520 6a75 7374  plicity, we just
+000008d0: 2063 616c 6c20 7468 6520 4f70 656e 4149   call the OpenAI
+000008e0: 2041 5049 2c20 6275 7420 796f 7520 636f   API, but you co
+000008f0: 756c 6420 7265 706c 6163 6520 7468 6973  uld replace this
+00000900: 2077 6974 6820 616e 204d 4c20 6d6f 6465   with an ML mode
+00000910: 6c20 7275 6e20 6c6f 6361 6c6c 792e 0a0a  l run locally...
+00000920: 266e 6273 703b 0a0a 3c64 6976 2061 6c69  &nbsp;..<div ali
+00000930: 676e 3d22 6365 6e74 6572 223e 0a3c 696d  gn="center">.<im
+00000940: 6720 7372 633d 2264 6f63 732f 696d 6167  g src="docs/imag
+00000950: 6573 2f64 616c 6c65 2e67 6966 2220 616c  es/dalle.gif" al
+00000960: 743d 2241 2066 726f 6e74 656e 6420 7772  t="A frontend wr
+00000970: 6170 7065 7220 666f 7220 4441 4c4c c2b7  apper for DALL..
+00000980: 452c 2073 686f 776e 2069 6e20 7468 6520  E, shown in the 
+00000990: 7072 6f63 6573 7320 6f66 2067 656e 6572  process of gener
+000009a0: 6174 696e 6720 616e 2069 6d61 6765 2e22  ating an image."
+000009b0: 2077 6964 7468 3d22 3535 3022 202f 3e0a   width="550" />.
+000009c0: 3c2f 6469 763e 0a0a 266e 6273 703b 0a0a  </div>..&nbsp;..
+000009d0: 4865 7265 2069 7320 7468 6520 636f 6d70  Here is the comp
+000009e0: 6c65 7465 2063 6f64 6520 746f 2063 7265  lete code to cre
+000009f0: 6174 6520 7468 6973 2e20 5468 6973 2069  ate this. This i
+00000a00: 7320 616c 6c20 646f 6e65 2069 6e20 6f6e  s all done in on
+00000a10: 6520 5079 7468 6f6e 2066 696c 6521 0a0a  e Python file!..
+00000a20: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00000a30: 2072 6566 6c65 7820 6173 2072 780a 696d   reflex as rx.im
+00000a40: 706f 7274 206f 7065 6e61 690a 0a6f 7065  port openai..ope
+00000a50: 6e61 692e 6170 695f 6b65 7920 3d20 2259  nai.api_key = "Y
+00000a60: 4f55 525f 4150 495f 4b45 5922 0a0a 636c  OUR_API_KEY"..cl
+00000a70: 6173 7320 5374 6174 6528 7278 2e53 7461  ass State(rx.Sta
+00000a80: 7465 293a 0a20 2020 2022 2222 5468 6520  te):.    """The 
+00000a90: 6170 7020 7374 6174 652e 2222 220a 2020  app state.""".  
+00000aa0: 2020 7072 6f6d 7074 203d 2022 220a 2020    prompt = "".  
+00000ab0: 2020 696d 6167 655f 7572 6c20 3d20 2222    image_url = ""
+00000ac0: 0a20 2020 2070 726f 6365 7373 696e 6720  .    processing 
+00000ad0: 3d20 4661 6c73 650a 2020 2020 636f 6d70  = False.    comp
+00000ae0: 6c65 7465 203d 2046 616c 7365 0a0a 2020  lete = False..  
+00000af0: 2020 6465 6620 6765 745f 696d 6167 6528    def get_image(
+00000b00: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00000b10: 2222 4765 7420 7468 6520 696d 6167 6520  ""Get the image 
+00000b20: 6672 6f6d 2074 6865 2070 726f 6d70 742e  from the prompt.
+00000b30: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+00000b40: 656c 662e 7072 6f6d 7074 203d 3d20 2222  elf.prompt == ""
+00000b50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00000b60: 7475 726e 2072 782e 7769 6e64 6f77 5f61  turn rx.window_a
+00000b70: 6c65 7274 2822 5072 6f6d 7074 2045 6d70  lert("Prompt Emp
+00000b80: 7479 2229 0a0a 2020 2020 2020 2020 7365  ty")..        se
+00000b90: 6c66 2e70 726f 6365 7373 696e 672c 2073  lf.processing, s
+00000ba0: 656c 662e 636f 6d70 6c65 7465 203d 2054  elf.complete = T
+00000bb0: 7275 652c 2046 616c 7365 0a20 2020 2020  rue, False.     
+00000bc0: 2020 2079 6965 6c64 0a20 2020 2020 2020     yield.       
+00000bd0: 2072 6573 706f 6e73 6520 3d20 6f70 656e   response = open
+00000be0: 6169 2e49 6d61 6765 2e63 7265 6174 6528  ai.Image.create(
+00000bf0: 7072 6f6d 7074 3d73 656c 662e 7072 6f6d  prompt=self.prom
+00000c00: 7074 2c20 6e3d 312c 2073 697a 653d 2231  pt, n=1, size="1
+00000c10: 3032 3478 3130 3234 2229 0a20 2020 2020  024x1024").     
+00000c20: 2020 2073 656c 662e 696d 6167 655f 7572     self.image_ur
+00000c30: 6c20 3d20 7265 7370 6f6e 7365 5b22 6461  l = response["da
+00000c40: 7461 225d 5b30 5d5b 2275 726c 225d 0a20  ta"][0]["url"]. 
+00000c50: 2020 2020 2020 2073 656c 662e 7072 6f63         self.proc
+00000c60: 6573 7369 6e67 2c20 7365 6c66 2e63 6f6d  essing, self.com
+00000c70: 706c 6574 6520 3d20 4661 6c73 652c 2054  plete = False, T
+00000c80: 7275 650a 2020 2020 2020 2020 0a0a 6465  rue.        ..de
+00000c90: 6620 696e 6465 7828 293a 0a20 2020 2072  f index():.    r
+00000ca0: 6574 7572 6e20 7278 2e63 656e 7465 7228  eturn rx.center(
+00000cb0: 0a20 2020 2020 2020 2072 782e 7673 7461  .        rx.vsta
+00000cc0: 636b 280a 2020 2020 2020 2020 2020 2020  ck(.            
+00000cd0: 7278 2e68 6561 6469 6e67 2822 4441 4c4c  rx.heading("DALL
+00000ce0: c2b7 4522 292c 0a20 2020 2020 2020 2020  ..E"),.         
+00000cf0: 2020 2072 782e 696e 7075 7428 706c 6163     rx.input(plac
+00000d00: 6568 6f6c 6465 723d 2245 6e74 6572 2061  eholder="Enter a
+00000d10: 2070 726f 6d70 7422 2c20 6f6e 5f62 6c75   prompt", on_blu
+00000d20: 723d 5374 6174 652e 7365 745f 7072 6f6d  r=State.set_prom
+00000d30: 7074 292c 0a20 2020 2020 2020 2020 2020  pt),.           
+00000d40: 2072 782e 6275 7474 6f6e 280a 2020 2020   rx.button(.    
+00000d50: 2020 2020 2020 2020 2020 2020 2247 656e              "Gen
+00000d60: 6572 6174 6520 496d 6167 6522 2c0a 2020  erate Image",.  
+00000d70: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
+00000d80: 5f63 6c69 636b 3d53 7461 7465 2e67 6574  _click=State.get
+00000d90: 5f69 6d61 6765 2c0a 2020 2020 2020 2020  _image,.        
+00000da0: 2020 2020 2020 2020 6973 5f6c 6f61 6469          is_loadi
+00000db0: 6e67 3d53 7461 7465 2e70 726f 6365 7373  ng=State.process
+00000dc0: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
+00000dd0: 2020 2020 2077 6964 7468 3d22 3130 3025       width="100%
+00000de0: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
+00000df0: 2c0a 2020 2020 2020 2020 2020 2020 7278  ,.            rx
+00000e00: 2e63 6f6e 6428 0a20 2020 2020 2020 2020  .cond(.         
+00000e10: 2020 2020 2020 2053 7461 7465 2e63 6f6d         State.com
+00000e20: 706c 6574 652c 0a20 2020 2020 2020 2020  plete,.         
+00000e30: 2020 2020 2020 2020 2020 2020 7278 2e69              rx.i
+00000e40: 6d61 6765 280a 2020 2020 2020 2020 2020  mage(.          
+00000e50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000e60: 7263 3d53 7461 7465 2e69 6d61 6765 5f75  rc=State.image_u
+00000e70: 726c 2c0a 2020 2020 2020 2020 2020 2020  rl,.            
+00000e80: 2020 2020 2020 2020 2020 2020 2068 6569               hei
+00000e90: 6768 743d 2232 3565 6d22 2c0a 2020 2020  ght="25em",.    
+00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000eb0: 2020 2020 2077 6964 7468 3d22 3235 656d       width="25em
+00000ec0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000ed0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00000ee0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00000ef0: 2020 2020 7061 6464 696e 673d 2232 656d      padding="2em
+00000f00: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
+00000f10: 6861 646f 773d 226c 6722 2c0a 2020 2020  hadow="lg",.    
+00000f20: 2020 2020 2020 2020 626f 7264 6572 5f72          border_r
+00000f30: 6164 6975 733d 226c 6722 2c0a 2020 2020  adius="lg",.    
+00000f40: 2020 2020 292c 0a20 2020 2020 2020 2077      ),.        w
+00000f50: 6964 7468 3d22 3130 3025 222c 0a20 2020  idth="100%",.   
+00000f60: 2020 2020 2068 6569 6768 743d 2231 3030       height="100
+00000f70: 7668 222c 0a20 2020 2029 0a0a 2320 4164  vh",.    )..# Ad
+00000f80: 6420 7374 6174 6520 616e 6420 7061 6765  d state and page
+00000f90: 2074 6f20 7468 6520 6170 702e 0a61 7070   to the app..app
+00000fa0: 203d 2072 782e 4170 7028 7374 6174 653d   = rx.App(state=
+00000fb0: 5374 6174 6529 0a61 7070 2e61 6464 5f70  State).app.add_p
+00000fc0: 6167 6528 696e 6465 782c 2074 6974 6c65  age(index, title
+00000fd0: 3d22 7265 666c 6578 3a44 414c 4cc2 b745  ="reflex:DALL..E
+00000fe0: 2229 0a61 7070 2e63 6f6d 7069 6c65 2829  ").app.compile()
+00000ff0: 0a60 6060 0a0a 4c65 7427 7320 6272 6561  .```..Let's brea
+00001000: 6b20 7468 6973 2064 6f77 6e2e 0a0a 2323  k this down...##
+00001010: 2320 2a2a 5549 2049 6e20 5265 666c 6578  # **UI In Reflex
+00001020: 2a2a 0a0a 4c65 7427 7320 7374 6172 7420  **..Let's start 
+00001030: 7769 7468 2074 6865 2055 492e 0a0a 6060  with the UI...``
+00001040: 6070 7974 686f 6e0a 6465 6620 696e 6465  `python.def inde
+00001050: 7828 293a 0a20 2020 2072 6574 7572 6e20  x():.    return 
+00001060: 7278 2e63 656e 7465 7228 0a20 2020 2020  rx.center(.     
+00001070: 2020 202e 2e2e 0a20 2020 2029 0a60 6060     ....    ).```
+00001080: 0a0a 5468 6973 2060 696e 6465 7860 2066  ..This `index` f
+00001090: 756e 6374 696f 6e20 6465 6669 6e65 7320  unction defines 
+000010a0: 7468 6520 6672 6f6e 7465 6e64 206f 6620  the frontend of 
+000010b0: 7468 6520 6170 702e 0a0a 5765 2075 7365  the app...We use
+000010c0: 2064 6966 6665 7265 6e74 2063 6f6d 706f   different compo
+000010d0: 6e65 6e74 7320 7375 6368 2061 7320 6063  nents such as `c
+000010e0: 656e 7465 7260 2c20 6076 7374 6163 6b60  enter`, `vstack`
+000010f0: 2c20 6069 6e70 7574 602c 2061 6e64 2060  , `input`, and `
+00001100: 6275 7474 6f6e 6020 746f 2062 7569 6c64  button` to build
+00001110: 2074 6865 2066 726f 6e74 656e 642e 2043   the frontend. C
+00001120: 6f6d 706f 6e65 6e74 7320 6361 6e20 6265  omponents can be
+00001130: 206e 6573 7465 6420 7769 7468 696e 2065   nested within e
+00001140: 6163 6820 6f74 6865 720a 746f 2063 7265  ach other.to cre
+00001150: 6174 6520 636f 6d70 6c65 7820 6c61 796f  ate complex layo
+00001160: 7574 732e 2041 6e64 2079 6f75 2063 616e  uts. And you can
+00001170: 2075 7365 206b 6579 776f 7264 2061 7267   use keyword arg
+00001180: 7320 746f 2073 7479 6c65 2074 6865 6d20  s to style them 
+00001190: 7769 7468 2074 6865 2066 756c 6c20 706f  with the full po
+000011a0: 7765 7220 6f66 2043 5353 2e0a 0a52 6566  wer of CSS...Ref
+000011b0: 6c65 7820 636f 6d65 7320 7769 7468 205b  lex comes with [
+000011c0: 3630 2b20 6275 696c 742d 696e 2063 6f6d  60+ built-in com
+000011d0: 706f 6e65 6e74 735d 2868 7474 7073 3a2f  ponents](https:/
+000011e0: 2f72 6566 6c65 782e 6465 762f 646f 6373  /reflex.dev/docs
+000011f0: 2f6c 6962 7261 7279 2920 746f 2068 656c  /library) to hel
+00001200: 7020 796f 7520 6765 7420 7374 6172 7465  p you get starte
+00001210: 642e 2057 6520 6172 6520 6163 7469 7665  d. We are active
+00001220: 6c79 2061 6464 696e 6720 6d6f 7265 2063  ly adding more c
+00001230: 6f6d 706f 6e65 6e74 732c 2061 6e64 2069  omponents, and i
+00001240: 7427 7320 6561 7379 2074 6f20 5b63 7265  t's easy to [cre
+00001250: 6174 6520 796f 7572 206f 776e 2063 6f6d  ate your own com
+00001260: 706f 6e65 6e74 735d 2868 7474 7073 3a2f  ponents](https:/
+00001270: 2f72 6566 6c65 782e 6465 762f 646f 6373  /reflex.dev/docs
+00001280: 2f61 6476 616e 6365 642d 6775 6964 652f  /advanced-guide/
+00001290: 7772 6170 7069 6e67 2d72 6561 6374 292e  wrapping-react).
+000012a0: 0a0a 2323 2320 2a2a 5374 6174 652a 2a0a  ..### **State**.
+000012b0: 0a52 6566 6c65 7820 7265 7072 6573 656e  .Reflex represen
+000012c0: 7473 2079 6f75 7220 5549 2061 7320 6120  ts your UI as a 
+000012d0: 6675 6e63 7469 6f6e 206f 6620 796f 7572  function of your
+000012e0: 2073 7461 7465 2e0a 0a60 6060 7079 7468   state...```pyth
+000012f0: 6f6e 0a63 6c61 7373 2053 7461 7465 2872  on.class State(r
+00001300: 782e 5374 6174 6529 3a0a 2020 2020 2222  x.State):.    ""
+00001310: 2254 6865 2061 7070 2073 7461 7465 2e22  "The app state."
+00001320: 2222 0a20 2020 2070 726f 6d70 7420 3d20  "".    prompt = 
+00001330: 2222 0a20 2020 2069 6d61 6765 5f75 726c  "".    image_url
+00001340: 203d 2022 220a 2020 2020 7072 6f63 6573   = "".    proces
+00001350: 7369 6e67 203d 2046 616c 7365 0a20 2020  sing = False.   
+00001360: 2063 6f6d 706c 6574 6520 3d20 4661 6c73   complete = Fals
+00001370: 650a 6060 600a 0a54 6865 2073 7461 7465  e.```..The state
+00001380: 2064 6566 696e 6573 2061 6c6c 2074 6865   defines all the
+00001390: 2076 6172 6961 626c 6573 2028 6361 6c6c   variables (call
+000013a0: 6564 2076 6172 7329 2069 6e20 616e 2061  ed vars) in an a
+000013b0: 7070 2074 6861 7420 6361 6e20 6368 616e  pp that can chan
+000013c0: 6765 2061 6e64 2074 6865 2066 756e 6374  ge and the funct
+000013d0: 696f 6e73 2074 6861 7420 6368 616e 6765  ions that change
+000013e0: 2074 6865 6d2e 0a0a 4865 7265 2074 6865   them...Here the
+000013f0: 2073 7461 7465 2069 7320 636f 6d70 7269   state is compri
+00001400: 7365 6420 6f66 2061 2060 7072 6f6d 7074  sed of a `prompt
+00001410: 6020 616e 6420 6069 6d61 6765 5f75 726c  ` and `image_url
+00001420: 602e 2054 6865 7265 2061 7265 2061 6c73  `. There are als
+00001430: 6f20 7468 6520 626f 6f6c 6561 6e73 2060  o the booleans `
+00001440: 7072 6f63 6573 7369 6e67 6020 616e 6420  processing` and 
+00001450: 6063 6f6d 706c 6574 6560 2074 6f20 696e  `complete` to in
+00001460: 6469 6361 7465 2077 6865 6e20 746f 2073  dicate when to s
+00001470: 686f 7720 7468 6520 6369 7263 756c 6172  how the circular
+00001480: 2070 726f 6772 6573 7320 616e 6420 696d   progress and im
+00001490: 6167 652e 0a0a 2323 2320 2a2a 4576 656e  age...### **Even
+000014a0: 7420 4861 6e64 6c65 7273 2a2a 0a0a 6060  t Handlers**..``
+000014b0: 6070 7974 686f 6e0a 6465 6620 6765 745f  `python.def get_
+000014c0: 696d 6167 6528 7365 6c66 293a 0a20 2020  image(self):.   
+000014d0: 2022 2222 4765 7420 7468 6520 696d 6167   """Get the imag
+000014e0: 6520 6672 6f6d 2074 6865 2070 726f 6d70  e from the promp
+000014f0: 742e 2222 220a 2020 2020 6966 2073 656c  t.""".    if sel
+00001500: 662e 7072 6f6d 7074 203d 3d20 2222 3a0a  f.prompt == "":.
+00001510: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00001520: 782e 7769 6e64 6f77 5f61 6c65 7274 2822  x.window_alert("
+00001530: 5072 6f6d 7074 2045 6d70 7479 2229 0a0a  Prompt Empty")..
+00001540: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
+00001550: 696e 672c 2073 656c 662e 636f 6d70 6c65  ing, self.comple
+00001560: 7465 203d 2054 7275 652c 2046 616c 7365  te = True, False
+00001570: 0a20 2020 2079 6965 6c64 0a20 2020 2072  .    yield.    r
+00001580: 6573 706f 6e73 6520 3d20 6f70 656e 6169  esponse = openai
+00001590: 2e49 6d61 6765 2e63 7265 6174 6528 7072  .Image.create(pr
+000015a0: 6f6d 7074 3d73 656c 662e 7072 6f6d 7074  ompt=self.prompt
+000015b0: 2c20 6e3d 312c 2073 697a 653d 2231 3032  , n=1, size="102
+000015c0: 3478 3130 3234 2229 0a20 2020 2073 656c  4x1024").    sel
+000015d0: 662e 696d 6167 655f 7572 6c20 3d20 7265  f.image_url = re
+000015e0: 7370 6f6e 7365 5b22 6461 7461 225d 5b30  sponse["data"][0
+000015f0: 5d5b 2275 726c 225d 0a20 2020 2073 656c  ]["url"].    sel
+00001600: 662e 7072 6f63 6573 7369 6e67 2c20 7365  f.processing, se
+00001610: 6c66 2e63 6f6d 706c 6574 6520 3d20 4661  lf.complete = Fa
+00001620: 6c73 652c 2054 7275 650a 6060 600a 0a57  lse, True.```..W
+00001630: 6974 6869 6e20 7468 6520 7374 6174 652c  ithin the state,
+00001640: 2077 6520 6465 6669 6e65 2066 756e 6374   we define funct
+00001650: 696f 6e73 2063 616c 6c65 6420 6576 656e  ions called even
+00001660: 7420 6861 6e64 6c65 7273 2074 6861 7420  t handlers that 
+00001670: 6368 616e 6765 2074 6865 2073 7461 7465  change the state
+00001680: 2076 6172 732e 2045 7665 6e74 2068 616e   vars. Event han
+00001690: 646c 6572 7320 6172 6520 7468 6520 7761  dlers are the wa
+000016a0: 7920 7468 6174 2077 6520 6361 6e20 6d6f  y that we can mo
+000016b0: 6469 6679 2074 6865 2073 7461 7465 2069  dify the state i
+000016c0: 6e20 5265 666c 6578 2e20 5468 6579 2063  n Reflex. They c
+000016d0: 616e 2062 6520 6361 6c6c 6564 2069 6e20  an be called in 
+000016e0: 7265 7370 6f6e 7365 2074 6f20 7573 6572  response to user
+000016f0: 2061 6374 696f 6e73 2c20 7375 6368 2061   actions, such a
+00001700: 7320 636c 6963 6b69 6e67 2061 2062 7574  s clicking a but
+00001710: 746f 6e20 6f72 2074 7970 696e 6720 696e  ton or typing in
+00001720: 2061 2074 6578 7420 626f 782e 2054 6865   a text box. The
+00001730: 7365 2061 6374 696f 6e73 2061 7265 2063  se actions are c
+00001740: 616c 6c65 6420 6576 656e 7473 2e0a 0a4f  alled events...O
+00001750: 7572 2044 414c 4cc2 b745 2e20 6170 7020  ur DALL..E. app 
+00001760: 6861 7320 616e 2065 7665 6e74 2068 616e  has an event han
+00001770: 646c 6572 2c20 6067 6574 5f69 6d61 6765  dler, `get_image
+00001780: 6020 746f 2077 6869 6368 2067 6574 2074  ` to which get t
+00001790: 6869 7320 696d 6167 6520 6672 6f6d 2074  his image from t
+000017a0: 6865 204f 7065 6e41 4920 4150 492e 2055  he OpenAI API. U
+000017b0: 7369 6e67 2060 7969 656c 6460 2069 6e20  sing `yield` in 
+000017c0: 7468 6520 6d69 6464 6c65 206f 6620 616e  the middle of an
+000017d0: 2065 7665 6e74 2068 616e 646c 6572 2077   event handler w
+000017e0: 696c 6c20 6361 7573 6520 7468 6520 5549  ill cause the UI
+000017f0: 2074 6f20 7570 6461 7465 2e20 4f74 6865   to update. Othe
+00001800: 7277 6973 6520 7468 6520 5549 2077 696c  rwise the UI wil
+00001810: 6c20 7570 6461 7465 2061 7420 7468 6520  l update at the 
+00001820: 656e 6420 6f66 2074 6865 2065 7665 6e74  end of the event
+00001830: 2068 616e 646c 6572 2e0a 0a23 2323 202a   handler...### *
+00001840: 2a52 6f75 7469 6e67 2a2a 0a0a 4669 6e61  *Routing**..Fina
+00001850: 6c6c 792c 2077 6520 6465 6669 6e65 206f  lly, we define o
+00001860: 7572 2061 7070 2061 6e64 2070 6173 7320  ur app and pass 
+00001870: 6974 206f 7572 2073 7461 7465 2e0a 0a60  it our state...`
+00001880: 6060 7079 7468 6f6e 0a61 7070 203d 2072  ``python.app = r
+00001890: 782e 4170 7028 7374 6174 653d 5374 6174  x.App(state=Stat
+000018a0: 6529 0a60 6060 0a0a 5765 2061 6464 2061  e).```..We add a
+000018b0: 2072 6f75 7465 2066 726f 6d20 7468 6520   route from the 
+000018c0: 726f 6f74 206f 6620 7468 6520 6170 7020  root of the app 
+000018d0: 746f 2074 6865 2069 6e64 6578 2063 6f6d  to the index com
+000018e0: 706f 6e65 6e74 2e20 5765 2061 6c73 6f20  ponent. We also 
+000018f0: 6164 6420 6120 7469 746c 6520 7468 6174  add a title that
+00001900: 2077 696c 6c20 7368 6f77 2075 7020 696e   will show up in
+00001910: 2074 6865 2070 6167 6520 7072 6576 6965   the page previe
+00001920: 772f 6272 6f77 7365 7220 7461 622e 0a0a  w/browser tab...
+00001930: 6060 6070 7974 686f 6e0a 6170 702e 6164  ```python.app.ad
+00001940: 645f 7061 6765 2869 6e64 6578 2c20 7469  d_page(index, ti
+00001950: 746c 653d 2244 414c 4c2d 4522 290a 6170  tle="DALL-E").ap
+00001960: 702e 636f 6d70 696c 6528 290a 6060 600a  p.compile().```.
+00001970: 0a59 6f75 2063 616e 2063 7265 6174 6520  .You can create 
+00001980: 6120 6d75 6c74 692d 7061 6765 2061 7070  a multi-page app
+00001990: 2062 7920 6164 6469 6e67 206d 6f72 6520   by adding more 
+000019a0: 726f 7574 6573 2e0a 0a23 2320 5374 6174  routes...## Stat
+000019b0: 7573 0a0a 5265 666c 6578 206c 6175 6e63  us..Reflex launc
+000019c0: 6865 6420 696e 2044 6563 656d 6265 7220  hed in December 
+000019d0: 3230 3232 2077 6974 6820 7468 6520 6e61  2022 with the na
+000019e0: 6d65 2050 796e 6563 6f6e 652e 0a0a 4173  me Pynecone...As
+000019f0: 206f 6620 4a75 6e65 2032 3032 332c 2077   of June 2023, w
+00001a00: 6520 6172 6520 696e 2074 6865 202a 2a50  e are in the **P
+00001a10: 7562 6c69 6320 4265 7461 2a2a 2073 7461  ublic Beta** sta
+00001a20: 6765 2e0a 0a2d 2020 203a 7768 6974 655f  ge...-   :white_
+00001a30: 6368 6563 6b5f 6d61 726b 3a20 2a2a 5075  check_mark: **Pu
+00001a40: 626c 6963 2041 6c70 6861 2a2a 3a20 416e  blic Alpha**: An
+00001a50: 796f 6e65 2063 616e 2069 6e73 7461 6c6c  yone can install
+00001a60: 2061 6e64 2075 7365 2052 6566 6c65 782e   and use Reflex.
+00001a70: 2054 6865 7265 206d 6179 2062 6520 6973   There may be is
+00001a80: 7375 6573 2c20 6275 7420 7765 2061 7265  sues, but we are
+00001a90: 2077 6f72 6b69 6e67 2074 6f20 7265 736f   working to reso
+00001aa0: 6c76 6520 7468 656d 2061 6374 6976 656c  lve them activel
+00001ab0: 792e 0a2d 2020 203a 6c61 7267 655f 6f72  y..-   :large_or
+00001ac0: 616e 6765 5f64 6961 6d6f 6e64 3a20 2a2a  ange_diamond: **
+00001ad0: 5075 626c 6963 2042 6574 612a 2a3a 2053  Public Beta**: S
+00001ae0: 7461 626c 6520 656e 6f75 6768 2066 6f72  table enough for
+00001af0: 206e 6f6e 2d65 6e74 6572 7072 6973 6520   non-enterprise 
+00001b00: 7573 652d 6361 7365 732e 0a2d 2020 202a  use-cases..-   *
+00001b10: 2a50 7562 6c69 6320 486f 7374 696e 6720  *Public Hosting 
+00001b20: 4265 7461 2a2a 3a20 5f4f 7074 696f 6e61  Beta**: _Optiona
+00001b30: 6c6c 795f 2c20 6465 706c 6f79 2061 6e64  lly_, deploy and
+00001b40: 2068 6f73 7420 796f 7572 2061 7070 7320   host your apps 
+00001b50: 6f6e 2052 6566 6c65 7821 0a2d 2020 202a  on Reflex!.-   *
+00001b60: 2a50 7562 6c69 632a 2a3a 2052 6566 6c65  *Public**: Refle
+00001b70: 7820 6973 2070 726f 6475 6374 696f 6e20  x is production 
+00001b80: 7265 6164 792e 0a0a 5265 666c 6578 2068  ready...Reflex h
+00001b90: 6173 206e 6577 2072 656c 6561 7365 7320  as new releases 
+00001ba0: 616e 6420 6665 6174 7572 6573 2063 6f6d  and features com
+00001bb0: 696e 6720 6576 6572 7920 7765 656b 2120  ing every week! 
+00001bc0: 4d61 6b65 2073 7572 6520 746f 203a 7374  Make sure to :st
+00001bd0: 6172 3a20 7374 6172 2061 6e64 203a 6579  ar: star and :ey
+00001be0: 6573 3a20 7761 7463 6820 7468 6973 2072  es: watch this r
+00001bf0: 6570 6f73 6974 6f72 7920 746f 2073 7461  epository to sta
+00001c00: 7920 7570 2074 6f20 6461 7465 2e0a 0a23  y up to date...#
+00001c10: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
+00001c20: 5765 2077 656c 636f 6d65 2063 6f6e 7472  We welcome contr
+00001c30: 6962 7574 696f 6e73 206f 6620 616e 7920  ibutions of any 
+00001c40: 7369 7a65 2120 4265 6c6f 7720 6172 6520  size! Below are 
+00001c50: 736f 6d65 2067 6f6f 6420 7761 7973 2074  some good ways t
+00001c60: 6f20 6765 7420 7374 6172 7465 6420 696e  o get started in
+00001c70: 2074 6865 2052 6566 6c65 7820 636f 6d6d   the Reflex comm
+00001c80: 756e 6974 792e 0a0a 2d20 2020 2a2a 4a6f  unity...-   **Jo
+00001c90: 696e 204f 7572 2044 6973 636f 7264 2a2a  in Our Discord**
+00001ca0: 3a20 4f75 7220 5b44 6973 636f 7264 5d28  : Our [Discord](
+00001cb0: 6874 7470 733a 2f2f 6469 7363 6f72 642e  https://discord.
+00001cc0: 6767 2f54 3557 5362 4332 5974 5129 2069  gg/T5WSbC2YtQ) i
+00001cd0: 7320 7468 6520 6265 7374 2070 6c61 6365  s the best place
+00001ce0: 2074 6f20 6765 7420 6865 6c70 206f 6e20   to get help on 
+00001cf0: 796f 7572 2052 6566 6c65 7820 7072 6f6a  your Reflex proj
+00001d00: 6563 7420 616e 6420 746f 2064 6973 6375  ect and to discu
+00001d10: 7373 2068 6f77 2079 6f75 2063 616e 2063  ss how you can c
+00001d20: 6f6e 7472 6962 7574 652e 0a2d 2020 202a  ontribute..-   *
+00001d30: 2a47 6974 4875 6220 4469 7363 7573 7369  *GitHub Discussi
+00001d40: 6f6e 732a 2a3a 2041 2067 7265 6174 2077  ons**: A great w
+00001d50: 6179 2074 6f20 7461 6c6b 2061 626f 7574  ay to talk about
+00001d60: 2066 6561 7475 7265 7320 796f 7520 7761   features you wa
+00001d70: 6e74 2061 6464 6564 206f 7220 7468 696e  nt added or thin
+00001d80: 6773 2074 6861 7420 6172 6520 636f 6e66  gs that are conf
+00001d90: 7573 696e 672f 6e65 6564 2063 6c61 7269  using/need clari
+00001da0: 6669 6361 7469 6f6e 2e0a 2d20 2020 2a2a  fication..-   **
+00001db0: 4769 7448 7562 2049 7373 7565 732a 2a3a  GitHub Issues**:
+00001dc0: 2054 6865 7365 2061 7265 2061 6e20 6578   These are an ex
+00001dd0: 6365 6c6c 656e 7420 7761 7920 746f 2072  cellent way to r
+00001de0: 6570 6f72 7420 6275 6773 2e20 4164 6469  eport bugs. Addi
+00001df0: 7469 6f6e 616c 6c79 2c20 796f 7520 6361  tionally, you ca
+00001e00: 6e20 7472 7920 616e 6420 736f 6c76 6520  n try and solve 
+00001e10: 616e 2065 7869 7374 696e 6720 6973 7375  an existing issu
+00001e20: 6520 616e 6420 7375 626d 6974 2061 2050  e and submit a P
+00001e30: 522e 0a0a 5765 2061 7265 2061 6374 6976  R...We are activ
+00001e40: 656c 7920 6c6f 6f6b 696e 6720 666f 7220  ely looking for 
+00001e50: 636f 6e74 7269 6275 746f 7273 2c20 6e6f  contributors, no
+00001e60: 206d 6174 7465 7220 796f 7572 2073 6b69   matter your ski
+00001e70: 6c6c 206c 6576 656c 206f 7220 6578 7065  ll level or expe
+00001e80: 7269 656e 6365 2e0a 0a23 2320 4c69 6365  rience...## Lice
+00001e90: 6e73 650a 0a52 6566 6c65 7820 6973 206f  nse..Reflex is o
+00001ea0: 7065 6e2d 736f 7572 6365 2061 6e64 206c  pen-source and l
+00001eb0: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
+00001ec0: 6520 5b41 7061 6368 6520 4c69 6365 6e73  e [Apache Licens
+00001ed0: 6520 322e 305d 284c 4943 454e 5345 292e  e 2.0](LICENSE).
+00001ee0: 0a                                       .
```

### Comparing `reflex-0.2.3a1/pyproject.toml` & `reflex-0.2.3a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.2.3a1"
+version = "0.2.3a2"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `reflex-0.2.3a1/reflex/.templates/apps/counter/counter.py` & `reflex-0.2.3a2/reflex/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/.templates/apps/default/default.py` & `reflex-0.2.3a2/reflex/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/.templates/assets/favicon.ico` & `reflex-0.2.3a2/reflex/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/.templates/jinja/web/pages/index.js.jinja2` & `reflex-0.2.3a2/reflex/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.2.3a2/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/.templates/web/bun.lockb` & `reflex-0.2.3a2/reflex/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/.templates/web/package.json` & `reflex-0.2.3a2/reflex/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/.templates/web/pages/_app.js` & `reflex-0.2.3a2/reflex/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/.templates/web/styles/code/prism.js` & `reflex-0.2.3a2/reflex/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/.templates/web/utils/state.js` & `reflex-0.2.3a2/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/__init__.py` & `reflex-0.2.3a2/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/app.py` & `reflex-0.2.3a2/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/base.py` & `reflex-0.2.3a2/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/compiler/compiler.py` & `reflex-0.2.3a2/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/compiler/templates.py` & `reflex-0.2.3a2/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/compiler/utils.py` & `reflex-0.2.3a2/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/__init__.py` & `reflex-0.2.3a2/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/base/bare.py` & `reflex-0.2.3a2/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/base/document.py` & `reflex-0.2.3a2/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/base/link.py` & `reflex-0.2.3a2/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/base/meta.py` & `reflex-0.2.3a2/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/base/script.py` & `reflex-0.2.3a2/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/component.py` & `reflex-0.2.3a2/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/datadisplay/code.py` & `reflex-0.2.3a2/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/datadisplay/datatable.py` & `reflex-0.2.3a2/reflex/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/datadisplay/divider.py` & `reflex-0.2.3a2/reflex/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/datadisplay/list.py` & `reflex-0.2.3a2/reflex/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/datadisplay/stat.py` & `reflex-0.2.3a2/reflex/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/datadisplay/table.py` & `reflex-0.2.3a2/reflex/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/datadisplay/tag.py` & `reflex-0.2.3a2/reflex/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/disclosure/accordion.py` & `reflex-0.2.3a2/reflex/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/disclosure/tabs.py` & `reflex-0.2.3a2/reflex/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/disclosure/transition.py` & `reflex-0.2.3a2/reflex/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/feedback/alert.py` & `reflex-0.2.3a2/reflex/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/feedback/circularprogress.py` & `reflex-0.2.3a2/reflex/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/feedback/progress.py` & `reflex-0.2.3a2/reflex/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/feedback/skeleton.py` & `reflex-0.2.3a2/reflex/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/feedback/spinner.py` & `reflex-0.2.3a2/reflex/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/__init__.py` & `reflex-0.2.3a2/reflex/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/button.py` & `reflex-0.2.3a2/reflex/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/checkbox.py` & `reflex-0.2.3a2/reflex/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/colormodeswitch.py` & `reflex-0.2.3a2/reflex/components/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/copytoclipboard.py` & `reflex-0.2.3a2/reflex/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/debounce.py` & `reflex-0.2.3a2/reflex/components/forms/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/editable.py` & `reflex-0.2.3a2/reflex/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/form.py` & `reflex-0.2.3a2/reflex/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/iconbutton.py` & `reflex-0.2.3a2/reflex/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/input.py` & `reflex-0.2.3a2/reflex/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/multiselect.py` & `reflex-0.2.3a2/reflex/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/numberinput.py` & `reflex-0.2.3a2/reflex/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/pininput.py` & `reflex-0.2.3a2/reflex/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/radio.py` & `reflex-0.2.3a2/reflex/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/rangeslider.py` & `reflex-0.2.3a2/reflex/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/select.py` & `reflex-0.2.3a2/reflex/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/slider.py` & `reflex-0.2.3a2/reflex/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/switch.py` & `reflex-0.2.3a2/reflex/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/textarea.py` & `reflex-0.2.3a2/reflex/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/forms/upload.py` & `reflex-0.2.3a2/reflex/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/graphing/plotly.py` & `reflex-0.2.3a2/reflex/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/graphing/victory.py` & `reflex-0.2.3a2/reflex/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/layout/__init__.py` & `reflex-0.2.3a2/reflex/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/layout/box.py` & `reflex-0.2.3a2/reflex/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/layout/card.py` & `reflex-0.2.3a2/reflex/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/layout/cond.py` & `reflex-0.2.3a2/reflex/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/layout/flex.py` & `reflex-0.2.3a2/reflex/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/layout/foreach.py` & `reflex-0.2.3a2/reflex/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/layout/grid.py` & `reflex-0.2.3a2/reflex/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/layout/html.py` & `reflex-0.2.3a2/reflex/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/layout/responsive.py` & `reflex-0.2.3a2/reflex/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/layout/stack.py` & `reflex-0.2.3a2/reflex/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/layout/wrap.py` & `reflex-0.2.3a2/reflex/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/libs/react_player.py` & `reflex-0.2.3a2/reflex/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/media/avatar.py` & `reflex-0.2.3a2/reflex/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/media/icon.py` & `reflex-0.2.3a2/reflex/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/media/image.py` & `reflex-0.2.3a2/reflex/components/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/navigation/breadcrumb.py` & `reflex-0.2.3a2/reflex/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/navigation/link.py` & `reflex-0.2.3a2/reflex/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/navigation/linkoverlay.py` & `reflex-0.2.3a2/reflex/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/navigation/stepper.py` & `reflex-0.2.3a2/reflex/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/overlay/__init__.py` & `reflex-0.2.3a2/reflex/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/overlay/alertdialog.py` & `reflex-0.2.3a2/reflex/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/overlay/banner.py` & `reflex-0.2.3a2/reflex/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/overlay/drawer.py` & `reflex-0.2.3a2/reflex/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/overlay/menu.py` & `reflex-0.2.3a2/reflex/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/overlay/modal.py` & `reflex-0.2.3a2/reflex/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/overlay/popover.py` & `reflex-0.2.3a2/reflex/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/overlay/tooltip.py` & `reflex-0.2.3a2/reflex/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/tags/iter_tag.py` & `reflex-0.2.3a2/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/tags/tag.py` & `reflex-0.2.3a2/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/tags/tagless.py` & `reflex-0.2.3a2/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/typography/highlight.py` & `reflex-0.2.3a2/reflex/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/components/typography/markdown.py` & `reflex-0.2.3a2/reflex/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/config.py` & `reflex-0.2.3a2/reflex/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,20 +161,14 @@
 
     # The rxdeploy url.
     rxdeploy_url: Optional[str] = None
 
     # The environment mode.
     env: constants.Env = constants.Env.DEV
 
-    # The path to the bun executable.
-    bun_path: str = constants.BUN_PATH
-
-    # Disable bun.
-    disable_bun: bool = False
-
     # Additional frontend packages to install.
     frontend_packages: List[str] = []
 
     # The Admin Dash.
     admin_dash: Optional[AdminDash] = None
 
     # Backend transport methods.
```

### Comparing `reflex-0.2.3a1/reflex/constants.py` & `reflex-0.2.3a2/reflex/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Constants used throughout the package."""
 
 import os
+import platform
 import re
 from enum import Enum
 from types import SimpleNamespace
 from typing import Any, Type
 
 # importlib is only available for Python 3.8+ so we need the backport for Python 3.7
 try:
@@ -39,20 +40,45 @@
 
 
 # App names and versions.
 # The name of the Reflex package.
 MODULE_NAME = "reflex"
 # The current version of Reflex.
 VERSION = metadata.version(MODULE_NAME)
-# Minimum version of Node.js required to run Reflex.
-MIN_NODE_VERSION = "16.8.0"
 
-# Valid bun versions.
-MIN_BUN_VERSION = "0.5.9"
-MAX_BUN_VERSION = "0.6.9"
+# Project dependencies.
+# The directory to store reflex dependencies.
+REFLEX_DIR = os.path.expandvars("$HOME/.reflex")
+
+# Bun config.
+# The Bun version.
+BUN_VERSION = "0.7.0"
+# The directory to store the bun.
+BUN_ROOT_PATH = f"{REFLEX_DIR}/.bun"
+# The bun path.
+BUN_PATH = f"{BUN_ROOT_PATH}/bin/bun"
+# Command to install bun.
+INSTALL_BUN = f"curl -fsSL https://bun.sh/install | env BUN_INSTALL={BUN_ROOT_PATH} bash -s -- bun-v{BUN_VERSION}"
+
+# NVM / Node config.
+# The Node version.
+NODE_VERSION = "18.17.0"
+# The directory to store nvm.
+NVM_ROOT_PATH = f"{REFLEX_DIR}/.nvm"
+# The nvm path.
+NVM_PATH = f"{NVM_ROOT_PATH}/nvm.sh"
+# The node bin path.
+NODE_BIN_PATH = f"{NVM_ROOT_PATH}/versions/node/v{NODE_VERSION}/bin"
+# The default path where node is installed.
+NODE_PATH = "node" if platform.system() == "Windows" else f"{NODE_BIN_PATH}/node"
+# Command to install nvm.
+INSTALL_NVM = f"curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | env NVM_DIR={NVM_ROOT_PATH} bash"
+# Command to install node.
+INSTALL_NODE = f". {NVM_ROOT_PATH}/nvm.sh && nvm install {NODE_VERSION}"
+
 
 # Files and directories used to init a new project.
 # The root directory of the reflex library.
 ROOT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 # The name of the assets directory.
 APP_ASSETS_DIR = "assets"
 # The template directory used during reflex init.
@@ -106,20 +132,14 @@
 FRONTEND_PORT = get_value("FRONTEND_PORT", "3000")
 # The backend default port.
 BACKEND_PORT = get_value("BACKEND_PORT", "8000")
 # The backend api url.
 API_URL = get_value("API_URL", "http://localhost:8000")
 # The deploy url
 DEPLOY_URL = get_value("DEPLOY_URL")
-# bun root location
-BUN_ROOT_PATH = "$HOME/.bun"
-# The default path where bun is installed.
-BUN_PATH = get_value("BUN_PATH", f"{BUN_ROOT_PATH}/bin/bun")
-# Command to install bun.
-INSTALL_BUN = f"curl -fsSL https://bun.sh/install | bash -s -- bun-v{MAX_BUN_VERSION}"
 # Default host in dev mode.
 BACKEND_HOST = get_value("BACKEND_HOST", "0.0.0.0")
 # The default timeout when launching the gunicorn server.
 TIMEOUT = get_value("TIMEOUT", 120, type_=int)
 # The command to run the backend in production mode.
 RUN_BACKEND_PROD = f"gunicorn --worker-class uvicorn.workers.UvicornH11Worker --preload --timeout {TIMEOUT} --log-level critical".split()
 RUN_BACKEND_PROD_WINDOWS = f"uvicorn --timeout-keep-alive {TIMEOUT}".split()
```

### Comparing `reflex-0.2.3a1/reflex/el/constants/html.py` & `reflex-0.2.3a2/reflex/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/el/constants/react.py` & `reflex-0.2.3a2/reflex/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/el/constants/reflex.py` & `reflex-0.2.3a2/reflex/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/el/element.py` & `reflex-0.2.3a2/reflex/el/element.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/el/elements/__init__.py` & `reflex-0.2.3a2/reflex/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/el/precompile.py` & `reflex-0.2.3a2/reflex/el/precompile.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/event.py` & `reflex-0.2.3a2/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/middleware/hydrate_middleware.py` & `reflex-0.2.3a2/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/middleware/middleware.py` & `reflex-0.2.3a2/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/model.py` & `reflex-0.2.3a2/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/reflex.py` & `reflex-0.2.3a2/reflex/reflex.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,43 +28,36 @@
 def init(
     name: str = typer.Option(None, help="Name of the app to be initialized."),
     template: constants.Template = typer.Option(
         constants.Template.DEFAULT, help="Template to use for the app."
     ),
 ):
     """Initialize a new Reflex app in the current directory."""
+    # Get the app name.
     app_name = prerequisites.get_default_app_name() if name is None else name
-
-    # Make sure they don't name the app "reflex".
-    if app_name == constants.MODULE_NAME:
-        console.print(
-            f"[red]The app directory cannot be named [bold]{constants.MODULE_NAME}."
-        )
-        raise typer.Exit()
-
     console.rule(f"[bold]Initializing {app_name}")
-    # Set up the web directory.
-    prerequisites.validate_and_install_bun()
-    prerequisites.initialize_web_directory()
+
+    # Set up the web project.
+    prerequisites.initialize_frontend_dependencies()
 
     # Migrate Pynecone projects to Reflex.
     prerequisites.migrate_to_reflex()
 
     # Set up the app directory, only if the config doesn't exist.
     if not os.path.exists(constants.CONFIG_FILE):
         prerequisites.create_config(app_name)
         prerequisites.initialize_app_directory(app_name, template)
         build.set_reflex_project_hash()
         telemetry.send("init", get_config().telemetry_enabled)
     else:
-        build.set_reflex_project_hash()
         telemetry.send("reinit", get_config().telemetry_enabled)
 
     # Initialize the .gitignore.
     prerequisites.initialize_gitignore()
+
     # Finish initializing the app.
     console.log(f"[bold green]Finished Initializing: {app_name}")
 
 
 @cli.command()
 def run(
     env: constants.Env = typer.Option(
@@ -80,15 +73,15 @@
     frontend_port: str = typer.Option(None, help="Specify a different frontend port."),
     backend_port: str = typer.Option(None, help="Specify a different backend port."),
     backend_host: str = typer.Option(None, help="Specify the backend host."),
 ):
     """Run the app in the current directory."""
     if platform.system() == "Windows":
         console.print(
-            "[yellow][WARNING] We strongly advise you to use Windows Subsystem for Linux (WSL) for optimal performance when using Reflex. Due to compatibility issues with one of our dependencies, Bun, you may experience slower performance on Windows. By using WSL, you can expect to see a significant speed increase."
+            "[yellow][WARNING] We strongly advise using Windows Subsystem for Linux (WSL) for optimal performance with reflex."
         )
     # Set ports as os env variables to take precedence over config and
     # .env variables(if override_os_envs flag in config is set to False).
     build.set_os_env(
         frontend_port=frontend_port,
         backend_port=backend_port,
         backend_host=backend_host,
```

### Comparing `reflex-0.2.3a1/reflex/route.py` & `reflex-0.2.3a2/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/state.py` & `reflex-0.2.3a2/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/style.py` & `reflex-0.2.3a2/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/testing.py` & `reflex-0.2.3a2/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/utils/build.py` & `reflex-0.2.3a2/reflex/utils/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,37 +202,34 @@
 
 
 def setup_frontend(
     root: Path,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
     disable_telemetry: bool = True,
 ):
-    """Set up the frontend.
+    """Set up the frontend to run the app.
 
     Args:
         root: The root path of the project.
         loglevel: The log level to use.
         disable_telemetry: Whether to disable the Next telemetry.
     """
-    # Validate bun version.
-    prerequisites.validate_and_install_bun(initialize=False)
-
-    # Initialize the web directory if it doesn't exist.
-    web_dir = prerequisites.create_web_directory(root)
+    # Initialize the dependencies.
+    prerequisites.initialize_frontend_dependencies()
 
     # Install frontend packages.
-    prerequisites.install_frontend_packages(web_dir)
+    prerequisites.install_frontend_packages()
 
     # Copy asset files to public folder.
     path_ops.cp(
         src=str(root / constants.APP_ASSETS_DIR),
         dest=str(root / constants.WEB_ASSETS_DIR),
     )
 
-    # set the environment variables in client(env.json)
+    # Set the environment variables in client (env.json).
     set_environment_variables()
 
     # Disable the Next telemetry.
     if disable_telemetry:
         new_process(
             [
                 prerequisites.get_package_manager(),
```

### Comparing `reflex-0.2.3a1/reflex/utils/console.py` & `reflex-0.2.3a2/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/utils/exec.py` & `reflex-0.2.3a2/reflex/utils/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,15 @@
     """
     # Start watching asset folder.
     start_watching_assets_folder(root)
 
     # Run the frontend in development mode.
     console.rule("[bold green]App Running")
     os.environ["PORT"] = get_config().frontend_port if port is None else port
-    run_process_and_launch_url(
-        [prerequisites.get_package_manager(), "run", "dev"], loglevel
-    )
+    run_process_and_launch_url(["npm", "run", "dev"], loglevel)
 
 
 def run_frontend_prod(
     root: Path,
     port: str,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
```

### Comparing `reflex-0.2.3a1/reflex/utils/format.py` & `reflex-0.2.3a2/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/utils/imports.py` & `reflex-0.2.3a2/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/utils/path_ops.py` & `reflex-0.2.3a2/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/utils/prerequisites.py` & `reflex-0.2.3a2/reflex/utils/prerequisites.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,46 +21,45 @@
 from redis import Redis
 
 from reflex import constants, model
 from reflex.config import get_config
 from reflex.utils import console, path_ops
 
 
-def check_node_version(min_version=constants.MIN_NODE_VERSION):
+def check_node_version():
     """Check the version of Node.js.
 
-    Args:
-        min_version: The minimum version of Node.js required.
-
     Returns:
-        Whether the version of Node.js is high enough.
+        Whether the version of Node.js is valid.
     """
     try:
         # Run the node -v command and capture the output
         result = subprocess.run(
-            ["node", "-v"], stdout=subprocess.PIPE, stderr=subprocess.PIPE
+            [constants.NODE_PATH, "-v"],
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
         )
         # The output will be in the form "vX.Y.Z", but version.parse() can handle it
         current_version = version.parse(result.stdout.decode())
         # Compare the version numbers
-        return current_version >= version.parse(min_version)
+        return current_version == version.parse(constants.NODE_VERSION)
     except Exception:
         return False
 
 
 def get_bun_version() -> Optional[version.Version]:
     """Get the version of bun.
 
     Returns:
         The version of bun.
     """
     try:
         # Run the bun -v command and capture the output
         result = subprocess.run(
-            [os.path.expandvars(get_config().bun_path), "-v"],
+            [constants.BUN_PATH, "-v"],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         return version.parse(result.stdout.decode().strip())
     except Exception:
         return None
 
@@ -69,35 +68,26 @@
     """Get the package manager executable.
 
     Returns:
         The path to the package manager.
 
     Raises:
         FileNotFoundError: If bun or npm is not installed.
-        Exit: If the app directory is invalid.
-
     """
-    config = get_config()
-
-    # Check that the node version is valid.
-    if not check_node_version():
-        console.print(
-            f"[red]Node.js version {constants.MIN_NODE_VERSION} or higher is required to run Reflex."
-        )
-        raise typer.Exit()
+    get_config()
 
     # On Windows, we use npm instead of bun.
-    if platform.system() == "Windows" or config.disable_bun:
+    if platform.system() == "Windows":
         npm_path = path_ops.which("npm")
         if npm_path is None:
             raise FileNotFoundError("Reflex requires npm to be installed on Windows.")
         return npm_path
 
     # On other platforms, we use bun.
-    return os.path.expandvars(get_config().bun_path)
+    return constants.BUN_PATH
 
 
 def get_app() -> ModuleType:
     """Get the app module based on the default config.
 
     Returns:
         The app based on the default config.
@@ -139,15 +129,24 @@
     """Get the default app name.
 
     The default app name is the name of the current directory.
 
     Returns:
         The default app name.
     """
-    return os.getcwd().split(os.path.sep)[-1].replace("-", "_")
+    app_name = os.getcwd().split(os.path.sep)[-1].replace("-", "_")
+
+    # Make sure the app is not named "reflex".
+    if app_name == constants.MODULE_NAME:
+        console.print(
+            f"[red]The app directory cannot be named [bold]{constants.MODULE_NAME}."
+        )
+        raise typer.Exit()
+
+    return app_name
 
 
 def create_config(app_name: str):
     """Create a new rxconfig file.
 
     Args:
         app_name: The name of the app.
@@ -156,29 +155,14 @@
     from reflex.compiler import templates
 
     config_name = f"{re.sub(r'[^a-zA-Z]', '', app_name).capitalize()}Config"
     with open(constants.CONFIG_FILE, "w") as f:
         f.write(templates.RXCONFIG.render(app_name=app_name, config_name=config_name))
 
 
-def create_web_directory(root: Path) -> str:
-    """Creates a web directory in the given root directory
-    and returns the path to the directory.
-
-    Args:
-        root (Path): The root directory of the project.
-
-    Returns:
-        The path to the web directory.
-    """
-    web_dir = str(root / constants.WEB_DIR)
-    path_ops.cp(constants.WEB_TEMPLATE_DIR, web_dir, overwrite=False)
-    return web_dir
-
-
 def initialize_gitignore():
     """Initialize the template .gitignore file."""
     # The files to add to the .gitignore file.
     files = constants.DEFAULT_GITIGNORE
 
     # Subtract current ignored files.
     if os.path.exists(constants.GITIGNORE_FILE):
@@ -228,56 +212,77 @@
 
     # Write the current version of distributed reflex package to a REFLEX_JSON."""
     with open(constants.REFLEX_JSON, "w") as f:
         reflex_json = {"version": constants.VERSION}
         json.dump(reflex_json, f, ensure_ascii=False)
 
 
-def validate_and_install_bun(initialize=True):
-    """Check that bun version requirements are met. If they are not,
-    ask user whether to install required version.
-
-    Args:
-        initialize: whether this function is called on `reflex init` or `reflex run`.
+def initialize_bun():
+    """Check that bun requirements are met, and install if not.
 
     Raises:
         Exit: If the bun version is not supported.
 
     """
-    bun_version = get_bun_version()
-    if bun_version is not None and (
-        bun_version < version.parse(constants.MIN_BUN_VERSION)
-        or bun_version > version.parse(constants.MAX_BUN_VERSION)
-    ):
-        console.print(
-            f"""[red]Bun version {bun_version} is not supported by Reflex. Please change your to bun version to be between {constants.MIN_BUN_VERSION} and {constants.MAX_BUN_VERSION}."""
-        )
-        action = console.ask(
-            "Enter 'yes' to install the latest supported bun version or 'no' to exit.",
-            choices=["yes", "no"],
-            default="no",
-        )
-
-        if action == "yes":
-            remove_existing_bun_installation()
-            install_bun()
-            return
-        else:
-            raise typer.Exit()
+    if platform.system == "Windows":
+        # Bun is not supported on Windows.
+        return
 
-    if initialize:
+    # Check the bun version.
+    if get_bun_version() != version.parse(constants.BUN_VERSION):
+        remove_existing_bun_installation()
         install_bun()
 
 
 def remove_existing_bun_installation():
     """Remove existing bun installation."""
-    package_manager = get_package_manager()
-    if os.path.exists(package_manager):
-        console.log("Removing bun...")
-        path_ops.rm(os.path.expandvars(constants.BUN_ROOT_PATH))
+    if os.path.exists(constants.BUN_PATH):
+        path_ops.rm(constants.BUN_ROOT_PATH)
+
+
+def initialize_node():
+    """Validate nodejs have install or not."""
+    if not check_node_version():
+        install_node()
+
+
+def install_node():
+    """Install nvm and nodejs onto the user's system.
+
+
+    Raises:
+        FileNotFoundError: if unzip or curl packages are not found.
+        Exit: if installation failed
+    """
+    if platform.system() == "Windows":
+        console.print(
+            f"[red]Node.js version {constants.NODE_VERSION} or higher is required to run Reflex."
+        )
+        raise typer.Exit()
+
+    # Only install if bun is not already installed.
+    console.log("Installing nvm...")
+
+    # Check if curl is installed
+    curl_path = path_ops.which("curl")
+    if curl_path is None:
+        raise FileNotFoundError("Reflex requires curl to be installed.")
+
+    # Create the nvm directory and install.
+    path_ops.mkdir(constants.NVM_ROOT_PATH)
+    result = subprocess.run(constants.INSTALL_NVM, shell=True)
+
+    if result.returncode != 0:
+        raise typer.Exit(code=result.returncode)
+
+    console.log("Installing node...")
+    result = subprocess.run(constants.INSTALL_NODE, shell=True)
+
+    if result.returncode != 0:
+        raise typer.Exit(code=result.returncode)
 
 
 def install_bun():
     """Install bun onto the user's system.
 
     Raises:
         FileNotFoundError: if unzip or curl packages are not found.
@@ -304,37 +309,32 @@
 
         result = subprocess.run(constants.INSTALL_BUN, shell=True)
 
         if result.returncode != 0:
             raise typer.Exit(code=result.returncode)
 
 
-def install_frontend_packages(web_dir: str):
-    """Installs the base and custom frontend packages
-    into the given web directory.
-
-    Args:
-        web_dir: The directory where the frontend code is located.
-    """
+def install_frontend_packages():
+    """Installs the base and custom frontend packages."""
     # Install the frontend packages.
     console.rule("[bold]Installing frontend packages")
 
     # Install the base packages.
     subprocess.run(
         [get_package_manager(), "install"],
-        cwd=web_dir,
+        cwd=constants.WEB_DIR,
         stdout=subprocess.PIPE,
     )
 
     # Install the app packages.
     packages = get_config().frontend_packages
     if len(packages) > 0:
         subprocess.run(
             [get_package_manager(), "add", *packages],
-            cwd=web_dir,
+            cwd=constants.WEB_DIR,
             stdout=subprocess.PIPE,
         )
 
 
 def is_initialized() -> bool:
     """Check whether the app is initialized.
 
@@ -353,14 +353,27 @@
     if not os.path.exists(constants.REFLEX_JSON):
         return False
     with open(constants.REFLEX_JSON) as f:  # type: ignore
         app_version = json.load(f)["version"]
     return app_version == constants.VERSION
 
 
+def initialize_frontend_dependencies():
+    """Initialize all the frontend dependencies."""
+    # Create the reflex directory.
+    path_ops.mkdir(constants.REFLEX_DIR)
+
+    # Install the frontend dependencies.
+    initialize_bun()
+    initialize_node()
+
+    # Set up the web directory.
+    initialize_web_directory()
+
+
 def check_admin_settings():
     """Check if admin settings are set and valid for logging in cli app."""
     admin_dash = get_config().admin_dash
     current_time = datetime.now()
     if admin_dash:
         if not admin_dash.models:
             console.print(
```

### Comparing `reflex-0.2.3a1/reflex/utils/processes.py` & `reflex-0.2.3a2/reflex/utils/processes.py`

 * *Files 7% similar despite different names*

```diff
@@ -130,16 +130,18 @@
     Args:
         args: A string, or a sequence of program arguments.
         **kwargs: Kwargs to override default wrap values to pass to subprocess.Popen as arguments.
 
     Returns:
         Execute a child program in a new process.
     """
+    env = os.environ.copy()
+    env["PATH"] = os.pathsep.join([env["PATH"], constants.NODE_BIN_PATH])
     kwargs = {
-        "env": os.environ,
+        "env": env,
         "stderr": subprocess.STDOUT,
         "stdout": subprocess.PIPE,  # Redirect stdout to a pipe
         "universal_newlines": True,  # Set universal_newlines to True for text mode
         "encoding": "UTF-8",
         **kwargs,
     }
     return subprocess.Popen(
```

### Comparing `reflex-0.2.3a1/reflex/utils/telemetry.py` & `reflex-0.2.3a2/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/utils/types.py` & `reflex-0.2.3a2/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/utils/watch.py` & `reflex-0.2.3a2/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/reflex/vars.py` & `reflex-0.2.3a2/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a1/PKG-INFO` & `reflex-0.2.3a2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.2.3a1
+Version: 0.2.3a2
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
@@ -63,15 +63,15 @@
 
 </div>
 
 ### README in different language
 
 ---
 
-[English](README.md) | [简体中文](/docs/zh/zh_cn/README.md) | [繁體中文](/docs/zh/zh_tw/README.md)
+[English](https://github.com/reflex-dev/reflex/blob/main/README.md) | [简体中文](https://github.com/reflex-dev/reflex/blob/main/docs/zh/zh_cn/README.md) | [繁體中文](https://github.com/reflex-dev/reflex/blob/main/docs/zh/zh_tw/README.md)
 
 ---
 
 ## 📦 1. Install
 
 Reflex requires the following to get started:
```

