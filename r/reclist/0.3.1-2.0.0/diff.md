# Comparing `tmp/reclist-0.3.1.tar.gz` & `tmp/reclist-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reclist-0.3.1.tar", last modified: Thu Nov  3 16:45:00 2022, max compression
+gzip compressed data, was "reclist-2.0.0.tar", last modified: Tue Jul 25 01:03:04 2023, max compression
```

## Comparing `reclist-0.3.1.tar` & `reclist-2.0.0.tar`

### file list

```diff
@@ -1,51 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:45:00.457701 reclist-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-03 16:38:07.000000 reclist-0.3.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3499 2022-11-03 16:38:07.000000 reclist-0.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-03 16:38:07.000000 reclist-0.3.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-11-03 16:38:07.000000 reclist-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-11-03 16:38:07.000000 reclist-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    20627 2022-11-03 16:45:00.461701 reclist-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17095 2022-11-03 16:38:07.000000 reclist-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:45:00.441700 reclist-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-11-03 16:38:07.000000 reclist-0.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-03 16:38:07.000000 reclist-0.3.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     4797 2022-11-03 16:38:07.000000 reclist-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-03 16:38:07.000000 reclist-0.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-11-03 16:38:07.000000 reclist-0.3.1/docs/core.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-03 16:38:07.000000 reclist-0.3.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-11-03 16:38:07.000000 reclist-0.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-11-03 16:38:07.000000 reclist-0.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-11-03 16:38:07.000000 reclist-0.3.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-03 16:38:07.000000 reclist-0.3.1/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:45:00.445701 reclist-0.3.1/reclist/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7550 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/abstractions.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/current.py
--rw-r--r--   0 runner    (1001) docker     (121)     3623 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:45:00.453701 reclist-0.3.1/reclist/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7013 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/metrics/distance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     5021 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/metrics/hits.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/metrics/perturbation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/metrics/price_homogeneity.py
--rw-r--r--   0 runner    (1001) docker     (121)     3799 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/metrics/standard_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)    11183 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/reclist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:45:00.453701 reclist-0.3.1/reclist/recommenders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/recommenders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5506 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/recommenders/prod2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:45:00.457701 reclist-0.3.1/reclist/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-11-03 16:38:07.000000 reclist-0.3.1/reclist/utils/train_w2v.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:45:00.449700 reclist-0.3.1/reclist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20627 2022-11-03 16:45:00.000000 reclist-0.3.1/reclist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-11-03 16:45:00.000000 reclist-0.3.1/reclist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 16:45:00.000000 reclist-0.3.1/reclist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 16:45:00.000000 reclist-0.3.1/reclist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-03 16:45:00.000000 reclist-0.3.1/reclist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-03 16:45:00.000000 reclist-0.3.1/reclist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-03 16:45:00.461701 reclist-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-11-03 16:38:07.000000 reclist-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:45:00.457701 reclist-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-03 16:38:07.000000 reclist-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-11-03 16:38:07.000000 reclist-0.3.1/tests/test_reclist.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 01:03:04.736948 reclist-2.0.0/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      165 2023-02-28 04:47:32.000000 reclist-2.0.0/AUTHORS.rst
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     3499 2023-02-28 04:47:32.000000 reclist-2.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)       89 2023-02-28 04:47:32.000000 reclist-2.0.0/HISTORY.rst
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1074 2023-07-14 01:35:32.000000 reclist-2.0.0/LICENSE
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      262 2023-02-28 04:47:32.000000 reclist-2.0.0/MANIFEST.in
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    14391 2023-07-25 01:03:04.736948 reclist-2.0.0/PKG-INFO
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    13598 2023-07-25 01:02:28.000000 reclist-2.0.0/README.rst
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 01:03:04.732948 reclist-2.0.0/reclist/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      103 2023-07-24 17:04:06.000000 reclist-2.0.0/reclist/__init__.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      107 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/charts.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     2884 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/logs.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1612 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/metadata.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 01:03:04.736948 reclist-2.0.0/reclist/metrics/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        0 2023-02-28 04:47:32.000000 reclist-2.0.0/reclist/metrics/__init__.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     7003 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/metrics/distance_metrics.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     4855 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/metrics/hits.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1032 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/metrics/perturbation.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1567 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/metrics/price_homogeneity.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    11840 2023-07-24 17:02:51.000000 reclist-2.0.0/reclist/metrics/standard_metrics.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     9036 2023-07-24 17:02:51.000000 reclist-2.0.0/reclist/reclist.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     5106 2023-07-14 01:35:32.000000 reclist-2.0.0/reclist/similarity_models.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 01:03:04.736948 reclist-2.0.0/reclist.egg-info/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)    14391 2023-07-25 01:03:04.000000 reclist-2.0.0/reclist.egg-info/PKG-INFO
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      629 2023-07-25 01:03:04.000000 reclist-2.0.0/reclist.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-07-25 01:03:04.000000 reclist-2.0.0/reclist.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        1 2023-03-11 01:25:56.000000 reclist-2.0.0/reclist.egg-info/not-zip-safe
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      258 2023-07-25 01:03:04.000000 reclist-2.0.0/reclist.egg-info/requires.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)        8 2023-07-25 01:03:04.000000 reclist-2.0.0/reclist.egg-info/top_level.txt
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)      424 2023-07-25 01:03:04.736948 reclist-2.0.0/setup.cfg
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     1540 2023-07-24 17:04:06.000000 reclist-2.0.0/setup.py
+drwxrwxr-x   0 vinid     (1000) vinid     (1000)        0 2023-07-25 01:03:04.736948 reclist-2.0.0/tests/
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)       37 2023-02-28 04:47:32.000000 reclist-2.0.0/tests/__init__.py
+-rw-rw-r--   0 vinid     (1000) vinid     (1000)     2619 2023-07-17 19:47:56.000000 reclist-2.0.0/tests/test_reclist.py
```

### Comparing `reclist-0.3.1/CONTRIBUTING.rst` & `reclist-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `reclist-0.3.1/LICENSE` & `reclist-2.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
```

### Comparing `reclist-0.3.1/PKG-INFO` & `reclist-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,368 +1,309 @@
 Metadata-Version: 2.1
 Name: reclist
-Version: 0.3.1
+Version: 2.0.0
 Summary: RecList
 Home-page: https://github.com/jacopotagliabue/reclist
 Author: RecList
 Author-email: 
 License: MIT license
