# Comparing `tmp/sanic-ext-23.3.0.tar.gz` & `tmp/sanic-ext-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanic-ext-23.3.0.tar", last modified: Sun Mar 26 19:59:24 2023, max compression
+gzip compressed data, was "sanic-ext-23.6.0.tar", last modified: Tue Jul 25 09:49:08 2023, max compression
```

## Comparing `sanic-ext-23.3.0.tar` & `sanic-ext-23.6.0.tar`

### file list

```diff
@@ -1,136 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.994142 sanic-ext-23.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-03-26 19:59:23.994142 sanic-ext-23.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.986142 sanic-ext-23.3.0/sanic_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.986142 sanic-ext-23.3.0/sanic_ext/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.986142 sanic-ext-23.3.0/sanic_ext/extensions/health/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/health/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/health/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/health/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.986142 sanic-ext-23.3.0/sanic_ext/extensions/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/http/cors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/http/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/http/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.986142 sanic-ext-23.3.0/sanic_ext/extensions/injection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/injection/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/injection/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/injection/injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/injection/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.986142 sanic-ext-23.3.0/sanic_ext/extensions/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/logging/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/sanic_ext/extensions/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/openapi/autodoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/openapi/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/openapi/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/openapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/openapi/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/openapi/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/openapi/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    11175 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/openapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/sanic_ext/extensions/openapi/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/openapi/ui/redoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/openapi/ui/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/sanic_ext/extensions/templating/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/templating/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/templating/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extensions/templating/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/sanic_ext/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extras/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/sanic_ext/extras/serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extras/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extras/serializer/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/sanic_ext/extras/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extras/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extras/validation/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extras/validation/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extras/validation/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extras/validation/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extras/validation/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/extras/validation/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/sanic_ext/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/utils/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/utils/route.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/sanic_ext/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.986142 sanic-ext-23.3.0/sanic_ext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-03-26 19:59:23.000000 sanic-ext-23.3.0/sanic_ext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-03-26 19:59:23.000000 sanic-ext-23.3.0/sanic_ext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 19:59:23.000000 sanic-ext-23.3.0/sanic_ext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-26 19:59:23.000000 sanic-ext-23.3.0/sanic_ext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-26 19:59:23.000000 sanic-ext-23.3.0/sanic_ext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-26 19:59:23.994142 sanic-ext-23.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/tests/extensions/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/http/test_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/tests/extensions/injection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/injection/test_add_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/injection/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/injection/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/injection/test_injection_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/injection/test_injection_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.990142 sanic-ext-23.3.0/tests/extensions/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/logging/test_custom_background_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.994142 sanic-ext-23.3.0/tests/extensions/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_autodoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24588 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_exclude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_external_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_model_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_model_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_security.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/openapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.994142 sanic-ext-23.3.0/tests/extensions/templating/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/templating/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.994142 sanic-ext-23.3.0/tests/extensions/templating/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/templating/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/templating/test_templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extensions/test_startup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:23.994142 sanic-ext-23.3.0/tests/extra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extra/__models__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extra/test_parse_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extra/test_request_counted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extra/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extra/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extra/test_validation_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extra/test_validation_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extra/test_validation_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-03-26 19:59:13.000000 sanic-ext-23.3.0/tests/extra/test_validation_pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.898285 sanic-ext-23.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-25 09:49:08.898285 sanic-ext-23.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.886285 sanic-ext-23.6.0/sanic_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.886285 sanic-ext-23.6.0/sanic_ext/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.886285 sanic-ext-23.6.0/sanic_ext/extensions/health/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/health/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/health/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/health/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.886285 sanic-ext-23.6.0/sanic_ext/extensions/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/http/cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/http/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/http/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.886285 sanic-ext-23.6.0/sanic_ext/extensions/injection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/injection/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/injection/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/injection/injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/injection/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.886285 sanic-ext-23.6.0/sanic_ext/extensions/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/logging/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.886285 sanic-ext-23.6.0/sanic_ext/extensions/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/openapi/autodoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/openapi/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/openapi/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/openapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/openapi/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/openapi/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/openapi/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/openapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.890285 sanic-ext-23.6.0/sanic_ext/extensions/openapi/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/openapi/ui/redoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/openapi/ui/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.890285 sanic-ext-23.6.0/sanic_ext/extensions/templating/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/templating/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/templating/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extensions/templating/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.890285 sanic-ext-23.6.0/sanic_ext/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extras/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.890285 sanic-ext-23.6.0/sanic_ext/extras/serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extras/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extras/serializer/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.890285 sanic-ext-23.6.0/sanic_ext/extras/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extras/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extras/validation/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extras/validation/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extras/validation/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extras/validation/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extras/validation/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/extras/validation/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.890285 sanic-ext-23.6.0/sanic_ext/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/utils/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/utils/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/sanic_ext/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.886285 sanic-ext-23.6.0/sanic_ext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-25 09:49:08.000000 sanic-ext-23.6.0/sanic_ext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-25 09:49:08.000000 sanic-ext-23.6.0/sanic_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:49:08.000000 sanic-ext-23.6.0/sanic_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-25 09:49:08.000000 sanic-ext-23.6.0/sanic_ext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 09:49:08.000000 sanic-ext-23.6.0/sanic_ext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 09:49:08.898285 sanic-ext-23.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.890285 sanic-ext-23.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.890285 sanic-ext-23.6.0/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.890285 sanic-ext-23.6.0/tests/extensions/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/http/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.890285 sanic-ext-23.6.0/tests/extensions/injection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/injection/test_add_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/injection/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/injection/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/injection/test_injection_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/injection/test_injection_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.890285 sanic-ext-23.6.0/tests/extensions/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/logging/test_custom_background_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.894285 sanic-ext-23.6.0/tests/extensions/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_autodoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24588 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_external_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_func_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_model_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_model_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/openapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.894285 sanic-ext-23.6.0/tests/extensions/templating/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/templating/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.894285 sanic-ext-23.6.0/tests/extensions/templating/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/templating/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/templating/test_templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extensions/test_startup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:49:08.898285 sanic-ext-23.6.0/tests/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extra/__models__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extra/test_parse_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extra/test_request_counted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extra/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extra/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extra/test_validation_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extra/test_validation_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extra/test_validation_msgspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extra/test_validation_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-25 09:48:56.000000 sanic-ext-23.6.0/tests/extra/test_validation_pydantic.py
```

### Comparing `sanic-ext-23.3.0/LICENSE` & `sanic-ext-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/PKG-INFO` & `sanic-ext-23.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanic-ext
-Version: 23.3.0
+Version: 23.6.0
 Summary: Extend your Sanic installation with some core functionality.
 Home-page: http://github.com/sanic-org/sanic-ext/
 Author: Sanic Community
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -111,7 +111,9 @@
 Go to the `User Guide <https://sanicframework.org/en/plugins/sanic-ext/getting-started.html>`_ to learn more
 
 ____
 
 .. warning:: Sanic Extensions is still in **ALPHA** release. The API is not likely to change. It will move to **BETA** with v22.3.
 
 
