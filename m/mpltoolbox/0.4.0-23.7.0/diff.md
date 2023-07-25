# Comparing `tmp/mpltoolbox-0.4.0.tar.gz` & `tmp/mpltoolbox-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpltoolbox-0.4.0.tar", last modified: Tue Jan 10 12:24:09 2023, max compression
+gzip compressed data, was "mpltoolbox-23.7.0.tar", last modified: Tue Jul 25 13:10:45 2023, max compression
```

## Comparing `mpltoolbox-0.4.0.tar` & `mpltoolbox-23.7.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:24:09.245634 mpltoolbox-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:24:09.237634 mpltoolbox-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:24:09.241634 mpltoolbox-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-01-10 12:24:09.245634 mpltoolbox-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:24:09.241634 mpltoolbox-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/callbacks.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/ellipses.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:24:09.241634 mpltoolbox-0.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   137750 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    75876 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    95767 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/lines.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/points.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/polygons.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/programmatic-control.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/rectangles.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/docs/spans.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-01-10 12:24:09.245634 mpltoolbox-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:24:09.241634 mpltoolbox-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:24:09.245634 mpltoolbox-0.4.0/src/mpltoolbox/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/ellipses.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/hspans.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/rectangles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-01-10 12:22:19.000000 mpltoolbox-0.4.0/src/mpltoolbox/vspans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:24:09.245634 mpltoolbox-0.4.0/src/mpltoolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-01-10 12:24:09.000000 mpltoolbox-0.4.0/src/mpltoolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-10 12:24:09.000000 mpltoolbox-0.4.0/src/mpltoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 12:24:09.000000 mpltoolbox-0.4.0/src/mpltoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-10 12:24:09.000000 mpltoolbox-0.4.0/src/mpltoolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-10 12:24:09.000000 mpltoolbox-0.4.0/src/mpltoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:10:45.201061 mpltoolbox-23.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:10:45.193061 mpltoolbox-23.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:10:45.197061 mpltoolbox-23.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-25 13:10:45.201061 mpltoolbox-23.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:10:45.197061 mpltoolbox-23.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/callbacks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/ellipses.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:10:45.197061 mpltoolbox-23.7.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   137750 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    75876 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    95767 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/lines.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/points.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/polygons.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/programmatic-control.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/rectangles.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/docs/spans.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 13:10:45.201061 mpltoolbox-23.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:10:45.197061 mpltoolbox-23.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:10:45.201061 mpltoolbox-23.7.0/src/mpltoolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/ellipses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/hspans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/rectangles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-25 13:09:08.000000 mpltoolbox-23.7.0/src/mpltoolbox/vspans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:10:45.201061 mpltoolbox-23.7.0/src/mpltoolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-25 13:10:45.000000 mpltoolbox-23.7.0/src/mpltoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-25 13:10:45.000000 mpltoolbox-23.7.0/src/mpltoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:10:45.000000 mpltoolbox-23.7.0/src/mpltoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 13:10:45.000000 mpltoolbox-23.7.0/src/mpltoolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 13:10:45.000000 mpltoolbox-23.7.0/src/mpltoolbox.egg-info/top_level.txt
```

### Comparing `mpltoolbox-0.4.0/.github/workflows/ci.yml` & `mpltoolbox-23.7.0/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python 3.9
-      uses: actions/setup-python@v2
+    - uses: actions/checkout@v3
+    - name: Set up Python
+      uses: actions/setup-python@v3
       with:
-        python-version: 3.9
+        python-version: '3.10'
     - name: Install dependencies
       run: |
         which python
         python -m pip install --upgrade pip
-        python -m pip install flake8 toml yapf==0.32 build pytest
+        python -m pip install flake8 toml black[jupyter] build pytest
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-    - name: Check yapf formatting
+    - name: Check black formatting
       run: |
-        yapf --diff --recursive .
+        black --check --diff .
     - name: Lint with flake8
       run: |
         flake8 . --count --statistics
     - name: Install docs requirements
       run: |
         pip install -r docs/requirements.txt
         sudo apt install pandoc
@@ -44,20 +44,20 @@
     # - name: Run python tests
     #   run: |
     #     python -m pytest test
     - name: Build documentation
       run: |
         sphinx-build -b html docs/. docs/build
     - name: Archive documentation artifacts
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: DocumentationHTML
         path: docs/build
     - name: Build a binary wheel and a source tarball
       if: startsWith(github.ref, 'refs/tags')
       run: |
         python -m build --sdist --wheel --outdir dist/ .
     - name: Publish to PyPI
       if: startsWith(github.ref, 'refs/tags')
-      uses: pypa/gh-action-pypi-publish@master
+      uses: pypa/gh-action-pypi-publish@v1.8.8
       with:
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `mpltoolbox-0.4.0/LICENSE` & `mpltoolbox-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpltoolbox-0.4.0/PKG-INFO` & `mpltoolbox-23.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltoolbox
-Version: 0.4.0
+Version: 23.7.0
 Summary: Interactive tools for matplotlib
 Home-page: https://github.com/scipp/mpltoolbox
 Author: Neil Vaytet
 Author-email: neil.vaytet@esss.se
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/mpltoolbox/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mpltoolbox-0.4.0/README.md` & `mpltoolbox-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mpltoolbox-0.4.0/docs/callbacks.ipynb` & `mpltoolbox-23.7.0/docs/callbacks.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960299707203277%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(7, '- `on_remove`: called when the shape is deleted "*

 * *            "(middle-click, or Ctrl + left-click)\\n'), (8, '- `on_vertex_press`: called when a "*

 * *            "vertex is clicked (left-click)\\n'), (12, '- `on_drag_move`: called for every "*

 * *            "movement during shape drag (right-click and hold)\\n')], delete: [12, 8, 7]}}, 1: "*

 * *            "{'source': {insert: [(3, '\\n')]}}, 3: {'source': {insert: [(6, 'x, y, z = "*

 * *            'np.meshgrid(xx, yy, zz, inde […]*

```diff
@@ -8,20 +8,20 @@
                 "# Callbacks\n",
                 "\n",
                 "Every tool in the `mpltoolbox` comes with entry points for adding callbacks to different events.\n",
                 "The different events are:\n",
                 "\n",
                 "- `on_create`: called when drawing the shape (rectangle, line or polygon) is complete\n",
                 "- `on_change`: called when the shape has changed in any way (position, size...)\n",
-                "- `on_remove`: called when the shape is deleted (middle click)\n",
-                "- `on_vertex_press`: called when a vertex is clicked (left click)\n",
+                "- `on_remove`: called when the shape is deleted (middle-click, or Ctrl + left-click)\n",
+                "- `on_vertex_press`: called when a vertex is clicked (left-click)\n",
                 "- `on_vertex_move`: called when a vertex is moved\n",
                 "- `on_vertex_release`: called when the mouse button is released after clicking a vertex\n",
                 "- `on_drag_press`: called when the entire shape (rectangle, line, etc..) is right clicked to initiate drag\n",
