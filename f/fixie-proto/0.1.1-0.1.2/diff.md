# Comparing `tmp/fixie-proto-0.1.1.tar.gz` & `tmp/fixie_proto-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixie-proto-0.1.1.tar", max compression
+gzip compressed data, was "fixie_proto-0.1.2.tar", max compression
```

## Comparing `fixie-proto-0.1.1.tar` & `fixie_proto-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,8 @@
--rw-r--r--   0        0        0     2460 2023-07-20 16:55:13.038944 fixie-proto-0.1.1/README.md
--rw-r--r--   0        0        0      333 2023-07-20 17:56:29.824895 fixie-proto-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3093 1970-01-01 00:00:00.000000 fixie-proto-0.1.1/setup.py
--rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 fixie-proto-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3428 2023-07-25 02:05:06.891240 fixie_proto-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 02:05:39.182147 fixie_proto-0.1.2/gen/python/fixie/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 02:05:39.186147 fixie_proto-0.1.2/gen/python/fixie/corpora/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 02:05:39.186147 fixie_proto-0.1.2/gen/python/fixie/corpora/v1/__init__.py
+-rw-r--r--   0        0        0     1838 2023-07-25 02:05:39.170146 fixie_proto-0.1.2/gen/python/fixie/corpora/v1/common_pb2.py
+-rw-r--r--   0        0        0     3595 2023-07-25 02:05:39.170146 fixie_proto-0.1.2/gen/python/fixie/corpora/v1/loader_pb2.py
+-rw-r--r--   0        0        0      425 2023-07-25 02:05:06.891240 fixie_proto-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4101 1970-01-01 00:00:00.000000 fixie_proto-0.1.2/PKG-INFO
```

### Comparing `fixie-proto-0.1.1/README.md` & `fixie_proto-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,70 @@
 # fixie-proto
 This repository contains protocol buffer definitions for working with the Fixie platform. The intention is for this to define our public-facing APIs. Tooling in this repository should then make it easy to use the *already compiled* protos in various languages.
 