+
+
```

### Comparing `sanic-ext-23.3.0/README.rst` & `sanic-ext-23.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/__init__.py` & `sanic-ext-23.6.0/sanic_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/bootstrap.py` & `sanic-ext-23.6.0/sanic_ext/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/config.py` & `sanic-ext-23.6.0/sanic_ext/config.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/base.py` & `sanic-ext-23.6.0/sanic_ext/extensions/base.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/health/extension.py` & `sanic-ext-23.6.0/sanic_ext/extensions/health/extension.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/health/monitor.py` & `sanic-ext-23.6.0/sanic_ext/extensions/health/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         now = datetime.now()
         health_state = {
             process_name: HealthState(last=now, name=process_name)
             for process_name in process_names
         }
         while self.run:
             try:
-                name, timestamp = health_queue.get_nowait()
+                name, timestamp = health_queue.get(timeout=0.05)
             except Empty:
                 ...
             else:
                 health_state[name].report(timestamp)
 
             for state in health_state.values():
                 try:
```

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/http/cors.py` & `sanic-ext-23.6.0/sanic_ext/extensions/http/cors.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/http/extension.py` & `sanic-ext-23.6.0/sanic_ext/extensions/http/extension.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/http/methods.py` & `sanic-ext-23.6.0/sanic_ext/extensions/http/methods.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/injection/constructor.py` & `sanic-ext-23.6.0/sanic_ext/extensions/injection/constructor.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 )
 
 from sanic import Request
 from sanic.app import Sanic
 from sanic.exceptions import ServerError
 
 from sanic_ext.exceptions import InitError
-from sanic_ext.utils.typing import is_attrs, is_optional, is_pydantic
+from sanic_ext.utils.typing import (
+    is_attrs,
+    is_msgspec,
+    is_optional,
+    is_pydantic,
+)
 
 if TYPE_CHECKING:
     from .registry import ConstantRegistry, InjectionRegistry
 
 
 class Constructor:
     EXEMPT_ANNOTATIONS = (Request,)
@@ -149,14 +154,15 @@
 
     def _get_hints(self):
         if (
             not isclass(self.func)
             or is_dataclass(self.func)
             or is_attrs(self.func)
             or is_pydantic(self.func)
+            or is_msgspec(self.func)
         ):
             return get_type_hints(self.func)
         elif isclass(self.func):
             return get_type_hints(self.func.__init__)
         raise InitError(f"Cannot get type hints for {self.func}")
```

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/injection/extension.py` & `sanic-ext-23.6.0/sanic_ext/extensions/injection/extension.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/injection/injector.py` & `sanic-ext-23.6.0/sanic_ext/extensions/injection/injector.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/injection/registry.py` & `sanic-ext-23.6.0/sanic_ext/extensions/injection/registry.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/logging/extension.py` & `sanic-ext-23.6.0/sanic_ext/extensions/logging/extension.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/logging/logger.py` & `sanic-ext-23.6.0/sanic_ext/extensions/logging/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def __call__(self, queue) -> None:
         signal_func(SIGINT, self.stop)
         signal_func(SIGTERM, self.stop)
 
         while self.run:
             try:
-                record: LogRecord = queue.get_nowait()
+                record: LogRecord = queue.get(timeout=0.05)
             except Empty:
                 continue
             logger = self.loggers.get(record.name)
             logger.handle(record)
 
     def stop(self, *_):
         if self.run:
```

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/openapi/autodoc.py` & `sanic-ext-23.6.0/sanic_ext/extensions/openapi/autodoc.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/openapi/blueprint.py` & `sanic-ext-23.6.0/sanic_ext/extensions/openapi/blueprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,27 +136,32 @@
             method_handlers,
             host,
         ) in get_all_routes(app, bp.url_prefix):
             # --------------------------------------------------------------- #
             # Methods
             # --------------------------------------------------------------- #
 
-            uri = uri if uri == "/" else uri.rstrip("/")
-
             for method, _handler in method_handlers:
                 if (
                     (method == "OPTIONS" and app.config.OAS_IGNORE_OPTIONS)
                     or (method == "HEAD" and app.config.OAS_IGNORE_HEAD)
                     or method == "TRACE"
                 ):
                     continue
 
                 if hasattr(_handler, "view_class"):
                     _handler = getattr(_handler.view_class, method.lower())
-                operation = OperationStore()[_handler]
+                store = OperationStore()
+                if (
+                    _handler not in store
+                    and (func := getattr(_handler, "__func__", None))
+                    and func in store
+                ):
+                    _handler = func
+                operation = store[_handler]
 
                 if operation._exclude or "openapi" in operation.tags:
                     continue
 
                 docstring = inspect.getdoc(_handler)
 
                 if (
```

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/openapi/builders.py` & `sanic-ext-23.6.0/sanic_ext/extensions/openapi/builders.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/openapi/constants.py` & `sanic-ext-23.6.0/sanic_ext/extensions/openapi/constants.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/openapi/definitions.py` & `sanic-ext-23.6.0/sanic_ext/extensions/openapi/definitions.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/openapi/extension.py` & `sanic-ext-23.6.0/sanic_ext/extensions/openapi/extension.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/openapi/openapi.py` & `sanic-ext-23.6.0/sanic_ext/extensions/openapi/openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     Double,
     Email,
     Float,
     Integer,
     Long,
     Object,
     Password,
