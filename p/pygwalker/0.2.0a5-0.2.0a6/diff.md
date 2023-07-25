# Comparing `tmp/pygwalker-0.2.0a5.tar.gz` & `tmp/pygwalker-0.2.0a6.tar.gz`

## Comparing `pygwalker-0.2.0a5.tar` & `pygwalker-0.2.0a6.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/.gitignore
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/index.html
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/package.json
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/postcss.config.js
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/tailwind.config.js
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/tsconfig.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/vite.config.ts
--rw-r--r--   0        0        0   133942 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/yarn.lock
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/index.css
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/index.tsx
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/components/defaultTab.tsx
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/components/loadingIcon.tsx
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/components/modal.tsx
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/components/options.tsx
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/components/button/base.ts
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/components/button/default.tsx
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/components/button/primary.tsx
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/components/codeExportModal/index.tsx
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/components/codeExportModal/saveConfigButton.tsx
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/components/initModal/index.tsx
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/dataSource/index.ts
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/interfaces/index.ts
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/notify/index.tsx
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/store/common.ts
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/store/communication.ts
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/tools/exportTool.tsx
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/tools/loginTool.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/tools/saveTool.tsx
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/utils/communication.ts
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/utils/graphicWalkerParser.ts
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/utils/save.ts
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/utils/screenshot.ts
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/app/src/utils/userConfig.ts
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/_constants.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/_typing.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/api/__init__.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/api/gwalker.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/api/html.py
--rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/api/pygwalker.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/api/walker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/communications/__init__.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/communications/base.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/communications/hacker_comm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/data_parsers/__init__.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/data_parsers/base.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/data_parsers/modin_parser.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/data_parsers/pandas_parser.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/data_parsers/polars_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/services/__init__.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/services/check_update.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/services/data_parsers.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/services/fname_encodings.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/services/format_invoke_walk_code.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/services/global_var.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/services/preview_image.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/services/render.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/services/spec.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/services/tip_tools.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/services/upload_data.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/.gitignore
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/index.html
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/preview.html
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/preview_list.html
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/pygwalker_iframe.html
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/walk.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/index.d.ts
--rw-r--r--   0        0        0  1935527 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/pygwalker-app.iife.js
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/components/defaultTab.d.ts
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/components/loadingIcon.d.ts
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/components/modal.d.ts
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/components/options.d.ts
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/components/button/base.d.ts
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/components/button/default.d.ts
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/components/button/primary.d.ts
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/components/codeExportModal/index.d.ts
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/components/codeExportModal/saveConfigButton.d.ts
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/components/initModal/index.d.ts
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/dataSource/index.d.ts
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/interfaces/index.d.ts
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/notify/index.d.ts
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/store/common.d.ts
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/store/communication.d.ts
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/tools/exportTool.d.ts
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/tools/loginTool.d.ts
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/tools/saveTool.d.ts
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/utils/communication.d.ts
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/utils/graphicWalkerParser.d.ts
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/utils/save.d.ts
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/utils/screenshot.d.ts
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/templates/dist/utils/userConfig.d.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/utils/__init__.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/utils/display.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/utils/encode.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/utils/execute_env_check.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/utils/log.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker/utils/randoms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker_utils/__init__.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker_utils/__main__.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker_utils/config.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pygwalker_utils/defaults.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/scripts/__init__.py
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/scripts/compile.sh
--rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/scripts/develop.sh
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/scripts/test-init.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/scripts/test-init.sh
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/.gitignore
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/LICENSE
--rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/README.md
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/pyproject.toml
--rw-r--r--   0        0        0    14582 2020-02-02 00:00:00.000000 pygwalker-0.2.0a5/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/index.html
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/package.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/postcss.config.js
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/tailwind.config.js
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/tsconfig.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/vite.config.ts
+-rw-r--r--   0        0        0   133942 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/yarn.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/index.css
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/index.tsx
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/components/defaultTab.tsx
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/components/loadingIcon.tsx
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/components/modal.tsx
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/components/options.tsx
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/components/button/base.ts
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/components/button/default.tsx
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/components/button/primary.tsx
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/components/codeExportModal/index.tsx
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/components/codeExportModal/saveConfigButton.tsx
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/components/initModal/index.tsx
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/dataSource/index.ts
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/interfaces/index.ts
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/notify/index.tsx
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/store/common.ts
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/store/communication.ts
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/tools/exportTool.tsx
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/tools/loginTool.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/tools/saveTool.tsx
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/utils/communication.ts
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/utils/graphicWalkerParser.ts
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/utils/save.ts
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/utils/screenshot.ts
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/app/src/utils/userConfig.ts
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/_constants.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/_typing.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/api/__init__.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/api/gwalker.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/api/html.py
+-rw-r--r--   0        0        0    10593 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/api/pygwalker.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/api/walker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/communications/__init__.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/communications/base.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/communications/hacker_comm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/data_parsers/__init__.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/data_parsers/base.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/data_parsers/modin_parser.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/data_parsers/pandas_parser.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/data_parsers/polars_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/services/__init__.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/services/check_update.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/services/data_parsers.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/services/fname_encodings.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/services/format_invoke_walk_code.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/services/global_var.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/services/preview_image.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/services/render.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/services/spec.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/services/tip_tools.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/services/upload_data.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/.gitignore
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/index.html
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/preview.html
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/preview_list.html
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/pygwalker_iframe.html
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/walk.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/index.d.ts
+-rw-r--r--   0        0        0  1935527 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/pygwalker-app.iife.js
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/components/defaultTab.d.ts
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/components/loadingIcon.d.ts
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/components/modal.d.ts
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/components/options.d.ts
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/components/button/base.d.ts
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/components/button/default.d.ts
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/components/button/primary.d.ts
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/components/codeExportModal/index.d.ts
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/components/codeExportModal/saveConfigButton.d.ts
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/components/initModal/index.d.ts
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/dataSource/index.d.ts
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/interfaces/index.d.ts
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/notify/index.d.ts
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/store/common.d.ts
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/store/communication.d.ts
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/tools/exportTool.d.ts
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/tools/loginTool.d.ts
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/tools/saveTool.d.ts
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/utils/communication.d.ts
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/utils/graphicWalkerParser.d.ts
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/utils/save.d.ts
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/utils/screenshot.d.ts
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/templates/dist/utils/userConfig.d.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/utils/__init__.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/utils/display.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/utils/encode.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/utils/execute_env_check.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/utils/log.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker/utils/randoms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker_utils/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker_utils/__main__.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker_utils/config.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pygwalker_utils/defaults.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/scripts/__init__.py
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/scripts/compile.sh
+-rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/scripts/develop.sh
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/scripts/test-init.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/scripts/test-init.sh
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/LICENSE
+-rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/README.md
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/pyproject.toml
+-rw-r--r--   0        0        0    14582 2020-02-02 00:00:00.000000 pygwalker-0.2.0a6/PKG-INFO
```

### Comparing `pygwalker-0.2.0a5/app/package.json` & `pygwalker-0.2.0a6/app/package.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/tsconfig.json` & `pygwalker-0.2.0a6/app/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/vite.config.ts` & `pygwalker-0.2.0a6/app/vite.config.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/yarn.lock` & `pygwalker-0.2.0a6/app/yarn.lock`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/index.tsx` & `pygwalker-0.2.0a6/app/src/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/components/defaultTab.tsx` & `pygwalker-0.2.0a6/app/src/components/defaultTab.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/components/loadingIcon.tsx` & `pygwalker-0.2.0a6/app/src/components/loadingIcon.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/components/modal.tsx` & `pygwalker-0.2.0a6/app/src/components/modal.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/components/options.tsx` & `pygwalker-0.2.0a6/app/src/components/options.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/components/button/default.tsx` & `pygwalker-0.2.0a6/app/src/components/button/default.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/components/button/primary.tsx` & `pygwalker-0.2.0a6/app/src/components/button/primary.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/components/codeExportModal/index.tsx` & `pygwalker-0.2.0a6/app/src/components/codeExportModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/components/codeExportModal/saveConfigButton.tsx` & `pygwalker-0.2.0a6/app/src/components/codeExportModal/saveConfigButton.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/components/initModal/index.tsx` & `pygwalker-0.2.0a6/app/src/components/initModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/dataSource/index.ts` & `pygwalker-0.2.0a6/app/src/dataSource/index.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/interfaces/index.ts` & `pygwalker-0.2.0a6/app/src/interfaces/index.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/notify/index.tsx` & `pygwalker-0.2.0a6/app/src/notify/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/store/common.ts` & `pygwalker-0.2.0a6/app/src/store/common.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/tools/exportTool.tsx` & `pygwalker-0.2.0a6/app/src/tools/exportTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/tools/loginTool.tsx` & `pygwalker-0.2.0a6/app/src/tools/loginTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/tools/saveTool.tsx` & `pygwalker-0.2.0a6/app/src/tools/saveTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/utils/communication.ts` & `pygwalker-0.2.0a6/app/src/utils/communication.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/utils/graphicWalkerParser.ts` & `pygwalker-0.2.0a6/app/src/utils/graphicWalkerParser.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/app/src/utils/save.ts` & `pygwalker-0.2.0a6/app/src/utils/save.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/__init__.py` & `pygwalker-0.2.0a6/pygwalker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # pylint: disable=wrong-import-position
 import logging
 
 from pygwalker.utils.randoms import rand_str as __rand_str
 from pygwalker_utils.config import get_config as __get_config
 
-__version__ = "0.2.0a5"
+__version__ = "0.2.0a6"
 __hash__ = __rand_str()
 
 from pygwalker.api.walker import walk
 from pygwalker.api.gwalker import GWalker
 from pygwalker.api.html import to_html
 from pygwalker.data_parsers.base import FieldSpec
```