-                "- `on_drag_move`: called for every movement during shape drag (right click and hold)\n",
+                "- `on_drag_move`: called for every movement during shape drag (right-click and hold)\n",
                 "- `on_drag_release`: called when the shape is released after drag\n",
                 "\n",
                 "Below is a couple of examples on how these callbacks are used."
             ]
         },
         {
             "cell_type": "code",
@@ -29,14 +29,15 @@
             "id": "83db812a-0d64-442c-b1bc-b222aa30292a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "plt.ioff()\n",
                 "import mpltoolbox as tbx"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c8045a0a-1922-4686-9c75-1e1439c408a7",
@@ -56,19 +57,19 @@
             "source": [
                 "N = 200\n",
                 "M = 300\n",
                 "L = 100\n",
                 "xx = np.arange(N, dtype=np.float64)\n",
                 "yy = np.arange(M, dtype=np.float64)\n",
                 "zz = np.arange(L, dtype=np.float64)\n",
-                "x, y, z = np.meshgrid(xx, yy, zz, indexing='ij')\n",
-                "b = N/20.0\n",
-                "c = M/2.0\n",
-                "d = L/2.0\n",
-                "r = np.sqrt(((x-c)/b)**2 + ((y-c)/b)**2 + ((z-d)/b)**2)\n",
+                "x, y, z = np.meshgrid(xx, yy, zz, indexing=\"ij\")\n",
+                "b = N / 20.0\n",
+                "c = M / 2.0\n",
+                "d = L / 2.0\n",
+                "r = np.sqrt(((x - c) / b) ** 2 + ((y - c) / b) ** 2 + ((z - d) / b) ** 2)\n",
                 "a = 10.0 * np.sin(r) + np.random.random([N, M, L])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "610fd362-36bc-4922-8629-2e7978f37aa4",
             "metadata": {},
@@ -83,15 +84,15 @@
             "id": "83d494dc-edf4-4f65-901b-40eeaa0ac0dd",
             "metadata": {},
             "outputs": [],
             "source": [
                 "fig, ax = plt.subplots(2, 1, figsize=(7, 7))\n",
                 "fig.canvas.header_visible = False\n",
                 "fig.tight_layout()\n",
-                "ax[0].imshow(a[..., 0], interpolation='none', origin='lower')"
+                "ax[0].imshow(a[..., 0], interpolation=\"none\", origin=\"lower\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "56f8e75a-1bb5-464b-be67-0aa9df616556",
             "metadata": {},
             "source": [
@@ -105,22 +106,23 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "6071cdd9-2b7c-4e1e-8532-50bcd962a850",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def make_line(new_point):\n",
-                "    l, = ax[1].plot(a[int(new_point.y), int(new_point.x), :])\n",
+                "    (l,) = ax[1].plot(a[int(new_point.y), int(new_point.x), :])\n",
                 "    new_point.associated = l\n",
                 "\n",
+                "\n",
                 "def update_line(new_point):\n",
-                "    new_point.associated.set_ydata(\n",
-                "        a[int(new_point.y), int(new_point.x), :])\n",
+                "    new_point.associated.set_ydata(a[int(new_point.y), int(new_point.x), :])\n",
+                "\n",
                 "\n",
-                "points = tbx.Points(ax=ax[0], mec='white')\n",
+                "points = tbx.Points(ax=ax[0], mec=\"white\")\n",
                 "points.on_create(make_line)\n",
                 "points.on_change(update_line)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -162,31 +164,36 @@
             "id": "37fea063-f036-4d06-a0b6-92d57e8f32d5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "fig2, ax2 = plt.subplots(2, 1, figsize=(7, 7))\n",
                 "fig2.canvas.header_visible = False\n",
                 "fig2.tight_layout()\n",
-                "ax2[0].imshow(a[..., 0], interpolation='none', origin='lower')\n",
+                "ax2[0].imshow(a[..., 0], interpolation=\"none\", origin=\"lower\")\n",
+                "\n",
                 "\n",
                 "def make_hist(new_rectangle):\n",
                 "    xy = new_rectangle.xy\n",
                 "    ix0 = int(xy[0])\n",
                 "    iy0 = int(xy[1])\n",
                 "    ix1 = int(xy[0] + new_rectangle.width)\n",
                 "    iy1 = int(xy[1] + new_rectangle.height)\n",
                 "    n, bins, patches = ax2[1].hist(\n",
-                "        a[min(iy0, iy1):max(iy0, iy1), min(ix0, ix1):max(ix0, ix1), :].ravel(),\n",
-                "        edgecolor=new_rectangle.edgecolor, facecolor='None')\n",
+                "        a[min(iy0, iy1) : max(iy0, iy1), min(ix0, ix1) : max(ix0, ix1), :].ravel(),\n",
+                "        edgecolor=new_rectangle.edgecolor,\n",
+                "        facecolor=\"None\",\n",
+                "    )\n",
                 "    new_rectangle.associated = patches\n",
                 "\n",
+                "\n",
                 "def update_hist(new_rectangle):\n",
                 "    new_rectangle.associated.remove()\n",
                 "    make_hist(new_rectangle)\n",
                 "\n",
+                "\n",
                 "rects = tbx.Rectangles(ax=ax2[0], facecolor=(0, 0, 0, 0.3))\n",
                 "rects.on_create(make_hist)\n",
                 "rects.on_change(update_hist)"
             ]
         },
         {
             "cell_type": "code",
@@ -230,32 +237,36 @@
             "id": "0654a4a4-0ebb-4156-a987-2dbff2623ac1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "fig, ax = plt.subplots(2, 1, figsize=(7, 7))\n",
                 "fig.canvas.header_visible = False\n",
                 "fig.tight_layout()\n",
-                "ax[0].imshow(a[..., 0], interpolation='none', origin='lower')\n",
+                "ax[0].imshow(a[..., 0], interpolation=\"none\", origin=\"lower\")\n",
+                "\n",
                 "\n",
                 "def make_line(p):\n",
-                "    l, = ax[1].plot(a[int(p.y), int(p.y), :])\n",
+                "    (l,) = ax[1].plot(a[int(p.y), int(p.y), :])\n",
                 "    p.associated = l\n",
                 "\n",
+                "\n",
                 "def update_line(p):\n",
                 "    p.associated.set_ydata(a[int(p.y), int(p.y), :])\n",
                 "\n",
+                "\n",
                 "def make_text(p):\n",
-                "    t = ax[1].text(50.0, np.random.random() * 10,\n",
-                "                   f'x={int(p.x)}; y={int(p.y)}')\n",
+                "    t = ax[1].text(50.0, np.random.random() * 10, f\"x={int(p.x)}; y={int(p.y)}\")\n",
                 "    p.text = t\n",
                 "\n",
+                "\n",
                 "def update_text(p):\n",
-                "    p.text.set_text(f'x={int(p.x)}; y={int(p.y)}')\n",
+                "    p.text.set_text(f\"x={int(p.x)}; y={int(p.y)}\")\n",
+                "\n",
                 "\n",
-                "points = tbx.Points(ax=ax[0], mec='white')\n",
+                "points = tbx.Points(ax=ax[0], mec=\"white\")\n",
                 "points.on_create(make_line)\n",
                 "points.on_create(make_text)\n",
                 "points.on_change(update_line)\n",
                 "points.on_change(update_text)"
             ]
         },
         {
@@ -295,13 +306,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `mpltoolbox-0.4.0/docs/conf.py` & `mpltoolbox-23.7.0/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2022 Scipp contributors (https://github.com/scipp)
 
 import os
 import sys
 
-src = os.path.abspath('../src')
-os.environ['PYTHONPATH'] = src
+src = os.path.abspath("../src")
+os.environ["PYTHONPATH"] = src
 sys.path.insert(0, src)
 
 # -- Project information -----------------------------------------------------
 
-project = 'mpltoolbox'
-copyright = '2022, Scipp contributors'
-author = 'Neil Vaytet'
+project = "mpltoolbox"
+copyright = "2022, Scipp contributors"
+author = "Neil Vaytet"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc', 'sphinx.ext.autosummary', 'sphinx.ext.mathjax', 'nbsphinx',
-    'sphinx_copybutton'
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.mathjax",
+    "nbsphinx",
+    "sphinx_copybutton",
 ]
 
-autodoc_typehints = 'description'
+autodoc_typehints = "description"
 
 autosummary_generate = True
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store', '**.ipynb_checkpoints']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", "**.ipynb_checkpoints"]
 
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
-html_sourcelink_suffix = ''  # Avoid .ipynb.txt extensions in sources
+source_suffix = ".rst"
+html_sourcelink_suffix = ""  # Avoid .ipynb.txt extensions in sources
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_book_theme'
+html_theme = "sphinx_book_theme"
 html_theme_options = {
-    'logo_only': True,
+    "logo_only": True,
     "repository_url": "https://github.com/scipp/mpltoolbox",
     "repository_branch": "main",
     "use_repository_button": True,
     "use_issues_button": True,
     "use_edit_page_button": True,
-    "show_toc_level": 2
+    "show_toc_level": 2,
 }
 html_logo = "images/logo.png"
 html_favicon = "images/favicon.ico"
```

### Comparing `mpltoolbox-0.4.0/docs/ellipses.ipynb` & `mpltoolbox-23.7.0/docs/ellipses.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962053571428571%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n')]}}, 3: {'source': {insert: [(2, "*

 * *            "'np.random.seed(20)  # Fixed for reproducibility\\n')], delete: [2]}}, 5: {'source': "*

 * *            "{insert: [(4, '- Middle-click (or Ctrl + left-click) to delete ellipse')], delete: "*

 * *            '[4]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.12'}}"}*