+    Schema,
     String,
     Time,
 )
 from sanic_ext.extras.validation.setup import do_validation, generate_schema
 from sanic_ext.utils.extraction import extract_request
 
 __all__ = (
@@ -259,25 +260,25 @@
 ) -> Callable[[T], T]:
     ...
 
 
 @overload
 def parameter(
     name: str,
-    schema: Optional[Type] = None,
+    schema: Optional[Union[Type, Schema]] = None,
     location: Optional[str] = None,
     parameter: None = None,
     **kwargs,
 ) -> Callable[[T], T]:
     ...
 
 
 def parameter(
     name: Optional[str] = None,
-    schema: Optional[Type] = None,
+    schema: Optional[Union[Type, Schema]] = None,
     location: Optional[str] = None,
     parameter: Optional[definitions.Parameter] = None,
     **kwargs,
 ) -> Callable[[T], T]:
     if parameter:
         if name or schema or location:
             raise SanicException(
```

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/openapi/types.py` & `sanic-ext-23.6.0/sanic_ext/extensions/openapi/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,23 +13,55 @@
     get_args,
     get_origin,
     get_type_hints,
 )
 
 from sanic_routing.patterns import alpha, ext, nonemptystr, parse_date, slug
 
-from sanic_ext.utils.typing import is_attrs, is_generic, is_pydantic
+from sanic_ext.utils.typing import (
+    UnionType,
+    is_attrs,
+    is_generic,
+    is_msgspec,
+    is_pydantic,
+)
 
 try:
     import attrs
 
     NOTHING: Any = attrs.NOTHING
 except ImportError:
     NOTHING = object()
 
+try:
+    import msgspec
+    from msgspec.inspect import Metadata as MsgspecMetadata
+    from msgspec.inspect import type_info as msgspec_type_info
+
+    MsgspecMetadata: Any = MsgspecMetadata
+    NODEFAULT: Any = msgspec.NODEFAULT
+    UNSET: Any = msgspec.UNSET
+
+    class MsgspecAdapter(msgspec.Struct):
+        name: str
+        default: Any
+        metadata: dict
+
+except ImportError:
+
+    def msgspec_type_info(struct):
+        pass
+
+    class MsgspecAdapter:
+        pass
+
+    MsgspecMetadata = object()
+    NODEFAULT = object()
+    UNSET = object()
+
 
 class Definition:
     __nullable__: Optional[List[str]] = []
     __ignore__: Optional[List[str]] = []
 
     def __init__(self, **kwargs):
         self._fields: Dict[str, Any] = self.guard(kwargs)
@@ -96,15 +128,15 @@
     enum: Union[List[Any], Enum]
 
     @staticmethod
     def make(value, **kwargs):
         _type = type(value)
         origin = get_origin(value)
         args = get_args(value)
-        if origin is Union:
+        if origin in (Union, UnionType):
             if type(None) in args:
                 kwargs["nullable"] = True
 
             filtered = [arg for arg in args if arg is not type(None)]  # noqa
 
             if len(filtered) == 1:
                 return Schema.make(filtered[0], **kwargs)
@@ -286,27 +318,41 @@
             kwargs["properties"] = properties
         super().__init__(type="object", **kwargs)
 
     @classmethod
     def make(cls, value: Any, **kwargs):
         extra: Dict[str, Any] = {}
 
-        # Extract from field metadata if pydantic, attrs, or dataclass
+        # Extract from field metadata if msgspec, pydantic, attrs, or dataclass
         if isclass(value):
             fields = ()
             if is_pydantic(value):
                 try:
                     value = value.__pydantic_model__
                 except AttributeError:
                     ...
                 extra = value.schema()["properties"]
             elif is_attrs(value):
                 fields = value.__attrs_attrs__
             elif is_dataclass(value):
                 fields = value.__dataclass_fields__.values()
+            elif is_msgspec(value):
+                # adapt to msgspec metadata layout -- annotated type --
+                # to match dataclass "metadata" attribute
+                fields = [
+                    MsgspecAdapter(
+                        name=f.name,
+                        default=MISSING
+                        if f.default in (UNSET, NODEFAULT)
+                        else f.default,
+                        metadata=getattr(f.type, "extra", {}),
+                    )
+                    for f in msgspec_type_info(value).fields
+                ]
+
             if fields:
                 extra = {
                     field.name: {
                         "title": field.name.title(),
                         **(
                             {"default": field.default}
                             if field.default not in (MISSING, NOTHING)
```

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/openapi/ui/redoc.html` & `sanic-ext-23.6.0/sanic_ext/extensions/openapi/ui/redoc.html`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/openapi/ui/swagger.html` & `sanic-ext-23.6.0/sanic_ext/extensions/openapi/ui/swagger.html`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/templating/engine.py` & `sanic-ext-23.6.0/sanic_ext/extensions/templating/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from functools import wraps
 from inspect import isawaitable
 from typing import TYPE_CHECKING, Dict, Optional, Union
 
 from jinja2 import Environment
 from sanic.compat import Header
+from sanic.request import Request
 from sanic.response import HTTPResponse
 
 from sanic_ext.extensions.templating.render import (
     LazyResponse,
     TemplateResponse,
 )
 
@@ -59,14 +60,16 @@
                 if isinstance(context, LazyResponse):
                     for attr in ("status", "headers", "content_type"):
                         value = getattr(context, attr, None)
                         if value:
                             params[attr] = value
                     context = context.context
 
+                context["request"] = Request.get_current()
+
                 content = render(**context)
                 if isawaitable(content):
                     content = await content
 
                 return HTTPResponse(content, **params)
 
             return decorated_function
```

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/templating/extension.py` & `sanic-ext-23.6.0/sanic_ext/extensions/templating/extension.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extensions/templating/render.py` & `sanic-ext-23.6.0/sanic_ext/extensions/templating/render.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from inspect import isawaitable
 from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 from sanic import Sanic
 from sanic.compat import Header
 from sanic.exceptions import SanicException
+from sanic.request import Request
 from sanic.response import HTTPResponse
 
 from sanic_ext.exceptions import ExtensionNotFound
 
 if TYPE_CHECKING:
     from jinja2 import Environment
 
@@ -72,14 +73,17 @@
         except AttributeError:
             raise ExtensionNotFound(
                 "The Templating extension does not appear to be enabled. "
                 "Perhaps jinja2 is not installed."
             )
 
     kwargs = context if context else {}
+
+    kwargs["request"] = Request.get_current()
+
     if template_name or template_source:
         template = (
             environment.get_template(template_name)
             if template_name
             else environment.from_string(template_source)
         )
```

### Comparing `sanic-ext-23.3.0/sanic_ext/extras/request.py` & `sanic-ext-23.6.0/sanic_ext/extras/request.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extras/serializer/decorator.py` & `sanic-ext-23.6.0/sanic_ext/extras/serializer/decorator.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extras/validation/check.py` & `sanic-ext-23.6.0/sanic_ext/extras/validation/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from __future__ import annotations
 
 from dataclasses import _HAS_DEFAULT_FACTORY  # type: ignore
 from typing import (
     Any,
     Literal,
+    Mapping,
     NamedTuple,
     Optional,
     Tuple,
     Union,
     get_args,
     get_origin,
 )
 
-from sanic_ext.utils.typing import UnionType, is_generic, is_optional
+from sanic_ext.utils.typing import (
+    UnionType,
+    is_generic,
+    is_msgspec,
+    is_optional,
+)
 
 MISSING: Tuple[Any, ...] = (_HAS_DEFAULT_FACTORY,)
 
 try:
     import attrs  # noqa
 
     NOTHING = attrs.NOTHING
@@ -25,14 +31,22 @@
         _HAS_DEFAULT_FACTORY,
         NOTHING,
     )
 except ImportError:
     ATTRS = False
 
 
