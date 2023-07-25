# Comparing `tmp/sanic-23.3.0.tar.gz` & `tmp/sanic-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanic-23.3.0.tar", last modified: Sun Mar 26 19:56:18 2023, max compression
+gzip compressed data, was "sanic-23.6.0.tar", last modified: Tue Jul 25 13:15:48 2023, max compression
```

## Comparing `sanic-23.3.0.tar` & `sanic-23.6.0.tar`

### file list

```diff
@@ -1,306 +1,316 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-26 19:56:02.000000 sanic-23.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-26 19:56:02.000000 sanic-23.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-26 19:56:02.000000 sanic-23.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-26 19:56:02.000000 sanic-23.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-03-26 19:56:18.431716 sanic-23.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-03-26 19:56:02.000000 sanic-23.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-26 19:56:02.000000 sanic-23.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.411716 sanic-23.3.0/sanic/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58849 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.411716 sanic-23.3.0/sanic/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/application/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/application/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/application/logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/application/motd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/application/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/application/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.411716 sanic-23.3.0/sanic/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/base/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/base/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/blueprint_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/blueprints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.411716 sanic-23.3.0/sanic/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/cli/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/cli/inspector_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.411716 sanic-23.3.0/sanic/cookies/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/cookies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/cookies/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/cookies/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11574 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/errorpages.py
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.411716 sanic-23.3.0/sanic/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/handlers/content_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/handlers/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/handlers/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15913 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.411716 sanic-23.3.0/sanic/http/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/http/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/http/http1.py
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/http/http3.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/http/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.415716 sanic-23.3.0/sanic/http/tls/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/http/tls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/http/tls/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/http/tls/creators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.415716 sanic-23.3.0/sanic/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/mixins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/mixins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/mixins/listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/mixins/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    26198 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/mixins/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/mixins/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    38350 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/mixins/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13466 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/mixins/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.415716 sanic-23.3.0/sanic/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/models/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/models/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/models/handler_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/models/http_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/models/protocol_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/models/server_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.415716 sanic-23.3.0/sanic/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/pages/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/pages/css.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/pages/directory_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/pages/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.415716 sanic-23.3.0/sanic/pages/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/pages/styles/BasePage.css
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/pages/styles/DirectoryPage.css
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/pages/styles/ErrorPage.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.415716 sanic-23.3.0/sanic/request/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/request/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/request/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/request/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.415716 sanic-23.3.0/sanic/response/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/response/convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)    17569 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/response/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.415716 sanic-23.3.0/sanic/server/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/async_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.419716 sanic-23.3.0/sanic/server/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/protocols/base_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/protocols/http_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/protocols/websocket_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.419716 sanic-23.3.0/sanic/server/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/websockets/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/websockets/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    35394 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/server/websockets/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.419716 sanic-23.3.0/sanic/touchup/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/touchup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/touchup/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.419716 sanic-23.3.0/sanic/touchup/schemes/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/touchup/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/touchup/schemes/altsvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/touchup/schemes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/touchup/schemes/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/touchup/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.419716 sanic-23.3.0/sanic/types/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/types/hashable_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/types/shared_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.419716 sanic-23.3.0/sanic/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/worker/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/worker/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/worker/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/worker/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/worker/multiplexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/worker/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/worker/reloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/worker/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-26 19:56:02.000000 sanic-23.3.0/sanic/worker/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.411716 sanic-23.3.0/sanic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-03-26 19:56:18.000000 sanic-23.3.0/sanic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-03-26 19:56:18.000000 sanic-23.3.0/sanic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 19:56:18.000000 sanic-23.3.0/sanic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-26 19:56:18.000000 sanic-23.3.0/sanic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-26 19:56:18.000000 sanic-23.3.0/sanic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-26 19:56:18.000000 sanic-23.3.0/sanic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-26 19:56:18.431716 sanic-23.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-03-26 19:56:02.000000 sanic-23.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.427716 sanic-23.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/asyncmock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.427716 sanic-23.3.0/tests/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/benchmark/test_route_resolution_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.427716 sanic-23.3.0/tests/certs/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/certs/createcerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.427716 sanic-23.3.0/tests/certs/invalid.certmissing/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/certs/invalid.certmissing/privkey.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.427716 sanic-23.3.0/tests/certs/localhost/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/certs/localhost/fullchain.pem
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/certs/localhost/privkey.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.427716 sanic-23.3.0/tests/certs/password/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/certs/password/fullchain.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/certs/password/privkey.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.427716 sanic-23.3.0/tests/certs/sanic.example/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/certs/sanic.example/fullchain.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/certs/sanic.example/privkey.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.427716 sanic-23.3.0/tests/fake/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/fake/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.427716 sanic-23.3.0/tests/http3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/http3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/http3/test_http_receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/http3/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/http3/test_session_ticket_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.407716 sanic-23.3.0/tests/performance/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.427716 sanic-23.3.0/tests/performance/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/performance/aiohttp/simple_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/tests/performance/bottle/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/performance/bottle/simple_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/tests/performance/falcon/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/performance/falcon/simple_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/tests/performance/golang/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/performance/golang/golang.http.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/tests/performance/kyoukai/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/performance/kyoukai/simple_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/tests/performance/sanic/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/performance/sanic/http_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/performance/sanic/simple_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/performance/sanic/varied_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/tests/performance/tornado/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/performance/tornado/simple_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/tests/performance/wheezy/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/performance/wheezy/simple_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/skip_test_custom_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/tests/static/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/static/app_test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/tests/static/bp/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/static/bp/decode me.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/static/bp/python.png
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/static/bp/test.file
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/static/decode me.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.407716 sanic-23.3.0/tests/static/nested/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/tests/static/nested/dir/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/static/nested/dir/foo.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/static/python.png
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/static/test.file
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/static/test.html
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_bad_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_blueprint_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_blueprint_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    29396 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_cancellederror.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_coffee.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15937 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_create_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_custom_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_dynamic_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16345 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_errorpages.py
--rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_exceptions_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_ext_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_graceful_shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_handler_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_http_alt_svc.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_json_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_json_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_keep_alive_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_late_adds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_middleware_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_motd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_multi_serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_named_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_payload_too_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_pipelining.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_reloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_request_cancel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_request_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_request_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    67088 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    30861 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_response_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_response_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_response_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    36009 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_server_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_server_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_signal_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    21445 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_static_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_test_client_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_timeout_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)    21841 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_touchup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_unix_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_url_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_url_for.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_url_for_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_utf8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_vhosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/test_ws_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:56:18.431716 sanic-23.3.0/tests/worker/
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/worker/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/worker/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/worker/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/worker/test_multiplexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/worker/test_reloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/worker/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/worker/test_shared_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/worker/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/worker/test_startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/worker/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-03-26 19:56:02.000000 sanic-23.3.0/tests/worker/test_worker_serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.164604 sanic-23.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 13:15:30.000000 sanic-23.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 13:15:30.000000 sanic-23.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-25 13:15:30.000000 sanic-23.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-25 13:15:30.000000 sanic-23.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-25 13:15:48.164604 sanic-23.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-25 13:15:30.000000 sanic-23.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-25 13:15:30.000000 sanic-23.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.124601 sanic-23.6.0/sanic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63523 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.124601 sanic-23.6.0/sanic/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/application/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/application/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/application/logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/application/motd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/application/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/application/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.124601 sanic-23.6.0/sanic/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/base/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/blueprint_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16199 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/blueprints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.124601 sanic-23.6.0/sanic/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/cli/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/cli/inspector_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.128602 sanic-23.6.0/sanic/cookies/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/cookies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/cookies/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/cookies/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/errorpages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23512 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.128602 sanic-23.6.0/sanic/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/handlers/content_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/handlers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/handlers/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15923 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.128602 sanic-23.6.0/sanic/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/http/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/http/http1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/http/http3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/http/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.128602 sanic-23.6.0/sanic/http/tls/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/http/tls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/http/tls/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/http/tls/creators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.132602 sanic-23.6.0/sanic/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/mixins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/mixins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/mixins/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/mixins/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26448 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/mixins/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/mixins/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39039 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/mixins/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13476 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/mixins/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.132602 sanic-23.6.0/sanic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/models/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/models/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/models/handler_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/models/http_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/models/protocol_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/models/server_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.132602 sanic-23.6.0/sanic/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/pages/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/pages/css.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/pages/directory_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/pages/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.132602 sanic-23.6.0/sanic/pages/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/pages/styles/BasePage.css
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/pages/styles/DirectoryPage.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/pages/styles/ErrorPage.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.132602 sanic-23.6.0/sanic/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/request/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/request/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32846 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/request/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.132602 sanic-23.6.0/sanic/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/response/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17704 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/response/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.136602 sanic-23.6.0/sanic/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/async_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.136602 sanic-23.6.0/sanic/server/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/protocols/base_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/protocols/http_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/protocols/websocket_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.136602 sanic-23.6.0/sanic/server/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/websockets/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/websockets/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35410 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/server/websockets/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.136602 sanic-23.6.0/sanic/touchup/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/touchup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/touchup/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.136602 sanic-23.6.0/sanic/touchup/schemes/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/touchup/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/touchup/schemes/altsvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/touchup/schemes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/touchup/schemes/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/touchup/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.136602 sanic-23.6.0/sanic/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/types/hashable_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/types/shared_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.140602 sanic-23.6.0/sanic/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/worker/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/worker/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/worker/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/worker/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/worker/multiplexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/worker/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/worker/reloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/worker/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-25 13:15:30.000000 sanic-23.6.0/sanic/worker/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.124601 sanic-23.6.0/sanic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-25 13:15:48.000000 sanic-23.6.0/sanic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-07-25 13:15:48.000000 sanic-23.6.0/sanic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:15:48.000000 sanic-23.6.0/sanic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 13:15:48.000000 sanic-23.6.0/sanic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-25 13:15:48.000000 sanic-23.6.0/sanic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 13:15:48.000000 sanic-23.6.0/sanic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 13:15:48.164604 sanic-23.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-25 13:15:30.000000 sanic-23.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.152603 sanic-23.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/asyncmock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.152603 sanic-23.6.0/tests/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/benchmark/test_route_resolution_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.152603 sanic-23.6.0/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/certs/createcerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.152603 sanic-23.6.0/tests/certs/invalid.certmissing/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/certs/invalid.certmissing/privkey.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.152603 sanic-23.6.0/tests/certs/localhost/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/certs/localhost/fullchain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/certs/localhost/privkey.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.152603 sanic-23.6.0/tests/certs/password/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/certs/password/fullchain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/certs/password/privkey.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/certs/sanic.example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/certs/sanic.example/fullchain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/certs/sanic.example/privkey.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/fake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/fake/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/http3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/http3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/http3/test_http_receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/http3/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/http3/test_session_ticket_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.116601 sanic-23.6.0/tests/performance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/performance/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/performance/aiohttp/simple_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/performance/bottle/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/performance/bottle/simple_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/performance/falcon/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/performance/falcon/simple_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/performance/golang/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/performance/golang/golang.http.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/performance/kyoukai/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/performance/kyoukai/simple_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/performance/sanic/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/performance/sanic/http_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/performance/sanic/simple_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/performance/sanic/varied_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/performance/tornado/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/performance/tornado/simple_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/performance/wheezy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/performance/wheezy/simple_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/skip_test_custom_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.156603 sanic-23.6.0/tests/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/static/app_test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.160604 sanic-23.6.0/tests/static/bp/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/static/bp/decode me.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/static/bp/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/static/bp/test.file
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/static/decode me.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.116601 sanic-23.6.0/tests/static/nested/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.160604 sanic-23.6.0/tests/static/nested/dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/static/nested/dir/foo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/static/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/static/test.file
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/static/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18033 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_blueprint_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11629 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_blueprint_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29396 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_cancellederror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_coffee.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15937 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_create_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_custom_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_dynamic_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_errorpages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_exceptions_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_ext_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_graceful_shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_handler_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_http_alt_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_json_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_json_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_keep_alive_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_late_adds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_middleware_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_motd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_multi_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_named_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_payload_too_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_pipelining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_reloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_request_cancel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_request_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_request_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67176 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_response_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_response_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_response_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36009 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_server_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_server_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_signal_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22170 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_static_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_test_client_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_timeout_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21841 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_touchup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_unix_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_url_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_url_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_url_for_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_utf8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_vhosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/test_ws_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.160604 sanic-23.6.0/tests/typing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.160604 sanic-23.6.0/tests/typing/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/typing/samples/app_custom_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/typing/samples/app_custom_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/typing/samples/app_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/typing/samples/app_fully_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/typing/samples/request_custom_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/typing/samples/request_custom_sanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/typing/samples/request_fully_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/typing/test_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:15:48.164604 sanic-23.6.0/tests/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/worker/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/worker/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/worker/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/worker/test_multiplexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/worker/test_reloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/worker/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/worker/test_shared_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/worker/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/worker/test_startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/worker/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-25 13:15:30.000000 sanic-23.6.0/tests/worker/test_worker_serve.py
```

### Comparing `sanic-23.3.0/LICENSE` & `sanic-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/Makefile` & `sanic-23.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/PKG-INFO` & `sanic-23.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: sanic
-Version: 23.3.0
+Version: 23.6.0
 Summary: A web server and web framework that's written to go fast. Build fast. Run fast.
 Home-page: http://github.com/sanic-org/sanic/
 Author: Sanic Community
 Author-email: admhpkns@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: all
 Provides-Extra: ext
 Provides-Extra: http3
 License-File: LICENSE
@@ -190,9 +189,7 @@
 
 We are always happy to have new contributions. We have `marked issues good for anyone looking to get started <https://github.com/sanic-org/sanic/issues?q=is%3Aopen+is%3Aissue+label%3Abeginner>`_, and welcome `questions on the forums <https://community.sanicframework.org/>`_. Please take a look at our `Contribution guidelines <https://github.com/sanic-org/sanic/blob/master/CONTRIBUTING.rst>`_.
 
 .. |Linode| image:: https://www.linode.com/wp-content/uploads/2021/01/Linode-Logo-Black.svg
     :alt: Linode
     :target: https://www.linode.com
     :width: 200px
-
-
```

### Comparing `sanic-23.3.0/README.rst` & `sanic-23.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/pyproject.toml` & `sanic-23.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools<60.0", "wheel"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 79
 
 [tool.isort]
 atomic = true
```

### Comparing `sanic-23.3.0/sanic/app.py` & `sanic-23.6.0/sanic/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,38 +13,42 @@
     ensure_future,
     get_running_loop,
     wait_for,
 )
 from asyncio.futures import Future
 from collections import defaultdict, deque
 from contextlib import contextmanager, suppress
