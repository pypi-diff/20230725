# Comparing `tmp/sbpack-2023.6.20rc2-py3-none-any.whl.zip` & `tmp/sbpack-2023.6.20rc3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 29559 bytes, number of entries: 17
+Zip file size: 30739 bytes, number of entries: 17
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 11:19 sbpack/__init__.py
 -rw-r--r--  2.0 unx     5781 b- defN 23-May-09 11:19 sbpack/lib.py
 -rw-r--r--  2.0 unx    13365 b- defN 23-May-09 11:19 sbpack/pack.py
 -rw-r--r--  2.0 unx     7929 b- defN 23-Jun-22 11:09 sbpack/schemadef.py
 -rw-r--r--  2.0 unx     3064 b- defN 23-May-09 11:19 sbpack/unpack.py
--rw-r--r--  2.0 unx       30 b- defN 23-Jul-12 10:22 sbpack/version.py
+-rw-r--r--  2.0 unx       30 b- defN 23-Jul-12 11:12 sbpack/version.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 11:19 sbpack/noncwl/__init__.py
 -rw-r--r--  2.0 unx     1591 b- defN 23-May-09 11:19 sbpack/noncwl/copy.py
--rw-r--r--  2.0 unx    19256 b- defN 23-Jul-12 08:37 sbpack/noncwl/nextflow.py
--rw-r--r--  2.0 unx     5666 b- defN 23-Jul-12 08:39 sbpack/noncwl/utils.py
+-rw-r--r--  2.0 unx    20436 b- defN 23-Jul-25 09:01 sbpack/noncwl/nextflow.py
+-rw-r--r--  2.0 unx     8520 b- defN 23-Jul-24 09:04 sbpack/noncwl/utils.py
 -rw-r--r--  2.0 unx    10528 b- defN 23-May-09 11:19 sbpack/noncwl/wdl.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/LICENSE
--rw-r--r--  2.0 unx     7479 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/WHEEL
--rw-r--r--  2.0 unx      214 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1350 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/RECORD
-17 files, 87709 bytes uncompressed, 27355 bytes compressed:  68.8%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-25 11:41 sbpack-2023.6.20rc3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7479 b- defN 23-Jul-25 11:41 sbpack-2023.6.20rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 11:41 sbpack-2023.6.20rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      214 b- defN 23-Jul-25 11:41 sbpack-2023.6.20rc3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-25 11:41 sbpack-2023.6.20rc3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1350 b- defN 23-Jul-25 11:41 sbpack-2023.6.20rc3.dist-info/RECORD
+17 files, 91743 bytes uncompressed, 28535 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: sbpack/noncwl/utils.py
 Comment: 
 
 Filename: sbpack/noncwl/wdl.py
 Comment: 
 
-Filename: sbpack-2023.6.20rc2.dist-info/LICENSE
+Filename: sbpack-2023.6.20rc3.dist-info/LICENSE
 Comment: 
 
-Filename: sbpack-2023.6.20rc2.dist-info/METADATA
+Filename: sbpack-2023.6.20rc3.dist-info/METADATA
 Comment: 
 
-Filename: sbpack-2023.6.20rc2.dist-info/WHEEL
+Filename: sbpack-2023.6.20rc3.dist-info/WHEEL
 Comment: 
 
-Filename: sbpack-2023.6.20rc2.dist-info/entry_points.txt
+Filename: sbpack-2023.6.20rc3.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbpack-2023.6.20rc2.dist-info/top_level.txt
+Filename: sbpack-2023.6.20rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: sbpack-2023.6.20rc2.dist-info/RECORD
+Filename: sbpack-2023.6.20rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbpack/version.py

```diff
@@ -1 +1 @@
-__version__ = "2023.06.20rc2"
+__version__ = "2023.06.20rc3"
```

## sbpack/noncwl/nextflow.py

