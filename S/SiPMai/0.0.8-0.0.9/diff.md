# Comparing `tmp/SiPMai-0.0.8.tar.gz` & `tmp/SiPMai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiPMai-0.0.8.tar", last modified: Mon Jul 24 02:49:10 2023, max compression
+gzip compressed data, was "SiPMai-0.0.9.tar", last modified: Tue Jul 25 10:51:00 2023, max compression
```

## Comparing `SiPMai-0.0.8.tar` & `SiPMai-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.830535 SiPMai-0.0.8/
--rw-rw-rw-   0        0        0     1086 2023-07-18 06:39:47.000000 SiPMai-0.0.8/LICENSE.md
--rw-rw-rw-   0        0        0     4409 2023-07-24 02:49:10.829533 SiPMai-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3895 2023-07-19 15:22:23.000000 SiPMai-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.695988 SiPMai-0.0.8/SiPMai/
--rw-rw-rw-   0        0        0      107 2023-07-24 02:46:10.000000 SiPMai-0.0.8/SiPMai/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.760529 SiPMai-0.0.8/SiPMai/gen_data/
--rw-rw-rw-   0        0        0       53 2023-07-19 03:54:35.000000 SiPMai-0.0.8/SiPMai/gen_data/__init__.py
--rw-rw-rw-   0        0        0     4687 2023-07-20 02:35:15.000000 SiPMai-0.0.8/SiPMai/gen_data/compute_img.py
--rw-rw-rw-   0        0        0     7272 2023-07-20 02:47:51.000000 SiPMai-0.0.8/SiPMai/gen_data/gen_all_data_pipeline.py
--rw-rw-rw-   0        0        0     3498 2023-07-17 15:04:41.000000 SiPMai-0.0.8/SiPMai/gen_data/prepare_dataset.py
--rw-rw-rw-   0        0        0    10801 2023-07-24 02:45:33.000000 SiPMai-0.0.8/SiPMai/gen_data/ray_generation.py
--rw-rw-rw-   0        0        0    11369 2023-07-19 10:21:20.000000 SiPMai-0.0.8/SiPMai/gen_data/smi_molecule_simulation.py
--rw-rw-rw-   0        0        0     2896 2023-07-19 03:08:31.000000 SiPMai-0.0.8/SiPMai/gen_data/smile_generation.py
--rw-rw-rw-   0        0        0     2063 2023-07-20 02:33:39.000000 SiPMai-0.0.8/SiPMai/gen_data/util_fn.py
-drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.767530 SiPMai-0.0.8/SiPMai/smiles/
--rw-rw-rw-   0        0        0        0 2023-07-19 05:06:31.000000 SiPMai-0.0.8/SiPMai/smiles/__init__.py
--rw-rw-rw-   0        0        0 41963544 2023-07-17 10:17:15.000000 SiPMai-0.0.8/SiPMai/smiles/pubchem_39_200_100k.json
-drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.814529 SiPMai-0.0.8/SiPMai/unittest/
--rw-rw-rw-   0        0        0        0 2023-07-19 03:45:56.000000 SiPMai-0.0.8/SiPMai/unittest/__init__.py
--rw-rw-rw-   0        0        0     2538 2023-07-19 07:42:46.000000 SiPMai-0.0.8/SiPMai/unittest/test_gen_data.py
-drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.828534 SiPMai-0.0.8/SiPMai/utils/
--rw-rw-rw-   0        0        0        0 2023-07-18 03:21:53.000000 SiPMai-0.0.8/SiPMai/utils/__init__.py
--rw-rw-rw-   0        0        0     6435 2023-07-20 03:25:52.000000 SiPMai-0.0.8/SiPMai/utils/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-07-24 02:49:10.733531 SiPMai-0.0.8/SiPMai.egg-info/
--rw-rw-rw-   0        0        0     4409 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      683 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      150 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-24 02:49:10.000000 SiPMai-0.0.8/SiPMai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 02:49:10.830535 SiPMai-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1815 2023-07-19 05:12:14.000000 SiPMai-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 10:51:00.339811 SiPMai-0.0.9/
+-rw-rw-rw-   0        0        0     1086 2023-07-18 06:39:47.000000 SiPMai-0.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0     4409 2023-07-25 10:51:00.338675 SiPMai-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3895 2023-07-19 15:22:23.000000 SiPMai-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 10:51:00.225891 SiPMai-0.0.9/SiPMai/
+-rw-rw-rw-   0        0        0      107 2023-07-25 10:49:45.000000 SiPMai-0.0.9/SiPMai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 10:51:00.257457 SiPMai-0.0.9/SiPMai/gen_data/
+-rw-rw-rw-   0        0        0       53 2023-07-19 03:54:35.000000 SiPMai-0.0.9/SiPMai/gen_data/__init__.py
+-rw-rw-rw-   0        0        0     4687 2023-07-20 02:35:15.000000 SiPMai-0.0.9/SiPMai/gen_data/compute_img.py
+-rw-rw-rw-   0        0        0     7875 2023-07-25 10:49:00.000000 SiPMai-0.0.9/SiPMai/gen_data/gen_all_data_pipeline.py
+-rw-rw-rw-   0        0        0     3498 2023-07-17 15:04:41.000000 SiPMai-0.0.9/SiPMai/gen_data/prepare_dataset.py
+-rw-rw-rw-   0        0        0    12934 2023-07-25 06:35:07.000000 SiPMai-0.0.9/SiPMai/gen_data/ray_generation.py
+-rw-rw-rw-   0        0        0    11369 2023-07-19 10:21:20.000000 SiPMai-0.0.9/SiPMai/gen_data/smi_molecule_simulation.py
+-rw-rw-rw-   0        0        0     2896 2023-07-19 03:08:31.000000 SiPMai-0.0.9/SiPMai/gen_data/smile_generation.py
+-rw-rw-rw-   0        0        0     2063 2023-07-20 02:33:39.000000 SiPMai-0.0.9/SiPMai/gen_data/util_fn.py
+drwxrwxrwx   0        0        0        0 2023-07-25 10:51:00.260459 SiPMai-0.0.9/SiPMai/smiles/
+-rw-rw-rw-   0        0        0        0 2023-07-19 05:06:31.000000 SiPMai-0.0.9/SiPMai/smiles/__init__.py
+-rw-rw-rw-   0        0        0 41963544 2023-07-17 10:17:15.000000 SiPMai-0.0.9/SiPMai/smiles/pubchem_39_200_100k.json
+drwxrwxrwx   0        0        0        0 2023-07-25 10:51:00.314584 SiPMai-0.0.9/SiPMai/unittest/
+-rw-rw-rw-   0        0        0        0 2023-07-19 03:45:56.000000 SiPMai-0.0.9/SiPMai/unittest/__init__.py
+-rw-rw-rw-   0        0        0     2538 2023-07-19 07:42:46.000000 SiPMai-0.0.9/SiPMai/unittest/test_gen_data.py
+drwxrwxrwx   0        0        0        0 2023-07-25 10:51:00.332670 SiPMai-0.0.9/SiPMai/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-18 03:21:53.000000 SiPMai-0.0.9/SiPMai/utils/__init__.py
+-rw-rw-rw-   0        0        0    11652 2023-07-25 07:10:56.000000 SiPMai-0.0.9/SiPMai/utils/dataloader.py
+-rw-rw-rw-   0        0        0     2475 2023-07-24 15:24:09.000000 SiPMai-0.0.9/SiPMai/utils/img_transform.py
+drwxrwxrwx   0        0        0        0 2023-07-25 10:51:00.244941 SiPMai-0.0.9/SiPMai.egg-info/
+-rw-rw-rw-   0        0        0     4409 2023-07-25 10:50:59.000000 SiPMai-0.0.9/SiPMai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-07-25 10:50:59.000000 SiPMai-0.0.9/SiPMai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 10:50:59.000000 SiPMai-0.0.9/SiPMai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-07-25 10:50:59.000000 SiPMai-0.0.9/SiPMai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      150 2023-07-25 10:50:59.000000 SiPMai-0.0.9/SiPMai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 10:50:59.000000 SiPMai-0.0.9/SiPMai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 10:51:00.339811 SiPMai-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1815 2023-07-19 05:12:14.000000 SiPMai-0.0.9/setup.py
```

### Comparing `SiPMai-0.0.8/LICENSE.md` & `SiPMai-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.8/PKG-INFO` & `SiPMai-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiPMai
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Simple Yet Effective Scanning Tunnel Microscope Image Simulator
 Home-page: http://github.com/GilesLuo/SiPMai
 Author: Zhiyao Luo, Yaotian Yang, Jiali Li
 Author-email: zhiyao.luo@eng.ox.ac.uk
 License: MIT
 Project-URL: Source Code, https://github.com/my_username/my_package
 Keywords: Chemistry Simulation,STM Image Synthesis
