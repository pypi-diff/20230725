# Comparing `tmp/AshCrypt-3.0.1.tar.gz` & `tmp/AshCrypt-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-3.0.1.tar", last modified: Sun Jul 23 12:59:24 2023, max compression
+gzip compressed data, was "dist/AshCrypt-3.0.2.tar", last modified: Tue Jul 25 15:02:41 2023, max compression
```

## Comparing `AshCrypt-3.0.1.tar` & `AshCrypt-3.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:59:24.000000 AshCrypt-3.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:59:24.000000 AshCrypt-3.0.1/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)    38088 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/AshCrypt/AshCryptGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:59:24.000000 AshCrypt-3.0.1/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 12:59:24.000000 AshCrypt-3.0.1/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-23 12:59:24.000000 AshCrypt-3.0.1/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-23 12:59:24.000000 AshCrypt-3.0.1/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 12:59:24.000000 AshCrypt-3.0.1/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-23 12:59:24.000000 AshCrypt-3.0.1/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-23 12:59:24.000000 AshCrypt-3.0.1/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-23 12:59:24.000000 AshCrypt-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 12:59:24.000000 AshCrypt-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-23 12:59:14.000000 AshCrypt-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38088 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:02:41.000000 AshCrypt-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-25 15:02:27.000000 AshCrypt-3.0.2/setup.py
```

### Comparing `AshCrypt-3.0.1/AshCrypt/AshCryptGUI.py` & `AshCrypt-3.0.2/AshCrypt/gui.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.1/AshCrypt/clicrypt.py` & `AshCrypt-3.0.2/AshCrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.1/AshCrypt/crypt.py` & `AshCrypt-3.0.2/AshCrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.1/AshCrypt/filecrypt.py` & `AshCrypt-3.0.2/AshCrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.1/AshCrypt/textcrypt.py` & `AshCrypt-3.0.2/AshCrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.1/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-3.0.2/AshCrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.1/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-3.0.2/AshCrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.1
+Version: 3.0.2
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-3.0.1/PKG-INFO` & `AshCrypt-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.1
+Version: 3.0.2
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-3.0.1/README.md` & `AshCrypt-3.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 My aim here is to make these tools accessible and user-friendly, even for individuals with a limited programming knowledge. By providing these resources, I hope to contribute to the preservation of privacy and enable individuals to take control of their own data security, so feel free to explore these tools.
 ## Overview ## 
 ![alt text](important/GUI.png)
 The project incorporates an App & a library called **AshCrypt** : 
 
 **App :** 
 <br>Full-fledged application that integrates all the modules in the library merging them into a unified and powerful software solution for developers and for people with no programming knowledge whatsoever