```diff
@@ -10,14 +10,19 @@
 
 from nf_core.schema import PipelineSchema
 from sbpack.version import __version__
 from sbpack.noncwl.utils import (
     get_dict_depth,
     zip_and_push_to_sb,
     get_readme,
+    get_tower_yml,
+    get_entrypoint,
+    get_config_files,
+    parse_config_file,
+    create_profile_enum,
     update_schema_code_package,
     install_or_upgrade_app,
     validate_inputs,
     GENERIC_FILE_ARRAY_INPUT,
     GENERIC_OUTPUT_DIRECTORY,
     WRAPPER_REQUIREMENTS,
     SKIP_NEXTFLOW_TOWER_KEYS,
@@ -34,14 +39,15 @@
     def __init__(self, workflow_path, dump_schema=False, sb_doc=None):
         self.sb_wrapper = dict()
         self.nf_ps = PipelineSchema()
         self.sb_package_id = None
         self.workflow_path = workflow_path
         self.dump_schema = dump_schema
         self.nf_schema_path = None
+        self.nf_config_files = None
         self.sb_doc = sb_doc
         self.executor_version = None
         self.output_schemas = None
         self.input_schemas = None
 
     @staticmethod
     def nf_schema_type_mapper(input_type_string):
@@ -75,23 +81,22 @@
         """
         return {
             'default': 'sbg:toolDefaultValue',
             'description': 'label',
             'help_text': 'doc',
         }
 
-    def nf_to_sb_input_mapper(self, port_id, port_data, required=False):
+    def nf_to_sb_input_mapper(self, port_id, port_data):
         """
         Convert a single input from Nextflow schema to SB schema
         """
         sb_input = dict()
         sb_input['id'] = port_id
         sb_input['type'] = self.nf_schema_type_mapper(port_data)
-        if not required:
-            sb_input['type'].append('null')
+        sb_input['type'].append('null')
         for nf_field, sb_field in self.nf_cwl_port_map().items():
             if nf_field in port_data:
                 sb_input[sb_field] = port_data[nf_field]
         sb_input['inputBinding'] = {
             'prefix': f'--{port_id}',
         }
         return sb_input
@@ -102,18 +107,21 @@
         definition contains multiple properties
         """
         cwl_inputs = list()
         for port_id, port_data in definition['properties'].items():
             cwl_inputs.append(self.nf_to_sb_input_mapper(
                 port_id,
                 port_data,
-                required=port_id in definition.get('required', [])),
-            )
+            ))
             # Nextflow schema field "required" lists input_ids
-            # for required inputs
+            # for required inputs.
+            # Reason we are not using definition.get('required', []) any longer
+            # is that some inputs can be contained in the profile. This means
+            # that they do not have to be provided explicitly through the
+            # command line.
         return cwl_inputs
 
     def nf_schema_build(self):
         """
         Build nextflow schema using nf_core schema build feature and save to
         a file
         """
@@ -180,14 +188,26 @@
             for file in self.input_schemas:
                 if file.name == self.nf_schema_path:
                     continue
                 if file.name.split('.').pop().lower() in \
                         ['yaml', 'yml', 'json', 'cwl']:
                     cwl_inputs.extend(self.parse_cwl(file, 'inputs'))
 
+        # Add profiles to the input
+        self.nf_config_files = get_config_files(self.workflow_path)
+        profiles = []
+        for path in self.nf_config_files:
+            profiles.extend(list(parse_config_file(path).keys()))
+
+        profiles = sorted(list(set(profiles)))
+
+        if profiles:
+            cwl_inputs.append(create_profile_enum(profiles))
+
+        # Add the generic file array input - auxiliary files
         cwl_inputs.append(GENERIC_FILE_ARRAY_INPUT)
 
         input_ids = set()
         for inp in cwl_inputs:
             base_id = inp['id']
             id_ = base_id
             i = 1
@@ -293,15 +313,15 @@
                         "name": clean_id
                     }
                 ]
             }
 
         # Case 2: Output is a File type
         elif re.fullmatch(file_pattern, key):
-            # create a list of files outptu
+            # create a list of files output
             converted_cwl_output = {
                 id_key: clean_id,
                 "label": name,
                 "type": "File[]?",
                 "outputBinding": {
                     "glob": key
                 }
@@ -330,15 +350,15 @@
         :return: list of outputs in CWL format.
         """
         outputs = list()
         yml_schema = ruamel.yaml.safe_load(yml_file)
 
         for key, value in yml_schema.items():
             # Tower yml file can use "tower" key in the yml file to designate
-            # some of the configurations tower uses. Since these are not output
+            # some configurations tower uses. Since these are not output
             # definitions, we skip these.
             if key in SKIP_NEXTFLOW_TOWER_KEYS and \
                     yml_file == 'tower.yml':
                 continue
             outputs.append(
                 self.make_output_type(key, value)
             )
@@ -387,14 +407,19 @@
     ):  # default nextflow entrypoint
         """
         Generate an SB app for a nextflow workflow, OR edit the one created and
         defined by the user
         """
         if output_schemas:
             self.output_schemas = output_schemas
+        if get_tower_yml(self.workflow_path):
+            if not self.output_schemas:
+                self.output_schemas = []
+            self.output_schemas.append(open(get_tower_yml(self.workflow_path)))
+
         if input_schemas:
             self.input_schemas = input_schemas
 
         if sb_schema:
             new_code_package = self.sb_package_id if \
                 self.sb_package_id else None
             schema_ext = sb_schema.split('/')[-1].split('.')[-1]
@@ -439,22 +464,25 @@
         help="SB platform profile as set in the SB API credentials file.",
     )
     parser.add_argument(
         "--appid", required=True,
         help="Takes the form {user or division}/{project}/{app_id}.",
     )
     parser.add_argument(
-        "--entrypoint", required=True,
-        help="Relative path to the workflow from the main workflow directory",
-    )
-    parser.add_argument(
         "--workflow-path", required=True,
         help="Path to the main workflow directory",
     )
     parser.add_argument(
+        "--entrypoint", required=False,
+        help="Relative path to the workflow from the main workflow directory. "
+             "If not provided, 'main.nf' will be used if available. "
+             "If not available, any '.nf' located in the workflow-path will "
+             "be used.",
+    )
+    parser.add_argument(
         "--sb-package-id", required=False,
         help="Id of an already uploaded package",
     )
     parser.add_argument(
         "--sb-doc", required=False,
         help="Path to a doc file for sb app. If not provided, README.md "
              "will be used if available",
@@ -503,14 +531,16 @@
              " if are string (str), file (file), directory (dir), list of file"
              " (files), or list of directory (dirs) type inputs.",
     )
 
     args = parser.parse_args()
 
     # Preprocess CLI parameter values
+    entrypoint = args.entrypoint or \
+        get_entrypoint(args.workflow_path) or 'main.nf'
 
     sb_doc = None
     if args.sb_doc:
         with open(args.sb_doc, 'r') as f:
             sb_doc = f.read()
 
     # Init api and nf_wrapper
@@ -528,15 +558,15 @@
         nf_wrapper.sb_package_id = zip_and_push_to_sb(
             api=api,
             workflow_path=args.workflow_path,
             project_id=project_id,
             folder_name='nextflow_workflows'
         )
         sb_app = nf_wrapper.generate_sb_app(
-            sb_entrypoint=args.entrypoint,
+            sb_entrypoint=entrypoint,
             sb_schema=args.sb_schema,
             executor_version=args.executor_version,
             manual_validation=args.manual_validation
         )
 
     else:
         # Zip and upload
@@ -554,15 +584,15 @@
         # Build or update nextflow inputs schema
         if not args.input_schema_files:
             nf_schema_path = nf_wrapper.nf_schema_build()
             nf_wrapper.nf_schema_path = nf_schema_path
 
         # Create app
         sb_app = nf_wrapper.generate_sb_app(
-            sb_entrypoint=args.entrypoint,
+            sb_entrypoint=entrypoint,
             executor_version=args.executor_version,
             output_schemas=args.output_schema_files,
             input_schemas=args.input_schema_files,
             manual_validation=args.manual_validation
         )
         # Dump app to local file
         out_format = 'json' if args.json else 'yaml'
```

