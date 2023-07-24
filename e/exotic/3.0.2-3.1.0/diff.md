# Comparing `tmp/exotic-3.0.2.zip` & `tmp/exotic-3.1.0.zip`

## zipinfo {}

```diff
@@ -1,118 +1,119 @@
-Zip file size: 6355426 bytes, number of entries: 116
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/exotic/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/.github/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/examples/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/exotic.egg-info/
--rw-r--r--  2.0 unx      465 b- defN 23-Jul-21 02:41 exotic-3.0.2/requirements.txt
--rw-r--r--  2.0 unx     1682 b- defN 23-Jul-21 02:42 exotic-3.0.2/setup.cfg
--rw-r--r--  2.0 unx    14575 b- defN 23-Jul-21 02:42 exotic-3.0.2/PKG-INFO
--rw-r--r--  2.0 unx     3359 b- defN 23-Jul-21 02:41 exotic-3.0.2/CODE_OF_CONDUCT.md
--rw-r--r--  2.0 unx     1556 b- defN 23-Jul-21 02:41 exotic-3.0.2/.gitignore
--rw-r--r--  2.0 unx      191 b- defN 23-Jul-21 02:41 exotic-3.0.2/CITATION.md
--rw-r--r--  2.0 unx      221 b- defN 23-Jul-21 02:41 exotic-3.0.2/MANIFEST.in
--rw-r--r--  2.0 unx      699 b- defN 23-Jul-21 02:41 exotic-3.0.2/AUTHORS.md
--rwxr-xr-x  2.0 unx      265 b- defN 23-Jul-21 02:41 exotic-3.0.2/run_exotic_windows.bat
--rw-r--r--  2.0 unx     2149 b- defN 23-Jul-21 02:41 exotic-3.0.2/LICENSE
--rwxr-xr-x  2.0 unx     5080 b- defN 23-Jul-21 02:41 exotic-3.0.2/run_exotic_linux.sh
--rw-r--r--  2.0 unx    13141 b- defN 23-Jul-21 02:41 exotic-3.0.2/README.md
--rw-r--r--  2.0 unx     5887 b- defN 23-Jul-21 02:41 exotic-3.0.2/inits.json
--rw-r--r--  2.0 unx     1890 b- defN 23-Jul-21 02:41 exotic-3.0.2/setup.py
--rw-r--r--  2.0 unx      387 b- defN 23-Jul-21 02:41 exotic-3.0.2/pyproject.toml
--rw-r--r--  2.0 unx      201 b- defN 23-Jul-21 02:41 exotic-3.0.2/CONTRIBUTING.md
--rwxr-xr-x  2.0 unx     4756 b- defN 23-Jul-21 02:41 exotic-3.0.2/run_exotic_mac.command
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/exotic/api/
--rw-r--r--  2.0 unx     9481 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/plots.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-21 02:42 exotic-3.0.2/exotic/version.py
--rw-r--r--  2.0 unx    80045 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/exotic_gui.py
--rw-r--r--  2.0 unx   117815 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/exotic.py
--rw-r--r--  2.0 unx     1239 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/animate.py
--rw-r--r--  2.0 unx     4752 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/plate_status.py
--rw-r--r--  2.0 unx    11472 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/utils.py
--rw-r--r--  2.0 unx     3027 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/__init__.py
--rw-r--r--  2.0 unx    27708 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/inputs.py
--rw-r--r--  2.0 unx    13768 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/output_files.py
--rw-r--r--  2.0 unx     5592 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/ew.py
--rw-r--r--  2.0 unx    15060 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/colab.py
--rw-r--r--  2.0 unx     4017 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/filters.py
--rw-r--r--  2.0 unx    18359 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/plotting.py
--rw-r--r--  2.0 unx     2916 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/versioning.py
--rw-r--r--  2.0 unx     5981 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/ld.py
--rw-r--r--  2.0 unx    27733 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/nested_linear_fitter.py
--rw-r--r--  2.0 unx     2322 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/__init__.py
--rw-r--r--  2.0 unx    48554 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/elca.py
--rw-r--r--  2.0 unx    17395 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/nea.py
--rw-r--r--  2.0 unx     9803 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/gael_ld.py
--rw-r--r--  2.0 unx     6591 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/plate_solution.py
--rw-r--r--  2.0 unx    14696 b- defN 23-Jul-21 02:41 exotic-3.0.2/exotic/api/output_aavso.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/.github/workflows/
--rw-r--r--  2.0 unx      260 b- defN 23-Jul-21 02:41 exotic-3.0.2/.github/dependabot.yml
--rw-r--r--  2.0 unx     1073 b- defN 23-Jul-21 02:41 exotic-3.0.2/.github/workflows/python-publish.yml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/docs/regions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/docs/Images/
--rw-r--r--  2.0 unx    16096 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/docs/regions/German/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/docs/regions/Brazilian_Portuguese/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/docs/regions/English/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-21 02:42 exotic-3.0.2/docs/regions/Spanish (Español)/
--rw-r--r--  2.0 unx   223208 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
--rw-r--r--  2.0 unx   155973 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
--rw-r--r--  2.0 unx   611693 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
--rw-r--r--  2.0 unx    10330 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/German/Beispiel_Output.txt
--rw-r--r--  2.0 unx   180681 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
--rw-r--r--  2.0 unx      119 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/German/translators.md
--rw-r--r--  2.0 unx   132016 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/German/Benutzung-von-GitHub.pdf
--rw-r--r--  2.0 unx    28054 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
--rw-r--r--  2.0 unx      545 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/Brazilian_Portuguese/README.md
--rw-r--r--  2.0 unx    11401 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
--rw-r--r--  2.0 unx    86803 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/Getting-Started-with-EXOTIC.pdf
--rw-r--r--  2.0 unx   725191 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/How-EXOTIC-Works.pdf
--rw-r--r--  2.0 unx     9236 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
--rw-r--r--  2.0 unx     5893 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
--rw-r--r--  2.0 unx   598255 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
--rw-r--r--  2.0 unx     6151 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
--rw-r--r--  2.0 unx     5902 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
--rw-r--r--  2.0 unx    27943 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
--rw-r--r--  2.0 unx    10067 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/example_output.txt
--rw-r--r--  2.0 unx     2673 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
--rw-r--r--  2.0 unx   243586 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/How_to_Use_GitHub.pdf
--rw-r--r--  2.0 unx   229468 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/English/Introduction-to-Exoplanets.pdf
--rw-r--r--  2.0 unx   112871 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
--rw-r--r--  2.0 unx      129 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/regions/Spanish (Español)/translators.md
--rw-r--r--  2.0 unx   197330 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/exotic_planetparams.png
--rw-r--r--  2.0 unx   340120 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/ExoplanetWatch.png
--rw-r--r--  2.0 unx   189180 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/posterior_sample.png
--rw-r--r--  2.0 unx    74050 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/exotic_running.png
--rw-r--r--  2.0 unx   187434 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/exotic_inputobs.png
--rw-r--r--  2.0 unx   265478 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/transitsimple.jpg
--rw-r--r--  2.0 unx    45485 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/exotic_initssaved.png
--rw-r--r--  2.0 unx    57777 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/exotic_inputplanetparams.png
--rw-r--r--  2.0 unx   309812 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/HAT-P-32bExample.png
--rw-r--r--  2.0 unx    56356 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/Background_Estimate.png
--rw-r--r--  2.0 unx   617967 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/Hot_pixel_mask.png
--rw-r--r--  2.0 unx    46133 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/exotic_inputobsinfo.png
--rw-r--r--  2.0 unx    82591 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/exotic_loading.png
--rw-r--r--  2.0 unx    46372 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/exotic_saveinits.png
--rw-r--r--  2.0 unx    79523 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/centroids.png
--rw-r--r--  2.0 unx    53508 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/exotic_redmode.png
--rw-r--r--  2.0 unx    65879 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/exotic_welcome.png
--rw-r--r--  2.0 unx    46727 b- defN 23-Jul-21 02:41 exotic-3.0.2/docs/Images/exotic_runmode.png
--rw-r--r--  2.0 unx    28376 b- defN 23-Jul-21 02:41 exotic-3.0.2/examples/tess.py
--rw-r--r--  2.0 unx     3296 b- defN 23-Jul-21 02:41 exotic-3.0.2/examples/lc_fitter_unit_test.py
--rw-r--r--  2.0 unx   597675 b- defN 23-Jul-21 02:41 exotic-3.0.2/examples/Multiple_Lightcurve_fit.ipynb
--rw-r--r--  2.0 unx     4597 b- defN 23-Jul-21 02:41 exotic-3.0.2/examples/sampledata.json
--rw-r--r--  2.0 unx   248480 b- defN 23-Jul-21 02:41 exotic-3.0.2/examples/Exoplanet_Watch_API.ipynb
--rw-r--r--  2.0 unx     2244 b- defN 23-Jul-21 02:41 exotic-3.0.2/examples/global_fitter_unit_test.py
--rwxr-xr-x  2.0 unx     4479 b- defN 23-Jul-21 02:41 exotic-3.0.2/examples/interactive_fitter.py
--rw-r--r--  2.0 unx    20643 b- defN 23-Jul-21 02:41 exotic-3.0.2/tests/test_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-21 02:41 exotic-3.0.2/tests/__init__.py
--rw-r--r--  2.0 unx    14575 b- defN 23-Jul-21 02:42 exotic-3.0.2/exotic.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-21 02:42 exotic-3.0.2/exotic.egg-info/not-zip-safe
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-21 02:42 exotic-3.0.2/exotic.egg-info/top_level.txt
--rw-r--r--  2.0 unx     3270 b- defN 23-Jul-21 02:42 exotic-3.0.2/exotic.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      483 b- defN 23-Jul-21 02:42 exotic-3.0.2/exotic.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-21 02:42 exotic-3.0.2/exotic.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-21 02:42 exotic-3.0.2/exotic.egg-info/entry_points.txt
-116 files, 7630400 bytes uncompressed, 6336790 bytes compressed:  17.0%
+Zip file size: 6361419 bytes, number of entries: 117
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/exotic/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/.github/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/examples/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/
+-rw-r--r--  2.0 unx      476 b- defN 23-Jul-24 23:33 exotic-3.1.0/requirements.txt
+-rw-r--r--  2.0 unx     1682 b- defN 23-Jul-24 23:34 exotic-3.1.0/setup.cfg
+-rw-r--r--  2.0 unx    14575 b- defN 23-Jul-24 23:34 exotic-3.1.0/PKG-INFO
+-rw-r--r--  2.0 unx     3359 b- defN 23-Jul-24 23:33 exotic-3.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--  2.0 unx     1556 b- defN 23-Jul-24 23:33 exotic-3.1.0/.gitignore
+-rw-r--r--  2.0 unx      191 b- defN 23-Jul-24 23:33 exotic-3.1.0/CITATION.md
+-rw-r--r--  2.0 unx      221 b- defN 23-Jul-24 23:33 exotic-3.1.0/MANIFEST.in
+-rw-r--r--  2.0 unx      699 b- defN 23-Jul-24 23:33 exotic-3.1.0/AUTHORS.md
+-rwxr-xr-x  2.0 unx      265 b- defN 23-Jul-24 23:33 exotic-3.1.0/run_exotic_windows.bat
+-rw-r--r--  2.0 unx     2149 b- defN 23-Jul-24 23:33 exotic-3.1.0/LICENSE
+-rwxr-xr-x  2.0 unx     5080 b- defN 23-Jul-24 23:33 exotic-3.1.0/run_exotic_linux.sh
+-rw-r--r--  2.0 unx    13141 b- defN 23-Jul-24 23:33 exotic-3.1.0/README.md
+-rw-r--r--  2.0 unx     5887 b- defN 23-Jul-24 23:33 exotic-3.1.0/inits.json
+-rw-r--r--  2.0 unx     1890 b- defN 23-Jul-24 23:33 exotic-3.1.0/setup.py
+-rw-r--r--  2.0 unx      362 b- defN 23-Jul-24 23:33 exotic-3.1.0/pyproject.toml
+-rw-r--r--  2.0 unx      201 b- defN 23-Jul-24 23:33 exotic-3.1.0/CONTRIBUTING.md
+-rwxr-xr-x  2.0 unx     4756 b- defN 23-Jul-24 23:33 exotic-3.1.0/run_exotic_mac.command
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/exotic/api/
+-rw-r--r--  2.0 unx     9481 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/plots.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic/version.py
+-rw-r--r--  2.0 unx    80045 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/exotic_gui.py
+-rw-r--r--  2.0 unx   117869 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/exotic.py
+-rw-r--r--  2.0 unx     1239 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/animate.py
+-rw-r--r--  2.0 unx     4752 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/plate_status.py
+-rw-r--r--  2.0 unx    11472 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/utils.py
+-rw-r--r--  2.0 unx     3027 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/__init__.py
+-rw-r--r--  2.0 unx    27708 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/inputs.py
+-rw-r--r--  2.0 unx    13768 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/output_files.py
+-rw-r--r--  2.0 unx     5592 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/ew.py
+-rw-r--r--  2.0 unx    15060 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/colab.py
+-rw-r--r--  2.0 unx     4017 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/filters.py
+-rw-r--r--  2.0 unx    18359 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/plotting.py
+-rw-r--r--  2.0 unx     2916 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/versioning.py
+-rw-r--r--  2.0 unx     5981 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/ld.py
+-rw-r--r--  2.0 unx    29599 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/nested_linear_fitter.py
+-rw-r--r--  2.0 unx     2322 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/__init__.py
+-rw-r--r--  2.0 unx    49191 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/elca.py
+-rw-r--r--  2.0 unx    17395 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/nea.py
+-rw-r--r--  2.0 unx     9803 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/gael_ld.py
+-rw-r--r--  2.0 unx     6591 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/plate_solution.py
+-rw-r--r--  2.0 unx    14763 b- defN 23-Jul-24 23:33 exotic-3.1.0/exotic/api/output_aavso.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/.github/workflows/
+-rw-r--r--  2.0 unx      260 b- defN 23-Jul-24 23:33 exotic-3.1.0/.github/dependabot.yml
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jul-24 23:33 exotic-3.1.0/.github/workflows/python-publish.yml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/regions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/Images/
+-rw-r--r--  2.0 unx    16096 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/regions/German/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/regions/Brazilian_Portuguese/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/regions/English/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-24 23:34 exotic-3.1.0/docs/regions/Spanish (Español)/
+-rw-r--r--  2.0 unx   223208 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
+-rw-r--r--  2.0 unx   155973 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
+-rw-r--r--  2.0 unx   611693 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
+-rw-r--r--  2.0 unx    10330 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/Beispiel_Output.txt
+-rw-r--r--  2.0 unx   180681 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
+-rw-r--r--  2.0 unx      119 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/translators.md
+-rw-r--r--  2.0 unx   132016 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/German/Benutzung-von-GitHub.pdf
+-rw-r--r--  2.0 unx    28054 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
+-rw-r--r--  2.0 unx      545 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/Brazilian_Portuguese/README.md
+-rw-r--r--  2.0 unx    11401 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
+-rw-r--r--  2.0 unx    86803 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf
+-rw-r--r--  2.0 unx   725191 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-EXOTIC-Works.pdf
+-rw-r--r--  2.0 unx     9236 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
+-rw-r--r--  2.0 unx     5893 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
+-rw-r--r--  2.0 unx   598255 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
+-rw-r--r--  2.0 unx     6151 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
+-rw-r--r--  2.0 unx     5902 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
+-rw-r--r--  2.0 unx    27943 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
+-rw-r--r--  2.0 unx    10067 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/example_output.txt
+-rw-r--r--  2.0 unx     2673 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
+-rw-r--r--  2.0 unx   243586 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/How_to_Use_GitHub.pdf
+-rw-r--r--  2.0 unx   229468 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/English/Introduction-to-Exoplanets.pdf
+-rw-r--r--  2.0 unx   112871 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
+-rw-r--r--  2.0 unx      129 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/regions/Spanish (Español)/translators.md
+-rw-r--r--  2.0 unx   197330 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_planetparams.png
+-rw-r--r--  2.0 unx   340120 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/ExoplanetWatch.png
+-rw-r--r--  2.0 unx   189180 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/posterior_sample.png
+-rw-r--r--  2.0 unx    74050 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_running.png
+-rw-r--r--  2.0 unx   187434 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_inputobs.png
+-rw-r--r--  2.0 unx   265478 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/transitsimple.jpg
+-rw-r--r--  2.0 unx    45485 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_initssaved.png
+-rw-r--r--  2.0 unx    57777 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_inputplanetparams.png
+-rw-r--r--  2.0 unx   309812 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/HAT-P-32bExample.png
+-rw-r--r--  2.0 unx    56356 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/Background_Estimate.png
+-rw-r--r--  2.0 unx   617967 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/Hot_pixel_mask.png
+-rw-r--r--  2.0 unx    46133 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_inputobsinfo.png
+-rw-r--r--  2.0 unx    82591 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_loading.png
+-rw-r--r--  2.0 unx    46372 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_saveinits.png
+-rw-r--r--  2.0 unx    79523 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/centroids.png
+-rw-r--r--  2.0 unx    53508 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_redmode.png
+-rw-r--r--  2.0 unx    65879 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_welcome.png
+-rw-r--r--  2.0 unx    46727 b- defN 23-Jul-24 23:33 exotic-3.1.0/docs/Images/exotic_runmode.png
+-rw-r--r--  2.0 unx    27673 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/tess.py
+-rw-r--r--  2.0 unx     3296 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/lc_fitter_unit_test.py
+-rw-r--r--  2.0 unx   597675 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/Multiple_Lightcurve_fit.ipynb
+-rw-r--r--  2.0 unx     4597 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/sampledata.json
+-rw-r--r--  2.0 unx   248480 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/Exoplanet_Watch_API.ipynb
+-rw-r--r--  2.0 unx     2244 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/global_fitter_unit_test.py
+-rw-r--r--  2.0 unx    22617 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/Multiple_Lightcurve_Fit_Detrended.ipynb
+-rwxr-xr-x  2.0 unx     4479 b- defN 23-Jul-24 23:33 exotic-3.1.0/examples/interactive_fitter.py
+-rw-r--r--  2.0 unx    20643 b- defN 23-Jul-24 23:33 exotic-3.1.0/tests/test_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-24 23:33 exotic-3.1.0/tests/__init__.py
+-rw-r--r--  2.0 unx    14575 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     3319 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      494 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-24 23:34 exotic-3.1.0/exotic.egg-info/entry_points.txt
+117 files, 7654984 bytes uncompressed, 6342585 bytes compressed:  17.1%
```