-<br>check [GUI](https://github.com/AshGw/AES-256#AshCryptGUI) header for more info.
+<br>check [GUI](https://github.com/AshGw/AES-256#GUI) header for more info.
 
 **Library :** 
 <br>A simple, secure, and developer-oriented library for performing encryption and decryption operations on data using the AES-256 (CBC) encryption algorithm.
 <br>The core of the library is the module `crypt`
 It offers cryptographic capabilities and top security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
@@ -33,50 +33,41 @@
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner.
 
 <br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [database](https://github.com/AshGw/AES-256#database-1) header to learn more.
 
 ## Installation ##
-There are many ways to go by this : 
 ### If you want to use it as a library ###
 You can simply use **pip**
 <br>First upgrade the package installer 
 ```bash
 pip install --upgrade pip 
 ```
 Then install the Library 
 ```bash
 pip install AshCrypt
 ```
 This will install the latest version of `AshCrypt`.
 You can start using it in your code by importing its modules :
 
 ```python
-from AshCrypt.crypt import *
+from AshCrypt import crypt as ac
 ```
 That's it.
-### Ready-to-go Executable files:
-If you want to use the App right away : 
-<br>**For Windows** : Download this repo as a ZIP file, extract the content
-<br>then click on `Executables > AshCryptGUI.exe` This will automatically run the GUI
 
 ### Whole repo installation 
 Now if you want to get the whole repo with no manual configurations
 <br>Run this command in the Terminal
 ```bash
 curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/important/setup.sh | bash
 ```
 This will run the commands in [setup.sh](important/setup.sh).
 <br>It will clone & install all the dependencies needed on your machine and activate the development mode, inside the directory you're currently at.
 
-you can use this command to automate the environment setup process if you haven't done it  already
-```bash
-curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/Docker-build/env-setup.sh | bash
-```
 <details>
 <summary>Got Errors ?</summary>
 
 <h5>For Debian based systems</h5>
 
 1) Install `curl` if you don't have it already 
 ```bash
@@ -93,15 +84,15 @@
 ```
 <br>Now if none of this works you might just use the docker image for this purpose, so check this [directory](Docker-build)
 </details>
 
 **After the library is installed** 
 <br>To run the GUI 
 ```shell
-python -m AshCrypt.AshCryptGUI
+python -m AshCrypt.gui
 ```
 
 **NOTE**:
 You  can use `clicrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints intended for use within systems where you can't use GUI's.
 
 
 To run the CLI 
@@ -145,25 +136,25 @@
 ```python
 message = b'dG\xe2\x91\x18\x8dC\x81\x04\xd7.D\xf9\t\xf8\x81\x06\xe8\xf2\n\x15\xa5b\xcf\xb2\xda\x93\x96\x05\xad\xa1\x1a\xb5\x08\xaf\xe8x\xcc\xf8\xa1\xe9B`\xdaL\xf8\xd6r\xcd"\n\x93\xb0\xda\xce@\x14;\xd1\xdcd\x9c\xd6X\xc5\xd1\xeb:\x91\x8c\xd4\xcd\xf9\xcdP\xea\xf4VJH\xf5\x83m(/\xa2[\xcdK\xc4$\xbd\xf1\xbd\x8d\xbe\x17\'\xb5\xb2)\xa88\n\xfb`\xfeX\x1c\t\xd2`\x00\x00\x002\x00\xd2;\x9a\x93\xf2XB|\xd7C\xe6\xa9\'\xc6\xb3j\x1b\xe7\x82(\x05\xact`\xd7\x8d\xa0\xec\xea\xaf|'
 ```
 3) Now pass the arguments accordingly. If you have a normal message and you try to decrypt it, an Exception will be raised so pass the arguments to the right classes. 
 <br><br>So first create an instance of either the `Enc` or `Dec` class. 
 <br>Here I chose to encrypt a message 
 ```python
-instanceE = Enc(message=message, mainkey=mainkey)
+a = Enc(message=message, mainkey=mainkey)
 ```
 
 4) Now you'd have to specify the output, you can encrypt to bytes or encrypt to URL-safe strings.
 <br> Here I chose to encrypt to bytes
 ```python
-output = instanceE.enc_to_bytes()
+output = a.enc_to_bytes()
 ```
 you can also encrypt to a URL safe string
 ```python
-output = instanceE.enc_to_str()
+output = a.enc_to_str()
 ```
 <br> The same logic applies to the decryption process simply switch `Enc` with `Dec` and `enc_to_bytes` to `dec_to_bytes`
 That simple, that's it.
 
 
 
 
@@ -185,55 +176,14 @@
 - Encrypting to a string has URL-safe string representation 
 ### Regarding KDFs
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50 ( which is secure enough ), the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
 <br>You can check how it works by checking this [Jupyter Notebook](demo/performance-check.ipynb) demo file
-## AshCryptGUI ##
-The GUI as mentioned above is a fully functional application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
-### Usage ###
-1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. Then insert it in the `MAINKEY` entry
-2) Now you're able to encrypt files or text (text is limited to 200 characters max)
-####  Text : 
-- You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
-- Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
-<br>If the text cannot be decrypted it will display itself , so you might as well use this to display the key you're using as a qr code 
-
-#### Files
-- Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
-- The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extension you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
-#### Database
-- Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by 
-1) Specify the actual path where you want your database to be 
-2) Give it a name, it must be a valid file name that ends with `.db` .<br>
-If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically connect.
-3) Did I mention the keys' database ? well if you give a database it will also create a keys database with the same name as the database you chose plus `Keys` added to its name. This database holds the actual keys and the reference to these keys.
-<br>The only common piece of data that the two separate databases have in common are the key reference values.  
-
-**Note** : If your main database gets compromised , then the attacker wouldnt have anything useful , they can never know the actual key from the reference key so no problem with that if it only contains encrypted content BUT NEVER GET YOUR KEYS DATABASE EXPOSED ! 
-<br>If anyone gets hold of your main database they would only see some encrypted content and some key reference that is actually 100% independent of the actual key used for encryption so they have nothing , but if they get hold of the keys database they can look for matching refs and use the matching key to decrypt that binary encrypted data to its actual format.
-That's why I made two different databases not two tables within a single database. 
-<br> So you keep your keys database safe and secure.
-
-
-**Info** Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
-`Name` that holds the filename in both databases , although in the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
-<br>`Contnet` in the main db that holds the entire content of the given file, in keys db that holds the actual 256 bit long encryption key.
-<br>`Key` in  both db's that holds the `KeyRef` or key reference value
-#### Usage 
-The buttons are self-explanatory so do what you see fit. the result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
-<br>Just click buttons and check the result in the output console, it will guide you through the process.
-
-<br>To run the GUI anywhere
-```shell
-python -m AshCrypt.AshCryptGUI
-```
-
-
 
 
 ## filecrypt ## 
 If you want to encrypt a file :
 1) Follow the steps above to set the key up.
 2) Create an instance of the class CryptFiles and pass 2 arguments, the first one being the target file and the second argument being the key :
 ```python
@@ -315,70 +265,107 @@
 
 **content** : This can be a single character or a whole movie in binary, that depends on your specific needs.
 
 **key** : This key column wasn't indeed meant to store a key itself but rather store a reference to the actual key. The key itself should be stored somewhere else safe and secure preferably off-grid and completely separate from any vulnerable devices on you can have it on a separate database stored safely away, you can even write it down on a piece of paper if you want , just make sure to rotate your keys from time to time.
 
 1) Create a connection to the database :
 ```python
-connect = Database('test.db')
+conn = Database('test.db')
 ```
 This would automatically set the default table name to `Classifed` if no arguments are passed to the other class functions then they would all be working on the default table name , if you want to set your default table name instead of `Classified` you can pass your table name as the second argument : 
 ```python
-connect = Database('test.db','MyDefaultTable')
+conn = Database('test.db','MyDefaultTable')
 ```
 2) create/add the table to the database :
 ```python
-connect.addtable()
+conn.addtable()
 ```
 Added the default table that's been set to the database,  if you want to pass an argument to the function that would create another table of your choice
 
 3) Set a reference to the key not the key itself : 
 ```python
  key = '#5482A'
 ```
 4) Use the connection to perform various tasks <br>
 The content can be anything post encryption bytes or string format
 ```python
 content='Some Encrypted Content'
-connect.insert(content=content,key='#1E89JO', optional_table_name=None)
+conn.insert(content=content,key='#1E89JO', optional_table_name=None)
 ```
 If the optional table name is `None` then it will insert into the default table , else it would insert into the table you specify
 
 
 5) You can check the tables you have , it returns a generator object, yields the result of each element so you must run a for loop over it
 ```python
-for e in connect.show_tables():
+for e in conn.show_tables():
         print(e)
 ```
 You can check the current size of the database using the size property method 
 ```python
-print(connect.size) # Size of the Database in MB 
+print(conn.size) # Size of the Database in MB 
 ```
 
 6) Check the module itself so you can run through all the available methods.
 <br>The methods available perform the usual operations like insertion, deletion , updating the database and more..
 
 
 7) to run more complex queries I've dedicated a query function that takes in `*queries` and returns the result fetched 
 ```python
 query = 'SELECT COUNT(*) AS cc ,content FROM Classified WHERE key = "#5482A" ORDER BY cc DESC '
-print(connect.query(query))
+print(conn.query(query))
 ```
 The result fetched should look like this : 
  ```python
 [{'query 0': ['SUCCESS', [(1, 'some encrypted content of bytes or strings')]]}]
 ```
 If some error has occurred while querying like : 
 ```python
 query = 'SELECT COUNT(*) AS cc ,content FROM DoesntExist WHERE key = "#5482A" ORDER BY cc DESC '
 ```
 The result fetched should look similar to this : 
 ```python
 [{'query 0': ('FAILURE', 'no such table: DoesntExist')}]
 ```
