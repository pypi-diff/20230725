# Comparing `tmp/papyrus_structure_pipeline-0.0.3.tar.gz` & `tmp/papyrus_structure_pipeline-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papyrus_structure_pipeline-0.0.3.tar", last modified: Mon Mar  6 08:20:17 2023, max compression
+gzip compressed data, was "papyrus_structure_pipeline-0.0.4.tar", last modified: Tue Jul 25 06:52:19 2023, max compression
```

## Comparing `papyrus_structure_pipeline-0.0.3.tar` & `papyrus_structure_pipeline-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 08:20:17.911731 papyrus_structure_pipeline-0.0.3/
--rw-rw-rw-   0        0        0     1100 2023-03-03 09:57:18.000000 papyrus_structure_pipeline-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     9678 2023-03-06 08:20:17.911731 papyrus_structure_pipeline-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8781 2023-03-03 10:22:13.000000 papyrus_structure_pipeline-0.0.3/README.md
--rw-rw-rw-   0        0        0     1257 2023-03-06 08:20:17.916813 papyrus_structure_pipeline-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-03-03 09:57:18.000000 papyrus_structure_pipeline-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:20:17.890712 papyrus_structure_pipeline-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-03-06 08:20:17.896722 papyrus_structure_pipeline-0.0.3/src/papyrus_structure_pipeline/
--rw-rw-rw-   0        0        0      148 2023-03-06 08:18:47.000000 papyrus_structure_pipeline-0.0.3/src/papyrus_structure_pipeline/__init__.py
--rw-rw-rw-   0        0        0    14205 2023-03-06 08:17:34.000000 papyrus_structure_pipeline-0.0.3/src/papyrus_structure_pipeline/standardizer.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:20:17.906730 papyrus_structure_pipeline-0.0.3/src/papyrus_structure_pipeline.egg-info/
--rw-rw-rw-   0        0        0     9678 2023-03-06 08:20:17.000000 papyrus_structure_pipeline-0.0.3/src/papyrus_structure_pipeline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-03-06 08:20:17.000000 papyrus_structure_pipeline-0.0.3/src/papyrus_structure_pipeline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 08:20:17.000000 papyrus_structure_pipeline-0.0.3/src/papyrus_structure_pipeline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-03-06 08:20:17.000000 papyrus_structure_pipeline-0.0.3/src/papyrus_structure_pipeline.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-03-06 08:20:17.000000 papyrus_structure_pipeline-0.0.3/src/papyrus_structure_pipeline.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 08:20:17.910738 papyrus_structure_pipeline-0.0.3/tests/
--rw-rw-rw-   0        0        0     4049 2023-03-03 09:57:18.000000 papyrus_structure_pipeline-0.0.3/tests/test_standardizer.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:52:19.600894 papyrus_structure_pipeline-0.0.4/
+-rw-rw-rw-   0        0        0     1100 2023-03-03 09:57:18.000000 papyrus_structure_pipeline-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     9678 2023-07-25 06:52:19.600894 papyrus_structure_pipeline-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8781 2023-03-03 10:22:13.000000 papyrus_structure_pipeline-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1257 2023-07-25 06:52:19.606909 papyrus_structure_pipeline-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-03-03 09:57:18.000000 papyrus_structure_pipeline-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:52:19.579452 papyrus_structure_pipeline-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 06:52:19.585221 papyrus_structure_pipeline-0.0.4/src/papyrus_structure_pipeline/
+-rw-rw-rw-   0        0        0      148 2023-07-25 06:50:25.000000 papyrus_structure_pipeline-0.0.4/src/papyrus_structure_pipeline/__init__.py
+-rw-rw-rw-   0        0        0    16113 2023-07-25 06:50:06.000000 papyrus_structure_pipeline-0.0.4/src/papyrus_structure_pipeline/standardizer.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:52:19.599888 papyrus_structure_pipeline-0.0.4/src/papyrus_structure_pipeline.egg-info/
+-rw-rw-rw-   0        0        0     9678 2023-07-25 06:52:19.000000 papyrus_structure_pipeline-0.0.4/src/papyrus_structure_pipeline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-07-25 06:52:19.000000 papyrus_structure_pipeline-0.0.4/src/papyrus_structure_pipeline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:52:19.000000 papyrus_structure_pipeline-0.0.4/src/papyrus_structure_pipeline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-07-25 06:52:19.000000 papyrus_structure_pipeline-0.0.4/src/papyrus_structure_pipeline.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-25 06:52:19.000000 papyrus_structure_pipeline-0.0.4/src/papyrus_structure_pipeline.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 06:52:19.600894 papyrus_structure_pipeline-0.0.4/tests/
+-rw-rw-rw-   0        0        0     4049 2023-03-03 09:57:18.000000 papyrus_structure_pipeline-0.0.4/tests/test_standardizer.py
```

### Comparing `papyrus_structure_pipeline-0.0.3/LICENSE` & `papyrus_structure_pipeline-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `papyrus_structure_pipeline-0.0.3/PKG-INFO` & `papyrus_structure_pipeline-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papyrus_structure_pipeline
-Version: 0.0.3
+Version: 0.0.4
 Summary: Papyrus Structure Pipeline
 Home-page: https://github.com/OlivierBeq/Papyrus_structure_pipeline
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: cheminformatics,molecule,standardization
```

