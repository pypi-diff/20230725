# Comparing `tmp/sparglim-0.1.0rc0.tar.gz` & `tmp/sparglim-0.1.0rc1.tar.gz`

## Comparing `sparglim-0.1.0rc0.tar` & `sparglim-0.1.0rc1.tar`

### file list

```diff
@@ -1,49 +1,52 @@
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.editorconfig
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/RELEASE.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/docs/Makefile
--rwxr-xr-x   0        0        0     4786 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/docs/conf.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/docs/index.rst
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/docs/make.bat
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/docs/usage.rst
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/Dockerfile.lab
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/dev/Dockerfile.lab
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/dev/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/dev/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/dev/k8s/lab-service.yaml
--rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/dev/k8s/reload.sh
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/example/k8s/lab-service.yaml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/exceptions.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/py.typed
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/utils.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/config/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/config/builder.py
--rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/config/configer.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/config/k8s.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/server/__init__.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/server/cli.py
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/server/daemon.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/server/tailer.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/sql/__init__.py
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/sparglim/sql/magic.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/conftest.py
--rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/test_builder.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/test_daemon.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/test_magic.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/example/people.json
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/mock/sbin/entrypoint.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/mock/sbin/mock_spark_server.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/tests/mock/sbin/start-connect-server.sh
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/LICENSE
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/README.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 sparglim-0.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/.editorconfig
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/RELEASE.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/dev/Dockerfile.lab
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/dev/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/dev/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/dev/k8s/lab-service.yaml
+-rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/dev/k8s/reload.sh
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/docker/Dockerfile.lab
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/docker/Dockerfile.sparglim-server
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/docs/Makefile
+-rwxr-xr-x   0        0        0     4786 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/docs/conf.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/docs/index.rst
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/docs/make.bat
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/docs/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/example/pyspark-app/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/example/pyspark-app/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/example/pyspark-app/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/example/pyspark-app/k8s/lab-service.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/example/sparglim-server/README.md
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/exceptions.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/py.typed
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/utils.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/config/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/config/builder.py
+-rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/config/configer.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/config/k8s.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/server/__init__.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/server/cli.py
+-rw-r--r--   0        0        0     8553 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/server/daemon.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/server/tailer.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/sql/__init__.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/sparglim/sql/magic.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/tests/conftest.py
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/tests/test_builder.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/tests/test_daemon.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/tests/test_magic.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/tests/example/people.json
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/tests/mock/sbin/entrypoint.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/tests/mock/sbin/mock_spark_server.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/tests/mock/sbin/start-connect-server.sh
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/README.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 sparglim-0.1.0rc1/PKG-INFO
```