-from functools import partial
+from functools import partial, wraps
 from inspect import isawaitable
 from os import environ
 from socket import socket
 from traceback import format_exc
 from types import SimpleNamespace
 from typing import (
     TYPE_CHECKING,
     Any,
     AnyStr,
     Awaitable,
     Callable,
+    ClassVar,
     Coroutine,
     Deque,
     Dict,
+    Generic,
     Iterable,
     Iterator,
     List,
     Optional,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
+    cast,
+    overload,
 )
 from urllib.parse import urlencode, urlunparse
 
 from sanic_routing.exceptions import FinalizationError, NotFound
 from sanic_routing.route import Route
 
 from sanic.application.ext import setup_ext
@@ -79,15 +83,15 @@
 )
 from sanic.models.handler_types import ListenerType, MiddlewareType
 from sanic.models.handler_types import Sanic as SanicVar
 from sanic.request import Request
 from sanic.response import BaseHTTPResponse, HTTPResponse, ResponseStream
 from sanic.router import Router
 from sanic.server.websockets.impl import ConnectionClosed
-from sanic.signals import Signal, SignalRouter
+from sanic.signals import Event, Signal, SignalRouter
 from sanic.touchup import TouchUp, TouchUpMeta
 from sanic.types.shared_ctx import SharedContext
 from sanic.worker.inspector import Inspector
 from sanic.worker.loader import CertLoader
 from sanic.worker.manager import WorkerManager
 
 
@@ -98,16 +102,25 @@
     except ImportError:
         Extend = TypeVar("Extend", Type)  # type: ignore
 
 
 if OS_IS_WINDOWS:  # no cov
     enable_windows_color_support()
 
+ctx_type = TypeVar("ctx_type")
+config_type = TypeVar("config_type", bound=Config)
 
-class Sanic(StaticHandleMixin, BaseSanic, StartupMixin, metaclass=TouchUpMeta):
+
+class Sanic(
+    Generic[config_type, ctx_type],
+    StaticHandleMixin,
+    BaseSanic,
+    StartupMixin,
+    metaclass=TouchUpMeta,
+):
     """
     The main application instance
     """
 
     __touchup__ = (
         "handle_request",
         "handle_exception",
@@ -154,22 +167,110 @@
         "signal_router",
         "sock",
         "strict_slashes",
         "websocket_enabled",
         "websocket_tasks",
     )
 