## zipnote {}

```diff
@@ -1,349 +1,352 @@
-Filename: exotic-3.0.2/
+Filename: exotic-3.1.0/
 Comment: 
 
-Filename: exotic-3.0.2/exotic/
+Filename: exotic-3.1.0/exotic/
 Comment: 
 
-Filename: exotic-3.0.2/.github/
+Filename: exotic-3.1.0/.github/
 Comment: 
 
-Filename: exotic-3.0.2/docs/
+Filename: exotic-3.1.0/docs/
 Comment: 
 
-Filename: exotic-3.0.2/examples/
+Filename: exotic-3.1.0/examples/
 Comment: 
 
-Filename: exotic-3.0.2/tests/
+Filename: exotic-3.1.0/tests/
 Comment: 
 
-Filename: exotic-3.0.2/exotic.egg-info/
+Filename: exotic-3.1.0/exotic.egg-info/
 Comment: 
 
-Filename: exotic-3.0.2/requirements.txt
+Filename: exotic-3.1.0/requirements.txt
 Comment: 
 
-Filename: exotic-3.0.2/setup.cfg
+Filename: exotic-3.1.0/setup.cfg
 Comment: 
 
-Filename: exotic-3.0.2/PKG-INFO
+Filename: exotic-3.1.0/PKG-INFO
 Comment: 
 
-Filename: exotic-3.0.2/CODE_OF_CONDUCT.md
+Filename: exotic-3.1.0/CODE_OF_CONDUCT.md
 Comment: 
 
-Filename: exotic-3.0.2/.gitignore
+Filename: exotic-3.1.0/.gitignore
 Comment: 
 
-Filename: exotic-3.0.2/CITATION.md
+Filename: exotic-3.1.0/CITATION.md
 Comment: 
 
-Filename: exotic-3.0.2/MANIFEST.in
+Filename: exotic-3.1.0/MANIFEST.in
 Comment: 
 
-Filename: exotic-3.0.2/AUTHORS.md
+Filename: exotic-3.1.0/AUTHORS.md
 Comment: 
 
-Filename: exotic-3.0.2/run_exotic_windows.bat
+Filename: exotic-3.1.0/run_exotic_windows.bat
 Comment: 
 
-Filename: exotic-3.0.2/LICENSE
+Filename: exotic-3.1.0/LICENSE
 Comment: 
 
-Filename: exotic-3.0.2/run_exotic_linux.sh
+Filename: exotic-3.1.0/run_exotic_linux.sh
 Comment: 
 
-Filename: exotic-3.0.2/README.md
+Filename: exotic-3.1.0/README.md
 Comment: 
 
-Filename: exotic-3.0.2/inits.json
+Filename: exotic-3.1.0/inits.json
 Comment: 
 
-Filename: exotic-3.0.2/setup.py
+Filename: exotic-3.1.0/setup.py
 Comment: 
 
-Filename: exotic-3.0.2/pyproject.toml
+Filename: exotic-3.1.0/pyproject.toml
 Comment: 
 
-Filename: exotic-3.0.2/CONTRIBUTING.md
+Filename: exotic-3.1.0/CONTRIBUTING.md
 Comment: 
 
-Filename: exotic-3.0.2/run_exotic_mac.command
+Filename: exotic-3.1.0/run_exotic_mac.command
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/
+Filename: exotic-3.1.0/exotic/api/
 Comment: 
 
-Filename: exotic-3.0.2/exotic/plots.py
+Filename: exotic-3.1.0/exotic/plots.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/version.py
+Filename: exotic-3.1.0/exotic/version.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/exotic_gui.py
+Filename: exotic-3.1.0/exotic/exotic_gui.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/exotic.py
+Filename: exotic-3.1.0/exotic/exotic.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/animate.py
+Filename: exotic-3.1.0/exotic/animate.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/plate_status.py
+Filename: exotic-3.1.0/exotic/plate_status.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/utils.py
+Filename: exotic-3.1.0/exotic/utils.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/__init__.py
+Filename: exotic-3.1.0/exotic/__init__.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/inputs.py
+Filename: exotic-3.1.0/exotic/inputs.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/output_files.py
+Filename: exotic-3.1.0/exotic/output_files.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/ew.py
+Filename: exotic-3.1.0/exotic/api/ew.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/colab.py
+Filename: exotic-3.1.0/exotic/api/colab.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/filters.py
+Filename: exotic-3.1.0/exotic/api/filters.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/plotting.py
+Filename: exotic-3.1.0/exotic/api/plotting.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/versioning.py
+Filename: exotic-3.1.0/exotic/api/versioning.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/ld.py
+Filename: exotic-3.1.0/exotic/api/ld.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/nested_linear_fitter.py
+Filename: exotic-3.1.0/exotic/api/nested_linear_fitter.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/__init__.py
+Filename: exotic-3.1.0/exotic/api/__init__.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/elca.py
+Filename: exotic-3.1.0/exotic/api/elca.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/nea.py
+Filename: exotic-3.1.0/exotic/api/nea.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/gael_ld.py
+Filename: exotic-3.1.0/exotic/api/gael_ld.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/plate_solution.py
+Filename: exotic-3.1.0/exotic/api/plate_solution.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic/api/output_aavso.py
+Filename: exotic-3.1.0/exotic/api/output_aavso.py
 Comment: 
 
-Filename: exotic-3.0.2/.github/workflows/
+Filename: exotic-3.1.0/.github/workflows/
 Comment: 
 
-Filename: exotic-3.0.2/.github/dependabot.yml
+Filename: exotic-3.1.0/.github/dependabot.yml
 Comment: 
 
-Filename: exotic-3.0.2/.github/workflows/python-publish.yml
+Filename: exotic-3.1.0/.github/workflows/python-publish.yml
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/
+Filename: exotic-3.1.0/docs/regions/
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/
+Filename: exotic-3.1.0/docs/Images/
 Comment: 
 
-Filename: exotic-3.0.2/docs/README.md
+Filename: exotic-3.1.0/docs/README.md
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/German/
+Filename: exotic-3.1.0/docs/regions/German/
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/Brazilian_Portuguese/
+Filename: exotic-3.1.0/docs/regions/Brazilian_Portuguese/
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/
+Filename: exotic-3.1.0/docs/regions/English/
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/Spanish (Espa#U00f1ol)/
+Filename: exotic-3.1.0/docs/regions/Spanish (Espa#U00f1ol)/
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
+Filename: exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
+Filename: exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
+Filename: exotic-3.1.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/German/Beispiel_Output.txt
+Filename: exotic-3.1.0/docs/regions/German/Beispiel_Output.txt
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
+Filename: exotic-3.1.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/German/translators.md
+Filename: exotic-3.1.0/docs/regions/German/translators.md
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/German/Benutzung-von-GitHub.pdf
+Filename: exotic-3.1.0/docs/regions/German/Benutzung-von-GitHub.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
+Filename: exotic-3.1.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/Brazilian_Portuguese/README.md
+Filename: exotic-3.1.0/docs/regions/Brazilian_Portuguese/README.md
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
+Filename: exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/Getting-Started-with-EXOTIC.pdf
+Filename: exotic-3.1.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/How-EXOTIC-Works.pdf
+Filename: exotic-3.1.0/docs/regions/English/How-EXOTIC-Works.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
+Filename: exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
+Filename: exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
+Filename: exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
+Filename: exotic-3.1.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
+Filename: exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
+Filename: exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/example_output.txt
+Filename: exotic-3.1.0/docs/regions/English/example_output.txt
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
+Filename: exotic-3.1.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/How_to_Use_GitHub.pdf
+Filename: exotic-3.1.0/docs/regions/English/How_to_Use_GitHub.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/English/Introduction-to-Exoplanets.pdf
+Filename: exotic-3.1.0/docs/regions/English/Introduction-to-Exoplanets.pdf
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/Spanish (Espa#U00f1ol)/Introducci#U00f3n a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
+Filename: exotic-3.1.0/docs/regions/Spanish (Espa#U00f1ol)/Introducci#U00f3n a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
 Comment: 
 
-Filename: exotic-3.0.2/docs/regions/Spanish (Espa#U00f1ol)/translators.md
+Filename: exotic-3.1.0/docs/regions/Spanish (Espa#U00f1ol)/translators.md
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/exotic_planetparams.png
+Filename: exotic-3.1.0/docs/Images/exotic_planetparams.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/ExoplanetWatch.png
+Filename: exotic-3.1.0/docs/Images/ExoplanetWatch.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/posterior_sample.png
+Filename: exotic-3.1.0/docs/Images/posterior_sample.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/exotic_running.png
+Filename: exotic-3.1.0/docs/Images/exotic_running.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/exotic_inputobs.png
+Filename: exotic-3.1.0/docs/Images/exotic_inputobs.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/transitsimple.jpg
+Filename: exotic-3.1.0/docs/Images/transitsimple.jpg
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/exotic_initssaved.png
+Filename: exotic-3.1.0/docs/Images/exotic_initssaved.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/exotic_inputplanetparams.png
+Filename: exotic-3.1.0/docs/Images/exotic_inputplanetparams.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/HAT-P-32bExample.png
+Filename: exotic-3.1.0/docs/Images/HAT-P-32bExample.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/Background_Estimate.png
+Filename: exotic-3.1.0/docs/Images/Background_Estimate.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/Hot_pixel_mask.png
+Filename: exotic-3.1.0/docs/Images/Hot_pixel_mask.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/exotic_inputobsinfo.png
+Filename: exotic-3.1.0/docs/Images/exotic_inputobsinfo.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/exotic_loading.png
+Filename: exotic-3.1.0/docs/Images/exotic_loading.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/exotic_saveinits.png
+Filename: exotic-3.1.0/docs/Images/exotic_saveinits.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/centroids.png
+Filename: exotic-3.1.0/docs/Images/centroids.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/exotic_redmode.png
+Filename: exotic-3.1.0/docs/Images/exotic_redmode.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/exotic_welcome.png
+Filename: exotic-3.1.0/docs/Images/exotic_welcome.png
 Comment: 
 
-Filename: exotic-3.0.2/docs/Images/exotic_runmode.png
+Filename: exotic-3.1.0/docs/Images/exotic_runmode.png
 Comment: 
 
-Filename: exotic-3.0.2/examples/tess.py
+Filename: exotic-3.1.0/examples/tess.py
 Comment: 
 
-Filename: exotic-3.0.2/examples/lc_fitter_unit_test.py
+Filename: exotic-3.1.0/examples/lc_fitter_unit_test.py
 Comment: 
 
-Filename: exotic-3.0.2/examples/Multiple_Lightcurve_fit.ipynb
+Filename: exotic-3.1.0/examples/Multiple_Lightcurve_fit.ipynb
 Comment: 
 
-Filename: exotic-3.0.2/examples/sampledata.json
+Filename: exotic-3.1.0/examples/sampledata.json
 Comment: 
 
-Filename: exotic-3.0.2/examples/Exoplanet_Watch_API.ipynb
+Filename: exotic-3.1.0/examples/Exoplanet_Watch_API.ipynb
 Comment: 
 
-Filename: exotic-3.0.2/examples/global_fitter_unit_test.py
+Filename: exotic-3.1.0/examples/global_fitter_unit_test.py
 Comment: 
 
-Filename: exotic-3.0.2/examples/interactive_fitter.py
+Filename: exotic-3.1.0/examples/Multiple_Lightcurve_Fit_Detrended.ipynb
 Comment: 
 
-Filename: exotic-3.0.2/tests/test_utils.py
+Filename: exotic-3.1.0/examples/interactive_fitter.py
 Comment: 
 
-Filename: exotic-3.0.2/tests/__init__.py
+Filename: exotic-3.1.0/tests/test_utils.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic.egg-info/PKG-INFO
+Filename: exotic-3.1.0/tests/__init__.py
 Comment: 
 
-Filename: exotic-3.0.2/exotic.egg-info/not-zip-safe
+Filename: exotic-3.1.0/exotic.egg-info/PKG-INFO
 Comment: 
 
-Filename: exotic-3.0.2/exotic.egg-info/top_level.txt
+Filename: exotic-3.1.0/exotic.egg-info/not-zip-safe
 Comment: 
 
-Filename: exotic-3.0.2/exotic.egg-info/SOURCES.txt
+Filename: exotic-3.1.0/exotic.egg-info/top_level.txt
 Comment: 
 
-Filename: exotic-3.0.2/exotic.egg-info/requires.txt
+Filename: exotic-3.1.0/exotic.egg-info/SOURCES.txt
 Comment: 
 
-Filename: exotic-3.0.2/exotic.egg-info/dependency_links.txt
+Filename: exotic-3.1.0/exotic.egg-info/requires.txt
 Comment: 
 
-Filename: exotic-3.0.2/exotic.egg-info/entry_points.txt
+Filename: exotic-3.1.0/exotic.egg-info/dependency_links.txt
+Comment: 
+
+Filename: exotic-3.1.0/exotic.egg-info/entry_points.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `exotic-3.0.2/setup.cfg` & `exotic-3.1.0/setup.cfg`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/PKG-INFO` & `exotic-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exotic
-Version: 3.0.2
+Version: 3.1.0
 Summary: EXOTIC: EXOplanet Transit Interpretation Code
 Home-page: https://github.com/rzellem/EXOTIC
 Download-URL: https://github.com/rzellem/EXOTIC/releases/latest
 Author: Exoplanet Watch at NASA JPL
 Author-email: exoplanetwatch@jpl.nasa.gov
 License: Proprietary -- Copyright (c) 2019-present, California Institute of Technology.
 Project-URL: Documentation, https://github.com/rzellem/EXOTIC/wiki
```