### Comparing `papyrus_structure_pipeline-0.0.3/README.md` & `papyrus_structure_pipeline-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `papyrus_structure_pipeline-0.0.3/setup.cfg` & `papyrus_structure_pipeline-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `papyrus_structure_pipeline-0.0.3/src/papyrus_structure_pipeline/standardizer.py` & `papyrus_structure_pipeline-0.0.4/src/papyrus_structure_pipeline/standardizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """Standardizing methods."""
 
 from enum import Enum, auto
 from typing import Optional, Tuple, Union
 
 from rdkit import Chem
 from rdkit.Chem import AllChem
-from rdkit.Chem.MolStandardize.rdMolStandardize import TautomerEnumerator
+from rdkit.Chem.MolStandardize.rdMolStandardize import TautomerEnumerator, Uncharger
 from rdkit.rdBase import BlockLogs
 
 # Remove warnings of importing the ChEMBL Structure Pipeline
 with BlockLogs():
     from chembl_structure_pipeline import standardizer
     from chembl_structure_pipeline.exclude_flag import exclude_flag
 
@@ -49,82 +49,87 @@
 
 
 # Define salts not flagged by the ChEMBL structure pipeline
 SALTS = ['[Na+]', '[K+]', 'Cl', 'C1=NC=CC=C1', '[O-][Cl+3]([O-])([O-])[O-]', 'O=CN(C)C', '[No]',
          'C', 'C1COCCO1', 'CCCCCCN(C)C', 'CCCCCC', 'CN(C)C(=N)N', 'CN(C)C',
          'c1ccc([B-](c2ccccc2)(c2ccccc2)c2ccccc2)cc1']
 
-
 # Define metals as all but H, B, C, N, O, P, F, S, Cl, Br, I
 METALS = ["He", "Li", "Be", "Ne", "Na", "Mg", "Al", "Si", "Ar", "K", "Ca", "Sc", "Ti", "V", "Cr", "Mn", "Fe", "Co",
           "Ni", "Cu", "Zn", "Ga", "Ge", "As", "Se", "Kr", "Rb", "Sr", "Y", "Zr", "Nb", "Mo", "Tc", "Ru", "Rh", "Pd",
           "Ag", "Cd", "In", "Sn", "Sb", "Te", "Xe", "Cs", "Ba", "La", "Ce", "Pr", "Nd", "Pm", "Sm", "Eu", "Gd", "Tb",
           "Dy", "Ho", "Er", "Tm", "Yb", "Lu", "Hf", "Ta", "W", "Re", "Os", "Ir", "Pt", "Au", "Hg", "Tl", "Pb", "Bi",
           "Po", "At", "Rn", "Fr", "Ra", "Ac", "Th", "Pa", "U", "Np", "Pu", "Am", "Cm", "Bk", "Cf", "Es", "Fm", "Md",
           "No", "Lr", "Rf", "Db", "Sg", "Bh", "Hs", "Mt", "Ds", "Rg", "Cn", "Nh", "Fl", "Mc", "Lv", "Ts", "Og"]
 METALS = [f'[{metal}]' for metal in METALS]
 