```diff
@@ -15,14 +15,15 @@
             "execution_count": null,
             "id": "ddff48f4-b5f9-4ec6-bbb7-212e9574404d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "plt.ioff()\n",
                 "import mpltoolbox as tbx"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -45,15 +46,15 @@
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "np.random.seed(20) # Fixed for reproducibility\n",
+                "np.random.seed(20)  # Fixed for reproducibility\n",
                 "N = 3\n",
                 "\n",
                 "for i in range(N):\n",
                 "    x0, y0, x1, y1 = 100 * np.random.random(4)\n",
                 "    ellipses.click(x0, y0)\n",
                 "    ellipses.click(x1, y1)"
             ]
@@ -73,15 +74,15 @@
             "id": "f0a4d457-5a9d-412c-8d1e-50984cb460cb",
             "metadata": {},
             "source": [
                 "**Controls**\n",
                 "\n",
                 "- Left-click and hold to make new ellipse\n",
                 "- Right-click and hold to drag/move ellipse\n",
-                "- Middle-click to delete ellipse"
+                "- Middle-click (or Ctrl + left-click) to delete ellipse"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -93,13 +94,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `mpltoolbox-0.4.0/docs/images/favicon.ico` & `mpltoolbox-23.7.0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mpltoolbox-0.4.0/docs/images/logo.png` & `mpltoolbox-23.7.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `mpltoolbox-0.4.0/docs/images/logo.svg` & `mpltoolbox-23.7.0/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `mpltoolbox-0.4.0/docs/index.rst` & `mpltoolbox-23.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mpltoolbox-0.4.0/docs/lines.ipynb` & `mpltoolbox-23.7.0/docs/lines.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963293650793651%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n')]}}, 3: {'source': {insert: [(2, "*

 * *            "'np.random.seed(100)  # Fixed for reproducibility\\n')], delete: [2]}}, 5: {'source': "*

 * *            "{insert: [(5, '- Middle-click (or Ctrl + left-click) to delete line')], delete: "*

 * *            '[5]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.12'}}"}*

```diff
@@ -16,14 +16,15 @@
             "execution_count": null,
             "id": "ddff48f4-b5f9-4ec6-bbb7-212e9574404d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "plt.ioff()\n",
                 "import mpltoolbox as tbx"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -46,15 +47,15 @@
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "np.random.seed(100) # Fixed for reproducibility\n",
+                "np.random.seed(100)  # Fixed for reproducibility\n",
                 "N = 5\n",
                 "\n",
                 "for i in range(N):\n",
                 "    x0, y0, x1, y1 = 100 * np.random.random(4)\n",
                 "    lines.click(x0, y0)\n",
                 "    lines.click(x1, y1)"
             ]
@@ -75,15 +76,15 @@
             "metadata": {},
             "source": [
                 "**Controls**\n",
                 "\n",
                 "- Left-click to make new lines\n",
                 "- Left-click and hold on line vertex to move vertex\n",
                 "- Right-click and hold to drag/move the entire line\n",
-                "- Middle-click to delete line"
+                "- Middle-click (or Ctrl + left-click) to delete line"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -95,13 +96,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `mpltoolbox-0.4.0/docs/points.ipynb` & `mpltoolbox-23.7.0/docs/points.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9961667768959436%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n')]}}, 3: {'source': {insert: [(2, "*

 * *            "'np.random.seed(100)  # Fixed for reproducibility\\n')], delete: [2]}}, 5: {'source': "*

 * *            "{insert: [(4, '- Middle-click (or Ctrl + left-click) to delete point')], delete: "*

 * *            '[4]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.12'}}"}*

```diff
@@ -15,14 +15,15 @@
             "execution_count": null,
             "id": "ddff48f4-b5f9-4ec6-bbb7-212e9574404d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "plt.ioff()\n",
                 "import mpltoolbox as tbx"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -45,15 +46,15 @@
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "np.random.seed(100) # Fixed for reproducibility\n",
+                "np.random.seed(100)  # Fixed for reproducibility\n",
                 "N = 10\n",
                 "\n",
                 "for i in range(N):\n",
                 "    x, y = 100 * np.random.random(2)\n",
                 "    points.click(x, y)"
             ]
         },
@@ -72,15 +73,15 @@
             "id": "f0d78f65-1990-483b-913f-6d4dbc7a1cea",
             "metadata": {},
             "source": [
                 "**Controls**\n",
                 "\n",
                 "- Left-click to make new point\n",
                 "- Left-click and hold on point to move point\n",
-                "- Middle-click to delete point"
+                "- Middle-click (or Ctrl + left-click) to delete point"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -92,13 +93,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `mpltoolbox-0.4.0/docs/polygons.ipynb` & `mpltoolbox-23.7.0/docs/polygons.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964094932844934%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n')]}}, 3: {'source': {insert: [(2, "*

 * *            "'np.random.seed(2)  # Fixed for reproducibility\\n')], delete: [2]}}, 5: {'source': "*

 * *            "{insert: [(5, '- Middle-click (or Ctrl + left-click) to delete polygon')], delete: "*

 * *            '[5]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.12'}}"}*