-    _app_registry: Dict[str, "Sanic"] = {}
-    test_mode = False
+    _app_registry: ClassVar[Dict[str, "Sanic"]] = {}
+    test_mode: ClassVar[bool] = False
+
+    @overload
+    def __init__(
+        self: Sanic[Config, SimpleNamespace],
+        name: str,
+        config: None = None,
+        ctx: None = None,
+        router: Optional[Router] = None,
+        signal_router: Optional[SignalRouter] = None,
+        error_handler: Optional[ErrorHandler] = None,
+        env_prefix: Optional[str] = SANIC_PREFIX,
+        request_class: Optional[Type[Request]] = None,
+        strict_slashes: bool = False,
+        log_config: Optional[Dict[str, Any]] = None,
+        configure_logging: bool = True,
+        dumps: Optional[Callable[..., AnyStr]] = None,
+        loads: Optional[Callable[..., Any]] = None,
+        inspector: bool = False,
+        inspector_class: Optional[Type[Inspector]] = None,
+        certloader_class: Optional[Type[CertLoader]] = None,
+    ) -> None:
+        ...
+
+    @overload
+    def __init__(
+        self: Sanic[config_type, SimpleNamespace],
+        name: str,
+        config: Optional[config_type] = None,
+        ctx: None = None,
+        router: Optional[Router] = None,
+        signal_router: Optional[SignalRouter] = None,
+        error_handler: Optional[ErrorHandler] = None,
+        env_prefix: Optional[str] = SANIC_PREFIX,
+        request_class: Optional[Type[Request]] = None,
+        strict_slashes: bool = False,
+        log_config: Optional[Dict[str, Any]] = None,
+        configure_logging: bool = True,
+        dumps: Optional[Callable[..., AnyStr]] = None,
+        loads: Optional[Callable[..., Any]] = None,
+        inspector: bool = False,
+        inspector_class: Optional[Type[Inspector]] = None,
+        certloader_class: Optional[Type[CertLoader]] = None,
+    ) -> None:
+        ...
+
+    @overload
+    def __init__(
+        self: Sanic[Config, ctx_type],
+        name: str,
+        config: None = None,
+        ctx: Optional[ctx_type] = None,
+        router: Optional[Router] = None,
+        signal_router: Optional[SignalRouter] = None,
+        error_handler: Optional[ErrorHandler] = None,
+        env_prefix: Optional[str] = SANIC_PREFIX,
+        request_class: Optional[Type[Request]] = None,
+        strict_slashes: bool = False,
+        log_config: Optional[Dict[str, Any]] = None,
+        configure_logging: bool = True,
+        dumps: Optional[Callable[..., AnyStr]] = None,
+        loads: Optional[Callable[..., Any]] = None,
+        inspector: bool = False,
+        inspector_class: Optional[Type[Inspector]] = None,
+        certloader_class: Optional[Type[CertLoader]] = None,
+    ) -> None:
+        ...
+
+    @overload
+    def __init__(
+        self: Sanic[config_type, ctx_type],
+        name: str,
+        config: Optional[config_type] = None,
+        ctx: Optional[ctx_type] = None,
+        router: Optional[Router] = None,
+        signal_router: Optional[SignalRouter] = None,
+        error_handler: Optional[ErrorHandler] = None,
+        env_prefix: Optional[str] = SANIC_PREFIX,
+        request_class: Optional[Type[Request]] = None,
+        strict_slashes: bool = False,
+        log_config: Optional[Dict[str, Any]] = None,
+        configure_logging: bool = True,
+        dumps: Optional[Callable[..., AnyStr]] = None,
+        loads: Optional[Callable[..., Any]] = None,
+        inspector: bool = False,
+        inspector_class: Optional[Type[Inspector]] = None,
+        certloader_class: Optional[Type[CertLoader]] = None,
+    ) -> None:
+        ...
 
     def __init__(
         self,
-        name: Optional[str] = None,
-        config: Optional[Config] = None,
-        ctx: Optional[Any] = None,
+        name: str,
+        config: Optional[config_type] = None,
+        ctx: Optional[ctx_type] = None,
         router: Optional[Router] = None,
         signal_router: Optional[SignalRouter] = None,
         error_handler: Optional[ErrorHandler] = None,
         env_prefix: Optional[str] = SANIC_PREFIX,
         request_class: Optional[Type[Request]] = None,
         strict_slashes: bool = False,
         log_config: Optional[Dict[str, Any]] = None,
@@ -189,15 +290,17 @@
         if config and env_prefix != SANIC_PREFIX:
             raise SanicException(
                 "When instantiating Sanic with config, you cannot also pass "
                 "env_prefix"
             )
 
         # First setup config
-        self.config: Config = config or Config(env_prefix=env_prefix)
+        self.config: config_type = cast(
+            config_type, config or Config(env_prefix=env_prefix)
+        )
         if inspector:
             self.config.INSPECTOR = inspector
 
         # Then we can do the rest
         self._asgi_app: Optional[ASGIApp] = None
         self._asgi_lifespan: Optional[Lifespan] = None
         self._asgi_client: Any = None
@@ -213,15 +316,15 @@
         self.asgi = False
         self.auto_reload = False
         self.blueprints: Dict[str, Blueprint] = {}
         self.certloader_class: Type[CertLoader] = (
             certloader_class or CertLoader
         )
         self.configure_logging: bool = configure_logging
-        self.ctx: Any = ctx or SimpleNamespace()
+        self.ctx: ctx_type = cast(ctx_type, ctx or SimpleNamespace())
         self.error_handler: ErrorHandler = error_handler or ErrorHandler()
         self.inspector_class: Type[Inspector] = inspector_class or Inspector
         self.listeners: Dict[str, List[ListenerType[Any]]] = defaultdict(list)
         self.named_request_middleware: Dict[str, Deque[MiddlewareType]] = {}
         self.named_response_middleware: Dict[str, Deque[MiddlewareType]] = {}
         self.request_class: Type[Request] = request_class or Request
         self.request_middleware: Deque[MiddlewareType] = deque()
@@ -413,16 +516,19 @@
             else:
                 self.error_handler.add(exception, handler.handler, route_names)
         return handler.handler
 
     def _apply_listener(self, listener: FutureListener):
         return self.register_listener(listener.listener, listener.event)
 
-    def _apply_route(self, route: FutureRoute) -> List[Route]:
+    def _apply_route(
+        self, route: FutureRoute, overwrite: bool = False
+    ) -> List[Route]:
         params = route._asdict()
+        params["overwrite"] = overwrite
         websocket = params.pop("websocket", False)
         subprotocols = params.pop("subprotocols", None)
 
         if websocket:
             self.enable_websocket()
             websocket_handler = partial(
                 self._websocket_handler,
@@ -495,14 +601,27 @@
                 self.add_signal(None, event)
                 signal = self.signal_router.name_index[event]
                 self.signal_router.finalize()
             else:
                 raise NotFound("Could not find signal %s" % event)
         return await wait_for(signal.ctx.event.wait(), timeout=timeout)
 
+    def report_exception(
+        self, handler: Callable[[Sanic, Exception], Coroutine[Any, Any, None]]
+    ):
+        @wraps(handler)
+        async def report(exception: Exception) -> None:
+            await handler(self, exception)
+
+        self.add_signal(
+            handler=report, event=Event.SERVER_EXCEPTION_REPORT.value
+        )
+
+        return report
+
     def enable_websocket(self, enable=True):
         """Enable or disable the support for websocket.
 
         Websocket is enabled automatically if websocket routes are
         added to the application.
         """
         if not self.websocket_enabled:
@@ -546,14 +665,17 @@
                     if item.version_prefix == "/v":
                         if blueprint.version_prefix == "/v":
                             params["version_prefix"] = options.get(
                                 "version_prefix"
                             )
                         else:
                             params["version_prefix"] = blueprint.version_prefix
+                    name_prefix = getattr(blueprint, "name_prefix", None)
+                    if name_prefix and "name_prefix" not in params:
+                        params["name_prefix"] = name_prefix
                 self.blueprint(item, **params)
             return
         if blueprint.name in self.blueprints:
             assert self.blueprints[blueprint.name] is blueprint, (
                 'A blueprint with the name "%s" is already registered.  '
                 "Blueprint names must be unique." % (blueprint.name,)
             )
@@ -763,14 +885,20 @@
         A handler that catches specific exceptions and outputs a response.
 
         :param request: The current request object
         :param exception: The exception that was raised
         :raises ServerError: response 500
         """
         response = None
+        if not getattr(exception, "__dispatched__", False):
+            ...  # DO NOT REMOVE THIS LINE. IT IS NEEDED FOR TOUCHUP.
+            await self.dispatch(
+                "server.exception.report",
+                context={"exception": exception},
+            )
         await self.dispatch(
             "http.lifecycle.exception",
             inline=True,
             context={"request": request, "exception": exception},
         )
 
         if (
@@ -1193,46 +1321,52 @@
     @classmethod
     def _prep_task(
         cls,
         task,
         app,
         loop,
     ):
-        if callable(task):
+        async def do(task):
             try:
-                task = task(app)
-            except TypeError:
-                task = task()
+                if callable(task):
+                    try:
+                        task = task(app)
+                    except TypeError:
+                        task = task()
+                if isawaitable(task):
+                    await task
+            except CancelledError:
+                error_logger.warning(
+                    f"Task {task} was cancelled before it completed."
+                )
+                raise
+            except Exception as e:
+                await app.dispatch(
+                    "server.exception.report",
+                    context={"exception": e},
+                )
+                raise
 
-        return task
+        return do(task)
 
     @classmethod
     def _loop_add_task(
         cls,
         task,
         app,
         loop,
         *,
         name: Optional[str] = None,
         register: bool = True,
     ) -> Task:
         if not isinstance(task, Future):
             prepped = cls._prep_task(task, app, loop)
-            if sys.version_info < (3, 8):  # no cov
-                task = loop.create_task(prepped)
-                if name:
-                    error_logger.warning(
-                        "Cannot set a name for a task when using Python 3.7. "
-                        "Your task will be created without a name."
-                    )
-                task.get_name = lambda: name
-            else:
-                task = loop.create_task(prepped, name=name)
+            task = loop.create_task(prepped, name=name)
 
-        if name and register and sys.version_info > (3, 7):
+        if name and register:
             app._task_registry[name] = task
 
         return task
 
     @staticmethod
     async def dispatch_delayed_tasks(app, loop):
         for name in app._delayed_tasks:
```

### Comparing `sanic-23.3.0/sanic/application/constants.py` & `sanic-23.6.0/sanic/application/constants.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/application/ext.py` & `sanic-23.6.0/sanic/application/ext.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/application/logo.py` & `sanic-23.6.0/sanic/application/logo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import sys
 
 from os import environ
 
-from sanic.compat import is_atty
+from sanic.helpers import is_atty
 
 
 BASE_LOGO = """
 
                  Sanic
          Build Fast. Run Fast.
```

### Comparing `sanic-23.3.0/sanic/application/motd.py` & `sanic-23.6.0/sanic/application/motd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from shutil import get_terminal_size
 from textwrap import indent, wrap
 from typing import Dict, Optional
 
 from sanic import __version__
-from sanic.compat import is_atty
+from sanic.helpers import is_atty
 from sanic.log import logger
 
 
 class MOTD(ABC):
     def __init__(
         self,
         logo: Optional[str],
```

### Comparing `sanic-23.3.0/sanic/application/spinner.py` & `sanic-23.6.0/sanic/application/spinner.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/application/state.py` & `sanic-23.6.0/sanic/application/state.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/asgi.py` & `sanic-23.6.0/sanic/asgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,15 @@
             url_bytes,
             headers,
             version,
             method,
             instance.transport,
             sanic_app,
         )
+        request_class._current.set(instance.request)
         instance.request.stream = instance  # type: ignore
         instance.request_body = True
         instance.request.conn_info = ConnInfo(instance.transport)
 
         await instance.sanic_app.dispatch(
             "http.lifecycle.request",
             inline=True,
```

### Comparing `sanic-23.3.0/sanic/base/root.py` & `sanic-23.6.0/sanic/base/root.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/blueprint_group.py` & `sanic-23.6.0/sanic/blueprint_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,36 +61,39 @@
 
     __slots__ = (
         "_blueprints",
         "_url_prefix",
         "_version",
         "_strict_slashes",
         "_version_prefix",
+        "_name_prefix",
     )
 
     def __init__(
         self,
         url_prefix: Optional[str] = None,
         version: Optional[Union[int, str, float]] = None,
         strict_slashes: Optional[bool] = None,
         version_prefix: str = "/v",
+        name_prefix: Optional[str] = "",
     ):
         """
         Create a new Blueprint Group
 
         :param url_prefix: URL: to be prefixed before all the Blueprint Prefix
         :param version: API Version for the blueprint group. This will be
             inherited by each of the Blueprint
         :param strict_slashes: URL Strict slash behavior indicator
         """
         self._blueprints: List[Blueprint] = []
         self._url_prefix = url_prefix
         self._version = version
         self._version_prefix = version_prefix
         self._strict_slashes = strict_slashes
+        self._name_prefix = name_prefix
 
     @property
     def url_prefix(self) -> Optional[Union[int, str, float]]:
         """
         Retrieve the URL prefix being used for the Current Blueprint Group
 
         :return: string with url prefix
@@ -130,14 +133,23 @@
         """
         Version prefix; defaults to ``/v``
 
         :return: str
         """
         return self._version_prefix
 
+    @property
+    def name_prefix(self) -> Optional[str]:
+        """
+        Name prefix for the blueprint group
+
+        :return: str
+        """
+        return self._name_prefix
+
     def __iter__(self):
         """
         Tun the class Blueprint Group into an Iterable item
         """
         return iter(self._blueprints)
 
     def __getitem__(self, item):
```

### Comparing `sanic-23.3.0/sanic/blueprints.py` & `sanic-23.6.0/sanic/blueprints.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         "_apps",
         "_future_routes",
         "_future_statics",
         "_future_middleware",
         "_future_listeners",
         "_future_exceptions",
         "_future_signals",
+        "_allow_route_overwrite",
         "copied_from",
         "ctx",
         "exceptions",
         "host",
         "listeners",
         "middlewares",
         "routes",
@@ -106,23 +107,24 @@
         "version",
         "version_prefix",
         "websocket_routes",
     )
 
     def __init__(
         self,
-        name: str = None,
+        name: str,
         url_prefix: Optional[str] = None,
         host: Optional[Union[List[str], str]] = None,
         version: Optional[Union[int, str, float]] = None,
         strict_slashes: Optional[bool] = None,
         version_prefix: str = "/v",
     ):
         super().__init__(name=name)
         self.reset()
+        self._allow_route_overwrite = False
         self.copied_from = ""
         self.ctx = SimpleNamespace()
         self.host = host
         self.strict_slashes = strict_slashes
         self.url_prefix = (
             url_prefix[:-1]
             if url_prefix and url_prefix.endswith("/")
@@ -165,27 +167,29 @@
     middleware = lazy(BaseSanic.middleware)
     route = lazy(BaseSanic.route)
     signal = lazy(BaseSanic.signal)
     static = lazy(BaseSanic.static, as_decorator=False)
 
     def reset(self):
         self._apps: Set[Sanic] = set()
+        self._allow_route_overwrite = False
         self.exceptions: List[RouteHandler] = []
         self.listeners: Dict[str, List[ListenerType[Any]]] = {}
         self.middlewares: List[MiddlewareType] = []
         self.routes: List[Route] = []
         self.statics: List[RouteHandler] = []
         self.websocket_routes: List[Route] = []
 
     def copy(
         self,
         name: str,
         url_prefix: Optional[Union[str, Default]] = _default,
         version: Optional[Union[int, str, float, Default]] = _default,
         version_prefix: Union[str, Default] = _default,
+        allow_route_overwrite: Union[bool, Default] = _default,
         strict_slashes: Optional[Union[bool, Default]] = _default,
         with_registration: bool = True,
         with_ctx: bool = False,
     ):
         """
         Copy a blueprint instance with some optional parameters to
         override the values of attributes in the old instance.
@@ -221,14 +225,16 @@
             new_bp.url_prefix = url_prefix
         if not isinstance(version, Default):
             new_bp.version = version
         if not isinstance(strict_slashes, Default):
             new_bp.strict_slashes = strict_slashes
         if not isinstance(version_prefix, Default):
             new_bp.version_prefix = version_prefix
+        if not isinstance(allow_route_overwrite, Default):
+            new_bp._allow_route_overwrite = allow_route_overwrite
 
         for key, value in attrs_backup.items():
             setattr(self, key, value)
 
         if with_registration and self._apps:
             if new_bp._future_statics:
                 raise SanicException(
@@ -246,14 +252,15 @@
     @staticmethod
     def group(
         *blueprints: Union[Blueprint, BlueprintGroup],
         url_prefix: Optional[str] = None,
         version: Optional[Union[int, str, float]] = None,
         strict_slashes: Optional[bool] = None,
         version_prefix: str = "/v",
+        name_prefix: Optional[str] = "",
     ) -> BlueprintGroup:
         """
         Create a list of blueprints, optionally grouping them under a
         general URL prefix.
 
         :param blueprints: blueprints to be registered as a group
         :param url_prefix: URL route to be prepended to all sub-prefixes
@@ -271,14 +278,15 @@
                     yield i
 
         bps = BlueprintGroup(
             url_prefix=url_prefix,
             version=version,
             strict_slashes=strict_slashes,
             version_prefix=version_prefix,
+            name_prefix=name_prefix,
         )
         for bp in chain(blueprints):
             bps.append(bp)
         return bps
 
     def register(self, app, options):
         """
@@ -291,14 +299,15 @@
         """
 
         self._apps.add(app)
         url_prefix = options.get("url_prefix", self.url_prefix)
         opt_version = options.get("version", None)
         opt_strict_slashes = options.get("strict_slashes", None)
         opt_version_prefix = options.get("version_prefix", self.version_prefix)
+        opt_name_prefix = options.get("name_prefix", None)
         error_format = options.get(
             "error_format", app.config.FALLBACK_ERROR_FORMAT
         )
 
         routes = []
         middleware = []
         exception_handlers = []
@@ -306,14 +315,18 @@
         registered = set()
 
         # Routes
         for future in self._future_routes:
             # Prepend the blueprint URI prefix if available
             uri = self._setup_uri(future.uri, url_prefix)
 
+            route_error_format = (
+                future.error_format if future.error_format else error_format
+            )
+
             version_prefix = self.version_prefix
             for prefix in (
                 future.version_prefix,
                 opt_version_prefix,
             ):
                 if prefix and prefix != "/v":
                     version_prefix = prefix
@@ -322,15 +335,18 @@
             version = self._extract_value(
                 future.version, opt_version, self.version
             )
             strict_slashes = self._extract_value(
                 future.strict_slashes, opt_strict_slashes, self.strict_slashes
             )
 
-            name = app._generate_name(future.name)
+            name = future.name
+            if opt_name_prefix:
+                name = f"{opt_name_prefix}_{future.name}"
+            name = app._generate_name(name)
             host = future.host or self.host
             if isinstance(host, list):
                 host = tuple(host)
 
             apply_route = FutureRoute(
                 future.handler,
                 uri,
@@ -342,23 +358,25 @@
                 name,
                 future.ignore_body,
                 future.websocket,
                 future.subprotocols,
                 future.unquote,
                 future.static,
                 version_prefix,
-                error_format,
+                route_error_format,
                 future.route_context,
             )
 
             if (self, apply_route) in app._future_registry:
                 continue
 
             registered.add(apply_route)
-            route = app._apply_route(apply_route)
+            route = app._apply_route(
+                apply_route, overwrite=self._allow_route_overwrite
+            )
 
             # If it is a copied BP, then make sure all of the names of routes
             # matchup with the new BP name
             if self.copied_from:
                 for r in route:
                     r.name = r.name.replace(self.copied_from, self.name)
                     r.extra.ident = r.extra.ident.replace(
```

### Comparing `sanic-23.3.0/sanic/cli/app.py` & `sanic-23.6.0/sanic/cli/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,18 @@
         except ImportError as e:
             if app_loader.module_name.startswith(e.name):  # type: ignore
                 error_logger.error(
                     f"No module named {e.name} found.\n"
                     "  Example File: project/sanic_server.py -> app\n"
                     "  Example Module: project.sanic_server.app"
                 )
+                error_logger.error(
+                    "\nThe error below might have caused the above one:\n"
+                    f"{e.msg}"
+                )
                 sys.exit(1)
             else:
                 raise e
         return app
 
     def _build_run_kwargs(self):
         for group in self.groups:
```

### Comparing `sanic-23.3.0/sanic/cli/arguments.py` & `sanic-23.6.0/sanic/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/cli/base.py` & `sanic-23.6.0/sanic/cli/base.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/cli/inspector.py` & `sanic-23.6.0/sanic/cli/inspector.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/cli/inspector_client.py` & `sanic-23.6.0/sanic/cli/inspector_client.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/compat.py` & `sanic-23.6.0/sanic/compat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import asyncio
 import os
+import platform
 import signal
 import sys
 
 from contextlib import contextmanager
 from enum import Enum
 from typing import Awaitable, Union
 
 from multidict import CIMultiDict  # type: ignore
 
 from sanic.helpers import Default
+from sanic.log import error_logger
 
 
 if sys.version_info < (3, 8):  # no cov
     StartMethod = Union[Default, str]
 else:  # no cov
     from typing import Literal
 
     StartMethod = Union[
         Default, Literal["fork"], Literal["forkserver"], Literal["spawn"]
     ]
 
 OS_IS_WINDOWS = os.name == "nt"
+PYPY_IMPLEMENTATION = platform.python_implementation() == "PyPy"
 UVLOOP_INSTALLED = False
 
 try:
     import uvloop  # type: ignore # noqa
 
     UVLOOP_INSTALLED = True
 except ImportError:
@@ -69,28 +72,60 @@
 def enable_windows_color_support():
     import ctypes
 
     kernel = ctypes.windll.kernel32
     kernel.SetConsoleMode(kernel.GetStdHandle(-11), 7)
 
 
+def pypy_os_module_patch() -> None:
+    """
+    The PyPy os module is missing the 'readlink' function, which causes issues
+    withaiofiles. This workaround replaces the missing 'readlink' function
+    with 'os.path.realpath', which serves the same purpose.
+    """
+    if hasattr(os, "readlink"):
+        error_logger.warning(
+            "PyPy: Skipping patching of the os module as it appears the "
+            "'readlink' function has been added."
+        )
+        return
+
+    module = sys.modules["os"]
+    module.readlink = os.path.realpath  # type: ignore
+
+
+def pypy_windows_set_console_cp_patch() -> None:
+    """
+    A patch function for PyPy on Windows that sets the console code page to
+    UTF-8 encodingto allow for proper handling of non-ASCII characters. This
+    function uses ctypes to call the Windows API functions SetConsoleCP and
+    SetConsoleOutputCP to set the code page.
+    """
+    from ctypes import windll  # type: ignore
+
+    code: int = windll.kernel32.GetConsoleOutputCP()
+    if code != 65001:
+        windll.kernel32.SetConsoleCP(65001)
+        windll.kernel32.SetConsoleOutputCP(65001)
+
+
 class Header(CIMultiDict):
     """
     Container used for both request and response headers. It is a subclass of
     `CIMultiDict
     <https://multidict.readthedocs.io/en/stable/multidict.html#cimultidictproxy>`_.
 
     It allows for multiple values for a single key in keeping with the HTTP
     spec. Also, all keys are *case in-sensitive*.
 
     Please checkout `the MultiDict documentation
     <https://multidict.readthedocs.io/en/stable/multidict.html#multidict>`_
     for more details about how to use the object. In general, it should work
     very similar to a regular dictionary.
-    """
+    """  # noqa: E501
 
     def __getattr__(self, key: str) -> str:
         if key.startswith("_"):
             return self.__getattribute__(key)
         key = key.rstrip("_").replace("_", "-")
         return ",".join(self.getall(key, default=[]))
 
@@ -108,14 +143,20 @@
 
     def stat_async(path) -> Awaitable[os.stat_result]:
         return trio.Path(path).stat()
 
     open_async = trio.open_file
     CancelledErrors = tuple([asyncio.CancelledError, trio.Cancelled])
 else:
+    if PYPY_IMPLEMENTATION:
+        pypy_os_module_patch()
+
+        if OS_IS_WINDOWS:
+            pypy_windows_set_console_cp_patch()
+
     from aiofiles import open as aio_open  # type: ignore
     from aiofiles.os import stat as stat_async  # type: ignore  # noqa: F401
 
     async def open_async(file, mode="r", **kwargs):
         return aio_open(file, mode, **kwargs)
 
     CancelledErrors = tuple([asyncio.CancelledError])
@@ -139,11 +180,7 @@
         if die:
             raise KeyboardInterrupt("Non-graceful Ctrl+C")
         die = True
 
     die = False
     signal.signal(signal.SIGINT, ctrlc_handler)
     app.add_task(stay_active)
-
-
-def is_atty() -> bool:
-    return bool(sys.stdout and sys.stdout.isatty())
```

### Comparing `sanic-23.3.0/sanic/config.py` & `sanic-23.6.0/sanic/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,42 +39,42 @@
     "ACCESS_LOG": False,
     "AUTO_EXTEND": True,
     "AUTO_RELOAD": False,
     "EVENT_AUTOREGISTER": False,
     "DEPRECATION_FILTER": "once",
     "FORWARDED_FOR_HEADER": "X-Forwarded-For",
     "FORWARDED_SECRET": None,
-    "GRACEFUL_SHUTDOWN_TIMEOUT": 15.0,  # 15 sec
+    "GRACEFUL_SHUTDOWN_TIMEOUT": 15.0,
     "INSPECTOR": False,
     "INSPECTOR_HOST": "localhost",
     "INSPECTOR_PORT": 6457,
     "INSPECTOR_TLS_KEY": _default,
     "INSPECTOR_TLS_CERT": _default,
     "INSPECTOR_API_KEY": "",
-    "KEEP_ALIVE_TIMEOUT": 5,  # 5 seconds
+    "KEEP_ALIVE_TIMEOUT": 120,
     "KEEP_ALIVE": True,
     "LOCAL_CERT_CREATOR": LocalCertCreator.AUTO,
     "LOCAL_TLS_KEY": _default,
     "LOCAL_TLS_CERT": _default,
     "LOCALHOST": "localhost",
     "MOTD": True,
     "MOTD_DISPLAY": {},
     "NOISY_EXCEPTIONS": False,
     "PROXIES_COUNT": None,
     "REAL_IP_HEADER": None,
-    "REQUEST_BUFFER_SIZE": 65536,  # 64 KiB
-    "REQUEST_MAX_HEADER_SIZE": 8192,  # 8 KiB, but cannot exceed 16384
+    "REQUEST_BUFFER_SIZE": 65536,
+    "REQUEST_MAX_HEADER_SIZE": 8192,  # Cannot exceed 16384
     "REQUEST_ID_HEADER": "X-Request-ID",
-    "REQUEST_MAX_SIZE": 100000000,  # 100 megabytes
-    "REQUEST_TIMEOUT": 60,  # 60 seconds
-    "RESPONSE_TIMEOUT": 60,  # 60 seconds
+    "REQUEST_MAX_SIZE": 100_000_000,
+    "REQUEST_TIMEOUT": 60,
+    "RESPONSE_TIMEOUT": 60,
     "TLS_CERT_PASSWORD": "",
     "TOUCHUP": _default,
     "USE_UVLOOP": _default,
-    "WEBSOCKET_MAX_SIZE": 2**20,  # 1 megabyte
+    "WEBSOCKET_MAX_SIZE": 2**20,  # 1 MiB
     "WEBSOCKET_PING_INTERVAL": 20,
     "WEBSOCKET_PING_TIMEOUT": 20,
 }
 
 
 class DescriptorMeta(ABCMeta):
     def __init__(cls, *_):
```

### Comparing `sanic-23.3.0/sanic/constants.py` & `sanic-23.6.0/sanic/constants.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/cookies/request.py` & `sanic-23.6.0/sanic/cookies/request.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/cookies/response.py` & `sanic-23.6.0/sanic/cookies/response.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/errorpages.py` & `sanic-23.6.0/sanic/errorpages.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,16 +88,18 @@
         :return: The formatted exception
         :rtype: str
         """
         output = (
             self.full
             if self.debug and not getattr(self.exception, "quiet", False)
             else self.minimal
-        )
-        return output()
+        )()
+        output.status = self.status
+        output.headers.update(self.headers)
+        return output
 
     def minimal(self) -> HTTPResponse:  # noqa
         """
         Provide a formatted message that is meant to not show any sensitive
         data or details.
         """
         raise NotImplementedError
@@ -121,15 +123,15 @@
         page = ErrorPage(
             debug=self.debug,
             title=super().title,
             text=super().text,
             request=self.request,
             exc=self.exception,
         )
-        return html(page.render(), status=self.status, headers=self.headers)
+        return html(page.render())
 
     def minimal(self) -> HTTPResponse:
         return self.full()
 
 
 class TextRenderer(BaseRenderer):
     """
@@ -142,28 +144,25 @@
     def full(self) -> HTTPResponse:
         return text(
             self.OUTPUT_TEXT.format(
                 title=self.title,
                 text=self.text,
                 bar=("=" * len(self.title)),
                 body=self._generate_body(full=True),
-            ),
-            status=self.status,
+            )
         )
 
     def minimal(self) -> HTTPResponse:
         return text(
             self.OUTPUT_TEXT.format(
                 title=self.title,
                 text=self.text,
                 bar=("=" * len(self.title)),
                 body=self._generate_body(full=False),
-            ),
-            status=self.status,
-            headers=self.headers,
+            )
         )
 
     @property
     def title(self):
         return f"⚠️ {super().title}"
 
     def _generate_body(self, *, full):
@@ -214,19 +213,19 @@
 class JSONRenderer(BaseRenderer):
     """
     Render an exception as JSON.
     """
 
     def full(self) -> HTTPResponse:
         output = self._generate_output(full=True)
-        return json(output, status=self.status, dumps=self.dumps)
+        return json(output, dumps=self.dumps)
 
     def minimal(self) -> HTTPResponse:
         output = self._generate_output(full=False)
-        return json(output, status=self.status, dumps=self.dumps)
+        return json(output, dumps=self.dumps)
 
     def _generate_output(self, *, full):
         output = {
             "description": self.title,
             "status": self.status,
             "message": self.text,
         }
@@ -309,15 +308,15 @@
 
 def exception_response(
     request: Request,
     exception: Exception,
     debug: bool,
     fallback: str,
     base: t.Type[BaseRenderer],
-    renderer: t.Type[t.Optional[BaseRenderer]] = None,
+    renderer: t.Optional[t.Type[BaseRenderer]] = None,
 ) -> HTTPResponse:
     """
     Render a response for the default FALLBACK exception handler.
     """
     if not renderer:
         mt = guess_mime(request, fallback)
         renderer = RENDERERS_BY_CONTENT_TYPE.get(mt, base)
```

### Comparing `sanic-23.3.0/sanic/exceptions.py` & `sanic-23.6.0/sanic/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 message = self.message
             elif status_code:
                 msg: bytes = STATUS_CODES.get(status_code, b"")
                 message = msg.decode("utf8")
 
         super().__init__(message)
 
-        self.status_code = status_code
+        self.status_code = status_code or self.status_code
         self.quiet = quiet
         self.headers = headers
 
 
 class HTTPException(SanicException):
     """
     A base class for other exceptions and should not be called directly.
```

### Comparing `sanic-23.3.0/sanic/handlers/content_range.py` & `sanic-23.6.0/sanic/handlers/content_range.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/handlers/directory.py` & `sanic-23.6.0/sanic/handlers/directory.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/handlers/error.py` & `sanic-23.6.0/sanic/handlers/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from typing import Dict, List, Optional, Tuple, Type
 
 from sanic.errorpages import BaseRenderer, TextRenderer, exception_response
 from sanic.exceptions import ServerError
 from sanic.log import error_logger
 from sanic.models.handler_types import RouteHandler
+from sanic.request.types import Request
 from sanic.response import text
+from sanic.response.types import HTTPResponse
 
 
 class ErrorHandler:
     """
     Provide :class:`sanic.app.Sanic` application with a mechanism to handle
     and process any and all uncaught exceptions in a way the application
     developer will set fit.
@@ -144,15 +146,15 @@
 
             if self.debug:
                 return text(response_message % (handler.__name__, url), 500)
             else:
                 return text("An error occurred while handling an error", 500)
         return response
 
-    def default(self, request, exception):
+    def default(self, request: Request, exception: Exception) -> HTTPResponse:
         """
         Provide a default behavior for the objects of :class:`ErrorHandler`.
         If a developer chooses to extent the :class:`ErrorHandler` they can
         provide a custom implementation for this method to behave in a way
         they see fit.
 
         :param request: Incoming request
```

### Comparing `sanic-23.3.0/sanic/headers.py` & `sanic-23.6.0/sanic/headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,15 @@
         ret += b"%b: %b\r\n" % h
     ret += b"\r\n"
     return ret
 
 
 def parse_credentials(
     header: Optional[str],
-    prefixes: Union[List, Tuple, Set] = None,
+    prefixes: Optional[Union[List, Tuple, Set]] = None,
 ) -> Tuple[Optional[str], Optional[str]]:
     """Parses any header with the aim to retrieve any credentials from it."""
     if not prefixes or not isinstance(prefixes, (list, tuple, set)):
         prefixes = ("Basic", "Bearer", "Token")
     if header is not None:
         for prefix in prefixes:
             if prefix in header:
```

### Comparing `sanic-23.3.0/sanic/helpers.py` & `sanic-23.6.0/sanic/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Defines basics of HTTP standard."""
 
+import sys
+
 from importlib import import_module
 from inspect import ismodule
 from typing import Dict
 
 
 STATUS_CODES: Dict[int, bytes] = {
     100: b"Continue",
@@ -153,14 +155,18 @@
     module = import_module(module, package=package)
     obj = getattr(module, klass)
     if ismodule(obj):
         return obj
     return obj()
 
 
+def is_atty() -> bool:
+    return bool(sys.stdout and sys.stdout.isatty())
+
+
 class Default:
     """
     It is used to replace `None` or `object()` as a sentinel
     that represents a default value. Sometimes we want to set
     a value to `None` so we cannot use `None` to represent the
     default value, and `object()` is hard to be typed.
     """
```

### Comparing `sanic-23.3.0/sanic/http/constants.py` & `sanic-23.6.0/sanic/http/constants.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/http/http1.py` & `sanic-23.6.0/sanic/http/http1.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/http/http3.py` & `sanic-23.6.0/sanic/http/http3.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/http/stream.py` & `sanic-23.6.0/sanic/http/stream.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/http/tls/context.py` & `sanic-23.6.0/sanic/http/tls/context.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/http/tls/creators.py` & `sanic-23.6.0/sanic/http/tls/creators.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/log.py` & `sanic-23.6.0/sanic/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import sys
 
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Dict
 from warnings import warn
 
-from sanic.compat import is_atty
+from sanic.helpers import is_atty
 
 
 # Python 3.11 changed the way Enum formatting works for mixed-in types.
 if sys.version_info < (3, 11, 0):
 
     class StrEnum(str, Enum):
         pass
```

### Comparing `sanic-23.3.0/sanic/middleware.py` & `sanic-23.6.0/sanic/middleware.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/mixins/base.py` & `sanic-23.6.0/sanic/mixins/base.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/mixins/exceptions.py` & `sanic-23.6.0/sanic/mixins/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,7 +34,19 @@
             future_exception = FutureException(handler, exceptions)
             self._future_exceptions.add(future_exception)
             if apply:
                 self._apply_exception_handler(future_exception)
             return handler
 
         return decorator
+
+    def all_exceptions(self, handler):
+        """
+        This method enables the process of creating a global exception
+        handler for the current blueprint under question.
+
+        :param handler: A coroutine function to handle exceptions
+
+        :return a decorated method to handle global exceptions for any
+            route registered under this blueprint.
+        """
+        return self.exception(Exception)(handler)
```

### Comparing `sanic-23.3.0/sanic/mixins/listeners.py` & `sanic-23.6.0/sanic/mixins/listeners.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/mixins/middleware.py` & `sanic-23.6.0/sanic/mixins/middleware.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/mixins/routes.py` & `sanic-23.6.0/sanic/mixins/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,19 @@
                 subprotocols,
                 unquote,
                 static,
                 version_prefix,
                 error_format,
                 route_context,
             )
-
+            overwrite = getattr(self, "_allow_route_overwrite", False)
+            if overwrite:
+                self._future_routes = set(
+                    filter(lambda x: x.uri != uri, self._future_routes)
+                )
             self._future_routes.add(route)
 
             args = list(signature(handler).parameters.keys())
             if websocket and len(args) < 2:
                 handler_name = handler.__name__
 
                 raise ValueError(
@@ -178,15 +182,15 @@
                     f"in the {handler_name}() route?"
                 )
 
             if not websocket and stream:
                 handler.is_stream = stream
 
             if apply:
-                self._apply_route(route)
+                self._apply_route(route, overwrite=overwrite)
 
             if static:
                 return route, handler
             return handler
 
         return decorator
```

### Comparing `sanic-23.3.0/sanic/mixins/signals.py` & `sanic-23.6.0/sanic/mixins/signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 from typing import Any, Callable, Dict, Optional, Set, Union
 
 from sanic.base.meta import SanicMeta
 from sanic.models.futures import FutureSignal
 from sanic.models.handler_types import SignalHandler
-from sanic.signals import Signal
+from sanic.signals import Event, Signal
 from sanic.types import HashableDict
 
 
 class SignalMixin(metaclass=SanicMeta):
     def __init__(self, *args, **kwargs) -> None:
         self._future_signals: Set[FutureSignal] = set()
 
@@ -76,7 +76,13 @@
         self.signal(event=event, condition=condition, exclusive=exclusive)(
             handler
         )
         return handler
 
     def event(self, event: str):
         raise NotImplementedError
+
+    def catch_exception(self, handler):
+        async def signal_handler(exception: Exception):
+            await handler(self, exception)
+
+        self.signal(Event.SERVER_LIFECYCLE_EXCEPTION)(signal_handler)
```

### Comparing `sanic-23.3.0/sanic/mixins/startup.py` & `sanic-23.6.0/sanic/mixins/startup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,30 @@
     get_event_loop,
     get_running_loop,
     new_event_loop,
 )
 from contextlib import suppress
 from functools import partial
 from importlib import import_module
