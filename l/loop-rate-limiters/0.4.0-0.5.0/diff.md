# Comparing `tmp/loop-rate-limiters-0.4.0.tar.gz` & `tmp/loop-rate-limiters-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loop-rate-limiters-0.4.0.tar", last modified: Thu Apr 13 18:18:58 2023, max compression
+gzip compressed data, was "loop-rate-limiters-0.5.0.tar", last modified: Tue Jul 25 12:30:59 2023, max compression
```

## Comparing `loop-rate-limiters-0.4.0.tar` & `loop-rate-limiters-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     2662 2023-01-20 14:30:45.658299 loop-rate-limiters-0.4.0/.github/workflows/main.yml
--rw-r--r--   0        0        0       39 2023-01-17 15:33:40.872366 loop-rate-limiters-0.4.0/.gitignore
--rw-r--r--   0        0        0      586 2023-04-13 18:18:15.934034 loop-rate-limiters-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-01-17 15:33:40.872366 loop-rate-limiters-0.4.0/LICENSE
--rw-r--r--   0        0        0     1702 2023-01-20 14:30:45.658299 loop-rate-limiters-0.4.0/README.md
--rw-r--r--   0        0        0      824 2023-04-13 18:14:28.520187 loop-rate-limiters-0.4.0/loop_rate_limiters/__init__.py
--rw-r--r--   0        0        0     4732 2023-04-13 18:13:51.023598 loop-rate-limiters-0.4.0/loop_rate_limiters/async_rate_limiter.py
--rw-r--r--   0        0        0     3017 2023-04-13 18:14:19.952092 loop-rate-limiters-0.4.0/loop_rate_limiters/rate_limiter.py
--rw-r--r--   0        0        0     1491 2023-01-20 14:30:45.658299 loop-rate-limiters-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      699 2023-01-17 15:33:40.876365 loop-rate-limiters-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     2096 2023-01-17 15:33:40.876365 loop-rate-limiters-0.4.0/tests/test_async_rate.py
--rw-r--r--   0        0        0     1902 2023-01-20 14:30:45.658299 loop-rate-limiters-0.4.0/tests/test_rate_limiter.py
--rw-r--r--   0        0        0      632 2023-01-20 14:30:45.662299 loop-rate-limiters-0.4.0/tox.ini
--rw-r--r--   0        0        0     2797 1970-01-01 00:00:00.000000 loop-rate-limiters-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      718 2023-07-25 12:28:10.832468 loop-rate-limiters-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2022-12-02 14:27:49.222419 loop-rate-limiters-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1936 2023-07-22 13:48:54.222531 loop-rate-limiters-0.5.0/README.md
+-rw-r--r--   0        0        0      824 2023-07-25 12:28:19.048731 loop-rate-limiters-0.5.0/loop_rate_limiters/__init__.py
+-rw-r--r--   0        0        0     5039 2023-07-23 13:54:53.476919 loop-rate-limiters-0.5.0/loop_rate_limiters/async_rate_limiter.py
+-rw-r--r--   0        0        0     3432 2023-07-23 13:55:37.312390 loop-rate-limiters-0.5.0/loop_rate_limiters/rate_limiter.py
+-rw-r--r--   0        0        0     1687 2023-07-25 12:30:47.761115 loop-rate-limiters-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      699 2022-12-02 14:47:28.358593 loop-rate-limiters-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     2096 2022-12-16 09:45:38.300362 loop-rate-limiters-0.5.0/tests/test_async_rate.py
+-rw-r--r--   0        0        0     2078 2023-07-22 13:48:54.258530 loop-rate-limiters-0.5.0/tests/test_rate_limiter.py
+-rw-r--r--   0        0        0      632 2023-01-19 19:48:53.196347 loop-rate-limiters-0.5.0/tox.ini
+-rw-r--r--   0        0        0      488 1970-01-01 00:00:00.000000 loop-rate-limiters-0.5.0/setup.py
+-rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 loop-rate-limiters-0.5.0/PKG-INFO
```

### Comparing `loop-rate-limiters-0.4.0/CHANGELOG.md` & `loop-rate-limiters-0.5.0/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.5.0] - 2023/07/25
+
+### Added
+
+- AsyncRateLimiter: ``warn`` constructor argument
+- RateLimiter: ``warn`` constructor argument
+
 ## [0.4.0] - 2023/04/13
 
 ### Added
 
 - RateLimiter: warn when the limiter is running late
 
 ## [0.3.0] - 2023/01/20