-## Buf Schema Registry (BSR)
+## Usage
+
+### Buf Schema Registry (BSR)
 
 For languages supported by the Buf Schema Registry, instructions for adding these protos like a normal dependency can be found [here](https://buf.build/fixie-ai/fixie/assets/main).  For example, to add a TypeScript dependency using yarn:
 
 ```
 yarn config set npmScopes.buf.npmRegistryServer https://buf.build/gen/npm/v1/
 yarn add @buf/fixie-ai_fixie.bufbuild_connect-es@latest
 ```
 
 As of July 2023, BSR has support for JavaScript/Typscript, Go, JVM-based languages like Java and Kotlin, and Swift.
 
-## Directly supported languages
+### Directly supported languages
 
 We also support additional languages (albeit with fewer options) directly. In particular, Python is available via pip: [PyPI](https://pypi.org/project/fixie-proto/).
 
 ```
 pip install fixie-proto
 ```
 
-## Including Fixie protos in a proto library
+### Inclusion in a proto library
 
 The easiest way to depend on Fixie protos for your own proto library is by building with [Buf](https://buf.build/docs/introduction/) and adding `buf.build/fixie-ai/fixie` as a dependency in your buf.yaml.
 
 If you're using protoc instead, consider including this repository as a submodule in your own repository.
 
 
-## Other languages
+### Other languages
 
 Buf can be used to easily compile our protos in other languages too, including: Ruby, Objective-C, PHP, C#, Scala, C++, Dart, and Rust.  You'll need to create a [buf.gen.yaml file](https://buf.build/docs/generate/overview/) that uses the relevant protoc plugin for your language. You can also define language-specific proto options without modifying the proto files themselves using [managed mode](https://buf.build/docs/generate/managed-mode/#managed). You can then compile the protos in your language of choice by running:
 
 ```
 buf generate --template buf.gen.yaml buf.build/fixie-ai/fixie
 ```
 
 If you'd prefer to use protoc, see the advice above about including Fixie protos in your own proto library.
 
 ## Using JSON instead
 
 If you'd prefer not to deal with protos, we've got you covered! All of our APIs can accept and return JSON instead. Just set your Content-Type header to `application/json` instead of `application/proto`.
 
+Our OpenAPI spec matches the proto API. You can view it [here](https://petstore.swagger.io/?url=https://gist.githubusercontent.com/mdepinet/1382c315186d178f587f3d9ca382b74e/raw/be61192d0fe190e646cc52a494017ba7dbe3a33b/loader.swagger.json).
+
 <!-- TODO(mdepinet): Figure out how/where to publish the generated OpenAPI and then link to that here. -->
 
+
+## Contributing
+
+### Tools
+
+To work in this repository, you'll need to install Buf and Just. If you are using homebrew:
+
+```
+brew install bufbuild/buf/buf
+brew install just
+```
+
+Otherwise see [the Buf docs](https://buf.build/docs/installation/) and [the Just docs](https://just.systems/man/en/chapter_4.html) for other installation options.
+
+### Presubmit
+
+Please run "just" before sending PRs. This will format and lint your proto files in addition to identifying breaking changes. (These will also be run for you any time a PR is created.)
+
+### Releases
+
+New versions are pushed to BSR whenever a PR is merged into main. These events will also cause a push to PyPI as long as the version in pyproject.toml was incremented.
```

### Comparing `fixie-proto-0.1.1/setup.py` & `fixie_proto-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,90 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fixie-proto
+Version: 0.1.2
+Summary: 
+Author: Fixie.ai Team
+Author-email: founders@fixie.ai
+Requires-Python: >=3,<4
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: protobuf (>=4.21.1,<5)
+Description-Content-Type: text/markdown
 
-packages = \
-['python']
+# fixie-proto
+This repository contains protocol buffer definitions for working with the Fixie platform. The intention is for this to define our public-facing APIs. Tooling in this repository should then make it easy to use the *already compiled* protos in various languages.
 
-package_data = \
-{'': ['*']}
+## Usage
 
-install_requires = \
-['protobuf>=4.21.1,<5']
-
-setup_kwargs = {
-    'name': 'fixie-proto',
-    'version': '0.1.1',
-    'description': '',
-    'long_description': "# fixie-proto\nThis repository contains protocol buffer definitions for working with the Fixie platform. The intention is for this to define our public-facing APIs. Tooling in this repository should then make it easy to use the *already compiled* protos in various languages.\n\n## Buf Schema Registry (BSR)\n\nFor languages supported by the Buf Schema Registry, instructions for adding these protos like a normal dependency can be found [here](https://buf.build/fixie-ai/fixie/assets/main).  For example, to add a TypeScript dependency using yarn:\n\n```\nyarn config set npmScopes.buf.npmRegistryServer https://buf.build/gen/npm/v1/\nyarn add @buf/fixie-ai_fixie.bufbuild_connect-es@latest\n```\n\nAs of July 2023, BSR has support for JavaScript/Typscript, Go, JVM-based languages like Java and Kotlin, and Swift.\n\n## Directly supported languages\n\nWe also support additional languages (albeit with fewer options) directly. In particular, Python is available via pip: [PyPI](https://pypi.org/project/fixie-proto/).\n\n```\npip install fixie-proto\n```\n\n## Including Fixie protos in a proto library\n\nThe easiest way to depend on Fixie protos for your own proto library is by building with [Buf](https://buf.build/docs/introduction/) and adding `buf.build/fixie-ai/fixie` as a dependency in your buf.yaml.\n\nIf you're using protoc instead, consider including this repository as a submodule in your own repository.\n\n\n## Other languages\n\nBuf can be used to easily compile our protos in other languages too, including: Ruby, Objective-C, PHP, C#, Scala, C++, Dart, and Rust.  You'll need to create a [buf.gen.yaml file](https://buf.build/docs/generate/overview/) that uses the relevant protoc plugin for your language. You can also define language-specific proto options without modifying the proto files themselves using [managed mode](https://buf.build/docs/generate/managed-mode/#managed). You can then compile the protos in your language of choice by running:\n\n```\nbuf generate --template buf.gen.yaml buf.build/fixie-ai/fixie\n```\n\nIf you'd prefer to use protoc, see the advice above about including Fixie protos in your own proto library.\n\n## Using JSON instead\n\nIf you'd prefer not to deal with protos, we've got you covered! All of our APIs can accept and return JSON instead. Just set your Content-Type header to `application/json` instead of `application/proto`.\n\n<!-- TODO(mdepinet): Figure out how/where to publish the generated OpenAPI and then link to that here. -->\n\n",
-    'author': 'Fixie.ai Team',
-    'author_email': 'founders@fixie.ai',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+### Buf Schema Registry (BSR)
 
+For languages supported by the Buf Schema Registry, instructions for adding these protos like a normal dependency can be found [here](https://buf.build/fixie-ai/fixie/assets/main).  For example, to add a TypeScript dependency using yarn:
+
+```
+yarn config set npmScopes.buf.npmRegistryServer https://buf.build/gen/npm/v1/
+yarn add @buf/fixie-ai_fixie.bufbuild_connect-es@latest
+```
+
+As of July 2023, BSR has support for JavaScript/Typscript, Go, JVM-based languages like Java and Kotlin, and Swift.
+
+### Directly supported languages
+
+We also support additional languages (albeit with fewer options) directly. In particular, Python is available via pip: [PyPI](https://pypi.org/project/fixie-proto/).
+
+```
+pip install fixie-proto
+```
+
+### Inclusion in a proto library
+
+The easiest way to depend on Fixie protos for your own proto library is by building with [Buf](https://buf.build/docs/introduction/) and adding `buf.build/fixie-ai/fixie` as a dependency in your buf.yaml.
+
+If you're using protoc instead, consider including this repository as a submodule in your own repository.
+
+
+### Other languages
+
+Buf can be used to easily compile our protos in other languages too, including: Ruby, Objective-C, PHP, C#, Scala, C++, Dart, and Rust.  You'll need to create a [buf.gen.yaml file](https://buf.build/docs/generate/overview/) that uses the relevant protoc plugin for your language. You can also define language-specific proto options without modifying the proto files themselves using [managed mode](https://buf.build/docs/generate/managed-mode/#managed). You can then compile the protos in your language of choice by running:
+
+```
+buf generate --template buf.gen.yaml buf.build/fixie-ai/fixie
+```
+
+If you'd prefer to use protoc, see the advice above about including Fixie protos in your own proto library.
+
+## Using JSON instead
+
+If you'd prefer not to deal with protos, we've got you covered! All of our APIs can accept and return JSON instead. Just set your Content-Type header to `application/json` instead of `application/proto`.
+
+Our OpenAPI spec matches the proto API. You can view it [here](https://petstore.swagger.io/?url=https://gist.githubusercontent.com/mdepinet/1382c315186d178f587f3d9ca382b74e/raw/be61192d0fe190e646cc52a494017ba7dbe3a33b/loader.swagger.json).
+
+<!-- TODO(mdepinet): Figure out how/where to publish the generated OpenAPI and then link to that here. -->
+
+
+## Contributing
+
+### Tools
+
+To work in this repository, you'll need to install Buf and Just. If you are using homebrew:
+
+```
+brew install bufbuild/buf/buf
+brew install just
+```
+
+Otherwise see [the Buf docs](https://buf.build/docs/installation/) and [the Just docs](https://just.systems/man/en/chapter_4.html) for other installation options.
+
+### Presubmit
+
+Please run "just" before sending PRs. This will format and lint your proto files in addition to identifying breaking changes. (These will also be run for you any time a PR is created.)
+
+### Releases
+
+New versions are pushed to BSR whenever a PR is merged into main. These events will also cause a push to PyPI as long as the version in pyproject.toml was incremented.
 
-setup(**setup_kwargs)
```