-from multiprocessing import Manager, Pipe, get_context
+from multiprocessing import (
+    Manager,
+    Pipe,
+    get_context,
+    get_start_method,
+    set_start_method,
+)
 from multiprocessing.context import BaseContext
 from pathlib import Path
 from socket import SHUT_RDWR, socket
 from ssl import SSLContext
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    ClassVar,
     Dict,
     List,
     Mapping,
     Optional,
     Set,
     Tuple,
     Type,
@@ -37,17 +44,17 @@
 )
 
 from sanic.application.ext import setup_ext
 from sanic.application.logo import get_logo
 from sanic.application.motd import MOTD
 from sanic.application.state import ApplicationServerInfo, Mode, ServerStage
 from sanic.base.meta import SanicMeta
-from sanic.compat import OS_IS_WINDOWS, StartMethod, is_atty
+from sanic.compat import OS_IS_WINDOWS, StartMethod
 from sanic.exceptions import ServerKilled
-from sanic.helpers import Default, _default
+from sanic.helpers import Default, _default, is_atty
 from sanic.http.constants import HTTP
 from sanic.http.tls import get_ssl_context, process_to_context
 from sanic.http.tls.context import SanicSSLContext
 from sanic.log import Colors, error_logger, logger
 from sanic.models.handler_types import ListenerType
 from sanic.server import Signal as ServerSignal
 from sanic.server import try_use_uvloop
@@ -77,21 +84,25 @@
 else:  # no cov
     from typing import Literal
 
     HTTPVersion = Union[HTTP, Literal[1], Literal[3]]
 
 
 class StartupMixin(metaclass=SanicMeta):
-    _app_registry: Dict[str, Sanic]
+    _app_registry: ClassVar[Dict[str, Sanic]]
+
     config: Config
     listeners: Dict[str, List[ListenerType[Any]]]
     state: ApplicationState
     websocket_enabled: bool
     multiplexer: WorkerMultiplexer
-    start_method: StartMethod = _default
+
+    test_mode: ClassVar[bool]
+    start_method: ClassVar[StartMethod] = _default
+    START_METHOD_SET: ClassVar[bool] = False
 
     def setup_loop(self):
         if not self.asgi:
             if self.config.USE_UVLOOP is True or (
                 isinstance(self.config.USE_UVLOOP, Default)
                 and not OS_IS_WINDOWS
             ):
@@ -688,27 +699,43 @@
         return (
             cls.start_method
             if not isinstance(cls.start_method, Default)
             else "spawn"
         )
 
     @classmethod
+    def _set_startup_method(cls) -> None:
+        if cls.START_METHOD_SET and not cls.test_mode:
+            return
+
+        method = cls._get_startup_method()
+        set_start_method(method, force=cls.test_mode)
+        cls.START_METHOD_SET = True
+
+    @classmethod
     def _get_context(cls) -> BaseContext:
         method = cls._get_startup_method()
         logger.debug("Creating multiprocessing context using '%s'", method)
-        return get_context(method)
+        actual = get_start_method()
+        if method != actual:
+            raise RuntimeError(
+                f"Start method '{method}' was requested, but '{actual}' "
+                "was actually set."
+            )
+        return get_context()
 
     @classmethod
     def serve(
         cls,
         primary: Optional[Sanic] = None,
         *,
         app_loader: Optional[AppLoader] = None,
         factory: Optional[Callable[[], Sanic]] = None,
     ) -> None:
