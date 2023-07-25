# Comparing `tmp/olympix-test-generator-1.2.0.tar.gz` & `tmp/olympix-test-generator-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olympix-test-generator-1.2.0.tar", last modified: Tue Jul 25 16:15:56 2023, max compression
+gzip compressed data, was "olympix-test-generator-1.2.1.tar", last modified: Tue Jul 25 17:00:13 2023, max compression
```

## Comparing `olympix-test-generator-1.2.0.tar` & `olympix-test-generator-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-25 16:16:58.897413 olympix-test-generator-1.2.0/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1794 2023-07-25 16:16:58.895413 olympix-test-generator-1.2.0/PKG-INFO
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1272 2023-07-25 16:16:22.000000 olympix-test-generator-1.2.0/README.md
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-25 16:16:58.808066 olympix-test-generator-1.2.0/olympix_test_generator/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 16:57:55.000000 olympix-test-generator-1.2.0/olympix_test_generator/__init__.py
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     6647 2023-07-25 16:11:50.000000 olympix-test-generator-1.2.0/olympix_test_generator/client.py
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-25 16:16:58.879938 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1794 2023-07-25 16:16:57.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/PKG-INFO
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      364 2023-07-25 16:16:58.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/SOURCES.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        1 2023-07-25 16:16:57.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/dependency_links.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       63 2023-07-25 16:16:57.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/entry_points.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      203 2023-07-25 16:16:57.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/requires.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       23 2023-07-25 16:16:57.000000 olympix-test-generator-1.2.0/olympix_test_generator.egg-info/top_level.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       38 2023-07-25 16:16:58.898416 olympix-test-generator-1.2.0/setup.cfg
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      988 2023-07-25 15:40:51.000000 olympix-test-generator-1.2.0/setup.py
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-25 17:24:00.838957 olympix-test-generator-1.2.1/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1868 2023-07-25 17:24:00.836465 olympix-test-generator-1.2.1/PKG-INFO
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1357 2023-07-25 17:19:12.000000 olympix-test-generator-1.2.1/README.md
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-25 17:24:00.744609 olympix-test-generator-1.2.1/olympix_test_generator/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 16:57:55.000000 olympix-test-generator-1.2.1/olympix_test_generator/__init__.py
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     6647 2023-07-25 16:11:50.000000 olympix-test-generator-1.2.1/olympix_test_generator/client.py
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-25 17:24:00.822743 olympix-test-generator-1.2.1/olympix_test_generator.egg-info/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1868 2023-07-25 17:23:59.000000 olympix-test-generator-1.2.1/olympix_test_generator.egg-info/PKG-INFO
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      364 2023-07-25 17:24:00.000000 olympix-test-generator-1.2.1/olympix_test_generator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        1 2023-07-25 17:23:59.000000 olympix-test-generator-1.2.1/olympix_test_generator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       63 2023-07-25 17:23:59.000000 olympix-test-generator-1.2.1/olympix_test_generator.egg-info/entry_points.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      203 2023-07-25 17:23:59.000000 olympix-test-generator-1.2.1/olympix_test_generator.egg-info/requires.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       23 2023-07-25 17:23:59.000000 olympix-test-generator-1.2.1/olympix_test_generator.egg-info/top_level.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       38 2023-07-25 17:24:00.839961 olympix-test-generator-1.2.1/setup.cfg
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      988 2023-07-25 17:23:17.000000 olympix-test-generator-1.2.1/setup.py
```

### Comparing `olympix-test-generator-1.2.0/PKG-INFO` & `olympix-test-generator-1.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 Metadata-Version: 2.1
 Name: olympix-test-generator
-Version: 1.2.0
+Version: 1.2.1
 Summary: Used to auto-generate unit tests for smart contracts using the Forge framework.
 Home-page: https://github.com/olympix/olympix-test-generator
 Author: Evan Fenster
 Author-email: evan@olympix.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Olympix Test Generator
 