```diff
@@ -15,14 +15,15 @@
             "execution_count": null,
             "id": "ddff48f4-b5f9-4ec6-bbb7-212e9574404d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "plt.ioff()\n",
                 "import mpltoolbox as tbx"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -45,15 +46,15 @@
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "np.random.seed(2) # Fixed for reproducibility\n",
+                "np.random.seed(2)  # Fixed for reproducibility\n",
                 "N = [5, 4]\n",
                 "\n",
                 "for n in N:\n",
                 "    a = 100 * np.random.random((n, 2))\n",
                 "    x = a[:, 0]\n",
                 "    y = a[:, 1]\n",
                 "    for i in range(n):\n",
@@ -77,15 +78,15 @@
             "metadata": {},
             "source": [
                 "**Controls**\n",
                 "\n",
                 "- Left-click to make new polygon\n",
                 "- Left-click and hold on polygon vertex to move vertex\n",
                 "- Right-click and hold to drag/move the entire polygon\n",
-                "- Middle-click to delete polygon"
+                "- Middle-click (or Ctrl + left-click) to delete polygon"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -97,13 +98,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `mpltoolbox-0.4.0/docs/programmatic-control.ipynb` & `mpltoolbox-23.7.0/docs/programmatic-control.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999702380952381%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n')]}}}"}*

```diff
@@ -27,14 +27,15 @@
             "execution_count": null,
             "id": "ddff48f4-b5f9-4ec6-bbb7-212e9574404d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "plt.ioff()\n",
                 "import mpltoolbox as tbx"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `mpltoolbox-0.4.0/docs/rectangles.ipynb` & `mpltoolbox-23.7.0/docs/rectangles.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962053571428571%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n')]}}, 3: {'source': {insert: [(2, "*

 * *            "'np.random.seed(20)  # Fixed for reproducibility\\n')], delete: [2]}}, 5: {'source': "*

 * *            "{insert: [(4, '- Middle-click (or Ctrl + left-click) to delete rectangle')], delete: "*

 * *            '[4]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.12'}}"}*

```diff
@@ -15,14 +15,15 @@
             "execution_count": null,
             "id": "ddff48f4-b5f9-4ec6-bbb7-212e9574404d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "plt.ioff()\n",
                 "import mpltoolbox as tbx"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -45,15 +46,15 @@
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "np.random.seed(20) # Fixed for reproducibility\n",
+                "np.random.seed(20)  # Fixed for reproducibility\n",
                 "N = 3\n",
                 "\n",
                 "for i in range(N):\n",
                 "    x0, y0, x1, y1 = 100 * np.random.random(4)\n",
                 "    rects.click(x0, y0)\n",
                 "    rects.click(x1, y1)"
             ]
@@ -73,15 +74,15 @@
             "id": "896224cb-0611-4217-8a6c-07eea4b1d2b6",
             "metadata": {},
             "source": [
                 "**Controls**\n",
                 "\n",
                 "- Left-click and hold to make new rectangle\n",
                 "- Right-click and hold to drag/move rectangle\n",
-                "- Middle-click to delete rectangle"
+                "- Middle-click (or Ctrl + left-click) to delete rectangle"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -93,13 +94,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `mpltoolbox-0.4.0/docs/spans.ipynb` & `mpltoolbox-23.7.0/docs/spans.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962053571428572%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n')]}}, 3: {'source': {insert: [(2, "*

 * *            "'np.random.seed(10)  # Fixed for reproducibility\\n')], delete: [2]}}, 5: {'source': "*

 * *            "{insert: [(4, '- Middle-click (or Ctrl + left-click) to delete span')], delete: "*

 * *            "[4]}}, 8: {'source': {insert: [(0, 'np.random.seed(1)  # Fixed for "*

 * *            "reproducibility\\n')], delete: [0]}}, 10: {'source': {insert: [(4, '- Middle-click "*

 * *            "(or Ctrl + left-click) to delete span')], […]*

```diff
@@ -17,14 +17,15 @@
             "execution_count": null,
             "id": "ddff48f4-b5f9-4ec6-bbb7-212e9574404d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "plt.ioff()\n",
                 "import mpltoolbox as tbx"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -47,15 +48,15 @@
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "\n",
-                "np.random.seed(10) # Fixed for reproducibility\n",
+                "np.random.seed(10)  # Fixed for reproducibility\n",
                 "N = 2\n",
                 "\n",
                 "for i in range(N):\n",
                 "    x0, y0, x1, y1 = 100 * np.random.random(4)\n",
                 "    vspans.click(x0, y0)\n",
                 "    vspans.click(x1, y1)"
             ]
@@ -75,15 +76,15 @@
             "id": "896224cb-0611-4217-8a6c-07eea4b1d2b6",
             "metadata": {},
             "source": [
                 "**Controls**\n",
                 "\n",
                 "- Left-click and hold to make new vertical span\n",
                 "- Right-click and hold to drag/move span\n",
-                "- Middle-click to delete span"
+                "- Middle-click (or Ctrl + left-click) to delete span"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bbc29aab-f385-4cf1-87eb-48c7a9681f45",
             "metadata": {},
             "source": [
@@ -112,15 +113,15 @@
             "execution_count": null,
             "id": "748d584e-8b97-4e6a-bdf4-d312fc1bb3cb",
             "metadata": {
                 "nbsphinx": "hidden"
             },
             "outputs": [],
             "source": [
-                "np.random.seed(1) # Fixed for reproducibility\n",
+                "np.random.seed(1)  # Fixed for reproducibility\n",
                 "N = 2\n",
                 "\n",
                 "for i in range(N):\n",
                 "    x0, y0, x1, y1 = 100 * np.random.random(4)\n",
                 "    hspans.click(x0, y0)\n",
                 "    hspans.click(x1, y1)"
             ]
@@ -140,15 +141,15 @@
             "id": "01a53414-0bef-4645-a727-bc3591ef444f",
             "metadata": {},
             "source": [
                 "**Controls**\n",
                 "\n",
                 "- Left-click and hold to make new horizontal span\n",
                 "- Right-click and hold to drag/move span\n",
-                "- Middle-click to delete span"
+                "- Middle-click (or Ctrl + left-click) to delete span"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -160,13 +161,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `mpltoolbox-0.4.0/setup.cfg` & `mpltoolbox-23.7.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,11 @@
 [options.packages.find]
 where = src
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203
 
-[yapf]
-based_on_style = pep8
-column_limit = 88
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mpltoolbox-0.4.0/src/mpltoolbox/ellipses.py` & `mpltoolbox-23.7.0/src/mpltoolbox/ellipses.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
 import numpy as np
 from typing import Tuple
 
 
 class Ellipse(Patch):