+        cls._set_startup_method()
         os.environ["SANIC_MOTD_OUTPUT"] = "true"
         apps = list(cls._app_registry.values())
         if factory:
             primary = factory()
         else:
             if not primary:
                 if app_loader:
```

### Comparing `sanic-23.3.0/sanic/mixins/static.py` & `sanic-23.6.0/sanic/mixins/static.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
         if not isinstance(file_or_directory, (str, bytes, PurePath)):
             raise ValueError(
                 f"Static route must be a valid path, not {file_or_directory}"
             )
 
         try:
-            file_or_directory = Path(file_or_directory)
+            file_or_directory = Path(file_or_directory).resolve()
         except TypeError:
             raise TypeError(
                 "Static file or directory must be a path-like object or string"
             )
 
         if directory_handler and (directory_view or index):
             raise ValueError(
```

### Comparing `sanic-23.3.0/sanic/models/asgi.py` & `sanic-23.6.0/sanic/models/asgi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import asyncio
-import sys
 
 from typing import Any, Awaitable, Callable, MutableMapping, Optional, Union
 
 from sanic.exceptions import BadRequest
 from sanic.models.protocol_types import TransportProtocol
 from sanic.server.websockets.connection import WebSocketConnection
 
@@ -12,28 +11,18 @@
 ASGIMessage = MutableMapping[str, Any]
 ASGISend = Callable[[ASGIMessage], Awaitable[None]]
 ASGIReceive = Callable[[], Awaitable[ASGIMessage]]
 
 
 class MockProtocol:  # no cov
     def __init__(self, transport: "MockTransport", loop):
-        # This should be refactored when < 3.8 support is dropped
         self.transport = transport
-        # Fixup for 3.8+; Sanic still supports 3.7 where loop is required
-        loop = loop if sys.version_info[:2] < (3, 8) else None
-        # Optional in 3.9, necessary in 3.10 because the parameter "loop"
-        # was completely removed
-        if not loop:
-            self._not_paused = asyncio.Event()
-            self._not_paused.set()
-            self._complete = asyncio.Event()
-        else:
-            self._not_paused = asyncio.Event(loop=loop)
-            self._not_paused.set()
-            self._complete = asyncio.Event(loop=loop)
+        self._not_paused = asyncio.Event()
+        self._not_paused.set()
+        self._complete = asyncio.Event()
 
     def pause_writing(self) -> None:
         self._not_paused.clear()
 
     def resume_writing(self) -> None:
         self._not_paused.set()
```

### Comparing `sanic-23.3.0/sanic/models/futures.py` & `sanic-23.6.0/sanic/models/futures.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/models/handler_types.py` & `sanic-23.6.0/sanic/models/handler_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from asyncio.events import AbstractEventLoop
 from typing import Any, Callable, Coroutine, Optional, TypeVar, Union
 
 import sanic
 
-from sanic.request import Request
+from sanic import request
 from sanic.response import BaseHTTPResponse, HTTPResponse
 
 
 Sanic = TypeVar("Sanic", bound="sanic.Sanic")
+Request = TypeVar("Request", bound="request.Request")
 
 MiddlewareResponse = Union[
     Optional[HTTPResponse], Coroutine[Any, Any, Optional[HTTPResponse]]
 ]
 RequestMiddlewareType = Callable[[Request], MiddlewareResponse]
 ResponseMiddlewareType = Callable[
     [Request, BaseHTTPResponse], MiddlewareResponse
```

### Comparing `sanic-23.3.0/sanic/models/http_types.py` & `sanic-23.6.0/sanic/models/http_types.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/models/protocol_types.py` & `sanic-23.6.0/sanic/models/protocol_types.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/models/server_types.py` & `sanic-23.6.0/sanic/models/server_types.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/pages/base.py` & `sanic-23.6.0/sanic/pages/base.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/pages/css.py` & `sanic-23.6.0/sanic/pages/css.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/pages/directory_page.py` & `sanic-23.6.0/sanic/pages/directory_page.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/pages/error.py` & `sanic-23.6.0/sanic/pages/error.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/pages/styles/BasePage.css` & `sanic-23.6.0/sanic/pages/styles/BasePage.css`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/pages/styles/DirectoryPage.css` & `sanic-23.6.0/sanic/pages/styles/DirectoryPage.css`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/pages/styles/ErrorPage.css` & `sanic-23.6.0/sanic/pages/styles/ErrorPage.css`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/request/form.py` & `sanic-23.6.0/sanic/request/form.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/request/parameters.py` & `sanic-23.6.0/sanic/request/parameters.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/request/types.py` & `sanic-23.6.0/sanic/request/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from __future__ import annotations
 
 from contextvars import ContextVar
 from inspect import isawaitable
+from types import SimpleNamespace
 from typing import (
     TYPE_CHECKING,
     Any,
     DefaultDict,
     Dict,
+    Generic,
     List,
     Optional,
     Tuple,
     Union,
     cast,
 )
 
 from sanic_routing.route import Route
+from typing_extensions import TypeVar
 
 from sanic.http.constants import HTTP  # type: ignore
 from sanic.http.stream import Stream
 from sanic.models.asgi import ASGIScope
 from sanic.models.http_types import Credentials
 
 
 if TYPE_CHECKING:
-    from sanic.server import ConnInfo
     from sanic.app import Sanic
+    from sanic.config import Config
+    from sanic.server import ConnInfo
 
 import uuid
 
 from collections import defaultdict
-from types import SimpleNamespace
 from urllib.parse import parse_qs, parse_qsl, urlunparse
 
 from httptools import parse_url
 from httptools.parser.errors import HttpParserInvalidURLError
 
 from sanic.compat import CancelledErrors, Header
 from sanic.constants import (
@@ -64,26 +67,40 @@
 
 
 try:
     from ujson import loads as json_loads  # type: ignore
 except ImportError:
     from json import loads as json_loads  # type: ignore
 
+if TYPE_CHECKING:
+    # The default argument of TypeVar is proposed to be added in Python 3.13
+    # by PEP 696 (https://www.python.org/dev/peps/pep-0696/).
+    # Therefore, we use typing_extensions.TypeVar for compatibility.
+    # For more information, see:
+    # https://discuss.python.org/t/pep-696-type-defaults-for-typevarlikes
+    sanic_type = TypeVar(
+        "sanic_type", bound=Sanic, default=Sanic[Config, SimpleNamespace]
+    )
+else:
+    sanic_type = TypeVar("sanic_type")
+ctx_type = TypeVar("ctx_type")
 
-class Request:
+
+class Request(Generic[sanic_type, ctx_type]):
     """
     Properties of an HTTP request such as URL, headers, etc.
     """
 
     _current: ContextVar[Request] = ContextVar("request")
     _loads = json_loads
 
     __slots__ = (
         "__weakref__",
         "_cookies",
+        "_ctx",
         "_id",
         "_ip",
         "_parsed_url",
         "_port",
         "_protocol",
         "_remote_addr",
         "_request_middleware_started",
@@ -92,15 +109,14 @@
         "_socket",
         "_stream_id",
         "_match_info",
         "_name",
         "app",
         "body",
         "conn_info",
-        "ctx",
         "head",
         "headers",
         "method",
         "parsed_accept",
         "parsed_args",
         "parsed_cookies",
         "parsed_credentials",
@@ -121,15 +137,15 @@
     def __init__(
         self,
         url_bytes: bytes,
         headers: Header,
         version: str,
         method: str,
         transport: TransportProtocol,
-        app: Sanic,
+        app: sanic_type,
         head: bytes = b"",
         stream_id: int = 0,
     ):
         self.raw_url = url_bytes
         try:
             self._parsed_url = parse_url(url_bytes)
         except HttpParserInvalidURLError:
@@ -145,15 +161,15 @@
         self.method = method
         self.transport = transport
         self.head = head
 
         # Init but do not inhale
         self.body = b""
         self.conn_info: Optional[ConnInfo] = None
-        self.ctx = SimpleNamespace()
+        self._ctx: Optional[ctx_type] = None
         self.parsed_accept: Optional[AcceptList] = None
         self.parsed_args: DefaultDict[
             Tuple[bool, bool, str, str], RequestParameters
         ] = defaultdict(RequestParameters)
         self.parsed_cookies: Optional[RequestParameters] = None
         self.parsed_credentials: Optional[Credentials] = None
         self.parsed_files: Optional[RequestParameters] = None
@@ -172,14 +188,18 @@
         self._match_info: Dict[str, Any] = {}
         self._protocol = None
 
     def __repr__(self):
         class_name = self.__class__.__name__
         return f"<{class_name}: {self.method} {self.path}>"
 
+    @staticmethod
+    def make_context() -> ctx_type:
+        return cast(ctx_type, SimpleNamespace())
+
     @classmethod
     def get_current(cls) -> Request:
         """
         Retrieve the current request object
 
         This implements `Context Variables
         <https://docs.python.org/3/library/contextvars.html>`_
@@ -202,14 +222,23 @@
         return request
 
     @classmethod
     def generate_id(*_):
         return uuid.uuid4()
 
     @property
+    def ctx(self) -> ctx_type:
+        """
+        :return: The current request context
+        """
+        if not self._ctx:
+            self._ctx = self.make_context()
+        return self._ctx
+
+    @property
     def stream_id(self):
         """
         Access the HTTP/3 stream ID.
 
         Raises :exc:`sanic.exceptions.ServerError` if it is not an
         HTTP/3 request.
         """
@@ -805,28 +834,40 @@
                 or {}
             )
         return self.parsed_forwarded
 
     @property
     def remote_addr(self) -> str:
         """
-        Client IP address, if available.
-        1. proxied remote address `self.forwarded['for']`
-        2. local remote address `self.ip`
+        Client IP address, if available from proxy.
 
         :return: IPv4, bracketed IPv6, UNIX socket name or arbitrary string
         :rtype: str
         """
         if not hasattr(self, "_remote_addr"):
-            self._remote_addr = str(
-                self.forwarded.get("for", "")
-            )  # or self.ip
+            self._remote_addr = str(self.forwarded.get("for", ""))
         return self._remote_addr
 
     @property
+    def client_ip(self) -> str:
+        """
+        Client IP address.
+        1. proxied remote address `self.forwarded['for']`
+        2. local peer address `self.ip`
+
+        New in Sanic 23.6. Prefer this over `remote_addr` for determining the
+        client address regardless of whether the service runs behind a proxy
+        or not (proxy deployment needs separate configuration).
+
+        :return: IPv4, bracketed IPv6, UNIX socket name or arbitrary string
+        :rtype: str
+        """
+        return self.remote_addr or self.ip
+
+    @property
     def scheme(self) -> str:
         """
         Determine request scheme.
         1. `config.SERVER_NAME` if in full URL format
         2. proxied proto/scheme
         3. local connection protocol
```

### Comparing `sanic-23.3.0/sanic/response/convenience.py` & `sanic-23.6.0/sanic/response/convenience.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/response/types.py` & `sanic-23.6.0/sanic/response/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,17 @@
     from sanic.http.http3 import HTTPReceiver
     from sanic.request import Request
 else:
     Request = TypeVar("Request")
 
 
 try:
-    from ujson import dumps as json_dumps
+    from ujson import dumps as ujson_dumps
+
+    json_dumps = partial(ujson_dumps, escape_forward_slashes=False)
 except ImportError:
     # This is done in order to ensure that the JSON response is
     # kept consistent across both ujson and inbuilt json usage.
     from json import dumps
 
     json_dumps = partial(dumps, separators=(",", ":"))
 
@@ -341,15 +343,15 @@
     )
 
     def __init__(
         self,
         body: Optional[Any] = None,
         status: int = 200,
         headers: Optional[Union[Header, Dict[str, str]]] = None,
-        content_type: Optional[str] = None,
+        content_type: str = "application/json",
         dumps: Optional[Callable[..., str]] = None,
         **kwargs: Any,
     ):
         self._initialized = False
         self._body_manually_set = False
 
         self._use_dumps = dumps or BaseHTTPResponse._dumps
@@ -516,15 +518,17 @@
             [Union[BaseHTTPResponse, ResponseStream]],
             Coroutine[Any, Any, None],
         ],
         status: int = 200,
         headers: Optional[Union[Header, Dict[str, str]]] = None,
         content_type: Optional[str] = None,
     ):
-        if not isinstance(headers, Header):
+        if headers is None:
+            headers = Header()
+        elif not isinstance(headers, Header):
             headers = Header(headers)
         self.streaming_fn = streaming_fn
         self.status = status
         self.headers = headers or Header()
         self.content_type = content_type
         self.request: Optional[Request] = None
         self._cookies: Optional[CookieJar] = None
```

### Comparing `sanic-23.3.0/sanic/router.py` & `sanic-23.6.0/sanic/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,19 +71,20 @@
         uri: str,
         methods: Iterable[str],
         handler: RouteHandler,
         host: Optional[Union[str, Iterable[str]]] = None,
         strict_slashes: bool = False,
         stream: bool = False,
         ignore_body: bool = False,
-        version: Union[str, float, int] = None,
+        version: Optional[Union[str, float, int]] = None,
         name: Optional[str] = None,
         unquote: bool = False,
         static: bool = False,
         version_prefix: str = "/v",
+        overwrite: bool = False,
         error_format: Optional[str] = None,
     ) -> Union[Route, List[Route]]:
         """
         Add a handler to the router
 
         :param uri: the path of the route
         :type uri: str
@@ -118,14 +119,15 @@
         params = dict(
             path=uri,
             handler=handler,
             methods=frozenset(map(str, methods)) if methods else None,
             name=name,
             strict=strict_slashes,
             unquote=unquote,
+            overwrite=overwrite,
         )
 
         if isinstance(host, str):
             hosts = [host]
         else:
             hosts = host or [None]  # type: ignore
```

### Comparing `sanic-23.3.0/sanic/server/async_server.py` & `sanic-23.6.0/sanic/server/async_server.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/server/events.py` & `sanic-23.6.0/sanic/server/events.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/server/loop.py` & `sanic-23.6.0/sanic/server/loop.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/server/protocols/base_protocol.py` & `sanic-23.6.0/sanic/server/protocols/base_protocol.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/server/protocols/http_protocol.py` & `sanic-23.6.0/sanic/server/protocols/http_protocol.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/server/protocols/websocket_protocol.py` & `sanic-23.6.0/sanic/server/protocols/websocket_protocol.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/server/runners.py` & `sanic-23.6.0/sanic/server/runners.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 
-import sys
-
 from ssl import SSLContext
 from typing import TYPE_CHECKING, Dict, Optional, Type, Union
 
 from sanic.config import Config
 from sanic.exceptions import ServerError
 from sanic.http.constants import HTTP
 from sanic.http.tls import get_ssl_context
@@ -247,16 +245,15 @@
         # Let's roughly calcucate time.
         graceful = app.config.GRACEFUL_SHUTDOWN_TIMEOUT
         start_shutdown: float = 0
         while connections and (start_shutdown < graceful):
             loop.run_until_complete(asyncio.sleep(0.1))
             start_shutdown = start_shutdown + 0.1
 
-        if sys.version_info > (3, 7):
-            app.shutdown_tasks(graceful - start_shutdown)
+        app.shutdown_tasks(graceful - start_shutdown)
 
         # Force close non-idle connection after waiting for
         # graceful_shutdown_timeout
         for conn in connections:
             if hasattr(conn, "websocket") and conn.websocket:
                 conn.websocket.fail_connection(code=1001)
             else:
```

### Comparing `sanic-23.3.0/sanic/server/socket.py` & `sanic-23.6.0/sanic/server/socket.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/server/websockets/connection.py` & `sanic-23.6.0/sanic/server/websockets/connection.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/server/websockets/frame.py` & `sanic-23.6.0/sanic/server/websockets/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
         Read the next message.
         :meth:`get` returns a single :class:`str` or :class:`bytes`.
         If the :message was fragmented, :meth:`get` waits until the last frame
         is received, then it reassembles the message.
         If ``timeout`` is set and elapses before a complete message is
         received, :meth:`get` returns ``None``.
         """
+        completed: bool
         async with self.read_mutex:
             if timeout is not None and timeout <= 0:
                 if not self.message_complete.is_set():
                     return None
             if self.get_in_progress:
                 # This should be guarded against with the read_mutex,
                 # exception is only here as a failsafe
```

### Comparing `sanic-23.3.0/sanic/server/websockets/impl.py` & `sanic-23.6.0/sanic/server/websockets/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ConnectionClosedError,
     ConnectionClosedOK,
 )
 from websockets.frames import Frame, Opcode
 
 
 try:  # websockets < 11.0
-    from websockets.connection import Event, State
+    from websockets.connection import Event, State  # type: ignore
     from websockets.server import ServerConnection as ServerProtocol
 except ImportError:  # websockets >= 11.0
     from websockets.protocol import Event, State  # type: ignore
     from websockets.server import ServerProtocol  # type: ignore
 
 from websockets.typing import Data
```

### Comparing `sanic-23.3.0/sanic/signals.py` & `sanic-23.6.0/sanic/signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from sanic.exceptions import InvalidSignal
 from sanic.log import error_logger, logger
 from sanic.models.handler_types import SignalHandler
 
 
 class Event(Enum):
+    SERVER_EXCEPTION_REPORT = "server.exception.report"
     SERVER_INIT_AFTER = "server.init.after"
     SERVER_INIT_BEFORE = "server.init.before"
     SERVER_SHUTDOWN_AFTER = "server.shutdown.after"
     SERVER_SHUTDOWN_BEFORE = "server.shutdown.before"
     HTTP_LIFECYCLE_BEGIN = "http.lifecycle.begin"
     HTTP_LIFECYCLE_COMPLETE = "http.lifecycle.complete"
     HTTP_LIFECYCLE_EXCEPTION = "http.lifecycle.exception"
@@ -35,14 +36,15 @@
     HTTP_LIFECYCLE_SEND = "http.lifecycle.send"
     HTTP_MIDDLEWARE_AFTER = "http.middleware.after"
     HTTP_MIDDLEWARE_BEFORE = "http.middleware.before"
 
 
 RESERVED_NAMESPACES = {
     "server": (
+        Event.SERVER_EXCEPTION_REPORT.value,
         Event.SERVER_INIT_AFTER.value,
         Event.SERVER_INIT_BEFORE.value,
         Event.SERVER_SHUTDOWN_AFTER.value,
         Event.SERVER_SHUTDOWN_BEFORE.value,
     ),
     "http": (
         Event.HTTP_LIFECYCLE_BEGIN.value,
@@ -164,14 +166,25 @@
                     if isawaitable(maybe_coroutine):
                         retval = await maybe_coroutine
                         if retval:
                             return retval
                     elif maybe_coroutine:
                         return maybe_coroutine
             return None
+        except Exception as e:
+            if self.ctx.app.debug and self.ctx.app.state.verbosity >= 1:
+                error_logger.exception(e)
+
+            if event != Event.SERVER_EXCEPTION_REPORT.value:
+                await self.dispatch(
+                    Event.SERVER_EXCEPTION_REPORT.value,
+                    context={"exception": e},
+                )
+                setattr(e, "__dispatched__", True)
+            raise e
         finally:
             for signal_event in events:
                 signal_event.clear()
 
     async def dispatch(
         self,
         event: str,
@@ -213,22 +226,14 @@
         else:
             name = event
             trigger = ""
 
         if not trigger:
             event = ".".join([*parts[:2], "<__trigger__>"])
 
-        try:
-            # Attaching __requirements__ and __trigger__ to the handler
-            # is deprecated and will be removed in v23.6.
-            handler.__requirements__ = condition  # type: ignore
-            handler.__trigger__ = trigger  # type: ignore
-        except AttributeError:
-            pass
-
         signal = super().add(
             event,
             handler,
             name=name,
             append=True,
         )  # type: ignore
```

### Comparing `sanic-23.3.0/sanic/touchup/meta.py` & `sanic-23.6.0/sanic/touchup/meta.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/touchup/schemes/altsvc.py` & `sanic-23.6.0/sanic/touchup/schemes/altsvc.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/touchup/schemes/base.py` & `sanic-23.6.0/sanic/touchup/schemes/base.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/touchup/schemes/ode.py` & `sanic-23.6.0/sanic/touchup/schemes/ode.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/touchup/service.py` & `sanic-23.6.0/sanic/touchup/service.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/types/shared_ctx.py` & `sanic-23.6.0/sanic/types/shared_ctx.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/utils.py` & `sanic-23.6.0/sanic/utils.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/views.py` & `sanic-23.6.0/sanic/views.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/worker/inspector.py` & `sanic-23.6.0/sanic/worker/inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,18 +79,15 @@
         return await self._respond(request, output)
 
     async def _info(self, request: Request):
         return await self._respond(request, self._state_to_json())
 
     async def _respond(self, request: Request, output: Any):
         name = request.match_info.get("action", "info")
-        return json(
-            {"meta": {"action": name}, "result": output},
-            escape_forward_slashes=False,
-        )
+        return json({"meta": {"action": name}, "result": output})
 
     def _state_to_json(self) -> Dict[str, Any]:
         output = {"info": self.app_info}
         output["workers"] = self._make_safe(dict(self.worker_state))
         return output
 
     @staticmethod
```

### Comparing `sanic-23.3.0/sanic/worker/loader.py` & `sanic-23.6.0/sanic/worker/loader.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/worker/manager.py` & `sanic-23.6.0/sanic/worker/manager.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/worker/multiplexer.py` & `sanic-23.6.0/sanic/worker/multiplexer.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/worker/process.py` & `sanic-23.6.0/sanic/worker/process.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/worker/reloader.py` & `sanic-23.6.0/sanic/worker/reloader.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/worker/serve.py` & `sanic-23.6.0/sanic/worker/serve.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic/worker/state.py` & `sanic-23.6.0/sanic/worker/state.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/sanic.egg-info/PKG-INFO` & `sanic-23.6.0/sanic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: sanic
-Version: 23.3.0
+Version: 23.6.0
 Summary: A web server and web framework that's written to go fast. Build fast. Run fast.
 Home-page: http://github.com/sanic-org/sanic/
 Author: Sanic Community
 Author-email: admhpkns@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: all
 Provides-Extra: ext
 Provides-Extra: http3
 License-File: LICENSE
@@ -190,9 +189,7 @@
 
 We are always happy to have new contributions. We have `marked issues good for anyone looking to get started <https://github.com/sanic-org/sanic/issues?q=is%3Aopen+is%3Aissue+label%3Abeginner>`_, and welcome `questions on the forums <https://community.sanicframework.org/>`_. Please take a look at our `Contribution guidelines <https://github.com/sanic-org/sanic/blob/master/CONTRIBUTING.rst>`_.
 
 .. |Linode| image:: https://www.linode.com/wp-content/uploads/2021/01/Linode-Logo-Black.svg
     :alt: Linode
     :target: https://www.linode.com
     :width: 200px
-
-
```

### Comparing `sanic-23.3.0/sanic.egg-info/SOURCES.txt` & `sanic-23.6.0/sanic.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -242,14 +242,22 @@
 tests/static/python.png
 tests/static/test.file
 tests/static/test.html
 tests/static/bp/decode me.txt
 tests/static/bp/python.png
 tests/static/bp/test.file
 tests/static/nested/dir/foo.txt
+tests/typing/test_typing.py
+tests/typing/samples/app_custom_config.py
+tests/typing/samples/app_custom_ctx.py
+tests/typing/samples/app_default.py
+tests/typing/samples/app_fully_custom.py
+tests/typing/samples/request_custom_ctx.py
+tests/typing/samples/request_custom_sanic.py
+tests/typing/samples/request_fully_custom.py
 tests/worker/test_inspector.py
 tests/worker/test_loader.py
 tests/worker/test_manager.py
 tests/worker/test_multiplexer.py
 tests/worker/test_reloader.py
 tests/worker/test_runner.py
 tests/worker/test_shared_ctx.py
```

### Comparing `sanic-23.3.0/sanic.egg-info/requires.txt` & `sanic-23.6.0/sanic.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-sanic-routing>=22.8.0
+sanic-routing>=23.6.0
 httptools>=0.0.10
 aiofiles>=0.6.0
 websockets>=10.0
 multidict<7.0,>=5.0
 html5tagger>=1.2.1
 tracerite>=1.0.0
+typing-extensions>=4.4.0
 
 [:sys_platform != "win32" and implementation_name == "cpython"]
 uvloop>=0.15.0
 ujson>=1.35
 
 [all]
-black
+docutils
+enum-tools[sphinx]
+bandit
+pytest==7.1.*
+pygments
+tox
+coverage
 cryptography
+m2r2
+pytest-benchmark
 flake8
 chardet==3.*
-uvicorn<0.15.0
-beautifulsoup4
-bandit
-m2r2
-pytest-sanic
-pytest==7.1.*
-sphinx_rtd_theme>=0.4.3
 mistune<2.0.0
-pygments
-sanic-testing>=23.3.0
-enum-tools[sphinx]
+pytest-sanic
 isort>=5.0.0
-sphinx>=2.1.2
-pytest-benchmark
-mypy<0.910,>=0.901
-coverage
-tox
+black
 towncrier
+uvicorn<0.15.0
 slotscheck<1,>=0.8.0
-docutils
+sanic-testing>=23.6.0
+sphinx>=2.1.2
+beautifulsoup4
+sphinx_rtd_theme>=0.4.3
+mypy
 
 [all:sys_platform != "win32" and implementation_name == "cpython"]
 types-ujson
 
 [dev]
-sanic-testing>=23.3.0
+sanic-testing>=23.6.0
 pytest==7.1.*
 coverage
 beautifulsoup4
 pytest-sanic
 pytest-benchmark
 chardet==3.*
 flake8
 black
 isort>=5.0.0
 bandit
-mypy<0.910,>=0.901
+mypy
 docutils
 pygments
 uvicorn<0.15.0
 slotscheck<1,>=0.8.0
 cryptography
 tox
 towncrier
@@ -75,26 +76,26 @@
 [ext]
 sanic-ext
 
 [http3]
 aioquic
 
 [test]
-sanic-testing>=23.3.0
+sanic-testing>=23.6.0
 pytest==7.1.*
 coverage
 beautifulsoup4
 pytest-sanic
 pytest-benchmark
 chardet==3.*
 flake8
 black
 isort>=5.0.0
 bandit
-mypy<0.910,>=0.901
+mypy
 docutils
 pygments
 uvicorn<0.15.0
 slotscheck<1,>=0.8.0
 
 [test:sys_platform != "win32" and implementation_name == "cpython"]
 types-ujson
```

### Comparing `sanic-23.3.0/setup.py` & `sanic-23.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,20 +79,19 @@
         "A web server and web framework that's written to go fast. "
         "Build fast. Run fast."
     ),
     "long_description": long_description,
     "packages": find_packages(exclude=("tests", "tests.*")),
     "package_data": {"sanic": ["py.typed", "pages/styles/*"]},
     "platforms": "any",
-    "python_requires": ">=3.7",
+    "python_requires": ">=3.8",
     "classifiers": [
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     "entry_points": {"console_scripts": ["sanic = sanic.__main__:main"]},
 }
@@ -100,38 +99,39 @@
 env_dependency = (
     '; sys_platform != "win32" ' 'and implementation_name == "cpython"'
 )
 ujson = "ujson>=1.35" + env_dependency
 uvloop = "uvloop>=0.15.0" + env_dependency
 types_ujson = "types-ujson" + env_dependency
 requirements = [
-    "sanic-routing>=22.8.0",
+    "sanic-routing>=23.6.0",
     "httptools>=0.0.10",
     uvloop,
     ujson,
     "aiofiles>=0.6.0",
     "websockets>=10.0",
     "multidict>=5.0,<7.0",
     "html5tagger>=1.2.1",
     "tracerite>=1.0.0",
+    "typing-extensions>=4.4.0",
 ]
 
 tests_require = [
-    "sanic-testing>=23.3.0",
+    "sanic-testing>=23.6.0",
     "pytest==7.1.*",
     "coverage",
     "beautifulsoup4",
     "pytest-sanic",
     "pytest-benchmark",
     "chardet==3.*",
     "flake8",
     "black",
     "isort>=5.0.0",
     "bandit",
-    "mypy>=0.901,<0.910",
+    "mypy",
     "docutils",
     "pygments",
     "uvicorn<0.15.0",
     "slotscheck>=0.8.0,<1",
     types_ujson,
 ]
```

### Comparing `sanic-23.3.0/tests/asyncmock.py` & `sanic-23.6.0/tests/asyncmock.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/benchmark/test_route_resolution_benchmark.py` & `sanic-23.6.0/tests/benchmark/test_route_resolution_benchmark.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/certs/createcerts.py` & `sanic-23.6.0/tests/certs/createcerts.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/certs/localhost/fullchain.pem` & `sanic-23.6.0/tests/certs/localhost/fullchain.pem`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/certs/password/fullchain.pem` & `sanic-23.6.0/tests/certs/password/fullchain.pem`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/certs/password/privkey.pem` & `sanic-23.6.0/tests/certs/password/privkey.pem`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/certs/sanic.example/fullchain.pem` & `sanic-23.6.0/tests/certs/sanic.example/fullchain.pem`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/certs/sanic.example/privkey.pem` & `sanic-23.6.0/tests/certs/sanic.example/privkey.pem`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/client.py` & `sanic-23.6.0/tests/client.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/conftest.py` & `sanic-23.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/fake/server.py` & `sanic-23.6.0/tests/fake/server.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/http3/test_http_receiver.py` & `sanic-23.6.0/tests/http3/test_http_receiver.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/http3/test_server.py` & `sanic-23.6.0/tests/http3/test_server.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/http3/test_session_ticket_store.py` & `sanic-23.6.0/tests/http3/test_session_ticket_store.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/performance/sanic/http_response.py` & `sanic-23.6.0/tests/performance/sanic/http_response.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/performance/sanic/varied_server.py` & `sanic-23.6.0/tests/performance/sanic/varied_server.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/performance/wheezy/simple_server.py` & `sanic-23.6.0/tests/performance/wheezy/simple_server.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/skip_test_custom_protocol.py` & `sanic-23.6.0/tests/skip_test_custom_protocol.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/static/bp/python.png` & `sanic-23.6.0/tests/static/bp/python.png`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/static/python.png` & `sanic-23.6.0/tests/static/python.png`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/static/test.html` & `sanic-23.6.0/tests/static/test.html`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_app.py` & `sanic-23.6.0/tests/test_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         "sanic.error",
         logging.ERROR,
         f"Exception occurred while handling uri: 'http://127.0.0.1:{port}/'",
     ) in caplog.record_tuples
 
 
 def test_app_name_required():
-    with pytest.raises(SanicException):
+    with pytest.raises(TypeError):
         Sanic()
 
 
 def test_app_has_test_mode_sync():
     app = Sanic("test")
 
     @app.get("/")
```

### Comparing `sanic-23.3.0/tests/test_asgi.py` & `sanic-23.6.0/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_bad_request.py` & `sanic-23.6.0/tests/test_bad_request.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_base.py` & `sanic-23.6.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_blueprint_copy.py` & `sanic-23.6.0/tests/test_blueprint_copy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-from sanic import Blueprint, Sanic
+import pytest
+
+from sanic_routing.exceptions import RouteExists
+
+from sanic import Blueprint, Request, Sanic
 from sanic.response import text
 
 
 def test_bp_copy(app: Sanic):
     bp1 = Blueprint("test_bp1", version=1)
     bp1.ctx.test = 1
     assert hasattr(bp1.ctx, "test")
@@ -70,7 +74,80 @@
     route_names = [route.name for route in app.router.routes]
     assert "test_bp_copy.test_bp1.handle_request" in route_names
     assert "test_bp_copy.test_bp2.handle_request" in route_names
     assert "test_bp_copy.test_bp3.handle_request" in route_names
     assert "test_bp_copy.test_bp4.handle_request" in route_names
     assert "test_bp_copy.test_bp5.handle_request" in route_names
     assert "test_bp_copy.test_bp6.handle_request" in route_names
+
+
+def test_bp_copy_without_route_overwriting(app: Sanic):
+    bpv1 = Blueprint("bp_v1", version=1, url_prefix="my_api")
+
+    @bpv1.route("/")
+    async def handler(request: Request):
+        return text("v1")
+
+    app.blueprint(bpv1)
+
+    bpv2 = bpv1.copy("bp_v2", version=2, allow_route_overwrite=False)
+    bpv3 = bpv1.copy(
+        "bp_v3",
+        version=3,
+        allow_route_overwrite=False,
+        with_registration=False,
+    )
+
+    with pytest.raises(RouteExists, match="Route already registered*"):
+
+        @bpv2.route("/")
+        async def handler(request: Request):
+            return text("v2")
+
+        app.blueprint(bpv2)
+
+    with pytest.raises(RouteExists, match="Route already registered*"):
+
+        @bpv3.route("/")
+        async def handler(request: Request):
+            return text("v3")
+
+        app.blueprint(bpv3)
+
+
+def test_bp_copy_with_route_overwriting(app: Sanic):
+    bpv1 = Blueprint("bp_v1", version=1, url_prefix="my_api")
+
+    @bpv1.route("/")
+    async def handler(request: Request):
+        return text("v1")
+
+    app.blueprint(bpv1)
+
+    bpv2 = bpv1.copy("bp_v2", version=2, allow_route_overwrite=True)
+    bpv3 = bpv1.copy(
+        "bp_v3", version=3, allow_route_overwrite=True, with_registration=False
+    )
+
+    @bpv2.route("/")
+    async def handler(request: Request):
+        return text("v2")
+
+    app.blueprint(bpv2)
+
+    @bpv3.route("/")
+    async def handler(request: Request):
+        return text("v3")
+
+    app.blueprint(bpv3)
+
+    _, response = app.test_client.get("/v1/my_api")
+    assert response.status == 200
+    assert response.text == "v1"
+
+    _, response = app.test_client.get("/v2/my_api")
+    assert response.status == 200
+    assert response.text == "v2"
+
+    _, response = app.test_client.get("/v3/my_api")
+    assert response.status == 200
+    assert response.text == "v3"
```

### Comparing `sanic-23.3.0/tests/test_blueprint_group.py` & `sanic-23.6.0/tests/test_blueprint_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 from pytest import raises
 
 from sanic.app import Sanic
 from sanic.blueprint_group import BlueprintGroup
 from sanic.blueprints import Blueprint
 from sanic.exceptions import BadRequest, Forbidden, SanicException, ServerError
 from sanic.request import Request
@@ -336,7 +338,44 @@
 
     app = Sanic("PropTest")
     app.blueprint(three)
     app.router.finalize()
 
     routes = [route.path for route in app.router.routes]
     assert routes == ["three/one/four"]
+
+
+@pytest.mark.asyncio
+async def test_multiple_nested_bp_group():
+    bp1 = Blueprint("bp1", url_prefix="/bp1")
+    bp2 = Blueprint("bp2", url_prefix="/bp2")
+
+    bp1.add_route(lambda _: ..., "/", name="route1")
+    bp2.add_route(lambda _: ..., "/", name="route2")
+
+    group_a = Blueprint.group(
+        bp1, bp2, url_prefix="/group-a", name_prefix="group-a"
+    )
+    group_b = Blueprint.group(
+        bp1, bp2, url_prefix="/group-b", name_prefix="group-b"
+    )
+
+    app = Sanic("PropTest")
+    app.blueprint(group_a)
+    app.blueprint(group_b)
+
+    await app._startup()
+
+    routes = [route.path for route in app.router.routes]
+    assert routes == [
+        "group-a/bp1",
+        "group-a/bp2",
+        "group-b/bp1",
+        "group-b/bp2",
+    ]
+    names = [route.name for route in app.router.routes]
+    assert names == [
+        "PropTest.group-a_bp1.route1",
+        "PropTest.group-a_bp2.route2",
+        "PropTest.group-b_bp1.route1",
+        "PropTest.group-b_bp2.route2",
+    ]
```

### Comparing `sanic-23.3.0/tests/test_blueprints.py` & `sanic-23.6.0/tests/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_cancellederror.py` & `sanic-23.6.0/tests/test_cancellederror.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_cli.py` & `sanic-23.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_coffee.py` & `sanic-23.6.0/tests/test_coffee.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_config.py` & `sanic-23.6.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_constants.py` & `sanic-23.6.0/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_cookies.py` & `sanic-23.6.0/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_create_task.py` & `sanic-23.6.0/tests/test_create_task.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_custom_request.py` & `sanic-23.6.0/tests/test_custom_request.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_deprecation.py` & `sanic-23.6.0/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_dynamic_routes.py` & `sanic-23.6.0/tests/test_dynamic_routes.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_errorpages.py` & `sanic-23.6.0/tests/test_errorpages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 
 import pytest
 
+import sanic
+
 from sanic import Sanic
 from sanic.config import Config
 from sanic.errorpages import TextRenderer, exception_response, guess_mime
 from sanic.exceptions import NotFound, SanicException
 from sanic.handlers import ErrorHandler
 from sanic.request import Request
 from sanic.response import HTTPResponse, empty, html, json, text
@@ -201,14 +203,35 @@
     _, response = app.test_client.get("/text")
     assert response.content_type == "application/json"
 
     _, response = app.test_client.get("/json")
     assert response.content_type == "text/plain; charset=utf-8"
 
 
+def test_blueprint_error_response_from_explicit_format(app):
+    bp = sanic.Blueprint("MyBlueprint")
+
+    @bp.get("/text", error_format="json")
+    def text_response(request):
+        raise Exception("oops")
+        return text("Never gonna see this")
+
+    @bp.get("/json", error_format="text")
+    def json_response(request):
+        raise Exception("oops")
+        return json({"message": "Never gonna see this"})
+
+    app.blueprint(bp)
+    _, response = app.test_client.get("/text")
+    assert response.content_type == "application/json"
+
+    _, response = app.test_client.get("/json")
+    assert response.content_type == "text/plain; charset=utf-8"
+
+
 def test_unknown_fallback_format(app):
     with pytest.raises(SanicException, match="Unknown format: bad"):
         app.config.FALLBACK_ERROR_FORMAT = "bad"
 
 
 def test_route_error_format_unknown(app):
     with pytest.raises(SanicException, match="Unknown format: bad"):
@@ -523,7 +546,30 @@
         guess_mime(fake_request, fallback)
 
     (logmsg,) = [
         r.message for r in caplog.records if r.funcName == "guess_mime"
     ]
 
     assert logmsg == expected
+
+
+@pytest.mark.parametrize(
+    "format,expected",
+    (
+        ("html", "text/html; charset=utf-8"),
+        ("text", "text/plain; charset=utf-8"),
+        ("json", "application/json"),
+    ),
+)
+def test_exception_header_on_renderers(app: Sanic, format, expected):
+    app.config.FALLBACK_ERROR_FORMAT = format
+
+    @app.get("/test")
+    def test(request):
+        raise SanicException(
+            "test", status_code=400, headers={"exception": "test"}
+        )
+
+    _, response = app.test_client.get("/test")
+    assert response.status == 400
+    assert response.headers.get("exception") == "test"
+    assert response.content_type == expected
```

### Comparing `sanic-23.3.0/tests/test_exceptions.py` & `sanic-23.6.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_exceptions_handler.py` & `sanic-23.6.0/tests/test_exceptions_handler.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_ext_integration.py` & `sanic-23.6.0/tests/test_ext_integration.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_graceful_shutdown.py` & `sanic-23.6.0/tests/test_graceful_shutdown.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_handler.py` & `sanic-23.6.0/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_handler_annotations.py` & `sanic-23.6.0/tests/test_handler_annotations.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_headers.py` & `sanic-23.6.0/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_helpers.py` & `sanic-23.6.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_http.py` & `sanic-23.6.0/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_http_alt_svc.py` & `sanic-23.6.0/tests/test_http_alt_svc.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_json_decoding.py` & `sanic-23.6.0/tests/test_json_decoding.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_json_encoding.py` & `sanic-23.6.0/tests/test_json_encoding.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_keep_alive_timeout.py` & `sanic-23.6.0/tests/test_keep_alive_timeout.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from sanic.compat import OS_IS_WINDOWS
 from sanic.response import text
 
 
 CONFIG_FOR_TESTS = {"KEEP_ALIVE_TIMEOUT": 2, "KEEP_ALIVE": True}
 
 PORT = 42001  # test_keep_alive_timeout_reuse doesn't work with random port
+MAX_LOOPS = 15
 port_counter = count()
 
 
 def get_port():
     return next(port_counter) + PORT
 
 
@@ -65,105 +66,155 @@
     bool(environ.get("SANIC_NO_UVLOOP")) or OS_IS_WINDOWS,
     reason="Not testable with current client",
 )
 def test_keep_alive_timeout_reuse():
     """If the server keep-alive timeout and client keep-alive timeout are
     both longer than the delay, the client _and_ server will successfully
     reuse the existing connection."""
-    port = get_port()
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    client = ReusableClient(keep_alive_timeout_app_reuse, loop=loop, port=port)
-    with client:
-        headers = {"Connection": "keep-alive"}
-        request, response = client.get("/1", headers=headers)
-        assert response.status == 200
-        assert response.text == "OK"
-        assert request.protocol.state["requests_count"] == 1
-
-        loop.run_until_complete(aio_sleep(1))
-
-        request, response = client.get("/1")
-        assert response.status == 200
-        assert response.text == "OK"
-        assert request.protocol.state["requests_count"] == 2
+    loops = 0
+    while True:
+        port = get_port()
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
+        client = ReusableClient(
+            keep_alive_timeout_app_reuse, loop=loop, port=port
+        )
+        try:
+            with client:
+                headers = {"Connection": "keep-alive"}
+                request, response = client.get("/1", headers=headers)
+                assert response.status == 200
+                assert response.text == "OK"
+                assert request.protocol.state["requests_count"] == 1
+
+                loop.run_until_complete(aio_sleep(1))
+
+                request, response = client.get("/1")
+                assert response.status == 200
+                assert response.text == "OK"
+                assert request.protocol.state["requests_count"] == 2
+        except OSError:
+            loops += 1
+            if loops > MAX_LOOPS:
+                raise
+            continue
+        else:
+            break
 
 
 @pytest.mark.skipif(
     bool(environ.get("SANIC_NO_UVLOOP"))
     or OS_IS_WINDOWS
     or platform.system() != "Linux",
     reason="Not testable with current client",
 )
 def test_keep_alive_client_timeout():
     """If the server keep-alive timeout is longer than the client
     keep-alive timeout, client will try to create a new connection here."""
-    port = get_port()
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    client = ReusableClient(
-        keep_alive_app_client_timeout, loop=loop, port=port
-    )
-    with client:
-        headers = {"Connection": "keep-alive"}
-        request, response = client.get("/1", headers=headers, timeout=1)
-
-        assert response.status == 200
-        assert response.text == "OK"
-        assert request.protocol.state["requests_count"] == 1
-
-        loop.run_until_complete(aio_sleep(2))
-        request, response = client.get("/1", timeout=1)
-        assert request.protocol.state["requests_count"] == 1
+    loops = 0
+    while True:
+        try:
+            port = get_port()
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+            client = ReusableClient(
+                keep_alive_app_client_timeout, loop=loop, port=port
+            )
+            with client:
+                headers = {"Connection": "keep-alive"}
+                request, response = client.get(
+                    "/1", headers=headers, timeout=1
+                )
+
+                assert response.status == 200
+                assert response.text == "OK"
+                assert request.protocol.state["requests_count"] == 1
+
+                loop.run_until_complete(aio_sleep(2))
+                request, response = client.get("/1", timeout=1)
+                assert request.protocol.state["requests_count"] == 1
+        except OSError:
+            loops += 1
+            if loops > MAX_LOOPS:
+                raise
+            continue
+        else:
+            break
 
 
 @pytest.mark.skipif(
     bool(environ.get("SANIC_NO_UVLOOP")) or OS_IS_WINDOWS,
     reason="Not testable with current client",
 )
 def test_keep_alive_server_timeout():
     """If the client keep-alive timeout is longer than the server
     keep-alive timeout, the client will either a 'Connection reset' error
     _or_ a new connection. Depending on how the event-loop handles the
     broken server connection."""
-    port = get_port()
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    client = ReusableClient(
-        keep_alive_app_server_timeout, loop=loop, port=port
-    )
-    with client:
-        headers = {"Connection": "keep-alive"}
-        request, response = client.get("/1", headers=headers, timeout=60)
-
-        assert response.status == 200
-        assert response.text == "OK"
-        assert request.protocol.state["requests_count"] == 1
-
-        loop.run_until_complete(aio_sleep(3))
-        request, response = client.get("/1", timeout=60)
-
-        assert request.protocol.state["requests_count"] == 1
+    loops = 0
+    while True:
+        try:
+            port = get_port()
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+            client = ReusableClient(
+                keep_alive_app_server_timeout, loop=loop, port=port
+            )
+            with client:
+                headers = {"Connection": "keep-alive"}
+                request, response = client.get(
+                    "/1", headers=headers, timeout=60
+                )
+
+                assert response.status == 200
+                assert response.text == "OK"
+                assert request.protocol.state["requests_count"] == 1
+
+                loop.run_until_complete(aio_sleep(3))
+                request, response = client.get("/1", timeout=60)
+
+                assert request.protocol.state["requests_count"] == 1
+        except OSError:
+            loops += 1
+            if loops > MAX_LOOPS:
+                raise
+            continue
+        else:
+            break
 
 
 @pytest.mark.skipif(
     bool(environ.get("SANIC_NO_UVLOOP")) or OS_IS_WINDOWS,
     reason="Not testable with current client",
 )
 def test_keep_alive_connection_context():
-    port = get_port()
-    loop = asyncio.new_event_loop()
-    asyncio.set_event_loop(loop)
-    client = ReusableClient(keep_alive_app_context, loop=loop, port=port)
-    with client:
-        headers = {"Connection": "keep-alive"}
-        request1, _ = client.post("/ctx", headers=headers)
-
-        loop.run_until_complete(aio_sleep(1))
-        request2, response = client.get("/ctx")
-
-        assert response.text == "hello"
-        assert id(request1.conn_info.ctx) == id(request2.conn_info.ctx)
-        assert (
-            request1.conn_info.ctx.foo == request2.conn_info.ctx.foo == "hello"
-        )
-        assert request2.protocol.state["requests_count"] == 2
+    loops = 0
+    while True:
+        try:
+            port = get_port()
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+            client = ReusableClient(
+                keep_alive_app_context, loop=loop, port=port
+            )
+            with client:
+                headers = {"Connection": "keep-alive"}
+                request1, _ = client.post("/ctx", headers=headers)
+
+                loop.run_until_complete(aio_sleep(1))
+                request2, response = client.get("/ctx")
+
+                assert response.text == "hello"
+                assert id(request1.conn_info.ctx) == id(request2.conn_info.ctx)
+                assert (
+                    request1.conn_info.ctx.foo
+                    == request2.conn_info.ctx.foo
+                    == "hello"
+                )
+                assert request2.protocol.state["requests_count"] == 2
+        except OSError:
+            loops += 1
+            if loops > MAX_LOOPS:
+                raise
+            continue
+        else:
+            break
```

### Comparing `sanic-23.3.0/tests/test_late_adds.py` & `sanic-23.6.0/tests/test_late_adds.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_logging.py` & `sanic-23.6.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_logo.py` & `sanic-23.6.0/tests/test_logo.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_middleware.py` & `sanic-23.6.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_middleware_priority.py` & `sanic-23.6.0/tests/test_middleware_priority.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_motd.py` & `sanic-23.6.0/tests/test_motd.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_multi_serve.py` & `sanic-23.6.0/tests/test_multi_serve.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_multiprocessing.py` & `sanic-23.6.0/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_named_routes.py` & `sanic-23.6.0/tests/test_named_routes.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_payload_too_large.py` & `sanic-23.6.0/tests/test_payload_too_large.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_pipelining.py` & `sanic-23.6.0/tests/test_pipelining.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_prepare.py` & `sanic-23.6.0/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_redirect.py` & `sanic-23.6.0/tests/test_redirect.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,14 @@
 
     @app.route("/api/v1/test/<test>/")
     async def init_handler(request, test):
         return redirect(f"/api/v2/test/{use_in_uri}/")
 
     @app.route("/api/v2/test/<test>/", unquote=True)
     async def target_handler(request, test):
-        assert test == test_str
+        assert test == quote(test_str)
         return text("OK")
 
     _, response = app.test_client.get(f"/api/v1/test/{use_in_uri}/")
     assert response.status == 200
 
     assert response.body == b"OK"
```

### Comparing `sanic-23.3.0/tests/test_reloader.py` & `sanic-23.6.0/tests/test_reloader.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_request.py` & `sanic-23.6.0/tests/test_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,7 +306,33 @@
         ("POST", False),
         ("PUT", False),
     ),
 )
 def test_request_cacheable(method, cacheable):
     request = Request(b"/", {}, None, method, None, None)
     assert request.is_cacheable is cacheable
+
+
+def test_custom_ctx():
+    class CustomContext:
+        FOO = "foo"
+
+    class CustomRequest(Request[Sanic, CustomContext]):
+        @staticmethod
+        def make_context() -> CustomContext:
+            return CustomContext()
+
+    app = Sanic("Test", request_class=CustomRequest)
+
+    @app.get("/")
+    async def handler(request: CustomRequest):
+        return response.json(
+            [
+                isinstance(request, CustomRequest),
+                isinstance(request.ctx, CustomContext),
+                request.ctx.FOO,
+            ]
+        )
+
+    _, resp = app.test_client.get("/")
+
+    assert resp.json == [True, True, "foo"]
```

### Comparing `sanic-23.3.0/tests/test_request_cancel.py` & `sanic-23.6.0/tests/test_request_cancel.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_request_data.py` & `sanic-23.6.0/tests/test_request_data.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_request_stream.py` & `sanic-23.6.0/tests/test_request_stream.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_requests.py` & `sanic-23.6.0/tests/test_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,14 +509,15 @@
         "X-Forwarded-For": "127.0.1.1",
         "X-Scheme": "ws",
         "Host": "local.site",
     }
     request, response = app.test_client.get("/", headers=headers)
     assert response.json == {"for": "127.0.0.2", "proto": "ws"}
     assert request.remote_addr == "127.0.0.2"
+    assert request.client_ip == "127.0.0.2"
     assert request.scheme == "ws"
     assert request.server_name == "local.site"
     assert request.server_port == 80
 
     app.config.FORWARDED_SECRET = "mySecret"
     request, response = app.test_client.get("/", headers=headers)
     assert response.json == {
@@ -733,14 +734,15 @@
     request, response = app.test_client.get("/", headers=headers)
     assert request.remote_addr == "127.0.0.2"
     assert response.body == b"127.0.0.2"
 
     headers = {"X-Forwarded-For": "127.0.1.1"}
     request, response = app.test_client.get("/", headers=headers)
     assert request.remote_addr == ""
+    assert request.client_ip == "127.0.0.1"
     assert response.body == b""
 
     headers = {"X-Forwarded-For": "127.0.0.1, 127.0.1.2"}
     request, response = app.test_client.get("/", headers=headers)
     assert request.remote_addr == "127.0.0.1"
     assert response.body == b"127.0.0.1"
```

### Comparing `sanic-23.3.0/tests/test_response.py` & `sanic-23.6.0/tests/test_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from pytest import LogCaptureFixture
 
 from sanic import Request, Sanic
 from sanic.compat import Header
 from sanic.cookies import CookieJar
 from sanic.response import (
     HTTPResponse,
+    ResponseStream,
     empty,
     file,
     file_stream,
     json,
     raw,
     text,
 )
@@ -939,7 +940,21 @@
             "if-modified-since": formatdate(
                 last_modified.timestamp(), usegmt=True
             )
         },
     )
     assert response.status == 304
     assert response.body == b""
+
+
+def test_stream_response_with_default_headers(app: Sanic):
+    async def sample_streaming_fn(response_):
+        await response_.write("foo")
+
+    @app.route("/")
+    async def test(request: Request):
+        return ResponseStream(sample_streaming_fn, content_type="text/csv")
+
+    _, response = app.test_client.get("/")
+    assert response.text == "foo"
+    assert response.headers["Transfer-Encoding"] == "chunked"
+    assert response.headers["Content-Type"] == "text/csv"
```

### Comparing `sanic-23.3.0/tests/test_response_file.py` & `sanic-23.6.0/tests/test_response_file.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_response_json.py` & `sanic-23.6.0/tests/test_response_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,7 +209,16 @@
         with pytest.raises(
             TypeError, match="pop doesn't accept a default argument for lists"
         ):
             response.pop(21, "nah nah")
 
     _, resp = json_app.test_client.get("/json-pop")
     assert resp.body == json_dumps(["b"]).encode()
+
+
+def test_json_response_class_sets_proper_content_type(json_app: Sanic):
+    @json_app.get("/json-class")
+    async def handler(request: Request):
+        return JSONResponse(JSON_BODY)
+
+    _, resp = json_app.test_client.get("/json-class")
+    assert resp.headers["content-type"] == "application/json"
```

### Comparing `sanic-23.3.0/tests/test_response_timeout.py` & `sanic-23.6.0/tests/test_response_timeout.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_routes.py` & `sanic-23.6.0/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_server_events.py` & `sanic-23.6.0/tests/test_server_events.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_server_loop.py` & `sanic-23.6.0/tests/test_server_loop.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_signal_handlers.py` & `sanic-23.6.0/tests/test_signal_handlers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import asyncio
 import os
 import signal
 
 from queue import Queue
 from types import SimpleNamespace
+from typing import Optional
 from unittest.mock import MagicMock
 
 import pytest
 
 from sanic_testing.testing import HOST, PORT
 
+from sanic import Sanic
 from sanic.compat import ctrlc_workaround_for_windows
-from sanic.exceptions import BadRequest
+from sanic.exceptions import BadRequest, ServerError
 from sanic.response import HTTPResponse
+from sanic.signals import Event
 
 
 async def stop(app, loop):
     await asyncio.sleep(0.1)
     app.stop()
 
 
@@ -144,7 +147,30 @@
     async def hello_route(request):
         return HTTPResponse()
 
     with pytest.raises(
         BadRequest, match="Invalid event registration: Missing event name"
     ):
         app.listener(stop)
+
+
+def test_signal_server_lifecycle_exception(app: Sanic):
+    trigger: Optional[Exception] = None
+
+    @app.route("/hello")
+    async def hello_route(request):
+        return HTTPResponse()
+
+    @app.signal(Event.SERVER_EXCEPTION_REPORT)
+    async def test_signal(exception: Exception):
+        nonlocal trigger
+        trigger = exception
+
+    @app.before_server_start
+    async def test_before_server_start(app):
+        raise ServerError("test_before_server_start")
+
+    with pytest.raises(ServerError, match="test_before_server_start"):
+        app.run(single_process=True)
+
+    assert isinstance(trigger, ServerError)
+    assert str(trigger) == "test_before_server_start"
```

### Comparing `sanic-23.3.0/tests/test_static.py` & `sanic-23.6.0/tests/test_static.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,39 @@
     request, response = app.test_client.get("/testing.file")
     assert response.status == 200
     assert response.body == get_file_content(static_file_directory, file_name)
 
 
 @pytest.mark.parametrize(
     "file_name",
+    [
+        "test.file",
+        "decode me.txt",
+        "python.png",
+        "symlink",
+        "hard_link",
+    ],
+)
+def test_static_file_pathlib_relative_path_traversal(
+    app, static_file_directory, file_name
+):
+    """Get the current working directory and check if it ends with "sanic" """
+    cwd = Path.cwd()
+    if not str(cwd).endswith("sanic"):
+        pytest.skip("Current working directory does not end with 'sanic'")
+
+    file_path = "./tests/static/../static/"
+    app.static("/", file_path)
+    _, response = app.test_client.get(f"/{file_name}")
+    assert response.status == 200
+    assert response.body == get_file_content(static_file_directory, file_name)
+
+
+@pytest.mark.parametrize(
+    "file_name",
     [b"test.file", b"decode me.txt", b"python.png"],
 )
 def test_static_file_bytes(app, static_file_directory, file_name):
     bsep = os.path.sep.encode("utf-8")
     file_path = static_file_directory.encode("utf-8") + bsep + file_name
     message = "Static file or directory must be a path-like object or string"
     with pytest.raises(TypeError, match=message):
```

### Comparing `sanic-23.3.0/tests/test_static_directory.py` & `sanic-23.6.0/tests/test_static_directory.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_tasks.py` & `sanic-23.6.0/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_test_client_port.py` & `sanic-23.6.0/tests/test_test_client_port.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_timeout_logic.py` & `sanic-23.6.0/tests/test_timeout_logic.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_tls.py` & `sanic-23.6.0/tests/test_tls.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_touchup.py` & `sanic-23.6.0/tests/test_touchup.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_unix_socket.py` & `sanic-23.6.0/tests/test_unix_socket.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_url_building.py` & `sanic-23.6.0/tests/test_url_building.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_url_for.py` & `sanic-23.6.0/tests/test_url_for.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_url_for_static.py` & `sanic-23.6.0/tests/test_url_for_static.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_utf8.py` & `sanic-23.6.0/tests/test_utf8.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_utils.py` & `sanic-23.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_versioning.py` & `sanic-23.6.0/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_vhosts.py` & `sanic-23.6.0/tests/test_vhosts.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_views.py` & `sanic-23.6.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_websockets.py` & `sanic-23.6.0/tests/test_websockets.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/test_ws_handlers.py` & `sanic-23.6.0/tests/test_ws_handlers.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/worker/test_inspector.py` & `sanic-23.6.0/tests/worker/test_inspector.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/worker/test_loader.py` & `sanic-23.6.0/tests/worker/test_loader.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/worker/test_manager.py` & `sanic-23.6.0/tests/worker/test_manager.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/worker/test_multiplexer.py` & `sanic-23.6.0/tests/worker/test_multiplexer.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/worker/test_reloader.py` & `sanic-23.6.0/tests/worker/test_reloader.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/worker/test_runner.py` & `sanic-23.6.0/tests/worker/test_runner.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/worker/test_shared_ctx.py` & `sanic-23.6.0/tests/worker/test_shared_ctx.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/worker/test_socket.py` & `sanic-23.6.0/tests/worker/test_socket.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/worker/test_startup.py` & `sanic-23.6.0/tests/worker/test_startup.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/worker/test_state.py` & `sanic-23.6.0/tests/worker/test_state.py`

 * *Files identical despite different names*

### Comparing `sanic-23.3.0/tests/worker/test_worker_serve.py` & `sanic-23.6.0/tests/worker/test_worker_serve.py`

 * *Files identical despite different names*

