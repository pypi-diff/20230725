# Comparing `tmp/dwiqc-0.8.0-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,27 @@
-Zip file size: 27661 bytes, number of entries: 24
+Zip file size: 29453 bytes, number of entries: 25
 -rw-r--r--  2.0 unx      225 b- defN 23-Jul-05 14:23 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-Jul-24 16:32 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jul-25 18:46 dwiqc/__version__.py
 -rw-r--r--  2.0 unx     1352 b- defN 23-Jul-05 14:23 dwiqc/browser/__init__.py
--rw-r--r--  2.0 unx       61 b- defN 23-Jul-05 14:23 dwiqc/cli/__init__.py
+-rw-r--r--  2.0 unx       94 b- defN 23-Jul-25 18:43 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6998 b- defN 23-Jul-24 15:35 dwiqc/cli/get.py
--rw-r--r--  2.0 unx     6881 b- defN 23-Jul-24 16:31 dwiqc/cli/process.py
+-rw-r--r--  2.0 unx     3620 b- defN 23-Jul-25 18:43 dwiqc/cli/install_containers.py
+-rw-r--r--  2.0 unx     6955 b- defN 23-Jul-25 18:43 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx     4237 b- defN 23-Jul-24 15:35 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      383 b- defN 23-Jul-13 14:56 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-Jul-05 14:23 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx     1029 b- defN 23-Jul-13 14:57 dwiqc/config/prequal.yaml
 -rw-r--r--  2.0 unx      634 b- defN 23-Jul-13 14:58 dwiqc/config/qsiprep.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-Jul-05 14:23 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-Jul-05 14:23 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx    15862 b- defN 23-Jul-18 18:16 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4656 b- defN 23-Jul-05 14:23 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     8449 b- defN 23-Jul-20 14:45 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-Jul-05 14:23 dwiqc/tasks/qsiprep_EQ.py
 -rw-r--r--  2.0 unx    13087 b- defN 23-Jul-24 16:31 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     6784 b- defN 23-Jul-24 16:32 dwiqc-0.8.0.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-Jul-24 16:32 dwiqc-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      460 b- defN 23-Jul-24 16:32 dwiqc-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-24 16:32 dwiqc-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-24 16:32 dwiqc-0.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1881 b- defN 23-Jul-24 16:32 dwiqc-0.8.0.dist-info/RECORD
-24 files, 81019 bytes uncompressed, 24657 bytes compressed:  69.6%
+-rwxr-xr-x  2.0 unx     7186 b- defN 23-Jul-25 18:50 dwiqc-0.9.0.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-Jul-25 18:50 dwiqc-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      460 b- defN 23-Jul-25 18:50 dwiqc-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-25 18:50 dwiqc-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-25 18:50 dwiqc-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1969 b- defN 23-Jul-25 18:50 dwiqc-0.9.0.dist-info/RECORD
+25 files, 85236 bytes uncompressed, 26311 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: dwiqc/cli/__init__.py
 Comment: 
 
 Filename: dwiqc/cli/get.py
 Comment: 
 
+Filename: dwiqc/cli/install_containers.py
+Comment: 
+
 Filename: dwiqc/cli/process.py
 Comment: 
 
 Filename: dwiqc/cli/tandem.py
 Comment: 
 
 Filename: dwiqc/config/__init__.py
@@ -48,26 +51,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.8.0.data/scripts/dwiQC.py
+Filename: dwiqc-0.9.0.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.8.0.dist-info/LICENSE
+Filename: dwiqc-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.8.0.dist-info/METADATA
+Filename: dwiqc-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.8.0.dist-info/WHEEL
+Filename: dwiqc-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.8.0.dist-info/top_level.txt
+Filename: dwiqc-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.8.0.dist-info/RECORD
+Filename: dwiqc-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/cli/__init__.py

```diff
@@ -1,3 +1,4 @@
 from . import get
 from . import process
 from . import tandem
+from . import install_containers
```

## dwiqc/cli/process.py

```diff
@@ -44,14 +44,15 @@
 
 
     # load data into pybids as layout
 
     layout = BIDSLayout(args.bids_dir)
 
     # grab the dwi and json files using pybids and os
+    # If diffusion files or fieldmap files don't exist, exit the program.
 
     try:
         dwi_file = os.path.basename(layout.get(subject=args.sub, extension='.nii.gz', suffix='dwi', run=args.run, return_type='filename').pop())
     except IndexError:
         logger.error("No diffusion data found. Double check bids directory to verify. Exiting.")
         sys.exit()
```

## Comparing `dwiqc-0.8.0.data/scripts/dwiQC.py` & `dwiqc-0.9.0.data/scripts/dwiQC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 #!python
 import sys
 import dwiqc
 import dwiqc.cli as cli
 import logging
 import argparse as ap
+import os
 import dwiqc.config as config
 
 
 logger = logging.getLogger(__name__)