-
     def __init__(self, x: float, y: float, number: int, ax: Axes, **kwargs):
         super().__init__(x=x, y=y, number=number, ax=ax, **kwargs)
 
     def __repr__(self):
-        return (f'Ellipse: center={self.center}, width={self.width}, '
-                f'height={self.height}, '
-                f'edgecolor={self.edgecolor}, facecolor={self.facecolor}')
+        return (
+            f"Ellipse: center={self.center}, width={self.width}, "
+            f"height={self.height}, "
+            f"edgecolor={self.edgecolor}, facecolor={self.facecolor}"
+        )
 
     def _make_patch(self, x: float, y: float, **kwargs):
         self._patch = mp.Ellipse((x, y), 0, 0, **kwargs)
         self._ax.add_patch(self._patch)
 
     def _make_vertices(self) -> Tuple[np.ndarray]:
         center = self.center
@@ -31,26 +32,28 @@
         height = self.height
         lft = center[0] - 0.5 * width
         cen = center[0]
         rgt = center[0] + 0.5 * width
         btm = center[1] - 0.5 * height
         mid = center[1]
         top = center[1] + 0.5 * height
-        return (np.array([lft, cen, rgt, rgt, rgt, cen, lft,
-                          lft]), np.array([btm, btm, btm, mid, top, top, top, mid]))
+        return (
+            np.array([lft, cen, rgt, rgt, rgt, cen, lft, lft]),
+            np.array([btm, btm, btm, mid, top, top, top, mid]),
+        )
 
     def move_vertex(self, event: Event, ind: int):
         props = super().get_new_patch_props(event=event, ind=ind)
         center = list(self.center)
-        if 'width' in props:
-            center[0] = props['corner'][0] + 0.5 * props['width']
-        if 'height' in props:
-            center[1] = props['corner'][1] + 0.5 * props['height']
-        props['center'] = center
-        del props['corner']
+        if "width" in props:
+            center[0] = props["corner"][0] + 0.5 * props["width"]
+        if "height" in props:
+            center[1] = props["corner"][1] + 0.5 * props["height"]
+        props["center"] = center
+        del props["corner"]
         self.update(**props)
 
     @property
     def center(self) -> Tuple[float]:
         return self._patch.get_center()
 
     @center.setter
```

### Comparing `mpltoolbox-0.4.0/src/mpltoolbox/hspans.py` & `mpltoolbox-23.7.0/src/mpltoolbox/hspans.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,28 @@
 from functools import partial
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
 from typing import Tuple
 
 
 class Hspan(Patch):
-
-    def __init__(self,
-                 x: float,
-                 y: float,
-                 number: int,
-                 ax: Axes,
-                 hide_median=False,
-                 **kwargs):
+    def __init__(
+        self, x: float, y: float, number: int, ax: Axes, hide_median=False, **kwargs
+    ):
         super().__init__(x=x, y=y, number=number, ax=ax, **kwargs)
         self._vertices.set_transform(self._patch.get_transform())
-        self._median = self._ax.axhline(y, ls='dashed', color=self.edgecolor)
+        self._median = self._ax.axhline(y, ls="dashed", color=self.edgecolor)
         if hide_median:
             self._median.set_visible(False)
 
     def __repr__(self):
-        return (f'VSpan: bottom={self.bottom}, top={self.top}, '
-                f'edgecolor={self.edgecolor}, facecolor={self.facecolor}')
+        return (
+            f"VSpan: bottom={self.bottom}, top={self.top}, "
+            f"edgecolor={self.edgecolor}, facecolor={self.facecolor}"
+        )
 
     def _update_vertices(self):
         super()._update_vertices()
         corners = self._patch.get_xy()
         mid = 0.5 * (corners[0, 1] + corners[1, 1])
         self._median.set_ydata([mid, mid])
```

### Comparing `mpltoolbox-0.4.0/src/mpltoolbox/lines.py` & `mpltoolbox-23.7.0/src/mpltoolbox/lines.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 from matplotlib.pyplot import Artist, Axes
 from matplotlib.backend_bases import Event
 import uuid
 from typing import Tuple
 
 
 class Line:
-
-    def __init__(self,
-                 x: float,
-                 y: float,
-                 number: int,
-                 ax: Axes,
-                 n=2,
-                 hide_vertices: bool = False,
-                 **kwargs):
+    def __init__(
+        self,
+        x: float,
+        y: float,
+        number: int,
+        ax: Axes,
+        n=2,
+        hide_vertices: bool = False,
+        **kwargs,
+    ):
         self._max_clicks = n
         self._ax = ax
         kwargs = parse_kwargs(kwargs, number)
-        if set(['ls', 'linestyle']).isdisjoint(set(kwargs.keys())):
-            kwargs['ls'] = 'solid'
-        if 'marker' not in kwargs:
-            kwargs['marker'] = 'o'
-        self._line, = self._ax.plot(x, y, **kwargs)
+        if set(["ls", "linestyle"]).isdisjoint(set(kwargs.keys())):
+            kwargs["ls"] = "solid"
+        if "marker" not in kwargs:
+            kwargs["marker"] = "o"
+        (self._line,) = self._ax.plot(x, y, **kwargs)
         if hide_vertices:
-            self.mec = 'None'
-            self.mfc = 'None'
+            self.mec = "None"
+            self.mfc = "None"
         self._line.parent = self
         self.id = uuid.uuid1().hex
 
     def __repr__(self):
-        return f'Line: x={self.x}, y={self.y}, color={self.color}'
+        return f"Line: x={self.x}, y={self.y}, color={self.color}"
 
     def __str__(self):
         return repr(self)
 
     def __len__(self):
         return len(self.x)
 
@@ -51,16 +52,18 @@
         new_data[0][ind] = event.xdata
         new_data[1][ind] = event.ydata
         self.xy = new_data
 
     def after_persist_vertex(self, event: Event):
         # Duplicate the last vertex
         new_data = self.xy
-        self.xy = (np.append(new_data[0],
-                             new_data[0][-1]), np.append(new_data[1], new_data[1][-1]))
+        self.xy = (
+            np.append(new_data[0], new_data[0][-1]),
+            np.append(new_data[1], new_data[1][-1]),
+        )
 
     @property
     def x(self) -> np.ndarray:
         return self._line.get_xdata()
 
     @x.setter
     def x(self, x: np.ndarray):
```

### Comparing `mpltoolbox-0.4.0/src/mpltoolbox/patch.py` & `mpltoolbox-23.7.0/src/mpltoolbox/patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,36 +6,35 @@
 from matplotlib.backend_bases import Event
 from matplotlib.colors import to_rgb
 from typing import Dict
 import uuid
 
 
 class Patch:
-
-    def __init__(self,
-                 x: float,
-                 y: float,
-                 number: int,
-                 ax: Axes,
-                 hide_vertices: bool = False,
-                 **kwargs):
+    def __init__(
+        self,
+        x: float,
+        y: float,
+        number: int,
+        ax: Axes,
+        hide_vertices: bool = False,
+        **kwargs,
+    ):
         self._max_clicks = 2
         self._ax = ax
         kwargs = parse_kwargs(kwargs, number)