## sbpack/noncwl/utils.py

```diff
@@ -1,34 +1,35 @@
 import os
 import time
 import shutil
 import logging
 import json
 import yaml
+import re
 from sevenbridges.errors import NotFound
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 PACKAGE_SIZE_LIMIT = 100 * 1024 * 1024
 
 # A generic SB input array of files that should be available on the
 # instance but are not explicitly provided to the execution as wdl params.
 GENERIC_FILE_ARRAY_INPUT = {
-    "type": "File[]?",
     "id": "auxiliary_files",
+    "type": "File[]?",
     "label": "Auxiliary files",
     "doc": "List of files not added as explicit workflow inputs but "
            "required for workflow execution."
 }
 
 GENERIC_OUTPUT_DIRECTORY = {
     "id": "nf_workdir",
+    "type": "Directory?",
     "label": "Work Directory",
-    "type": "Directory",
     "doc": "This is a template output. "
            "Please change glob to directories specified in "
            "publishDir in the workflow.",
     "outputBinding": {
         "glob": "work"
     }
 }
@@ -43,27 +44,58 @@
         "listing": [
             "$(inputs.auxiliary_files)"
         ]
     }
 ]
 
 
+# Keys that should be skipped when parsing nextflow tower yaml file
 SKIP_NEXTFLOW_TOWER_KEYS = [
     'tower',
     'mail',
 ]
 
 
+def create_profile_enum(profiles: list):
+    """
+    If profiles are defined in the config file, this input stores the profiles
+    They are added to the commandline as -profile foo,bar,foobar
+    :param profiles: list of profiles
+    :return: Profiles enum array input
+    """
+    return {
+        "id": "profile",
+        "type": [
+            "null",
+            {
+                "type": "array",
+                "items": {
+                    "type": "enum",
+                    "name": "profile",
+                    "symbols": profiles
+                }
+            }
+        ],
+        "label": "Profiles",
+        "doc": "Select which profile(s) you want to use for task execution.",
+        "inputBinding": {
+            "prefix": "-profile",
+            "itemSeparator": ",",
+            "shellQuote": False,
+        }
+    }
+
+
 def validate_inputs(inputs):
     types = {
-        'str': 'string',
-        'file': 'File',
-        'dir': 'Directory',
-        'files': 'File[]',
-        'dirs': 'Directory[]'
+        'str': 'string?',
+        'file': 'File?',
+        'dir': 'Directory?',
+        'files': 'File[]?',
+        'dirs': 'Directory[]?'
     }
     exit_codes = ['e', 'exit', 'quit', 'q']
 
     for input_ in inputs:
         if 'string' in input_['type']:
             new_type = input(f'What input type is "{input_["id"]}"?\n')
             while new_type.lower() not in \
@@ -74,17 +106,14 @@
                 for key, val in types.items():
                     print(f"\t{key}: {val}")
                 new_type = input()
             if new_type in exit_codes:
                 break
 
             nt = types[new_type]
-            input_['type'].remove('string')
-            if 'null' in input_['type']:
-                nt += '?'
             input_['type'] = nt
     return inputs
 
 
 def get_dict_depth(dict_, level=0):
     """
     Find the depth of the dictionary. Example:
@@ -107,37 +136,41 @@
 def zip_and_push_to_sb(api, workflow_path, project_id, folder_name):
     """
     Create .zip package file. Upload .zip file to the designated folder
     for packages on SevenBridges Platform. Delete local .zip file.
     """
 
     basename = os.path.basename(os.path.abspath(workflow_path)) + '_' + \
-               time.strftime("%Y%m%d-%H%M%S")
+        time.strftime("%Y%m%d-%H%M%S")
 
     zip_path = os.path.join(os.path.dirname(workflow_path), basename + '.zip')
     shutil.make_archive(zip_path[:-4], 'zip', root_dir=workflow_path,
                         base_dir='./')
 
     if os.path.getsize(zip_path) > PACKAGE_SIZE_LIMIT:
         logger.error(f"File size too big: {os.path.getsize(zip_path)}")
         raise FileExistsError  # Add the right error
 
-    folder_found = list(api.files.query(project=project_id, names=[folder_name],
-                                        limit=100).all())
+    folder_found = list(api.files.query(
+        project=project_id,
+        names=[folder_name],
+        limit=100,
+    ).all())
 
     if not folder_found:
         folder_created = api.files.create_folder(
             project=api.projects.get(project_id),
             name=folder_name
         )
         folder_id = folder_created.id
     else:
         folder_id = folder_found[0].id
 
-    print(f'Uploading file {zip_path}, please wait for the upload to complete.')
+    print(f'Uploading file {zip_path}, '
+          f'please wait for the upload to complete.')
     u = api.files.upload(zip_path, parent=folder_id, overwrite=False)
 
     uploaded_file_id = u.result().id
     print(f'Upload complete!')
 
     os.remove(zip_path)
     print(f'Local file {zip_path} deleted.')
@@ -151,14 +184,88 @@
     """
     for file in os.listdir(path):
         if file.lower() == 'readme.md':
             return os.path.join(path, file)
     return None
 
 
+def get_tower_yml(path):
+    """
+    Find tower.yml file is there is one in the path folder
+    """
+    for file in os.listdir(path):
+        if file.lower() == 'tower.yml':
+            return os.path.join(path, file)
+    return None
+
+
+def get_entrypoint(path):
+    """
+    Auto find main.nf or similar file is there is one in the path folder.
+    """
+    possible_paths = []
+    for file in os.listdir(path):
+        if file.lower() == 'main.nf':
+            return file
+
+        if file.lower().endswith('.nf'):
+            possible_paths.append(file)
+
+    if possible_paths:
+        return possible_paths.pop()
+    return None
+
+
+def get_config_files(path):
+    """
+    Auto find config files.
+    """
+    paths = []
+    for file in os.listdir(path):
+        if file.lower().endswith('.config'):
+            paths.append(os.path.join(path, file))
+    return paths or None
+
+
+def parse_config_file(file_path):
+    profiles_text = ""
+
+    with open(file_path, 'r') as file:
+        found_profiles = False
+        brackets = 0
+
+        for line in file.readlines():
+            if found_profiles:
+                profiles_text += line
+                brackets += line.count("{") - line.count("}")
+
+            if brackets < 0:
+                break
+
+            if re.findall(r'profiles\s+\{', line):
+                profiles_text += "{\n"
+                found_profiles = True
+
+    # Extract profiles using regex
+    profiles = {}
+    pattern = re.compile(r'^\s*(\w+)\s*{([^}]+)}', re.MULTILINE | re.DOTALL)
+    blocks = re.findall(pattern, profiles_text)
+    for name, content in blocks:
+        settings = dict(re.findall(r'\s*([a-zA-Z.]+)\s*=\s*(.*)', content))
+        profiles[name] = settings
+        include_path = re.findall(
+            r'includeConfig\s+[\'\"]([a-zA-Z_.\\/]+)[\'\"]', content)
+        if include_path:
+            profiles[name]['includeConfig'] = include_path
+
+    # return currently returns includeConfig and settings, which are not used
+    # but could be used in the future versions of sbpack
+    return profiles
+
+
 def update_schema_code_package(sb_schema, schema_ext, new_code_package):
     """
     Update the package in the sb_schema
     """
     if schema_ext.lower() in ['json', 'cwl']:
         with open(sb_schema, 'r') as file:
             sb_schema_json = json.load(file)
```

