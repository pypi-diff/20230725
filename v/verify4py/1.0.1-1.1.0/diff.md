# Comparing `tmp/verify4py-1.0.1.tar.gz` & `tmp/verify4py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verify4py-1.0.1.tar", last modified: Fri Jul 21 04:08:23 2023, max compression
+gzip compressed data, was "verify4py-1.1.0.tar", last modified: Tue Jul 25 06:29:11 2023, max compression
```

## Comparing `verify4py-1.0.1.tar` & `verify4py-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:08:23.507861 verify4py-1.0.1/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1065 2022-04-11 09:13:53.000000 verify4py-1.0.1/LICENSE
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9388 2023-07-21 04:08:23.507861 verify4py-1.0.1/PKG-INFO
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     8817 2023-07-21 04:05:08.000000 verify4py-1.0.1/README.md
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       84 2022-04-11 09:22:24.000000 verify4py-1.0.1/pyproject.toml
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       38 2023-07-21 04:08:23.507861 verify4py-1.0.1/setup.cfg
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      907 2023-07-21 04:08:19.000000 verify4py-1.0.1/setup.py
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:08:23.503860 verify4py-1.0.1/src/
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:08:23.503860 verify4py-1.0.1/src/verify4py/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    10980 2023-07-21 04:05:08.000000 verify4py-1.0.1/src/verify4py/Issuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3815 2022-05-13 07:31:57.000000 verify4py-1.0.1/src/verify4py/JsonIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2909 2022-07-06 07:22:13.000000 verify4py-1.0.1/src/verify4py/PdfIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3662 2022-07-06 10:35:49.000000 verify4py-1.0.1/src/verify4py/UniversityDiplomaIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        0 2022-04-11 09:38:54.000000 verify4py-1.0.1/src/verify4py/__init__.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    27300 2023-07-21 04:05:08.000000 verify4py-1.0.1/src/verify4py/certify_sc_utils.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2788 2022-05-10 06:21:26.000000 verify4py-1.0.1/src/verify4py/chainpoint.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1067 2022-07-06 08:44:53.000000 verify4py-1.0.1/src/verify4py/json_utils.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      689 2022-07-06 07:08:53.000000 verify4py-1.0.1/src/verify4py/pdf.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    19898 2022-07-04 09:06:21.000000 verify4py-1.0.1/src/verify4py/university_abi.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1526 2023-07-21 04:05:08.000000 verify4py-1.0.1/src/verify4py/utils.py
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-21 04:08:23.503860 verify4py-1.0.1/src/verify4py.egg-info/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9388 2023-07-21 04:08:23.000000 verify4py-1.0.1/src/verify4py.egg-info/PKG-INFO
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      537 2023-07-21 04:08:23.000000 verify4py-1.0.1/src/verify4py.egg-info/SOURCES.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        1 2023-07-21 04:08:23.000000 verify4py-1.0.1/src/verify4py.egg-info/dependency_links.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       42 2023-07-21 04:08:23.000000 verify4py-1.0.1/src/verify4py.egg-info/requires.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       10 2023-07-21 04:08:23.000000 verify4py-1.0.1/src/verify4py.egg-info/top_level.txt
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-25 06:29:11.228254 verify4py-1.1.0/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1065 2022-04-11 09:13:53.000000 verify4py-1.1.0/LICENSE
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9382 2023-07-25 06:29:11.228254 verify4py-1.1.0/PKG-INFO
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     8817 2023-07-21 04:05:08.000000 verify4py-1.1.0/README.md
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       84 2022-04-11 09:22:24.000000 verify4py-1.1.0/pyproject.toml
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       38 2023-07-25 06:29:11.228254 verify4py-1.1.0/setup.cfg
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      879 2023-07-25 06:29:03.000000 verify4py-1.1.0/setup.py
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-25 06:29:11.224254 verify4py-1.1.0/src/
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-25 06:29:11.224254 verify4py-1.1.0/src/verify4py/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    10496 2023-07-25 06:27:39.000000 verify4py-1.1.0/src/verify4py/Issuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3509 2023-07-25 06:27:39.000000 verify4py-1.1.0/src/verify4py/JsonIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2909 2022-07-06 07:22:13.000000 verify4py-1.1.0/src/verify4py/PdfIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3662 2022-07-06 10:35:49.000000 verify4py-1.1.0/src/verify4py/UniversityDiplomaIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        0 2022-04-11 09:38:54.000000 verify4py-1.1.0/src/verify4py/__init__.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    27300 2023-07-21 04:05:08.000000 verify4py-1.1.0/src/verify4py/certify_sc_utils.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1067 2022-07-06 08:44:53.000000 verify4py-1.1.0/src/verify4py/json_utils.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      689 2022-07-06 07:08:53.000000 verify4py-1.1.0/src/verify4py/pdf.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    19898 2022-07-04 09:06:21.000000 verify4py-1.1.0/src/verify4py/university_abi.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1526 2023-07-21 04:05:08.000000 verify4py-1.1.0/src/verify4py/utils.py
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2023-07-25 06:29:11.224254 verify4py-1.1.0/src/verify4py.egg-info/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     9382 2023-07-25 06:29:10.000000 verify4py-1.1.0/src/verify4py.egg-info/PKG-INFO
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      509 2023-07-25 06:29:11.000000 verify4py-1.1.0/src/verify4py.egg-info/SOURCES.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        1 2023-07-25 06:29:10.000000 verify4py-1.1.0/src/verify4py.egg-info/dependency_links.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       23 2023-07-25 06:29:11.000000 verify4py-1.1.0/src/verify4py.egg-info/requires.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       10 2023-07-25 06:29:11.000000 verify4py-1.1.0/src/verify4py.egg-info/top_level.txt
```

### Comparing `verify4py-1.0.1/LICENSE` & `verify4py-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.1/PKG-INFO` & `verify4py-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: verify4py
-Version: 1.0.1
+Version: 1.1.0
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6,<3.11
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Verify4py 
 Verify4py нь сертификат, диплом, дансны хуулга зэрэг бичиг баримтыг блокчэйн дээр
 баталгаажуулж өгөх https://github.com/corex-mn/certify-sc ухаалаг гэрээтэй харьцдаг python хэлний сан юм.
