# Comparing `tmp/gitautobackup-1.2.0.0.tar.gz` & `tmp/gitautobackup-2.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitautobackup-1.2.0.0.tar", last modified: Tue Jun  6 18:01:14 2023, max compression
+gzip compressed data, was "gitautobackup-2.0.0.0.tar", last modified: Tue Jul 25 18:19:23 2023, max compression
```

## Comparing `gitautobackup-1.2.0.0.tar` & `gitautobackup-2.0.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 18:01:13.998214 gitautobackup-1.2.0.0/
--rw-rw-rw-   0        0        0    17098 2023-05-30 17:53:38.000000 gitautobackup-1.2.0.0/LICENSE
--rw-rw-rw-   0        0        0    46152 2023-06-06 18:01:13.994214 gitautobackup-1.2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7399 2023-06-06 17:48:44.000000 gitautobackup-1.2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 18:01:13.967295 gitautobackup-1.2.0.0/gitautobackup.egg-info/
--rw-rw-rw-   0        0        0    46152 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      158 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-06 18:01:13.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-06 18:01:11.000000 gitautobackup-1.2.0.0/gitautobackup.egg-info/zip-safe
--rw-rw-rw-   0        0        0    23671 2023-06-06 18:00:36.000000 gitautobackup-1.2.0.0/gitautobackup.py
--rw-rw-rw-   0        0        0     3198 2023-06-01 18:32:58.000000 gitautobackup-1.2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 18:01:13.999773 gitautobackup-1.2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 18:19:23.570771 gitautobackup-2.0.0.0/
+-rw-rw-rw-   0        0        0    17098 2023-05-30 17:53:38.000000 gitautobackup-2.0.0.0/LICENSE
+-rw-rw-rw-   0        0        0    46206 2023-07-25 18:19:23.557191 gitautobackup-2.0.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7453 2023-07-25 00:17:20.000000 gitautobackup-2.0.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 18:19:23.542429 gitautobackup-2.0.0.0/gitautobackup.egg-info/
+-rw-rw-rw-   0        0        0    46206 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      151 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-25 18:19:23.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 18:19:21.000000 gitautobackup-2.0.0.0/gitautobackup.egg-info/zip-safe
+-rw-rw-rw-   0        0        0    31039 2023-07-25 11:21:52.000000 gitautobackup-2.0.0.0/gitautobackup.py
+-rw-rw-rw-   0        0        0     3160 2023-07-25 00:26:17.000000 gitautobackup-2.0.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 18:19:23.570771 gitautobackup-2.0.0.0/setup.cfg
```

### Comparing `gitautobackup-1.2.0.0/LICENSE` & `gitautobackup-2.0.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitautobackup-1.2.0.0/PKG-INFO` & `gitautobackup-2.0.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 1.2.0.0
+Version: 2.0.0.0
 Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -443,17 +443,17 @@
 Here are a few of the possible arguments to use:
 
 - ``-p`` / ``--path`` specifies the repository path
 - ``-m`` / ``--message`` specifies the commit's message.
 - ``-t`` / ``--tag`` sets a tag for the commit
 - ``-a`` / ``--archive`` / ``--archive_path`` sets a path for a archive file to be made. If this isn't used a archive file will not be made.
 - ``-f`` / ``--force`` / ``--force_commit`` makes a commit be made even if nothing was changed
-- ``--fc`` / ``--force_compress`` forces the repository's database to always be compressed, even if its not really necessary. This cannot be combined with ``--fnc`` or ``--fca``
-- ``--fnc`` / ``--force_no_compress`` forces the repository's database to never be compressed, even if it might be beneficial. This cannot be combined with ``--fc`` or ``--fca``
-- ``--fca`` / ``--force_compress_aggressive`` forces the repository's database compressed aggressively (taking a much longer time), even if its not necessary. This cannot be combined with ``--fc`` or ``--fnc``
+- ``--fc`` / ``--force_cleanup`` forces the repository's database to always be cleaned, even if its not really necessary. This cannot be combined with ``--fnc`` or ``--fca``
+- ``--fnc`` / ``--force_no_cleanup`` forces the repository's database to never be cleaned, even if it might be beneficial. This cannot be combined with ``--fc`` or ``--fca``
+- ``--fca`` / ``--force_cleanup_aggressive`` forces the repository's database cleaned aggressively (taking a much longer time), even if its not necessary. This cannot be combined with ``--fc`` or ``--fnc``
 - ``-v`` / ``--verbose`` makes the output of the program more noisy. This cannot be combined with ``-q``
 - ``-q`` / ``--quiet`` greatly reduces the output of the program. This cannot be combined with ``-v``
 
 There are also the traditional arguments that report various information about this software then exit:
 
 - ``--ver`` / ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
 - ``-h`` / ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
@@ -479,39 +479,39 @@
 
 ```bash:
 python -m gitautobackup "./repo" -m "automatic backup after big change"
 ```
 
 ## Module Interface
 
-This module can also be interfaced with as a normal module. The points of intreast include the ``main`` function for interfacing with this just like it was the command line (this means **parsing the arguments**, meaning that the features outlined in the Command Line Interface section above), and the ``auto_git_backup`` command for a more direct ussage of the command.
-While both can manage to acheave the same result its suggested to use ``auto_git_backup`` unless there is a specific reason to use ``main``.
+This module can also be interfaced with as a normal module. The points of intreast include the ``main`` function for interfacing with this just like it was the command line (this means **parsing the arguments**, meaning that the features outlined in the Command Line Interface section above), and the ``main_cli`` command for a more direct ussage of the command.
+While both can manage to acheave the same result its suggested to use ``main_cli`` unless there is a specific reason to use ``main``.
 
 More information about this module can be found in the main file as all functions have been documented in there.
 
 ### Module Example
 
 ```python:
-from gitautobackup import auto_git_backup
+from gitautobackup import main_cli
 
 myrepopath = "./project/repo/" #this assumes the folder "./project/repo/" has a already initialised non bare git repository already.
 
-if auto_git_backup(myrepopath, commit_message = "Automatic Backup No. 1", force_commit = True):
+if main_cli(myrepopath, commit_message = "Automatic Backup No. 1", force_commit = True):
   print("Backup successful")
 else:
   print("Backup failure")
 ```
 
 ## Licence
 
 This is licenced under the Mozilla Public License 2.0 (MPL 2.0) Licence. See the ``Licence`` file in this repository for more information.
 
 ## Credits
 