## Comparing `sbpack-2023.6.20rc2.dist-info/LICENSE` & `sbpack-2023.6.20rc3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbpack-2023.6.20rc2.dist-info/METADATA` & `sbpack-2023.6.20rc3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbpack
-Version: 2023.6.20rc2
+Version: 2023.6.20rc3
 Summary: Command line tool to upload and download CWL to and from SB powered platforms.
 Home-page: UNKNOWN
 Author: Seven Bridges
 Author-email: pavle.marinkovic@velsera.com
 Maintainer: Seven Bridges
 Maintainer-email: pavle.marinkovic@velsera.com
 License: UNKNOWN
```

## Comparing `sbpack-2023.6.20rc2.dist-info/RECORD` & `sbpack-2023.6.20rc3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 sbpack/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sbpack/lib.py,sha256=iLN5s31rS9Mg64teYZLk0Cicdjuyb6KdwCjL52r1nrQ,5781
 sbpack/pack.py,sha256=4vutKrWeas4NhtaLcHKIWfp-8pHMo3hkWR75oz6GTZw,13365
 sbpack/schemadef.py,sha256=9UVZNi5nUMJz5ZZM9j4z53X8Svizmc_eUTtl0mTapB8,7929
 sbpack/unpack.py,sha256=amyfuytRxvsz0-RARfP1Hm4tbpmMVCfLSaM8U3woh-o,3064