+try:
+    import msgspec
+
+    MSGSPEC = True
+except ImportError:
+    MSGSPEC = False
+
+
 class Hint(NamedTuple):
     hint: Any
     model: bool
     literal: bool
     typed: bool
     nullable: bool
     origin: Optional[Any]
@@ -165,25 +179,38 @@
                 )
             except ValueError:
                 if not hint.allow_missing or value not in MISSING:
                     raise
     except ValueError as e:
         raise TypeError(e)
 
-    return model(**hydration_values)
+    if MSGSPEC and is_msgspec(model):
+        try:
+            return msgspec.from_builtins(
+                hydration_values, model, str_values=True, str_keys=True
+            )
+        except msgspec.ValidationError as e:
+            raise TypeError(e)
+    else:
+        return model(**hydration_values)
 
 
 def _check_types(value, literal, expected):
     if literal:
         if expected is Any:
             return
         elif value != expected:
             raise ValueError(f"Value '{value}' must be {expected}")
     else:
-        if not isinstance(value, expected):
+        if MSGSPEC and is_msgspec(expected) and isinstance(value, Mapping):
+            try:
+                expected(**value)
+            except (TypeError, msgspec.ValidationError):
+                raise ValueError(f"Value '{value}' is not of type {expected}")
+        elif not isinstance(value, expected):
             raise ValueError(f"Value '{value}' is not of type {expected}")
 
 
 def _check_nullability(
     value, nullable, allowed, schema, allow_multiple, allow_coerce
 ):
     if not nullable and value is None:
```

### Comparing `sanic-ext-23.3.0/sanic_ext/extras/validation/decorator.py` & `sanic-ext-23.6.0/sanic_ext/extras/validation/decorator.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extras/validation/schema.py` & `sanic-ext-23.6.0/sanic_ext/extras/validation/schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,43 +9,54 @@
     Tuple,
     Union,
     get_args,
     get_origin,
     get_type_hints,
 )
 
-from sanic_ext.utils.typing import is_attrs, is_generic
+from sanic_ext.utils.typing import is_attrs, is_generic, is_msgspec
 
 from .check import Hint
 
 try:
     UnionType = types.UnionType  # type: ignore
 except AttributeError:
     UnionType = type("UnionType", (), {})
 
 try:
     from attr import NOTHING, Attribute
 except ModuleNotFoundError:
     NOTHING = object()  # type: ignore
     Attribute = type("Attribute", (), {})  # type: ignore
 
+try:
+    from msgspec.inspect import type_info as msgspec_type_info
+except ModuleNotFoundError:
+
+    def msgspec_type_info(val):
+        pass
+
 
 def make_schema(agg, item):
     if type(item) in (bool, str, int, float):
         return agg
 
     if is_generic(item) and (args := get_args(item)):
         for arg in args:
             make_schema(agg, arg)
-    elif item.__name__ not in agg and (is_dataclass(item) or is_attrs(item)):
-        fields = (
-            item.__dataclass_fields__
-            if is_dataclass(item)
-            else {attr.name: attr for attr in item.__attrs_attrs__}
-        )
+    elif item.__name__ not in agg and (
+        is_dataclass(item) or is_attrs(item) or is_msgspec(item)
+    ):
+        if is_dataclass(item):
+            fields = item.__dataclass_fields__
+        elif is_msgspec(item):
+            fields = {f.name: f.type for f in msgspec_type_info(item).fields}
+        else:
+            fields = {attr.name: attr for attr in item.__attrs_attrs__}
+
         sig = signature(item)
         hints = parse_hints(get_type_hints(item), fields)
 
         agg[item.__name__] = {
             "sig": sig,
             "hints": hints,
         }
```

### Comparing `sanic-ext-23.3.0/sanic_ext/extras/validation/setup.py` & `sanic-ext-23.6.0/sanic_ext/extras/validation/setup.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/extras/validation/validators.py` & `sanic-ext-23.6.0/sanic_ext/extras/validation/validators.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/utils/route.py` & `sanic-ext-23.6.0/sanic_ext/utils/route.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext/utils/typing.py` & `sanic-ext-23.6.0/sanic_ext/utils/typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 try:
     import attrs  # noqa
 
     ATTRS = True
 except ImportError:
     ATTRS = False
 
+try:
+    from msgspec import Struct
+
+    MSGSPEC = True
+except ImportError:
+    MSGSPEC = False
+
 
 def is_generic(item):
     return (
         isinstance(item, typing._GenericAlias)
         or isinstance(item, UnionType)
         or hasattr(item, "__origin__")
     )
@@ -43,14 +50,18 @@
     )
 
 
 def is_attrs(model):
     return ATTRS and (hasattr(model, "__attrs_attrs__"))
 
 
+def is_msgspec(model):
+    return MSGSPEC and issubclass(model, Struct)
+
+
 def flat_values(
     item: typing.Union[
         typing.Dict[str, typing.Any], typing.Iterable[typing.Any]
     ]
 ) -> typing.Set[typing.Any]:
     values = set()
     if isinstance(item, dict):
```

### Comparing `sanic-ext-23.3.0/sanic_ext/utils/version.py` & `sanic-ext-23.6.0/sanic_ext/utils/version.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/sanic_ext.egg-info/PKG-INFO` & `sanic-ext-23.6.0/sanic_ext.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanic-ext
-Version: 23.3.0
+Version: 23.6.0
 Summary: Extend your Sanic installation with some core functionality.
 Home-page: http://github.com/sanic-org/sanic-ext/
 Author: Sanic Community
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -111,7 +111,9 @@
 Go to the `User Guide <https://sanicframework.org/en/plugins/sanic-ext/getting-started.html>`_ to learn more
 
 ____
 
 .. warning:: Sanic Extensions is still in **ALPHA** release. The API is not likely to change. It will move to **BETA** with v22.3.
 
 