## Comparing `exotic-3.0.2/CODE_OF_CONDUCT.md` & `exotic-3.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/.gitignore` & `exotic-3.1.0/.gitignore`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/AUTHORS.md` & `exotic-3.1.0/AUTHORS.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/LICENSE` & `exotic-3.1.0/LICENSE`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/run_exotic_linux.sh` & `exotic-3.1.0/run_exotic_linux.sh`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/README.md` & `exotic-3.1.0/README.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/inits.json` & `exotic-3.1.0/inits.json`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/setup.py` & `exotic-3.1.0/setup.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/run_exotic_mac.command` & `exotic-3.1.0/run_exotic_mac.command`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/plots.py` & `exotic-3.1.0/exotic/plots.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/exotic_gui.py` & `exotic-3.1.0/exotic/exotic_gui.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/exotic.py` & `exotic-3.1.0/exotic/exotic.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 import logging
 from logging.handlers import TimedRotatingFileHandler
 from matplotlib.animation import FuncAnimation
 # Pyplot imports
 import matplotlib.pyplot as plt
 import numpy as np
 # photometry
-from photutils import CircularAperture
+from photutils.aperture import CircularAperture
 import pandas as pd
 import requests
 # scipy imports
 from scipy.optimize import least_squares
 from scipy.stats import mode
 from scipy.signal import savgol_filter
 from scipy.ndimage import binary_erosion
