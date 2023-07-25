# Comparing `tmp/meson_vs_gen-0.1.0.tar.gz` & `tmp/meson_vs_gen-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meson_vs_gen-0.1.0.tar", max compression
+gzip compressed data, was "meson_vs_gen-0.2.0.tar", max compression
```

## Comparing `meson_vs_gen-0.1.0.tar` & `meson_vs_gen-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-07-20 19:04:33.793496 meson_vs_gen-0.1.0/LICENSE
--rw-r--r--   0        0        0     8561 2023-07-20 19:04:33.793496 meson_vs_gen-0.1.0/README.md
--rw-r--r--   0        0        0     1440 2023-07-20 19:04:33.793496 meson_vs_gen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-20 19:04:33.818495 meson_vs_gen-0.1.0/vsgen/__init__.py
--rw-r--r--   0        0        0       71 2023-07-20 19:04:33.794495 meson_vs_gen-0.1.0/vsgen/__main__.py
--rw-r--r--   0        0        0     3799 2023-07-20 19:04:33.794495 meson_vs_gen-0.1.0/vsgen/api.py
--rw-r--r--   0        0        0      440 2023-07-20 19:04:33.794495 meson_vs_gen-0.1.0/vsgen/cli/__init__.py
--rw-r--r--   0        0        0     2380 2023-07-20 19:04:33.794495 meson_vs_gen-0.1.0/vsgen/cli/_pathconfig.py
--rw-r--r--   0        0        0     1573 2023-07-20 19:04:33.794495 meson_vs_gen-0.1.0/vsgen/cli/generate.py
--rw-r--r--   0        0        0     1221 2023-07-20 19:04:33.794495 meson_vs_gen-0.1.0/vsgen/cli/project.py
--rw-r--r--   0        0        0     2776 2023-07-20 19:04:33.794495 meson_vs_gen-0.1.0/vsgen/cli/solution.py
--rw-r--r--   0        0        0     9983 2023-07-20 19:04:33.794495 meson_vs_gen-0.1.0/vsgen/configfile.py
--rw-r--r--   0        0        0     1009 2023-07-20 19:04:33.794495 meson_vs_gen-0.1.0/vsgen/configuration.py
--rw-r--r--   0        0        0     6826 2023-07-20 19:04:33.795496 meson_vs_gen-0.1.0/vsgen/introspector.py
--rw-r--r--   0        0        0     3358 2023-07-20 19:04:33.795496 meson_vs_gen-0.1.0/vsgen/runsettings.py
--rw-r--r--   0        0        0     6010 2023-07-20 19:04:33.795496 meson_vs_gen-0.1.0/vsgen/sln.py
--rw-r--r--   0        0        0    12216 2023-07-20 19:04:33.795496 meson_vs_gen-0.1.0/vsgen/vcxproj.py
--rw-r--r--   0        0        0     9749 1970-01-01 00:00:00.000000 meson_vs_gen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-25 11:54:34.935475 meson_vs_gen-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9649 2023-07-25 11:54:34.935475 meson_vs_gen-0.2.0/README.md
+-rw-r--r--   0        0        0     1440 2023-07-25 11:54:34.936475 meson_vs_gen-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 11:54:34.959475 meson_vs_gen-0.2.0/vsgen/__init__.py
+-rw-r--r--   0        0        0       71 2023-07-25 11:54:34.936475 meson_vs_gen-0.2.0/vsgen/__main__.py
+-rw-r--r--   0        0        0     4213 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/api.py
+-rw-r--r--   0        0        0      440 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/cli/__init__.py
+-rw-r--r--   0        0        0     2380 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/cli/_pathconfig.py
+-rw-r--r--   0        0        0     1573 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/cli/generate.py
+-rw-r--r--   0        0        0     1221 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/cli/project.py
+-rw-r--r--   0        0        0     2776 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/cli/solution.py
+-rw-r--r--   0        0        0    10848 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/configfile.py
+-rw-r--r--   0        0        0     1043 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/configuration.py
+-rw-r--r--   0        0        0     8807 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/introspector.py
+-rw-r--r--   0        0        0     3358 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/runsettings.py
+-rw-r--r--   0        0        0     6010 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/sln.py
+-rw-r--r--   0        0        0    12465 2023-07-25 11:54:34.937475 meson_vs_gen-0.2.0/vsgen/vcxproj.py
+-rw-r--r--   0        0        0    10837 1970-01-01 00:00:00.000000 meson_vs_gen-0.2.0/PKG-INFO
```

### Comparing `meson_vs_gen-0.1.0/LICENSE` & `meson_vs_gen-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.1.0/README.md` & `meson_vs_gen-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,21 @@
 
 
 The config file contains the following keys:
 
 - `outputdir`: (optional) Where to generate the solution files, if not specified
   on the command line. Default is to use current dir.
 - `projectdir`: (optional) Name of a subdirectory where to write project files.