-Description: =======
-        RecList
-        =======
-        
-        
-        .. image:: https://img.shields.io/pypi/v/reclist.svg
-                :target: https://pypi.python.org/pypi/reclist
-        
-        .. image:: https://readthedocs.org/projects/reclist/badge/?version=latest
-                :target: https://reclist.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/workflows/Python%20package/badge.svg
-                :target: https://github.com/jacopotagliabue/reclist/actions
-        
-        .. image:: https://img.shields.io/github/contributors/jacopotagliabue/reclist
-                :target: https://github.com/jacopotagliabue/reclist/graphs/contributors/
-                :alt: Contributors
-        
-        .. image:: https://img.shields.io/badge/License-MIT-blue.svg
-                :target: https://lbesson.mit-license.org/
-                :alt: License
-        
-        .. image:: https://pepy.tech/badge/reclist
-                :target: https://pepy.tech/project/reclist
-                :alt: Downloads
-        
-        .. image:: https://img.shields.io/badge/youtube-video-red
-                :target: https://www.youtube.com/watch?v=cAlJYxFYA04
-                :alt: YouTube
-        
-        
-        RecList
-        
-        
-        * Free software: MIT license
-        * Documentation: https://reclist.readthedocs.io.
-        
-        Overview
-        --------
-        
-        *RecList* is an open source library providing behavioral, "black-box" testing for recommender systems. Inspired by the pioneering work of
-        `Ribeiro et al. 2020 <https://aclanthology.org/2020.acl-main.442.pdf>`__ in NLP, we introduce a general plug-and-play procedure to scale up behavioral testing,
-        with an easy-to-extend interface for custom use cases.
-        
-        While quantitative metrics over held-out data points are important, a lot more tests are needed for recommenders
-        to properly function in the wild and not erode our confidence in them: for example, a model may boast an accuracy improvement over the entire dataset, but actually be significantly worse than another on rare items or new users; or again, a model that correctly recommends HDMI cables as add-on for shoppers buying a TV, may also wrongly  recommend TVs to shoppers just buying a cable.
-        
-        *RecList* goal is to operationalize these important intuitions into a practical package for testing research and production models in a more nuanced way, without
-        requiring unnecessary custom code and ad hoc procedures. To streamline comparisons among existing models, *RecList* ships with popular datasets and ready-made behavioral tests: read the `TDS blog post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__ as a gentle introduction to the main use cases, check the `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__ for more details on the relevant literature.
-        
-        If you are not familiar with the library, we suggest first taking our small tour to get acquainted with the main abstractions through ready-made models and public datasets.
-        
-        Quick Links
-        ~~~~~~~~~~~
-        
-        * Our `talk <https://www.youtube.com/watch?v=cAlJYxFYA04>`__ at Stitch Fix Algo Hour, for a general presentation.
-        * Our `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__, with in-depth analysis, detailed use cases and scholarly references (`arxiv <https://arxiv.org/abs/2111.09963>`__).
-        * A `colab notebook <https://colab.research.google.com/drive/1Wn5mm0csEkyWqmBBDxNBkfGR6CNfWeH-?usp=sharing>`__, showing how to train a cart recommender model from scratch and use the library to test it.
-        * Our `blog post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__, with examples and practical tips.
-        
-        
-        Supporters
-        ~~~~~~~~~~
-        RecList is a community project made possible by the generous support of these awesome folks. Make sure to check them out!
-        
-        Comet
-        =====
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/raw/main/images/comet.png
-           :target: https://www.comet.com/?utm_source=jacopot&utm_medium=referral&utm_campaign=online_jacopot_2022&utm_content=github_reclist
-           :width: 175
-        
-        Neptune
-        =======
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/raw/main/images/neptune.png
-           :target: https://neptune.ai
-           :width: 175
-        
-        Gantry
-        ======
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/raw/main/images/gantry.png
-           :target: https://gantry.io/
-           :width: 175
-        
-        
-        Project updates
-        ~~~~~~~~~~~~~~~
-        
-        *Community Support*: RecList is an open source community project made possible by the support of the awesome folks at `Comet <https://www.comet.ml/site/>`__, `Neptune <https://neptune.ai/>`__ and `Gantry <https://gantry.io/>`__.
-        Soon RecList tests will be natively integrated with the MLOps tools you already know and love!
-        
-        *June 2022*: We launched a `website <https://reclist.io/>`__ to collect RecList materials, such as talks and presentations.
-        RecList is powering the `Data Challenge <https://reclist.io/cikm2022-cup/>`__ at CIKM 2022: fill `the form <https://docs.google.com/forms/d/e/1FAIpQLSfAypzM1mvd79JfRGRbb9QMfXGMoVYosdjU9C4NFEWNSNUZXQ/viewform>`__ for updates.
-        
-        In the last few months, we presented this library to practioners at Tubi, eBay, NVIDIA, BBC and other RecSys companies: we are in the process of collecting our thoughts after all the feedback we received, as we plan a beta release for this package in the next few months - come back often for updates, as we will also open a call for collaboration!
-        
-        Please remember that the library is in alpha (i.e. enough working code to finish the paper and tinker with it). We welcome early feedback, but please be advised that the package may change substantially in the near future ("If you're not embarrassed by the first version, you've launched too late").
-        
-        Summary
-        ~~~~~~~
-        
-        This doc is structured as follows:
-        
-        * `Quick Start`_
-        * `A Guided Tour`_
-        * `Capabilities`_
-        * `Roadmap`_
-        * `Talks and Presentations`_
-        * `License and Citation`_
-        * `Acknowledgments`_
-        
-        Quick Start
-        -----------
-        
-        If you want to see *RecList* in action, clone the repository, create and activate a virtual env, and install the required packages from pip (you can install from root of course). If you prefer to experiment in an interactive, no-installation-required fashion, try out our `colab notebook <https://colab.research.google.com/drive/1Wn5mm0csEkyWqmBBDxNBkfGR6CNfWeH-?usp=sharing>`__.
-        
-        Sample scripts are divided by use-cases: similar items, complementary items or session-based recommendations. When executing one, a suitable public dataset will be downloaded, and a baseline model trained: finally, the script will run a pre-made suite of behavioral tests to show typical results.
-        
-        .. code-block:: bash
-        
-            git clone https://github.com/jacopotagliabue/reclist
-            cd reclist
-            python3 -m venv venv
-            source venv/bin/activate
-            pip install reclist
-            python examples/coveo_complementary_rec.py
-        
-        Running *your* model on one of the supported dataset, leveraging the pre-made tests, is as easy as implementing a simple interface, *RecModel*.
-        
-        Once you've run successfully the sample script, take the guided tour below to learn more about the abstractions and the out-of-the-box capabilities of *RecList*.
-        
-        A Guided Tour
-        -------------
-        
-        An instance of `RecList <https://github.com/jacopotagliabue/reclist/blob/main/reclist/reclist.py>`__ represents a suite of tests for recommender systems: given
-        a dataset (more appropriately, an instance of `RecDataset <https://github.com/jacopotagliabue/reclist/blob/main/reclist/abstractions.py>`__)
-        and a model (an instance of `RecModel <https://github.com/jacopotagliabue/reclist/blob/main/reclist/abstractions.py>`__), it will run the specified tests on the target dataset, using the supplied model.
-        
-        For example, the following code instantiates a pre-made suite of tests that contains sensible defaults for a `cart recommendation use case <https://github.com/jacopotagliabue/reclist/blob/main/reclist/reclist.py>`__:
-        
-        .. code-block:: python
-        
-            rec_list = CoveoCartRecList(
-                model=model,
-                dataset=coveo_dataset
-            )
-            # invoke rec_list to run tests
-            rec_list(verbose=True)
-        
-        Our library pre-packages standard recSys KPIs and important behavioral tests, divided by use cases, but it is built with extensibility in mind: you can re-use tests in new suites, or you can write new domain-specific suites and tests.
-        
-        Any suite must inherit the *RecList* interface, and then declare with Pytonic decorators its tests. In this case, the test re-uses a standard function:
-        
-        .. code-block:: python
-        
-            class MyRecList(RecList):
-        
-                @rec_test(test_type='stats')
-                def basic_stats(self):
-                    """
-                    Basic statistics on training, test and prediction data
-                    """
-                    from reclist.metrics.standard_metrics import statistics
-                    return statistics(self._x_train,
-                        self._y_train,
-                        self._x_test,
-                        self._y_test,
-                        self._y_preds)
-        
-        
-        Any model can be tested, as long as its predictions are wrapped in a *RecModel*. This allows for pure "black-box" testings,
-        a SaaS provider can be tested just by wrapping the proper API call in the method:
-        
-        .. code-block:: python
-        
-            class MyCartModel(RecModel):
-        
-                def __init__(self, **kwargs):
-                    super().__init__(**kwargs)
-        
-                def predict(self, prediction_input: list, *args, **kwargs):
-                    """
-                    Implement the abstract method, accepting a list of lists, each list being
-                    the content of a cart: the predictions returned by the model are the top K
-                    items suggested to complete the cart.
-                    """
-        
-                    return
-        
-        More generally, the logical workflow of a typical RecList implementation is as follows (see our `blog post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__ for a longer explanation):
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/workflow.gif
-           :height: 400
-        
-        While many standard KPIs are available in the package, the philosophy behind *RecList* is that metrics like Hit Rate provide only a partial picture
-        of the expected behavior of recommenders in the wild: two models with very similar accuracy can have very different behavior on, say, the long-tail, or
-        model A can be better than model B overall, but at the expense of providing disastrous performance on a set of inputs that are particularly important in production.
-        
-        *RecList* recognizes that outside of academic benchmarks, some mistakes are worse than others, and not all inputs are created equal: when possible, it tries
-        to operationalize through scalable code behavioral insights for debugging and error analysis; it also
-        provides extensible abstractions when domain knowledge and custom logic are needed.
-        
-        Once you run a suite of tests, results are dumped automatically and versioned in a local folder, structured as follows
-        (name of the suite, name of the model, run timestamp):
-        
-        .. code-block::
-        
-            .reclist/
-              myList/
-                myModel/
-                  1637357392/
-                  1637357404/
-        
-        If you start using *RecList* as part of your standard testings - either for research or production purposes - you can use the JSON report
-        for machine-to-machine communication with downstream system (e.g. you may want to automatically fail the model pipeline if certain behavioral tests are not passed).
-        
-        Note: our app is deprecated, as RecList Beta will have connectors with existing apps (experiment trackers, model cards, etc.).
-        
-        Capabilities
-        ------------
-        
-        *RecList* provides a dataset and model agnostic framework to scale up behavioral tests. As long as the proper abstractions
-        are implemented, all the out-of-the-box components can be re-used. For example:
-        
-        * you can use a public dataset provided by *RecList* to train your new cart recommender model, and then use the *RecTests* we provide for that use case;
-        
-        * you can use some baseline model on your custom dataset, to establish a baseline for your project;
-        
-        * you can use a custom model, on a private dataset and define from scratch a new suite of tests, mixing existing methods and domain-specific tests.
-        
-        We list below what we currently support out-of-the-box, with particular focus on datasets and tests, as the models we provide
-        are convenient baselines, but they are not meant to be SOTA research models.
-        
-        Datasets
-        ~~~~~~~~
-        
-        RecList features convenient wrappers around popular datasets, to help test models over known benchmarks
-        in a standardized way.
-        
-        * `Coveo Data Challenge <https://github.com/coveooss/SIGIR-ecom-data-challenge>`__
-        * (a smaller version of) `The Million Playlist Dataset <https://engineering.atspotify.com/2018/05/30/introducing-the-million-playlist-dataset-and-recsys-challenge-2018/>`__
-        * (a smaller version of) `MovieLens <https://grouplens.org/datasets/movielens/>`__
-        
-        Behavioral Tests
-        ~~~~~~~~~~~~~~~~
-        
-        RecList helps report standard quantitative metrics over popular (or custom) datasets, such as the ones collected in
-        *standard_metrics.py*: hit rate, mrr, coverage, popularity bias, etc. However, RecList raison d'etre is providing plug-and-play
-        behavioral tests, as agnostic as possible to the underlying models and datasets, while leaving open the possibility of writing
-        personalized tests when domain knowledge and custom logic are necessary.
-        
-        Tests descriptions are available in our (WIP) `docs <https://reclist.readthedocs.io>`__, but we share here some examples from our `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__.
-        
-        First, RecList allows to compare the performance of models which may have similar aggregate KPIs (e.g. hit rate on the entire
-        test set) in different slices. When plotting HR by product popularity, it is easy to spot that
-        prod2vec works much better with rarer items than the alternatives:
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/hit_rate_dist.png
-           :height: 175
-        
-        When slicing by important meta-data (in this simulated example, brands), RecList uncovers significant differences
-        in performance for different groups; since the features we care about vary across datasets,
-        the package allows for a generic way to partition the test set and compute per-slice metrics:
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/slice_dist.png
-           :height: 175
-        
-        Finally, RecList can take advantage of the latent item space to compute the cosine distances <query item, ground truth> and
-        <query item, prediction> for missed predictions in the test set. In a cart recommender use case, we expect items to
-        reflect the complementary nature of the suggestions: if a TV is in the cart, a model should recommend a HDMI cable,
-        not another TV. As we see in the comparison below, Google's predictions better match the label distribution,
-        suggesting that the model better capture the nature of the task:
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/distance_to_query.png
-           :height: 175
-        
-        Roadmap
-        -------
-        
-        We have exciting news about our Beta, including the usage of RecList as main library for the `CIKM Data Challenge <https://reclist.io/cikm2022-cup/>`__!
-        
-        Contributing
-        ~~~~~~~~~~~~
-        
-        We will update this repo with some guidelines for contributions as soon as the codebase becomes more stable. Check back often for updates!
-        
-        Acknowledgments
-        ---------------
-        
-        The original authors are:
-        
-        * Patrick John Chia - `LinkedIn <https://www.linkedin.com/in/patrick-john-chia-b0a34019b/>`__, `GitHub <https://github.com/patrickjohncyh>`__
-        * Jacopo Tagliabue - `LinkedIn <https://www.linkedin.com/in/jacopotagliabue/>`__, `GitHub <https://github.com/jacopotagliabue>`__
-        * Federico Bianchi - `LinkedIn <https://www.linkedin.com/in/federico-bianchi-3b7998121/>`__, `GitHub <https://github.com/vinid>`__
-        * Chloe He - `LinkedIn <https://www.linkedin.com/in/chloe-he//>`__, `GitHub <https://github.com/chloeh13q>`__
-        * Brian Ko - `LinkedIn <https://www.linkedin.com/in/briankosw/>`__, `GitHub <https://github.com/briankosw>`__
-        
-        If you have questions or feedback, please reach out to: :code:`jacopo dot tagliabue at tooso dot ai`.
-        
-        Talks and Presentations
-        -----------------------
-        
-        Past and upcoming talks and presentations can be found at our new `website <https://reclist.io/>`__.
-        
-        License and Citation
-        --------------------
-        
-        All the code is released under an open MIT license. If you found *RecList* useful, please cite our WWW paper:
-        
-        .. code-block:: bash
-        
-            @inproceedings{10.1145/3487553.3524215,
-                author = {Chia, Patrick John and Tagliabue, Jacopo and Bianchi, Federico and He, Chloe and Ko, Brian},
-                title = {Beyond NDCG: Behavioral Testing of Recommender Systems with RecList},
-                year = {2022},
-                isbn = {9781450391306},
-                publisher = {Association for Computing Machinery},
-                address = {New York, NY, USA},
-                url = {https://doi.org/10.1145/3487553.3524215},
-                doi = {10.1145/3487553.3524215},
-                pages = {99–104},
-                numpages = {6},
-                keywords = {recommender systems, open source, behavioral testing},
-                location = {Virtual Event, Lyon, France},
-                series = {WWW '22 Companion}
-            }
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2021-11-16)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: reclist
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=======
+RecList
+=======
+
+.. image:: images/reclist.png
+        :width: 30%
+        :alt: Rocket Emoji
+
+
+.. image:: https://img.shields.io/pypi/v/reclist.svg
+        :target: https://pypi.python.org/pypi/reclist
+
+.. image:: https://readthedocs.org/projects/reclist/badge/?version=latest
+        :target: https://reclist.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+.. image:: https://github.com/jacopotagliabue/reclist/workflows/Python%20package/badge.svg
+        :target: https://github.com/jacopotagliabue/reclist/actions
+
+.. image:: https://img.shields.io/github/contributors/jacopotagliabue/reclist
+        :target: https://github.com/jacopotagliabue/reclist/graphs/contributors/
+        :alt: Contributors
+
+.. image:: https://img.shields.io/badge/License-MIT-blue.svg
+        :target: https://lbesson.mit-license.org/
+        :alt: License
+
+.. image:: https://pepy.tech/badge/reclist
+        :target: https://pepy.tech/project/reclist
+        :alt: Downloads
+
+.. image:: https://img.shields.io/badge/youtube-video-red
+        :target: https://www.youtube.com/watch?v=cAlJYxFYA04
+        :alt: YouTube
+
+
+
+Overview
+--------
+
+*RecList* is an open source library providing behavioral, "black-box" testing for recommender systems. Inspired by the pioneering work of
+`Ribeiro et al. 2020 <https://aclanthology.org/2020.acl-main.442.pdf>`__ in NLP, we introduce a general plug-and-play procedure to scale up behavioral testing, with an easy-to-extend interface for custom use cases.
+
+While quantitative metrics over held-out data points are important, a lot more tests are needed for recommenders
+to properly function in the wild and not erode our confidence in them: for example, a model may boast an accuracy improvement over the entire dataset, but actually be significantly worse than another on rare items or new users; or again, a model that correctly recommends HDMI cables as add-on for shoppers buying a TV, may also wrongly  recommend TVs to shoppers just buying a cable.
+
+*RecList* goal is to operationalize these important intuitions into a practical package for testing research and production models in a more nuanced way, without
+requiring unnecessary custom code and ad hoc procedures.
+
+If you are not familiar with the library, we suggest first taking our small tour to get acquainted with the main abstractions through ready-made models and tests.
+
+Colab Tutorials
+~~~~~~~~~~~~~~~
+
+
+.. |colab1_tutorial| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :target: https://colab.research.google.com/drive/1GVsVB1a3H9qbRQvwtb0TBDxq8A5nXc5w?usp=sharing
+    :alt: Open In Colab
+
+.. |colab2_tutorial| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :target: https://colab.research.google.com/drive/1QeXglfCUEcscHB6L0Gch2qDKDDlfwLlq?usp=sharing
+    :alt: Open In Colab
+
+.. |colab3_tutorial| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :target: https://colab.research.google.com/drive/1ek-TIT1ZJta59-O73GaXsOINvt46dnkz?usp=sharing
+    :alt: Open In Colab
+
++--------------------------------------------------------------------------------+------------------+
+| Name                                                                           | Link             |
++================================================================================+==================+
+| Tutorial 101 - Introduction to Reclist                                         | |colab1_tutorial||
++--------------------------------------------------------------------------------+------------------+
+| Tutorial - RecList at EvalRS2023 (KDD)                                         | |colab2_tutorial||
++--------------------------------------------------------------------------------+------------------+
+| Tutorial -  FashionCLIP Evaluation with RecList                                | |colab3_tutorial||
++--------------------------------------------------------------------------------+------------------+
+
+Quick Links
+~~~~~~~~~~~
+
+* The original `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__ (`arxiv <https://arxiv.org/abs/2111.09963>`__) and initial `release post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__.
+* `EvalRS22@CIKM <https://github.com/RecList/evalRS-CIKM-2022>`__ and `EvalRS23@KDD <https://reclist.io/kdd2023-cup/>`__ , for music recommendations with RecList.
+* A `colab notebook <https://colab.research.google.com/drive/1GVsVB1a3H9qbRQvwtb0TBDxq8A5nXc5w>`__, for a quick interactive tour.
+* Our `website <https://reclist.io/>`__ for past talks and presentations.
+
+
+Status
+~~~~~~~~~~~
+
+* *RecList* is free software released under the MIT license, and it has been adopted by popular `open-source <https://github.com/RecList/evalRS-CIKM-2022>`__  `data challenges <https://reclist.io/kdd2023-cup/>`__.
+* After a major API re-factoring, *RecList* is now in *beta*.
+
+Summary
+~~~~~~~
+
+This doc is structured as follows:
+
+* `Quick Start`_
+* `A Guided Tour`_
+* `Capabilities`_
+* `License and Citation`_
+* `Acknowledgments`_
+
+Quick Start
+-----------
+
+You can take a quick tour online using our `colab notebook <https://colab.research.google.com/drive/1GVsVB1a3H9qbRQvwtb0TBDxq8A5nXc5w>`__.
+If you want to use *RecList* locally, clone the repository, create and activate a virtual env, and install the required packages from pip (you can also install from root of course).
+
+.. code-block:: bash
+
+    git clone https://github.com/jacopotagliabue/reclist
+    cd reclist
+    python3 -m venv venv
+    source venv/bin/activate
+    pip install reclist
+    cd examples
+    python dummy.py
+
+The sample script will run a suite of tests on a dummy dataset and model, showcasing a typical workflow with the library. Note the commented arguments in the script, which you can use to customize the behavior of the library
+once you familiarize yourself with the basic patterns (e.g. using S3 to store the plots, leveraging a third-party tool to track experiments).
+
+Once your development setup is working as expected, you can run
+
+.. code-block:: bash
+
+    python evalrs_2023.py
+
+to explore tests on a real-world `dataset <https://github.com/RecList/evalRS-KDD-2023>`__ (make sure the `files <https://github.com/RecList/evalRS-KDD-2023/blob/c1b42ec8cb81562417bbb3c2713d301dc652141d/evaluation/utils.py#L18C11-L18C11>`__ are available in the `examples` folder before you run the script).
+Finally, once you've run successfully the sample scripts, take the guided tour below to learn more about the abstractions and the full capabilities of *RecList*.
+
+A Guided Tour
+-------------
+
+An instance of `RecList <https://github.com/jacopotagliabue/reclist/blob/main/reclist/reclist.py>`__ represents a suite of tests for recommender systems.
+
+As *evalrs_2023.py* shows, we leave users quite a wide range of options: we provide out of the box standard metrics
+in case your dataset is DataFrame-shaped (or you can / wish turn it into such a shape), but don't force you any pattern if you just want to use *RecList*
+for the scaffolding it provides.
+
+For example, the following code only assumes you have a dataset with golden labels, predictions, and metadata (e.g. item features) in the shape of a DataFrame:
+
+.. code-block:: python
+
+    cdf = DFSessionRecList(
+        dataset=df_events,
+        model_name="myDataFrameRandomModel",
+        predictions=df_predictions,
+        y_test=df_dataset,
+        logger=LOGGER.LOCAL,
+        metadata_store= METADATA_STORE.LOCAL,
+        similarity_model=my_sim_model,
+    )
+
+    cdf(verbose=True)
+
+Our library pre-packages standard recSys metrics and important behavioral tests, but it is built with extensibility in mind: you can re-use tests in new suites, or you can write new domain-specific suites and tests.
+Any suite must inherit from the main interface, and then declare its tests as functions decorated with *@rec_test*.
+
+In the example, an instance is created with one slice-based test: the decorator and return type are used to automatically generate a chart.
+
+.. code-block:: python
+
+    class MyRecList(RecList):
+
+        @rec_test(test_type="AccuracyByCountry", display_type=CHART_TYPE.BARS)
+        def accuracy_by_country(self):
+            """
+            Compute the accuracy by country
+
+            NOTE: the accuracy here is just a random number.
+            """
+            from random import randint
+            return {"US": randint(0, 100), "CA": randint(0, 100), "FR": randint(0, 100) }
+
+
+Inheritance is powerful, as we can build new suites by re-using existing ones. Here, we inherit the tests from an existing "parent" list and just add one more to create a new suite:
+
+.. code-block:: python
+
+    class ChildRecList(MyParentRecList):
+
+        @rec_test(test_type='custom_test', display_type=CHART_TYPE.SCALAR)
+        def my_test(self):
+            """
+            Custom test, returning my lucky number as an example
+            """
+            from random import randint
+
+            return { "luck_number": randint(0, 100) }
+
+
+Any model can be tested, as no assumption is made on the model's structure, but only the availability of *predictions*
+and *ground truth*. Once again, while our example leverages a DataFrame-shaped dataset for these entities, you are free to build your own
+RecList instance with any shape you prefer, provided you implement the metrics accordingly (see the `examples/dummy.py` script for an example with different input types).
+
+Once you run a suite of tests, results are dumped automatically and versioned in a folder (local or on S3), structured as follows
+(name of the suite, name of the model, run timestamp):
+
+.. code-block::
+
+    .reclist/
+      myList/
+        myModel/
+          1637357392/
+          1637357404/
+
+If you use *RecList* as part of your standard testings - either for research or production purposes - you can use the JSON report
+for machine-to-machine communication with downstream systems (e.g. you may want to automatically fail the `pipeline <https://github.com/jacopotagliabue/recs-at-resonable-scale>`__  if tests are not passed).
+
+Capabilities
+------------
+
+*RecList* provides a dataset and model agnostic framework to scale up behavioral tests. We provide some suggested abstractions
+based on DataFrames to make existing tests and metrics fully re-usable, but we don't force any pattern on the user. As out-of-the box functionality, the package provides:
+
+* tests and metrics to be used on your own datasets and models;
+
+* automated storage of results, with versioning, both in a local folder or on S3;
+
+* flexible, Python interface to declare tests-as-functions, and annotate them with *display_type* for automated charts;
+
+* pre-built connectors with popular experiment trackers (e.g. Neptune, Comet), and an extensible interface to add your own (see the scripts in the `examples` folder for snippets on how to use third-party trackers);
+
+* reference implementations based on popular data challenges that used RecList: for an example of the "less wrong" latent space metric you can check the song2vec implementation `here <https://github.com/RecList/evalRS-KDD-2023/blob/c1b42ec8cb81562417bbb3c2713d301dc652141d/evaluation/eval.py#L42>`__.
+
+
+Acknowledgments
+---------------
+
+The original authors are:
+
+* Patrick John Chia - `LinkedIn <https://www.linkedin.com/in/patrick-john-chia-b0a34019b/>`__, `GitHub <https://github.com/patrickjohncyh>`__
+* Jacopo Tagliabue - `LinkedIn <https://www.linkedin.com/in/jacopotagliabue/>`__, `GitHub <https://github.com/jacopotagliabue>`__
+* Federico Bianchi - `LinkedIn <https://www.linkedin.com/in/federico-bianchi-3b7998121/>`__, `GitHub <https://github.com/vinid>`__
+* Chloe He - `LinkedIn <https://www.linkedin.com/in/chloe-he//>`__, `GitHub <https://github.com/chloeh13q>`__
+* Brian Ko - `LinkedIn <https://www.linkedin.com/in/briankosw/>`__, `GitHub <https://github.com/briankosw>`__
+
+*RecList* is a community project made possible by the generous support of awesome folks. Between June and December 2022, the development of our beta has been supported by `Comet <https://www.comet.com/>`__, `Neptune <https://neptune.ai/homepage>`__ , `Gantry <https://gantry.io/>`__.
+Our beta has been developed with the help of:
+
+* Unnati Patel - `LinkedIn <https://www.linkedin.com/in/unnati-p-16626610a/>`__
+* Ciro Greco - `LinkedIn <https://www.linkedin.com/in/cirogreco/>`__
+
+If you have questions or feedback, please reach out to: :code:`jacopo dot tagliabue at nyu dot edu`.
+
+License and Citation
+--------------------
+
+All the code is released under an open MIT license. If you found *RecList* useful, please cite our WWW paper:
+
+.. code-block:: bash
+
+    @inproceedings{10.1145/3487553.3524215,
+        author = {Chia, Patrick John and Tagliabue, Jacopo and Bianchi, Federico and He, Chloe and Ko, Brian},
+        title = {Beyond NDCG: Behavioral Testing of Recommender Systems with RecList},
+        year = {2022},
+        isbn = {9781450391306},
+        publisher = {Association for Computing Machinery},
+        address = {New York, NY, USA},
+        url = {https://doi.org/10.1145/3487553.3524215},
+        doi = {10.1145/3487553.3524215},
+        pages = {99–104},
+        numpages = {6},
+        keywords = {recommender systems, open source, behavioral testing},
+        location = {Virtual Event, Lyon, France},
+        series = {WWW '22 Companion}
+    }
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.0 (2021-11-16)
+------------------
+
+* First release on PyPI.
```

### Comparing `reclist-0.3.1/README.rst` & `reclist-2.0.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 =======
 RecList
 =======
 
+.. image:: images/reclist.png
+        :width: 30%
+        :alt: Rocket Emoji
+
 
 .. image:: https://img.shields.io/pypi/v/reclist.svg
         :target: https://pypi.python.org/pypi/reclist
 
 .. image:: https://readthedocs.org/projects/reclist/badge/?version=latest
         :target: https://reclist.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
@@ -26,288 +30,223 @@
         :alt: Downloads
 
 .. image:: https://img.shields.io/badge/youtube-video-red
         :target: https://www.youtube.com/watch?v=cAlJYxFYA04
         :alt: YouTube
 
 
-RecList
-
-
-* Free software: MIT license
-* Documentation: https://reclist.readthedocs.io.
 
 Overview
 --------
 
 *RecList* is an open source library providing behavioral, "black-box" testing for recommender systems. Inspired by the pioneering work of
-`Ribeiro et al. 2020 <https://aclanthology.org/2020.acl-main.442.pdf>`__ in NLP, we introduce a general plug-and-play procedure to scale up behavioral testing,
-with an easy-to-extend interface for custom use cases.
+`Ribeiro et al. 2020 <https://aclanthology.org/2020.acl-main.442.pdf>`__ in NLP, we introduce a general plug-and-play procedure to scale up behavioral testing, with an easy-to-extend interface for custom use cases.
 
 While quantitative metrics over held-out data points are important, a lot more tests are needed for recommenders
 to properly function in the wild and not erode our confidence in them: for example, a model may boast an accuracy improvement over the entire dataset, but actually be significantly worse than another on rare items or new users; or again, a model that correctly recommends HDMI cables as add-on for shoppers buying a TV, may also wrongly  recommend TVs to shoppers just buying a cable.
 
 *RecList* goal is to operationalize these important intuitions into a practical package for testing research and production models in a more nuanced way, without
-requiring unnecessary custom code and ad hoc procedures. To streamline comparisons among existing models, *RecList* ships with popular datasets and ready-made behavioral tests: read the `TDS blog post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__ as a gentle introduction to the main use cases, check the `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__ for more details on the relevant literature.
-
-If you are not familiar with the library, we suggest first taking our small tour to get acquainted with the main abstractions through ready-made models and public datasets.
-
-Quick Links
-~~~~~~~~~~~
-
-* Our `talk <https://www.youtube.com/watch?v=cAlJYxFYA04>`__ at Stitch Fix Algo Hour, for a general presentation.
-* Our `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__, with in-depth analysis, detailed use cases and scholarly references (`arxiv <https://arxiv.org/abs/2111.09963>`__).
-* A `colab notebook <https://colab.research.google.com/drive/1Wn5mm0csEkyWqmBBDxNBkfGR6CNfWeH-?usp=sharing>`__, showing how to train a cart recommender model from scratch and use the library to test it.
-* Our `blog post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__, with examples and practical tips.
-
-
-Supporters
-~~~~~~~~~~
-RecList is a community project made possible by the generous support of these awesome folks. Make sure to check them out!
-
-Comet
-=====
+requiring unnecessary custom code and ad hoc procedures.
 
-.. image:: https://github.com/jacopotagliabue/reclist/raw/main/images/comet.png
-   :target: https://www.comet.com/?utm_source=jacopot&utm_medium=referral&utm_campaign=online_jacopot_2022&utm_content=github_reclist
-   :width: 175
+If you are not familiar with the library, we suggest first taking our small tour to get acquainted with the main abstractions through ready-made models and tests.
 
-Neptune
-=======
-
-.. image:: https://github.com/jacopotagliabue/reclist/raw/main/images/neptune.png
-   :target: https://neptune.ai
-   :width: 175
-
-Gantry
-======
+Colab Tutorials
+~~~~~~~~~~~~~~~
 
-.. image:: https://github.com/jacopotagliabue/reclist/raw/main/images/gantry.png
-   :target: https://gantry.io/
-   :width: 175
 
+.. |colab1_tutorial| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :target: https://colab.research.google.com/drive/1GVsVB1a3H9qbRQvwtb0TBDxq8A5nXc5w?usp=sharing
+    :alt: Open In Colab
+
+.. |colab2_tutorial| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :target: https://colab.research.google.com/drive/1QeXglfCUEcscHB6L0Gch2qDKDDlfwLlq?usp=sharing
+    :alt: Open In Colab
+
+.. |colab3_tutorial| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :target: https://colab.research.google.com/drive/1ek-TIT1ZJta59-O73GaXsOINvt46dnkz?usp=sharing
+    :alt: Open In Colab
+
++--------------------------------------------------------------------------------+------------------+
+| Name                                                                           | Link             |
++================================================================================+==================+
+| Tutorial 101 - Introduction to Reclist                                         | |colab1_tutorial||
++--------------------------------------------------------------------------------+------------------+
+| Tutorial - RecList at EvalRS2023 (KDD)                                         | |colab2_tutorial||
++--------------------------------------------------------------------------------+------------------+
+| Tutorial -  FashionCLIP Evaluation with RecList                                | |colab3_tutorial||
++--------------------------------------------------------------------------------+------------------+
 
-Project updates
-~~~~~~~~~~~~~~~
+Quick Links
+~~~~~~~~~~~
 
-*Community Support*: RecList is an open source community project made possible by the support of the awesome folks at `Comet <https://www.comet.ml/site/>`__, `Neptune <https://neptune.ai/>`__ and `Gantry <https://gantry.io/>`__.
-Soon RecList tests will be natively integrated with the MLOps tools you already know and love!
+* The original `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__ (`arxiv <https://arxiv.org/abs/2111.09963>`__) and initial `release post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__.
+* `EvalRS22@CIKM <https://github.com/RecList/evalRS-CIKM-2022>`__ and `EvalRS23@KDD <https://reclist.io/kdd2023-cup/>`__ , for music recommendations with RecList.
+* A `colab notebook <https://colab.research.google.com/drive/1GVsVB1a3H9qbRQvwtb0TBDxq8A5nXc5w>`__, for a quick interactive tour.
+* Our `website <https://reclist.io/>`__ for past talks and presentations.
 
-*June 2022*: We launched a `website <https://reclist.io/>`__ to collect RecList materials, such as talks and presentations.
-RecList is powering the `Data Challenge <https://reclist.io/cikm2022-cup/>`__ at CIKM 2022: fill `the form <https://docs.google.com/forms/d/e/1FAIpQLSfAypzM1mvd79JfRGRbb9QMfXGMoVYosdjU9C4NFEWNSNUZXQ/viewform>`__ for updates.
 
-In the last few months, we presented this library to practioners at Tubi, eBay, NVIDIA, BBC and other RecSys companies: we are in the process of collecting our thoughts after all the feedback we received, as we plan a beta release for this package in the next few months - come back often for updates, as we will also open a call for collaboration!
+Status
+~~~~~~~~~~~
 
-Please remember that the library is in alpha (i.e. enough working code to finish the paper and tinker with it). We welcome early feedback, but please be advised that the package may change substantially in the near future ("If you're not embarrassed by the first version, you've launched too late").
+* *RecList* is free software released under the MIT license, and it has been adopted by popular `open-source <https://github.com/RecList/evalRS-CIKM-2022>`__  `data challenges <https://reclist.io/kdd2023-cup/>`__.
+* After a major API re-factoring, *RecList* is now in *beta*.
 
 Summary
 ~~~~~~~
 
 This doc is structured as follows:
 
 * `Quick Start`_
 * `A Guided Tour`_
 * `Capabilities`_
-* `Roadmap`_
-* `Talks and Presentations`_
 * `License and Citation`_
 * `Acknowledgments`_
 
 Quick Start
 -----------
 
-If you want to see *RecList* in action, clone the repository, create and activate a virtual env, and install the required packages from pip (you can install from root of course). If you prefer to experiment in an interactive, no-installation-required fashion, try out our `colab notebook <https://colab.research.google.com/drive/1Wn5mm0csEkyWqmBBDxNBkfGR6CNfWeH-?usp=sharing>`__.
-
-Sample scripts are divided by use-cases: similar items, complementary items or session-based recommendations. When executing one, a suitable public dataset will be downloaded, and a baseline model trained: finally, the script will run a pre-made suite of behavioral tests to show typical results.
+You can take a quick tour online using our `colab notebook <https://colab.research.google.com/drive/1GVsVB1a3H9qbRQvwtb0TBDxq8A5nXc5w>`__.
+If you want to use *RecList* locally, clone the repository, create and activate a virtual env, and install the required packages from pip (you can also install from root of course).
 
 .. code-block:: bash
 
     git clone https://github.com/jacopotagliabue/reclist
     cd reclist
     python3 -m venv venv
     source venv/bin/activate
     pip install reclist
-    python examples/coveo_complementary_rec.py
+    cd examples
+    python dummy.py
+
+The sample script will run a suite of tests on a dummy dataset and model, showcasing a typical workflow with the library. Note the commented arguments in the script, which you can use to customize the behavior of the library
+once you familiarize yourself with the basic patterns (e.g. using S3 to store the plots, leveraging a third-party tool to track experiments).
+
+Once your development setup is working as expected, you can run
 
-Running *your* model on one of the supported dataset, leveraging the pre-made tests, is as easy as implementing a simple interface, *RecModel*.
+.. code-block:: bash
+
+    python evalrs_2023.py
 
-Once you've run successfully the sample script, take the guided tour below to learn more about the abstractions and the out-of-the-box capabilities of *RecList*.
+to explore tests on a real-world `dataset <https://github.com/RecList/evalRS-KDD-2023>`__ (make sure the `files <https://github.com/RecList/evalRS-KDD-2023/blob/c1b42ec8cb81562417bbb3c2713d301dc652141d/evaluation/utils.py#L18C11-L18C11>`__ are available in the `examples` folder before you run the script).
+Finally, once you've run successfully the sample scripts, take the guided tour below to learn more about the abstractions and the full capabilities of *RecList*.
 
 A Guided Tour
 -------------
 
-An instance of `RecList <https://github.com/jacopotagliabue/reclist/blob/main/reclist/reclist.py>`__ represents a suite of tests for recommender systems: given
-a dataset (more appropriately, an instance of `RecDataset <https://github.com/jacopotagliabue/reclist/blob/main/reclist/abstractions.py>`__)
-and a model (an instance of `RecModel <https://github.com/jacopotagliabue/reclist/blob/main/reclist/abstractions.py>`__), it will run the specified tests on the target dataset, using the supplied model.
+An instance of `RecList <https://github.com/jacopotagliabue/reclist/blob/main/reclist/reclist.py>`__ represents a suite of tests for recommender systems.
+
+As *evalrs_2023.py* shows, we leave users quite a wide range of options: we provide out of the box standard metrics
+in case your dataset is DataFrame-shaped (or you can / wish turn it into such a shape), but don't force you any pattern if you just want to use *RecList*
+for the scaffolding it provides.
 
-For example, the following code instantiates a pre-made suite of tests that contains sensible defaults for a `cart recommendation use case <https://github.com/jacopotagliabue/reclist/blob/main/reclist/reclist.py>`__:
+For example, the following code only assumes you have a dataset with golden labels, predictions, and metadata (e.g. item features) in the shape of a DataFrame:
 
 .. code-block:: python
 
-    rec_list = CoveoCartRecList(
-        model=model,
-        dataset=coveo_dataset
+    cdf = DFSessionRecList(
+        dataset=df_events,
+        model_name="myDataFrameRandomModel",
+        predictions=df_predictions,
+        y_test=df_dataset,
+        logger=LOGGER.LOCAL,
+        metadata_store= METADATA_STORE.LOCAL,
+        similarity_model=my_sim_model,
     )
-    # invoke rec_list to run tests
-    rec_list(verbose=True)
 
-Our library pre-packages standard recSys KPIs and important behavioral tests, divided by use cases, but it is built with extensibility in mind: you can re-use tests in new suites, or you can write new domain-specific suites and tests.
+    cdf(verbose=True)
 
-Any suite must inherit the *RecList* interface, and then declare with Pytonic decorators its tests. In this case, the test re-uses a standard function:
+Our library pre-packages standard recSys metrics and important behavioral tests, but it is built with extensibility in mind: you can re-use tests in new suites, or you can write new domain-specific suites and tests.
+Any suite must inherit from the main interface, and then declare its tests as functions decorated with *@rec_test*.
+
+In the example, an instance is created with one slice-based test: the decorator and return type are used to automatically generate a chart.
 
 .. code-block:: python
 
     class MyRecList(RecList):
 
-        @rec_test(test_type='stats')
-        def basic_stats(self):
+        @rec_test(test_type="AccuracyByCountry", display_type=CHART_TYPE.BARS)
+        def accuracy_by_country(self):
             """
-            Basic statistics on training, test and prediction data
+            Compute the accuracy by country
+
+            NOTE: the accuracy here is just a random number.
             """
-            from reclist.metrics.standard_metrics import statistics
-            return statistics(self._x_train,
-                self._y_train,
-                self._x_test,
-                self._y_test,
-                self._y_preds)
+            from random import randint
+            return {"US": randint(0, 100), "CA": randint(0, 100), "FR": randint(0, 100) }
 
 
-Any model can be tested, as long as its predictions are wrapped in a *RecModel*. This allows for pure "black-box" testings,
-a SaaS provider can be tested just by wrapping the proper API call in the method:
+Inheritance is powerful, as we can build new suites by re-using existing ones. Here, we inherit the tests from an existing "parent" list and just add one more to create a new suite:
 
 .. code-block:: python
 
-    class MyCartModel(RecModel):
-
-        def __init__(self, **kwargs):
-            super().__init__(**kwargs)
+    class ChildRecList(MyParentRecList):
 
-        def predict(self, prediction_input: list, *args, **kwargs):
+        @rec_test(test_type='custom_test', display_type=CHART_TYPE.SCALAR)
+        def my_test(self):
             """
-            Implement the abstract method, accepting a list of lists, each list being
-            the content of a cart: the predictions returned by the model are the top K
-            items suggested to complete the cart.
+            Custom test, returning my lucky number as an example
             """
+            from random import randint
 
-            return
+            return { "luck_number": randint(0, 100) }
 
-More generally, the logical workflow of a typical RecList implementation is as follows (see our `blog post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__ for a longer explanation):
 
-.. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/workflow.gif
-   :height: 400
+Any model can be tested, as no assumption is made on the model's structure, but only the availability of *predictions*
+and *ground truth*. Once again, while our example leverages a DataFrame-shaped dataset for these entities, you are free to build your own
+RecList instance with any shape you prefer, provided you implement the metrics accordingly (see the `examples/dummy.py` script for an example with different input types).
 
-While many standard KPIs are available in the package, the philosophy behind *RecList* is that metrics like Hit Rate provide only a partial picture
-of the expected behavior of recommenders in the wild: two models with very similar accuracy can have very different behavior on, say, the long-tail, or
-model A can be better than model B overall, but at the expense of providing disastrous performance on a set of inputs that are particularly important in production.
-
-*RecList* recognizes that outside of academic benchmarks, some mistakes are worse than others, and not all inputs are created equal: when possible, it tries
-to operationalize through scalable code behavioral insights for debugging and error analysis; it also
-provides extensible abstractions when domain knowledge and custom logic are needed.
-
-Once you run a suite of tests, results are dumped automatically and versioned in a local folder, structured as follows
+Once you run a suite of tests, results are dumped automatically and versioned in a folder (local or on S3), structured as follows
 (name of the suite, name of the model, run timestamp):
 
 .. code-block::
 
     .reclist/
       myList/
         myModel/
           1637357392/
           1637357404/
 
-If you start using *RecList* as part of your standard testings - either for research or production purposes - you can use the JSON report
-for machine-to-machine communication with downstream system (e.g. you may want to automatically fail the model pipeline if certain behavioral tests are not passed).
-
-Note: our app is deprecated, as RecList Beta will have connectors with existing apps (experiment trackers, model cards, etc.).
+If you use *RecList* as part of your standard testings - either for research or production purposes - you can use the JSON report
+for machine-to-machine communication with downstream systems (e.g. you may want to automatically fail the `pipeline <https://github.com/jacopotagliabue/recs-at-resonable-scale>`__  if tests are not passed).
 
 Capabilities
 ------------
 
-*RecList* provides a dataset and model agnostic framework to scale up behavioral tests. As long as the proper abstractions
-are implemented, all the out-of-the-box components can be re-used. For example:
-
-* you can use a public dataset provided by *RecList* to train your new cart recommender model, and then use the *RecTests* we provide for that use case;
-
-* you can use some baseline model on your custom dataset, to establish a baseline for your project;
-
-* you can use a custom model, on a private dataset and define from scratch a new suite of tests, mixing existing methods and domain-specific tests.
-
-We list below what we currently support out-of-the-box, with particular focus on datasets and tests, as the models we provide
-are convenient baselines, but they are not meant to be SOTA research models.
-
-Datasets
-~~~~~~~~
-
-RecList features convenient wrappers around popular datasets, to help test models over known benchmarks
-in a standardized way.
-
-* `Coveo Data Challenge <https://github.com/coveooss/SIGIR-ecom-data-challenge>`__
-* (a smaller version of) `The Million Playlist Dataset <https://engineering.atspotify.com/2018/05/30/introducing-the-million-playlist-dataset-and-recsys-challenge-2018/>`__
-* (a smaller version of) `MovieLens <https://grouplens.org/datasets/movielens/>`__
-
-Behavioral Tests
-~~~~~~~~~~~~~~~~
-
-RecList helps report standard quantitative metrics over popular (or custom) datasets, such as the ones collected in
-*standard_metrics.py*: hit rate, mrr, coverage, popularity bias, etc. However, RecList raison d'etre is providing plug-and-play
-behavioral tests, as agnostic as possible to the underlying models and datasets, while leaving open the possibility of writing
-personalized tests when domain knowledge and custom logic are necessary.
-
-Tests descriptions are available in our (WIP) `docs <https://reclist.readthedocs.io>`__, but we share here some examples from our `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__.
-
-First, RecList allows to compare the performance of models which may have similar aggregate KPIs (e.g. hit rate on the entire
-test set) in different slices. When plotting HR by product popularity, it is easy to spot that
-prod2vec works much better with rarer items than the alternatives:
-
-.. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/hit_rate_dist.png
-   :height: 175
-
-When slicing by important meta-data (in this simulated example, brands), RecList uncovers significant differences
-in performance for different groups; since the features we care about vary across datasets,
-the package allows for a generic way to partition the test set and compute per-slice metrics:
-
-.. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/slice_dist.png
-   :height: 175
+*RecList* provides a dataset and model agnostic framework to scale up behavioral tests. We provide some suggested abstractions
+based on DataFrames to make existing tests and metrics fully re-usable, but we don't force any pattern on the user. As out-of-the box functionality, the package provides:
 
-Finally, RecList can take advantage of the latent item space to compute the cosine distances <query item, ground truth> and
-<query item, prediction> for missed predictions in the test set. In a cart recommender use case, we expect items to
-reflect the complementary nature of the suggestions: if a TV is in the cart, a model should recommend a HDMI cable,
-not another TV. As we see in the comparison below, Google's predictions better match the label distribution,
-suggesting that the model better capture the nature of the task:
+* tests and metrics to be used on your own datasets and models;
 
-.. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/distance_to_query.png
-   :height: 175
+* automated storage of results, with versioning, both in a local folder or on S3;
 
-Roadmap
--------
+* flexible, Python interface to declare tests-as-functions, and annotate them with *display_type* for automated charts;
 
-We have exciting news about our Beta, including the usage of RecList as main library for the `CIKM Data Challenge <https://reclist.io/cikm2022-cup/>`__!
+* pre-built connectors with popular experiment trackers (e.g. Neptune, Comet), and an extensible interface to add your own (see the scripts in the `examples` folder for snippets on how to use third-party trackers);
 
-Contributing
-~~~~~~~~~~~~
+* reference implementations based on popular data challenges that used RecList: for an example of the "less wrong" latent space metric you can check the song2vec implementation `here <https://github.com/RecList/evalRS-KDD-2023/blob/c1b42ec8cb81562417bbb3c2713d301dc652141d/evaluation/eval.py#L42>`__.
 
-We will update this repo with some guidelines for contributions as soon as the codebase becomes more stable. Check back often for updates!
 
 Acknowledgments
 ---------------
 
 The original authors are:
 
 * Patrick John Chia - `LinkedIn <https://www.linkedin.com/in/patrick-john-chia-b0a34019b/>`__, `GitHub <https://github.com/patrickjohncyh>`__
 * Jacopo Tagliabue - `LinkedIn <https://www.linkedin.com/in/jacopotagliabue/>`__, `GitHub <https://github.com/jacopotagliabue>`__
 * Federico Bianchi - `LinkedIn <https://www.linkedin.com/in/federico-bianchi-3b7998121/>`__, `GitHub <https://github.com/vinid>`__
 * Chloe He - `LinkedIn <https://www.linkedin.com/in/chloe-he//>`__, `GitHub <https://github.com/chloeh13q>`__
 * Brian Ko - `LinkedIn <https://www.linkedin.com/in/briankosw/>`__, `GitHub <https://github.com/briankosw>`__
 
-If you have questions or feedback, please reach out to: :code:`jacopo dot tagliabue at tooso dot ai`.
+*RecList* is a community project made possible by the generous support of awesome folks. Between June and December 2022, the development of our beta has been supported by `Comet <https://www.comet.com/>`__, `Neptune <https://neptune.ai/homepage>`__ , `Gantry <https://gantry.io/>`__.
+Our beta has been developed with the help of:
 
-Talks and Presentations
------------------------
+* Unnati Patel - `LinkedIn <https://www.linkedin.com/in/unnati-p-16626610a/>`__
+* Ciro Greco - `LinkedIn <https://www.linkedin.com/in/cirogreco/>`__
 
-Past and upcoming talks and presentations can be found at our new `website <https://reclist.io/>`__.
+If you have questions or feedback, please reach out to: :code:`jacopo dot tagliabue at nyu dot edu`.
 
 License and Citation
 --------------------
 
 All the code is released under an open MIT license. If you found *RecList* useful, please cite our WWW paper:
 
 .. code-block:: bash
```

### Comparing `reclist-0.3.1/reclist/abstractions.py` & `reclist-2.0.0/reclist/reclist.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,105 +1,33 @@
-
-from datetime import datetime
+import json
 import os
-from abc import ABC, abstractmethod
-from functools import wraps
-from pathlib import Path
 import time
-import json
-from reclist.utils.train_w2v import train_embeddings
-from reclist.current import current
-
-class RecDataset(ABC):
-    """
-    Implements an abstract class for the dataset
-    """
-    def __init__(self, force_download=False):
-        """
-        :param force_download: allows to force the download of the dataset in case it is needed.
-        :type: force_download: bool, optional
-        """
-        self._x_train = None
-        self._y_train = None
-        self._x_test = None
-        self._y_test = None
-        self._catalog = None
-        self.force_download = force_download
-        self.load()
-
-    @abstractmethod
-    def load(self):
-        """
-        Abstract method that should implement dataset loading
-        :return:
-        """
-        return
-
-    @property
-    def x_train(self):
-        return self._x_train
-
-    @property
-    def y_train(self):
-        return self._y_train
-
-    @property
-    def x_test(self):
-        return self._x_test
-
-    @property
-    def y_test(self):
-        return self._y_test
-
-    @property
-    def catalog(self):
-        return self._catalog
-
-
-class RecModel(ABC):
-    """
-    Abstract class for recommendation model
-    """
-
-    def __init__(self, model=None):
-        """
-
-        :param model: a model that can be used in the predict function
-        """
-        self._model = model
-
-    @abstractmethod
-    def predict(self, prediction_input: list, *args, **kwargs):
-        """
-        The predict function should implement the behaviour of the model at inference time.
-
-        :param prediction_input: the input that is used to to do the prediction
-        :param args:
-        :param kwargs:
-        :return:
-        """
-        return NotImplementedError
-
-    @property
-    def model(self):
-        return self._model
-
+from abc import ABC
+from pathlib import Path
+from functools import wraps
+import pandas as pd
+from reclist.charts import CHART_TYPE
+from reclist.logs import LOGGER, logger_factory
+from reclist.metadata import METADATA_STORE, metadata_store_factory
+import datetime
 
-def rec_test(test_type: str):
+def rec_test(test_type: str, display_type: CHART_TYPE = None):
     """
     Rec test decorator
     """
+
     def decorator(f):
         @wraps(f)
         def w(*args, **kwargs):
             return f(*args, **kwargs)
 
         # add attributes to f
         w.is_test = True
         w.test_type = test_type
+        w.display_type = display_type
         try:
             w.test_desc = f.__doc__.lstrip().rstrip()
         except:
             w.test_desc = ""
         try:
             # python 3
             w.name = w.__name__
@@ -108,138 +36,232 @@
             w.name = w.__func__.func_name
         return w
 
     return decorator
 
 
 class RecList(ABC):
-    META_DATA_FOLDER = '.reclist'
 
-    def __init__(self, model: RecModel, dataset: RecDataset, y_preds: list = None):
+    # this is the target metadata folder
+    # it can be overwritten by the user
+    # if an env variable is set
+    META_DATA_FOLDER = os.environ.get("RECLIST_META_DATA_FOLDER", ".reclist")
+
+    def __init__(
+            self,
+            model_name: str,
+            logger: LOGGER = LOGGER.LOCAL,
+            metadata_store: METADATA_STORE = METADATA_STORE.LOCAL,
+            **kwargs,
+            ):
         """
         :param model:
         :param dataset:
-        :param y_preds:
         """
 
         self.name = self.__class__.__name__
+        self.model_name = model_name
         self._rec_tests = self.get_tests()
-        self._x_train = dataset.x_train
-        self._y_train = dataset.y_train
-        self._x_test = dataset.x_test
-        self._y_test = dataset.y_test
-        self._y_preds = y_preds if y_preds else model.predict(dataset.x_test)
-        self.rec_model = model
-        self.product_data = dataset.catalog
         self._test_results = []
-        self._test_data = {}
-        self._dense_repr = {}
-
-        assert len(self._y_test) == len(self._y_preds)
+        self.logger = logger
+        self.logger_service = logger_factory(logger)(**kwargs)
+        # if s3 is used, we need to specify the bucket
+        self.metadata_bucket = kwargs["bucket"] if "bucket" in kwargs else None
+        assert self.metadata_bucket is not None if metadata_store == METADATA_STORE.S3 else True, \
+            "If using S3, you need to specify the bucket"
+        self.metadata_store_service = metadata_store_factory(metadata_store)(**kwargs)
+        self.metadata_store = metadata_store
 
-    def train_dense_repr(self, type_name: str, type_fn):
-        """
-        Train a dense representation over a type of meta-data & store into object
-        """
-        # type_fn: given a SKU returns some type i.e. brand
-        x_train_transformed = [[type_fn(e) for e in session if type_fn(e)] for session in self._x_train]
-        wv = train_embeddings(x_train_transformed)
-        # store a dict
-        self._dense_repr[type_name] = {word: list(wv.get_vector(word)) for word in wv.key_to_index}
+        return
 
     def get_tests(self):
         """
         Helper to extract methods decorated with rec_test
         """
 
         nodes = {}
         for _ in self.__dir__():
-            if not hasattr(self,_):
+            if not hasattr(self, _):
                 continue
             func = getattr(self, _)
-            if hasattr(func, 'is_test'):
+            if hasattr(func, "is_test"):
                 nodes[func.name] = func
 
         return nodes
 
-    def __call__(self, verbose=True, *args, **kwargs):
+    def create_data_store(self):
+        """
+        Each reclist run stores artifacts in
+
+        METADATA_FOLDER/ReclistName/ModelName/RunEpochTimeMs
+        """
         run_epoch_time_ms = round(time.time() * 1000)
-        # create datastore
-        current._report_path = os.path.join(self.META_DATA_FOLDER,
-                                        self.name,
-                                        self.rec_model.__class__.__name__,
-                                        str(run_epoch_time_ms))
-
-        Path(os.path.join(current.report_path, 'artifacts')).mkdir(parents=True, exist_ok=True)
-        Path(os.path.join(current.report_path, 'results')).mkdir(parents=True, exist_ok=True)
-        Path(os.path.join(current.report_path, 'plots')).mkdir(parents=True, exist_ok=True)
+        # specify a bucket as the root of the datastore if using s3
+        bucket = self.metadata_bucket if self.metadata_store == METADATA_STORE.S3 else ''
+        # create datastore path
+        report_path = os.path.join(
+            bucket,
+            self.META_DATA_FOLDER,
+            self.name,
+            self.model_name,
+            str(run_epoch_time_ms),
+        )
+        # create subfolders in the local file system if needed
+        folders = ["artifacts", "results", "plots"]
+        if self.metadata_store == METADATA_STORE.LOCAL:
+            for folder in folders:
+                Path(os.path.join(report_path, folder)).mkdir(
+                    parents=True, exist_ok=True
+                )
+
+        return report_path
+
+    def _display_rich_table(self, table_name: str, results: list):
+        from rich.console import Console
+        from rich.table import Table
+        # build the rich table
+        table = Table(title=table_name)
+        table.add_column("Type", justify="right", style="cyan", no_wrap=True)
+        table.add_column("Description ", style="magenta", no_wrap=False)
+        table.add_column("Result", justify="right", style="green")
+        for result in results:
+            # rich needs strings to display
+            printable_result = None
+            if isinstance(result['result'], float):
+                printable_result = str(round(result['result'], 4))
+            elif isinstance(result['result'], dict):
+                printable_result = json.dumps(result['result'], indent=4)
+            elif isinstance(result['result'], list):
+                printable_result = json.dumps(
+                    result['result'][:3] + ["..."],
+                    indent=4
+                )
+            else:
+                printable_result = str(result['result'])
+            table.add_row(
+                result['name'],
+                result['description'],
+                printable_result
+                )
+        # print out the table
+        console = Console()
+        console.print(table)
+
+        return
+
+    def __call__(self, verbose=True, *args, **kwargs):
+        from rich.progress import track
 
+        self.meta_store_path = self.create_data_store()
         # iterate through tests
-        for test_func_name, test in self._rec_tests.items():
+        for test_func_name, test in track(self._rec_tests.items(), description="Running RecTests"):
             test_result = test(*args, **kwargs)
             # we could store the results in the test function itself
             # test.__func__.test_result = test_result
-            self._test_results.append({
-                'test_name': test.test_type,
-                'description': test.test_desc,
-                'test_result': test_result}
+            self._test_results.append(
+                {
+                    "name": test.test_type,
+                    "description": test.test_desc,
+                    "result": test_result,
+                    "display_type": str(test.display_type),
+                }
             )
-            if verbose:
-                print("============= TEST RESULTS ===============")
-                print("Test Type        : {}".format(test.test_type))
-                print("Test Description : {}".format(test.test_desc))
-                print("Test Result      : {}\n".format(test_result))
-        # at the end, we dump it locally
-        if verbose:
-            print("Generating reports at {}".format(datetime.utcnow()))
-        self.generate_report(run_epoch_time_ms)
+            self.logger_service.write(test.test_type, test_result)
+        # finally, display all results in a table
+        self._display_rich_table(self.name, self._test_results)
+        # at the end, dump results to json and generate plots
+        test_2_fig = self._generate_report_and_plot(self._test_results, self.meta_store_path)
+        for test, fig in test_2_fig.items():
+            self.logger_service.save_plot(name=test, fig=fig)
 
-    def generate_report(self, epoch_time_ms: int):
-        # create path first: META_DATA_FOLDER / RecList / Model / Run Time
-        report_path = os.path.join(
-            self.META_DATA_FOLDER,
-            self.name,
-            self.rec_model.__class__.__name__,
-            str(epoch_time_ms)
-        )
-        # now, dump results
-        self.dump_results_to_json(self._test_results, report_path, epoch_time_ms)
-        # now, store artifacts
-        self.store_artifacts(report_path)
-
-    def store_artifacts(self, report_path: str):
-        target_path = os.path.join(current.report_path, 'artifacts')
-        # store predictions
-        with open(os.path.join(target_path, 'model_predictions.json'), 'w') as f:
-            json.dump({
-                'x_test': self._x_test,
-                'y_test': self._y_test,
-                'y_preds': self._y_preds
-            }, f)
-
-    def dump_results_to_json(self, test_results: list, report_path: str, epoch_time_ms: int):
-        target_path = os.path.join(report_path, 'results')
-        # make sure the folder is there, with all intermediate parents
-        Path(target_path).mkdir(parents=True, exist_ok=True)
+        return
+
+    def _generate_report_and_plot(self, test_results: list, meta_store_path: str):
+        """
+        Store a copy of the results into a file in the metadata store
+
+        TODO: decide what to do with artifacts
+        """
+        # dump results to json
+        report_file_name = self._dump_results_to_json(test_results, meta_store_path)
+        # generate and save plots if applicable
+        test_2_fig = self._generate_plots(test_results)
+        for test_name, fig in test_2_fig.items():
+            if self.metadata_store == METADATA_STORE.LOCAL:
+                # TODO: decide if we want to save the plot in S3 or not
+                fig.savefig(os.path.join(meta_store_path, "plots", "{}.png".format(test_name)))
+        # TODO: decide how store artifacts / if / where
+        # self.store_artifacts(report_path)
+        return test_2_fig
+
+    def _generate_plots(self, test_results: list):
+        test_2_fig = {}
+        for test_result in test_results:
+            display_type = test_result['display_type']
+            fig = None
+            if display_type == str(CHART_TYPE.SCALAR):
+                # TODO: decide how to plot scalars
+                pass
+            elif display_type == str(CHART_TYPE.BARS):
+                fig = self._bar_chart(test_result)
+            elif display_type == str(CHART_TYPE.BINS):
+                fig = self._bin_chart(test_result)
+            # append fig to the mapping
+            if fig is not None:
+                test_2_fig[test_result['name']] = fig
+
+        return test_2_fig
+
+    def _bin_chart(self, test_result: dict):
+        import matplotlib.pyplot as plt
+
+        fig, ax = plt.subplots()
+        ax.set_xlabel('x')
+        ax.set_ylabel('y')
+        ax.set_title(test_result['name'])
+        data = test_result['result']
+        assert isinstance(data, list), "data must be a list"
+        ax.hist(data, color='lightgreen', ec='black')
+
+        return fig
+
+    def _bar_chart(self, test_result: dict):
+        import matplotlib.pyplot as plt
+
+        fig, ax = plt.subplots()
+        ax.set_xlabel('x')
+        ax.set_ylabel('y')
+        ax.set_title(test_result['name'])
+        data = test_result['result'].keys()
+        # cast keys to string; matplotlib requirement
+        ax.bar([str(_) for _ in data], [test_result['result'][_] for _ in data])
+
+        return fig
+
+
+    def _dump_results_to_json(self, test_results: list, report_path: str):
         report = {
-            'metadata': {
-                'run_time': epoch_time_ms,
-                'model_name': self.rec_model.__class__.__name__,
-                'reclist': self.name,
-                'tests': list(self._rec_tests.keys())
+            "metadata": {
+                "finish_time": datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+                "model_name": self.model_name,
+                "reclist": self.name,
+                "tests": list(self._rec_tests.keys()),
             },
-            'data': test_results
+            "data": test_results,
         }
-        with open(os.path.join(target_path, 'report.json'), 'w') as f:
-            json.dump(report, f)
+        report_file_name = os.path.join(report_path, "results", "report.json")
+        self.metadata_store_service.write_file(
+            report_file_name,
+            report,
+            is_json=True
+        )
 
-    @property
-    def test_results(self):
-        return self._test_results
-
-    @property
-    def test_data(self):
-        return self._test_data
+        return report_file_name
 
     @property
     def rec_tests(self):
         return self._rec_tests
+
+
+
+
+
```

### Comparing `reclist-0.3.1/reclist/metrics/distance_metrics.py` & `reclist-2.0.0/reclist/metrics/distance_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,83 @@
-from scipy.spatial.distance import cosine
-import matplotlib.pyplot as plt
-from reclist.current import current
-import os
 import json
-import networkx as nx
-from networkx.algorithms.shortest_paths.generic import shortest_path
+import os
 from statistics import mean
-from reclist.metrics.standard_metrics import sample_misses_at_k, sample_hits_at_k
+
+import matplotlib.pyplot as plt
+import networkx as nx
 import numpy as np
+from networkx.algorithms.shortest_paths.generic import shortest_path
+from scipy.spatial.distance import cosine
+
+from reclist.current import current
+from reclist.metrics.standard_metrics import sample_hits_at_k, sample_misses_at_k
+
+
+def similarity_item(function, item1, item2):
+    return function(item1, item2)
 
 def error_by_cosine_distance(model, y_test, y_preds, k=3, bins=25, debug=False):
-    if not(hasattr(model.__class__, 'get_vector') and callable(getattr(model.__class__, 'get_vector'))):
-        error_msg = "Error : Model {} does not support retrieval of vector embeddings".format(model.__class__)
+    if not (
+        hasattr(model.__class__, "get_vector")
+        and callable(getattr(model.__class__, "get_vector"))
+    ):
+        error_msg = (
+            "Error : Model {} does not support retrieval of vector embeddings".format(
+                model.__class__
+            )
+        )
         print(error_msg)
         return error_msg
     misses = sample_misses_at_k(y_preds, y_test, k=k, size=-1)
     cos_distances = []
     for m in misses:
-        if m['Y_PRED']:
-            vector_test = model.get_vector(m['Y_TEST'][0])
-            vector_pred = model.get_vector(m['Y_PRED'][0])
+        if m["Y_PRED"]:
+            vector_test = model.get_vector(m["Y_TEST"][0])
+            vector_pred = model.get_vector(m["Y_PRED"][0])
             if vector_pred and vector_test:
                 cos_dist = cosine(vector_pred, vector_test)
                 cos_distances.append(cos_dist)
 
     histogram = np.histogram(cos_distances, bins=bins, density=False)
     # cast to list
     histogram = (histogram[0].tolist(), histogram[1].tolist())
     # debug / viz
     if debug:
         plt.hist(cos_distances, bins=bins)
-        plt.title('dist over cosine distance prod space')
-        plt.savefig(os.path.join(current.report_path,
-                                 'plots',
-                                 'distance_to_predictions.png'))
+        plt.title("dist over cosine distance prod space")
+        plt.savefig(
+            os.path.join(current.report_path, "plots", "distance_to_predictions.png")
+        )
         plt.clf()
         # plt.show()
 
-    return {'mean': np.mean(cos_distances), 'histogram': histogram}
+    return {"mean": np.mean(cos_distances), "histogram": histogram}
+
 
 def distance_to_query(model, x_test, y_test, y_preds, k=3, bins=25, debug=False):
-    if not(hasattr(model.__class__, 'get_vector') and callable(getattr(model.__class__, 'get_vector'))):
-        error_msg = "Error : Model {} does not support retrieval of vector embeddings".format(model.__class__)
+    if not (
+        hasattr(model.__class__, "get_vector")
+        and callable(getattr(model.__class__, "get_vector"))
+    ):
+        error_msg = (
+            "Error : Model {} does not support retrieval of vector embeddings".format(
+                model.__class__
+            )
+        )
         print(error_msg)
         return error_msg
     misses = sample_misses_at_k(y_preds, y_test, x_test=x_test, k=k, size=-1)
     x_to_y_cos = []
     x_to_p_cos = []
     for m in misses:
-        if m['Y_PRED']:
-            vector_x = model.get_vector(m['X_TEST'][0])
-            vector_y = model.get_vector(m['Y_TEST'][0])
-            vectors_p = [model.get_vector(_) for _ in m['Y_PRED']]
-            c_dists =[]
+        if m["Y_PRED"]:
+            vector_x = model.get_vector(m["X_TEST"][0])
+            vector_y = model.get_vector(m["Y_TEST"][0])
+            vectors_p = [model.get_vector(_) for _ in m["Y_PRED"]]
+            c_dists = []
             if not vector_x or not vector_y:
                 continue
             x_to_y_cos.append(cosine(vector_x, vector_y))
             for v_p in vectors_p:
                 if not v_p:
                     continue
                 cos_dist = cosine(v_p, vector_x)
@@ -71,109 +92,117 @@
     h_xy = (h_xy[0].tolist(), h_xy[1].tolist())
     h_xp = (h_xp[0].tolist(), h_xp[1].tolist())
 
     # debug / viz
     if debug:
         plt.hist(x_to_y_cos, bins=bins, alpha=0.5)
         plt.hist(x_to_p_cos, bins=bins, alpha=0.5)
-        plt.title('distribution of distance to input')
-        plt.legend(['Distance from Input to Label',
-                    'Distance from Input to Label'],
-                   loc='upper right')
+        plt.title("distribution of distance to input")
+        plt.legend(
+            ["Distance from Input to Label", "Distance from Input to Label"],
+            loc="upper right",
+        )
         # plt.show()
-        plt.savefig(os.path.join(current.report_path,
-                                 'plots',
-                                 'distance_to_query.png'))
+        plt.savefig(os.path.join(current.report_path, "plots", "distance_to_query.png"))
         plt.clf()
 
     return {
-        'histogram_x_to_y': h_xy,
-        'histogram_x_to_p': h_xp,
-        'raw_distances_x_to_y': x_to_y_cos,
-        'raw_distances_x_to_p': x_to_p_cos,
+        "histogram_x_to_y": h_xy,
+        "histogram_x_to_p": h_xp,
+        "raw_distances_x_to_y": x_to_y_cos,
+        "raw_distances_x_to_p": x_to_p_cos,
     }
 
 
-
 def shortest_path_length():
     pass
 
 
-get_nodes = lambda nodes, ancestors="": [] if not nodes else ['_'.join([ancestors, nodes[0]])] + \
-                                                             get_nodes(nodes[1:], '_'.join([ancestors, nodes[0]]))
+get_nodes = (
+    lambda nodes, ancestors="": []
+    if not nodes
+    else ["_".join([ancestors, nodes[0]])]
+    + get_nodes(nodes[1:], "_".join([ancestors, nodes[0]]))
+)
 
 
 def graph_distance_test(y_test, y_preds, product_data, k=3):
     path_lengths = []
     misses = sample_misses_at_k(y_preds, y_test, k=k, size=-1)
-    for _y, _y_p in zip([_['Y_TEST'] for _ in misses],
-                        [_['Y_PRED'] for _ in misses]):
+    for _y, _y_p in zip([_["Y_TEST"] for _ in misses], [_["Y_PRED"] for _ in misses]):
         if not _y_p:
             continue
         _y_sku = _y[0]
         _y_p_sku = _y_p[0]
 
         if _y_sku not in product_data or _y_p_sku not in product_data:
             continue
-        if not product_data[_y_sku]['CATEGORIES'] or not product_data[_y_p_sku]['CATEGORIES']:
+        if (
+            not product_data[_y_sku]["CATEGORIES"]
+            or not product_data[_y_p_sku]["CATEGORIES"]
+        ):
             continue
         # extract graph information
-        catA = json.loads(product_data[_y_sku]['CATEGORIES'])
-        catB = json.loads(product_data[_y_p_sku]['CATEGORIES'])
+        catA = json.loads(product_data[_y_sku]["CATEGORIES"])
+        catB = json.loads(product_data[_y_p_sku]["CATEGORIES"])
         catA_nodes = [get_nodes(c) for c in catA]
         catB_nodes = [get_nodes(c) for c in catB]
         all_nodes = list(set([n for c in catA_nodes + catB_nodes for n in c]))
-        all_edges = [(n1, n2) for c in catA_nodes + catB_nodes for n1, n2 in zip(c[:-1], c[1:])]
+        all_edges = [
+            (n1, n2) for c in catA_nodes + catB_nodes for n1, n2 in zip(c[:-1], c[1:])
+        ]
         all_edges = list(set(all_edges))
 
         # build graph
         G = nx.Graph()
         G.add_nodes_from(all_nodes)
         G.add_edges_from(all_edges)
 
         # get leaves
         cat1_leaves = [c[-1] for c in catA_nodes]
         cat2_leaves = [c[-1] for c in catB_nodes]
 
-        all_paths = [shortest_path(G, c1_l, c2_l) for c1_l in cat1_leaves for c2_l in cat2_leaves]
+        all_paths = [
+            shortest_path(G, c1_l, c2_l) for c1_l in cat1_leaves for c2_l in cat2_leaves
+        ]
         s_path = min(all_paths, key=len)
         s_path_len = len(s_path) - 1
         path_lengths.append(s_path_len)
 
     histogram = np.histogram(path_lengths, bins=np.arange(0, max(path_lengths)))
     histogram = (histogram[0].tolist(), histogram[1].tolist())
-    return {'mean': mean(path_lengths), 'hist': histogram}
-
+    return {"mean": mean(path_lengths), "hist": histogram}
 
 
-def generic_cosine_distance(embeddings: dict,
-                            type_fn,
-                            y_test,
-                            y_preds,
-                            k=10,
-                            bins=25,
-                            debug=False):
+def generic_cosine_distance(
+    embeddings: dict, type_fn, y_test, y_preds, k=10, bins=25, debug=False
+):
 
     misses = sample_misses_at_k(y_preds, y_test, k=k, size=-1)
     cos_distances = []
     for m in misses:
-        if m['Y_TEST'] and m['Y_PRED'] and type_fn(m['Y_TEST'][0]) and type_fn(m['Y_PRED'][0]):
-            vector_test = embeddings.get(type_fn(m['Y_TEST'][0]), None)
-            vector_pred = embeddings.get(type_fn(m['Y_PRED'][0]), None)
+        if (
+            m["Y_TEST"]
+            and m["Y_PRED"]
+            and type_fn(m["Y_TEST"][0])
+            and type_fn(m["Y_PRED"][0])
+        ):
+            vector_test = embeddings.get(type_fn(m["Y_TEST"][0]), None)
+            vector_pred = embeddings.get(type_fn(m["Y_PRED"][0]), None)
             if vector_pred and vector_test:
                 cos_dist = cosine(vector_pred, vector_test)
                 cos_distances.append(cos_dist)
 
     # TODO: Maybe sample some examples from the bins
     histogram = np.histogram(cos_distances, bins=bins, density=False)
     # cast to list
     histogram = (histogram[0].tolist(), histogram[1].tolist())
     # debug / viz
     if debug:
         plt.hist(cos_distances, bins=bins)
-        plt.title('cosine distance misses')
-        plt.savefig(os.path.join(current.report_path,
-                                 'plots',
-                                 'cosine_distance_over_type.png'))
+        plt.title("cosine distance misses")
+        plt.savefig(
+            os.path.join(current.report_path, "plots", "cosine_distance_over_type.png")
+        )
         plt.clf()
 
-    return {'mean': np.mean(cos_distances), 'histogram': histogram}
+    return {"mean": np.mean(cos_distances), "histogram": histogram}
```

### Comparing `reclist-0.3.1/reclist/metrics/hits.py` & `reclist-2.0.0/reclist/metrics/hits.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from collections import Counter, defaultdict
-import numpy as np
 import math
-from reclist.metrics.standard_metrics import hit_rate_at_k, sample_hits_at_k, sample_misses_at_k
-from collections import defaultdict
 import os
+from collections import Counter, defaultdict
+
 import matplotlib.pyplot as plt
+import numpy as np
+
 from reclist.current import current
+from reclist.metrics.standard_metrics import (
+    hit_rate_at_k,
+    sample_hits_at_k,
+    sample_misses_at_k,
+)
 
 
 def hits_distribution_by_rating(y_test, y_preds, debug=False):
     """
     Calculates the distribution of hit-rate across movie ratings in testing data
     """
     hits = defaultdict(int)
@@ -31,26 +36,27 @@
     if debug:
         x_tick_names = list(hits_distribution_by_rating.keys())
         x_tick_idx = list(range(len(x_tick_names)))
         plt.figure(dpi=150)
         plt.bar(
             x_tick_idx,
             [hit_rate for hit_rate in hits_distribution_by_rating.values()],
-            align='center'
+            align="center",
         )
         plt.xticks(
             list(range(len(hits_distribution_by_rating))), x_tick_names, fontsize=10
         )
-        plt.savefig(os.path.join(current.report_path,
-                                'plots',
-                                'hit_distribution_rating.png'))
+        plt.savefig(
+            os.path.join(current.report_path, "plots", "hit_distribution_rating.png")
+        )
         plt.clf()
 
     return hits_distribution_by_rating
 
+
 def roundup(x: int):
     div = 10.0 ** (len(str(x)))
     return int(math.ceil(x / div)) * div
 
 
 def hits_distribution(x_train, x_test, y_test, y_preds, k=3, debug=False):
     # get product interaction frequency
@@ -61,63 +67,70 @@
         # TODO: allow for generic metric
         hit_per_interaction_cnt[_x_cnt].append(hit_rate_at_k([_y_pred], [_y_test], k=k))
     # get max product frequency
     max_cnt = prod_interaction_cnt.most_common(1)[0][1]
     # round up to nearest place
     max_cnt = int(roundup(max_cnt))
     # generate log-bins
-    indices = np.logspace(1, np.log10(max_cnt), num=int(np.log10(max_cnt))).astype(np.int64)
+    indices = np.logspace(1, np.log10(max_cnt), num=int(np.log10(max_cnt))).astype(
+        np.int64
+    )
     indices = np.concatenate(([0], indices))
-    counts_per_bin = [[_ for i in range(low, high) for _ in hit_per_interaction_cnt[i]]
-                      for low, high in zip(indices[:-1], indices[1:])]
+    counts_per_bin = [
+        [_ for i in range(low, high) for _ in hit_per_interaction_cnt[i]]
+        for low, high in zip(indices[:-1], indices[1:])
+    ]
 
     histogram = [np.mean(counts) if counts else 0 for counts in counts_per_bin]
     count = [len(counts) for counts in counts_per_bin]
 
     if debug:
         # debug / visualization
-        plt.bar(indices[1:], histogram, width=-np.diff(indices) / 1.05, align='edge')
-        plt.xscale('log', base=10)
-        plt.title('HIT Distribution Across Product Frequency')
+        plt.bar(indices[1:], histogram, width=-np.diff(indices) / 1.05, align="edge")
+        plt.xscale("log", base=10)
+        plt.title("HIT Distribution Across Product Frequency")
         # plt.show()
-        plt.savefig(os.path.join(current.report_path, 'plots', 'hit_distribution.png'))
+        plt.savefig(os.path.join(current.report_path, "plots", "hit_distribution.png"))
         plt.clf()
 
     return {
-        'histogram': {int(k): v for k, v in zip(indices[1:], histogram)},
-        'counts': {int(k): v for k, v in zip(indices[1:], count)}
+        "histogram": {int(k): v for k, v in zip(indices[1:], histogram)},
+        "counts": {int(k): v for k, v in zip(indices[1:], count)},
     }
 
 
-def hits_distribution_by_slice(slices,
-                               y_test,
-                               y_preds,
-                               k=3,
-                               sample_size=3,
-                               debug=False):
+def hits_distribution_by_slice(
+    slices, y_test, y_preds, k=3, sample_size=3, debug=False
+):
     hit_rate_per_slice = defaultdict(dict)
     for slice_name, slice_idx in slices.items():
         # get predictions for slice
         slice_y_preds = [y_preds[_] for _ in slice_idx]
         # get labels for slice
         slice_y_test = [y_test[_] for _ in slice_idx]
         # TODO: We may want to allow for generic metric to be used here
         slice_hr = hit_rate_at_k(slice_y_preds, slice_y_test, k=k)
         # store results
-        hit_rate_per_slice[slice_name]['hit_rate'] = slice_hr
+        hit_rate_per_slice[slice_name]["hit_rate"] = slice_hr
         # hit_rate_per_slice[slice_name]['hits'] = sample_hits_at_k(slice_y_preds, slice_y_test, k=k, size=sample_size)
         # hit_rate_per_slice[slice_name]['misses'] = sample_misses_at_k(slice_y_preds, slice_y_test, k=k, size=sample_size)
 
     # debug / visualization
     if debug:
         x_tick_names = list(hit_rate_per_slice.keys())
         x_tick_idx = list(range(len(x_tick_names)))
         plt.figure(dpi=150)
-        plt.bar(x_tick_idx, [_['hit_rate'] for _ in hit_rate_per_slice.values()], align='center')
-        plt.xticks(list(range(len(hit_rate_per_slice))), x_tick_names, rotation=45, fontsize=5)
-        plt.savefig(os.path.join(current.report_path,
-                                 'plots',
-                                 'hit_distribution_slice.png'))
+        plt.bar(
+            x_tick_idx,
+            [_["hit_rate"] for _ in hit_rate_per_slice.values()],
+            align="center",
+        )
+        plt.xticks(
+            list(range(len(hit_rate_per_slice))), x_tick_names, rotation=45, fontsize=5
+        )
+        plt.savefig(
+            os.path.join(current.report_path, "plots", "hit_distribution_slice.png")
+        )
         plt.clf()
 
     # cast to normal dict
     return dict(hit_rate_per_slice)
```

### Comparing `reclist-0.3.1/reclist/metrics/perturbation.py` & `reclist-2.0.0/reclist/metrics/perturbation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import numpy as np
 
 
-def session_perturbation_test(model,
-                              x_test,
-                              y_preds,
-                              perturbation_fn,
-                              id_fn,
-                              k):
+def session_perturbation_test(model, x_test, y_preds, perturbation_fn, id_fn, k):
     # generate perturbations
-    perturbed_pairs = [(perturbation_fn(_x), _y_p) for _x, _y_p in zip(x_test, y_preds) if perturbation_fn(_x)]
+    perturbed_pairs = [
+        (perturbation_fn(_x), _y_p)
+        for _x, _y_p in zip(x_test, y_preds)
+        if perturbation_fn(_x)
+    ]
     # extract perturbed x and original y
     x_test_p, y_preds_o = zip(*perturbed_pairs)
     # make new predictions over perturbed inputs
     y_preds_n = model.predict(x_test_p)
     # extract atomic unit for comparison
     y_preds_o, y_preds_n = id_fn(y_preds_o), id_fn(y_preds_n)
     # check for overlapping predictions
```

### Comparing `reclist-0.3.1/reclist/metrics/price_homogeneity.py` & `reclist-2.0.0/reclist/metrics/price_homogeneity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-import numpy as np
-import matplotlib.pyplot as plt
 import os
+
+import matplotlib.pyplot as plt
+import numpy as np
+
 from reclist.current import current
 
-def price_homogeneity_test(y_test, y_preds, product_data, price_sel_fn, bins=25, debug=True):
+
+def price_homogeneity_test(
+    y_test, y_preds, product_data, price_sel_fn, bins=25, debug=True
+):
     """
 
     :param y_test: test data
     :param y_preds: predicted data
     :param product_data: catalog data
     :param bins: bins on which we split the data for the product comparison
     :param debug: shows plots
@@ -23,23 +28,18 @@
         if _y[0] not in product_data or _y_pred[0] not in product_data:
             continue
         _y_info = product_data[_y[0]]
         _y_pred_info = product_data[_y_pred[0]]
         if price_sel_fn(_y_info) and price_sel_fn(_y_pred_info):
             y_item_price = price_sel_fn(_y_info)
             pred_item_price = price_sel_fn(_y_pred_info)
-            price_diff = np.abs(np.log10(pred_item_price/y_item_price))
+            price_diff = np.abs(np.log10(pred_item_price / y_item_price))
             abs_log_price_diff.append(price_diff)
 
     histogram = np.histogram(abs_log_price_diff, bins=bins, density=False)
     histogram = (histogram[0].tolist(), histogram[1].tolist())
     if debug:
         plt.hist(abs_log_price_diff, bins=25)
-        plt.savefig(os.path.join(current.report_path,
-                                 'plots',
-                                 'price_homogeneity.png'))
+        plt.savefig(os.path.join(current.report_path, "plots", "price_homogeneity.png"))
         plt.clf()
 
-    return {
-        'mean': np.mean(abs_log_price_diff),
-        'histogram': histogram
-    }
+    return {"mean": np.mean(abs_log_price_diff), "histogram": histogram}
```

### Comparing `reclist-0.3.1/reclist.egg-info/PKG-INFO` & `reclist-2.0.0/reclist.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,368 +1,309 @@
 Metadata-Version: 2.1
 Name: reclist
-Version: 0.3.1
+Version: 2.0.0
 Summary: RecList
 Home-page: https://github.com/jacopotagliabue/reclist
 Author: RecList
 Author-email: 
 License: MIT license
-Description: =======
-        RecList
-        =======
-        
-        
-        .. image:: https://img.shields.io/pypi/v/reclist.svg
-                :target: https://pypi.python.org/pypi/reclist
-        
-        .. image:: https://readthedocs.org/projects/reclist/badge/?version=latest
-                :target: https://reclist.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/workflows/Python%20package/badge.svg
-                :target: https://github.com/jacopotagliabue/reclist/actions
-        
-        .. image:: https://img.shields.io/github/contributors/jacopotagliabue/reclist
-                :target: https://github.com/jacopotagliabue/reclist/graphs/contributors/
-                :alt: Contributors
-        
-        .. image:: https://img.shields.io/badge/License-MIT-blue.svg
-                :target: https://lbesson.mit-license.org/
-                :alt: License
-        
-        .. image:: https://pepy.tech/badge/reclist
-                :target: https://pepy.tech/project/reclist
-                :alt: Downloads
-        
-        .. image:: https://img.shields.io/badge/youtube-video-red
-                :target: https://www.youtube.com/watch?v=cAlJYxFYA04
-                :alt: YouTube
-        
-        
-        RecList
-        
-        
-        * Free software: MIT license
-        * Documentation: https://reclist.readthedocs.io.
-        
-        Overview
-        --------
-        
-        *RecList* is an open source library providing behavioral, "black-box" testing for recommender systems. Inspired by the pioneering work of
-        `Ribeiro et al. 2020 <https://aclanthology.org/2020.acl-main.442.pdf>`__ in NLP, we introduce a general plug-and-play procedure to scale up behavioral testing,
-        with an easy-to-extend interface for custom use cases.
-        
-        While quantitative metrics over held-out data points are important, a lot more tests are needed for recommenders
-        to properly function in the wild and not erode our confidence in them: for example, a model may boast an accuracy improvement over the entire dataset, but actually be significantly worse than another on rare items or new users; or again, a model that correctly recommends HDMI cables as add-on for shoppers buying a TV, may also wrongly  recommend TVs to shoppers just buying a cable.
-        
-        *RecList* goal is to operationalize these important intuitions into a practical package for testing research and production models in a more nuanced way, without
-        requiring unnecessary custom code and ad hoc procedures. To streamline comparisons among existing models, *RecList* ships with popular datasets and ready-made behavioral tests: read the `TDS blog post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__ as a gentle introduction to the main use cases, check the `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__ for more details on the relevant literature.
-        
-        If you are not familiar with the library, we suggest first taking our small tour to get acquainted with the main abstractions through ready-made models and public datasets.
-        
-        Quick Links
-        ~~~~~~~~~~~
-        
-        * Our `talk <https://www.youtube.com/watch?v=cAlJYxFYA04>`__ at Stitch Fix Algo Hour, for a general presentation.
-        * Our `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__, with in-depth analysis, detailed use cases and scholarly references (`arxiv <https://arxiv.org/abs/2111.09963>`__).
-        * A `colab notebook <https://colab.research.google.com/drive/1Wn5mm0csEkyWqmBBDxNBkfGR6CNfWeH-?usp=sharing>`__, showing how to train a cart recommender model from scratch and use the library to test it.
-        * Our `blog post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__, with examples and practical tips.
-        
-        
-        Supporters
-        ~~~~~~~~~~
-        RecList is a community project made possible by the generous support of these awesome folks. Make sure to check them out!
-        
-        Comet
-        =====
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/raw/main/images/comet.png
-           :target: https://www.comet.com/?utm_source=jacopot&utm_medium=referral&utm_campaign=online_jacopot_2022&utm_content=github_reclist
-           :width: 175
-        
-        Neptune
-        =======
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/raw/main/images/neptune.png
-           :target: https://neptune.ai
-           :width: 175
-        
-        Gantry
-        ======
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/raw/main/images/gantry.png
-           :target: https://gantry.io/
-           :width: 175
-        
-        
-        Project updates
-        ~~~~~~~~~~~~~~~
-        
-        *Community Support*: RecList is an open source community project made possible by the support of the awesome folks at `Comet <https://www.comet.ml/site/>`__, `Neptune <https://neptune.ai/>`__ and `Gantry <https://gantry.io/>`__.
-        Soon RecList tests will be natively integrated with the MLOps tools you already know and love!
-        
-        *June 2022*: We launched a `website <https://reclist.io/>`__ to collect RecList materials, such as talks and presentations.
-        RecList is powering the `Data Challenge <https://reclist.io/cikm2022-cup/>`__ at CIKM 2022: fill `the form <https://docs.google.com/forms/d/e/1FAIpQLSfAypzM1mvd79JfRGRbb9QMfXGMoVYosdjU9C4NFEWNSNUZXQ/viewform>`__ for updates.
-        
-        In the last few months, we presented this library to practioners at Tubi, eBay, NVIDIA, BBC and other RecSys companies: we are in the process of collecting our thoughts after all the feedback we received, as we plan a beta release for this package in the next few months - come back often for updates, as we will also open a call for collaboration!
-        
-        Please remember that the library is in alpha (i.e. enough working code to finish the paper and tinker with it). We welcome early feedback, but please be advised that the package may change substantially in the near future ("If you're not embarrassed by the first version, you've launched too late").
-        
-        Summary
-        ~~~~~~~
-        
-        This doc is structured as follows:
-        
-        * `Quick Start`_
-        * `A Guided Tour`_
-        * `Capabilities`_
-        * `Roadmap`_
-        * `Talks and Presentations`_
-        * `License and Citation`_
-        * `Acknowledgments`_
-        
-        Quick Start
-        -----------
-        
-        If you want to see *RecList* in action, clone the repository, create and activate a virtual env, and install the required packages from pip (you can install from root of course). If you prefer to experiment in an interactive, no-installation-required fashion, try out our `colab notebook <https://colab.research.google.com/drive/1Wn5mm0csEkyWqmBBDxNBkfGR6CNfWeH-?usp=sharing>`__.
-        
-        Sample scripts are divided by use-cases: similar items, complementary items or session-based recommendations. When executing one, a suitable public dataset will be downloaded, and a baseline model trained: finally, the script will run a pre-made suite of behavioral tests to show typical results.
-        
-        .. code-block:: bash
-        
-            git clone https://github.com/jacopotagliabue/reclist
-            cd reclist
-            python3 -m venv venv
-            source venv/bin/activate
-            pip install reclist
-            python examples/coveo_complementary_rec.py
-        
-        Running *your* model on one of the supported dataset, leveraging the pre-made tests, is as easy as implementing a simple interface, *RecModel*.
-        
-        Once you've run successfully the sample script, take the guided tour below to learn more about the abstractions and the out-of-the-box capabilities of *RecList*.
-        
-        A Guided Tour
-        -------------
-        
-        An instance of `RecList <https://github.com/jacopotagliabue/reclist/blob/main/reclist/reclist.py>`__ represents a suite of tests for recommender systems: given
-        a dataset (more appropriately, an instance of `RecDataset <https://github.com/jacopotagliabue/reclist/blob/main/reclist/abstractions.py>`__)
-        and a model (an instance of `RecModel <https://github.com/jacopotagliabue/reclist/blob/main/reclist/abstractions.py>`__), it will run the specified tests on the target dataset, using the supplied model.
-        
-        For example, the following code instantiates a pre-made suite of tests that contains sensible defaults for a `cart recommendation use case <https://github.com/jacopotagliabue/reclist/blob/main/reclist/reclist.py>`__:
-        
-        .. code-block:: python
-        
-            rec_list = CoveoCartRecList(
-                model=model,
-                dataset=coveo_dataset
-            )
-            # invoke rec_list to run tests
-            rec_list(verbose=True)
-        
-        Our library pre-packages standard recSys KPIs and important behavioral tests, divided by use cases, but it is built with extensibility in mind: you can re-use tests in new suites, or you can write new domain-specific suites and tests.
-        
-        Any suite must inherit the *RecList* interface, and then declare with Pytonic decorators its tests. In this case, the test re-uses a standard function:
-        
-        .. code-block:: python
-        
-            class MyRecList(RecList):
-        
-                @rec_test(test_type='stats')
-                def basic_stats(self):
-                    """
-                    Basic statistics on training, test and prediction data
-                    """
-                    from reclist.metrics.standard_metrics import statistics
-                    return statistics(self._x_train,
-                        self._y_train,
-                        self._x_test,
-                        self._y_test,
-                        self._y_preds)
-        
-        
-        Any model can be tested, as long as its predictions are wrapped in a *RecModel*. This allows for pure "black-box" testings,
-        a SaaS provider can be tested just by wrapping the proper API call in the method:
-        
-        .. code-block:: python
-        
-            class MyCartModel(RecModel):
-        
-                def __init__(self, **kwargs):
-                    super().__init__(**kwargs)
-        
-                def predict(self, prediction_input: list, *args, **kwargs):
-                    """
-                    Implement the abstract method, accepting a list of lists, each list being
-                    the content of a cart: the predictions returned by the model are the top K
-                    items suggested to complete the cart.
-                    """
-        
-                    return
-        
-        More generally, the logical workflow of a typical RecList implementation is as follows (see our `blog post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__ for a longer explanation):
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/workflow.gif
-           :height: 400
-        
-        While many standard KPIs are available in the package, the philosophy behind *RecList* is that metrics like Hit Rate provide only a partial picture
-        of the expected behavior of recommenders in the wild: two models with very similar accuracy can have very different behavior on, say, the long-tail, or
-        model A can be better than model B overall, but at the expense of providing disastrous performance on a set of inputs that are particularly important in production.
-        
-        *RecList* recognizes that outside of academic benchmarks, some mistakes are worse than others, and not all inputs are created equal: when possible, it tries
-        to operationalize through scalable code behavioral insights for debugging and error analysis; it also
-        provides extensible abstractions when domain knowledge and custom logic are needed.
-        
-        Once you run a suite of tests, results are dumped automatically and versioned in a local folder, structured as follows
-        (name of the suite, name of the model, run timestamp):
-        
-        .. code-block::
-        
-            .reclist/
-              myList/
-                myModel/
-                  1637357392/
-                  1637357404/
-        
-        If you start using *RecList* as part of your standard testings - either for research or production purposes - you can use the JSON report
-        for machine-to-machine communication with downstream system (e.g. you may want to automatically fail the model pipeline if certain behavioral tests are not passed).
-        
-        Note: our app is deprecated, as RecList Beta will have connectors with existing apps (experiment trackers, model cards, etc.).
-        
-        Capabilities
-        ------------
-        
-        *RecList* provides a dataset and model agnostic framework to scale up behavioral tests. As long as the proper abstractions
-        are implemented, all the out-of-the-box components can be re-used. For example:
-        
-        * you can use a public dataset provided by *RecList* to train your new cart recommender model, and then use the *RecTests* we provide for that use case;
-        
-        * you can use some baseline model on your custom dataset, to establish a baseline for your project;
-        
-        * you can use a custom model, on a private dataset and define from scratch a new suite of tests, mixing existing methods and domain-specific tests.
-        
-        We list below what we currently support out-of-the-box, with particular focus on datasets and tests, as the models we provide
-        are convenient baselines, but they are not meant to be SOTA research models.
-        
-        Datasets
-        ~~~~~~~~
-        
-        RecList features convenient wrappers around popular datasets, to help test models over known benchmarks
-        in a standardized way.
-        
-        * `Coveo Data Challenge <https://github.com/coveooss/SIGIR-ecom-data-challenge>`__
-        * (a smaller version of) `The Million Playlist Dataset <https://engineering.atspotify.com/2018/05/30/introducing-the-million-playlist-dataset-and-recsys-challenge-2018/>`__
-        * (a smaller version of) `MovieLens <https://grouplens.org/datasets/movielens/>`__
-        
-        Behavioral Tests
-        ~~~~~~~~~~~~~~~~
-        
-        RecList helps report standard quantitative metrics over popular (or custom) datasets, such as the ones collected in
-        *standard_metrics.py*: hit rate, mrr, coverage, popularity bias, etc. However, RecList raison d'etre is providing plug-and-play
-        behavioral tests, as agnostic as possible to the underlying models and datasets, while leaving open the possibility of writing
-        personalized tests when domain knowledge and custom logic are necessary.
-        
-        Tests descriptions are available in our (WIP) `docs <https://reclist.readthedocs.io>`__, but we share here some examples from our `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__.
-        
-        First, RecList allows to compare the performance of models which may have similar aggregate KPIs (e.g. hit rate on the entire
-        test set) in different slices. When plotting HR by product popularity, it is easy to spot that
-        prod2vec works much better with rarer items than the alternatives:
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/hit_rate_dist.png
-           :height: 175
-        
-        When slicing by important meta-data (in this simulated example, brands), RecList uncovers significant differences
-        in performance for different groups; since the features we care about vary across datasets,
-        the package allows for a generic way to partition the test set and compute per-slice metrics:
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/slice_dist.png
-           :height: 175
-        
-        Finally, RecList can take advantage of the latent item space to compute the cosine distances <query item, ground truth> and
-        <query item, prediction> for missed predictions in the test set. In a cart recommender use case, we expect items to
-        reflect the complementary nature of the suggestions: if a TV is in the cart, a model should recommend a HDMI cable,
-        not another TV. As we see in the comparison below, Google's predictions better match the label distribution,
-        suggesting that the model better capture the nature of the task:
-        
-        .. image:: https://github.com/jacopotagliabue/reclist/blob/main/images/distance_to_query.png
-           :height: 175
-        
-        Roadmap
-        -------
-        
-        We have exciting news about our Beta, including the usage of RecList as main library for the `CIKM Data Challenge <https://reclist.io/cikm2022-cup/>`__!
-        
-        Contributing
-        ~~~~~~~~~~~~
-        
-        We will update this repo with some guidelines for contributions as soon as the codebase becomes more stable. Check back often for updates!
-        
-        Acknowledgments
-        ---------------
-        
-        The original authors are:
-        
-        * Patrick John Chia - `LinkedIn <https://www.linkedin.com/in/patrick-john-chia-b0a34019b/>`__, `GitHub <https://github.com/patrickjohncyh>`__
-        * Jacopo Tagliabue - `LinkedIn <https://www.linkedin.com/in/jacopotagliabue/>`__, `GitHub <https://github.com/jacopotagliabue>`__
-        * Federico Bianchi - `LinkedIn <https://www.linkedin.com/in/federico-bianchi-3b7998121/>`__, `GitHub <https://github.com/vinid>`__
-        * Chloe He - `LinkedIn <https://www.linkedin.com/in/chloe-he//>`__, `GitHub <https://github.com/chloeh13q>`__
-        * Brian Ko - `LinkedIn <https://www.linkedin.com/in/briankosw/>`__, `GitHub <https://github.com/briankosw>`__
-        
-        If you have questions or feedback, please reach out to: :code:`jacopo dot tagliabue at tooso dot ai`.
-        
-        Talks and Presentations
-        -----------------------
-        
-        Past and upcoming talks and presentations can be found at our new `website <https://reclist.io/>`__.
-        
-        License and Citation
-        --------------------
-        
-        All the code is released under an open MIT license. If you found *RecList* useful, please cite our WWW paper:
-        
-        .. code-block:: bash
-        
-            @inproceedings{10.1145/3487553.3524215,
-                author = {Chia, Patrick John and Tagliabue, Jacopo and Bianchi, Federico and He, Chloe and Ko, Brian},
-                title = {Beyond NDCG: Behavioral Testing of Recommender Systems with RecList},
-                year = {2022},
-                isbn = {9781450391306},
-                publisher = {Association for Computing Machinery},
-                address = {New York, NY, USA},
-                url = {https://doi.org/10.1145/3487553.3524215},
-                doi = {10.1145/3487553.3524215},
-                pages = {99–104},
-                numpages = {6},
-                keywords = {recommender systems, open source, behavioral testing},
-                location = {Virtual Event, Lyon, France},
-                series = {WWW '22 Companion}
-            }
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2021-11-16)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: reclist
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=======
+RecList
+=======
+
+.. image:: images/reclist.png
+        :width: 30%
+        :alt: Rocket Emoji
+
+
+.. image:: https://img.shields.io/pypi/v/reclist.svg
+        :target: https://pypi.python.org/pypi/reclist
+
+.. image:: https://readthedocs.org/projects/reclist/badge/?version=latest
+        :target: https://reclist.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+.. image:: https://github.com/jacopotagliabue/reclist/workflows/Python%20package/badge.svg
+        :target: https://github.com/jacopotagliabue/reclist/actions
+
+.. image:: https://img.shields.io/github/contributors/jacopotagliabue/reclist
+        :target: https://github.com/jacopotagliabue/reclist/graphs/contributors/
+        :alt: Contributors
+
+.. image:: https://img.shields.io/badge/License-MIT-blue.svg
+        :target: https://lbesson.mit-license.org/
+        :alt: License
+
+.. image:: https://pepy.tech/badge/reclist
+        :target: https://pepy.tech/project/reclist
+        :alt: Downloads
+
+.. image:: https://img.shields.io/badge/youtube-video-red
+        :target: https://www.youtube.com/watch?v=cAlJYxFYA04
+        :alt: YouTube
+
+
+
+Overview
+--------
+
+*RecList* is an open source library providing behavioral, "black-box" testing for recommender systems. Inspired by the pioneering work of
+`Ribeiro et al. 2020 <https://aclanthology.org/2020.acl-main.442.pdf>`__ in NLP, we introduce a general plug-and-play procedure to scale up behavioral testing, with an easy-to-extend interface for custom use cases.
+
+While quantitative metrics over held-out data points are important, a lot more tests are needed for recommenders
+to properly function in the wild and not erode our confidence in them: for example, a model may boast an accuracy improvement over the entire dataset, but actually be significantly worse than another on rare items or new users; or again, a model that correctly recommends HDMI cables as add-on for shoppers buying a TV, may also wrongly  recommend TVs to shoppers just buying a cable.
+
+*RecList* goal is to operationalize these important intuitions into a practical package for testing research and production models in a more nuanced way, without
+requiring unnecessary custom code and ad hoc procedures.
+
+If you are not familiar with the library, we suggest first taking our small tour to get acquainted with the main abstractions through ready-made models and tests.
+
+Colab Tutorials
+~~~~~~~~~~~~~~~
+
+
+.. |colab1_tutorial| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :target: https://colab.research.google.com/drive/1GVsVB1a3H9qbRQvwtb0TBDxq8A5nXc5w?usp=sharing
+    :alt: Open In Colab
+
+.. |colab2_tutorial| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :target: https://colab.research.google.com/drive/1QeXglfCUEcscHB6L0Gch2qDKDDlfwLlq?usp=sharing
+    :alt: Open In Colab
+
+.. |colab3_tutorial| image:: https://colab.research.google.com/assets/colab-badge.svg
+    :target: https://colab.research.google.com/drive/1ek-TIT1ZJta59-O73GaXsOINvt46dnkz?usp=sharing
+    :alt: Open In Colab
+
++--------------------------------------------------------------------------------+------------------+
+| Name                                                                           | Link             |
++================================================================================+==================+
+| Tutorial 101 - Introduction to Reclist                                         | |colab1_tutorial||
++--------------------------------------------------------------------------------+------------------+
+| Tutorial - RecList at EvalRS2023 (KDD)                                         | |colab2_tutorial||
++--------------------------------------------------------------------------------+------------------+
+| Tutorial -  FashionCLIP Evaluation with RecList                                | |colab3_tutorial||
++--------------------------------------------------------------------------------+------------------+
+
+Quick Links
+~~~~~~~~~~~
+
+* The original `paper <https://dl.acm.org/doi/abs/10.1145/3487553.3524215>`__ (`arxiv <https://arxiv.org/abs/2111.09963>`__) and initial `release post <https://towardsdatascience.com/ndcg-is-not-all-you-need-24eb6d2f1227>`__.
+* `EvalRS22@CIKM <https://github.com/RecList/evalRS-CIKM-2022>`__ and `EvalRS23@KDD <https://reclist.io/kdd2023-cup/>`__ , for music recommendations with RecList.
+* A `colab notebook <https://colab.research.google.com/drive/1GVsVB1a3H9qbRQvwtb0TBDxq8A5nXc5w>`__, for a quick interactive tour.
+* Our `website <https://reclist.io/>`__ for past talks and presentations.
+
+
+Status
+~~~~~~~~~~~
+
+* *RecList* is free software released under the MIT license, and it has been adopted by popular `open-source <https://github.com/RecList/evalRS-CIKM-2022>`__  `data challenges <https://reclist.io/kdd2023-cup/>`__.
+* After a major API re-factoring, *RecList* is now in *beta*.
+
+Summary
+~~~~~~~
+
+This doc is structured as follows:
+
+* `Quick Start`_
+* `A Guided Tour`_
+* `Capabilities`_
+* `License and Citation`_
+* `Acknowledgments`_
+
+Quick Start
+-----------
+
+You can take a quick tour online using our `colab notebook <https://colab.research.google.com/drive/1GVsVB1a3H9qbRQvwtb0TBDxq8A5nXc5w>`__.
+If you want to use *RecList* locally, clone the repository, create and activate a virtual env, and install the required packages from pip (you can also install from root of course).
+
+.. code-block:: bash
+
+    git clone https://github.com/jacopotagliabue/reclist
+    cd reclist
+    python3 -m venv venv
+    source venv/bin/activate
+    pip install reclist
+    cd examples
+    python dummy.py
+
+The sample script will run a suite of tests on a dummy dataset and model, showcasing a typical workflow with the library. Note the commented arguments in the script, which you can use to customize the behavior of the library
+once you familiarize yourself with the basic patterns (e.g. using S3 to store the plots, leveraging a third-party tool to track experiments).
+
+Once your development setup is working as expected, you can run
+
+.. code-block:: bash
+
+    python evalrs_2023.py
+
+to explore tests on a real-world `dataset <https://github.com/RecList/evalRS-KDD-2023>`__ (make sure the `files <https://github.com/RecList/evalRS-KDD-2023/blob/c1b42ec8cb81562417bbb3c2713d301dc652141d/evaluation/utils.py#L18C11-L18C11>`__ are available in the `examples` folder before you run the script).
+Finally, once you've run successfully the sample scripts, take the guided tour below to learn more about the abstractions and the full capabilities of *RecList*.
+
+A Guided Tour
+-------------
+
+An instance of `RecList <https://github.com/jacopotagliabue/reclist/blob/main/reclist/reclist.py>`__ represents a suite of tests for recommender systems.
+
+As *evalrs_2023.py* shows, we leave users quite a wide range of options: we provide out of the box standard metrics
+in case your dataset is DataFrame-shaped (or you can / wish turn it into such a shape), but don't force you any pattern if you just want to use *RecList*
+for the scaffolding it provides.
+
+For example, the following code only assumes you have a dataset with golden labels, predictions, and metadata (e.g. item features) in the shape of a DataFrame:
+
+.. code-block:: python
+
+    cdf = DFSessionRecList(
+        dataset=df_events,
+        model_name="myDataFrameRandomModel",
+        predictions=df_predictions,
+        y_test=df_dataset,
+        logger=LOGGER.LOCAL,
+        metadata_store= METADATA_STORE.LOCAL,
+        similarity_model=my_sim_model,
+    )
+
+    cdf(verbose=True)
+
+Our library pre-packages standard recSys metrics and important behavioral tests, but it is built with extensibility in mind: you can re-use tests in new suites, or you can write new domain-specific suites and tests.
+Any suite must inherit from the main interface, and then declare its tests as functions decorated with *@rec_test*.
+
+In the example, an instance is created with one slice-based test: the decorator and return type are used to automatically generate a chart.
+
+.. code-block:: python
+
+    class MyRecList(RecList):
+
+        @rec_test(test_type="AccuracyByCountry", display_type=CHART_TYPE.BARS)
+        def accuracy_by_country(self):
+            """
+            Compute the accuracy by country
+
+            NOTE: the accuracy here is just a random number.
+            """
+            from random import randint
+            return {"US": randint(0, 100), "CA": randint(0, 100), "FR": randint(0, 100) }
+
+
+Inheritance is powerful, as we can build new suites by re-using existing ones. Here, we inherit the tests from an existing "parent" list and just add one more to create a new suite:
+
+.. code-block:: python
+
+    class ChildRecList(MyParentRecList):
+
+        @rec_test(test_type='custom_test', display_type=CHART_TYPE.SCALAR)
+        def my_test(self):
+            """
+            Custom test, returning my lucky number as an example
+            """
+            from random import randint
+
+            return { "luck_number": randint(0, 100) }
+
+
+Any model can be tested, as no assumption is made on the model's structure, but only the availability of *predictions*
+and *ground truth*. Once again, while our example leverages a DataFrame-shaped dataset for these entities, you are free to build your own
+RecList instance with any shape you prefer, provided you implement the metrics accordingly (see the `examples/dummy.py` script for an example with different input types).
+
+Once you run a suite of tests, results are dumped automatically and versioned in a folder (local or on S3), structured as follows
+(name of the suite, name of the model, run timestamp):
+
+.. code-block::
+
+    .reclist/
+      myList/
+        myModel/
+          1637357392/
+          1637357404/
+
+If you use *RecList* as part of your standard testings - either for research or production purposes - you can use the JSON report
+for machine-to-machine communication with downstream systems (e.g. you may want to automatically fail the `pipeline <https://github.com/jacopotagliabue/recs-at-resonable-scale>`__  if tests are not passed).
+
+Capabilities
+------------
+
+*RecList* provides a dataset and model agnostic framework to scale up behavioral tests. We provide some suggested abstractions
+based on DataFrames to make existing tests and metrics fully re-usable, but we don't force any pattern on the user. As out-of-the box functionality, the package provides:
+
+* tests and metrics to be used on your own datasets and models;
+
+* automated storage of results, with versioning, both in a local folder or on S3;
+
+* flexible, Python interface to declare tests-as-functions, and annotate them with *display_type* for automated charts;
+
+* pre-built connectors with popular experiment trackers (e.g. Neptune, Comet), and an extensible interface to add your own (see the scripts in the `examples` folder for snippets on how to use third-party trackers);
+
+* reference implementations based on popular data challenges that used RecList: for an example of the "less wrong" latent space metric you can check the song2vec implementation `here <https://github.com/RecList/evalRS-KDD-2023/blob/c1b42ec8cb81562417bbb3c2713d301dc652141d/evaluation/eval.py#L42>`__.
+
+
+Acknowledgments
+---------------
+
+The original authors are:
+
+* Patrick John Chia - `LinkedIn <https://www.linkedin.com/in/patrick-john-chia-b0a34019b/>`__, `GitHub <https://github.com/patrickjohncyh>`__
+* Jacopo Tagliabue - `LinkedIn <https://www.linkedin.com/in/jacopotagliabue/>`__, `GitHub <https://github.com/jacopotagliabue>`__
+* Federico Bianchi - `LinkedIn <https://www.linkedin.com/in/federico-bianchi-3b7998121/>`__, `GitHub <https://github.com/vinid>`__
+* Chloe He - `LinkedIn <https://www.linkedin.com/in/chloe-he//>`__, `GitHub <https://github.com/chloeh13q>`__
+* Brian Ko - `LinkedIn <https://www.linkedin.com/in/briankosw/>`__, `GitHub <https://github.com/briankosw>`__
+
+*RecList* is a community project made possible by the generous support of awesome folks. Between June and December 2022, the development of our beta has been supported by `Comet <https://www.comet.com/>`__, `Neptune <https://neptune.ai/homepage>`__ , `Gantry <https://gantry.io/>`__.
+Our beta has been developed with the help of:
+
+* Unnati Patel - `LinkedIn <https://www.linkedin.com/in/unnati-p-16626610a/>`__
+* Ciro Greco - `LinkedIn <https://www.linkedin.com/in/cirogreco/>`__
+
+If you have questions or feedback, please reach out to: :code:`jacopo dot tagliabue at nyu dot edu`.
+
+License and Citation
+--------------------
+
+All the code is released under an open MIT license. If you found *RecList* useful, please cite our WWW paper:
+
+.. code-block:: bash
+
+    @inproceedings{10.1145/3487553.3524215,
+        author = {Chia, Patrick John and Tagliabue, Jacopo and Bianchi, Federico and He, Chloe and Ko, Brian},
+        title = {Beyond NDCG: Behavioral Testing of Recommender Systems with RecList},
+        year = {2022},
+        isbn = {9781450391306},
+        publisher = {Association for Computing Machinery},
+        address = {New York, NY, USA},
+        url = {https://doi.org/10.1145/3487553.3524215},
+        doi = {10.1145/3487553.3524215},
+        pages = {99–104},
+        numpages = {6},
+        keywords = {recommender systems, open source, behavioral testing},
+        location = {Virtual Event, Lyon, France},
+        series = {WWW '22 Companion}
+    }
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.0 (2021-11-16)
+------------------
+
+* First release on PyPI.
```

### Comparing `reclist-0.3.1/setup.py` & `reclist-2.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
-with open('README.rst') as readme_file:
+with open("README.rst") as readme_file:
     readme = readme_file.read()
 
-with open('HISTORY.rst') as history_file:
+with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-with open('requirements.txt') as f:
+with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-setup_requirements = ['pytest-runner', ]
-
-test_requirements = ['pytest>=3', ]
+setup_requirements = [
+    "pytest-runner",
+]
+
+test_requirements = [
+    "pytest>=3",
+]
+
+style_packages = [
+    "black==22.3.0",
+    # "flake8==5.0.4",
+    "isort==5.10.1",
+]
 
 setup(
+
     author="RecList",
     author_email='',
     python_requires='>=3.6',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
     ],
     description="RecList",
     install_requires=requirements,
     license="MIT license",
-    long_description=readme + '\n\n' + history,
-    long_description_content_type='text/x-rst',
+    long_description=readme + "\n\n" + history,
+    long_description_content_type="text/x-rst",
     include_package_data=True,
-    keywords='reclist',
-    name='reclist',
-    packages=find_packages(include=['reclist', 'reclist.*']),
-    test_suite='tests',
+    keywords="reclist",
+    name="reclist",
+    packages=find_packages(include=["reclist", "reclist.*"]),
+    test_suite="tests",
     tests_require=test_requirements,
+
     url='https://github.com/jacopotagliabue/reclist',
-    version='0.3.1',
+    version='2.0.0',
     zip_safe=False,
+    extras_require={
+        "dev": style_packages + ["pre-commit==2.20.0"],
+    },
 )
```