### Comparing `sparglim-0.1.0rc0/.pre-commit-config.yaml` & `sparglim-0.1.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/RELEASE.md` & `sparglim-0.1.0rc1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/.github/workflows/python-package.yml` & `sparglim-0.1.0rc1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/.github/workflows/python-publish.yml` & `sparglim-0.1.0rc1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/docs/Makefile` & `sparglim-0.1.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/docs/conf.py` & `sparglim-0.1.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/docs/make.bat` & `sparglim-0.1.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/example/dev/Dockerfile.lab` & `sparglim-0.1.0rc1/dev/Dockerfile.lab`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 
 COPY --chown=application:application ./ ./sparglim
 RUN pip install --no-cache-dir ./sparglim[all]
 
 ENTRYPOINT ["tini","--","jupyter-lab", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--IdentityProvider.token=''"]
 EXPOSE 8888
 
-# docker build -t wh1isper/sparglim-lab:dev -f example/dev/Dockerfile.lab . && ./example/dev/k8s/reload.sh
+# docker build -t wh1isper/sparglim-lab:dev -f dev/Dockerfile.lab . && ./example/dev/k8s/reload.sh
```

### Comparing `sparglim-0.1.0rc0/example/dev/k8s/deployment.yaml` & `sparglim-0.1.0rc1/dev/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/example/k8s/deployment.yaml` & `sparglim-0.1.0rc1/example/pyspark-app/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/sparglim/utils.py` & `sparglim-0.1.0rc1/sparglim/utils.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/sparglim/config/builder.py` & `sparglim-0.1.0rc1/sparglim/config/builder.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/sparglim/config/configer.py` & `sparglim-0.1.0rc1/sparglim/config/configer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/sparglim/config/k8s.py` & `sparglim-0.1.0rc1/sparglim/config/k8s.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/sparglim/server/cli.py` & `sparglim-0.1.0rc1/sparglim/server/cli.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/sparglim/server/daemon.py` & `sparglim-0.1.0rc1/sparglim/server/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from datetime import datetime
 from functools import wraps
 from pathlib import Path
 from typing import List, Optional
 
 import psutil
 
-from sparglim.config import SparkEnvConfiger
+from sparglim.config.configer import SparkEnvConfiger
 from sparglim.exceptions import DaemonError, UnconfigurableError
 from sparglim.log import logger
 from sparglim.server.tailer import Tailer
 from sparglim.utils import get_scala_version, get_spark_version, port_is_used
 
 
 class Daemon:
```

### Comparing `sparglim-0.1.0rc0/sparglim/server/tailer.py` & `sparglim-0.1.0rc1/sparglim/server/tailer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/sparglim/sql/magic.py` & `sparglim-0.1.0rc1/sparglim/sql/magic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #  Copyright (c) 2023 Wh1isper
 #  Licensed under the BSD 3-Clause
 import os
-from typing import List, Literal, Optional, Union
+from typing import List, Optional
 
 from IPython.core.magic import Magics, cell_magic, line_magic, magics_class
 from pyspark.sql import SparkSession
 
-from sparglim.config import ConfigBuilder
+from sparglim.config.builder import ConfigBuilder
 from sparglim.exceptions import UnconfigurableError
 from sparglim.log import logger
 
 
 @magics_class
 class SparkMagic(Magics):
     """
```

### Comparing `sparglim-0.1.0rc0/tests/conftest.py` & `sparglim-0.1.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/tests/test_builder.py` & `sparglim-0.1.0rc1/tests/test_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from datetime import date, datetime
 from typing import Dict
 
 import pytest
 from pyspark.sql import Row
 
-from sparglim.config import ConfigBuilder
+from sparglim.config.builder import ConfigBuilder
 from sparglim.exceptions import UnconfigurableError
 
 
 @pytest.fixture
 def config_builder():
     c = ConfigBuilder()
     yield c
```

### Comparing `sparglim-0.1.0rc0/tests/test_daemon.py` & `sparglim-0.1.0rc1/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/tests/test_magic.py` & `sparglim-0.1.0rc1/tests/test_magic.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/tests/mock/sbin/entrypoint.py` & `sparglim-0.1.0rc1/tests/mock/sbin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/tests/mock/sbin/mock_spark_server.py` & `sparglim-0.1.0rc1/tests/mock/sbin/mock_spark_server.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/.gitignore` & `sparglim-0.1.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/LICENSE` & `sparglim-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/README.md` & `sparglim-0.1.0rc1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ![](https://img.shields.io/github/license/wh1isper/sparglim)
-![](https://img.shields.io/github/v/release/wh1isper/sparglim)
+![](https://img.shields.io/github/v/release/wh1isper/sparglim?logo=github)
+![](https://img.shields.io/github/v/release/wh1isper/sparglim?include_prereleases&label=pre-release&logo=github)
 ![](https://img.shields.io/pypi/dm/sparglim)
 ![](https://img.shields.io/github/last-commit/wh1isper/sparglim)
 ![](https://img.shields.io/pypi/pyversions/sparglim)
 
 # Sparglim
 
 Sparglim is aimed at providing a clean solution for PySpark applications in cloud-native scenarios (On K8S、Connect Server etc.).
```

### Comparing `sparglim-0.1.0rc0/pyproject.toml` & `sparglim-0.1.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc0/PKG-INFO` & `sparglim-0.1.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparglim
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: sparglim
 Project-URL: Source, https://github.com/wh1isper/sparglim
 Author-email: wh1isper <9573586@qq.com>
 License: BSD license
 License-File: LICENSE
 Keywords: sparglim
 Classifier: Programming Language :: Python :: 3
@@ -36,15 +36,16 @@
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-timeout; extra == 'test'
 Requires-Dist: pytype; extra == 'test'
 Requires-Dist: sparglim[all]; extra == 'test'
 Description-Content-Type: text/markdown
 
 ![](https://img.shields.io/github/license/wh1isper/sparglim)
-![](https://img.shields.io/github/v/release/wh1isper/sparglim)
+![](https://img.shields.io/github/v/release/wh1isper/sparglim?logo=github)
+![](https://img.shields.io/github/v/release/wh1isper/sparglim?include_prereleases&label=pre-release&logo=github)
 ![](https://img.shields.io/pypi/dm/sparglim)
 ![](https://img.shields.io/github/last-commit/wh1isper/sparglim)
 ![](https://img.shields.io/pypi/pyversions/sparglim)
 
 # Sparglim
 
 Sparglim is aimed at providing a clean solution for PySpark applications in cloud-native scenarios (On K8S、Connect Server etc.).
```