-- `case_insensitive_targets`: If true, lower case targets match project names containing uppercase characters.
+- `case_insensitive_targets`: (optional) If true, lower case targets match project names containing uppercase characters.
+- `only_relative_files`: (optional) If true, do not add files outside target source dir
+                         (i.e. where target meson.build file is located) into the project.
+- `include_from_env`: (optional) If true, will use `INCLUDE` env var for system include path.
+                                 If 'auto', will use `INCLUDE` if it is defined.
+                                 If false (default), will no rewrite the include path.
+                                 This is useful when using a different build tools version that the IDE.                         
 - `configs`: map build directories to config names.
 - `archs`: (optional) map cpu_family to arch name. If not specified,
   use the cpu_family as the arch name.
 - `projects`: The projects to generate. See project specifications below
   for more details.
 - `solutions`: The solutions to generate. See solution specifications below
   for more details.
@@ -94,14 +100,17 @@
 
 If the value is a boolean, `true` means to generate the project with default settings,
 and `false` means to not generate that project.
 
 If the value is a map, the following keys are recognized:
 
 - `target`: the build target name. `true` means to use the project name as the target name.
+            If target name begins with `dep:`, this is the name of an internal dependency object,
+            used for a header only project. This project will not compile, but will display files
+            from that dependency.
   `all` is used for a target that generates all targets.
 - `subdir`: if specified, put the generated project into that subdir of the project dir.
 
 #### Solution specifications
 
 For each solution, the key is the name of the solution to generate.
 
@@ -136,22 +145,26 @@
 
 You can also modify or override the `cpu_arch` dictionary,
 mapping cpu_family to arch name for the solution and projects.
 
 The next step is to call `set_config`. The method takes the following arguments:
 - `builddir`: meson build dir, absolute, or relative to `self.basedir`.
 - `name`: (optional) config name to use (default is builddir name).
+- `use_include_from_env`: (optional) If `True`, will use the `INCLUDE` env var
+                          as system include path.
 
 The `project` method is used to create a `VcxProj` object. Arguments are:
 - `name`: The project name.
 - `target`: (optional) The build target name. Default is project name.
 - `subdir`: (optional) Subdir (relative to projectdir) where to write the project.
   If `True`, the subdir is the project name. If `False`, no subdir is used.
 - `update`: (optional) If `True`, update existing project instead of overwriting it.
   Default is `True`.
+- `only_relative_files`: (optional) If `True`, will not reference source files that
+                         are not relative to the project root.
 
 The method returns a `VcxProj` object.
 
 The `solution` method is used to create a `SolutionFile` object.
 Arguments are:
 - `name`: The solution name.
 - `update`: Whether to update existing files instead of overwriting them.
