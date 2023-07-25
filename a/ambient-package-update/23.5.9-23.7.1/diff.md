# Comparing `tmp/ambient-package-update-23.5.9.tar.gz` & `tmp/ambient_package_update-23.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient-package-update-23.5.9.tar", last modified: Tue May  9 16:08:20 2023, max compression
+gzip compressed data, was "ambient_package_update-23.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ambient-package-update-23.5.9.tar` & `ambient_package_update-23.7.1.tar`

### file list

```diff
@@ -1,33 +1,37 @@
--rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient-package-update-23.5.9/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/.gitignore
--rw-r--r--   0        0        0      904 2023-05-04 13:34:24.555311 ambient-package-update-23.5.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      822 2023-05-09 16:07:40.602900 ambient-package-update-23.5.9/CHANGES.md
--rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/LICENSE.md
--rw-r--r--   0        0        0     3992 2023-05-09 16:03:59.316283 ambient-package-update-23.5.9/README.md
--rw-r--r--   0        0        0       93 2023-05-09 16:07:40.618528 ambient-package-update-23.5.9/ambient_package_update/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/ambient_package_update/metadata/__init__.py
--rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/ambient_package_update/metadata/author.py
--rw-r--r--   0        0        0      454 2023-05-09 16:06:49.855781 ambient-package-update-23.5.9/ambient_package_update/metadata/constants.py
--rw-r--r--   0        0        0      592 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/ambient_package_update/metadata/package.py
--rw-r--r--   0        0        0      113 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/ambient_package_update/metadata/readme.py
--rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/ambient_package_update/metadata/ruff_ignored_inspection.py
--rw-r--r--   0        0        0     3823 2023-05-09 16:01:10.150288 ambient-package-update-23.5.9/main.py
--rw-r--r--   0        0        0     2550 2023-05-04 13:59:19.861070 ambient-package-update-23.5.9/pyproject.toml
--rw-r--r--   0        0        0     1744 2023-05-09 08:09:25.681131 ambient-package-update-23.5.9/requirements.txt
--rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/scripts/setup_venv.ps1
--rw-r--r--   0        0        0      566 2023-05-09 08:09:25.681131 ambient-package-update-23.5.9/scripts/setup_venv_unix.sh
--rw-r--r--   0        0        0       82 2023-05-04 09:31:48.690822 ambient-package-update-23.5.9/templates/.coveragerc.tpl
--rw-r--r--   0        0        0      288 2023-05-04 09:25:12.333150 ambient-package-update-23.5.9/templates/.editorconfig.tpl
--rw-r--r--   0        0        0     1784 2023-05-04 13:49:38.761775 ambient-package-update-23.5.9/templates/.github/workflows/ci.yml.tpl
--rw-r--r--   0        0        0      904 2023-05-04 13:34:24.540644 ambient-package-update-23.5.9/templates/.pre-commit-config.yaml.tpl
--rw-r--r--   0        0        0      551 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/templates/.readthedocs.yml.tpl
--rw-r--r--   0        0        0     1121 2023-05-04 09:29:00.483983 ambient-package-update-23.5.9/templates/LICENSE.md.tpl
--rw-r--r--   0        0        0      137 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/templates/MANIFEST.in.tpl
--rw-r--r--   0        0        0     5131 2023-05-09 08:12:34.842033 ambient-package-update-23.5.9/templates/Readme.md.tpl
--rw-r--r--   0        0        0      654 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/templates/docs/Makefile.tpl
--rw-r--r--   0        0        0     2847 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/templates/docs/conf.py.tpl
--rw-r--r--   0        0        0      795 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/templates/docs/make.bat.tpl
--rw-r--r--   0        0        0     3742 2023-05-04 13:33:46.734472 ambient-package-update-23.5.9/templates/pyproject.toml.tpl
--rw-r--r--   0        0        0       56 2023-05-04 09:29:24.289641 ambient-package-update-23.5.9/templates/pytest.init.tpl
--rw-r--r--   0        0        0       69 2023-05-03 13:01:37.336270 ambient-package-update-23.5.9/templates/setup.cfg.tpl
--rw-r--r--   0        0        0     5160 1970-01-01 00:00:00.000000 ambient-package-update-23.5.9/PKG-INFO
+-rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient_package_update-23.7.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/.gitignore
+-rw-r--r--   0        0        0      904 2023-07-25 07:49:48.645779 ambient_package_update-23.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1462 2023-07-25 08:05:08.152906 ambient_package_update-23.7.1/CHANGES.md
+-rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/LICENSE.md
+-rw-r--r--   0        0        0     4457 2023-07-25 08:05:08.168549 ambient_package_update-23.7.1/README.md
+-rw-r--r--   0        0        0       93 2023-07-25 07:56:30.784223 ambient_package_update-23.7.1/ambient_package_update/__init__.py
+-rw-r--r--   0        0        0     3773 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/cli.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/ambient_package_update/metadata/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/ambient_package_update/metadata/author.py
+-rw-r--r--   0        0        0      454 2023-05-09 16:06:49.855781 ambient_package_update-23.7.1/ambient_package_update/metadata/constants.py
+-rw-r--r--   0        0        0      592 2023-05-10 08:37:32.317360 ambient_package_update-23.7.1/ambient_package_update/metadata/package.py
+-rw-r--r--   0        0        0      192 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/metadata/readme.py
+-rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/ambient_package_update/metadata/ruff_ignored_inspection.py
+-rw-r--r--   0        0        0       82 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/.coveragerc.tpl
+-rw-r--r--   0        0        0      288 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/.editorconfig.tpl
+-rw-r--r--   0        0        0     1784 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/.github/workflows/ci.yml.tpl
+-rw-r--r--   0        0        0      904 2023-07-25 07:49:48.645779 ambient_package_update-23.7.1/ambient_package_update/templates/.pre-commit-config.yaml.tpl
+-rw-r--r--   0        0        0      551 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/.readthedocs.yml.tpl
+-rw-r--r--   0        0        0     1121 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/LICENSE.md.tpl
+-rw-r--r--   0        0        0      137 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/MANIFEST.in.tpl
+-rw-r--r--   0        0        0     5231 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/README.md.tpl
+-rw-r--r--   0        0        0      654 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/docs/Makefile.tpl
+-rw-r--r--   0        0        0     2847 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/docs/conf.py.tpl
+-rw-r--r--   0        0        0      795 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/docs/make.bat.tpl
+-rw-r--r--   0        0        0     3808 2023-07-25 07:54:21.598162 ambient_package_update-23.7.1/ambient_package_update/templates/pyproject.toml.tpl
+-rw-r--r--   0        0        0       56 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/pytest.init.tpl
+-rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.7.1/ambient_package_update/templates/scripts/publish_to_pypi.ps1.tpl
+-rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.7.1/ambient_package_update/templates/scripts/publish_to_pypi.sh.tpl
+-rw-r--r--   0        0        0       69 2023-05-22 13:32:26.231832 ambient_package_update-23.7.1/ambient_package_update/templates/setup.cfg.tpl
+-rw-r--r--   0        0        0     2549 2023-07-25 08:59:34.407282 ambient_package_update-23.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1740 2023-07-25 08:59:49.665764 ambient_package_update-23.7.1/requirements.txt
+-rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.7.1/scripts/unix/publish_to_pypi.sh
+-rw-r--r--   0        0        0      566 2023-05-09 08:09:25.681131 ambient_package_update-23.7.1/scripts/unix/setup_venv_unix.sh
+-rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.7.1/scripts/windows/publish_to_pypi.ps1
+-rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/scripts/windows/setup_venv.ps1
+-rw-r--r--   0        0        0     5605 1970-01-01 00:00:00.000000 ambient_package_update-23.7.1/PKG-INFO
```