+
+
```

### Comparing `sanic-ext-23.3.0/sanic_ext.egg-info/SOURCES.txt` & `sanic-ext-23.6.0/sanic_ext.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,19 @@
 tests/extensions/openapi/test_body.py
 tests/extensions/openapi/test_config.py
 tests/extensions/openapi/test_decorators.py
 tests/extensions/openapi/test_definitions.py
 tests/extensions/openapi/test_deprecated.py
 tests/extensions/openapi/test_exclude.py
 tests/extensions/openapi/test_external_docs.py
+tests/extensions/openapi/test_func_handler.py
 tests/extensions/openapi/test_model_fields.py
 tests/extensions/openapi/test_model_spec.py
 tests/extensions/openapi/test_parameter.py
+tests/extensions/openapi/test_paths.py
 tests/extensions/openapi/test_schema.py
 tests/extensions/openapi/test_security.py
 tests/extensions/openapi/test_specification.py
 tests/extensions/openapi/test_summary.py
 tests/extensions/openapi/test_tag.py
 tests/extensions/openapi/test_typing.py
 tests/extensions/openapi/utils.py
@@ -103,9 +105,10 @@
 tests/extra/__models__.py
 tests/extra/test_parse_hint.py
 tests/extra/test_request_counted.py
 tests/extra/test_serializer.py
 tests/extra/test_validation.py
 tests/extra/test_validation_attrs.py
 tests/extra/test_validation_dataclass.py
+tests/extra/test_validation_msgspec.py
 tests/extra/test_validation_multiple.py
 tests/extra/test_validation_pydantic.py
```

### Comparing `sanic-ext-23.3.0/setup.cfg` & `sanic-ext-23.6.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sanic-ext
-version = 23.3.0
+version = 23.6.0
 url = http://github.com/sanic-org/sanic-ext/
 license = MIT
 author = Sanic Community
 description = Extend your Sanic installation with some core functionality.
 long_description = file: README.rst
 platforms = any
 classifiers =
```

### Comparing `sanic-ext-23.3.0/tests/conftest.py` & `sanic-ext-23.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/http/test_methods.py` & `sanic-ext-23.6.0/tests/extensions/http/test_methods.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/injection/test_add_dependency.py` & `sanic-ext-23.6.0/tests/extensions/injection/test_add_dependency.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/injection/test_constants.py` & `sanic-ext-23.6.0/tests/extensions/injection/test_constants.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/injection/test_dependency.py` & `sanic-ext-23.6.0/tests/extensions/injection/test_dependency.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/injection/test_injection_config.py` & `sanic-ext-23.6.0/tests/extensions/injection/test_injection_config.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/injection/test_injection_registry.py` & `sanic-ext-23.6.0/tests/extensions/injection/test_injection_registry.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/logging/test_custom_background_logger.py` & `sanic-ext-23.6.0/tests/extensions/logging/test_custom_background_logger.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_autodoc.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_autodoc.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_body.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_body.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_config.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_config.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_decorators.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_decorators.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_definitions.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_definitions.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_deprecated.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_exclude.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_exclude.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_external_docs.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_external_docs.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_model_fields.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_model_fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+import sys
 from dataclasses import dataclass, field
 from typing import List
 from uuid import UUID
 
 import attrs
 import pytest
+from msgspec import Meta, Struct
 from pydantic import BaseModel, Field
 from pydantic.dataclasses import dataclass as pydataclass
 
 from sanic_ext import openapi
 
 from .utils import get_spec
 
+if sys.version_info >= (3, 9):
+    from typing import Annotated
+
 
 @dataclass
 class FooDataclass:
     links: List[UUID]
     priority: int = field(
         metadata={"openapi": {"exclusiveMinimum": 1, "exclusiveMaximum": 10}}
     )
@@ -43,24 +48,44 @@
 @pydataclass
 class FooPydanticDataclass:
     links: List[UUID]
     priority: int = Field(gt=1, lt=10)
     ident: str = Field("XXXX", example="ABC123")
 
 
