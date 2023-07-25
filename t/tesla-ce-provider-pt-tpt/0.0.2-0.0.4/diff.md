# Comparing `tmp/tesla-ce-provider-pt-tpt-0.0.2.tar.gz` & `tmp/tesla-ce-provider-pt-tpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesla-ce-provider-pt-tpt-0.0.2.tar", last modified: Mon Sep 12 09:42:21 2022, max compression
+gzip compressed data, was "tesla-ce-provider-pt-tpt-0.0.4.tar", last modified: Tue Jul 25 15:14:16 2023, max compression
```

## Comparing `tesla-ce-provider-pt-tpt-0.0.2.tar` & `tesla-ce-provider-pt-tpt-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 09:42:21.849979 tesla-ce-provider-pt-tpt-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3399 2022-09-12 09:42:21.849979 tesla-ce-provider-pt-tpt-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-12 09:42:21.849979 tesla-ce-provider-pt-tpt-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 09:42:21.841979 tesla-ce-provider-pt-tpt-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 09:42:21.845979 tesla-ce-provider-pt-tpt-0.0.2/src/tesla_ce_provider_pt_tpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3399 2022-09-12 09:42:21.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tesla_ce_provider_pt_tpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-09-12 09:42:21.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tesla_ce_provider_pt_tpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 09:42:21.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tesla_ce_provider_pt_tpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-09-12 09:42:21.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tesla_ce_provider_pt_tpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-12 09:42:21.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tesla_ce_provider_pt_tpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 09:42:21.845979 tesla-ce-provider-pt-tpt-0.0.2/src/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2567 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tests/test_validation_tpt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 09:42:21.845979 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 09:42:21.845979 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/data/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-12 09:42:21.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/data/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 09:42:21.845979 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/provider/
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8047 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/provider/tpt.py
--rw-r--r--   0 runner    (1001) docker     (121)     9389 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/provider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 09:42:21.845979 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 09:42:21.849979 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/base_tpt_lib_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/invalid_api_url.py
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/invalid_secret.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/request_failed.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-09-12 09:42:12.000000 tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.349770 tesla-ce-provider-pt-tpt-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-25 15:14:16.349770 tesla-ce-provider-pt-tpt-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:14:16.349770 tesla-ce-provider-pt-tpt-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-25 15:14:16.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 15:14:16.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:14:16.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-25 15:14:16.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 15:14:16.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tests/test_validation_tpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 15:14:15.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/data/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/tpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.349770 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/base_tpt_lib_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/invalid_api_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/invalid_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/request_failed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/timeout.py
```

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/LICENSE` & `tesla-ce-provider-pt-tpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/PKG-INFO` & `tesla-ce-provider-pt-tpt-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,31 @@
-Metadata-Version: 2.1
-Name: tesla-ce-provider-pt-tpt
-Version: 0.0.2
-Summary: TeSLA CE Plagiarism Provider
-Home-page: https://tesla-ce.github.io
-Author: Roger Muñoz Bernaus
-Author-email: rmunozber@uoc.edu
-License: UNKNOWN
-Project-URL: Documentation, https://tesla-ce.github.io/provider-pt-tpt/
-Project-URL: Source, https://github.com/tesla-ce/provider-pt-tpt
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-pt-tpt.svg)](https://pypi.python.org/pypi/tesla-ce-provider-pt-tpt/)
-        [![codecov](https://codecov.io/gh/tesla-ce/provider-pt-tpt/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-pt-tpt)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt?ref=badge_shield)
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-pt-tpt)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-pt-tpt)
-        
-        
-        # TeSLA CE Plagiarism Tool based on TPT
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
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt?ref=badge_large)
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-pt-tpt.svg)](https://pypi.python.org/pypi/tesla-ce-provider-pt-tpt/)
+[![codecov](https://codecov.io/gh/tesla-ce/provider-pt-tpt/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-pt-tpt)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt?ref=badge_shield)
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-pt-tpt)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-pt-tpt)
+
+
+# TeSLA CE Plagiarism Tool based on TPT
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
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt?ref=badge_large)
```

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/README.md` & `tesla-ce-provider-pt-tpt-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: tesla-ce-provider-pt-tpt
+Version: 0.0.4
+Summary: TeSLA CE Plagiarism Provider
+Home-page: https://tesla-ce.github.io
+Author: Roger Muñoz Bernaus
+Author-email: rmunozber@uoc.edu
+License: UNKNOWN
+Project-URL: Documentation, https://tesla-ce.github.io/provider-pt-tpt/
+Project-URL: Source, https://github.com/tesla-ce/provider-pt-tpt
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-pt-tpt.svg)](https://pypi.python.org/pypi/tesla-ce-provider-pt-tpt/)
 [![codecov](https://codecov.io/gh/tesla-ce/provider-pt-tpt/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-pt-tpt)
 [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt?ref=badge_shield)
 [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-pt-tpt)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-pt-tpt)
 
 
@@ -25,7 +43,9 @@
 ## Credits
 Credits: Include a section for credits in order to highlight and link to the authors of your project.
 
 ## License
 This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
 
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt?ref=badge_large)
+
+
```

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/setup.py` & `tesla-ce-provider-pt-tpt-0.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     packages=setuptools.find_packages('src', exclude='__pycache__'),
     package_dir={'': 'src'},  # tell distutils packages are under src
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Operating System :: POSIX :: Linux",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     package_data={
         '': ['*.cfg', 'VERSION'],
         'tpt': [
             'data/*',
                     ],
     },
     include_package_data=True,
```

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tesla_ce_provider_pt_tpt.egg-info/PKG-INFO` & `tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: tesla-ce-provider-pt-tpt
-Version: 0.0.2
+Version: 0.0.4
 Summary: TeSLA CE Plagiarism Provider
 Home-page: https://tesla-ce.github.io
 Author: Roger Muñoz Bernaus
 Author-email: rmunozber@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/provider-pt-tpt/
 Project-URL: Source, https://github.com/tesla-ce/provider-pt-tpt
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-pt-tpt.svg)](https://pypi.python.org/pypi/tesla-ce-provider-pt-tpt/)
-        [![codecov](https://codecov.io/gh/tesla-ce/provider-pt-tpt/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-pt-tpt)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt?ref=badge_shield)
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-pt-tpt)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-pt-tpt)
-        
-        
-        # TeSLA CE Plagiarism Tool based on TPT
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
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt?ref=badge_large)
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-pt-tpt.svg)](https://pypi.python.org/pypi/tesla-ce-provider-pt-tpt/)
+[![codecov](https://codecov.io/gh/tesla-ce/provider-pt-tpt/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-pt-tpt)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt?ref=badge_shield)
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-pt-tpt)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-pt-tpt)
+
+
+# TeSLA CE Plagiarism Tool based on TPT
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
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-pt-tpt?ref=badge_large)
+
+
```

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tesla_ce_provider_pt_tpt.egg-info/SOURCES.txt` & `tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tests/__init__.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tests/conftest.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tests/test_validation_tpt.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tests/test_validation_tpt.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tests/utils.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tpt/__init__.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tpt/provider/__init__.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tpt/provider/tpt.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/tpt.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tpt/provider/utils.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                     if attempt.get('open_text') is True:
                         content_raw_text += attempt.get('answer')+'\n\r'
 
             files_structure.append({
                 "filename": context.get('type')+'.txt',
                 "mimetype": 'text/plain',
                 "status": "ACCEPTED",
-                "content": content_raw_text
+                "content": content_raw_text.encode('utf-8')
             })
 
         # check if sample has attachments
         for decompress_file in decompress_files:
             # skip content.txt file
             if decompress_file == FILENAME_CONTENT:
                 continue
```

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/__init__.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/base_tpt_lib_exception.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/base_tpt_lib_exception.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/invalid_api_url.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/invalid_api_url.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/invalid_secret.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/invalid_secret.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/request_failed.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/request_failed.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.2/src/tpt/tpt_lib/exceptions/timeout.py` & `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/timeout.py`

 * *Files identical despite different names*