-Olympix Test Generator is a Python package designed to assist with the generation of unit tests for Solidity smart contracts. These unit tests are specifically designed to be ran through [Foundry](https://book.getfoundry.sh/), a tool for writing unit tests in Solidity. 
+Olympix Test Generator is a Python-based utility tool to streamline the process of generating unit tests for Solidity smart contracts. These unit tests are tailored to be compatible with [Foundry](https://book.getfoundry.sh/), a specialized tool for writing unit tests in Solidity.
+
+## Prerequisites
+
+- Python 3.7 or later
+- Solidity 0.8.0 or later
 
 ## Installation
 
-You can install Olympix Test Generator using pip:
+Install the Olympix Test Generator through pip:
 
 ```bash
 pip install olympix-test-generator
 ```
 
-## Usage
-
-The package includes a command-line interface for generating tests.
+## Configuration
 
-Before running the script, make sure to set the `OLYMPIX_API_KEY` environment variable in your system.
+Prior to running the script, you'll need to set the `OLYMPIX_API_KEY` environment variable in your system.
 
-To generate a test, run:
+For Unix or Linux:
 
 ```bash
-olympix generate
+export OLYMPIX_API_KEY=your-api-key
+```
+
+For Windows:
+
+```cmd
+setx OLYMPIX_API_KEY "your-api-key"
 ```
 
-The tool will guide you through the process of generating the test. 
+## Usage
 
-A test contract will be written in the same directory as the selected smart contract, or in a neighboring test folder if it exists. No existing files will be overwritten. The tests are also outputted to the console. 
+Olympix Test Generator offers a command-line interface for creating tests.
 
-## Project Structure
+Initiate the test generation process with:
 
-The project includes the following Python files:
+```bash
+olympix generate
+```
 
-- `client.py`: The main script for interacting with the Olympix DevSecTools API. It includes an interactive command-line interface.
+Upon executing the command, the tool will guide you through the steps required to generate the test. 
 
-## Dependencies
+A test contract will be created either in the same directory as the chosen smart contract, or in an adjacent test folder, should one exist. Existing files will remain unaffected. The generated tests are also displayed on the console. 
 
-This project's dependencies are specified in the `requirements.txt` file.
+For optimal results, generate tests for one function at a time.
```

### Comparing `olympix-test-generator-1.2.0/README.md` & `olympix-test-generator-1.2.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 # Olympix Test Generator
 
-Olympix Test Generator is a Python package designed to assist with the generation of unit tests for Solidity smart contracts. These unit tests are specifically designed to be ran through [Foundry](https://book.getfoundry.sh/), a tool for writing unit tests in Solidity. 
+Olympix Test Generator is a Python-based utility tool to streamline the process of generating unit tests for Solidity smart contracts. These unit tests are tailored to be compatible with [Foundry](https://book.getfoundry.sh/), a specialized tool for writing unit tests in Solidity.
+
+## Prerequisites
+
+- Python 3.7 or later
+- Solidity 0.8.0 or later
 
 ## Installation
 
-You can install Olympix Test Generator using pip:
+Install the Olympix Test Generator through pip:
 
 ```bash
 pip install olympix-test-generator
 ```
 
-## Usage
-
-The package includes a command-line interface for generating tests.
+## Configuration
 
-Before running the script, make sure to set the `OLYMPIX_API_KEY` environment variable in your system.
+Prior to running the script, you'll need to set the `OLYMPIX_API_KEY` environment variable in your system.
 
-To generate a test, run:
+For Unix or Linux:
 
 ```bash
-olympix generate
+export OLYMPIX_API_KEY=your-api-key
+```
+
+For Windows:
+
+```cmd
+setx OLYMPIX_API_KEY "your-api-key"
 ```
 
-The tool will guide you through the process of generating the test. 
+## Usage
 
-A test contract will be written in the same directory as the selected smart contract, or in a neighboring test folder if it exists. No existing files will be overwritten. The tests are also outputted to the console. 
+Olympix Test Generator offers a command-line interface for creating tests.
 
-## Project Structure
+Initiate the test generation process with:
 
-The project includes the following Python files:
+```bash
+olympix generate
+```
 
-- `client.py`: The main script for interacting with the Olympix DevSecTools API. It includes an interactive command-line interface.
+Upon executing the command, the tool will guide you through the steps required to generate the test. 
 
-## Dependencies
+A test contract will be created either in the same directory as the chosen smart contract, or in an adjacent test folder, should one exist. Existing files will remain unaffected. The generated tests are also displayed on the console. 
 
-This project's dependencies are specified in the `requirements.txt` file.
+For optimal results, generate tests for one function at a time.
```

### Comparing `olympix-test-generator-1.2.0/olympix_test_generator/client.py` & `olympix-test-generator-1.2.1/olympix_test_generator/client.py`

 * *Files identical despite different names*

### Comparing `olympix-test-generator-1.2.0/olympix_test_generator.egg-info/PKG-INFO` & `olympix-test-generator-1.2.1/olympix_test_generator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 Metadata-Version: 2.1
 Name: olympix-test-generator
-Version: 1.2.0
+Version: 1.2.1
 Summary: Used to auto-generate unit tests for smart contracts using the Forge framework.
 Home-page: https://github.com/olympix/olympix-test-generator
 Author: Evan Fenster
 Author-email: evan@olympix.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Olympix Test Generator
 
-Olympix Test Generator is a Python package designed to assist with the generation of unit tests for Solidity smart contracts. These unit tests are specifically designed to be ran through [Foundry](https://book.getfoundry.sh/), a tool for writing unit tests in Solidity. 
+Olympix Test Generator is a Python-based utility tool to streamline the process of generating unit tests for Solidity smart contracts. These unit tests are tailored to be compatible with [Foundry](https://book.getfoundry.sh/), a specialized tool for writing unit tests in Solidity.
+
+## Prerequisites
+
+- Python 3.7 or later
+- Solidity 0.8.0 or later
 
 ## Installation
 
-You can install Olympix Test Generator using pip:
+Install the Olympix Test Generator through pip:
 
 ```bash
 pip install olympix-test-generator
 ```
 
-## Usage
-
-The package includes a command-line interface for generating tests.
+## Configuration
 
-Before running the script, make sure to set the `OLYMPIX_API_KEY` environment variable in your system.
+Prior to running the script, you'll need to set the `OLYMPIX_API_KEY` environment variable in your system.
 
-To generate a test, run:
+For Unix or Linux:
 
 ```bash
-olympix generate
+export OLYMPIX_API_KEY=your-api-key
+```
+
+For Windows:
+
+```cmd
+setx OLYMPIX_API_KEY "your-api-key"
 ```
 
-The tool will guide you through the process of generating the test. 
+## Usage
 
-A test contract will be written in the same directory as the selected smart contract, or in a neighboring test folder if it exists. No existing files will be overwritten. The tests are also outputted to the console. 
+Olympix Test Generator offers a command-line interface for creating tests.
 
-## Project Structure
+Initiate the test generation process with:
 
-The project includes the following Python files:
+```bash
+olympix generate
+```
 
-- `client.py`: The main script for interacting with the Olympix DevSecTools API. It includes an interactive command-line interface.
+Upon executing the command, the tool will guide you through the steps required to generate the test. 
 
-## Dependencies
+A test contract will be created either in the same directory as the chosen smart contract, or in an adjacent test folder, should one exist. Existing files will remain unaffected. The generated tests are also displayed on the console. 
 
-This project's dependencies are specified in the `requirements.txt` file.
+For optimal results, generate tests for one function at a time.
```

### Comparing `olympix-test-generator-1.2.0/setup.py` & `olympix-test-generator-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="olympix-test-generator",
-    version="1.2.0",
+    version="1.2.1",
     packages=find_packages(),
     author="Evan Fenster",
     author_email="evan@olympix.ai",
     description="Used to auto-generate unit tests for smart contracts using the Forge framework.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/olympix/olympix-test-generator",
```