```

### Comparing `meson_vs_gen-0.1.0/pyproject.toml` & `meson_vs_gen-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "meson-vs-gen"
-version = "0.1.0"
+version = "0.2.0"
 description = "Generates Visual Studio solutions and projects for meson projects"
 authors = ["Charles Brunet <charles.brunet@optelgroup.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/optelgroup-public/meson-vs-gen"
 keywords = ["visualstudio", "meson"]
 classifiers = [
```

### Comparing `meson_vs_gen-0.1.0/vsgen/api.py` & `meson_vs_gen-0.2.0/vsgen/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,29 +27,30 @@
             'x86_64': 'x64',
             'x86': 'Win32',
         }
 
         self._intro: Optional[Introspector] = None
         self._config: Optional[Configuration] = None
 
-    def set_config(self, builddir: PathOrStr, name: Optional[str] = None) -> bool:
+    def set_config(self, builddir: PathOrStr, name: Optional[str] = None, use_include_from_env: bool = False) -> bool:
         try:
             self._intro = Introspector(self.basedir / builddir)
         except RuntimeError:
             return False
 
         cpu_family = self._intro.cpu_family()
         arch = self.cpu_arch.get(cpu_family, cpu_family)
 
         self._config = Configuration(
             name or self._intro.build_dir.name,
             arch,
             self._intro.is_debug(),
             self._intro.toolset(),
             self._intro.build_dir,
+            use_include_from_env,
         )
         return True
 
     @property
     def introspector(self) -> Introspector:
         if self._intro is None:
             raise RuntimeError("Generator not configurated. Call `set_config()` first.")
@@ -65,15 +66,20 @@
             raise RuntimeError("Generator not configurated. Call `set_config()` first.")
         return self._config
 
     def all_targets(self) -> list[str]:
         return self.introspector.all_targets()
 
     def project(
-        self, name: str, target: Union[str, bool, None] = None, subdir: Union[PathOrStr, bool] = False, update: bool = True
+        self,
+        name: str,
+        target: Union[str, bool, None] = None,
+        subdir: Union[PathOrStr, bool] = False,
+        update: bool = True,
+        only_relative_files: bool = False
     ) -> VcxProj:
         project_path = self.projectdir
         if subdir is True:
             project_path /= name
         elif subdir:
             project_path /= subdir
 
@@ -86,31 +92,36 @@
         vcxproj.add_config(self.config)
 
         if target is True or not target:
             target = name
         output = self.introspector.get_target_filename(target)
         extra_paths = self.introspector.get_target_extra_paths(target)
 
-        if output:
+        if target.startswith('dep:'):
+            build_params = BuildParams(
+                None,
+                *self.introspector.get_target_params(target)
+            )
+        elif output:
             output = Path(output).relative_to(self.builddir)
 
             build_params = BuildParams(
                 str(output),
                 *self.introspector.get_target_params(target),
                 extra_paths,
             )
         else:
             build_params = BuildParams(output=target)
 
         vcxproj.add_build_params(str(self.config), build_params)
 
-        if output:
-            vcxproj.add_sources(self.introspector.get_target_sources(target))
-            vcxproj.add_headers(self.introspector.get_target_headers(target))
-            vcxproj.add_extra_files(self.introspector.get_target_extra_files(target, self.basedir))
+        if output or target.startswith('dep:'):
+            vcxproj.add_sources(self.introspector.get_target_sources(target, only_relative_files))
+            vcxproj.add_headers(self.introspector.get_target_headers(target, only_relative_files))
+            vcxproj.add_extra_files(self.introspector.get_target_extra_files(target, self.basedir, only_relative_files))
         elif target == 'all':
             vcxproj.add_extra_files(self.introspector.get_build_files())
 
         return vcxproj
 
     def solution(self, name: str, update: bool = True) -> SolutionFile:
         sln = SolutionFile(self.outputdir / name)
```

### Comparing `meson_vs_gen-0.1.0/vsgen/cli/_pathconfig.py` & `meson_vs_gen-0.2.0/vsgen/cli/_pathconfig.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.1.0/vsgen/cli/generate.py` & `meson_vs_gen-0.2.0/vsgen/cli/generate.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.1.0/vsgen/cli/project.py` & `meson_vs_gen-0.2.0/vsgen/cli/project.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.1.0/vsgen/cli/solution.py` & `meson_vs_gen-0.2.0/vsgen/cli/solution.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.1.0/vsgen/configfile.py` & `meson_vs_gen-0.2.0/vsgen/configfile.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,27 +46,32 @@
 
         if self.data['projects'].get('*'):
             results.update(self._analyse_targets(targets))
 
         return results
 
     def generate(self, basepath: Path, outputpath: Optional[Path] = None, update: bool = True):
+
+        use_include_from_env = self.data.get('include_from_env', False)
+        if use_include_from_env == 'auto':
+            use_include_from_env = os.environ.get('INCLUDE', None) is not None
+
         if not outputpath:
             outputpath = Path(self.data.get('outputdir', '.'))
 
         gen = Generator(outputpath, basepath, self.data.get('projectdir', ''))
         gen.cpu_arch = self.data.get('archs', {})
 
         projects = []
         solutions = {}
         for config_path, config_name in self.data.get('configs', {}).items():
-            if not gen.set_config(config_path, config_name):
+            if not gen.set_config(config_path, config_name, use_include_from_env):
                 continue
 
-            projects = self._generate_projects(gen, update, self.data.get('case_insensitive_targets', False))
+            projects = self._generate_projects(gen, update)
             solutions = self._generate_solutions(gen, projects, update)
             update = True
 
         self._generate_runsettings(gen, solutions, projects)
 
     def _analyse_targets(self, targets: set[str]) -> dict:
         listed_targets = set()
@@ -96,15 +101,18 @@
 
     def _analyse_solutions_with_unexisting_projects(self):
         pass
 
     def _analyse_solutions_without_build(self):
         pass
 
-    def _generate_projects(self, gen: Generator, update: bool, ci_targets: bool=False) -> list[VcxProj]:
+    def _generate_projects(self, gen: Generator, update: bool) -> list[VcxProj]:
+        ci_targets = self.data.get('case_insensitive_targets', False)
+        orf = self.data.get('only_relative_files', False)
+
         projects = []
         all_targets = set(gen.all_targets())
 
         default_config = {
             'target': True,
             'subdir': '',
         }
@@ -117,29 +125,38 @@
                 continue
 
             if config is False:
                 if name in all_targets:
                     all_targets.remove(name)
                 elif ci_targets and name.lower() in all_targets:
                     all_targets.remove(name.lower())
+                elif 'dep:' + name in all_targets:
+                    all_targets.remove('dep:' + name)
+                elif ci_targets and 'dep:' + name.lower() in all_targets:
+                    all_targets.remove('dep:' + name.lower())
                 continue
 
             if config is True:
                 config = default_config
             elif isinstance(config, str):
                 config = default_config | {'target': config}
             else:
                 config = default_config | config
 
             target = config['target']
             if target is True:
                 target = name
 
-                if target not in all_targets and ci_targets and name.lower() in all_targets:
-                    target = name.lower()
+                if target not in all_targets:
+                    if ci_targets and target.lower() in all_targets:
+                        target = target.lower()
+                    elif 'dep:' + target in all_targets:
+                        target = 'dep:' + target
+                    elif ci_targets and 'dep:' + target.lower() in all_targets:
+                        target = 'dep:' + target.lower()
 
             elif target is False:
                 continue
 
             if isinstance(target, list):
                 for t in target.copy():
                     if t not in all_targets and t not in self.SPECIAL_TARGETS:
@@ -155,19 +172,21 @@
 
             else:
                 if target in all_targets:
                     all_targets.remove(target)
                 elif target not in self.SPECIAL_TARGETS:
                     continue
 
-            project = gen.project(name, target, config['subdir'], update).write()
+            project = gen.project(name, target, config['subdir'], update, orf).write()
             projects.append(project)
 
         if self.data.get('projects', {}).get('*'):
             for target in all_targets:
+                if target.startswith('dep:'):
+                    continue
                 project = gen.project(target, target, default_config['subdir'], update).write()
                 projects.append(project)
 
         return projects
 
     def _generate_solutions(self, gen: Generator, projects: list[VcxProj], update: bool) -> dict[str, SolutionFile]:
         solutions = {}
```

### Comparing `meson_vs_gen-0.1.0/vsgen/configuration.py` & `meson_vs_gen-0.2.0/vsgen/configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 @dataclass(eq=True)
 class Configuration(BaseConfig):
 
     is_debug: bool
     toolset: str
     builddir: Path
+    use_env_include: bool = False
 
 
 @dataclass
 class BuildParams:
 
     output: str | None = None
     include_directories: list[Path] = field(default_factory=list)
```

### Comparing `meson_vs_gen-0.1.0/vsgen/introspector.py` & `meson_vs_gen-0.2.0/vsgen/introspector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from functools import lru_cache
 import json
 from pathlib import Path
-import re
-from typing import Any, Optional
+from typing import Any, Optional, Iterable
 
 
 def lmfind(d: list[dict[str, Any]], v: Any, key: str = 'name', default: Any = None) -> Any:
     for item in d:
         if item.get(key, ...) == v:
             return item
     return default
@@ -32,14 +31,15 @@
 
 
 class Introspector:
 
     INFO_DIR = 'meson-info'
     INFO_FILE = 'meson-info.json'
     LANGUAGES = {'cpp', 'c'}
+    HEADER_SUFFIXES = ('.h', '.hh', '.hpp', 'h++', '.H')
 
     def __init__(self, build_dir: Path):
         self.build_dir = build_dir
         self.intro_data = {}
 
         info_file = self.build_dir / self.INFO_DIR / self.INFO_FILE
         if not info_file.exists():
@@ -76,94 +76,139 @@
                     return f'v{int(version[0])-6}0'
 
         raise UnsuportedLanguageError(
             "vsgen is only compatible with projects using {} language".format(" and ".join(self.LANGUAGES))
         )
 
     def get_target_filename(self, target: str) -> Optional[str]:
+        if target.startswith('dep:'):
+            return None
+
         data = self._target_data(target)
         if not data:
             return None
 
         return data['filename'][0]
 
     def get_target_params(self, target: str) -> tuple[list[Path], list[str], list[str]]:
+        includes = []
+        macros = []
+        options = []
+
         data = self._target_data(target)
         if not data:
             return [], [], []
 
-        includes = []
-        macros = []
-        options = []
+        if target.startswith('dep:'):
+            includes.extend(map(Path, data['include_directories']))
+            for param in data['compile_args']:
+                if param.startswith(('-I', '/I')):
+                    includes.append(Path(param[2:]))
+                elif param.startswith(('-D', '/D')):
+                    macros.append(param[2:])
+                else:
+                    options.append(param)
 
-        for sources in data["target_sources"]:
-            lang = sources.get("language")
-            if lang in self.LANGUAGES:
-                for param in sources['parameters']:
-                    if param.startswith(('-I', '/I')):
-                        includes.append(Path(param[2:]))
-                    elif param.startswith(('-D', '/D')):
-                        macros.append(param[2:])
-                    else:
-                        options.append(param)
+        else:
+            for sources in data["target_sources"]:
+                lang = sources.get("language")
+                if lang in self.LANGUAGES:
+                    for param in sources['parameters']:
+                        if param.startswith(('-I', '/I')):
+                            includes.append(Path(param[2:]))
+                        elif param.startswith(('-D', '/D')):
+                            macros.append(param[2:])
+                        else:
+                            options.append(param)
 
         return includes, macros, options
+    
+    def _filter_sources(self, sources: Iterable[Path], rel_dir: Path):
+        for src in sources:
+            if src.is_relative_to(rel_dir):
+                yield src
 
-    def get_target_sources(self, target: str) -> list[Path]:
+    def get_target_sources(self, target: str, only_relative_files: bool = False) -> list[Path]:
         data = self._target_data(target)
         if not data:
             return []
 
         sources = []
-        for source_item in data["target_sources"]:
-            if source_item.get("linker"):
-                continue
-            sources.extend(map(Path, source_item['sources']))
-            sources.extend(map(Path, source_item.get('unity_sources', [])))
-            for s in source_item['generated_sources']:
-                if not re.search(r'-unity\d+\.c', s):
-                    sources.append(Path(s))
+
+        if target.startswith('dep:'):
+            sources.extend(map(Path, data['sources']))
+
+        else:
+            for source_item in data["target_sources"]:
+                if source_item.get("linker"):
+                    continue
+
+                source_files = map(Path, source_item['sources'])
+                if only_relative_files:
+                    source_dir = Path(data['defined_in']).parent
+                    source_files = self._filter_sources(source_files, source_dir)
+                sources.extend(source_files)
+
+                unity_sources = map(Path, source_item.get('unity_sources', []))
+                if only_relative_files:
+                    unity_sources = self._filter_sources(unity_sources, source_dir)
+                else:
+                    unity_sources = (us for us in unity_sources if not us.is_relative_to(self.build_dir))
+                sources.extend(unity_sources)
 
         return sources
 
-    def get_target_headers(self, target: str) -> list[Path]:
+    def get_target_headers(self, target: str, only_relative_files: bool = False) -> list[Path]:
         data = self._target_data(target)
         if not data:
             return []
 
+        if not target.startswith('dep:'):
+            source_dir = Path(data['defined_in']).parent
+
         headers = []
         for s in data['extra_files']:
-            if s.endswith(('.h', '.hh', '.hpp', 'h++', '.H')):
-                headers.append(Path(s))
+            if s.endswith(self.HEADER_SUFFIXES):
+                s = Path(s)
+                if target.startswith('dep:') or not only_relative_files or s.is_relative_to(source_dir):
+                    headers.append(s)
 
         return headers
 
-    def get_target_extra_files(self, target: str, sources_root: Path) -> list[Path]:
+    def get_target_extra_files(self, target: str, sources_root: Path, only_relative_files: bool = False) -> list[Path]:
         data = self._target_data(target)
         if not data:
             return []
+        
+        if not target.startswith('dep:'):
+            source_dir = Path(data['defined_in']).parent
 
         extras = set()
         for s in data['extra_files']:
-            if s.endswith(('.h', '.hh', '.hpp', 'h++', '.H')):
-                extras.add(Path(s))
-
-        # meson.build files
-        source_dir = Path(data['defined_in']).parent
-        for m in self.intro_data['buildsystem_files']:
-            if (e := Path(m)).is_relative_to(source_dir):
-                extras.add(e)
-
-        if def_file := data.get('vs_module_defs'):
-            def_file = (sources_root / def_file).resolve()
-            extras.add(def_file)
+            if not s.endswith(self.HEADER_SUFFIXES):
+                s = Path(s)
+                if target.startswith('dep:') or not only_relative_files or s.is_relative_to(source_dir):
+                    extras.add(s)
+
+        if not target.startswith('dep:'):
+            # meson.build files
+            for m in self.intro_data['buildsystem_files']:
+                if (e := Path(m)).is_relative_to(source_dir):
+                    extras.add(e)
+
+            if def_file := data.get('vs_module_defs'):
+                def_file = (sources_root / def_file).resolve()
+                extras.add(def_file)
 
         return list(sorted(extras))
 
     def get_target_extra_paths(self, target: str) -> list[Path]:
+        if target.startswith('dep:'):
+            return []
+
         data = self._target_data(target)
         if not data:
             return []
 
         target_id = data["id"]
 
         test_data = lmfind(self.intro_data["tests"], [target_id], key="depends")
@@ -173,30 +218,25 @@
         return list(map(Path, test_data.get("extra_paths", [])))
 
     def get_build_files(self) -> list[Path]:
         return list(map(Path, self.intro_data['buildsystem_files']))
 
     @lru_cache(maxsize=None)
     def _target_data(self, target: str) -> Optional[dict]:
+        if target.startswith('dep:'):
+            return lmfind(self.intro_data['dependencies'], [target[4:]], key='meson_variables', default=None)
+
         target_data = lmfind(self.intro_data["targets"], target)
 
         if target_data and target_data['type'] == "alias":
 
             depends = target_data.get("depends")
             if depends and len(depends) > 0:
                 target_data = lmfind(self.intro_data["targets"], depends[0], key="id")
 
-            else:
-                # Fallback waiting for #11758
-                name = target_data['id'].removesuffix('@run')
-                for data in self.intro_data["targets"]:
-                    if data['id'].startswith(name) and data['id'] != target_data['id']:
-                        return data
-                return None
-
         return target_data
 
     def all_targets(self) -> list[str]:
         targets = {}
 
         for target_data in self.intro_data['targets']:
             if target_data['type'] == 'alias':
@@ -204,8 +244,13 @@
                 for tname, tid in reversed(targets.items()):
                     if tid.startswith(prefix):
                         del targets[tname]
                         break
 
             targets[target_data['name']] = target_data['id']
 
+        for dep_data in self.intro_data['dependencies']:
+            if dep_data['type'] == 'internal' and dep_data['meson_variables']:
+                target_name = 'dep:' + dep_data['meson_variables'][0]
+                targets[target_name] = dep_data['name']
+
         return list(targets)
```

### Comparing `meson_vs_gen-0.1.0/vsgen/runsettings.py` & `meson_vs_gen-0.2.0/vsgen/runsettings.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.1.0/vsgen/sln.py` & `meson_vs_gen-0.2.0/vsgen/sln.py`

 * *Files identical despite different names*

### Comparing `meson_vs_gen-0.1.0/vsgen/vcxproj.py` & `meson_vs_gen-0.2.0/vsgen/vcxproj.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,16 @@
             elif label is None:
                 if include_directories := self._read_opt_node(config_node, 'NMakeIncludeSearchPath'):
                     params.include_directories = list(map(Path, include_directories.split(';')))
                 if macros := self._read_opt_node(config_node, 'NMakePreprocessorDefinitions'):
                     params.macros = macros.split(' ')
                 if additional_options := self._read_opt_node(config_node, 'AdditionalOptions'):
                     params.additional_options = additional_options.split(';')
+                if self._read_opt_node(config_node, 'IncludePath') == '$(INCLUDE)':
+                    config.use_env_include = True
 
                 build_cmd = self._read_opt_node(config_node, 'NMakeBuildCommandLine', '')
                 m = re.fullmatch(r'ninja -C (\S+) (\S+)', build_cmd)
                 params.output = m[2] if m else None
 
     def _load_files(self, project_xml: ET.Element):
         for filetype in ("ClCompile", "ClInclude", "None"):
@@ -103,15 +105,15 @@
         if not self.filepath.exists():
             raise FileNotFoundError(f'{self.filepath} does not exist')
 
         project_xml = ET.parse(self.filepath).getroot()
         self._load_configs(project_xml)
         self._load_files(project_xml)
 
-    def _read_opt_node(self, parent: ET.Element, name: str, default: Optional[str] = None) -> Optional[str]:
+    def _read_opt_node(self, parent: ET.Element, name: str, default: Optional[str] = None) -> str | None:
         node = parent.find(f'{{{self.NS}}}{name}')
         if node is None:
             return default
         return node.text or default
 
     def remove_user_file(self) -> None:
         self.userpath.unlink(missing_ok=True)
@@ -210,14 +212,17 @@
                     map(self._relpath, params.include_directories)
                 )
             if params.additional_options:
                 ET.SubElement(compile_cmd, 'AdditionalOptions').text = ' '.join(params.additional_options)
             ET.SubElement(compile_cmd, 'LocalDebuggerWorkingDirectory').text = '$(BuildDir)'
             ET.SubElement(compile_cmd, 'LocalDebuggerEnvironment').text = 'PATH=$(DllPaths)'
 