-        defaut_color = f'C{number}'
-        if set(['ec', 'edgecolor']).isdisjoint(set(kwargs.keys())):
-            kwargs['ec'] = defaut_color
-        if set(['fc', 'facecolor']).isdisjoint(set(kwargs.keys())):
-            kwargs['fc'] = to_rgb(defaut_color) + (0.05, )
+        defaut_color = f"C{number}"
+        if set(["ec", "edgecolor"]).isdisjoint(set(kwargs.keys())):
+            kwargs["ec"] = defaut_color
+        if set(["fc", "facecolor"]).isdisjoint(set(kwargs.keys())):
+            kwargs["fc"] = to_rgb(defaut_color) + (0.05,)
         self._make_patch(x=x, y=y, **kwargs)
-        self._vertices, = self._ax.plot(*self._make_vertices(),
-                                        'o',
-                                        ls='None',
-                                        mec=self.edgecolor,
-                                        mfc='None')
+        (self._vertices,) = self._ax.plot(
+            *self._make_vertices(), "o", ls="None", mec=self.edgecolor, mfc="None"
+        )
         if hide_vertices:
             self._vertices.set_visible(False)
         self._vertices.parent = self
         self._patch.parent = self
         self.id = uuid.uuid1().hex
 
     def __str__(self):
@@ -137,16 +136,16 @@
         elif ind == 6:
             width = xopp - x
             height = y - yopp
             corner[0] = x
         elif ind == 7:
             width = xopp - x
             corner[0] = x
-        out = {'corner': corner}
+        out = {"corner": corner}
         if width is not None:
-            out['width'] = width
+            out["width"] = width
         if height is not None:
-            out['height'] = height
+            out["height"] = height
         return out
 
     def after_persist_vertex(self, event: Event):
         return
```

### Comparing `mpltoolbox-0.4.0/src/mpltoolbox/points.py` & `mpltoolbox-23.7.0/src/mpltoolbox/points.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 from .tool import Tool
 from functools import partial
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
 
 
 class Point(Line):
-
     def __init__(self, x: float, y: float, number: int, ax: Axes, **kwargs):
         super().__init__(x=x, y=y, number=number, ax=ax, **kwargs)
         self._max_clicks = 1
 
     def __repr__(self):
-        return f'Point: x={self.x}, y={self.y}, color={self.color}'
+        return f"Point: x={self.x}, y={self.y}, color={self.color}"
 
     def __str__(self):
         return repr(self)
 
     def __len__(self):
         return 1
```

### Comparing `mpltoolbox-0.4.0/src/mpltoolbox/polygons.py` & `mpltoolbox-23.7.0/src/mpltoolbox/polygons.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,77 +8,84 @@
 from matplotlib.pyplot import Artist, Axes
 from matplotlib.backend_bases import Event
 from typing import Tuple
 import uuid
 
 
 class Polygon:
-
-    def __init__(self,
-                 x: float,
-                 y: float,
-                 number: int,
-                 ax: Axes,
-                 hide_vertices: bool = False,
-                 **kwargs):
+    def __init__(
+        self,
+        x: float,
+        y: float,
+        number: int,
+        ax: Axes,
+        hide_vertices: bool = False,
+        **kwargs,
+    ):
         self._max_clicks = 0
         self._ax = ax
         line_kwargs = parse_kwargs(kwargs, number)
         fill_kwargs = {}
-        for arg in ('ec', 'edgecolor', 'fc', 'facecolor', 'alpha'):
+        for arg in ("ec", "edgecolor", "fc", "facecolor", "alpha"):
             if arg in line_kwargs:
                 fill_kwargs[arg] = line_kwargs.pop(arg)
-        if set(['mfc', 'markerfacecolor']).isdisjoint(set(line_kwargs.keys())):
-            line_kwargs['mfc'] = 'None'
-        if set(['ls', 'linestyle']).isdisjoint(set(line_kwargs.keys())):
-            line_kwargs['ls'] = 'solid'
-        if 'marker' not in line_kwargs:
-            line_kwargs['marker'] = 'o'
-        if 'alpha' not in fill_kwargs:
-            fill_kwargs['alpha'] = 0.05
-        if set(['fc', 'facecolor']).isdisjoint(set(fill_kwargs.keys())):
-            fill_kwargs['fc'] = None
-
-        self._vertices, = self._ax.plot(x, y, **line_kwargs)
-        if fill_kwargs['fc'] is None:
-            fill_kwargs['fc'] = self._vertices.get_color()
-        self._fill, = self._ax.fill(x, y, **fill_kwargs)
+        if set(["mfc", "markerfacecolor"]).isdisjoint(set(line_kwargs.keys())):
+            line_kwargs["mfc"] = "None"
+        if set(["ls", "linestyle"]).isdisjoint(set(line_kwargs.keys())):
+            line_kwargs["ls"] = "solid"
+        if "marker" not in line_kwargs:
+            line_kwargs["marker"] = "o"
+        if "alpha" not in fill_kwargs:
+            fill_kwargs["alpha"] = 0.05
+        if set(["fc", "facecolor"]).isdisjoint(set(fill_kwargs.keys())):
+            fill_kwargs["fc"] = None
+
+        (self._vertices,) = self._ax.plot(x, y, **line_kwargs)
+        if fill_kwargs["fc"] is None:
+            fill_kwargs["fc"] = self._vertices.get_color()
+        (self._fill,) = self._ax.fill(x, y, **fill_kwargs)
         if hide_vertices:
-            self.mec = 'None'
-            self.mfc = 'None'
+            self.mec = "None"
+            self.mfc = "None"
         self._fill.parent = self
         self._vertices.parent = self
         self.id = uuid.uuid1().hex
         self._distance_from_first_point = 0.05
         self._first_point_position_data = (x, y)
         self._first_point_position_axes = self._data_to_axes_transform(x, y)
 
     def __repr__(self):
-        return (f'Polygon: x={self.x}, y={self.y}, '
-                f'edgecolor={self.edgecolor}, facecolor={self.facecolor}')
+        return (
+            f"Polygon: x={self.x}, y={self.y}, "
+            f"edgecolor={self.edgecolor}, facecolor={self.facecolor}"
+        )
 
     def __str__(self):
         return repr(self)
 
     def __len__(self):
         return len(self.x)
 
     def after_persist_vertex(self, event: Event):
         new_data = self.xy
-        self.xy = (np.append(new_data[0],
-                             new_data[0][-1]), np.append(new_data[1], new_data[1][-1]))
+        self.xy = (
+            np.append(new_data[0], new_data[0][-1]),
+            np.append(new_data[1], new_data[1][-1]),
+        )
 
     def _data_to_axes_transform(self, x: float, y: float) -> Tuple[float]:
         trans = self._ax.transData.transform((x, y))
         return self._ax.transAxes.inverted().transform(trans)
 
     def _get_distance_from_first_point(self, x: float, y: float) -> float:
         xdisplay, ydisplay = self._data_to_axes_transform(x, y)