```

### Comparing `verify4py-1.0.1/README.md` & `verify4py-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.1/setup.py` & `verify4py-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="verify4py",
-    version="1.0.1",
+    version="1.1.0",
     author="Surenbayar Doloonjin",
     author_email="surenbayar@corex.mn",
     description="Issue certificates using blockchain and smart contract",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/teo-mn/verify4py",
     project_urls={
@@ -18,10 +18,10 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6,<3.11",
-    install_requires=['web3==6.6.1', 'merkletools==1.0.3', 'pdfrw==0.3']
+    python_requires=">=3.6",
+    install_requires=['web3==6.6.1', 'pdfrw==0.3']
 )
```

### Comparing `verify4py-1.0.1/src/verify4py/Issuer.py` & `verify4py-1.1.0/src/verify4py/Issuer.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import time
 
 from web3 import Web3
 from web3.auto import w3
 import verify4py.utils as Utils
 from verify4py.certify_sc_utils import abi as abi_cert
 from verify4py.university_abi import abi as abi_univ
-from verify4py.chainpoint import ChainPointV2
 
 DEFAULT_GAS_LIMIT = 2000000
 VERSION = "v1.0-python"
 
 
 class Issuer:
     def __init__(self, smart_contract_address,
@@ -61,22 +60,19 @@
               passphrase: str = "",
               do_hash=False,
               hash_image: str = "",
               hash_json: str = ""
               ):
         pk = self.get_pk(private_key, key_store, passphrase)
 
-        cp = ChainPointV2(self.hash_type)
-        cp.add_leaf([hash_value], do_hash=do_hash)
-        cp.make_tree()
         # check credit
         if self.get_credit(self.issuer_address) == 0:
             raise ValueError("Not enough credit")
 
-        cert = self.get_certificate(cp.get_merkle_root())
+        cert = self.get_certificate(hash_value)
 
         if cert.isRevoked:  # isRevoked flag
             raise ValueError("Certificate revoked")
 
         if cert.id > 0:  # id
             raise ValueError("Certificate already registered")
 
@@ -85,17 +81,17 @@
 
         tx, error = self.__issue_util(hash_value, self.issuer_address, id, expire_date, VERSION, desc, pk,
                                       hash_image, hash_json)
         if error is not None:
             print(error)
             raise RuntimeError(error)
             # insert proof