@@ -1171,16 +1171,16 @@
 
     if debug:
         minb = data[yv, xv][mask].min()
         maxb = data[yv, xv][mask].mean() + 3 * data[yv, xv][mask].std()
         nanmask = np.nan * np.zeros(mask.shape)
         nanmask[mask] = 1
         bgsky = data[yv, xv] * nanmask
-        cmode = mode(dat.flatten(), nan_policy='omit').mode[0]
-        amode = mode(bgsky.flatten(), nan_policy='omit').mode[0]
+        cmode = mode(dat.flatten(), nan_policy='omit', keepdims=True).mode[0]
+        amode = mode(bgsky.flatten(), nan_policy='omit', keepdims=True).mode[0]
 
         fig, ax = plt.subplots(2, 2, figsize=(9, 9))
         im = ax[0, 0].imshow(data[yv, xv], vmin=minb, vmax=maxb, cmap='inferno')
         ax[0, 0].set_title("Original Data")
         from mpl_toolkits.axes_grid1 import make_axes_locatable
         divider = make_axes_locatable(ax[0, 0])
         cax = divider.append_axes('right', size='5%', pad=0.05)
@@ -1197,15 +1197,15 @@
         ax[1, 1].imshow(dat, vmin=minb, vmax=maxb, cmap='inferno')
         ax[1, 1].set_title("Clipped Sky Background")
 
         ax[0, 1].imshow(bgsky, vmin=minb, vmax=maxb, cmap='inferno')
         ax[0, 1].set_title("Sky Annulus")
         plt.tight_layout()
         plt.show()
-    return mode(dat.flatten(), nan_policy='omit').mode[0], np.nanstd(dat.flatten()), np.sum(mask)
+    return mode(dat.flatten(), nan_policy='omit', keepdims=True).mode[0], np.nanstd(dat.flatten()), np.sum(mask)
 
 
 def jd_bjd(non_bjd, p_dict, info_dict):
     try:
         goodTimes = JDUTC_to_BJDTDB(non_bjd, ra=p_dict['ra'], dec=p_dict['dec'], lat=info_dict['lat'],
                                     longi=info_dict['long'], alt=info_dict['elev'])[0]
     except:
```

## Comparing `exotic-3.0.2/exotic/animate.py` & `exotic-3.1.0/exotic/animate.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/plate_status.py` & `exotic-3.1.0/exotic/plate_status.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/utils.py` & `exotic-3.1.0/exotic/utils.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/__init__.py` & `exotic-3.1.0/exotic/__init__.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/inputs.py` & `exotic-3.1.0/exotic/inputs.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/output_files.py` & `exotic-3.1.0/exotic/output_files.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/api/ew.py` & `exotic-3.1.0/exotic/api/ew.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/api/colab.py` & `exotic-3.1.0/exotic/api/colab.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/api/filters.py` & `exotic-3.1.0/exotic/api/filters.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/api/plotting.py` & `exotic-3.1.0/exotic/api/plotting.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/api/versioning.py` & `exotic-3.1.0/exotic/api/versioning.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/api/ld.py` & `exotic-3.1.0/exotic/api/ld.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/api/nested_linear_fitter.py` & `exotic-3.1.0/exotic/api/nested_linear_fitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                 self.results['posterior']['errlo'][i],
                 self.results['posterior']['errup'][i]]
 
         # final model
         self.model = self.epochs * self.parameters['m'] + self.parameters['b']
         self.residuals = self.data - self.model
 