-sbpack/version.py,sha256=cbvH7ow8kBCTtMJ_Hx1HXp7gj58hLztjgRdMM6LU6mg,30
+sbpack/version.py,sha256=6IZQFwrweR7fNuoLQu_McUQGjWgcn4OfSiQxnp_TtO0,30
 sbpack/noncwl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sbpack/noncwl/copy.py,sha256=oMAJrGJ6FiU4BF2pyqUOcdTam9Ft64vL8n-ywAKIne8,1591
-sbpack/noncwl/nextflow.py,sha256=hyabWMHRYMquFfuc0RKNeW6QhcLQJFK5HlqwE9V1Wt8,19256
-sbpack/noncwl/utils.py,sha256=Pfojwv5FYqJ-TZ1ZrkMytAUkgBB5IHwhdL0aOvUWrfo,5666
+sbpack/noncwl/nextflow.py,sha256=bkz35nOARt-hKDgEO-1Olwc9W_fVuBscBHeHeyH4chQ,20436
+sbpack/noncwl/utils.py,sha256=FdhMB6Ae7DNaUCTl4fyomVmYUYTu0uMuOGPSwbbDryM,8520
 sbpack/noncwl/wdl.py,sha256=-CqDLqbCiGOhnG5iEUJC2FMXZmorFggtGpeDtBpHWgU,10528
