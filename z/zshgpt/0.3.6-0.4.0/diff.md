# Comparing `tmp/zshgpt-0.3.6.tar.gz` & `tmp/zshgpt-0.4.0.tar.gz`

## Comparing `zshgpt-0.3.6.tar` & `zshgpt-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 zshgpt-0.3.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    81149 2020-02-02 00:00:00.000000 zshgpt-0.3.6/Peek 2023-07-17 17-27.gif
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 zshgpt-0.3.6/cicd_plan.md
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 zshgpt-0.3.6/.github/workflows/release.yml
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 zshgpt-0.3.6/.github/workflows/test.yml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 zshgpt-0.3.6/snap/snapcraft.yaml
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 zshgpt-0.3.6/src/zshgpt/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.3.6/src/zshgpt/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.3.6/src/zshgpt/__main__.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 zshgpt-0.3.6/src/zshgpt/cli/__init__.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 zshgpt-0.3.6/src/zshgpt/cli/messages.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 zshgpt-0.3.6/tests/test_main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 zshgpt-0.3.6/zsh_plugin/zsh_plugin.zsh
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 zshgpt-0.3.6/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.3.6/LICENSE.txt
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 zshgpt-0.3.6/README.md
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 zshgpt-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3430 2020-02-02 00:00:00.000000 zshgpt-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 zshgpt-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    81149 2020-02-02 00:00:00.000000 zshgpt-0.4.0/Peek 2023-07-17 17-27.gif
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 zshgpt-0.4.0/cicd_plan.md
+-rw-r--r--   0        0        0    75940 2020-02-02 00:00:00.000000 zshgpt-0.4.0/icon.png
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 zshgpt-0.4.0/zshgpt.plugin.zsh
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 zshgpt-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 zshgpt-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 zshgpt-0.4.0/snap/snapcraft.yaml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 zshgpt-0.4.0/src/zshgpt/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.4.0/src/zshgpt/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-0.4.0/src/zshgpt/__main__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 zshgpt-0.4.0/src/zshgpt/cli/__init__.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 zshgpt-0.4.0/src/zshgpt/cli/messages.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 zshgpt-0.4.0/tests/test_main.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 zshgpt-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 zshgpt-0.4.0/README.md
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 zshgpt-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 zshgpt-0.4.0/PKG-INFO
```

### Comparing `zshgpt-0.3.6/Peek 2023-07-17 17-27.gif` & `zshgpt-0.4.0/Peek 2023-07-17 17-27.gif`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.6/.github/workflows/release.yml` & `zshgpt-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.6/.github/workflows/test.yml` & `zshgpt-0.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.6/src/zshgpt/cli/__init__.py` & `zshgpt-0.4.0/src/zshgpt/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.6/src/zshgpt/cli/messages.py` & `zshgpt-0.4.0/src/zshgpt/cli/messages.py`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.6/.gitignore` & `zshgpt-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.6/LICENSE.txt` & `zshgpt-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zshgpt-0.3.6/README.md` & `zshgpt-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # zshgpt
 
 [![PyPI - Version](https://img.shields.io/pypi/v/zshgpt.svg)](https://pypi.org/project/zshgpt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zshgpt.svg)](https://pypi.org/project/zshgpt)
 
+![Icon](icon.png)
 -----
 
 **Table of Contents**
 
 - [About](#about)
 - [Installation](#installation)
 - [Prerequisite](#prerequisite)
@@ -33,38 +34,71 @@
 
 ```bash
 # Who was Norways first prime minister?
 # Norway's first prime minister was Frederik Stang, serving from 1873 to 1880.
 ```
 
 ## Prerequisite
-* Python >= 3.7
+### Must have
+* Python >= 3.8
 * ZSH + Oh-my-zsh
 * Valid Openai API-key
     * make sure to save under `OPENAI_API_KEY` env.
-    * `export OPENAI_API_KEY='sk-...'`
+    * **`export OPENAI_API_KEY='sk-...'`**
+
+### Nice to have
+* pipx
+* Oh-my-zsh
+* zplug
 
 ## Installation
+⚠️All installations needs to have OPEN_API_KEY set⚠️.
 
-With zshgpt alone, you can ask questions with `zshgpt # Show me all my drives` and it will return an answer from GPT. But the true performance boost comes when you also add the zsh plugin.
-```bash
-pip install zshgpt # Or preferably install with pipx
+`~/.zshrc`
+```
+export OPEN_API_KEY="sk-..."
+```
+
+### Standalone python package
+With zshgpt alone `pipx install zshgpt` , you can ask questions with `zshgpt # Show me all my drives` and it will return an answer from GPT. But the true ✨magic✨ comes when you also add the zsh plugin.
+
+### Manually with zsh
+```zsh
+curl https://raw.githubusercontent.com/AndersSteenNilsen/zshgpt/main/zshgpt.plugin.zsh -o ~ # Copy plugin
+echo "source ~/zshgpt.plugin.zsh" >> ~/.zshrc # Add to zshrc
+exec zsh # Reload zsh
+```
+
+### Manually with oh-my-zsh
+```zsh
 mkdir $ZSH_CUSTOM/plugins/zshgpt
 curl https://raw.githubusercontent.com/AndersSteenNilsen/zshgpt/main/zsh_plugin/zsh_plugin.zsh -o $ZSH_CUSTOM/plugins/zshgpt/zshgpt.plugin.zsh
 ```
 Then add zshgpt in your list of plugins in `~/.zshrc`
 
 ```
 plugins(
     ...
     zshgpt
     ...
 )
 ```
 
+```zsh
+omz reload
+```
+
+### With zplug
+`~/.zshrc`
+```
+...
+zplug "AndersSteenNilsen/zshgpt"
+zplug load
+```
+
 ## Future plans
 
 ### Functionaliy
 * Remember last couple messages so you could do something like:
 ```bash
 # Open README.md <-- USER
 # You can open the README.md file using a text editor of your choice. Here's an example using vim:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zshgpt-0.3.6/pyproject.toml` & `zshgpt-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,39 +3,38 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "zshgpt"
 dynamic = ["version"]
 description = 'Level up z shell with GPT'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Anders Steen", email = "anders.steen@knowit.no" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "click", "openai"
 ]
 
 [project.urls]
-Documentation = "https://github.com/unknown/zshgpt#readme"
-Issues = "https://github.com/unknown/zshgpt/issues"
-Source = "https://github.com/unknown/zshgpt"
+Documentation = "https://github.com/AndersSteenNilsen/zshgpt#readme"
+Issues = "https://github.com/AndersSteenNilsen/zshgpt/issues"
+Source = "https://github.com/AndersSteenNilsen/zshgpt"
 
 [project.scripts]
 zshgpt = "zshgpt.cli:zshgpt"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
@@ -51,15 +50,15 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+python = ["3.8", "3.9", "3.10", "3.11"]
 
 
 [tool.hatch.version]
 # path = "src/zshgpt/__about__.py"
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
@@ -88,20 +87,20 @@
 ]
 all = [
   "style",
   "typing",
 ]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
```