-    def plot_oc(self, savefile=None, ylim='none', show_2sigma=False):
+    def plot_oc(self, savefile=None, ylim='none', show_2sigma=False, prior_name="Prior"):
         """ Plot the data in the form of residuals vs. time
 
         Parameters
         ----------
         savefile : str, optional
             Save the figure to a file.
         ylim : str, optional
@@ -189,25 +189,25 @@
             # plot an invisible line so the 2nd axes are happy
             ax2.plot(epochs, (model-prior)*24*60, ls='--', color='r', alpha=0)
 
             # why is this so small!?!?!? consistent to within machine precision?
             #ax.plot(epochs, (model-prior)*24*60, ls='--', color='r')
 
             if show_2sigma:
-                ax.fill_between(epochs, np.percentile(diff_p,2,axis=0)*24*60, np.percentile(diff_p,98,axis=0)*24*60, alpha=0.1, color='r', label=r'Prior ($\pm$ 2$\sigma$)')
+                ax.fill_between(epochs, np.percentile(diff_p,2,axis=0)*24*60, np.percentile(diff_p,98,axis=0)*24*60, alpha=0.1, color='r', label=rf'{prior_name} ($\pm$ 2$\sigma$)')
             else:
                 # show ~1 sigma
-                ax.fill_between(epochs, np.percentile(diff_p,36,axis=0)*24*60, np.percentile(diff_p,64,axis=0)*24*60, alpha=0.1, color='r', label=r'Prior ($\pm$ 1$\sigma$)')
+                ax.fill_between(epochs, np.percentile(diff_p,36,axis=0)*24*60, np.percentile(diff_p,64,axis=0)*24*60, alpha=0.1, color='r', label=rf'{prior_name} ($\pm$ 1$\sigma$)')
 
             if ylim == 'prior':
                 ax.set_ylim([ min(np.percentile(diff_p,1,axis=0)*24*60),
                             max(np.percentile(diff_p,99,axis=0)*24*60)])
             elif ylim == 'average':
                 ax.set_ylim([ 0.5*(min(np.percentile(diff,1,axis=0)*24*60) + min(np.percentile(diff_p,1,axis=0)*24*60)),
-                            0.5*(max(np.percentile(diff,99,axis=0)*24*60) + max(np.percentile(diff_p,99,axis=0)*24*60))])
+                              0.5*(max(np.percentile(diff,99,axis=0)*24*60) + max(np.percentile(diff_p,99,axis=0)*24*60))])
 
         ax.axhline(0,color='black',alpha=0.5,ls='--',
                    label="Period: {:.7f}+-{:.7f} days\nT_mid: {:.7f}+-{:.7f} BJD".format(self.parameters['m'], self.errors['m'], self.parameters['b'], self.errors['b']))
 
         # TODO sig figs
         #lclabel2 = r"$T_{mid}$ = %s $\pm$ %s BJD$_{TDB}$" %(
         #    str(round_to_2(self.parameters['tmid'], self.errors.get('tmid',0))),
@@ -277,32 +277,34 @@
             },
             hist_kwargs={
                 'color':'black',
             }
         )
         return fig
 
-    def plot_periodogram(self):
+    def plot_periodogram(self, minper=0, maxper=0, maxper2=50):
         """ Search the residuals for periodic signals. """
 
         ########################################
         # create basis vectors for Tn = T0 + n*P
         basis = np.ones((2, len(self.epochs)))
         basis[1] = self.epochs
         res_linear = sm.WLS(self.data, basis.T, weights=1.0/self.dataerr**2).fit()
         coeffs_linear = res_linear.params #retrieve the slope and intercept
         y_bestfit_linear = np.dot(basis.T, coeffs_linear) # reconstruct signal
         residuals = self.data - y_bestfit_linear
         ########################################
 
-
         # compute a period range based on nyquist frequency
         si = np.argsort(self.epochs)
-        minper = max(2,2 * np.diff(self.epochs[si]).min())
-        maxper = (np.max(self.epochs) - np.min(self.epochs))*3.
+
+        if minper == 0:
+            minper = max(3,2 * np.diff(self.epochs[si]).min())
+        if maxper == 0:
+            maxper = (np.max(self.epochs) - np.min(self.epochs))*3.
 
         # recompute on new grid
         ls = LombScargle(self.epochs, residuals, dy=self.dataerr)
         freq,power = ls.autopower(maximum_frequency=1./minper, minimum_frequency=1./maxper, nyquist_factor=2)
 
         # Phase fold data at max peak
         mi = np.argmax(power)
@@ -329,19 +331,20 @@
         y_bestfit_linear_first_order = np.dot(basis[:2].T, coeffs_first_order[:2])
         residuals_linear = self.data - y_bestfit_linear_first_order
         ########################################
 
 
         ########################################
         # subtract first order solution from data and recompute periodogram
-        maxper = 50 # constrain second order solution to be less than 50 days
+        maxper = maxper2
 
         # recompute on new grid
         ls2 = LombScargle(self.epochs, residuals_linear, dy=self.dataerr)
-        freq2,power2 = ls.autopower(maximum_frequency=1./(1.01*per), minimum_frequency=1./maxper, nyquist_factor=2)
+        #freq2,power2 = ls.autopower(maximum_frequency=1./(1.01*per), minimum_frequency=1./maxper, nyquist_factor=2)
+        freq2,power2 = ls.autopower(maximum_frequency=1./(1+minper), minimum_frequency=1./maxper, nyquist_factor=2)
 
         # find max period
         mi2 = np.argmax(power2)
         per2 = 1./freq2[mi2]
 
         # create basis vectors for second order solution
         basis = np.ones((6, len(self.epochs)))
@@ -353,55 +356,77 @@
 
         # perform the weighted least squares regression
         res_second_order = sm.WLS(self.data, basis.T, weights=1.0/self.dataerr**2).fit()
         coeffs_second_order = res_second_order.params
         y_bestfit_second_order = np.dot(basis.T, coeffs_second_order) # reconstruct signal
         ########################################
 
+        # find the best bic
+        bics = [res_linear.bic, res_first_order.bic, res_second_order.bic]
+        best_bic = np.argmin(bics)
 
         ########################################
         # create plot
         fig, ax = plt.subplots(4, figsize=(10,14))
 
         # periodogram plot for residuals
         ax[0].semilogx(self.periods,self.power,'k-',label='Data', zorder=5)
         ax[0].set_xlabel("Period [epoch]",fontsize=14)
         ax[0].set_ylabel('Power',fontsize=14)
-        ax[0].axvline(per,color='red',label=f'Period: {per:.2f}',alpha=0.75, zorder=10)
-        ax[0].axvline(per2,color='cyan', alpha=0.5, label=f'Period: {per2:.2f}', zorder=10)
-        ax[0].set_title("Lomb-Scargle Periodogram")
-        ax[0].set_ylim([0,0.5*(self.power.max()+np.percentile(self.power,99))])
-        ax[0].set_xlim([minper,maxper])
+        ax[0].axvline(per,color='red',label=f'Period: {per:.2f} epochs',alpha=0.75, zorder=10)
+        # find power at closest period
+        idx = np.argmin(np.abs(self.periods-per))
+        per_power1 = self.power[idx]
+
+        # find power at closest period
+        idx = np.argmin(np.abs(self.periods-per2))
+        per_power2 = self.power[idx]
+
+        ax[0].set_title("Lomb-Scargle Periodogram", fontsize=18)
+        ax[0].set_xlim([minper, (np.max(self.epochs) - np.min(self.epochs))*3.])
 
         # plot false alarm probability on lomb-scargle periodogram
-        fp = ls.false_alarm_probability(power.max(), method='bootstrap')
-        fp_levels = ls.false_alarm_level([0.01, 0.05, 0.1], method='bootstrap')
+        fp = ls.false_alarm_probability(power.max(), method='davies')
+        fp_levels = ls.false_alarm_level([0.01, 0.05, 0.1], method='davies')
+
+        # set upper y-limit on plot
+        ax[0].set_ylim([0, self.power.max()])
 
         # plot as horizontal line
-        ax[0].axhline(fp_levels[0], color='red', ls='--', label='99% FAP')
+        ax[0].axhline(fp_levels[0], color='red', ls='--', label=f'99% FAP (Power = {fp_levels[0]:.1f})')
 
         # plot lomb-scargle for detrended data
-        ax[0].semilogx(1./freq2,power2*0.99,'g-',alpha=0.5,label='Detrended Data', zorder=7)
+        ax[0].semilogx(1./freq2,power2*0.99,'g-',alpha=0.5,label='Data - Fourier Fit 1', zorder=7)
 
         # plot false alarm probability on lomb-scargle periodogram
-        fp = ls2.false_alarm_probability(power2.max(), method='bootstrap')
-        fp_levels = ls2.false_alarm_level([0.01, 0.05, 0.1], method='bootstrap')
+        fp = ls2.false_alarm_probability(power2.max(), method='davies')
+        fp_levels2 = ls2.false_alarm_level([0.01, 0.05, 0.1], method='davies')
+
+        # best period + false alarm for second order solution
+        ax[0].axvline(per2,color='cyan', alpha=0.5, label=f'Period: {per2:.2f} epochs', zorder=10)
+        ax[0].axhline(fp_levels2[0], color='cyan', ls='--', label=f'99% FAP (Power = {fp_levels2[0]:.1f})')
 
         # add horizontal dotted line at zero
-        ax[1].axhline(0, color='black', ls='--', label=f"Linear Fit (BIC: {res_linear.bic:.2f})")
+        linear_label = f"Linear Fit (BIC: {res_linear.bic:.2f})"
+        if best_bic == 0:
+            linear_label += " best"
+        ax[1].axhline(0, color='black', ls='--', label=linear_label)
 
         # super sample fourier solution for first order
         xnew = np.linspace(self.epochs.min(), self.epochs.max(), 1000)
         basis_new = np.ones((2, len(xnew)))
         basis_new[0] = np.sin(2*np.pi*xnew/per)
         basis_new[1] = np.cos(2*np.pi*xnew/per)
         y_bestfit_new = np.dot(basis_new.T, coeffs_first_order[2:]) # reconstruct signal
 
         # plot first order fourier solution
-        ax[1].plot(xnew, y_bestfit_new*24*60, 'r-', label=f'Fourier Fit 1st (BIC: {res_first_order.bic:.2f})', alpha=0.75)
+        fourier1_label = f'Fourier Fit 1st (BIC: {res_first_order.bic:.2f})'
+        if per_power1 < fp_levels[0]:
+            fourier1_label += " below 99% FAP"
+        ax[1].plot(xnew, y_bestfit_new*24*60, 'r-', label=fourier1_label, alpha=0.75)
 
         # set up ax labels
         ax[1].set_xlabel(f"Epochs",fontsize=14)
         ax[1].set_ylabel("O-C [min]",fontsize=14)
         ax[1].grid(True,ls='--')
         depoch = self.epochs.max() - self.epochs.min()
         ax[1].set_xlim([self.epochs.min()-depoch*0.01, self.epochs.max()+depoch*0.01])
@@ -418,15 +443,18 @@
         basis_new[0] = np.sin(2*np.pi*xnew/per)
         basis_new[1] = np.cos(2*np.pi*xnew/per)
         basis_new[2] = np.sin(4*np.pi*xnew/per2)
         basis_new[3] = np.cos(4*np.pi*xnew/per2)
         y_bestfit_new2 = np.dot(basis_new.T, coeffs_second_order[2:]) # reconstruct signal
 
         # plot first order fourier solution
-        ax[1].plot(xnew, y_bestfit_new2*24*60, 'c-', label=f'Fourier Fit 2nd (BIC: {res_second_order.bic:.2f})', alpha=0.75)
+        fourier2_label = f'Fourier Fit 2nd (BIC: {res_second_order.bic:.2f})'
+        if per_power2 < fp_levels2[0]: # should be fp_levels2?
+            fourier2_label += " below 99% FAP"
+        ax[1].plot(xnew, y_bestfit_new2*24*60, 'c-', label=fourier2_label, alpha=0.75)
 
         # set up ax labels
         ax[1].set_xlabel(f"Epochs",fontsize=14)
         ax[1].set_ylabel("O-C [min]",fontsize=14)
         ax[1].grid(True,ls='--')
         ax[1].legend(loc='best')
         ax[0].legend(loc='best')
@@ -538,28 +566,40 @@
 
         ax[3].legend(loc='best')
 
         return fig,ax
 
 def main():
     Tc = np.array([ # measured mid-transit times
-    2456588.69897499, 2456593.73645465, 2456646.65419785,
-       2456923.85589088, 2456971.73409754, 2458042.70521614,
-       2458047.75761158, 2458095.62091434, 2458100.66454441,
-       2453912.51471333, 2454461.86099   , 2455215.32701,
-       2455530.3197    , 2456543.33866   , 2459854.549103  
-    ])
+        2459150.837905, 2459524.851045,
+        2459546.613126, 2459565.643663, 2459584.690470, 2459584.686476,
+        2459909.739104, 2459957.337739, 2459169.880602, 2458416.424861,
+        2458428.664794, 2459145.400124, 2458430.025044, 2459164.440695,
+        2458415.064846, 2458435.465269, 2458412.344658, 2459150.840070,
+        2459160.360691, 2458431.384897, 2459146.760284, 2459154.920516,
+        2458417.784945, 2459161.720466, 2459167.160761, 2458427.304939,
+        2458413.705181, 2459163.080605, 2459153.560229, 2459168.520861,
+        2458425.945068, 2459148.120269, 2458434.105274, 2458432.745423,
+        2459152.200558, 2459165.800918, 2459159.000645, 2459149.480289,
+        2455870.450027, 2456663.347570, 2457420.884390, 2457658.888900])
 
     Tc_error = np.array([
-    0.00237294, 0.00290445, 0.00647494, 0.00445833, 0.00477952,
-       0.00310127, 0.00209248, 0.00099052, 0.00563974, 0.00054,
-       0.00024   , 0.00015   , 0.00016   , 0.00028   , 0.000382 
-    ])
+        0.001674, 0.000715,
+        0.000758, 0.001560, 0.000371, 0.001651,
+        0.000955, 0.000176, 0.000154, 0.000357,
+        0.000381, 0.000141, 0.000362, 0.000149,
+        0.000336, 0.000368, 0.000379, 0.000153,
+        0.000153, 0.000349, 0.000149, 0.000146,
+        0.000385, 0.000146, 0.000153, 0.000360,
+        0.000356, 0.000147, 0.000147, 0.000146,
+        0.000363, 0.000142, 0.000357, 0.000368,
+        0.000160, 0.000160, 0.000151, 0.000160,
+        0.000140, 0.000120, 0.000800, 0.000140 ])
 
-    P = 2.5199412024  # orbital period for your target
+    P = 1.360029  # orbital period for your target
 
     Tc_norm = Tc - Tc.min()  #normalize the data to the first observation
     #print(Tc_norm)
     orbit = np.rint(Tc_norm / P)  #number of orbits since first observation (rounded to nearest integer)
     #print(orbit)
 
     #make a n x 2 matrix with 1's in the first column and values of orbit in the second
@@ -594,19 +634,14 @@
 
     # used to plot red overlay in O-C figure
     prior = {
         'm':[slope, slope_std_dev],         # value from WLS (replace with literature value)
         'b':[intercept, intercept_std_dev]  # value from WLS (replace with literature value)
     }
 
-    prior = {
-        'm':[2.5199412024020322, 2.59214970054424e-06],
-        'b':[2459854.54339036, 0.0024412]
-    }
-
     lf = linear_fitter( Tc, Tc_error, bounds, prior=prior )
 
     lf.plot_triangle()
     plt.subplots_adjust(top=0.9,hspace=0.2,wspace=0.2)
     plt.savefig("posterior.png")
     plt.close()
     print("image saved to: posterior.png")
```

## Comparing `exotic-3.0.2/exotic/api/__init__.py` & `exotic-3.1.0/exotic/api/__init__.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/api/elca.py` & `exotic-3.1.0/exotic/api/elca.py`

 * *Files 7% similar despite different names*

```diff
@@ -715,16 +715,24 @@
             detrend = self.lc_data[n]['flux']/(model*airmass)
             self.lc_data[n]['priors']['a1'] = np.mean(detrend)
             self.lc_data[n]['residuals'] = self.lc_data[n]['flux'] - model*airmass*self.lc_data[n]['priors']['a1']
             self.lc_data[n]['detrend'] = self.lc_data[n]['flux']/(airmass*self.lc_data[n]['priors']['a1'])
             # phase
             self.lc_data[n]['phase'] = get_phase(self.lc_data[n]['time'], self.lc_data[n]['priors']['per'], self.lc_data[n]['priors']['tmid'])
 
+            # upscale model for plotting
+            self.lc_data[n]['time_upsample'] = np.linspace(min(self.lc_data[n]['time']), max(self.lc_data[n]['time']), 1000)
+            self.lc_data[n]['transit_upsample'] = transit(self.lc_data[n]['time_upsample'], self.lc_data[n]['priors'])
+
     def plot_bestfits(self):
         nrows = len(self.lc_data)//4+1
+        # make sure there isn't an extra row
+        if len(self.lc_data)%4 == 0:
+            nrows -= 1
+
         fig,ax = plt.subplots(nrows, 4, figsize=(5+5*nrows, 5*nrows))
 
         # turn off all axes
         for i in range(nrows*4):
             ri = int(i/4)
             ci = i%4
             if ax.ndim == 1:
@@ -746,39 +754,40 @@
             model = transit(self.lc_data[i]['time'], self.lc_data[i]['priors'])
             airmass = np.exp(self.lc_data[i]['airmass']*self.lc_data[i]['priors']['a2'])
             detrend = self.lc_data[i]['flux']/(model*airmass)
 
             if ax.ndim == 1:
                 ax[i].axis('on')
                 ax[i].errorbar(self.lc_data[i]['time'], self.lc_data[i]['flux']/airmass/detrend.mean(), yerr=self.lc_data[i]['ferr']/airmass/detrend.mean(), 
-                                ls='none', marker=nmarker, color=ncolor, alpha=0.5)
-                ax[i].plot(self.lc_data[i]['time'], model, 'r-', zorder=2)
+                                ls='none', marker=nmarker, color=ncolor, alpha=0.5, zorder=1)
+                
+                ax[i].plot(self.lc_data[i]['time_upsample'], self.lc_data[i]['transit_upsample'], 'r-', zorder=2)
                 ax[i].set_xlabel("Time [BJD]", fontsize=14)
                 ax[i].set_ylabel("Relative Flux", fontsize=14)
                 ax[i].set_title(f"{self.lc_data[i].get('name','')}", fontsize=16)
             else:
                 ax[ri,ci].axis('on')
                 ax[ri,ci].errorbar(self.lc_data[i]['time'], self.lc_data[i]['flux']/airmass/detrend.mean(), yerr=self.lc_data[i]['ferr']/airmass/detrend.mean(), 
-                                   ls='none', marker=nmarker, color=ncolor, alpha=0.5)
-                ax[ri,ci].plot(self.lc_data[i]['time'], model, 'r-', zorder=2)
+                                   ls='none', marker=nmarker, color=ncolor, alpha=0.5, zorder=1)
+                ax[ri,ci].plot(self.lc_data[i]['time_upsample'], self.lc_data[i]['transit_upsample'], 'r-', zorder=2)
                 ax[ri,ci].set_xlabel("Time[BJD]", fontsize=14)
                 ax[ri,ci].set_ylabel("Relative Flux", fontsize=14)
                 ax[ri,ci].set_title(f"{self.lc_data[i].get('name','')}", fontsize=16)
 
         plt.tight_layout()
         return fig
 
-    def plot_bestfit(self, title="", bin_dt=30./(60*24), alpha=0.05, phase_limits='median'):
+    def plot_bestfit(self, title="", bin_dt=30./(60*24), alpha=0.05, ylim_sigma=5, phase_limits='median', show_legend=True):
         f = plt.figure(figsize=(15,12))
         f.subplots_adjust(top=0.92,bottom=0.09,left=0.1,right=0.98, hspace=0)
         ax_lc = plt.subplot2grid((4,5), (0,0), colspan=5,rowspan=3)
         ax_res = plt.subplot2grid((4,5), (3,0), colspan=5, rowspan=1)
         axs = [ax_lc, ax_res]
 
-        axs[0].set_title(title)
+        axs[0].set_title(title, fontsize=18)
         axs[0].set_ylabel("Relative Flux", fontsize=14)
         axs[0].grid(True,ls='--')
 
         try:
             rprs2 = self.parameters['rprs']**2
             rprs2err = 2*self.parameters['rprs']*self.errors['rprs']
         except:
@@ -863,17 +872,18 @@
         self.time_upsample = np.linspace(minp*self.parameters['per']+self.parameters['tmid'], 
                                          maxp*self.parameters['per']+self.parameters['tmid'], 10000)
         self.transit_upsample = transit(self.time_upsample, self.lc_data[0]['priors'])
         self.phase_upsample = get_phase(self.time_upsample, self.parameters['per'], self.parameters['tmid'])
         sii = np.argsort(self.phase_upsample)
         axs[0].plot(self.phase_upsample[sii], self.transit_upsample[sii], 'r-', zorder=3, label=lclabel, lw=3)
 
+        # set up axes limits
         axs[0].set_xlim([min(self.phase_upsample), max(self.phase_upsample)])
         axs[0].set_xlabel("Phase ", fontsize=14)
-        axs[0].set_ylim([1-self.parameters['rprs']**2-5*min_std, 1+5*min_std])
+        axs[0].set_ylim([1-self.parameters['rprs']**2-ylim_sigma*min_std, 1+ylim_sigma*min_std])
         axs[1].set_xlim([min(self.phase_upsample), max(self.phase_upsample)])
         axs[1].set_xlabel("Phase", fontsize=14)
         axs[1].set_ylim([-5*min_std*1e2, 5*min_std*1e2])
 
         # compute average min and max for all the data
         mins = []; maxs = []
         for n in range(len(self.lc_data)):
@@ -898,17 +908,20 @@
             axs[0].set_xlim([phase_limits[0], phase_limits[1]])
             axs[1].set_xlim([phase_limits[0], phase_limits[1]])
         else:
             axs[0].set_xlim([min(self.phase_upsample), max(self.phase_upsample)])
             axs[1].set_xlim([min(self.phase_upsample), max(self.phase_upsample)])
 
         axs[0].get_xaxis().set_visible(False)
-        axs[0].legend(loc='best',ncol=len(self.lc_data)//7+1)
         axs[1].set_ylabel("Residuals [%]", fontsize=14)
         axs[1].grid(True,ls='--',axis='y')
+    
+        if show_legend:
+            axs[0].legend(loc='best',ncol=len(self.lc_data)//7+1)
+    
         return f,axs
 
     def plot_stack(self, title="", bin_dt=30./(60*24), dy=0.02):
         f, ax = plt.subplots(1,figsize=(9,12))
         
         ax.set_title(title)
         ax.set_ylabel("Relative Flux", fontsize=14)
```

## Comparing `exotic-3.0.2/exotic/api/nea.py` & `exotic-3.1.0/exotic/api/nea.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/api/gael_ld.py` & `exotic-3.1.0/exotic/api/gael_ld.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/api/plate_solution.py` & `exotic-3.1.0/exotic/api/plate_solution.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic/api/output_aavso.py` & `exotic-3.1.0/exotic/api/output_aavso.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,14 @@
                     f",u0={round_to_2(ld0)}"
                     f",u1={round_to_2(ld1)}"
                     f",u2={round_to_2(ld2)}"
                     f",u3={round_to_2(ld3)}\n"
                     f"#PRIORS-XC={dumps(priors_dict)}\n"  # code yields
                     f"#RESULTS=Tc={round_to_2(self.fit.parameters['tmid'], self.fit.errors['tmid'])} +/- {round_to_2(self.fit.errors['tmid'])}"
                     f",Rp/R*={round_to_2(self.fit.parameters['rprs'], self.fit.errors['rprs'])} +/- {round_to_2(self.fit.errors['rprs'])}"
-                    f",a/R*={round_to_2(self.fit.parameters['ars'], self.fit.errors['ars'])} +/- {round_to_2(self.fit.errors['ars'])}"
                     f",Am1=0"
                     f",Am2=0\n"
                     f"#RESULTS-XC={dumps(results_dict)}\n")  # code yields
 
             f.write(
                 "# EXOTIC is developed by Exoplanet Watch (exoplanets.nasa.gov/exoplanet-watch/), a citizen science "
                 "project managed by NASA's Jet Propulsion Laboratory on behalf of NASA's Universe of Learning. "
@@ -167,15 +166,14 @@
                         f",u0={round_to_2(ld0)}"
                         f",u1={round_to_2(ld1)}"
                         f",u2={round_to_2(ld2)}"
                         f",u3={round_to_2(ld3)}\n"
                         f"#PRIORS-XC={dumps(priors_dict)}\n"  # code yields
                         f"#RESULTS=Tc={round_to_2(self.fit.parameters['tmid'], self.fit.errors['tmid'])} +/- {round_to_2(self.fit.errors['tmid'])}"
                         f",Rp/R*={round_to_2(self.fit.parameters['rprs'], self.fit.errors['rprs'])} +/- {round_to_2(self.fit.errors['rprs'])}"
-                        f",a/R*={round_to_2(self.fit.parameters['ars'], self.fit.errors['ars'])} +/- {round_to_2(self.fit.errors['ars'])}"
                         f",Am1=0"
                         f",Am2=0\n"
                         f"#RESULTS-XC={dumps(results_dict)}\n")  # code yields
 
                 f.write(
                     "# EXOTIC is developed by Exoplanet Watch (exoplanets.nasa.gov/exoplanet-watch/), a citizen science "
                     "project managed by NASA's Jet Propulsion Laboratory on behalf of NASA's Universe of Learning. "
@@ -245,18 +243,14 @@
             'uncertainty': str(round_to_2(fit.errors['tmid'])),
             'units': "BJD_TDB"
         },
         'Rp/R*': {
             'value': str(round_to_2(fit.parameters['rprs'], fit.errors['rprs'])),
             'uncertainty': str(round_to_2(fit.errors['rprs']))
         },
-        'a/R*': {
-            'value': str(round_to_2(fit.parameters['ars'], fit.errors['ars'])),
-            'uncertainty': str(round_to_2(fit.errors['ars'])),
-        },
         'Am1': {
             'value': 0,
             'uncertainty': None
         },
         'Am2': {
             'value': 0,
             'uncertainty': None
@@ -264,8 +258,23 @@
         'Duration': {
             'value': str(round_to_2(mean(durs))),
             'uncertainty': str(round_to_2(std(durs))),
             'units': "days"
         }
     }
 
+    # try to add a/Rs if it exists
+    if 'ars' in fit.errors:
+        results['a/R*'] = {
+            'value': str(round_to_2(fit.parameters['ars'], fit.errors['ars'])),
+            'uncertainty': str(round_to_2(fit.errors['ars'])),
+        }
+
+    # check for inclination
+    if 'inc' in fit.errors:
+        results['inc'] = {
+            'value': str(round_to_2(fit.parameters['inc'], fit.errors['inc'])),
+            'uncertainty': str(round_to_2(fit.errors['inc'])),
+            'units': "degrees"
+        }
+
     return priors, filter_type, results
```

## Comparing `exotic-3.0.2/.github/workflows/python-publish.yml` & `exotic-3.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/README.md` & `exotic-3.1.0/docs/README.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf` & `exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf` & `exotic-3.1.0/docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Mac-Benutzer.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/German/Wie-EXOTIC-funktioniert.pdf` & `exotic-3.1.0/docs/regions/German/Wie-EXOTIC-funktioniert.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/German/Beispiel_Output.txt` & `exotic-3.1.0/docs/regions/German/Beispiel_Output.txt`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf` & `exotic-3.1.0/docs/regions/German/Einfuehrung-in-Exoplaneten.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/German/Benutzung-von-GitHub.pdf` & `exotic-3.1.0/docs/regions/German/Benutzung-von-GitHub.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf` & `exotic-3.1.0/docs/regions/Brazilian_Portuguese/Como-executar-o-EXOTIC-na-nuvem-colaborativa-do-Google.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/Brazilian_Portuguese/README.md` & `exotic-3.1.0/docs/regions/Brazilian_Portuguese/README.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md` & `exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Ubuntu.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/Getting-Started-with-EXOTIC.pdf` & `exotic-3.1.0/docs/regions/English/Getting-Started-with-EXOTIC.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/How-EXOTIC-Works.pdf` & `exotic-3.1.0/docs/regions/English/How-EXOTIC-Works.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md` & `exotic-3.1.0/docs/regions/English/EXOTIC Installation Instructions for Windows 10.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md` & `exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-openSUSE-Linux.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf` & `exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-with-the-Python-Notebook.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md` & `exotic-3.1.0/docs/regions/English/EXOTIC-Installation-Instructions-for-Mac-Users.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md` & `exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Fedora-Linux.md`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf` & `exotic-3.1.0/docs/regions/English/How-to-Run-EXOTIC-in-Google-Cloud-Collab.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/example_output.txt` & `exotic-3.1.0/docs/regions/English/example_output.txt`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt` & `exotic-3.1.0/docs/regions/English/How-to-select-comparision-stars-using-AAVSO-Star-Charts.txt`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/How_to_Use_GitHub.pdf` & `exotic-3.1.0/docs/regions/English/How_to_Use_GitHub.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/English/Introduction-to-Exoplanets.pdf` & `exotic-3.1.0/docs/regions/English/Introduction-to-Exoplanets.pdf`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx` & `exotic-3.1.0/docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/exotic_planetparams.png` & `exotic-3.1.0/docs/Images/exotic_planetparams.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/ExoplanetWatch.png` & `exotic-3.1.0/docs/Images/ExoplanetWatch.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/posterior_sample.png` & `exotic-3.1.0/docs/Images/posterior_sample.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/exotic_running.png` & `exotic-3.1.0/docs/Images/exotic_running.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/exotic_inputobs.png` & `exotic-3.1.0/docs/Images/exotic_inputobs.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/transitsimple.jpg` & `exotic-3.1.0/docs/Images/transitsimple.jpg`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/exotic_initssaved.png` & `exotic-3.1.0/docs/Images/exotic_initssaved.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/exotic_inputplanetparams.png` & `exotic-3.1.0/docs/Images/exotic_inputplanetparams.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/HAT-P-32bExample.png` & `exotic-3.1.0/docs/Images/HAT-P-32bExample.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/Background_Estimate.png` & `exotic-3.1.0/docs/Images/Background_Estimate.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/Hot_pixel_mask.png` & `exotic-3.1.0/docs/Images/Hot_pixel_mask.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/exotic_inputobsinfo.png` & `exotic-3.1.0/docs/Images/exotic_inputobsinfo.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/exotic_loading.png` & `exotic-3.1.0/docs/Images/exotic_loading.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/exotic_saveinits.png` & `exotic-3.1.0/docs/Images/exotic_saveinits.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/centroids.png` & `exotic-3.1.0/docs/Images/centroids.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/exotic_redmode.png` & `exotic-3.1.0/docs/Images/exotic_redmode.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/exotic_welcome.png` & `exotic-3.1.0/docs/Images/exotic_welcome.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/docs/Images/exotic_runmode.png` & `exotic-3.1.0/docs/Images/exotic_runmode.png`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/examples/tess.py` & `exotic-3.1.0/examples/tess.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # first create an environment with the proper dependencies + version
 # git clone https://github.com/rzellem/EXOTIC.git
 # cd EXOTIC
 # git checkout tess
-# cd examples
 # conda create -n tess python=3.9
 # conda activate tess
-# pip install pandas scipy matplotlib astropy statsmodels cython
-# pip install wotan transitleastsquares pylightcurve lightkurve ultranest==3.5.6
-# cd ..
+# pip install pandas scipy matplotlib astropy statsmodels cython numpy==1.21.6
+# pip install wotan transitleastsquares pylightcurve lightkurve==2.0.6 ultranest==3.5.6
 # pip install .
 # cd examples
 # python tess.py -t "HAT-P-18 b"
 import os
 import copy
 import json
 import pickle
@@ -735,31 +733,12 @@
             'Time (JD)':myfit.time,
             'Relative Flux':myfit.data,
             'Relative Flux Error':myfit.dataerr,
         }
 
         # create AAVSO formatted csv
         csv_lk = OutputFiles(myfit, prior, infoDict, planetdir)
-        try:
-            csv_lk.aavso_csv(airmass,u0,u1,u2,u3,tmidstr)
-            csv_lk.aavso(airmass,u0,u1,u2,u3, tmidstr)
-        except:
-            print(f"Failed to create AAVSO csv for {args.target} - Sector {lcdata['sector']}")
+        csv_lk.aavso_csv(airmass,u0,u1,u2,u3,tmidstr)
+        csv_lk.aavso(airmass,u0,u1,u2,u3, tmidstr)
 
     # save sv pickle
-    pickle.dump(sv, open(os.path.join(planetdir, planetname+"_data.pkl"),"wb"))
-        
-    # O-C plot
-    tmids = np.array([lc['pars']['tmid'] for lc in sv['lightcurves']])
-    tmiderr = np.array([lc['errors']['tmid'] for lc in sv['lightcurves']])
-    sectors = np.array([lc['sector'] for lc in sv['lightcurves']])
-    ratios = np.array([lc['partial_ratio'] for lc in sv['lightcurves']])
-
-    # mask out partial transits
-    dmask = ratios > 0.75
-    tmids = tmids[dmask]
-    tmiderr = tmiderr[dmask]
-    sectors = sectors[dmask]
-    ratios = ratios[dmask]
-
-    # TODO finish making O-C plot?
-    # use example from exotic.api.nested_linear_fitter
+    pickle.dump(sv, open(os.path.join(planetdir, planetname+"_data.pkl"),"wb"))
```

## Comparing `exotic-3.0.2/examples/lc_fitter_unit_test.py` & `exotic-3.1.0/examples/lc_fitter_unit_test.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/examples/Multiple_Lightcurve_fit.ipynb` & `exotic-3.1.0/examples/Multiple_Lightcurve_fit.ipynb`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/examples/sampledata.json` & `exotic-3.1.0/examples/sampledata.json`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/examples/Exoplanet_Watch_API.ipynb` & `exotic-3.1.0/examples/Exoplanet_Watch_API.ipynb`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/examples/global_fitter_unit_test.py` & `exotic-3.1.0/examples/global_fitter_unit_test.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/examples/interactive_fitter.py` & `exotic-3.1.0/examples/interactive_fitter.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/tests/test_utils.py` & `exotic-3.1.0/tests/test_utils.py`

 * *Files identical despite different names*

## Comparing `exotic-3.0.2/exotic.egg-info/PKG-INFO` & `exotic-3.1.0/exotic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exotic
-Version: 3.0.2
+Version: 3.1.0
 Summary: EXOTIC: EXOplanet Transit Interpretation Code
 Home-page: https://github.com/rzellem/EXOTIC
 Download-URL: https://github.com/rzellem/EXOTIC/releases/latest
 Author: Exoplanet Watch at NASA JPL
 Author-email: exoplanetwatch@jpl.nasa.gov
 License: Proprietary -- Copyright (c) 2019-present, California Institute of Technology.
 Project-URL: Documentation, https://github.com/rzellem/EXOTIC/wiki
```

## Comparing `exotic-3.0.2/exotic.egg-info/SOURCES.txt` & `exotic-3.1.0/exotic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 docs/regions/German/EXOTIC-Installationsanweisungen-fuer-Windows-Benutzer.pdf
 docs/regions/German/Einfuehrung-in-Exoplaneten.pdf
 docs/regions/German/Wie-EXOTIC-funktioniert.pdf
 docs/regions/German/translators.md
 docs/regions/Spanish (Español)/Introducción a los Exoplanetas (Introduction-to-Exoplanets) - SPA.docx
 docs/regions/Spanish (Español)/translators.md
 examples/Exoplanet_Watch_API.ipynb
+examples/Multiple_Lightcurve_Fit_Detrended.ipynb
 examples/Multiple_Lightcurve_fit.ipynb
 examples/global_fitter_unit_test.py
 examples/interactive_fitter.py
 examples/lc_fitter_unit_test.py
 examples/sampledata.json
 examples/tess.py
 exotic/__init__.py
```