-sbpack-2023.6.20rc2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbpack-2023.6.20rc2.dist-info/METADATA,sha256=4wGl5vDVxLmb5oosqeKcQVYDkijcxKbaHnhn0x2IKVc,7479
-sbpack-2023.6.20rc2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sbpack-2023.6.20rc2.dist-info/entry_points.txt,sha256=FkTSv3CUlZDSBAYV9d12g1Xn5baiWk0-w1giWiP7QtU,214
-sbpack-2023.6.20rc2.dist-info/top_level.txt,sha256=jYfNbA_EM0kCUdebAs2xxFukxE1XlzB_BbAr4t25Jmg,7
-sbpack-2023.6.20rc2.dist-info/RECORD,,
+sbpack-2023.6.20rc3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbpack-2023.6.20rc3.dist-info/METADATA,sha256=pPYE8__LFfRpFlYjJFuBRbRNqUJB3GkTmKUx4-Uf1iA,7479
+sbpack-2023.6.20rc3.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sbpack-2023.6.20rc3.dist-info/entry_points.txt,sha256=FkTSv3CUlZDSBAYV9d12g1Xn5baiWk0-w1giWiP7QtU,214
+sbpack-2023.6.20rc3.dist-info/top_level.txt,sha256=jYfNbA_EM0kCUdebAs2xxFukxE1XlzB_BbAr4t25Jmg,7
+sbpack-2023.6.20rc3.dist-info/RECORD,,
```