### Comparing `pygwalker-0.2.0a5/pygwalker/_typing.py` & `pygwalker-0.2.0a6/pygwalker/_typing.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/api/gwalker.py` & `pygwalker-0.2.0a6/pygwalker/api/gwalker.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/api/html.py` & `pygwalker-0.2.0a6/pygwalker/api/html.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/api/pygwalker.py` & `pygwalker-0.2.0a6/pygwalker/api/pygwalker.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/api/walker.py` & `pygwalker-0.2.0a6/pygwalker/api/walker.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/communications/base.py` & `pygwalker-0.2.0a6/pygwalker/communications/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/communications/hacker_comm.py` & `pygwalker-0.2.0a6/pygwalker/communications/hacker_comm.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/data_parsers/base.py` & `pygwalker-0.2.0a6/pygwalker/data_parsers/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/data_parsers/modin_parser.py` & `pygwalker-0.2.0a6/pygwalker/data_parsers/modin_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/data_parsers/pandas_parser.py` & `pygwalker-0.2.0a6/pygwalker/data_parsers/pandas_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/data_parsers/polars_parser.py` & `pygwalker-0.2.0a6/pygwalker/data_parsers/polars_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/services/check_update.py` & `pygwalker-0.2.0a6/pygwalker/services/check_update.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/services/data_parsers.py` & `pygwalker-0.2.0a6/pygwalker/services/data_parsers.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/services/format_invoke_walk_code.py` & `pygwalker-0.2.0a6/pygwalker/services/format_invoke_walk_code.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/services/preview_image.py` & `pygwalker-0.2.0a6/pygwalker/services/preview_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,25 +48,27 @@
         desc=desc,
     )
 
     return html
 
 
 def render_preview_html_for_multi_charts(charts_map: Dict[str, ChartData], gid: str, preview_id: str) -> str:
+    tab_name = "tab-pyg-" + str(gid)
     items = []
     for chart_data in charts_map.values():
         div_id = f"{gid}-{chart_data.title}".replace(" ", "")
         chart_html = render_preview_html(chart_data, div_id, custom_title="")
         items.append({
             "tab_id": "tab-" + div_id,
             "chart_title": chart_data.title,
             "chart_html": chart_html
         })
 
     html = jinja_env.get_template("preview_list.html").render(
+        tab_name=tab_name,
         preview_id=preview_id,
         items=items
     )
 
     return html
```

### Comparing `pygwalker-0.2.0a5/pygwalker/services/render.py` & `pygwalker-0.2.0a6/pygwalker/services/render.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/services/spec.py` & `pygwalker-0.2.0a6/pygwalker/services/spec.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/services/tip_tools.py` & `pygwalker-0.2.0a6/pygwalker/services/tip_tools.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/services/upload_data.py` & `pygwalker-0.2.0a6/pygwalker/services/upload_data.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/templates/index.html` & `pygwalker-0.2.0a6/pygwalker/templates/index.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/templates/preview.html` & `pygwalker-0.2.0a6/pygwalker/templates/preview.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/templates/preview_list.html` & `pygwalker-0.2.0a6/pygwalker/templates/preview_list.html`

 * *Files 13% similar despite different names*

```diff
@@ -39,15 +39,19 @@
 </style>
 
 <body>
     <div id="{{ preview_id }}">
         <div class="tabs">
             {% for item in items %}
             <div class="tab-pane">