-This project uses the ``pathlib``, ``GitPython`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
+This project uses the ``pathlib`` (or alternatively ``pathlib2`` if ``pathlib2`` is available to import and ``pathlib`` is not), ``GitPython`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
 
 While not required, feel free to credit "*Markus Hammer*" (or just "*Markus*") if you find this code or script usefull for whatever you may be doing with it.
 
 **Thanks!**
 
 Mozilla Public License Version 2.0
 ==================================
```

### Comparing `gitautobackup-1.2.0.0/README.md` & `gitautobackup-2.0.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 Here are a few of the possible arguments to use:
 
 - ``-p`` / ``--path`` specifies the repository path
 - ``-m`` / ``--message`` specifies the commit's message.
 - ``-t`` / ``--tag`` sets a tag for the commit
 - ``-a`` / ``--archive`` / ``--archive_path`` sets a path for a archive file to be made. If this isn't used a archive file will not be made.
 - ``-f`` / ``--force`` / ``--force_commit`` makes a commit be made even if nothing was changed
-- ``--fc`` / ``--force_compress`` forces the repository's database to always be compressed, even if its not really necessary. This cannot be combined with ``--fnc`` or ``--fca``
-- ``--fnc`` / ``--force_no_compress`` forces the repository's database to never be compressed, even if it might be beneficial. This cannot be combined with ``--fc`` or ``--fca``
-- ``--fca`` / ``--force_compress_aggressive`` forces the repository's database compressed aggressively (taking a much longer time), even if its not necessary. This cannot be combined with ``--fc`` or ``--fnc``
+- ``--fc`` / ``--force_cleanup`` forces the repository's database to always be cleaned, even if its not really necessary. This cannot be combined with ``--fnc`` or ``--fca``
+- ``--fnc`` / ``--force_no_cleanup`` forces the repository's database to never be cleaned, even if it might be beneficial. This cannot be combined with ``--fc`` or ``--fca``
+- ``--fca`` / ``--force_cleanup_aggressive`` forces the repository's database cleaned aggressively (taking a much longer time), even if its not necessary. This cannot be combined with ``--fc`` or ``--fnc``
 - ``-v`` / ``--verbose`` makes the output of the program more noisy. This cannot be combined with ``-q``
 - ``-q`` / ``--quiet`` greatly reduces the output of the program. This cannot be combined with ``-v``
 
 There are also the traditional arguments that report various information about this software then exit:
 
 - ``--ver`` / ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
 - ``-h`` / ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
@@ -74,36 +74,36 @@
 
 ```bash:
 python -m gitautobackup "./repo" -m "automatic backup after big change"
 ```
 
 ## Module Interface
 
-This module can also be interfaced with as a normal module. The points of intreast include the ``main`` function for interfacing with this just like it was the command line (this means **parsing the arguments**, meaning that the features outlined in the Command Line Interface section above), and the ``auto_git_backup`` command for a more direct ussage of the command.
-While both can manage to acheave the same result its suggested to use ``auto_git_backup`` unless there is a specific reason to use ``main``.
+This module can also be interfaced with as a normal module. The points of intreast include the ``main`` function for interfacing with this just like it was the command line (this means **parsing the arguments**, meaning that the features outlined in the Command Line Interface section above), and the ``main_cli`` command for a more direct ussage of the command.
+While both can manage to acheave the same result its suggested to use ``main_cli`` unless there is a specific reason to use ``main``.
 
 More information about this module can be found in the main file as all functions have been documented in there.
 
 ### Module Example
 
 ```python:
-from gitautobackup import auto_git_backup
+from gitautobackup import main_cli
 
 myrepopath = "./project/repo/" #this assumes the folder "./project/repo/" has a already initialised non bare git repository already.
 
-if auto_git_backup(myrepopath, commit_message = "Automatic Backup No. 1", force_commit = True):
+if main_cli(myrepopath, commit_message = "Automatic Backup No. 1", force_commit = True):
   print("Backup successful")
 else:
   print("Backup failure")
 ```
 
 ## Licence
 
 This is licenced under the Mozilla Public License 2.0 (MPL 2.0) Licence. See the ``Licence`` file in this repository for more information.
 
 ## Credits
 
-This project uses the ``pathlib``, ``GitPython`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
+This project uses the ``pathlib`` (or alternatively ``pathlib2`` if ``pathlib2`` is available to import and ``pathlib`` is not), ``GitPython`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
 
 While not required, feel free to credit "*Markus Hammer*" (or just "*Markus*") if you find this code or script usefull for whatever you may be doing with it.
 
 **Thanks!**
```

### Comparing `gitautobackup-1.2.0.0/gitautobackup.egg-info/PKG-INFO` & `gitautobackup-2.0.0.0/gitautobackup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitautobackup
-Version: 1.2.0.0
+Version: 2.0.0.0
 Summary: A basic CLI program and python moldule that allows for quickly making and comming changes to a git repository, along with a few other tools
 Author-email: Markus Hammer <107761433+MarkusHammer@users.noreply.github.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -443,17 +443,17 @@
 Here are a few of the possible arguments to use:
 
 - ``-p`` / ``--path`` specifies the repository path
 - ``-m`` / ``--message`` specifies the commit's message.
 - ``-t`` / ``--tag`` sets a tag for the commit
 - ``-a`` / ``--archive`` / ``--archive_path`` sets a path for a archive file to be made. If this isn't used a archive file will not be made.
 - ``-f`` / ``--force`` / ``--force_commit`` makes a commit be made even if nothing was changed