-
+home_dir = os.path.expanduser("~")
 
 
 
 def main():
     parser = ap.ArgumentParser()
     parser.add_argument('-v', '--verbose', action='store_true',
         help='Enable verbose logging')
     parser.add_argument('-c', '--xnat-config', default=config.xnat_download(),
         help='dwiQC configuration file')
     parser.add_argument('--insecure', action='store_true',
         help='Disable SSL certificate verification')
     subparsers = parser.add_subparsers(help='sub-command help')
+
+    # install mode
+    parser_install = subparsers.add_parser('install-containers', help='install-containers -h')
+    parser_install.add_argument('--install-location', default=os.path.join(home_dir, '.config/dwiqc/containers/'),
+        help='Path to desired container installation location')
+    parser_install.set_defaults(func=cli.install_containers.do)
     
     # get mode
     parser_get = subparsers.add_parser('get', help='get -h')
     parser_get.add_argument('--label', required=True,
         help='XNAT MR Session name')
     parser_get.add_argument('--project',
         help='XNAT Project name')
```

## Comparing `dwiqc-0.8.0.dist-info/LICENSE` & `dwiqc-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.8.0.dist-info/RECORD` & `dwiqc-0.9.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=xE4sIpMv_Q09jQCkVZp6Lcy8lxGosaISpn9CIaIfTxA,247
+dwiqc/__version__.py,sha256=_Rndhv2k1gd53i2_ksgFijdNkUcpbwa4hKMI6iUsmRw,247
 dwiqc/browser/__init__.py,sha256=4lK-1-VH4l6ppP_5Ju6MeYIctiQmFQfGA7gclqh8euE,1352
-dwiqc/cli/__init__.py,sha256=1Y4dYEbkHH-jZ3cwbFnlb6TthH_K0t4xT_-IphRBu6k,61
+dwiqc/cli/__init__.py,sha256=QD5zUAU1PHaJdE14htZyZCCUOYQ1rHHMtT2v8lBF8QE,94
 dwiqc/cli/get.py,sha256=Eu7VTB6Od_BrOMpTqS5EvFZ-NDPRsbD3FZ0-Q72E2XE,6998
-dwiqc/cli/process.py,sha256=y7np2vLLxl-tuR8usrt84YYxyDqYPCKJJig-fybBRfI,6881
+dwiqc/cli/install_containers.py,sha256=ajk8WOjJ-Aijnr4kdm81embtYy0EviM1AKa-6ovZ5Fw,3620
+dwiqc/cli/process.py,sha256=sKhQZp-1-aiMZpqQaDoxAStilQYPgaxc_aBuQg4mX0w,6955
 dwiqc/cli/tandem.py,sha256=nn-EqvSLCy5X1Z66e1c9OZfff-ThiOOPQihl04WPXpY,4237
 dwiqc/config/__init__.py,sha256=X33iA2gj1lDc6fsIYPUcqvZUDV--IphhJY4JTNd-Yg0,383
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/config/prequal.yaml,sha256=tm6Jrb5aj7M2EqD87oXXG1VWryws44hn-uzRISeGNkM,1029
 dwiqc/config/qsiprep.yaml,sha256=QlGuIa2jAwNSWkv8CirhWVk50eRoIGVvieiUWGk9k-8,634
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
 dwiqc/tasks/prequal.py,sha256=BZNfFuBglguxeYqozr-_crVTXFxeXc4I5Oms_nkZ-SA,15862
 dwiqc/tasks/prequal_EQ.py,sha256=hvs6qjRNoJXuCzdvP-9BnaZc4xwvI9LHSgmueRobt1Q,4656
 dwiqc/tasks/qsiprep.py,sha256=7rtKi6NHPN3kl2imSk12h5gW1DX0qmWVsL1ie9jkfJ4,8449
 dwiqc/tasks/qsiprep_EQ.py,sha256=oj9kJ4hRBlq8mT4Mp-ogakoOTVFbfJ2yUxcwoXPN4j8,3872
 dwiqc/xnat/__init__.py,sha256=fjdic3dblSWMag4vOwCcgyHgD2pBcu7qICNrt7HBwVU,13087
-dwiqc-0.8.0.data/scripts/dwiQC.py,sha256=YQhcmOtSt3SgobN5s2EaRsl--aR0vQariL8JAxaA-xk,6784
-dwiqc-0.8.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.8.0.dist-info/METADATA,sha256=1N5Qe5X-yGxnpyTFwzW6DOO_p9J5N2rByIzqfBi2AR8,460
-dwiqc-0.8.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-dwiqc-0.8.0.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.8.0.dist-info/RECORD,,
+dwiqc-0.9.0.data/scripts/dwiQC.py,sha256=Nd-pDUAXJgqUOc7Olk6QD_u7zyxiO9gXzRzAWU1lY2c,7186
+dwiqc-0.9.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.9.0.dist-info/METADATA,sha256=YWJTtrRFa3t8-ofw5iCfpHmUCGI19eVWaPmzspssr2A,460
+dwiqc-0.9.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+dwiqc-0.9.0.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.9.0.dist-info/RECORD,,
```

