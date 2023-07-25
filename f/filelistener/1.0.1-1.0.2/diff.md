# Comparing `tmp/filelistener-1.0.1.tar.gz` & `tmp/filelistener-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filelistener-1.0.1.tar", last modified: Tue Jul 25 17:47:47 2023, max compression
+gzip compressed data, was "filelistener-1.0.2.tar", last modified: Tue Jul 25 18:29:36 2023, max compression
```

## Comparing `filelistener-1.0.1.tar` & `filelistener-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 17:47:47.172078 filelistener-1.0.1/
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 17:47:47.157248 filelistener-1.0.1/Content/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:49:10.000000 filelistener-1.0.1/Content/__init__.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     6054 2023-07-25 17:46:19.000000 filelistener-1.0.1/Content/duplicate_content.py
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 17:47:47.159235 filelistener-1.0.1/Content/modules/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:10:47.000000 filelistener-1.0.1/Content/modules/__init__.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     1563 2023-07-21 04:19:28.000000 filelistener-1.0.1/Content/modules/duplicate_zip_files.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-25 17:47:47.171246 filelistener-1.0.1/PKG-INFO
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      421 2023-07-25 17:46:19.000000 filelistener-1.0.1/README.md
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 17:47:47.169842 filelistener-1.0.1/filelistener.egg-info/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-25 17:47:46.000000 filelistener-1.0.1/filelistener.egg-info/PKG-INFO
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      352 2023-07-25 17:47:47.000000 filelistener-1.0.1/filelistener.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-25 17:47:46.000000 filelistener-1.0.1/filelistener.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       58 2023-07-25 17:47:46.000000 filelistener-1.0.1/filelistener.egg-info/entry_points.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        9 2023-07-25 17:47:46.000000 filelistener-1.0.1/filelistener.egg-info/requires.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        8 2023-07-25 17:47:46.000000 filelistener-1.0.1/filelistener.egg-info/top_level.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       38 2023-07-25 17:47:47.172307 filelistener-1.0.1/setup.cfg
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      496 2023-07-25 17:46:19.000000 filelistener-1.0.1/setup.py
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 18:29:36.428695 filelistener-1.0.2/
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 18:29:36.417344 filelistener-1.0.2/Content/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:49:10.000000 filelistener-1.0.2/Content/__init__.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     6429 2023-07-25 18:27:52.000000 filelistener-1.0.2/Content/duplicate_content.py
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 18:29:36.419778 filelistener-1.0.2/Content/modules/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:10:47.000000 filelistener-1.0.2/Content/modules/__init__.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     1563 2023-07-21 04:19:28.000000 filelistener-1.0.2/Content/modules/duplicate_zip_files.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-25 18:29:36.426759 filelistener-1.0.2/PKG-INFO
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      421 2023-07-25 17:46:19.000000 filelistener-1.0.2/README.md
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 18:29:36.425536 filelistener-1.0.2/filelistener.egg-info/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      352 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       58 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/entry_points.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        9 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/requires.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        8 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/top_level.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       38 2023-07-25 18:29:36.429147 filelistener-1.0.2/setup.cfg
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      496 2023-07-25 18:29:32.000000 filelistener-1.0.2/setup.py
```

### Comparing `filelistener-1.0.1/Content/duplicate_content.py` & `filelistener-1.0.2/Content/duplicate_content.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,45 +103,52 @@
     enable_delete = args.delete
 
     duplicate_files = check_files_in_folder(folder_path)
 
     # After checking for duplicate files in the folder, print duplicate zip files
     print_duplicate_zip_files(folder_path)
 
-    # Ask the user if they want to delete the duplicate files
-    if enable_delete:
-        found_duplicates = False  # Initialize the flag
-        duplicates_to_print = set()  # Use a set to store duplicate file names
-        for size, hash_dict in duplicate_files.items():
-            for file_hash, file_info_list in hash_dict.items():
-                if file_hash == 'file_paths':
-                    continue
-
-                if len(file_info_list) > 1:
-                    found_duplicates = True
-                    # Store the duplicates for later printing
-                    for file_info in file_info_list[1:]:
-                        file_path, _ = file_info
-                        duplicates_to_print.add(os.path.basename(file_path))
-                    # Delete all files except the first one (keep the original)
-                    for file_info in file_info_list[1:]:
-                        file_path, _ = file_info
-                        os.remove(file_path)
-                    print(f"\033[31mDeleted duplicate files with hash {file_hash} and size {size} bytes.\033[0m")
-
-        if not found_duplicates:
-            print("\033[32mNo duplicates found.\033[0m")
-        elif duplicates_to_print and found_duplicates:
-            print("\033[32mDeletion of duplicate files completed.\033[0m")
-            # Print the duplicates that were deleted
-            print("\nDeleted duplicates:")
-            for file_name in duplicates_to_print:
-                print(file_name)
-            print()
+    found_duplicates = False
+    duplicates_to_print = set()
+    for size, hash_dict in duplicate_files.items():
+        for file_hash, file_info_list in hash_dict.items():
+            if file_hash == 'file_paths':
+                continue
+
+            if len(file_info_list) > 1:
+                found_duplicates = True
+                # Store the duplicates for later printing
+                for file_info in file_info_list[1:]:
+                    file_path, _ = file_info
+                    duplicates_to_print.add(os.path.basename(file_path))
+
+    if not found_duplicates:
+        print("\033[32mNo duplicates found.\033[0m")
+    elif duplicates_to_print and found_duplicates:
+        if enable_delete:
+            print("\033[33mType 'delete' to confirm deletion of duplicates or press enter to skip. \033[0m")
+            user_input = input(">>")
+            if user_input.strip().lower() == 'delete':
+                # Delete the duplicate files permanently
+                for size, hash_dict in duplicate_files.items():
+                    for file_hash, file_info_list in hash_dict.items():
+                        if file_hash == 'file_paths':
+                            continue
+
+                        if len(file_info_list) > 1:
+                            for file_info in file_info_list[1:]:
+                                file_path, _ = file_info
+                                os.remove(file_path)
+                            print(f"\033[31mDeleted duplicate files with hash {file_hash} and size {size} bytes.\033[0m")
+                print("\033[32mDeletion of duplicate files completed.\033[0m")
+            else:
+                print("\033[32mDeletion canceled. Duplicates are still available.\033[0m")
+        else:
+            print("\033[32mDuplicates are still available.\033[0m")
 
-    else:
-        print("Deletion canceled.")
+    if enable_delete and not found_duplicates:
+        print("\033[33mNo duplicates found. Nothing to delete.\033[0m")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `filelistener-1.0.1/Content/modules/duplicate_zip_files.py` & `filelistener-1.0.2/Content/modules/duplicate_zip_files.py`

 * *Files identical despite different names*