-
 # Define organic atoms
 ORGANIC_ATOMS = ['C', 'H', 'O', 'N', 'P', 'S', 'F', 'Cl', 'I', 'Br']
 
 
 def standardize(mol: Chem.Mol,
                 remove_additional_salts: bool = True,
                 remove_additional_metals: bool = True,
                 filter_mixtures: bool = True,
                 filter_inorganic: bool = True,
+                uncharge: bool = True,
                 filter_non_small_molecule: bool = True,
                 canonicalize_tautomer: bool = True,
                 small_molecule_min_mw: float = 200,
                 small_molecule_max_mw: float = 800,
                 tautomer_allow_stereo_removal: bool = True,
                 tautomer_max_tautomers: int = 2 ** 32 - 1,
                 return_type: bool = False,
                 raise_error: bool = True
                 ) -> Union[Chem.Mol, Tuple[Optional[Chem.Mol], StandardizationResult]]:
     """Standardize a molecule from either a RDKit molecule or SMILES.
 
     Steps:
     1) Use the ChEMBL structure pipeline (get parent molecule & standardization)
-    2) If extended:
-        2.1) remove supplementary salts & metals
-        2.2) check if a mixture
-        2.3) check if organic
-        2.4) check if 200 <= MW <= 800
-    3) canonicalize tautomer
-    4) Use the ChEMBL structure pipeline (get parent molecule & standardization)
+    2) remove supplementary salts & metals
+    3) check if a mixture
+    4) check if organic
+    5) uncharge
+    5) check if 200 <= MW <= 800
+    6) canonicalize tautomer
+    7) Use the ChEMBL structure pipeline (get parent molecule & standardization)
 
     :param mol: RDKit molecule to be standardized
     :param remove_additional_salts: should additional salts then those
     dealt with in the ChEMBL Structure Pipeline be removed
     :param remove_additional_metals: should salt removal also remove metal atoms
     :param filter_mixtures: should mixtures be filtered out
     :param filter_inorganic: should inorganic molecules be filtered out
-    :param filter_non_small_molecule: should non-small molecules be filtred out
+    :param uncharge: should formal charges be removed (based on a list of substructures)
+    :param filter_non_small_molecule: should non-small molecules be filtered out
     :param canonicalize_tautomer: should a canonical tautomer be determined
     :param small_molecule_min_mw: minimum molecular weight to be a valid small molecule
     :param small_molecule_max_mw: maximum molecular weight to be a valid small molecule
-    :param tautomer_allow_stereo_removal: allow stereocenters to be remove by tautomerization
+    :param tautomer_allow_stereo_removal: allow stereocenters to be removed by tautomerization
     :param tautomer_max_tautomers: maximum number of tautomers to enumerate (ignored if 0)
     :param return_type: If True, include the `StandardizationResult` in the return value
+    :param raise_error: If True, standardization failures raise exceptions, if False, None is returned
+    (with the standardization error if `return_type` is set).
     :return: a tuple of either the standardized molecule or None and a standardization_result flag
     """
     # Apply ChEMBL standardization
     try:
         std_mol = _apply_chembl_standardization(mol)
         # Remove additional salts
         if remove_additional_salts:
             std_mol = _remove_supplementary_salts(std_mol, include_metals=remove_additional_metals)
         # Ensure is not a mixture
         if filter_mixtures and is_mixture(std_mol):
             return (None, StandardizationResult.MIXTURE_MOLECULE) if return_type else None
         # Ensure organic
         if filter_inorganic and not is_organic(std_mol):
             return (None, StandardizationResult.INORGANIC_MOLECULE) if return_type else None
+        # Remove charges
+        if uncharge:
+            std_mol = _uncharge(std_mol)
         # Ensure small molecule
         if filter_non_small_molecule and not is_small_molecule(std_mol,
                                                                min_molwt=small_molecule_min_mw,
                                                                max_molwt=small_molecule_max_mw):
             return (None, StandardizationResult.NON_SMALL_MOLECULE) if return_type else None
         # Obtain canonical tautomer
         if canonicalize_tautomer:
