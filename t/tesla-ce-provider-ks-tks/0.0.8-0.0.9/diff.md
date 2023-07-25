# Comparing `tmp/tesla-ce-provider-ks-tks-0.0.8.tar.gz` & `tmp/tesla-ce-provider-ks-tks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesla-ce-provider-ks-tks-0.0.8.tar", last modified: Tue Feb  8 19:01:09 2022, max compression
+gzip compressed data, was "tesla-ce-provider-ks-tks-0.0.9.tar", last modified: Tue Jul 25 16:32:45 2023, max compression
```

## Comparing `tesla-ce-provider-ks-tks-0.0.8.tar` & `tesla-ce-provider-ks-tks-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 19:01:09.962418 tesla-ce-provider-ks-tks-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2022-02-08 19:01:09.962418 tesla-ce-provider-ks-tks-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2522 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-08 19:01:09.962418 tesla-ce-provider-ks-tks-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 19:01:09.962418 tesla-ce-provider-ks-tks-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 19:01:09.962418 tesla-ce-provider-ks-tks-0.0.8/src/tesla_ce_provider_ks_tks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2022-02-08 19:01:09.000000 tesla-ce-provider-ks-tks-0.0.8/src/tesla_ce_provider_ks_tks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-02-08 19:01:09.000000 tesla-ce-provider-ks-tks-0.0.8/src/tesla_ce_provider_ks_tks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-08 19:01:09.000000 tesla-ce-provider-ks-tks-0.0.8/src/tesla_ce_provider_ks_tks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-02-08 19:01:09.000000 tesla-ce-provider-ks-tks-0.0.8/src/tesla_ce_provider_ks_tks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-02-08 19:01:09.000000 tesla-ce-provider-ks-tks-0.0.8/src/tesla_ce_provider_ks_tks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 19:01:09.962418 tesla-ce-provider-ks-tks-0.0.8/src/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tests/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tests/test_verification.py
--rw-r--r--   0 runner    (1001) docker     (121)     2994 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tests/test_verification_mixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     5489 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tests/tks_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 19:01:09.962418 tesla-ce-provider-ks-tks-0.0.8/src/tks/
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 19:01:09.962418 tesla-ce-provider-ks-tks-0.0.8/src/tks/data/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-08 19:01:09.000000 tesla-ce-provider-ks-tks-0.0.8/src/tks/data/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tks/data/options.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 19:01:09.962418 tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 19:01:09.962418 tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/models/
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6679 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/models/guassian_mixtures_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     4978 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/models/guassian_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6741 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/tks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-02-08 19:01:03.000000 tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:32:45.976566 tesla-ce-provider-ks-tks-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-25 16:32:45.972566 tesla-ce-provider-ks-tks-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 16:32:45.976566 tesla-ce-provider-ks-tks-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:32:45.972566 tesla-ce-provider-ks-tks-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:32:45.972566 tesla-ce-provider-ks-tks-0.0.9/src/tesla_ce_provider_ks_tks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-25 16:32:45.000000 tesla-ce-provider-ks-tks-0.0.9/src/tesla_ce_provider_ks_tks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-25 16:32:45.000000 tesla-ce-provider-ks-tks-0.0.9/src/tesla_ce_provider_ks_tks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:32:45.000000 tesla-ce-provider-ks-tks-0.0.9/src/tesla_ce_provider_ks_tks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 16:32:45.000000 tesla-ce-provider-ks-tks-0.0.9/src/tesla_ce_provider_ks_tks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 16:32:45.000000 tesla-ce-provider-ks-tks-0.0.9/src/tesla_ce_provider_ks_tks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:32:45.972566 tesla-ce-provider-ks-tks-0.0.9/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tests/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tests/test_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tests/test_verification_mixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tests/tks_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:32:45.972566 tesla-ce-provider-ks-tks-0.0.9/src/tks/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:32:45.972566 tesla-ce-provider-ks-tks-0.0.9/src/tks/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 16:32:45.000000 tesla-ce-provider-ks-tks-0.0.9/src/tks/data/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tks/data/options.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:32:45.972566 tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:32:45.972566 tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/models/guassian_mixtures_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/models/guassian_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/tks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-25 16:32:37.000000 tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/utils.py
```

### Comparing `tesla-ce-provider-ks-tks-0.0.8/LICENSE` & `tesla-ce-provider-ks-tks-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/PKG-INFO` & `tesla-ce-provider-ks-tks-0.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,29 @@
-Metadata-Version: 2.1
-Name: tesla-ce-provider-ks-tks
-Version: 0.0.8
-Summary: TeSLA CE Keystroke Provider
-Home-page: https://tesla-ce.github.io
-Author: Roger Munoz
-Author-email: rmunoz@uoc.edu
-License: UNKNOWN
-Project-URL: Documentation, https://tesla-ce.github.io/provider-ks-tks/
-Project-URL: Source, https://github.com/tesla-ce/provider-ks-tks
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-ks-tks.svg)](https://pypi.python.org/pypi/tesla-ce-provider-ks-tks/)
-        [![codecov](https://codecov.io/gh/tesla-ce/provider-ks-tks/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-ks-tks)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks?ref=badge_shield)
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-ks-tks)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-ks-tks)
-        # TKS: TeSLA CE Keystroke Dynamics Recognition provider 
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
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks?ref=badge_large)
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-ks-tks.svg)](https://pypi.python.org/pypi/tesla-ce-provider-ks-tks/)
+[![codecov](https://codecov.io/gh/tesla-ce/provider-ks-tks/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-ks-tks)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks?ref=badge_shield)
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-ks-tks)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-ks-tks)
+# TKS: TeSLA CE Keystroke Dynamics Recognition provider 
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
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks?ref=badge_large)
```

### Comparing `tesla-ce-provider-ks-tks-0.0.8/README.md` & `tesla-ce-provider-ks-tks-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: tesla-ce-provider-ks-tks
+Version: 0.0.9
+Summary: TeSLA CE Keystroke Provider
+Home-page: https://tesla-ce.github.io
+Author: Roger Munoz
+Author-email: rmunoz@uoc.edu
+License: UNKNOWN
+Project-URL: Documentation, https://tesla-ce.github.io/provider-ks-tks/
+Project-URL: Source, https://github.com/tesla-ce/provider-ks-tks
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-ks-tks.svg)](https://pypi.python.org/pypi/tesla-ce-provider-ks-tks/)
 [![codecov](https://codecov.io/gh/tesla-ce/provider-ks-tks/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-ks-tks)
 [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks?ref=badge_shield)
 [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-ks-tks)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-ks-tks)
 # TKS: TeSLA CE Keystroke Dynamics Recognition provider 
 
@@ -23,7 +41,9 @@
 ## Credits
 Credits: Include a section for credits in order to highlight and link to the authors of your project.
 
 ## License
 This project is licensed under [AGPL v3 licence](http://www.gnu.org/licenses/agpl-3.0).
 
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks?ref=badge_large)
+
+
```

### Comparing `tesla-ce-provider-ks-tks-0.0.8/setup.py` & `tesla-ce-provider-ks-tks-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
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
         'tks': [
             'data/*',
                     ],
     },
     include_package_data=True,
```

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tesla_ce_provider_ks_tks.egg-info/PKG-INFO` & `tesla-ce-provider-ks-tks-0.0.9/src/tesla_ce_provider_ks_tks.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 Metadata-Version: 2.1
 Name: tesla-ce-provider-ks-tks
-Version: 0.0.8
+Version: 0.0.9
 Summary: TeSLA CE Keystroke Provider
 Home-page: https://tesla-ce.github.io
 Author: Roger Munoz
 Author-email: rmunoz@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/provider-ks-tks/
 Project-URL: Source, https://github.com/tesla-ce/provider-ks-tks
-Description: [![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-ks-tks.svg)](https://pypi.python.org/pypi/tesla-ce-provider-ks-tks/)
-        [![codecov](https://codecov.io/gh/tesla-ce/provider-ks-tks/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-ks-tks)
-        [![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks?ref=badge_shield)
-        [![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-ks-tks)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-ks-tks)
-        # TKS: TeSLA CE Keystroke Dynamics Recognition provider 
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
-        [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks?ref=badge_large)
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
+[![PyPi Version](https://img.shields.io/pypi/v/tesla-ce-provider-ks-tks.svg)](https://pypi.python.org/pypi/tesla-ce-provider-ks-tks/)
+[![codecov](https://codecov.io/gh/tesla-ce/provider-ks-tks/branch/main/graph/badge.svg?token=PJJQMW981P)](https://codecov.io/gh/tesla-ce/provider-ks-tks)
+[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks.svg?type=shield)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks?ref=badge_shield)
+[![Quality gate](https://sonar.sunai.uoc.edu/api/project_badges/quality_gate?project=tesla-ce_provider-ks-tks)](https://sonar.sunai.uoc.edu/dashboard?id=tesla-ce_provider-ks-tks)
+# TKS: TeSLA CE Keystroke Dynamics Recognition provider 
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
+[![FOSSA Status](https://app.fossa.com/api/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks.svg?type=large)](https://app.fossa.com/projects/custom%2B26246%2Fgithub.com%2Ftesla-ce%2Fprovider-ks-tks?ref=badge_large)
+
+
```

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tesla_ce_provider_ks_tks.egg-info/SOURCES.txt` & `tesla-ce-provider-ks-tks-0.0.9/src/tesla_ce_provider_ks_tks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tests/__init__.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tests/conftest.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tests/test_notification.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tests/test_notification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tests/test_validation.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tests/test_verification.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tests/test_verification.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tests/test_verification_mixtures.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tests/test_verification_mixtures.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tests/tks_utils.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tests/tks_utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tks/__init__.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tks/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tks/data/options.json` & `tesla-ce-provider-ks-tks-0.0.9/src/tks/data/options.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.0.9'"}*

```diff
@@ -38,10 +38,10 @@
             }
         },
         "type": "object"
     },
     "queue": "ks_tks",
     "service_port": null,
     "url": "https://github.com/tesla-ce/provider-ks-tks",
-    "version": "0.0.5",
+    "version": "0.0.9",
     "warning_below": 0.6
 }
```

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/__init__.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/constants.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/constants.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/models/__init__.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/models/guassian_mixtures_model.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/models/guassian_mixtures_model.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/models/guassian_model.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/models/guassian_model.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/tks.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/tks.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-ks-tks-0.0.8/src/tks/provider/utils.py` & `tesla-ce-provider-ks-tks-0.0.9/src/tks/provider/utils.py`

 * *Files identical despite different names*

