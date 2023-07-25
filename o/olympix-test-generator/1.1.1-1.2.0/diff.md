# Comparing `tmp/olympix-test-generator-1.1.1.tar.gz` & `tmp/olympix-test-generator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olympix-test-generator-1.1.1.tar", last modified: Mon Jul 24 19:33:55 2023, max compression
+gzip compressed data, was "olympix-test-generator-1.2.0.tar", last modified: Tue Jul 25 16:15:56 2023, max compression
```

## Comparing `olympix-test-generator-1.1.1.tar` & `olympix-test-generator-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-24 20:11:17.826102 olympix-test-generator-1.1.1/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1894 2023-07-24 20:11:17.820034 olympix-test-generator-1.1.1/PKG-INFO
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1051 2023-07-20 20:36:15.000000 olympix-test-generator-1.1.1/README.md
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-24 20:11:17.532111 olympix-test-generator-1.1.1/olympix_test_generator/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 16:57:55.000000 olympix-test-generator-1.1.1/olympix_test_generator/__init__.py
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     2897 2023-07-24 20:10:41.000000 olympix-test-generator-1.1.1/olympix_test_generator/client.py
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-24 20:11:17.769515 olympix-test-generator-1.1.1/olympix_test_generator.egg-info/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1894 2023-07-24 20:11:17.000000 olympix-test-generator-1.1.1/olympix_test_generator.egg-info/PKG-INFO
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      364 2023-07-24 20:11:17.000000 olympix-test-generator-1.1.1/olympix_test_generator.egg-info/SOURCES.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        1 2023-07-24 20:11:17.000000 olympix-test-generator-1.1.1/olympix_test_generator.egg-info/dependency_links.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       64 2023-07-24 20:11:17.000000 olympix-test-generator-1.1.1/olympix_test_generator.egg-info/entry_points.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      203 2023-07-24 20:11:17.000000 olympix-test-generator-1.1.1/olympix_test_generator.egg-info/requires.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       23 2023-07-24 20:11:17.000000 olympix-test-generator-1.1.1/olympix_test_generator.egg-info/top_level.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       38 2023-07-24 20:11:17.826769 olympix-test-generator-1.1.1/setup.cfg
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      988 2023-07-24 20:09:13.000000 olympix-test-generator-1.1.1/setup.py
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-25 16:16:58.897413 olympix-test-generator-1.2.0/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1794 2023-07-25 16:16:58.895413 olympix-test-generator-1.2.0/PKG-INFO
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1272 2023-07-25 16:16:22.000000 olympix-test-generator-1.2.0/README.md
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-25 16:16:58.808066 olympix-test-generator-1.2.0/olympix_test_generator/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 16:57:55.000000 olympix-test-generator-1.2.0/olympix_test_generator/__init__.py
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     6647 2023-07-25 16:11:50.000000 olympix-test-generator-1.2.0/olympix_test_generator/client.py
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-25 16:16:58.879938 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1794 2023-07-25 16:16:57.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/PKG-INFO
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      364 2023-07-25 16:16:58.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        1 2023-07-25 16:16:57.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       63 2023-07-25 16:16:57.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/entry_points.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      203 2023-07-25 16:16:57.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/requires.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       23 2023-07-25 16:16:57.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/top_level.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       38 2023-07-25 16:16:58.898416 olympix-test-generator-1.2.0/setup.cfg
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      988 2023-07-25 15:40:51.000000 olympix-test-generator-1.2.0/setup.py
```

### Comparing `olympix-test-generator-1.1.1/PKG-INFO` & `olympix-test-generator-1.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: olympix-test-generator
-Version: 1.1.1
+Version: 1.2.0
 Summary: Used to auto-generate unit tests for smart contracts using the Forge framework.
 Home-page: https://github.com/olympix/olympix-test-generator
 Author: Evan Fenster
 Author-email: evan@olympix.ai