-- ``--fc`` / ``--force_compress`` forces the repository's database to always be compressed, even if its not really necessary. This cannot be combined with ``--fnc`` or ``--fca``
-- ``--fnc`` / ``--force_no_compress`` forces the repository's database to never be compressed, even if it might be beneficial. This cannot be combined with ``--fc`` or ``--fca``
-- ``--fca`` / ``--force_compress_aggressive`` forces the repository's database compressed aggressively (taking a much longer time), even if its not necessary. This cannot be combined with ``--fc`` or ``--fnc``
+- ``--fc`` / ``--force_cleanup`` forces the repository's database to always be cleaned, even if its not really necessary. This cannot be combined with ``--fnc`` or ``--fca``
+- ``--fnc`` / ``--force_no_cleanup`` forces the repository's database to never be cleaned, even if it might be beneficial. This cannot be combined with ``--fc`` or ``--fca``
+- ``--fca`` / ``--force_cleanup_aggressive`` forces the repository's database cleaned aggressively (taking a much longer time), even if its not necessary. This cannot be combined with ``--fc`` or ``--fnc``
 - ``-v`` / ``--verbose`` makes the output of the program more noisy. This cannot be combined with ``-q``
 - ``-q`` / ``--quiet`` greatly reduces the output of the program. This cannot be combined with ``-v``
 
 There are also the traditional arguments that report various information about this software then exit:
 
 - ``--ver`` / ``--version`` prints the program version and then exits. You don't need a input file if you run this command.
 - ``-h`` / ``--help`` prints some details about the programs arguments and then exits. You don't need a input file if you run this command.
@@ -479,39 +479,39 @@
 
 ```bash:
 python -m gitautobackup "./repo" -m "automatic backup after big change"
 ```
 
 ## Module Interface
 
-This module can also be interfaced with as a normal module. The points of intreast include the ``main`` function for interfacing with this just like it was the command line (this means **parsing the arguments**, meaning that the features outlined in the Command Line Interface section above), and the ``auto_git_backup`` command for a more direct ussage of the command.
-While both can manage to acheave the same result its suggested to use ``auto_git_backup`` unless there is a specific reason to use ``main``.
+This module can also be interfaced with as a normal module. The points of intreast include the ``main`` function for interfacing with this just like it was the command line (this means **parsing the arguments**, meaning that the features outlined in the Command Line Interface section above), and the ``main_cli`` command for a more direct ussage of the command.
+While both can manage to acheave the same result its suggested to use ``main_cli`` unless there is a specific reason to use ``main``.
 
 More information about this module can be found in the main file as all functions have been documented in there.
 
 ### Module Example
 
 ```python:
-from gitautobackup import auto_git_backup
+from gitautobackup import main_cli
 
 myrepopath = "./project/repo/" #this assumes the folder "./project/repo/" has a already initialised non bare git repository already.
 
-if auto_git_backup(myrepopath, commit_message = "Automatic Backup No. 1", force_commit = True):
+if main_cli(myrepopath, commit_message = "Automatic Backup No. 1", force_commit = True):
   print("Backup successful")
 else:
   print("Backup failure")
 ```
 
 ## Licence
 
 This is licenced under the Mozilla Public License 2.0 (MPL 2.0) Licence. See the ``Licence`` file in this repository for more information.
 
 ## Credits
 
-This project uses the ``pathlib``, ``GitPython`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
+This project uses the ``pathlib`` (or alternatively ``pathlib2`` if ``pathlib2`` is available to import and ``pathlib`` is not), ``GitPython`` and optionally ``argparse`` modules, all very usefull python modules. Check them out if you want to make a simple CLI script like this, or for whatever else you might be up to in python. Also thank you to the developers of these modules for making these as they helped keep my sanity in check.
 
 While not required, feel free to credit "*Markus Hammer*" (or just "*Markus*") if you find this code or script usefull for whatever you may be doing with it.
 
 **Thanks!**
 
 Mozilla Public License Version 2.0
 ==================================
```