@@ -174,21 +179,22 @@
         raise ValueError('A RDKit molecule must be specified')
     block = BlockLogs()  # Disable RDKit outputs
     # Parameter of tautomer enumeration
     enumerator = TautomerEnumerator()
     enumerator.SetMaxTautomers(max_tautomers)
     # Enumerate tautomers
     if allow_stereo_removal:
+        enumerator.SetRemoveSp3Stereo(True)
+        enumerator.SetRemoveBondStereo(True)
         tautos = enumerator.Enumerate(mol)
     else:
         enumerator.SetRemoveSp3Stereo(False)
+        enumerator.SetRemoveBondStereo(False)
         tautos = enumerator.Enumerate(mol)
-
-        # Keep those with stereo unchanged if required
-
+        # Keep tautomers with stereo unchanged if required
         def get_num_ciral_centers(mol_: Chem.Mol):
             """Utility function."""
             return len([atom.GetChiralTag()
                         for atom in mol_.GetAtoms()
                         if atom.GetChiralTag() != AllChem.ChiralType.CHI_UNSPECIFIED])
 
         orig_chiral_centers = get_num_ciral_centers(mol)
@@ -299,7 +305,48 @@
         return frags[0] if not return_type else (frags[0], SaltStrippingResult.STRIPPED_MOLECULE)
     # Otherwise combine remaining fragments
     else:
         res = frags[0]
         for frag in frags[1:]:
             res = Chem.CombineMols(res, frag)
         return res if not return_type else (res, SaltStrippingResult.STRIPPED_MOLECULE)
+
+
+def _uncharge(mol: Chem.Mol) -> Chem.Mol:
+    """Uncharge the given RDKit molecule.
+
+    Adapted from Hans de Winter's contribution to B3DB
+    (https://github.com/theochem/B3DB/blob/main/cleaning/02_clean_smiles_chembl_way_20210215.py)
+    """
+    if mol is None:
+        raise ValueError('A RDKit molecule must be specified')
+    uncharger = Uncharger()
+    mol = uncharger.uncharge(mol)
+    # Do a second pass on zwitterions
+    romol = Chem.RWMol(mol)
+    neutralizing_smiles = [  # Imidazoles
+        ('[n+;H]', 'n'),
+        # Amines
+        ('[N+;!H0]', 'N'),
+        # Carboxylic acids and alcohols
+        ('[$([O-]);!$([O-][#7])]', 'O'),
+        # Thiols
+        ('[S-;X1]', 'S'),
+        # Sulfonamides
+        ('[$([N-;X2]S(=O)=O)]', 'N'),
+        # Enamines
+        ('[$([N-;X2][C,N]=C)]', 'N'),
+        # Tetrazoles
+        ('[n-]', '[nH]'),
+        # Sulfoxides
+        ('[$([S-]=O)]', 'S'),
+        # Amides
+        ('[$([N-]C=O)]', 'N')
+    ]
+    neutralizing_reactions = [(Chem.MolFromSmarts(x), Chem.MolFromSmiles(y, False)) for x, y in neutralizing_smiles]
+    for i, (reactant, product) in enumerate(neutralizing_reactions):
+        while romol.HasSubstructMatch(reactant):
+            rms = AllChem.ReplaceSubstructs(romol, reactant, product)
+            romol = rms[0]
+    mol = Chem.Mol(romol)
+    Chem.SanitizeMol(mol)
+    return mol
```

### Comparing `papyrus_structure_pipeline-0.0.3/src/papyrus_structure_pipeline.egg-info/PKG-INFO` & `papyrus_structure_pipeline-0.0.4/src/papyrus_structure_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papyrus-structure-pipeline
-Version: 0.0.3
+Version: 0.0.4
 Summary: Papyrus Structure Pipeline
 Home-page: https://github.com/OlivierBeq/Papyrus_structure_pipeline
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: cheminformatics,molecule,standardization
```

### Comparing `papyrus_structure_pipeline-0.0.3/tests/test_standardizer.py` & `papyrus_structure_pipeline-0.0.4/tests/test_standardizer.py`

 * *Files identical despite different names*

