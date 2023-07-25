# Comparing `tmp/tesla-ce-provider-fr-tfr-0.0.6.tar.gz` & `tmp/tesla-ce-provider-fr-tfr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesla-ce-provider-fr-tfr-0.0.6.tar", last modified: Wed Oct  6 19:34:56 2021, max compression
+gzip compressed data, was "tesla-ce-provider-fr-tfr-0.0.7.tar", last modified: Tue Jul 25 13:31:29 2023, max compression
```

## Comparing `tesla-ce-provider-fr-tfr-0.0.6.tar` & `tesla-ce-provider-fr-tfr-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 19:34:56.576009 tesla-ce-provider-fr-tfr-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2021-10-06 19:34:56.576009 tesla-ce-provider-fr-tfr-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-06 19:34:56.576009 tesla-ce-provider-fr-tfr-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 19:34:56.576009 tesla-ce-provider-fr-tfr-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 19:34:56.576009 tesla-ce-provider-fr-tfr-0.0.6/src/tesla_ce_provider_fr_tfr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2021-10-06 19:34:56.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tesla_ce_provider_fr_tfr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-10-06 19:34:56.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tesla_ce_provider_fr_tfr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-06 19:34:56.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tesla_ce_provider_fr_tfr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-10-06 19:34:56.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tesla_ce_provider_fr_tfr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-10-06 19:34:56.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tesla_ce_provider_fr_tfr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 19:34:56.576009 tesla-ce-provider-fr-tfr-0.0.6/src/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      778 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tests/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4828 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)    11254 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tests/test_verification.py
--rw-r--r--   0 runner    (1001) docker     (121)     4037 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tests/tfr_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 19:34:56.576009 tesla-ce-provider-fr-tfr-0.0.6/src/tfr/
--rw-r--r--   0 runner    (1001) docker     (121)      846 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tfr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 19:34:56.576009 tesla-ce-provider-fr-tfr-0.0.6/src/tfr/data/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-10-06 19:34:56.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tfr/data/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      956 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tfr/data/options.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-06 19:34:56.576009 tesla-ce-provider-fr-tfr-0.0.6/src/tfr/provider/
--rw-r--r--   0 runner    (1001) docker     (121)      840 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tfr/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tfr/provider/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    13862 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tfr/provider/tfr.py
--rw-r--r--   0 runner    (1001) docker     (121)     5212 2021-10-06 19:34:49.000000 tesla-ce-provider-fr-tfr-0.0.6/src/tfr/provider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.237404 tesla-ce-provider-fr-tfr-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-25 13:31:29.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-25 13:31:29.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 13:31:29.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 13:31:29.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 13:31:29.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-25 13:31:19.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tests/tfr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 13:31:28.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/data/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/data/options.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 13:31:29.241404 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/tfr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-25 13:31:20.000000 tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/utils.py
```

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/LICENSE` & `tesla-ce-provider-fr-tfr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/PKG-INFO` & `tesla-ce-provider-fr-tfr-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: tesla-ce-provider-fr-tfr
-Version: 0.0.6
+Version: 0.0.7
 Summary: TeSLA CE Face Recognition Provider
 Home-page: https://tesla-ce.github.io
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/provider-fr-tfr/
 Project-URL: Source, https://github.com/tesla-ce/provider-fr-tfr
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-fr-tfr.svg)](https://pypi.python.org/pypi/tesla-ce-provider-fr-tfr/)
-        [![codecov](https://codecov.io/gh/tesla-ce/provider-fr-tfr/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-fr-tfr)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr?ref=badge_shield)
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-fr-tfr)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-fr-tfr)
-        # TFR: TeSLA CE Face Recognition provider 
-        
-        | :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
-        | --- |
-        
-        ## Description
-        Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
-        
-        ## Installation
-        Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
-        
-        ## Usage
-        Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
-        
-        ## Contributing
-        Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
-        
-        ## Credits
-        Credits: Include a section for credits in order to highlight and link to the authors of your project.
-        
-        ## License
-        This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
-        
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr?ref=badge_large)
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-fr-tfr.svg)](https://pypi.python.org/pypi/tesla-ce-provider-fr-tfr/)
+[![codecov](https://codecov.io/gh/tesla-ce/provider-fr-tfr/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-fr-tfr)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr?ref=badge_shield)
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-fr-tfr)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-fr-tfr)
+# TFR: TeSLA CE Face Recognition provider 
+
+| :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
+| --- |
+
+## Description
+Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
+
+## Installation
+Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
+
+## Usage
+Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
+
+## Contributing
+Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
+
+## Credits
+Credits: Include a section for credits in order to highlight and link to the authors of your project.
+
+## License
+This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
+
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr?ref=badge_large)
+
+
```

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/README.md` & `tesla-ce-provider-fr-tfr-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/setup.py` & `tesla-ce-provider-fr-tfr-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tesla_ce_provider_fr_tfr.egg-info/PKG-INFO` & `tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: tesla-ce-provider-fr-tfr
-Version: 0.0.6
+Version: 0.0.7
 Summary: TeSLA CE Face Recognition Provider
 Home-page: https://tesla-ce.github.io
 Author: Xavier Baro
 Author-email: xbaro@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/provider-fr-tfr/
 Project-URL: Source, https://github.com/tesla-ce/provider-fr-tfr
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-fr-tfr.svg)](https://pypi.python.org/pypi/tesla-ce-provider-fr-tfr/)
-        [![codecov](https://codecov.io/gh/tesla-ce/provider-fr-tfr/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-fr-tfr)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr?ref=badge_shield)
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-fr-tfr)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-fr-tfr)
-        # TFR: TeSLA CE Face Recognition provider 
-        
-        | :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
-        | --- |
-        
-        ## Description
-        Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
-        
-        ## Installation
-        Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
-        
-        ## Usage
-        Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
-        
-        ## Contributing
-        Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
-        
-        ## Credits
-        Credits: Include a section for credits in order to highlight and link to the authors of your project.
-        
-        ## License
-        This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
-        
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr?ref=badge_large)
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-fr-tfr.svg)](https://pypi.python.org/pypi/tesla-ce-provider-fr-tfr/)
+[![codecov](https://codecov.io/gh/tesla-ce/provider-fr-tfr/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-fr-tfr)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr?ref=badge_shield)
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-fr-tfr)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-fr-tfr)
+# TFR: TeSLA CE Face Recognition provider 
+
+| :warning: This repository is **under construction**. Final release of TeSLA Community Edition source code is expected by the **end of 2021** |
+| --- |
+
+## Description
+Description: A description of your project follows. A good description is clear, short, and to the point. Describe the importance of your project, and what it does.
+
+## Installation
+Installation: Installation is the next section in an effective README. Tell other users how to install your project locally. Optionally, include a gif to make the process even more clear for other people.
+
+## Usage
+Usage: The next section is usage, in which you instruct other people on how to use your project after they’ve installed it. This would also be a good place to include screenshots of your project in action.
+
+## Contributing
+Contributing: Larger projects often have sections on contributing to their project, in which contribution instructions are outlined. Sometimes, this is a separate file. If you have specific contribution preferences, explain them so that other developers know how to best contribute to your work. To learn more about how to help others contribute, check out the guide for setting guidelines for repository contributors.
+
+## Credits
+Credits: Include a section for credits in order to highlight and link to the authors of your project.
+
+## License
+This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
+
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-fr-tfr?ref=badge_large)
+
+
```

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tesla_ce_provider_fr_tfr.egg-info/SOURCES.txt` & `tesla-ce-provider-fr-tfr-0.0.7/src/tesla_ce_provider_fr_tfr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tests/__init__.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tests/conftest.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tests/test_notification.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_notification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tests/test_utils.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tests/test_validation.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tests/test_verification.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tests/test_verification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tests/tfr_utils.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tests/tfr_utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tfr/__init__.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tfr/data/options.json` & `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/data/options.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.0.7'"}*

```diff
@@ -42,10 +42,10 @@
             }
         },
         "type": "object"
     },
     "queue": "fr_tfr",
     "service_port": null,
     "url": "https://github.com/tesla-ce/provider-fr-tfr",
-    "version": "0.0.6",
+    "version": "0.0.7",
     "warning_below": 0.6
 }
```

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tfr/provider/__init__.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tfr/provider/models.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/models.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tfr/provider/tfr.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/tfr.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-fr-tfr-0.0.6/src/tfr/provider/utils.py` & `tesla-ce-provider-fr-tfr-0.0.7/src/tfr/provider/utils.py`

 * *Files identical despite different names*