-@pytest.mark.parametrize(
-    "Foo",
-    (
-        FooDataclass,
-        FooAttrs,
-        FooPydanticBaseModel,
-        FooPydanticDataclass,
-    ),
-)
-def test_pydantic_base_model(app, Foo):
+if sys.version_info >= (3, 9):
+
+    class FooStruct(Struct):
+        links: List[UUID]
+        priority: Annotated[
+            int,
+            Meta(
+                extra={
+                    "openapi": {"exclusiveMinimum": 1, "exclusiveMaximum": 10}
+                }
+            ),
+        ]
+        ident: Annotated[
+            str, Meta(extra={"openapi": {"example": "ABC123"}})
+        ] = "XXXX"
+
+
+models = [
+    FooDataclass,
+    FooAttrs,
+    FooPydanticBaseModel,
+    FooPydanticDataclass,
+]
+
+if sys.version_info >= (3, 9):
+    models.append(FooStruct)
+
+
+@pytest.mark.parametrize("Foo", models)
+def test_models(app, Foo):
     @app.get("/")
     @openapi.definition(body={"application/json": Foo})
     async def handler(_):
         ...
 
     spec = get_spec(app)
     foo_props = spec["paths"]["/"]["get"]["requestBody"]["content"][
```

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_model_spec.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_model_spec.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_parameter.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_parameter.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_schema.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_schema.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_security.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_security.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_specification.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_specification.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_summary.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_summary.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_tag.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_tag.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extensions/openapi/test_typing.py` & `sanic-ext-23.6.0/tests/extensions/openapi/test_typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,12 +37,14 @@
     ({"foo": List[str]}, True),
     ({"foo": Optional[str]}, True),
     ({"foo": Foo}, True),
     ({"foo": "str"}, False),
 ]
 if sys.version_info >= (3, 9):
     params.append(({"foo": list[str]}, True))
+if sys.version_info >= (3, 10):
+    params.append(({"foo": str | None}, True))
 
 
 @pytest.mark.parametrize("item,expected", params)
 def test_contains_annotations(item, expected):
     assert contains_annotations(item) == expected
```

### Comparing `sanic-ext-23.3.0/tests/extensions/templating/test_templating.py` & `sanic-ext-23.6.0/tests/extensions/templating/test_templating.py`

 * *Files 20% similar despite different names*

```diff
@@ -106,7 +106,48 @@
 
     @app.get("/one/two/three")
     async def handler(_):
         return await render(template_source=template)
 
     _, response = app.test_client.get("/one/two/three")
     assert response.text == "url: /one/two/three"
+
+
+def test_default_context():
+    app = Sanic("templating-from-string")
+    app.extend(
+        config={
+            "templating_path_to_templates": Path(__file__).parent / "templates"
+        }
+    )
+
+    template = r"{{ request.args.get('test') }}"
+
+    @app.get("/1")
+    async def handler1(_):
+        return await render(template_source=template)
+
+    @app.get("/2")
+    @app.ext.template("request_test.html")
+    async def handler2(_):
+        return {}
+
+    @app.get("/3")
+    async def handler3(_):
+        return await render("request_test.html", context={}, app=app)
+
+    @app.get("/4")
+    @app.ext.template("request_test.html")
+    async def handler4(_):
+        return await render(context={}, app=app)
+
+    _, response = app.test_client.get("/1?test=passing")
+    assert response.text == "passing"
+
+    _, response = app.test_client.get("/2?test=passing")
+    assert response.text == "passing"
+
+    _, response = app.test_client.get("/3?test=passing")
+    assert response.text == "passing"
+
+    _, response = app.test_client.get("/4?test=passing")
+    assert response.text == "passing"
```

### Comparing `sanic-ext-23.3.0/tests/extensions/test_startup.py` & `sanic-ext-23.6.0/tests/extensions/test_startup.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extra/__models__.py` & `sanic-ext-23.6.0/tests/extra/__models__.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extra/test_parse_hint.py` & `sanic-ext-23.6.0/tests/extra/test_parse_hint.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extra/test_request_counted.py` & `sanic-ext-23.6.0/tests/extra/test_request_counted.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extra/test_serializer.py` & `sanic-ext-23.6.0/tests/extra/test_serializer.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extra/test_validation.py` & `sanic-ext-23.6.0/tests/extra/test_validation.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extra/test_validation_attrs.py` & `sanic-ext-23.6.0/tests/extra/test_validation_attrs.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extra/test_validation_dataclass.py` & `sanic-ext-23.6.0/tests/extra/test_validation_dataclass.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extra/test_validation_multiple.py` & `sanic-ext-23.6.0/tests/extra/test_validation_multiple.py`

 * *Files identical despite different names*

### Comparing `sanic-ext-23.3.0/tests/extra/test_validation_pydantic.py` & `sanic-ext-23.6.0/tests/extra/test_validation_pydantic.py`

 * *Files identical despite different names*