-        dist = np.sqrt((xdisplay - self._first_point_position_axes[0])**2 +
-                       (ydisplay - self._first_point_position_axes[1])**2)
+        dist = np.sqrt(
+            (xdisplay - self._first_point_position_axes[0]) ** 2
+            + (ydisplay - self._first_point_position_axes[1]) ** 2
+        )
         return dist
 
     def move_vertex(self, event: Event, ind: int):
         x = event.xdata
         y = event.ydata
         if self._get_distance_from_first_point(x, y) < self._distance_from_first_point:
             x = self._first_point_position_data[0]
```

### Comparing `mpltoolbox-0.4.0/src/mpltoolbox/rectangles.py` & `mpltoolbox-23.7.0/src/mpltoolbox/rectangles.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
 import numpy as np
 from typing import Tuple
 
 
 class Rectangle(Patch):
-
     def __init__(self, x: float, y: float, number: int, ax: Axes, **kwargs):
         super().__init__(x=x, y=y, number=number, ax=ax, **kwargs)
 
     def __repr__(self):
-        return (f'Rectangle: xy={self.xy}, width={self.width}, height={self.height}, '
-                f'edgecolor={self.edgecolor}, facecolor={self.facecolor}')
+        return (
+            f"Rectangle: xy={self.xy}, width={self.width}, height={self.height}, "
+            f"edgecolor={self.edgecolor}, facecolor={self.facecolor}"
+        )
 
     def _make_patch(self, x: float, y: float, **kwargs):
         self._patch = mp.Rectangle((x, y), 0, 0, **kwargs)
         self._ax.add_patch(self._patch)
 
     def _make_vertices(self) -> Tuple[np.ndarray]:
         xy = self.xy
@@ -38,15 +39,15 @@
         x[1::2] = x_mid
         y[0:-1:2] = yc[:-1]
         y[1::2] = y_mid
         return (x, y)
 
     def move_vertex(self, event: Event, ind: int):
         props = super().get_new_patch_props(event=event, ind=ind)
-        props['xy'] = props.pop('corner')
+        props["xy"] = props.pop("corner")
         self.update(**props)
 
     @property
     def xy(self) -> Tuple[float]:
         return self._patch.get_xy()
 
     @xy.setter
```

### Comparing `mpltoolbox-0.4.0/src/mpltoolbox/tool.py` & `mpltoolbox-23.7.0/src/mpltoolbox/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 from functools import partial
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
 from typing import Callable, List, Tuple, Union
 
 
 class Tool:
-
-    def __init__(self,
-                 ax: Axes,
-                 spawner,
-                 *,
-                 autostart: bool = True,
-                 on_create: Callable = None,
-                 on_remove: Callable = None,
-                 on_change: Callable = None,
-                 on_vertex_press: Callable = None,
-                 on_vertex_move: Callable = None,
-                 on_vertex_release: Callable = None,
-                 on_drag_press: Callable = None,
-                 on_drag_move: Callable = None,
-                 on_drag_release: Callable = None,
-                 **kwargs):
+    def __init__(
+        self,
+        ax: Axes,
+        spawner,
+        *,
+        autostart: bool = True,
+        on_create: Callable = None,
+        on_remove: Callable = None,
+        on_change: Callable = None,
+        on_vertex_press: Callable = None,
+        on_vertex_move: Callable = None,
+        on_vertex_release: Callable = None,
+        on_drag_press: Callable = None,
+        on_drag_move: Callable = None,
+        on_drag_release: Callable = None,
+        **kwargs
+    ):
         self._ax = ax
         self._fig = ax.get_figure()
         self._connections = {}
 
         self._on_create = []
         self._on_remove = []
         self._on_change = []
@@ -153,18 +154,20 @@
     def _draw(self):
         self._fig.canvas.draw_idle()
 
     def start(self):
         """
         Activate the tool.
         """
-        self._connections['button_press_event'] = self._fig.canvas.mpl_connect(
-            'button_press_event', self._on_button_press)
-        self._connections['pick_event'] = self._fig.canvas.mpl_connect(
-            'pick_event', self._on_pick)
+        self._connections["button_press_event"] = self._fig.canvas.mpl_connect(
+            "button_press_event", self._on_button_press
+        )
+        self._connections["pick_event"] = self._fig.canvas.mpl_connect(
+            "pick_event", self._on_pick
+        )
 
     def stop(self):
         """
         Dectivate the tool.
         """
         self._disconnect(list(self._connections.keys()))
 
@@ -189,31 +192,34 @@
                 del self._connections[key]
 
     def _connect(self, connections: dict):
         for key, func in connections.items():
             self._connections[key] = self._fig.canvas.mpl_connect(key, func)
 
     def _on_button_press(self, event: Event):
-        if event.button != 1 or self._pick_lock or self._get_active_tool():
+        if (
+            event.button != 1
+            or self._pick_lock
+            or self._get_active_tool()
+            or event.modifiers
+        ):
             return
         if event.inaxes != self._ax:
             return
-        if 'motion_notify_event' not in self._connections:
+        if "motion_notify_event" not in self._connections:
             self._nclicks = 0
             self._spawn_new_owner(x=event.xdata, y=event.ydata)
-            self._connect({'motion_notify_event': self._on_motion_notify})
+            self._connect({"motion_notify_event": self._on_motion_notify})
         self._nclicks += 1
         self._persist_vertex(event=event, owner=self.children[-1])
 
     def _spawn_new_owner(self, x: float, y: float):
-        owner = self._spawner(x=x,
-                              y=y,
-                              number=self._owner_counter,
-                              ax=self._ax,
-                              **self._kwargs)
+        owner = self._spawner(
+            x=x, y=y, number=self._owner_counter, ax=self._ax, **self._kwargs
+        )
         self.children.append(owner)
         self._owner_counter += 1
         self._draw()
 
     def _on_motion_notify(self, event: Event):
         self._move_vertex(event=event, ind=None, owner=self.children[-1])
 
@@ -221,125 +227,139 @@
         if event.inaxes != self._ax:
             return
         owner.move_vertex(event=event, ind=ind)
         self._draw()
 
     def _persist_vertex(self, event: Event, owner):
         if self._nclicks == owner._max_clicks:
-            self._disconnect(['motion_notify_event'])
+            self._disconnect(["motion_notify_event"])
             self._finalize_owner()
         else:
             owner.after_persist_vertex(event)
         self._draw()
 
     def _finalize_owner(self):
         child = self.children[-1]
         child.set_picker(5.0)
         if self.on_create is not None:
             self.call_on_create(child)
 
     def _on_pick(self, event: Event):
+        mev = event.mouseevent
         if self._get_active_tool():
             return
-        if event.mouseevent.inaxes != self._ax:
+        if mev.inaxes != self._ax:
             return
         art = event.artist
-        if event.mouseevent.button == 1:
+        if (mev.button == 1) and ("ctrl" not in mev.modifiers):
             if not art.parent.is_moveable(art):
                 return
             self._pick_lock = True
             self._grab_vertex(event)
             if self.on_vertex_press is not None:
                 self.call_on_vertex_press(self._moving_vertex_owner)
-        if event.mouseevent.button == 3:
+        if mev.button == 3:
             if not art.parent.is_draggable(art):
                 return
             self._pick_lock = True
             self._grab_owner(event)
             if self.on_drag_press is not None:
                 self.call_on_drag_press(self._grabbed_owner)