-        proof = cp.get_receipt(0, tx, self.chain_id != 1104)
 
-        return (tx, proof), None
+
+        return (tx, None), None
 
     def __issue_util(self, hash_value, issuer_address, cert_num, expire_date, version, desc, pk,
                      hash_image="", hash_json=""):
         nonce = self.__client.eth.get_transaction_count(self.__client.to_checksum_address(issuer_address))
         try:
             if self.contract_type == "":
                 func = self.__contract_instance.functions.addCertification(hash_value, cert_num, expire_date, version,
@@ -127,64 +123,61 @@
             {'from': issuer_address, 'gasPrice': self.__client.to_wei('1000', 'gwei'),
              'nonce': nonce, 'gas': DEFAULT_GAS_LIMIT})
         signed = self.__client.eth.account.sign_transaction(tx, pk)
         tx_hash2 = self.__client.eth.send_raw_transaction(signed.rawTransaction)
         self.__client.eth.wait_for_transaction_receipt(tx_hash2)
 
     def revoke(self,
-               merkle_root,
+               hash,
                revoker_name,
                private_key: str = "",
                key_store="",
                passphrase: str = ""):
         pk = self.get_pk(private_key, key_store, passphrase)
         # check credit
         if self.get_credit(self.issuer_address) == 0:
             raise ValueError("Not enough credit")
 
-        cert = self.get_certificate(merkle_root)
+        cert = self.get_certificate(hash)
 
         if cert.id == 0:
             raise ValueError("Certificate not found")
         if cert.isRevoked:
             raise ValueError("Certificate already revoked")
 
-        tx, error = self.revoke_util(merkle_root, self.issuer_address, revoker_name, pk)
+        tx, error = self.revoke_util(hash, self.issuer_address, revoker_name, pk)
         if error is not None:
             print(error)
             raise RuntimeError(error)
 
         return tx, None
 
-    def revoke_util(self, merkle_root, revoker_address, revoker_name, pk):
+    def revoke_util(self, hash, revoker_address, revoker_name, pk):
         nonce = self.__client.eth.get_transaction_count(self.__client.to_checksum_address(revoker_address))
 
         try:
-            func = self.__contract_instance.functions.revoke(merkle_root, revoker_name)
+            func = self.__contract_instance.functions.revoke(hash, revoker_name)
             tx = func.build_transaction(
                 {'from': revoker_address, 'gasPrice': self.__client.to_wei('1000', 'gwei'), 'nonce': nonce,
                  'gas': DEFAULT_GAS_LIMIT})
             signed = self.__client.eth.account.sign_transaction(tx, pk)
             tx_hash = self.__client.eth.send_raw_transaction(signed.rawTransaction)
             tx_res = self.__client.eth.wait_for_transaction_receipt(tx_hash)
             if tx_res.status == 1:
                 return self.__client.to_hex(tx_hash), None
             return '', 'Failed on blockchain'
         except Exception as e:
             print(e)
             return '', e
 
-    def verify_hash(self, hash_value, chainpoint_proof: str):
-        proof = json.loads(chainpoint_proof)['proof']
-        cp = ChainPointV2(self.hash_type)
-        merkle_root = cp.calc_merkle_root(proof, hash_value)
-        self.verify_root(merkle_root)
+    def verify_hash(self, hash_value):
+        self.verify_root(hash_value)
 
-    def verify_root(self, merkle_root):
-        cert = self.get_certificate(merkle_root)
+    def verify_root(self, hash):
+        cert = self.get_certificate(hash)
         issuer = self.get_issuer(cert.issuer)
         state = 'ISSUED'
         if cert.id == 0:
             raise Exception("Hash not found in smart contract")
         if cert.isRevoked:
             state = 'REVOKED'
         else:
@@ -209,16 +202,16 @@
             arr2 = self.__contract_instance.functions.getRevokeInfo(arr[2]).call()
             if arr2[1] is True:
                 return False
             else:
                 return True
         return False
 