-License: UNKNOWN
-Description: # Olympix Test Generator
-        
-        Olympix Test Generator is a Python package designed to assist with the generation of unit tests for Solidity smart contracts. These unit tests are specifically designed to be ran through [Foundry](https://book.getfoundry.sh/), a tool for writing unit tests in Solidity. 
-        
-        ## Installation
-        
-        You can install Olympix Test Generator using pip:
-        
-        ```bash
-        pip install olympix-test-generator
-        ```
-        
-        ## Usage
-        
-        The package includes a command-line interface for generating tests.
-        
-        Before running the script, make sure to set the `OLYMPIX_API_KEY` environment variable in your system.
-        
-        To generate a test, run:
-        
-        ```bash
-        olympix generate
-        ```
-        
-        The tool will guide you through the process of generating the test.
-        
-        ## Project Structure
-        
-        The project includes the following Python files:
-        
-        - `client.py`: The main script for interacting with the Olympix DevSecTools API. It includes an interactive command-line interface.
-        
-        ## Dependencies
-        
-        This project's dependencies are specified in the `requirements.txt` file.
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+
+# Olympix Test Generator
+
+Olympix Test Generator is a Python package designed to assist with the generation of unit tests for Solidity smart contracts. These unit tests are specifically designed to be ran through [Foundry](https://book.getfoundry.sh/), a tool for writing unit tests in Solidity. 
+
+## Installation
+
+You can install Olympix Test Generator using pip:
+
+```bash
+pip install olympix-test-generator
+```
+
+## Usage
+
+The package includes a command-line interface for generating tests.
+
+Before running the script, make sure to set the `OLYMPIX_API_KEY` environment variable in your system.
+
+To generate a test, run:
+
+```bash
+olympix generate
+```
+
+The tool will guide you through the process of generating the test. 
+
+A test contract will be written in the same directory as the selected smart contract, or in a neighboring test folder if it exists. No existing files will be overwritten. The tests are also outputted to the console. 
+
+## Project Structure
+
+The project includes the following Python files:
+
+- `client.py`: The main script for interacting with the Olympix DevSecTools API. It includes an interactive command-line interface.
+
+## Dependencies
+
+This project's dependencies are specified in the `requirements.txt` file.
```

### Comparing `olympix-test-generator-1.1.1/README.md` & `olympix-test-generator-1.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 To generate a test, run:
 
 ```bash
 olympix generate
 ```
 
-The tool will guide you through the process of generating the test.
+The tool will guide you through the process of generating the test. 
+
+A test contract will be written in the same directory as the selected smart contract, or in a neighboring test folder if it exists. No existing files will be overwritten. The tests are also outputted to the console. 
 
 ## Project Structure
 
 The project includes the following Python files:
 
 - `client.py`: The main script for interacting with the Olympix DevSecTools API. It includes an interactive command-line interface.
```

### Comparing `olympix-test-generator-1.1.1/olympix_test_generator.egg-info/PKG-INFO` & `olympix-test-generator-1.2.0/olympix_test_generator.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 Metadata-Version: 2.1
 Name: olympix-test-generator
-Version: 1.1.1
+Version: 1.2.0
 Summary: Used to auto-generate unit tests for smart contracts using the Forge framework.
 Home-page: https://github.com/olympix/olympix-test-generator
 Author: Evan Fenster
 Author-email: evan@olympix.ai
-License: UNKNOWN
-Description: # Olympix Test Generator
-        
-        Olympix Test Generator is a Python package designed to assist with the generation of unit tests for Solidity smart contracts. These unit tests are specifically designed to be ran through [Foundry](https://book.getfoundry.sh/), a tool for writing unit tests in Solidity. 
-        
-        ## Installation
-        
-        You can install Olympix Test Generator using pip:
-        
-        ```bash
-        pip install olympix-test-generator
-        ```
-        
-        ## Usage
-        
-        The package includes a command-line interface for generating tests.
-        
-        Before running the script, make sure to set the `OLYMPIX_API_KEY` environment variable in your system.
-        
-        To generate a test, run:
-        
-        ```bash
-        olympix generate
-        ```
-        
-        The tool will guide you through the process of generating the test.
-        
-        ## Project Structure
-        
-        The project includes the following Python files:
-        
-        - `client.py`: The main script for interacting with the Olympix DevSecTools API. It includes an interactive command-line interface.
-        
-        ## Dependencies
-        
-        This project's dependencies are specified in the `requirements.txt` file.
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+
+# Olympix Test Generator
+
+Olympix Test Generator is a Python package designed to assist with the generation of unit tests for Solidity smart contracts. These unit tests are specifically designed to be ran through [Foundry](https://book.getfoundry.sh/), a tool for writing unit tests in Solidity. 
+
+## Installation
+
+You can install Olympix Test Generator using pip:
+
+```bash
+pip install olympix-test-generator
+```
+
+## Usage
+
+The package includes a command-line interface for generating tests.
+
+Before running the script, make sure to set the `OLYMPIX_API_KEY` environment variable in your system.
+
+To generate a test, run:
+
+```bash
+olympix generate
+```
+
+The tool will guide you through the process of generating the test. 
+
+A test contract will be written in the same directory as the selected smart contract, or in a neighboring test folder if it exists. No existing files will be overwritten. The tests are also outputted to the console. 
+
+## Project Structure
+
+The project includes the following Python files:
+
+- `client.py`: The main script for interacting with the Olympix DevSecTools API. It includes an interactive command-line interface.
+
+## Dependencies
+
+This project's dependencies are specified in the `requirements.txt` file.
```

### Comparing `olympix-test-generator-1.1.1/setup.py` & `olympix-test-generator-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="olympix-test-generator",
-    version="1.1.1",
+    version="1.2.0",
     packages=find_packages(),
     author="Evan Fenster",
     author_email="evan@olympix.ai",
     description="Used to auto-generate unit tests for smart contracts using the Forge framework.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/olympix/olympix-test-generator",
```