+            if config.use_env_include:
+                ET.SubElement(compile_cmd, 'IncludePath').text = '$(INCLUDE)'
+
         cat_nodes: dict[str, ET.Element] = {}
         for filename, category in sorted(self._files.items()):
             node = cat_nodes.get(category)
             if node is None:
                 node = ET.SubElement(root, 'ItemGroup')
                 cat_nodes[category] = node
             ET.SubElement(node, category, attrib={'Include': self._relpath(filename)})
```

### Comparing `meson_vs_gen-0.1.0/PKG-INFO` & `meson_vs_gen-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meson-vs-gen
-Version: 0.1.0
+Version: 0.2.0
 Summary: Generates Visual Studio solutions and projects for meson projects
 Home-page: https://gitlab.com/optelgroup-public/meson-vs-gen
 License: MIT
 Keywords: visualstudio,meson
 Author: Charles Brunet
 Author-email: charles.brunet@optelgroup.com
 Requires-Python: >=3.9,<4.0
@@ -103,15 +103,21 @@
 
 
 The config file contains the following keys:
 
 - `outputdir`: (optional) Where to generate the solution files, if not specified
   on the command line. Default is to use current dir.
 - `projectdir`: (optional) Name of a subdirectory where to write project files.
-- `case_insensitive_targets`: If true, lower case targets match project names containing uppercase characters.
+- `case_insensitive_targets`: (optional) If true, lower case targets match project names containing uppercase characters.
+- `only_relative_files`: (optional) If true, do not add files outside target source dir
+                         (i.e. where target meson.build file is located) into the project.
+- `include_from_env`: (optional) If true, will use `INCLUDE` env var for system include path.
+                                 If 'auto', will use `INCLUDE` if it is defined.
+                                 If false (default), will no rewrite the include path.
+                                 This is useful when using a different build tools version that the IDE.                         
 - `configs`: map build directories to config names.
 - `archs`: (optional) map cpu_family to arch name. If not specified,
   use the cpu_family as the arch name.
 - `projects`: The projects to generate. See project specifications below
   for more details.
 - `solutions`: The solutions to generate. See solution specifications below
   for more details.
