# Comparing `tmp/devcontainer_manager-1.4.0.tar.gz` & `tmp/devcontainer_manager-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcontainer_manager-1.4.0.tar", last modified: Fri May 12 19:47:23 2023, max compression
+gzip compressed data, was "devcontainer_manager-1.4.1.tar", last modified: Tue Jul 25 08:45:49 2023, max compression
```

## Comparing `devcontainer_manager-1.4.0.tar` & `devcontainer_manager-1.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/
--rw-rw-r--   0 root         (0) root         (0)     1061 2022-01-06 15:44:11.000000 devcontainer_manager-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-09 12:27:48.000000 devcontainer_manager-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6285 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5996 2023-04-09 12:55:25.000000 devcontainer_manager-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/devcontainer_manager/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 19:46:40.000000 devcontainer_manager-1.4.0/devcontainer_manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-12 19:36:15.000000 devcontainer_manager-1.4.0/devcontainer_manager/alias.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-05-01 17:41:46.000000 devcontainer_manager-1.4.0/devcontainer_manager/base_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/devcontainer_manager/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2376 2023-05-12 19:42:11.000000 devcontainer_manager-1.4.0/devcontainer_manager/cli/alias.py
--rw-r--r--   0 root         (0) root         (0)     4324 2023-04-29 20:20:31.000000 devcontainer_manager-1.4.0/devcontainer_manager/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     7672 2023-04-29 14:45:53.000000 devcontainer_manager-1.4.0/devcontainer_manager/config.py
--rw-r--r--   0 root         (0) root         (0)      336 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2463 2023-05-12 19:42:45.000000 devcontainer_manager-1.4.0/devcontainer_manager/global_config.py
--rw-r--r--   0 root         (0) root         (0)      412 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.399062 devcontainer_manager-1.4.0/devcontainer_manager/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.399062 devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/
--rw-rw-r--   0 root         (0) root         (0)      233 2022-01-07 00:28:25.000000 devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/build.sh
--rw-r--r--   0 root         (0) root         (0)      240 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1786 2023-05-12 19:44:09.000000 devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json
--rw-r--r--   0 root         (0) root         (0)     3449 2023-05-12 19:47:20.000000 devcontainer_manager-1.4.0/devcontainer_manager/types.py
--rw-r--r--   0 root         (0) root         (0)     1203 2022-11-13 22:15:55.000000 devcontainer_manager-1.4.0/devcontainer_manager/util.py
--rw-r--r--   0 root         (0) root         (0)     2691 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6285 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1061 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      408 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      991 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:45:49.922486 devcontainer_manager-1.4.1/
+-rw-rw-r--   0 root         (0) root         (0)     1061 2022-01-06 15:44:11.000000 devcontainer_manager-1.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      108 2023-04-09 12:27:48.000000 devcontainer_manager-1.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6338 2023-07-25 08:45:49.922486 devcontainer_manager-1.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6049 2023-05-12 19:55:37.000000 devcontainer_manager-1.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:45:49.922486 devcontainer_manager-1.4.1/devcontainer_manager/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-25 08:44:56.000000 devcontainer_manager-1.4.1/devcontainer_manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.1/devcontainer_manager/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-07-25 08:43:56.000000 devcontainer_manager-1.4.1/devcontainer_manager/alias.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-07-25 08:30:07.000000 devcontainer_manager-1.4.1/devcontainer_manager/base_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:45:49.922486 devcontainer_manager-1.4.1/devcontainer_manager/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.1/devcontainer_manager/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-05-12 19:42:11.000000 devcontainer_manager-1.4.1/devcontainer_manager/cli/alias.py
+-rw-r--r--   0 root         (0) root         (0)     4317 2023-07-25 08:38:34.000000 devcontainer_manager-1.4.1/devcontainer_manager/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     7672 2023-04-29 14:45:53.000000 devcontainer_manager-1.4.1/devcontainer_manager/config.py
+-rw-r--r--   0 root         (0) root         (0)      336 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.1/devcontainer_manager/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2023-05-12 19:42:45.000000 devcontainer_manager-1.4.1/devcontainer_manager/global_config.py
+-rw-r--r--   0 root         (0) root         (0)      412 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.1/devcontainer_manager/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:45:49.918486 devcontainer_manager-1.4.1/devcontainer_manager/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:45:49.918486 devcontainer_manager-1.4.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:45:49.922486 devcontainer_manager-1.4.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/
+-rw-rw-r--   0 root         (0) root         (0)      233 2022-01-07 00:28:25.000000 devcontainer_manager-1.4.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/build.sh
+-rw-r--r--   0 root         (0) root         (0)      240 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-05-12 19:44:09.000000 devcontainer_manager-1.4.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-07-25 08:45:17.000000 devcontainer_manager-1.4.1/devcontainer_manager/types.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2022-11-13 22:15:55.000000 devcontainer_manager-1.4.1/devcontainer_manager/util.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.1/devcontainer_manager/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:45:49.922486 devcontainer_manager-1.4.1/devcontainer_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6338 2023-07-25 08:45:49.000000 devcontainer_manager-1.4.1/devcontainer_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-07-25 08:45:49.000000 devcontainer_manager-1.4.1/devcontainer_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:45:49.000000 devcontainer_manager-1.4.1/devcontainer_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-25 08:45:49.000000 devcontainer_manager-1.4.1/devcontainer_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-25 08:45:49.000000 devcontainer_manager-1.4.1/devcontainer_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-25 08:45:49.000000 devcontainer_manager-1.4.1/devcontainer_manager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 08:45:49.922486 devcontainer_manager-1.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      991 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.1/setup.py
```

### Comparing `devcontainer_manager-1.4.0/LICENSE` & `devcontainer_manager-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.4.0/PKG-INFO` & `devcontainer_manager-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devcontainer_manager
-Version: 1.4.0
+Version: 1.4.1
 Summary: UNKNOWN
 Home-page: https://github.com/gnox/devcontainer-manager
 Author: gnox
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -174,22 +174,22 @@
 Global configuration can be found in `~/.devcontainer_manager/config.yaml` and
 contains following options:
 
 [//]: # (global_config_block_start)
 ```yaml
 base_config: []
 
-# default values for all configs for the current environment
-defaults: {}
-
 # directory for global templates
 template_dir: templates
 
 # default path for per-project override config (. is in '.devcontainer/')
 override_config_path: .devcontainer/overrides.yaml
+
+# path to global config that will be used as base for all other configs
+default_config_path: '{{ template_dir }}/default.yaml'
 ```
 [//]: # (global_config_block_end)
 
 ### Per Project Template Overrides
 To edit overrides, you can manually edit generated `.devcontainer/overrides.yaml`.
 
 Once the overrides exist, you can then call each subsequent generation using
```

### Comparing `devcontainer_manager-1.4.0/README.md` & `devcontainer_manager-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -161,22 +161,22 @@
 Global configuration can be found in `~/.devcontainer_manager/config.yaml` and
 contains following options:
 
 [//]: # (global_config_block_start)
 ```yaml
 base_config: []
 
-# default values for all configs for the current environment
-defaults: {}
-
 # directory for global templates
 template_dir: templates
 
 # default path for per-project override config (. is in '.devcontainer/')
 override_config_path: .devcontainer/overrides.yaml
+
+# path to global config that will be used as base for all other configs
+default_config_path: '{{ template_dir }}/default.yaml'
 ```
 [//]: # (global_config_block_end)
 
 ### Per Project Template Overrides
 To edit overrides, you can manually edit generated `.devcontainer/overrides.yaml`.
 
 Once the overrides exist, you can then call each subsequent generation using
```

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager/alias.py` & `devcontainer_manager-1.4.1/devcontainer_manager/alias.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 DEFAULT_ALIAS_FILENAME = "aliases.yaml"
 
 
 class AliasConfig(BaseYamlConfigModel):
     aliases: Optional[Dict[str, Path]] = Field(
         default_factory=dict,
         description=(
-            "aliases for templates, can be added using,\n" "`devcontainer_manager alias --help`"
+            "aliases for templates, can be added using,\n`devcontainer_manager alias --help`"
         ),
     )
 
     _not_none = validator("*", pre=True, allow_reuse=True)(default_if_none)
 
     def is_alias(self, alias: str):
         if isinstance(alias, Path):
@@ -29,9 +29,13 @@
         alias_path = self.aliases.get(alias, alias)
         if not alias_path.is_absolute():
             alias_path = self.config_path.parent / alias_path
         return alias_path
 
     def path_to_alias(self, path: Path):
         path = path.resolve()
-        ret = [k for k, p in self.aliases.items() if p.resolve() == path][0]
+        ret = [
+            k
+            for k, p in self.aliases.items()
+            if p.resolve() == path or path.relative_to(self.config_path.parent) == p
+        ][0]
         return path if not ret else ret
```

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager/base_config.py` & `devcontainer_manager-1.4.1/devcontainer_manager/base_config.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager/cli/alias.py` & `devcontainer_manager-1.4.1/devcontainer_manager/cli/alias.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager/cli/cli.py` & `devcontainer_manager-1.4.1/devcontainer_manager/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             typer.echo(
                 "Template argument not specified and "
                 f"{typer.style('.devcontainer/overrides.yaml', path_color)} does not exist"
             )
             raise typer.Exit(1)
         templates = [template_path.as_posix()]
     else:
-        templates = [alias_config.aliases.get(t, t) for t in templates]
+        templates = [alias_config.resolve(t) for t in templates]
 
     configs = [Config.parse_file(t).merge_bases() for t in templates]
     merged_config = global_config.merge_bases().defaults | reduce(lambda a, b: a | b, configs)
 
     if print_config:
         typer.echo(merged_config.yaml())
         raise typer.Exit()
```

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager/config.py` & `devcontainer_manager-1.4.1/devcontainer_manager/config.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager/global_config.py` & `devcontainer_manager-1.4.1/devcontainer_manager/global_config.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json` & `devcontainer_manager-1.4.1/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager/types.py` & `devcontainer_manager-1.4.1/devcontainer_manager/types.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager/util.py` & `devcontainer_manager-1.4.1/devcontainer_manager/util.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager/yaml.py` & `devcontainer_manager-1.4.1/devcontainer_manager/yaml.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager.egg-info/PKG-INFO` & `devcontainer_manager-1.4.1/devcontainer_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devcontainer-manager
-Version: 1.4.0
+Version: 1.4.1
 Summary: UNKNOWN
 Home-page: https://github.com/gnox/devcontainer-manager
 Author: gnox
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -174,22 +174,22 @@
 Global configuration can be found in `~/.devcontainer_manager/config.yaml` and
 contains following options:
 
 [//]: # (global_config_block_start)
 ```yaml
 base_config: []
 
-# default values for all configs for the current environment
-defaults: {}
-
 # directory for global templates
 template_dir: templates
 
 # default path for per-project override config (. is in '.devcontainer/')
 override_config_path: .devcontainer/overrides.yaml
+
+# path to global config that will be used as base for all other configs
+default_config_path: '{{ template_dir }}/default.yaml'
 ```
 [//]: # (global_config_block_end)
 
 ### Per Project Template Overrides
 To edit overrides, you can manually edit generated `.devcontainer/overrides.yaml`.
 
 Once the overrides exist, you can then call each subsequent generation using
```

### Comparing `devcontainer_manager-1.4.0/devcontainer_manager.egg-info/SOURCES.txt` & `devcontainer_manager-1.4.1/devcontainer_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.4.0/setup.py` & `devcontainer_manager-1.4.1/setup.py`

 * *Files identical despite different names*