### Comparing `gitautobackup-1.2.0.0/gitautobackup.py` & `gitautobackup-2.0.0.0/gitautobackup.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,35 +10,73 @@
 
     See the github repo for more info!
     
     This project is on github here:
     https://github.com/MarkusHammer/gitautobackup
 '''
 
-from pathlib import Path
+__version__ = "2.0.0.0"
+
 from git import Repo, InvalidGitRepositoryError, GitCommandNotFound, NoSuchPathError, RepositoryDirtyError, GitError
 
 try:
+    from pathlib import Path
+except ImportError:
+    from pathlib2 import Path
+
+try:
+    from datetime import datetime
+    DATETIME_IMPORTED = True
+except ImportError:
+    DATETIME_IMPORTED = False
+
+try:
+    from argparse import ArgumentParser
+    ARGPARSE_IMPORTED = True
+except ImportError:
+    ARGPARSE_IMPORTED = False
+
+try:
+    from sys import argv as cliargv
+    CLIARGV_IMPORTED = True
+except ImportError:
+    CLIARGV_IMPORTED = False
+
+try:
+    from sys import exit as end
+    END_IMPORTED = True
+except ImportError:
+    END_IMPORTED = False
+
+try:
     from typing import Union
 except ImportError:
     from typing_extensions import Union
 
 try:
     from typing import List
 except ImportError:
     from typing_extensions import List
 
-__version__ = "1.2.0.0"
+try:
+    from typing import Tuple
+except ImportError:
+    from typing_extensions import Tuple
+
+try:
+    from typing import Callable
+except ImportError:
+    from typing_extensions import Callable
+
 
 class InvalidArchiveFormatError(GitError, Exception):
     """Raised when a format for git archive when that format is not a valid format for git archive"""    
 
     def __init__(self, given_format:str, possible_formats:Union[List[str], None] = None):
-        """_summary_
-
+        """
         Args:
             format (str): The issue causing format.
             repo_reference (Union[Repo, None], optional): A optional list of possible valid formats, or None if this cant be given.
         """
 
         self.given_format = given_format
         self.possible_formats = []
@@ -47,16 +85,16 @@
             self.possible_formats = possible_formats
 
     def __str__(self) -> str:
         return f"The format {self.given_format} is not a valid format for a archive in git. {('Valid formats are ' + ' '.join(self.possible_formats)) if len(self.possible_formats) > 0 else ''}"
 
 
 def path_hunt_dir(path: Union[Path, str, None]) -> Union['Path', None]:
-    """_summary_
-
+    """Gets the parrent directory of a file if possible.
+    
     Args:
         path (Union[Path,str,None]): The path to search for the parent directory of. If this is set to None the return value will always also be None
 
     Returns:
         Union[Path,None]: Returns a Path of the directory if a directory was found, or None if one couldn't be found
     """
 
@@ -76,14 +114,38 @@
 
     if not path.is_dir():
         return None
     else:
         return path
 
 
+def assert_file(path: Union[Path, str, None]):
+    """Asserts that a file exists and is a file
+
+    Args:
+        path (Union[Path, str, None]): The path to assert exists and is a file
+
+    Raises:
+        NoSuchPathError: The path does not exist on the system
+        FileNotFoundError: The path is not a file
+    """
+    if path is None:
+        raise NoSuchPathError()
+
+    if not isinstance(path, Path):
+        path = Path(path)
+    path = path.expanduser()
+
+    if not path.exists():
+        raise NoSuchPathError()
+
+    if not path.is_file():
+        raise FileNotFoundError
+
+
 def assert_repo(path: Union[Path, str, None], allow_bare: bool = False):
     """Raises various exceptions to test if a path is or is not a git repo. This function does not return a value, use is_repo instead if you want that.
 
     Args:
         path (Union[Path,str,None]): The path to assert is a repository. Always raises NoSuchPathError when set to None.
         allow_bare (bool, optional): Don't raise InvalidGitRepositoryError if the repository is bare. Defaults to False.
 
@@ -94,14 +156,15 @@
     """
 
     if path is None:
         raise NoSuchPathError()
 
     if not isinstance(path, Path):
         path = Path(path)
+    path = path.expanduser()
 
     if not path.exists():
         raise NoSuchPathError()
 
     if not (path.is_dir() or str(path).endswith(".git")):
         raise InvalidGitRepositoryError()
 
@@ -135,220 +198,350 @@
     Args:
         nodatetime (bool, optional): Don't allow use fo the datetime module. Defaults to False.
 
     Returns:
         str: The ideal default commit name.
     """
 
-    if not nodatetime:
-        try:
-            from datetime import datetime
-            return f"Autosave on {datetime.now()}"
-        except ImportError:
-            pass
+    if DATETIME_IMPORTED and not nodatetime:
+        return f"Autosave on {datetime.now()}"
     return "Autosave"
 
 
 def get_default_file_location() -> Union[Path, None]:
     """Returns the most relevant default file location based on how this script/module is run and what is accessable. Returns None if nothing could be determined.
 
     Returns:
         Union[Path,None]: The path that was found, it one was found. If not this will be None.
     """
 
     possiblepath = path_hunt_dir(Path.cwd())
     if possiblepath is not None and possiblepath.exists():
         return possiblepath
 
-    try:
-        from sys import (argv as cliargv)
-    except ImportError:
-        pass
-    else:
+    if CLIARGV_IMPORTED:
         if len(cliargv) > 0 and isinstance(cliargv[0], str):
             possiblepath = path_hunt_dir(cliargv[0])
             if possiblepath is not None and possiblepath.exists():
                 return possiblepath
 
     # this only really helps if this file is run as the main script.
     # Unlikely that it will be needed however because argv is almost always guaranteed
     #   to work on any system that is able to suport the mandatory requirements of this script anyway.
     # Still good for a plan c however ...
     if __name__ == "__main__":
         try:
             _ = __file__
-        except NameError:
+        except (NameError, TypeError):
             pass
         else:
             possiblepath = path_hunt_dir(__file__)
             if possiblepath is not None and possiblepath.exists():
                 return possiblepath
 
     return None
 
 
-def auto_git_backup(repo_path: Union[Path, str, None] = None,
-                    commit_message: Union[str, None] = None,
-                    further_guess_paths: bool = False,
-                    verbose: bool = True,
-                    force_commit: bool = False,
-                    tag:Union[str,None] = None,
-                    force_tag:bool = False,
-                    tag_message:Union[str, None] = None,
-                    force_compress: Union[bool, None] = None,
-                    compress_aggressive:bool = False,
-                    archive_path:Union[Path, str, None] = None,
-                    archive_format:Union[str, None] = None
-                    ) -> bool:
-    """_summary_
+def resolve_repo(repo_path: Union[Path, str, None] = None,
+                 further_guess_paths: bool = False
+                 ) -> Repo:
+    """Attempts to smartley resolve a path to find a gitrepo withing it and possibly the default path location (as given by ```get_default_file_location```) if enabled.
+
+    Args:
+        repo_path (Union[Path, str, None], optional): The path to look for a git repo in. Defaults to None.
+        further_guess_paths (bool, optional): If the path is not defined, should the default path (as given by ```get_default_file_location```) be used instead. Defaults to False.
+
+    Raises:
+        InvalidGitRepositoryError: The path exists, but is not a git repo.
+        NoSuchPathError: The path is not something that exists.
+
+    Returns:
+        Repo: The resolved git repo object.
+    """
+    
+    if further_guess_paths and repo_path is None:
+        repo_path = get_default_file_location()
+
+    if repo_path is None:
+        raise InvalidGitRepositoryError()
+
+    repo_path = Path(repo_path)
+    if not repo_path.exists():
+        raise NoSuchPathError()
+    while not is_repo(repo_path) and len(repo_path.parents) > 0:
+        repo_path = repo_path.parent
+    assert_repo(repo_path)
+
+    return Repo(repo_path)
+
+
+def print_output(msg:Union[str,None] = None, *, print_func:Callable = print):
+    """Print out and lightly format a message, only if it would not appear empty.
+
+    Args:
+        msg (Union[str,None], optional): The message to print. Defaults to None.
+        print_func (Callable, optional): Overide the print function possibly called. Defaults to the callable of ```print()```.
+    """
+    
+    if msg is None:
+        return
+
+    msg = msg.strip()
+
+    if msg != "":
+        return
+
+    print_func(msg)
+
+
+def repo_get_archive_formats(repo:Repo) -> Tuple[str]:
+    """Retrieves the possible archive formats (as git archive would accept) available to this specific repo on this specific system.
+
+    Args:
+        repo (Repo): A repository to use to query what archive formats are available.
+
+    Returns:
+        Tuple[str]: A tuple of all formats
+    """
+    return tuple(x.strip() for x in repo.git.archive("--list").split())
+
+
+def archive_repo(repo:Repo,
+                 archive_paths:Union[Path, str, List[Union[Path, str]], Tuple[Union[Path, str]]],
+                 archive_format:Union[str, None] = None,
+                 *,
+                 verbose:bool = False
+                ):
+    """Archives a repository object to the given path (or paths), with the specified format, or the default format if not provided.
+    
+    Args:
+        repo(Repo): The Repo object in question, the one to create an archive from.
+        archive_paths(Union[Path, str, List[Union[Path, str]]): The (or a list or tuple of multiple) path (as a path object or string) to save the archive to.
+        archive_format(Union[str, None], optional): The string of the archive format to use, as is returned by ```repo_get_archive_formats()```, not case sensitive. Defaults to None.
+        verbose (bool, optional): Should the outputs of the functions be passed into the terminal. Defaults to False.
+    """
+
+    if archive_format is not None:
+        archive_format = archive_format.strip()
+        valid_archive_formats = repo_get_archive_formats(repo)
+
+        if archive_format not in valid_archive_formats:
+            if archive_format.lower() in valid_archive_formats:
+                archive_format = archive_format.lower()
+            elif archive_format.upper() in valid_archive_formats:
+                archive_format = archive_format.upper()
+            else:
+                raise InvalidArchiveFormatError(archive_format, valid_archive_formats)
+
+    if not isinstance(archive_paths, (list, tuple)):
+        archive_paths = (archive_paths, )
+
+    for archive_path in archive_paths:
+        archive_path = path_hunt_dir(Path(archive_path))
+
+        cmd_args = []
+        cmd_kwargs = {"o": archive_path}
+        if verbose:
+            cmd_args.append("-v")
+        if archive_format is not None:
+            cmd_kwargs["format"] = archive_format
+        cmd_args.append("HEAD")
+
+        msg = repo.git.archive(cmd_args, **cmd_kwargs)
+        if verbose:
+            print_output(msg)
+
+
+def cleanup_repo(repo:Repo,
+                 force_cleanup: Union[bool, None] = None,
+                 cleanup_aggressive:bool = False,
+                 *,
+                 verbose:bool = False
+                ):
+    """Attempts to garbage collect the given Repo if needed or forced. Can be done aggressively if specified.
+
+    Args:
+        repo (Repo):  The Repo object in question, the one to garbage collect.
+        force_cleanup (Union[bool, None], optional): Weather or not to cleanup even if not really needed. Defaults to None.
+        cleanup_aggressive (bool, optional): If cleaning up, should it be done aggressively? Defaults to False.
+        verbose (bool, optional): Should the outputs of the functions be passed into the terminal. Defaults to False.
+    """
+    cmd_args = []
+    if cleanup_aggressive:
+        cmd_args.append("--aggressive")
+    if force_cleanup is None:
+        cmd_args.append("--auto")
+
+    msg = repo.git.gc(cmd_args)
+    if verbose:
+        print_output(msg)
+
+
+def commit_repo(repo:Repo,
+                commit_message: Union[str, None] = None,
+                force_commit: bool = False,
+                tag:Union[str,None] = None,
+                force_tag:bool = False,
+                tag_message:Union[str, None] = None,
+                *,
+                verbose:bool = False
+                ):
+    """Makes a commit of all changes to the repository, with any specified message, tag, and tag message.
+
+    Args:
+        repo (Repo): The Repo object in question, the one to commit all changes to.
+        commit_message (Union[str, None], optional): The message to add to a commit. If None or not printable (whitespace) this will be automatically generated using ```default_commit_name()``` Defaults to None.
+        force_commit (bool, optional): Make a commit even if it would not contain any changes. Defaults to False.
+        tag (Union[str,None], optional): The tag to add to the repository. No tag is added if set to None. Defaults to None.
+        force_tag (bool, optional): Overwrite a tag if it already exists. Defaults to False.
+        tag_message (Union[str, None], optional): A message to add to the tag. No message is added if set to None. Defaults to None.
+        verbose (bool, optional): Should the outputs of the functions be passed into the terminal. Defaults to False.
+    """
+
+    msg = repo.git.add("--all", "--ignore-errors")
+    if verbose:
+        print_output(msg)
+
+    if verbose:
+        print_output(repo.git.status("-s"))
+
+    cmd_args = []
+    if force_commit:
+        cmd_args.append("--allow-empty")
+    if verbose:
+        cmd_args.append("-v")
+    if commit_message is None or commit_message.strip() == "":
+        commit_message = default_commit_name()
+
+    msg = repo.git.commit(cmd_args, m=commit_message)
+    if verbose:
+        print_output(msg)
+
+    print("commit done")
+
+    if tag is not None:
+        cmd_args = []
+        cmd_kwargs = {}
+        if force_tag:
+            cmd_args.append("-f")
+        if tag_message is not None:
+            cmd_args.append("-a")
+            cmd_kwargs["m"] = tag_message
+        cmd_args.append(tag)
+        cmd_args.append('HEAD')
+
+        msg = repo.git.tag(cmd_args, **cmd_kwargs)
+        if verbose:
+            print_output(msg)
+
+    print("tag done")
+
+
+def main_cli(repo_path: Union[Path, str, None] = None,
+             further_guess_paths: bool = False,
+
+             commit_message: Union[str, None] = None,
+             force_commit: bool = False,
+             tag:Union[str,None] = None,
+             force_tag:bool = False,
+             tag_message:Union[str, None] = None,
+
+             force_cleanup: Union[bool, None] = None,
+             cleanup_aggressive:bool = False,
+
+             archive_paths:Union[Path, str, None, List[Union[Path, str]], Tuple[Union[Path, str]]] = None,
+             archive_format:Union[str, None] = None,
+
+             *,
+
+             verbose: bool = True,
+            ) -> bool:
+    """Run the main command line interface's actions. The main CLI calls this, but this may also be called as a function if using this as a module. While not suggested, if you wish to pass cli arguments instead, please use the ```main()```function instead if possible.
 
     Args:
         repo_path (Union[Path,None], optional): The path of the target git repository. If set to None and further_guess_paths is set there will be an attempts to determine this using ```get_default_file_location()```. Defaults to None.
-        commit_message (Union[str,None], optional): The message of the commit being made. If None this will be automatically generated using ```default_commit_name()```. Defaults to None.
         further_guess_paths (bool, optional): If the path is set to none, should there be attempt to automatically guess the relevant path using ```get_default_file_location()```. Defaults to False.
-        verbose (bool, optional): Should this function print out non error related messages? Defaults to True.
+
+        commit_message (Union[str,None], optional): The message of the commit being made. If None this will be automatically generated using ```default_commit_name()```. Defaults to None.
         force_commit (bool, optional): Should a commit be made even if there is nothing to be committed? Defaults to False.
         tag (Union[str,None], optional): If a tag should be created, this should be the name of that tag. If no tag is to be made, this should be None, even if tag_force is True
         force_tag (bool, optional): Create the new tag even if an old one already exists. No effect if tag is None.
         tag_message (Union[str,None], optional): Add a message to the tag, or None if the tag should have no message. No effect if tag is None.
-        force_compress (Union[bool, None], optional): Should (or shouldn't) the database be compressed despite it possibly being beneficial. True forces the database to be compressed, False forces the databest to not be compressed, and None allows for this to be automatically determined by git instead. Defaults to None.
-        compress_aggressive (bool, optional): If the repo is compressed, should it be done aggressively?
+
+        force_cleanup (Union[bool, None], optional): Should (or shouldn't) the database be cleaned despite it possibly being beneficial. True forces the database to be cleaned, False forces the databest to not be cleaned, and None allows for this to be automatically determined by git instead. Defaults to None.
+        cleanup_aggressive (bool, optional): If the repo is cleaned, should it be done aggressively?
+
         archive_path (Union[Path,None], optional): If set to None no archive will be made, otherwide a archive will be output to the given location.
         archive_format (Union[str, None], optional): If set this will override the format of the archive being outputted, if set to None it will be inferred form the path.
 
+        verbose (bool, optional): Should this function print out non error related messages? Defaults to True.
+
     Raises:
         NOTE: This may not be a comprehensive list of all possible exceptions raised, as pathlib or git may raise various other exceptions as well, however what is stated below is the behaviour explicitly defined in raise statements.
         InvalidGitRepositoryError: Raised when the folder could not be opened as a git repo, if the path couldn't possibly be a git repo (if its not a directory and does not end with ".git"), or if it can be opened but it is a bare repo and allow_bare is False.
         InvalidArchiveFormatError: Raised when the given archive format is not a valid format for git archive.
         NoSuchPathError: Raised when the path doesn't exist on the system.
 
     Returns:
-        bool: Weather or not a commit was made.
+        bool: If commit was made to the repository.
     """
 
     made_a_backup: bool = False
 
-    if verbose:
-        try:
-            from pprint import pprint
-        except ImportError:
-            pprint = print
-
-    if further_guess_paths and repo_path is None:
-        repo_path = get_default_file_location()
-
-    if repo_path is None:
-        raise InvalidGitRepositoryError()
-
-    repo_path = Path(repo_path)
-    if not repo_path.exists():
-        raise NoSuchPathError()
-    while not is_repo(repo_path) and len(repo_path.parents) > 0:
-        repo_path = repo_path.parent
-    assert_repo(repo_path)
+    repo = resolve_repo(repo_path, further_guess_paths=further_guess_paths)
 
     if verbose:
-        print(f"Opening path as repo: {repo_path} {'and forcing a commit' if force_commit else ''}...")
+        print(f"Opening path as repo: {Path(repo.common_dir).parent} {'and forcing a commit' if force_commit else ''}...")
 
-    with Repo(repo_path) as repo:
-
-        if archive_path is not None and archive_format is not None:
-            valid_archive_formats = repo.git.archive("--list").split()
-            archive_format = archive_format.strip().lower()
-            if archive_format not in valid_archive_formats:
-                raise InvalidArchiveFormatError(archive_format, valid_archive_formats)
+    with repo:
 
         if force_commit or repo.is_dirty(untracked_files=True):
+            print("Commit...")
             made_a_backup = True
+            commit_repo(repo, commit_message, force_commit, tag, force_tag, tag_message, verbose=verbose)
 
-            msg = repo.git.add("--all", "--ignore-errors")
-            if verbose and msg != "":
-                pprint(msg)
-
-            if verbose:
-                pprint(repo.git.status("-s"))
-
-            cmd_args = []
-            if force_commit:
-                cmd_args.append("--allow-empty")
-            if verbose:
-                cmd_args.append("--verbose")
-            if commit_message is None or commit_message.strip() == "":
-                commit_message = default_commit_name()
-            msg = repo.git.commit(cmd_args, m=commit_message)
-            if verbose and msg != "":
-                pprint(msg)
-
-            if tag is not None:
-                cmd_args = ["-a"]
-                cmd_kwargs = {}
-                if force_tag:
-                    cmd_args.append("-f")
-                if tag_message is not None:
-                    cmd_kwargs["m"] = tag_message
-                cmd_args.append(tag)
-                msg = repo.git.tag(cmd_args, **cmd_kwargs)
-                if verbose and msg != "":
-                    pprint(msg)
-
-        if force_compress is None or force_compress is True:
-            cmd_args = []
-            if compress_aggressive:
-                cmd_args.append("--aggressive")
-            if force_compress is None:
-                cmd_args.append("--auto")
-            msg = repo.git.gc(cmd_args)
-            if verbose and msg != "":
-                pprint(msg)
-
-        if archive_path is not None:
-            archive_path = Path(archive_path)
-            cmd_args = []
-            cmd_kwargs = {"o": archive_path}
-            if verbose:
-                cmd_args.append("-v")
-            if archive_format is not None:
-                cmd_kwargs["format"] = archive_format
-            cmd_args.append("HEAD")
-            msg = repo.git.archive(cmd_args, **cmd_kwargs)
-            if verbose and msg != "":
-                pprint(msg)
+        if force_cleanup is None or force_cleanup is True:
+            print("Cleanup...")
+            cleanup_repo(repo, force_cleanup, cleanup_aggressive, verbose=verbose)
+
+        if archive_paths is not None:
+            print("Archive...")
+            archive_repo(repo, archive_paths, archive_format, verbose=verbose)
 
     return made_a_backup
 
 
 def main(*args, prog_arg: Union[str, None] = None) -> bool:
     """A function that when used as a module acts as the main entry point of the program. This allows for you to use this as you would normally via the cli but still import this as a module.
     Please note however that argv is only intended for the cli arguments and not for the name of the script running this, thats what the optional prog_arg argument is intended for.
     Also note that this function does not handle exceptions unlike how the cli turns these into user friendly messages. This is intended as the user of a module will most likely find these exceptions usefull.
 
     Args:
-        *args (Tuple[None]): The arguments form the command line, sans the one with the name of this program (what the sys module's argv puts in the [0]th spot), thats what prog_arg is for.
+        *args (Tuple[str]): The arguments form the command line, sans the one with the name of this program (what the sys module's argv puts in the [0]th spot), thats what prog_arg is for.
         prog_arg (Union[str, None], optional): This is used for what is traditionally used as the [0]th member if argv, the name of this program as it was called in the command line. THis is however, completely optional. Defaults to None.
 
     Returns:
-        bool: weather or not a backup was made by ```auto_git_backup```
+        bool: weather or not a backup was made
     """
 
     path = None
     force_commit = False
     force_tag = False
-    force_compress = None
-    compress_aggressive = False
+    force_cleanup = None
+    cleanup_aggressive = False
     commit_message = None
     tag = None
     tag_message = None
     verbose = True
     further_guess_paths = True
     archive_path = None
     archive_format = None
 
     # parse the cli args
-    try:
-        from argparse import ArgumentParser
+    if ARGPARSE_IMPORTED:
         parser = ArgumentParser(prog=prog_arg,
                                 description="""
                                 A basic CLI program that allows for quick formatting of a .gitignore file
                                 """)
 
         parser.add_argument('-p', '--path', '-d', '--dest', '-r', '--repo',
                             dest='repo_path', action='store', default=path, type=str,
@@ -366,53 +559,62 @@
         parser.add_argument('-a', '--archive', '--ap', '--archive_path',
                             dest='archive_path', action='store', default=archive_path, type=str,
                             help="A path to the location of the desired archive to be made. If not defined no archive will be made.")
         parser.add_argument('--af', '--archive_format',
                             dest='archive_format', action='store', default=archive_format, type=str,
                             help="Force the given type of format to be used for the file. If not defined it will be taken from the given path.")
 
-        parser.add_argument('-f', '--force', '--force_commit', dest='force_commit', action='store_true', default=force_commit,
+        parser.add_argument('-f', '--force', '--force_commit',
+                            dest='force_commit', action='store_true', default=force_commit,
                             help='Push a commit to the repo even if there are no changes')
-        parser.add_argument('--ft', '--force_tag', dest='force_tag', action='store_true', default=force_tag,
+        parser.add_argument('--ft', '--force_tag',
+                            dest='force_tag', action='store_true', default=force_tag,
                             help='If a tag is to be made, force it to overwrite any existing tags that may be in it`s way')
-        force_compress_group = parser.add_mutually_exclusive_group()
-        force_compress_group.add_argument('--fnc', '--force_no_compress', dest='force_no_compress', action='store_true',
-                                          help='Skip compressing the database even if it might be usefull')
-        force_compress_group.add_argument('--fc', '--force_compress', dest='force_compress', action='store_true',
-                                          help='Compress the database even if its not quite necessary')
-        force_compress_group.add_argument('--fca', '--force_compress_aggressive', dest='force_compress_aggressive', action='store_true',
-                                          help='Compress the database aggressively, even if its not quite necessary')
+
+        force_cleanup_group = parser.add_mutually_exclusive_group()
+        force_cleanup_group.add_argument('--fnc', '--force_no_cleanup',
+                                         dest='force_no_cleanup', action='store_true',
+                                         help='Skip cleaning the database even if it might be usefull')
+        force_cleanup_group.add_argument('--fc', '--force_cleanup',
+                                         dest='force_cleanup', action='store_true',
+                                         help='cleanup the database even if its not quite necessary')
+        force_cleanup_group.add_argument('--fca', '--force_cleanup_aggressive',
+                                         dest='force_cleanup_aggressive', action='store_true',
+                                         help='cleanup the database aggressively, even if its not quite necessary')
 
         loudness_group = parser.add_mutually_exclusive_group()
-        loudness_group.add_argument("-v", "--verbose", dest="verbose",
-                                    action="store_true", help="Print a verbose output of the process")
-        loudness_group.add_argument("-q", "--quiet", dest="quiet", action="store_true",
+        loudness_group.add_argument("-v", "--verbose",
+                                    dest="verbose", action="store_true",
+                                    help="Print a verbose output of the process")
+        loudness_group.add_argument("-q", "--quiet",
+                                    dest="quiet", action="store_true",
                                     help="Avoid printing anything to the terminal if possible")
 
         # don't forget to update it in the pyproject.toml to!
         parser.add_argument("--ver", "--version",
                             action='version', version=__version__)
-        parser.add_argument("--git", "--github", action='version',
-                            help="Give a link to the github repo page", version="https://github.com/MarkusHammer/gitautobackup")
+        parser.add_argument("--git", "--github",
+                            action='version', version="https://github.com/MarkusHammer/gitautobackup",
+                            help="Give a link to the github repo page")
 
         args = parser.parse_args(*args)
         path = args.repo_path
         if path is not None:
             path = path.strip("'").strip('"')
         force_commit = args.force_commit
         force_tag = args.force_tag
-        if args.force_compress:
-            force_compress = True
-        elif args.force_no_compress:
-            force_compress = False
-        elif args.force_compress_aggressive:
-            force_compress = True
-            compress_aggressive = True
+        if args.force_cleanup:
+            force_cleanup = True
+        elif args.force_no_cleanup:
+            force_cleanup = False
+        elif args.force_cleanup_aggressive:
+            force_cleanup = True
+            cleanup_aggressive = True
         else:
-            force_compress = None
+            force_cleanup = None
         commit_message = args.commit_message
         if commit_message is not None:
             commit_message = commit_message.strip("'").strip('"')
         tag = args.tag
         if tag is not None:
             tag = tag.strip("'").strip('"')
         tag_message = args.tag_message
@@ -425,15 +627,15 @@
         if archive_format is not None:
             archive_format = archive_format.strip("'").strip('"')
 
         if args.verbose:
             verbose = True
         elif args.quiet:
             verbose = False
-    except ImportError:
+    else:
         print("Argparse could not be loaded/found, please note that this will mean that explicitly specifying the path form the cli is required and all other cli arguments are not available")
         further_guess_paths = False
 
         next_is_message = False
         for arglet in args:
             arglet = arglet.strip().strip('"')
 
@@ -463,38 +665,34 @@
             print("No valid repository path was found")
             return False
         verbose = True
 
     if args.verbose:
         print("Making auto backup")
 
-    return auto_git_backup(path, commit_message=commit_message, further_guess_paths=further_guess_paths, verbose=verbose, force_commit=force_commit, tag = tag, tag_message = tag_message, force_tag = force_tag, force_compress=force_compress, compress_aggressive = compress_aggressive, archive_path = archive_path, archive_format = archive_format)
-
-
-def __main__():
-    from sys import (exit as end, argv)
-
-    scode = -1
-
-    try:
-        scode = 0 if main(argv[1:], prog_arg=argv[0]) else 1 #1 means not error but also no changes, 0 is no error and changes where made
-    except GitCommandNotFound:
-        print("Your system is not set up properly for use with the GitPython module. Please refer to it's documentation for setting it up before running this script.")
-        scode = -2
-    except (NoSuchPathError, FileNotFoundError, PermissionError):
-        print("The given path does not exist on this system or could not be accessed by this user.")
-        scode = -3
-    except InvalidGitRepositoryError:
-        print("The folder given is not a git repo, or is bare.")
-        scode = -4
-    except RepositoryDirtyError:
-        print("The repository already has some changes that could end up being overwritten. Please Handle these first before running this.")
-        scode = -5
-    except InvalidArchiveFormatError as exc:
-        print(str(exc))
-        scode = -6
-
-    end(scode)
+    return main_cli(path, commit_message=commit_message, further_guess_paths=further_guess_paths, force_commit=force_commit, tag = tag, tag_message = tag_message, force_tag = force_tag, force_cleanup=force_cleanup, cleanup_aggressive = cleanup_aggressive, archive_paths = archive_path, archive_format = archive_format, verbose=verbose)
 
 
-if __name__ == "__main__":
-    __main__()
+if CLIARGV_IMPORTED and END_IMPORTED: #this is the only way the CLI could be run
+    def __main__():
+        """PRIVATE USED TO RUN DIRECTLY FORM THE COMMAND LINE DO NOT USE THIS IF USING THIS AS A MODULE"""
+        scode = -1
+        try:
+            scode = 0 if main(cliargv[1:], prog_arg=cliargv[0]) else 1 #1 means not error but also no changes, 0 is no error and changes where made
+        except GitCommandNotFound:
+            print("Your system is not set up properly for use with the GitPython module. Please refer to it's documentation for setting it up before running this script.")
+            scode = -2
+        except (NoSuchPathError, FileNotFoundError, PermissionError):
+            print("The given path does not exist on this system or could not be accessed by this user.")
+            scode = -3
+        except InvalidGitRepositoryError:
+            print("The folder given is not a git repo, or is bare.")
+            scode = -4
+        except RepositoryDirtyError:
+            print("The repository already has some changes that could end up being overwritten. Please Handle these first before running this.")
+            scode = -5
+        except InvalidArchiveFormatError as exc:
+            print(str(exc))
+            scode = -6
+        end(scode)
+    if __name__ == "__main__":
+        __main__()
```

### Comparing `gitautobackup-1.2.0.0/pyproject.toml` & `gitautobackup-2.0.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -36,39 +36,39 @@
         "devtool",
         "small",
         "simple",
         "development",
         "utility"
     ]
     [project.optional-dependencies]
-        cli = ["argparse", "pprint"]
+        cli = ["argparse"]
         dev = ["setuptools>=64.0.0", "pip-tools", "validate-pyproject[all]", "build", "twine"]
     [project.scripts] 
         gitautobackup = "gitautobackup:__main__"
         gitbackup = "gitautobackup:__main__"
     [project.urls]
         Homepage = "https://github.com/MarkusHammer/gitautobackup"
         Github  = "https://github.com/MarkusHammer/gitautobackup"
         Issues = "https://github.com/MarkusHammer/gitautobackup/issues"
         "Pull Requests" = "https://github.com/MarkusHammer/gitautobackup/pulls"
         Git = "https://github.com/MarkusHammer/gitautobackup.git"
 
 [build-system]
     requires = ["setuptools>=64.0.0"]
     build-backend = "setuptools.build_meta"
-    
-    ### NOTE THIS MUST BE BUILT ON A VERSION OF PYTHON >= 3.10, 3.9.1 and 3.8.7 #THX https://github.com/pypa/build/issues/255#issuecomment-794560752
-    ### py -3.10 -m pip install pip-tools validate-pyproject[all] build twine setuptools
-    ### validate-pyproject pyproject.toml
-    ### pip-compile pyproject.toml
-    ### py -3.10 -m build
-    ### twine upload dist/* --verbose -u USERNAME -p PASSWORD
 
 [tool.setuptools]
     zip-safe = true
     [tool.setuptools.dynamic]
         version = {attr = "gitautobackup.__version__"}
         readme = {file = ["README.md", "LICENSE"], content-type = "text/markdown"}
 
 [tool.pylint."MESSAGES CONTROL"]
     disable = "C0301, C0415"
-    # Disables the warnings for importing out of the top level and long lines
+    # Disables the warnings for importing out of the top level and long lines
+
+### NOTE THIS MUST BE BUILT ON A VERSION OF PYTHON >= 3.10, 3.9.1 and 3.8.7 #THX https://github.com/pypa/build/issues/255#issuecomment-794560752
+### py -3.10 -m pip install pip-tools validate-pyproject[all] build twine setuptools
+### validate-pyproject pyproject.toml
+### pip-compile --resolver=backtracking pyproject.toml
+### py -3.10 -m build
+### twine upload dist/* --verbose
```