-        elif event.mouseevent.button == 2:
+        if (mev.button == 2) or ((mev.button == 1) and ("ctrl" in mev.modifiers)):
             if not art.parent.is_removable(art):
                 return
             self._remove_owner(art.parent)
             if self.on_remove is not None:
                 self.call_on_remove(art.parent)
 
     def _remove_owner(self, owner):
         owner.remove()
         self.children.remove(owner)
         self._draw()
 
     def _grab_vertex(self, event: Event):
-        self._connect({
-            'motion_notify_event':
-            self._on_vertex_motion,
-            'button_release_event':
-            partial(self._release_owner, kind='vertex')
-        })
-
+        self._connect(
+            {
+                "motion_notify_event": self._on_vertex_motion,
+                "button_release_event": partial(self._release_owner, kind="vertex"),
+            }
+        )
         self._moving_vertex_index = event.ind[0]
         self._moving_vertex_owner = event.artist.parent
 
     def _on_vertex_motion(self, event: Event):
-        self._move_vertex(event=event,
-                          ind=self._moving_vertex_index,
-                          owner=self._moving_vertex_owner)
+        self._move_vertex(
+            event=event, ind=self._moving_vertex_index, owner=self._moving_vertex_owner
+        )
         if self.on_vertex_move is not None:
             self.call_on_vertex_move(self._moving_vertex_owner)
         if self.on_change is not None:
             self.call_on_change(self._moving_vertex_owner)
 
     def _grab_owner(self, event: Event):
-        self._connect({
-            'motion_notify_event': self._move_owner,
-            'button_release_event': partial(self._release_owner, kind='drag')
-        })
+        self._connect(
+            {
+                "motion_notify_event": self._move_owner,
+                "button_release_event": partial(self._release_owner, kind="drag"),
+            }
+        )
         self._grabbed_owner = event.artist.parent
         self._grab_mouse_origin = event.mouseevent.xdata, event.mouseevent.ydata
         self._grabbed_owner_origin = self._grabbed_owner.xy
 
     def _move_owner(self, event: Event):
         if event.inaxes != self._ax:
             return
         dx = event.xdata - self._grab_mouse_origin[0]
         dy = event.ydata - self._grab_mouse_origin[1]
-        self._grabbed_owner.xy = (self._grabbed_owner_origin[0] + dx,
-                                  self._grabbed_owner_origin[1] + dy)
+        self._grabbed_owner.xy = (
+            self._grabbed_owner_origin[0] + dx,
+            self._grabbed_owner_origin[1] + dy,
+        )
         self._draw()
         if self.on_drag_move is not None:
             self.call_on_drag_move(self._grabbed_owner)
         if self.on_change is not None:
             self.call_on_change(self._grabbed_owner)
 
     def _release_owner(self, event: Event, kind: str):
-        self._disconnect(['motion_notify_event', 'button_release_event'])
+        self._disconnect(["motion_notify_event", "button_release_event"])
         self._pick_lock = False
-        if (kind == 'vertex') and (self.on_vertex_release is not None):
+        if (kind == "vertex") and (self.on_vertex_release is not None):
             self.call_on_vertex_release(self._moving_vertex_owner)
-        elif (kind == 'drag') and (self.on_drag_release is not None):
+        elif (kind == "drag") and (self.on_drag_release is not None):
             self.call_on_drag_release(self._grabbed_owner)
 
-    def click(self, x: Union[float, Tuple[float]], y: float = None, *, button: int = 1):
+    def click(
+        self,
+        x: Union[float, Tuple[float]],
+        y: float = None,
+        *,
+        button: int = 1,
+        modifiers: List[str] = None
+    ):
         """
         Simulate a click on the figure.
 
         :param x: If only a float is given: the x coordinate for the click event. If a
             tuple of length 2 is given, it contains both the x and y coordinates for
             the event.
         :param y: The y coordinate for the event. Can be `None` if `x` is a tuple of
             length 2.
-        : param button: 1 is for left-click, 2 is for middle-click, 3 is for
+        :param button: 1 is for left-click, 2 is for middle-click, 3 is for
             right-click.
+        :param modifiers: A list of modifier keys that were pressed during the click.
         """
         if y is None:
             y = x[1]
             x = x[0]
-        ev = DummyEvent(xdata=x, ydata=y, inaxes=self._ax, button=button)
-        if 'motion_notify_event' in self._connections:
+        ev = DummyEvent(
+            xdata=x, ydata=y, inaxes=self._ax, button=button, modifiers=modifiers
+        )
+        if "motion_notify_event" in self._connections:
             self._on_motion_notify(ev)
         self._on_button_press(ev)
 
     def remove(self, child):
         """
         Remove an artist from the figure.
```

### Comparing `mpltoolbox-0.4.0/src/mpltoolbox/vspans.py` & `mpltoolbox-23.7.0/src/mpltoolbox/vspans.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,34 @@
 from functools import partial
 from matplotlib.pyplot import Axes
 from matplotlib.backend_bases import Event
 from typing import Tuple
 
 
 class Vspan(Patch):
-
-    def __init__(self,
-                 x: float,
-                 y: float,
-                 number: int,
-                 ax: Axes,
-                 hide_median: bool = False,
-                 **kwargs):
+    def __init__(
+        self,
+        x: float,
+        y: float,
+        number: int,
+        ax: Axes,
+        hide_median: bool = False,
+        **kwargs,
+    ):
         super().__init__(x=x, y=y, number=number, ax=ax, **kwargs)
         self._vertices.set_transform(self._patch.get_transform())
-        self._median = self._ax.axvline(x, ls='dashed', color=self.edgecolor)
+        self._median = self._ax.axvline(x, ls="dashed", color=self.edgecolor)
         if hide_median:
             self._median.set_visible(False)
 
     def __repr__(self):
-        return (f'VSpan: left={self.left}, right={self.right}, '
-                f'edgecolor={self.edgecolor}, facecolor={self.facecolor}')
+        return (
+            f"VSpan: left={self.left}, right={self.right}, "
+            f"edgecolor={self.edgecolor}, facecolor={self.facecolor}"
+        )
 
     def _update_vertices(self):
         super()._update_vertices()
         corners = self._patch.get_xy()
         mid = 0.5 * (corners[0, 0] + corners[2, 0])
         self._median.set_xdata([mid, mid])
```

### Comparing `mpltoolbox-0.4.0/src/mpltoolbox.egg-info/PKG-INFO` & `mpltoolbox-23.7.0/src/mpltoolbox.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltoolbox
-Version: 0.4.0
+Version: 23.7.0
 Summary: Interactive tools for matplotlib
 Home-page: https://github.com/scipp/mpltoolbox
 Author: Neil Vaytet
 Author-email: neil.vaytet@esss.se
 License: BSD
 Project-URL: Bug Tracker, https://github.com/scipp/mpltoolbox/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mpltoolbox-0.4.0/src/mpltoolbox.egg-info/SOURCES.txt` & `mpltoolbox-23.7.0/src/mpltoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