### Comparing `ambient-package-update-23.5.9/.gitignore` & `ambient_package_update-23.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.9/.pre-commit-config.yaml` & `ambient_package_update-23.7.1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # you find the full pre-commit-tools docu under:
 # https://pre-commit.com/
 
 repos:
   - repo: https://github.com/ambv/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
         args: [ --check, --diff, --config, ./pyproject.toml ]
         language_version: python3.11
         stages: [ push ]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.264'
+    rev: 'v0.0.280'
     hooks:
       - id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.9.0
     hooks:
       - id: pyupgrade
         args: [ --py38-plus ]
         language_version: python3.11
         stages: [ push ]
 
   - repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
       - id: django-upgrade
-        args: [--target-version, "2.2"]
+        args: [--target-version, "3.2"]
         language_version: python3.11
         stages: [ push ]
```

### Comparing `ambient-package-update-23.5.9/LICENSE.md` & `ambient_package_update-23.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.9/README.md` & `ambient_package_update-23.7.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 [![pypi](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://pypi.python.org/pypi/ambient-package-update/)
 [![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
 
 # Ambient Package Update
 
-This repository will help keep all Python packages maintained by 
+This repository will help keep all Python packages maintained by
 [Ambient Digital](https://ambient.digital) tidy and up-to-date.
 
 This package will render all required configuration and installation files for your target package.
 
 Typical use-cases:
-* A new Python or Django version was release
-* A Python or Django version was deprecated
-* You want to update the Sphinx documentation builder
-* You want to update the linter versions
-* You want to add the third-party dependencies
+
+- A new Python or Django version was released
+- A Python or Django version was deprecated
+- You want to update the Sphinx documentation builder
+- You want to update the linter versions
+- You want to add the third-party dependencies
 
 ## Versioning
 
 This project follows the CalVer versioning pattern: `YY.MM.[RELEASE]`
 
-# Installation
-
-1. Ensure you have installed Python >=3.11 and the binary is in your system path
-2. Clone this package from GitHub
-3. Navigate into the project directory
-4. Execute scripts/setup_venv.ps1 on Windows or scripts/setup_venv_unix.sh on Unix/macOS
-
 ## How to update a package
 
 These steps will tell you how to update a package which was created by using this updater.
 
-* Navigate to the main directory of this package
-* Activate your virtualenv
-* Run `python .\main.py render-templates [PACKAGE_NAME]`
-* Open your target package in the IDE, validate the changes and increment the version accordingly
-* Release a new version of your target package
+- Navigate to the main directory of **your** package
+- Activate your virtualenv
+- Run `python -m ambient_package_update.cli render-templates`
+- Validate the changes and increment the version accordingly
+- Release a new version of your target package
 
 ## How to create a new package
 
 Just follow these steps if you want to create a new package and maintain it using this updater.
 
-* Create a new repo at GitHub
-* Check out the new repository in the same directory this updater lives in (not inside the updater!)
-* Create a directory ".ambient-package-update" and create a file "metadata.py" inside.
+- Create a new repo at GitHub
+- Check out the new repository in the same directory this updater lives in (not inside the updater!)
+- Create a directory ".ambient-package-update" and create a file "metadata.py" inside.
 
 ```python
 from ambient_package_update.metadata.author import PackageAuthor
 from ambient_package_update.metadata.constants import DEV_DEPENDENCIES
 from ambient_package_update.metadata.package import PackageMetadata
 from ambient_package_update.metadata.readme import ReadmeContent
 from ambient_package_update.metadata.ruff_ignored_inspection import RuffIgnoredInspection
@@ -72,43 +66,67 @@
         'dev': [
             *DEV_DEPENDENCIES,
         ],
         # you might add further extras here
     },
     ruff_ignore_list=[
         RuffIgnoredInspection(key='XYZ', comment="Reason why we need this exception"),
-        
+
     ],
 )
 ```
- 
-* Finally, follow the steps of the section above (`How to update a package`).
+
+- Install the `ambient_package_update` package
+  ```
+  # ideally in a virtual environment
+  pip install ambient-package-update
+  ```
+- Add `docs/index.rst` and link your readme and changelog to have a basic documentation (surely, you can add or write
+  more custom docs if you want!)
+- Enable the readthedocs hook in your GitHub repo to update your documentation on a commit basis
+- Finally, follow the steps of the section above (`How to update a package`).
 
 ## Contribution
 
+### Dependency updates
+
+The dependencies of this package are being maintained with `pip-tools`. 
+
+> pip install -U pip-tools
+
+To add/update/remove a package, please do so in the main `pyproject.toml`. Afterward, call the following command to
+reflect your changes in the `requirements.txt`.
+
+> pip-compile --upgrade
+
+To install the packages, run:
+
+> pip-sync
+
 ### Publish to PyPi
 
 - Update documentation about new/changed functionality
 
 - Update the `Changelog`
 
 - Increment version in main `__init__.py`
 
 - Increment version of this package in dependencies in `ambient_package_update/metadata/constants.py`
 
 - Create pull request / merge to master
 
 - This project uses the flit package to publish to PyPI. Thus publishing should be as easy as running:
+
   ```
   flit publish
   ```
 
   To publish to TestPyPI use the following ensure that you have set up your .pypirc as
   shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
 
   ```
   flit publish --repository testpypi
   ```
 
 ## Changelog
 
-Can be found at [GitHub](https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md).
+Can be found at [GitHub](https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md).
```

### Comparing `ambient-package-update-23.5.9/ambient_package_update/metadata/package.py` & `ambient_package_update-23.7.1/ambient_package_update/metadata/package.py`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.9/main.py` & `ambient_package_update-23.7.1/ambient_package_update/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from pathlib import Path
 
 import typer
 from jinja2 import Template
 
 from ambient_package_update.metadata.package import PackageMetadata
 
+BASE_PATH = Path(__file__).parent
+
 app = typer.Typer()
 
 """
 def deploy_to_test_pypi(package_name: str):
     subprocess.run("echo 'Publishing to test pypi'")
     subprocess.run(f"cd {package_name} && flit publish --repository testpypi")
 
@@ -52,76 +54,77 @@
         run_tests(package_name=package)
 
 
 """
 
 
 @app.command()
-def get_metadata(package_name: str) -> PackageMetadata:
-    sys.path.append(f"../{package_name}/.ambient-package-update")
+def get_metadata() -> PackageMetadata:
+    sys.path.append("./.ambient-package-update")
     try:
         m = import_module('metadata')
     except ModuleNotFoundError as e:
         raise RuntimeError('Please create a directory ".ambient-package-update" and add a "metadata.py".') from e
     sys.path.pop()
 
     return m.METADATA
 
 
 @app.command()
-def render_templates(package_name: str):
-    template_path = './templates'
+def render_templates():
+    template_path = BASE_PATH / "templates"
 
     template_list = []
     for path, subdirs, files in os.walk(template_path):
         print(path, subdirs, files)
         for file in files:
             template_list.append(Path(f"{path}/{file}"))
 
-    print(f'Start rending distribution templates for package "{package_name}".')
+    print('Start rending distribution templates.')
+    metadata_dict = get_metadata().__dict__
     for template in template_list:
         j2_template = Template(template.read_text(), keep_trailing_newline=True)
         j2_template.globals['current_year'] = datetime.now(tz=timezone.utc).date().year
 
-        rendered_string = j2_template.render(get_metadata(package_name).__dict__)
-
-        relative_template_path = str(template).replace('templates', '')
+        rendered_string = j2_template.render(metadata_dict)
 
-        print(relative_template_path)
+        relative_template_path = str(Path(template).relative_to(template_path))[:-4]
 
-        rendered_file_path = f'../{package_name}/{relative_template_path[:-4]}'
         # Create missing directories
-        os.makedirs(os.path.dirname(rendered_file_path), exist_ok=True)
+        print(relative_template_path)
+        relative_template_dir = os.path.dirname(relative_template_path)
+        if relative_template_dir:
+            os.makedirs(os.path.dirname(relative_template_path), exist_ok=True)
 
-        with open(rendered_file_path, 'w') as f:
+        with open(relative_template_path, 'w') as f:
             f.write(rendered_string)
 
-        abs_path = Path(rendered_file_path).resolve()
+        abs_path = Path(relative_template_path).resolve()
         print(f'> Successfully rendered template "{abs_path}".')
     print('Rendering finished.')
 
 
 @app.command()
 def build_docs(package_name: str):
     print(f'Building docs for package "{package_name}"')
     subprocess.call(f"cd ../{package_name} && sphinx-build docs/ docs/_build/html/", shell=True)
 
 
 @app.command()
-def run_tests(package_name: str):
-    print(f'Running tests for package "{package_name}"')
+def run_tests():
+    print('Running tests')
 
-    package_data = get_metadata(package_name)
-    dependency_list = package_data['dependencies']
+    package_data = get_metadata()
+    dependency_list = package_data.dependencies
 
-    if package_data['optional_dependencies']:
-        for _, opt_dependency in package_data['optional_dependencies'].items():
+    if package_data.optional_dependencies:
+        for _, opt_dependency in package_data.optional_dependencies.items():
             dependency_list += opt_dependency
 
     dependency_list = ' '.join(f'"{d}"' for d in dependency_list)
     subprocess.call(f"pip install {dependency_list}", shell=True)
 
-    subprocess.call(f"cd ../{package_name} && pytest --ds settings tests", shell=True)
+    subprocess.call("pytest --ds settings tests", shell=True)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `ambient-package-update-23.5.9/pyproject.toml` & `ambient_package_update-23.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "Topic :: Utilities",
 ]
 dynamic = ["version", "description"]
 license = {"file" = "LICENSE.md"}
 dependencies = [
-    'typer~=0.7',
+    'typer~=0.9',
     'Jinja2~=3.1',
-    'flit~=3.8',
-    'keyring~=23.13',
+    'flit~=3.9',
+    'keyring~=24.2',
     # Linting
-    'pre-commit~=3.2',
-    'black~=23.3',
+    'pre-commit~=3.3',
+    'black~=23.7',
 ]
 
 [project.urls]
 'Homepage' = 'https://github.com/ambient-innovation/ambient-package-update/'
 'Documentation' = 'https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md'
 'Maintained by' = 'https://ambient.digital/'
 'Bugtracker' = 'https://github.com/ambient-innovation/ambient-package-update/issues'
```

### Comparing `ambient-package-update-23.5.9/requirements.txt` & `ambient_package_update-23.7.1/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,81 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --extra=dev --output-file=requirements.txt --resolver=backtracking pyproject.toml
+#    pip-compile
 #
-black==23.3.0
+black==23.7.0
     # via ambient-package-update (pyproject.toml)
-certifi==2022.12.7
+certifi==2023.7.22
     # via requests
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.6
     # via
     #   black
     #   typer
-distlib==0.3.6
+colorama==0.4.6
+    # via click
+distlib==0.3.7
     # via virtualenv
-docutils==0.19
+docutils==0.20.1
     # via flit
-filelock==3.12.0
+filelock==3.12.2
     # via virtualenv
-flit==3.8.0
+flit==3.9.0
     # via ambient-package-update (pyproject.toml)
-flit-core==3.8.0
+flit-core==3.9.0
     # via flit
-identify==2.5.23
+identify==2.5.26
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.6.0
+importlib-metadata==6.8.0
     # via keyring
-jaraco-classes==3.2.3
+jaraco-classes==3.3.0
     # via keyring
 jinja2==3.1.2
     # via ambient-package-update (pyproject.toml)
-keyring==23.13.1
+keyring==24.2.0
     # via ambient-package-update (pyproject.toml)
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via jinja2
-more-itertools==9.1.0
+more-itertools==10.0.0
     # via jaraco-classes
 mypy-extensions==1.0.0
     # via black
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
 packaging==23.1
     # via black
 pathspec==0.11.1
     # via black
-platformdirs==3.5.0
+platformdirs==3.9.1
     # via
     #   black
     #   virtualenv
-pre-commit==3.3.1
+pre-commit==3.3.3
     # via ambient-package-update (pyproject.toml)
-pyyaml==6.0
+pywin32-ctypes==0.2.2
+    # via keyring
+pyyaml==6.0.1
     # via pre-commit
-requests==2.29.0
+requests==2.31.0
     # via flit
 tomli-w==1.0.0
     # via flit
 typer==0.9.0
     # via ambient-package-update (pyproject.toml)
-typing-extensions==4.5.0
+typing-extensions==4.7.1
     # via typer
-urllib3==1.26.15
+urllib3==2.0.4
     # via requests
-virtualenv==20.23.0
+virtualenv==20.24.2
     # via pre-commit
-zipp==3.15.0
+zipp==3.16.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `ambient-package-update-23.5.9/scripts/setup_venv_unix.sh` & `ambient_package_update-23.7.1/scripts/unix/setup_venv_unix.sh`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.9/templates/.github/workflows/ci.yml.tpl` & `ambient_package_update-23.7.1/ambient_package_update/templates/.github/workflows/ci.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.9/templates/.pre-commit-config.yaml.tpl` & `ambient_package_update-23.7.1/ambient_package_update/templates/.pre-commit-config.yaml.tpl`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # you find the full pre-commit-tools docu under:
 # https://pre-commit.com/
 
 repos:
   - repo: https://github.com/ambv/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
         args: [ --check, --diff, --config, ./pyproject.toml ]
         language_version: python3.11
         stages: [ push ]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.264'
+    rev: 'v0.0.280'
     hooks:
       - id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.9.0
     hooks:
       - id: pyupgrade
         args: [ --py38-plus ]
         language_version: python3.11
         stages: [ push ]
 
   - repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
       - id: django-upgrade
-        args: [--target-version, "2.2"]
+        args: [--target-version, "3.2"]
         language_version: python3.11
         stages: [ push ]
```

### Comparing `ambient-package-update-23.5.9/templates/.readthedocs.yml.tpl` & `ambient_package_update-23.7.1/ambient_package_update/templates/.readthedocs.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.9/templates/LICENSE.md.tpl` & `ambient_package_update-23.7.1/ambient_package_update/templates/LICENSE.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.9/templates/Readme.md.tpl` & `ambient_package_update-23.7.1/ambient_package_update/templates/README.md.tpl`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 * [Full documentation](https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/index.html)
 * Creator & Maintainer: [Ambient Digital](https://ambient.digital)
 
 {{ readme_content.content }}
 
 ## Installation
 
+{% if readme_content.installation %}
+  {{ readme_content.installation }}
+{% else %}
 - Install the package via pip:
 
   `pip install {{ package_name|replace("_", "-") }}`
 
   or via pipenv:
 
   `pipenv install {{ package_name|replace("_", "-") }}`
@@ -25,14 +28,15 @@
 
     ````
     INSTALLED_APPS = (
         ...
         '{{ package_name }}',
     )
      ````
+{% endif %}
 
 ## Contribute
 
 ### Setup package for development
 
 - Create a Python virtualenv and activate it
 - Install "pip-tools" with `pip install pip-tools`
```

### Comparing `ambient-package-update-23.5.9/templates/docs/Makefile.tpl` & `ambient_package_update-23.7.1/ambient_package_update/templates/docs/Makefile.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.9/templates/docs/conf.py.tpl` & `ambient_package_update-23.7.1/ambient_package_update/templates/docs/conf.py.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.9/templates/docs/make.bat.tpl` & `ambient_package_update-23.7.1/ambient_package_update/templates/docs/make.bat.tpl`

 * *Files identical despite different names*

### Comparing `ambient-package-update-23.5.9/templates/pyproject.toml.tpl` & `ambient_package_update-23.7.1/ambient_package_update/templates/pyproject.toml.tpl`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [build-system]
-requires = ["flit_core >=3.2,<4"]
+requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "{{ package_name|replace("_", "-") }}"
 authors = [{% for author in authors %}
     {'name' = '{{ author.name }}', 'email' = '{{ author.email }}'},{% endfor %}
 ]
 readme = "README.md"
 classifiers = [
     "Development Status :: {{ development_status }}",
     "Environment :: Web Environment",
     "Framework :: Django",
-    "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -50,14 +49,16 @@
 'Documentation' = 'https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/index.html'
 'Maintained by' = 'https://ambient.digital/'
 'Bugtracker' = 'https://github.com/ambient-innovation/{{ package_name|replace("_", "-") }}/issues'
 'Changelog' = 'https://{{ package_name|replace("_", "-") }}.readthedocs.io/en/latest/features/changelog.html'
 
 
 [tool.black]
+# use force-exclude, so that black also applies exclude when run using pre-commit: https://github.com/psf/black/issues/395
+force-exclude = '''.*/migrations/.*'''
 line-length = 120
 multi_line_output = 3
 skip-string-normalization = true
 include_trailing_comma = true
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
@@ -106,20 +107,17 @@
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py{38,39,310,311}-django{22,30,31,32,40,41,42}
 isolated_build = True
 
 [testenv]
+# Django deprecation overview: https://www.djangoproject.com/download/
 deps =
-    django22: Django>=2.2.28,<3.0
-    django30: Django>=3.0,<3.1
-    django31: Django>=3.1,<3.2
     django32: Django>=3.2,<3.3
-    django40: Django>=4.0,<4.1
     django41: Django>=4.1,<4.2
     django42: Django>=4.2,<4.3
 extras = {% for area, dependency_list in optional_dependencies.items() %}{{ area }},{% endfor %}
 commands =
     pytest --ds settings tests
 
 [gh-actions]
```

### Comparing `ambient-package-update-23.5.9/PKG-INFO` & `ambient_package_update-23.7.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,74 @@
 Metadata-Version: 2.1
 Name: ambient-package-update
-Version: 23.5.9
+Version: 23.7.1
 Summary: Ambient package update tool for clean and swift maintenance
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Dist: typer~=0.7
+Requires-Dist: typer~=0.9
 Requires-Dist: Jinja2~=3.1
-Requires-Dist: flit~=3.8
-Requires-Dist: keyring~=23.13
-Requires-Dist: pre-commit~=3.2
-Requires-Dist: black~=23.3
+Requires-Dist: flit~=3.9
+Requires-Dist: keyring~=24.2
+Requires-Dist: pre-commit~=3.3
+Requires-Dist: black~=23.7
 Project-URL: Bugtracker, https://github.com/ambient-innovation/ambient-package-update/issues
 Project-URL: Changelog, https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md
 Project-URL: Documentation, https://github.com/ambient-innovation/ambient-package-update/blob/master/README.md
 Project-URL: Homepage, https://github.com/ambient-innovation/ambient-package-update/
 Project-URL: Maintained by, https://ambient.digital/
 
 [![pypi](https://img.shields.io/pypi/v/ambient-package-update.svg)](https://pypi.python.org/pypi/ambient-package-update/)
 [![Downloads](https://pepy.tech/badge/ambient-package-update)](https://pepy.tech/project/ambient-package-update)
 
 # Ambient Package Update
 
-This repository will help keep all Python packages maintained by 
+This repository will help keep all Python packages maintained by
 [Ambient Digital](https://ambient.digital) tidy and up-to-date.
 
 This package will render all required configuration and installation files for your target package.
 
 Typical use-cases:
-* A new Python or Django version was release
-* A Python or Django version was deprecated
-* You want to update the Sphinx documentation builder
-* You want to update the linter versions
-* You want to add the third-party dependencies
+
+- A new Python or Django version was released
+- A Python or Django version was deprecated
+- You want to update the Sphinx documentation builder
+- You want to update the linter versions
+- You want to add the third-party dependencies
 
 ## Versioning
 
 This project follows the CalVer versioning pattern: `YY.MM.[RELEASE]`
 
-# Installation
-
-1. Ensure you have installed Python >=3.11 and the binary is in your system path
-2. Clone this package from GitHub
-3. Navigate into the project directory
-4. Execute scripts/setup_venv.ps1 on Windows or scripts/setup_venv_unix.sh on Unix/macOS
-
 ## How to update a package
 
 These steps will tell you how to update a package which was created by using this updater.
 
-* Navigate to the main directory of this package
-* Activate your virtualenv
-* Run `python .\main.py render-templates [PACKAGE_NAME]`
-* Open your target package in the IDE, validate the changes and increment the version accordingly
-* Release a new version of your target package
+- Navigate to the main directory of **your** package
+- Activate your virtualenv
+- Run `python -m ambient_package_update.cli render-templates`
+- Validate the changes and increment the version accordingly
+- Release a new version of your target package
 
 ## How to create a new package
 
 Just follow these steps if you want to create a new package and maintain it using this updater.
 
-* Create a new repo at GitHub
-* Check out the new repository in the same directory this updater lives in (not inside the updater!)
-* Create a directory ".ambient-package-update" and create a file "metadata.py" inside.
+- Create a new repo at GitHub
+- Check out the new repository in the same directory this updater lives in (not inside the updater!)
+- Create a directory ".ambient-package-update" and create a file "metadata.py" inside.
 
 ```python
 from ambient_package_update.metadata.author import PackageAuthor
 from ambient_package_update.metadata.constants import DEV_DEPENDENCIES
 from ambient_package_update.metadata.package import PackageMetadata
 from ambient_package_update.metadata.readme import ReadmeContent
 from ambient_package_update.metadata.ruff_ignored_inspection import RuffIgnoredInspection
@@ -100,43 +94,68 @@
         'dev': [
             *DEV_DEPENDENCIES,
         ],
         # you might add further extras here
     },
     ruff_ignore_list=[
         RuffIgnoredInspection(key='XYZ', comment="Reason why we need this exception"),
-        
+
     ],
 )
 ```
- 
-* Finally, follow the steps of the section above (`How to update a package`).
+
+- Install the `ambient_package_update` package
+  ```
+  # ideally in a virtual environment
+  pip install ambient-package-update
+  ```
+- Add `docs/index.rst` and link your readme and changelog to have a basic documentation (surely, you can add or write
+  more custom docs if you want!)
+- Enable the readthedocs hook in your GitHub repo to update your documentation on a commit basis
+- Finally, follow the steps of the section above (`How to update a package`).
 
 ## Contribution
 
+### Dependency updates
+
+The dependencies of this package are being maintained with `pip-tools`. 
+
+> pip install -U pip-tools
+
+To add/update/remove a package, please do so in the main `pyproject.toml`. Afterward, call the following command to
+reflect your changes in the `requirements.txt`.
+
+> pip-compile --upgrade
+
+To install the packages, run:
+
+> pip-sync
+
 ### Publish to PyPi
 
 - Update documentation about new/changed functionality
 
 - Update the `Changelog`
 
 - Increment version in main `__init__.py`
 
 - Increment version of this package in dependencies in `ambient_package_update/metadata/constants.py`
 
 - Create pull request / merge to master
 
 - This project uses the flit package to publish to PyPI. Thus publishing should be as easy as running:
+
   ```
   flit publish
   ```
 
   To publish to TestPyPI use the following ensure that you have set up your .pypirc as
   shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
 
   ```
   flit publish --repository testpypi
   ```
 
 ## Changelog
 
 Can be found at [GitHub](https://github.com/ambient-innovation/ambient-package-update/blob/master/CHANGES.md).
+
```

