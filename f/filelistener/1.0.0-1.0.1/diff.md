# Comparing `tmp/filelistener-1.0.0.tar.gz` & `tmp/filelistener-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filelistener-1.0.0.tar", last modified: Fri Jul 21 19:12:38 2023, max compression
+gzip compressed data, was "filelistener-1.0.1.tar", last modified: Tue Jul 25 17:47:47 2023, max compression
```

## Comparing `filelistener-1.0.0.tar` & `filelistener-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 19:12:38.310983 filelistener-1.0.0/
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 19:12:38.273903 filelistener-1.0.0/Content/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:49:10.000000 filelistener-1.0.0/Content/__init__.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     4480 2023-07-21 19:04:18.000000 filelistener-1.0.0/Content/duplicate_content.py
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 19:12:38.285483 filelistener-1.0.0/Content/modules/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:10:47.000000 filelistener-1.0.0/Content/modules/__init__.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     1563 2023-07-21 04:19:28.000000 filelistener-1.0.0/Content/modules/duplicate_zip_files.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      193 2023-07-21 19:12:38.309846 filelistener-1.0.0/PKG-INFO
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 19:12:38.308245 filelistener-1.0.0/filelistener.egg-info/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      193 2023-07-21 19:12:37.000000 filelistener-1.0.0/filelistener.egg-info/PKG-INFO
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      342 2023-07-21 19:12:37.000000 filelistener-1.0.0/filelistener.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-21 19:12:37.000000 filelistener-1.0.0/filelistener.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       58 2023-07-21 19:12:37.000000 filelistener-1.0.0/filelistener.egg-info/entry_points.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        9 2023-07-21 19:12:37.000000 filelistener-1.0.0/filelistener.egg-info/requires.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        8 2023-07-21 19:12:37.000000 filelistener-1.0.0/filelistener.egg-info/top_level.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       38 2023-07-21 19:12:38.311287 filelistener-1.0.0/setup.cfg
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      458 2023-07-21 19:07:10.000000 filelistener-1.0.0/setup.py
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 17:47:47.172078 filelistener-1.0.1/
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 17:47:47.157248 filelistener-1.0.1/Content/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:49:10.000000 filelistener-1.0.1/Content/__init__.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     6054 2023-07-25 17:46:19.000000 filelistener-1.0.1/Content/duplicate_content.py
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 17:47:47.159235 filelistener-1.0.1/Content/modules/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:10:47.000000 filelistener-1.0.1/Content/modules/__init__.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     1563 2023-07-21 04:19:28.000000 filelistener-1.0.1/Content/modules/duplicate_zip_files.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-25 17:47:47.171246 filelistener-1.0.1/PKG-INFO
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      421 2023-07-25 17:46:19.000000 filelistener-1.0.1/README.md
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 17:47:47.169842 filelistener-1.0.1/filelistener.egg-info/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-25 17:47:46.000000 filelistener-1.0.1/filelistener.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      352 2023-07-25 17:47:47.000000 filelistener-1.0.1/filelistener.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-25 17:47:46.000000 filelistener-1.0.1/filelistener.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       58 2023-07-25 17:47:46.000000 filelistener-1.0.1/filelistener.egg-info/entry_points.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        9 2023-07-25 17:47:46.000000 filelistener-1.0.1/filelistener.egg-info/requires.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        8 2023-07-25 17:47:46.000000 filelistener-1.0.1/filelistener.egg-info/top_level.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       38 2023-07-25 17:47:47.172307 filelistener-1.0.1/setup.cfg
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      496 2023-07-25 17:46:19.000000 filelistener-1.0.1/setup.py
```

### Comparing `filelistener-1.0.0/Content/duplicate_content.py` & `filelistener-1.0.1/Content/duplicate_content.py`

 * *Files 27% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             return file_hash
     except subprocess.CalledProcessError as e:
         # Handle any errors that might occur during the md5sum command execution
         print(f"Error calculating hash for {file_path}: {e}")
         return None
     
 
-def check_files_in_folder(folder_path, calculate_file_sizes):
+def check_files_in_folder(folder_path, calculate_file_sizes=True):
     """Check for duplicate files in a folder.
 
     This function traverses through the specified folder and its subdirectories,
     calculates the MD5 hash of each file, and identifies duplicate files by their hashes.
 
     Args:
         folder_path (str): The path to the folder.
@@ -86,24 +86,62 @@
                 continue
 
             if len(file_paths) > 1:
                 print(f"Duplicate files with hash {file_hash}:")
                 for file_path in file_paths:
                     print(file_path)
                 print()
+
+    return duplicate_files
+    
 def main():
     parser = argparse.ArgumentParser(description='Check for duplicate files in a folder.')
     parser.add_argument('-f', '--folder', required=True, help='Path to the folder')
-    parser.add_argument('-s', '--calculate-sizes',required=True, action='store_true', help='Calculate duplicate file sizes')
+    parser.add_argument('-d', '--delete', action='store_true', help='Flag to enable deletion of duplicates')
     args = parser.parse_args()
 
     folder_path = args.folder
-    calculate_sizes = args.calculate_sizes
+    enable_delete = args.delete
 
-    check_files_in_folder(folder_path, calculate_sizes)
+    duplicate_files = check_files_in_folder(folder_path)
 
     # After checking for duplicate files in the folder, print duplicate zip files
     print_duplicate_zip_files(folder_path)
 
+    # Ask the user if they want to delete the duplicate files
+    if enable_delete:
+        found_duplicates = False  # Initialize the flag
+        duplicates_to_print = set()  # Use a set to store duplicate file names
+        for size, hash_dict in duplicate_files.items():
+            for file_hash, file_info_list in hash_dict.items():
+                if file_hash == 'file_paths':
+                    continue
+
+                if len(file_info_list) > 1:
+                    found_duplicates = True
+                    # Store the duplicates for later printing
+                    for file_info in file_info_list[1:]:
+                        file_path, _ = file_info
+                        duplicates_to_print.add(os.path.basename(file_path))
+                    # Delete all files except the first one (keep the original)
+                    for file_info in file_info_list[1:]:
+                        file_path, _ = file_info
+                        os.remove(file_path)
+                    print(f"\033[31mDeleted duplicate files with hash {file_hash} and size {size} bytes.\033[0m")
+
+        if not found_duplicates:
+            print("\033[32mNo duplicates found.\033[0m")
+        elif duplicates_to_print and found_duplicates:
+            print("\033[32mDeletion of duplicate files completed.\033[0m")
+            # Print the duplicates that were deleted
+            print("\nDeleted duplicates:")
+            for file_name in duplicates_to_print:
+                print(file_name)
+            print()
+
+    else:
+        print("Deletion canceled.")
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `filelistener-1.0.0/Content/modules/duplicate_zip_files.py` & `filelistener-1.0.1/Content/modules/duplicate_zip_files.py`

 * *Files identical despite different names*