```

### Comparing `SiPMai-0.0.8/README.md` & `SiPMai-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.8/SiPMai/gen_data/compute_img.py` & `SiPMai-0.0.9/SiPMai/gen_data/compute_img.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.8/SiPMai/gen_data/gen_all_data_pipeline.py` & `SiPMai-0.0.9/SiPMai/gen_data/gen_all_data_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from SiPMai.gen_data.smile_generation import gen_smiles_main
 from SiPMai.gen_data.ray_generation import ray_gen_main
 from SiPMai.gen_data.prepare_dataset import gen_index_main
 import os
 import json
 from typing import Dict
+from SiPMai.utils.dataloader import get_dataset_mean_std
 
 
 def gen_all_data(smiles_file: str, num_mol: int, csv_file: str, min_atom: int, max_atom: int, num_cpus: int,
                  mol_save_dir: str,
                  resolution: int, blur_sigma: int, use_motion_blur: bool, use_gaussian_noise: bool,
                  gen_original_img: bool, gen_mol_drawing:bool, img_show: bool,
                  train_ratio: float, val_ratio: float, test_ratio: float, split_seed: int,
+                 redo_mean_std:bool, mean_std_batch_size:int,
                  development: bool = False) -> None:
     """
     Generate all data required for the molecular images.
 
     Args:
         smiles_file (str): The path to the file containing SMILES strings.
         num_mol (int): The number of molecules to be generated.
@@ -55,15 +57,16 @@
     if num_cpus == 0:
         num_cpus = os.cpu_count()
 
     ray_gen_main(smiles_dict, mol_save_dir,
                  resolution, blur_sigma, use_motion_blur, use_gaussian_noise, gen_original_img, gen_mol_drawing,
                  num_cpus, img_show, development)
     gen_index_main(mol_save_dir, train_ratio, val_ratio, test_ratio, split_seed)
-
+    get_dataset_mean_std(mol_save_dir, redo=redo_mean_std, num_workers=num_cpus, batch_size=mean_std_batch_size
+                            )
 
 def main() -> None:
     """
     Main function that parses command line arguments and calls the gen_all function.
     """
     print("Start generating data with preset parameters (100k dataset with 39 <= num_atom <= 200)... ")
     import argparse
@@ -98,26 +101,30 @@
     parser.add_argument("--show", type=bool, default=False, help="Whether to display the generated images.")
 
     # data indices args
     parser.add_argument("--split_seed", type=int, default=1, help="The seed for the random splitting of data.")
     parser.add_argument("--train_ratio", type=float, default=0.8, help="The ratio of data to be used for training.")
     parser.add_argument("--val_ratio", type=float, default=0.1, help="The ratio of data to be used for validation.")
     parser.add_argument("--test_ratio", type=float, default=0.1, help="The ratio of data to be used for testing.")
+
+    # compute mean and std args
+    parser.add_argument("--redo", type=bool, default=False, help="Whether to redo the mean and std computation.")
+    parser.add_argument("--batch_size", type=int, default=256, help="The batch size to be used for mean and std computation.")
     args = parser.parse_args()
 
     from pkg_resources import resource_filename
     args.smiles_file = resource_filename('SiPMai', f'smiles/{args.smiles_file}')
     cmd_dir = os.getcwd()
     args.mol_save_dir = os.path.join(cmd_dir, args.mol_save_dir)
     print("mol_save_dir set to command execution dir: ", args.mol_save_dir)
     gen_all_data(smiles_file=args.smiles_file, num_mol=args.num_mol, csv_file=args.csv_file, min_atom=args.min_atom,
                  max_atom=args.max_atom, num_cpus=args.num_cpus, mol_save_dir=args.mol_save_dir,
                  resolution=args.resolution, blur_sigma=args.blur_sigma, use_motion_blur=args.use_motion_blur,
                  use_gaussian_noise=args.use_gaussian_noise, gen_original_img=args.gen_original_img, gen_mol_drawing=args.gen_mol_drawing,
                  img_show=False,
                  train_ratio=args.train_ratio, val_ratio=args.val_ratio, test_ratio=args.test_ratio,
-                 split_seed=args.split_seed,
+                 split_seed=args.split_seed, mean_std_batch_size=args.batch_size, redo_mean_std=args.redo,
                  development=args.development)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `SiPMai-0.0.8/SiPMai/gen_data/prepare_dataset.py` & `SiPMai-0.0.9/SiPMai/gen_data/prepare_dataset.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.8/SiPMai/gen_data/ray_generation.py` & `SiPMai-0.0.9/SiPMai/gen_data/ray_generation.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,20 +50,19 @@
     done = np.array([os.path.exists(file) for file in check_list])
     if done.all():
         print("molecule already exists, skipping...")
         return True
 
     #         2D molecules were converted into 3D structures,
     #         and mechanical functions were used for Angle correction and optimization
-    mol_2D = Chem.MolFromSmiles(smi)
-    mol_2D_H = Chem.AddHs(mol_2D)
-    atom_num = mol_2D_H.GetNumAtoms()
-    bond_num = mol_2D_H.GetNumBonds()
-
     try:
+        mol_2D = Chem.MolFromSmiles(smi)
+        mol_2D_H = Chem.AddHs(mol_2D)
+        atom_num = mol_2D_H.GetNumAtoms()
+        bond_num = mol_2D_H.GetNumBonds()
         moleblock_2D = Chem.MolToMolBlock(mol_2D_H)  # Returns the two-dimensional coordinates of the atoms in the molecule
     except Chem.rdchem.KekulizeException:
         print("kekulize failed, molecule: ", molecule_name, ", skip...")
         return False
     if show:
         mol_3D = Chem.MolFromSmiles(smi)
         Draw.ShowMol(mol_3D, size=(550, 550), kekulize=False)
@@ -175,28 +174,85 @@
     except Exception as e:
         # to avoid the error of json.dump, remove the file if an exception occurs
         os.remove(json_name)
         raise ValueError("something wrong with json.dump. Json file removed to avoid saving broken files")
     return True
 
 
+@ray.remote
+def check_cid(cid, info_dir, json_dir, img_dir):
+    img_path = os.path.join(img_dir, f'{cid}_img.png')  # drawing not checked
+    json_path = os.path.join(json_dir, f'{cid}.json')
+    npz_path = os.path.join(info_dir, f'{cid}_points_info.npz')
+
+    # Checking the existence of files
+    img_exists = os.path.isfile(img_path)
+    json_exists = os.path.isfile(json_path)
+    npz_exists = os.path.isfile(npz_path)
+
+    # Checking the validity of the JSON file
+    json_valid = False
+    if json_exists:
+        try:
+            with open(json_path, 'r') as json_file:
+                json.load(json_file)
+            json_valid = True
+        except Exception:
+            pass
+
+    return cid, img_exists, json_exists, json_valid, npz_exists
+
+def get_task(molecule_dict, info_dir, json_dir, img_dir, num_workers):
+    task_dict = {}
+    broken_dict = {}
+    done_dict = {}
+
+    # Parallelize the check_cid task with ray
+    ray.init(num_cpus=num_workers)
+    futures = [check_cid.remote(cid, info_dir, json_dir, img_dir) for cid in molecule_dict.keys()]
+    for i in tqdm(range(len(futures)), desc='Checking generated files'):
+        result = ray.get(futures[i])
+        # result = futures[i]
+        cid, img_exists, json_exists, json_valid, npz_exists = result
+        if img_exists and json_exists and json_valid and npz_exists:
+            done_dict[cid] = molecule_dict[cid]
+        elif img_exists or json_exists or npz_exists:
+            broken_dict[cid] = molecule_dict[cid]
+        else:
+            task_dict[cid] = molecule_dict[cid]
+    ray.shutdown()
+
+    return task_dict, broken_dict, done_dict
+
+
 def ray_gen_main(mol_dict, save_dir, resolution, blur_sigma, use_motion_blur, use_gaussian_noise, gen_original_img=False, gen_mol_drawing=False,
                  num_cpu=None, show=False, debug_mode=False):
-    ray.init(num_cpus=num_cpu, local_mode=debug_mode)
+
 
     # prepare folders
     info_dir = os.path.join(save_dir, "info")
     json_dir = os.path.join(save_dir, "json")
     img_dir = os.path.join(save_dir, "img")
+
+    if os.path.exists(save_dir):
+        tasks = {}
+        task_dict, broken_dict, done_dict = get_task(mol_dict, info_dir, json_dir, img_dir, num_cpu)
+    else:
+        tasks = {}
+        task_dict = mol_dict
+        broken_dict = {}
+        done_dict = {}
+    print(
+        f"{len(task_dict)} molecules to process, {len(broken_dict)} broken molecules (need to be regenerated), {len(done_dict)} done")
     os.makedirs(info_dir, exist_ok=True)
     os.makedirs(json_dir, exist_ok=True)
     os.makedirs(img_dir, exist_ok=True)
 
-    tasks = {}
-    for mol, smiles in mol_dict.items():
+    ray.init(num_cpus=num_cpu, local_mode=debug_mode)
+    for mol, smiles in tqdm(task_dict.items(), desc="adding tasks to Ray"):
         task_id = points_height_matrix.remote(smiles, mol, resolution, info_dir, json_dir, img_dir,
                                               blur_sigma, use_motion_blur, use_gaussian_noise,
                                               gen_original_img, gen_mol_drawing, show)
         tasks[task_id] = mol
 
     pbar = tqdm(total=len(tasks), desc="Processing tasks")
     while len(tasks):
@@ -209,15 +265,15 @@
                 pbar.update()
             except ray.exceptions.RayTaskError as ex:
                 print(f"Task failed for molecule {tasks[ready_id]} with error: {ex}")
         time.sleep(0.5)  # To avoid busy waiting
 
     pbar.close()
     ray.shutdown()
-
+    return
 
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--smiles_file", type=str, default="../smiles/pubchem_39_200_100k.json")
     parser.add_argument("--save_dir", type=str, default="../data")
```

### Comparing `SiPMai-0.0.8/SiPMai/gen_data/smi_molecule_simulation.py` & `SiPMai-0.0.9/SiPMai/gen_data/smi_molecule_simulation.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.8/SiPMai/gen_data/smile_generation.py` & `SiPMai-0.0.9/SiPMai/gen_data/smile_generation.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.8/SiPMai/gen_data/util_fn.py` & `SiPMai-0.0.9/SiPMai/gen_data/util_fn.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.8/SiPMai/smiles/pubchem_39_200_100k.json` & `SiPMai-0.0.9/SiPMai/smiles/pubchem_39_200_100k.json`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.8/SiPMai/unittest/test_gen_data.py` & `SiPMai-0.0.9/SiPMai/unittest/test_gen_data.py`

 * *Files identical despite different names*

### Comparing `SiPMai-0.0.8/SiPMai.egg-info/PKG-INFO` & `SiPMai-0.0.9/SiPMai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiPMai
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Simple Yet Effective Scanning Tunnel Microscope Image Simulator
 Home-page: http://github.com/GilesLuo/SiPMai
 Author: Zhiyao Luo, Yaotian Yang, Jiali Li
 Author-email: zhiyao.luo@eng.ox.ac.uk
 License: MIT
 Project-URL: Source Code, https://github.com/my_username/my_package
 Keywords: Chemistry Simulation,STM Image Synthesis
```

### Comparing `SiPMai-0.0.8/SiPMai.egg-info/SOURCES.txt` & `SiPMai-0.0.9/SiPMai.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 SiPMai/gen_data/smile_generation.py
 SiPMai/gen_data/util_fn.py
 SiPMai/smiles/__init__.py
 SiPMai/smiles/pubchem_39_200_100k.json
 SiPMai/unittest/__init__.py
 SiPMai/unittest/test_gen_data.py
 SiPMai/utils/__init__.py
-SiPMai/utils/dataloader.py
+SiPMai/utils/dataloader.py
+SiPMai/utils/img_transform.py
```

### Comparing `SiPMai-0.0.8/setup.py` & `SiPMai-0.0.9/setup.py`

 * *Files identical despite different names*