```

### Comparing `loop-rate-limiters-0.4.0/LICENSE` & `loop-rate-limiters-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.4.0/README.md` & `loop-rate-limiters-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 # Loop rate limiters
 
-[![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/loop-rate-limiters/main.yml?branch=main)](https://github.com/stephane-caron/loop-rate-limiters/actions)
-[![Coverage](https://coveralls.io/repos/github/stephane-caron/loop-rate-limiters/badge.svg?branch=main)](https://coveralls.io/github/stephane-caron/loop-rate-limiters?branch=main)
-[![Conda version](https://img.shields.io/conda/vn/conda-forge/loop-rate-limiters.svg)](https://anaconda.org/conda-forge/loop-rate-limiters)
-[![PyPI version](https://img.shields.io/pypi/v/loop-rate-limiters)](https://pypi.org/project/loop-rate-limiters/)
-
-Simple loop frequency regulators in Python with an API similar to [``rospy.Rate``](https://wiki.ros.org/rospy/Overview/Time#Sleeping_and_Rates).
-
-## Installation
-
-From conda-forge:
-
-```sh
-conda install loop-rate-limiters -c conda-forge
-```
-
-From PyPI:
-
-```sh
-pip install loop-rate-limiters
-```
-
-## Usage
+[![Build](https://img.shields.io/github/actions/workflow/status/tasts-robots/loop-rate-limiters/main.yml?branch=main)](https://github.com/tasts-robots/loop-rate-limiters/actions)
+[![Coverage](https://coveralls.io/repos/github/tasts-robots/loop-rate-limiters/badge.svg?branch=main)](https://coveralls.io/github/tasts-robots/loop-rate-limiters?branch=main)
 
-The ``RateLimiter`` class provides a loop frequency limiter:
+Simple loop frequency regulators in Python with an API similar to ``rospy.Rate``:
 
 ```python
 from loop_rate_limiters import RateLimiter
 from time import perf_counter
 
 rate = RateLimiter(frequency=400.0)
 while True:
     print(f"Hello from loop at {perf_counter():.3f} s")
     rate.sleep()
 ```
 
-### asyncio
+A similar ``AsyncRateLimiter`` class is available for [asynchronous code](#asynchronous-io).
+
+## Installation
+
+### PyPI
+
+[![PyPI version](https://img.shields.io/pypi/v/loop-rate-limiters)](https://pypi.org/project/loop-rate-limiters/)
+[![PyPI downloads](https://static.pepy.tech/badge/loop-rate-limiters)](https://pepy.tech/project/loop-rate-limiters)
+
+```console
+$ pip install loop-rate-limiters
+```
+
+### Conda
+
+[![Conda version](https://anaconda.org/conda-forge/loop-rate-limiters/badges/version.svg)](https://anaconda.org/conda-forge/loop-rate-limiters)
+[![Conda downloads](https://anaconda.org/conda-forge/loop-rate-limiters/badges/downloads.svg)](https://anaconda.org/conda-forge/loop-rate-limiters)
+
+```console
+$ conda install loop-rate-limiters -c conda-forge
+```
+
+## Asynchronous I/O
 
 The ``AsyncRateLimiter`` class provides a loop frequency limiter for [asyncio](https://docs.python.org/3/library/asyncio.html):
 
 ```python
 import asyncio
 from loop_rate_limiters import AsyncRateLimiter
```

### Comparing `loop-rate-limiters-0.4.0/loop_rate_limiters/__init__.py` & `loop-rate-limiters-0.5.0/loop_rate_limiters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Loop rate limiters."""
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 from .async_rate_limiter import AsyncRateLimiter
 from .rate_limiter import RateLimiter
 
 __all__ = [
     "AsyncRateLimiter",
     "RateLimiter",
```

### Comparing `loop-rate-limiters-0.4.0/loop_rate_limiters/async_rate_limiter.py` & `loop-rate-limiters-0.5.0/loop_rate_limiters/async_rate_limiter.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,41 +49,49 @@
     Attributes:
         measured_period: Actual period in seconds measured at the end of the
             last call to :func:`sleep`.
         name: Human-readable name used for logging.
         period: Desired loop period in seconds.
         slack: Duration in seconds remaining until the next tick at the
             beginning of the last call to :func:`sleep`.
+        warn: If set (default), warn when the time between two calls
+            exceeded the rate clock.
     """
 
     _last_loop_time: float
     _loop: asyncio.AbstractEventLoop
     _next_tick: float
     measured_period: float
     name: str
     period: float
     slack: float
+    warn: bool
 
-    def __init__(self, frequency: float, name: str = "rate limiter"):
+    def __init__(
+        self, frequency: float, name: str = "rate limiter", warn: bool = True
+    ):
         """Initialize rate limiter.
 
         Args:
             frequency: Desired loop frequency in hertz.
             name: Human-readable name used for logging.
+            warn: If set (default), warn when the time between two calls
+                exceeded the rate clock.
         """
         loop = asyncio.get_event_loop()
         period = 1.0 / frequency
         assert loop.is_running()
         self._last_loop_time = loop.time()
         self._loop = loop
         self._next_tick = loop.time() + period
         self.measured_period = 0.0
         self.name = name
         self.period = period
         self.slack = 0.0
+        self.warn = warn
 
     async def remaining(self) -> float:
         """Get the time remaining until the next expected clock tick.
 
         Returns:
             Time remaining, in seconds, until the next expected clock tick.
         """
@@ -110,15 +118,15 @@
         """
         self.slack = self._next_tick - self._loop.time()
         if self.slack > 0.0:
             block_time = self._next_tick - block_duration
             while self._loop.time() < self._next_tick:
                 if self._loop.time() < block_time:
                     await asyncio.sleep(1e-5)  # non-zero sleep duration
-        elif self.slack < -0.1 * self.period:
+        elif self.slack < -0.1 * self.period and self.warn:
             logging.warning(
                 "%s is late by %f [ms]", self.name, round(1e3 * self.slack, 1)
             )
         loop_time = self._loop.time()
         self.measured_period = loop_time - self._last_loop_time
         self._last_loop_time = loop_time
         self._next_tick = loop_time + self.period
```

### Comparing `loop-rate-limiters-0.4.0/loop_rate_limiters/rate_limiter.py` & `loop-rate-limiters-0.5.0/loop_rate_limiters/rate_limiter.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,31 +28,46 @@
     This rate limniter is meant to be used in e.g. a loop or callback function.
     It is, in essence, the same as rospy.Rate_. It assumes Python's performance
     counter never jumps backward nor forward, so that it does not handle such
     cases contrary to rospy.Rate_.
 
     .. _rospy.Rate:
         https://github.com/ros/ros_comm/blob/noetic-devel/clients/rospy/src/rospy/timer.py
+
+    Attributes:
+        name: Human-readable name used for logging.
+        warn: If set (default), warn when the time between two calls
+            exceeded the rate clock.
     """
 
     __period: float
     __slack: float
     __next_tick: float
+    name: str
+    warn: bool
 
-    def __init__(self, frequency: float, name: str = "rate limiter"):
+    def __init__(
+        self,
+        frequency: float,
+        name: str = "rate limiter",
+        warn: bool = True,
+    ):
         """Initialize rate limiter.
 
         Args:
             frequency: Desired frequency in hertz.
             name: Human-readable name used for logging.
+            warn: If set (default), warn when the time between two calls
+                exceeded the rate clock.
         """
         period = 1.0 / frequency
         self.__next_tick = perf_counter() + period
         self.__period = period
         self.name = name
+        self.warn = warn
 
     @property
     def dt(self) -> float:
         """Desired period between two calls to :func:`sleep`, in seconds."""
         return self.__period
 
     @property
@@ -82,14 +97,14 @@
         return self.__next_tick - perf_counter()
 
     def sleep(self):
         """Sleep for the duration required to regulate inter-call frequency."""
         self.__slack = self.__next_tick - perf_counter()
         if self.__slack > 0.0:
             sleep(self.__slack)
-        elif self.__slack < -0.1 * self.period:
+        elif self.__slack < -0.1 * self.period and self.warn:
             logging.warning(
                 "%s is late by %f [ms]",
                 self.name,
                 round(1e3 * self.__slack, 1),
             )
         self.__next_tick = perf_counter() + self.__period
```

### Comparing `loop-rate-limiters-0.4.0/pyproject.toml` & `loop-rate-limiters-0.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -26,33 +26,43 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 dependencies = []
 keywords = ["rate", "loop", "frequency", "regulator", "limiter"]
 
 [project.urls]
-Source = "https://github.com/stephane-caron/loop-rate-limiters"
-Tracker = "https://github.com/stephane-caron/loop-rate-limiters/issues"
-Changelog = "https://github.com/stephane-caron/loop-rate-limiters/blob/master/CHANGELOG.md"
+Source = "https://github.com/tasts-robots/loop-rate-limiters"
+Tracker = "https://github.com/tasts-robots/loop-rate-limiters/issues"
+Changelog = "https://github.com/tasts-robots/loop-rate-limiters/blob/master/CHANGELOG.md"
 
 [tool.black]
 line-length = 79
 
 [tool.flit.module]
 name = "loop_rate_limiters"
 
+[tool.flit.sdist]
+exclude = [
+    ".github",
+    ".gitignore",
+]
+
 [tool.ruff]
 line-length = 79
 select = [
     # pyflakes
     "F",
     # pycodestyle
     "E",
     "W",
     # isort
     "I001",
     # pydocstyle
     "D"
 ]
+ignore = [
+    "D401",  # good for methods but not for class docstrings
+    "D405",  # British-style section names are also "proper"!
+]
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `loop-rate-limiters-0.4.0/tests/__init__.py` & `loop-rate-limiters-0.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.4.0/tests/test_async_rate.py` & `loop-rate-limiters-0.5.0/tests/test_async_rate.py`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.4.0/tests/test_rate_limiter.py` & `loop-rate-limiters-0.5.0/tests/test_rate_limiter.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,19 @@
         """Initialize a rate with 1 ms period."""
         self.rate = RateLimiter(frequency=1000.0)
 
     def test_init(self):
         """Constructor completed."""
         self.assertIsNotNone(self.rate)
 
+    def test_next_tick(self):
+        call_tick = time.perf_counter()
+        self.rate.sleep()
+        self.assertGreaterEqual(self.rate.next_tick, call_tick + self.rate.dt)
+
     def test_period_dt(self):
         """Check that period and dt are the same."""
         self.assertAlmostEqual(self.rate.period, self.rate.dt)
 
     def test_remaining(self):
         """
         After one period has expired, the "remaining" time becomes negative.
```

### Comparing `loop-rate-limiters-0.4.0/tox.ini` & `loop-rate-limiters-0.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `loop-rate-limiters-0.4.0/PKG-INFO` & `loop-rate-limiters-0.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loop-rate-limiters
-Version: 0.4.0
+Version: 0.5.0
 Summary: Loop rate limiters.
 Keywords: rate,loop,frequency,regulator,limiter
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -13,56 +13,58 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Project-URL: Changelog, https://github.com/stephane-caron/loop-rate-limiters/blob/master/CHANGELOG.md
-Project-URL: Source, https://github.com/stephane-caron/loop-rate-limiters
-Project-URL: Tracker, https://github.com/stephane-caron/loop-rate-limiters/issues
+Project-URL: Changelog, https://github.com/tasts-robots/loop-rate-limiters/blob/master/CHANGELOG.md
+Project-URL: Source, https://github.com/tasts-robots/loop-rate-limiters
+Project-URL: Tracker, https://github.com/tasts-robots/loop-rate-limiters/issues
 
 # Loop rate limiters
 
-[![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/loop-rate-limiters/main.yml?branch=main)](https://github.com/stephane-caron/loop-rate-limiters/actions)
-[![Coverage](https://coveralls.io/repos/github/stephane-caron/loop-rate-limiters/badge.svg?branch=main)](https://coveralls.io/github/stephane-caron/loop-rate-limiters?branch=main)
-[![Conda version](https://img.shields.io/conda/vn/conda-forge/loop-rate-limiters.svg)](https://anaconda.org/conda-forge/loop-rate-limiters)
-[![PyPI version](https://img.shields.io/pypi/v/loop-rate-limiters)](https://pypi.org/project/loop-rate-limiters/)
-
-Simple loop frequency regulators in Python with an API similar to [``rospy.Rate``](https://wiki.ros.org/rospy/Overview/Time#Sleeping_and_Rates).
-
-## Installation
-
-From conda-forge:
-
-```sh
-conda install loop-rate-limiters -c conda-forge
-```
-
-From PyPI:
-
-```sh
-pip install loop-rate-limiters
-```
-
-## Usage
+[![Build](https://img.shields.io/github/actions/workflow/status/tasts-robots/loop-rate-limiters/main.yml?branch=main)](https://github.com/tasts-robots/loop-rate-limiters/actions)
+[![Coverage](https://coveralls.io/repos/github/tasts-robots/loop-rate-limiters/badge.svg?branch=main)](https://coveralls.io/github/tasts-robots/loop-rate-limiters?branch=main)
 
-The ``RateLimiter`` class provides a loop frequency limiter:
+Simple loop frequency regulators in Python with an API similar to ``rospy.Rate``:
 
 ```python
 from loop_rate_limiters import RateLimiter
 from time import perf_counter
 
 rate = RateLimiter(frequency=400.0)
 while True:
     print(f"Hello from loop at {perf_counter():.3f} s")
     rate.sleep()
 ```
 
-### asyncio
+A similar ``AsyncRateLimiter`` class is available for [asynchronous code](#asynchronous-io).
+
+## Installation
+
+### PyPI
+
+[![PyPI version](https://img.shields.io/pypi/v/loop-rate-limiters)](https://pypi.org/project/loop-rate-limiters/)
+[![PyPI downloads](https://static.pepy.tech/badge/loop-rate-limiters)](https://pepy.tech/project/loop-rate-limiters)
+
+```console
+$ pip install loop-rate-limiters
+```
+
+### Conda
+
+[![Conda version](https://anaconda.org/conda-forge/loop-rate-limiters/badges/version.svg)](https://anaconda.org/conda-forge/loop-rate-limiters)
+[![Conda downloads](https://anaconda.org/conda-forge/loop-rate-limiters/badges/downloads.svg)](https://anaconda.org/conda-forge/loop-rate-limiters)
+
+```console
+$ conda install loop-rate-limiters -c conda-forge
+```
+
+## Asynchronous I/O
 
 The ``AsyncRateLimiter`` class provides a loop frequency limiter for [asyncio](https://docs.python.org/3/library/asyncio.html):
 
 ```python
 import asyncio
 from loop_rate_limiters import AsyncRateLimiter
```