-Thats it so simple !
+That's it so simple !
+
+
+## GUI ##
+The GUI as mentioned above is a fully functional application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
+### Usage ###
+1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. Then insert it in the `MAINKEY` entry
+2) Now you're able to encrypt files or text (text is limited to 200 characters max)
+####  Text : 
+- You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
+- Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
+<br>If the text cannot be decrypted it will display itself , so you might as well use this to display the key you're using as a qr code 
+
+#### Files
+- Under the `FILE PATH` label enter the file name (if it's in the current working directory) or submit the whole file path , the file can be of any type, click on `ENCRYPT FILE` Button to encrypt the given file , if the encryption turned out to be successful , you'll see a success message along with a `added .crypt extention to the file` message if the encryption wasn't successful you'll see an error message specifying the problem.<br>Note that you cannot re-encrypt a file that  has `.crypt` as extention.
+- The file name should be changed by now to `filename + '.crypt'` , if the file has .crypt extension you can go ahead and decrypt it , if the same key is used for both enc/dec operations then the result should be `success` + `removed .crypt extention` from the file.
+#### Database
+- Now you have some encrypted/decrypted files but you want to keep them stored somewhere safe, this is where the main database comes in , where you need to store your files + their content + reference to the key used for their encryption/decryption. you can specify your database by :
+1) Specifying the actual path where you want your database to be 
+2) Give it a name, it must be a valid file name that ends with `.db` .<br>
+If the database doesn't exist then a database with the name you've given will be created and automatically connected to.<br>If the given database already exists then it will automatically connect.
+3) Did I mention the keys' database ? well if you give a database file name it will also create the keys database with the same name as the database you chose plus `Keys` added to its name. This database holds the actual keys and the reference to these keys.
+<br>The only common data that these two separate databases have in common is the key reference values.  
+
+   
+**Info** Both databases have the same table called `Classified` that has 4 columns <br>`ID` which is auto generated & incremented for each piece of data that gets inserted<br>
+`Name` that holds the filename in both databases , although in the keys database if you haven't specified any file to operate on and keep selecting keys the keys name will be `STANDALONE` 
+<br>`Content` in the main db, that holds the entire content of the given file whereas for the keys db that holds the actual 256 bit encryption key.
+<br>`Key` in  both db's that holds the `KeyRef` or key reference value
+#### Usage 
+The buttons are self-explanatory so do what you see fit. the result of any task related to the databases is displayed in `DATABASE OUTPUT CONSOLE` although you can run a query anytime by writing a query and using `query` button , the result will be displayed to an `output.json` file that auto-deletes when you exit the app.
+<br>Just click buttons and check the result in the output console, it will guide you through the process.
+
+<br>To run the GUI anywhere
+```shell
+python -m AshCrypt.gui
+```
+
 
 ## License ##
 This project is licensed under the [MIT LICENSE](https://github.com/AshGw/AES-256/blob/main/LICENSE).
 ## Acknowledgments ##
 This cryptographic scheme is inspired by secure cryptographic practices and various open-source implementations.
```

### Comparing `AshCrypt-3.0.1/setup.py` & `AshCrypt-3.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('AshCrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='3.0.1',
+    version='3.0.2',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