-    def get_certificate(self, merkle_root):
-        arr = self.__contract_instance.functions.getCertification(merkle_root).call()
+    def get_certificate(self, hash):
+        arr = self.__contract_instance.functions.getCertification(hash).call()
         if self.contract_type == "":
             return CertStruct({
                 'id': arr[0],
                 'certNum': arr[1],
                 'hash': arr[2],
                 'issuer': arr[3],
                 'expireDate': arr[4],
@@ -227,15 +220,15 @@
                 'version': arr[7],
                 'description': arr[8],
                 'revokerName': arr[9],
                 'revokedAt': arr[10],
                 'txid': arr[11]
             })
 
-        arr2 = self.__contract_instance.functions.getRevokeInfo(merkle_root).call()
+        arr2 = self.__contract_instance.functions.getRevokeInfo(hash).call()
         return CertStruct({
             'id': arr[0],
             'certNum': arr[1],
             'hash': arr[2],
             'image_hash': arr[3],
             'meta_hash': arr[4],
             'issuer': arr[5],
```

### Comparing `verify4py-1.0.1/src/verify4py/JsonIssuer.py` & `verify4py-1.1.0/src/verify4py/JsonIssuer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import os
 
 import verify4py.utils as Utils
 from verify4py.Issuer import Issuer, VERSION
-from verify4py.chainpoint import ChainPointV2
 from verify4py.json_utils import json_wrap
 
 
 class JsonIssuer(Issuer):
     def __init__(self,
                  smart_contract_address,
                  node_host,
@@ -65,32 +64,29 @@
                 json.dump(json_data, f, indent=4)
         return tx, error
 
     def verify_json(self, file_path: str):
         if not os.path.exists(file_path) or not os.path.isfile(file_path):
             raise ValueError('Source path should be valid')
 
-        merkle_root = self.__verify_json_file(file_path)
-        return self.verify_root(merkle_root)
+        hash = self.__verify_json_file(file_path)
+        return self.verify_root(hash)
 
     def revoke_json(self, file_path: str, revoker_name: str,
                     private_key: str = "",
                     key_store="",
                     passphrase: str = ""):
         if not os.path.exists(file_path) or not os.path.isfile(file_path):
             raise ValueError('Source path should be valid')
-        merkle_root = self.__verify_json_file(file_path)
-        return self.revoke(merkle_root, revoker_name, private_key, key_store, passphrase)
+        hash = self.__verify_json_file(file_path)
+        return self.revoke(hash, revoker_name, private_key, key_store, passphrase)
 
     def __verify_json_file(self, file_path):
         f = open(file_path)
         json_data = json.load(f)
         verifymn = json_data['verifymn']
         chainpoint_proof = verifymn.pop("chainpointProof", None)
         json_data['verifymn'] = verifymn
         json_data['verifymn'] = verifymn
         wrapped_json_str = json_wrap(json_data)
         hash_val = Utils.calc_hash_str(wrapped_json_str)
-        chainpoint = ChainPointV2()
-        if not chainpoint.validate_proof(chainpoint_proof['proof'], hash_val, chainpoint_proof['merkleRoot']):
-            raise ValueError("Chainpoint proof doesn't match")
-        return chainpoint_proof['merkleRoot']
+        return hash_val
```

### Comparing `verify4py-1.0.1/src/verify4py/PdfIssuer.py` & `verify4py-1.1.0/src/verify4py/PdfIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.1/src/verify4py/UniversityDiplomaIssuer.py` & `verify4py-1.1.0/src/verify4py/UniversityDiplomaIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.1/src/verify4py/certify_sc_utils.py` & `verify4py-1.1.0/src/verify4py/certify_sc_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.1/src/verify4py/json_utils.py` & `verify4py-1.1.0/src/verify4py/json_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.1/src/verify4py/pdf.py` & `verify4py-1.1.0/src/verify4py/pdf.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.1/src/verify4py/university_abi.py` & `verify4py-1.1.0/src/verify4py/university_abi.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.1/src/verify4py/utils.py` & `verify4py-1.1.0/src/verify4py/utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-1.0.1/src/verify4py.egg-info/PKG-INFO` & `verify4py-1.1.0/src/verify4py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: verify4py
-Version: 1.0.1
+Version: 1.1.0
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6,<3.11
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Verify4py 
 Verify4py нь сертификат, диплом, дансны хуулга зэрэг бичиг баримтыг блокчэйн дээр
 баталгаажуулж өгөх https://github.com/corex-mn/certify-sc ухаалаг гэрээтэй харьцдаг python хэлний сан юм.
```