-                <input type="radio" name="tab" id="{{ item['tab_id'] }}" checked />
+                {% if loop.index == 1 %}
+                <input type="radio" name="{{ tab_name }}" id="{{ item['tab_id'] }}" checked />
+                {% else %}
+                <input type="radio" name="{{ tab_name }}" id="{{ item['tab_id'] }}" />
+                {% endif %}
                 <label class="tab-item" for="{{ item['tab_id'] }}">{{ item['chart_title'] }}</label>
                 <div class="tab-content">{{ item['chart_html'] | safe }}</div>
             </div>
             {% endfor %}
         </div>
     </div>
 </body>
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
 {% for item in items %}
-# {{ item['chart_title'] }}
+{% if loop.index == 1 %} # {% else %} o {% endif %} {{ item['chart_title'] }}
 {{ item['chart_html'] | safe }}
 {% endfor %}
```

### Comparing `pygwalker-0.2.0a5/pygwalker/templates/dist/pygwalker-app.iife.js` & `pygwalker-0.2.0a6/pygwalker/templates/dist/pygwalker-app.iife.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/templates/dist/interfaces/index.d.ts` & `pygwalker-0.2.0a6/pygwalker/templates/dist/interfaces/index.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/templates/dist/tools/saveTool.d.ts` & `pygwalker-0.2.0a6/pygwalker/templates/dist/tools/saveTool.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/templates/dist/utils/communication.d.ts` & `pygwalker-0.2.0a6/pygwalker/templates/dist/utils/communication.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker/utils/display.py` & `pygwalker-0.2.0a6/pygwalker/utils/display.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker_utils/__main__.py` & `pygwalker-0.2.0a6/pygwalker_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pygwalker_utils/config.py` & `pygwalker-0.2.0a6/pygwalker_utils/config.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/scripts/test-init.py` & `pygwalker-0.2.0a6/scripts/test-init.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/scripts/test-init.sh` & `pygwalker-0.2.0a6/scripts/test-init.sh`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/.gitignore` & `pygwalker-0.2.0a6/.gitignore`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/LICENSE` & `pygwalker-0.2.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/README.md` & `pygwalker-0.2.0a6/README.md`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/pyproject.toml` & `pygwalker-0.2.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a5/PKG-INFO` & `pygwalker-0.2.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygwalker
-Version: 0.2.0a5
+Version: 0.2.0a6
 Summary: pygwalker: Combining Jupyter Notebook with a Tableau-like UI
 Project-URL: homepage, https://github.com/Kanaries/pygwalker
 Project-URL: repository, https://github.com/Kanaries/pygwalker
 Author-email: "Asm.Def" <woojson@zju.edu.cn>
 License-File: LICENSE
 Keywords: data-analysis,data-exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygwalker Version: 0.2.0a5 Summary: pygwalker:
+Metadata-Version: 2.1 Name: pygwalker Version: 0.2.0a6 Summary: pygwalker:
 Combining Jupyter Notebook with a Tableau-like UI Project-URL: homepage, https:
 //github.com/Kanaries/pygwalker Project-URL: repository, https://github.com/
 Kanaries/pygwalker Author-email: "Asm.Def"
 zju.edu.cn> License-File: LICENSE Keywords: data-analysis,data-
 exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist: astor
```