@@ -124,14 +130,17 @@
 
 If the value is a boolean, `true` means to generate the project with default settings,
 and `false` means to not generate that project.
 
 If the value is a map, the following keys are recognized:
 
 - `target`: the build target name. `true` means to use the project name as the target name.
+            If target name begins with `dep:`, this is the name of an internal dependency object,
+            used for a header only project. This project will not compile, but will display files
+            from that dependency.
   `all` is used for a target that generates all targets.
 - `subdir`: if specified, put the generated project into that subdir of the project dir.
 
 #### Solution specifications
 
 For each solution, the key is the name of the solution to generate.
 
@@ -166,22 +175,26 @@
 
 You can also modify or override the `cpu_arch` dictionary,
 mapping cpu_family to arch name for the solution and projects.
 
 The next step is to call `set_config`. The method takes the following arguments:
 - `builddir`: meson build dir, absolute, or relative to `self.basedir`.
 - `name`: (optional) config name to use (default is builddir name).
+- `use_include_from_env`: (optional) If `True`, will use the `INCLUDE` env var
+                          as system include path.
 
 The `project` method is used to create a `VcxProj` object. Arguments are:
 - `name`: The project name.
 - `target`: (optional) The build target name. Default is project name.
 - `subdir`: (optional) Subdir (relative to projectdir) where to write the project.
   If `True`, the subdir is the project name. If `False`, no subdir is used.
 - `update`: (optional) If `True`, update existing project instead of overwriting it.
   Default is `True`.
+- `only_relative_files`: (optional) If `True`, will not reference source files that
+                         are not relative to the project root.
 
 The method returns a `VcxProj` object.
 
 The `solution` method is used to create a `SolutionFile` object.
 Arguments are:
 - `name`: The solution name.
 - `update`: Whether to update existing files instead of overwriting them.
```

