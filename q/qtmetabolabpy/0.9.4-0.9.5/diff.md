# Comparing `tmp/qtmetabolabpy-0.9.4.tar.gz` & `tmp/qtmetabolabpy-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmetabolabpy-0.9.4.tar", last modified: Fri Jul 21 11:28:53 2023, max compression
+gzip compressed data, was "qtmetabolabpy-0.9.5.tar", last modified: Tue Jul 25 19:32:44 2023, max compression
```

## Comparing `qtmetabolabpy-0.9.4.tar` & `qtmetabolabpy-0.9.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.014507 qtmetabolabpy-0.9.4/
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)    35149 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/LICENSE
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      364 2023-07-11 15:01:39.000000 qtmetabolabpy-0.9.4/MANIFEST.in
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     3745 2023-07-21 11:28:53.014277 qtmetabolabpy-0.9.4/PKG-INFO
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     2977 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/README.rst
-drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.011184 qtmetabolabpy-0.9.4/qtmetabolabpy/
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      195 2023-07-21 11:28:48.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/__init__.py
--rwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     5014 2023-07-16 19:58:28.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/__main__.py
-drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.012653 qtmetabolabpy-0.9.4/qtmetabolabpy/bash/
--rwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      556 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/bash/fix_pyside2
-drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.012975 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/
-drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.013289 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      884 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/Info.plist
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        9 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/PkgInfo
-drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.013455 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/Resources/
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)   173336 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Icon
--rwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)   376412 2023-07-21 11:25:55.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/qtMetaboLabPy.py
-drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.013712 qtmetabolabpy-0.9.4/qtmetabolabpy/ui/
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)   243075 2023-07-19 20:57:45.000000 qtmetabolabpy-0.9.4/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
-drwxr-xr-x   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        0 2023-07-21 11:28:53.012506 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     3745 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/PKG-INFO
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      607 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/SOURCES.txt
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)        1 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/dependency_links.txt
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       62 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/entry_points.txt
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       97 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/requires.txt
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       14 2023-07-21 11:28:52.000000 qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/top_level.txt
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)      323 2023-07-21 11:26:22.000000 qtmetabolabpy-0.9.4/requirements.txt
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)       38 2023-07-21 11:28:53.014546 qtmetabolabpy-0.9.4/setup.cfg
--rw-r--r--   0 ludwigc  (1699341573) ADF\Domain Users (1311385079)     3912 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.4/setup.py
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.008589 qtmetabolabpy-0.9.5/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079    35149 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/LICENSE
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      364 2023-07-11 15:01:39.000000 qtmetabolabpy-0.9.5/MANIFEST.in
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     3745 2023-07-25 19:32:44.008368 qtmetabolabpy-0.9.5/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     2977 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/README.rst
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.005553 qtmetabolabpy-0.9.5/qtmetabolabpy/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      195 2023-07-25 19:28:49.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/__init__.py
+-rwxr-xr-x   0 ludwigc  (1699341573) 1311385079     5014 2023-07-16 19:58:28.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/__main__.py
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.006656 qtmetabolabpy-0.9.5/qtmetabolabpy/bash/
+-rwxr-xr-x   0 ludwigc  (1699341573) 1311385079      556 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/bash/fix_pyside2
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.007026 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.007480 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      884 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/Info.plist
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079        9 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/PkgInfo
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.007656 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/Resources/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079   173336 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079        0 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Icon
+-rwxr-xr-x   0 ludwigc  (1699341573) 1311385079   376308 2023-07-24 18:45:31.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/qtMetaboLabPy.py
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.008009 qtmetabolabpy-0.9.5/qtmetabolabpy/ui/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079   242054 2023-07-24 23:32:39.000000 qtmetabolabpy-0.9.5/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
+drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:32:44.006517 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     3745 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/PKG-INFO
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      607 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079        1 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       62 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/entry_points.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       97 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/requires.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       14 2023-07-25 19:32:43.000000 qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/top_level.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079      323 2023-07-21 11:26:22.000000 qtmetabolabpy-0.9.5/requirements.txt
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079       38 2023-07-25 19:32:44.008635 qtmetabolabpy-0.9.5/setup.cfg
+-rw-r--r--   0 ludwigc  (1699341573) 1311385079     3912 2023-06-29 16:08:18.000000 qtmetabolabpy-0.9.5/setup.py
```

### Comparing `qtmetabolabpy-0.9.4/LICENSE` & `qtmetabolabpy-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.4/PKG-INFO` & `qtmetabolabpy-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.9.4/README.rst` & `qtmetabolabpy-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.4/qtmetabolabpy/__main__.py` & `qtmetabolabpy-0.9.5/qtmetabolabpy/__main__.py`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.4/qtmetabolabpy/bash/fix_pyside2` & `qtmetabolabpy-0.9.5/qtmetabolabpy/bash/fix_pyside2`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/Info.plist` & `qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.4/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns` & `qtmetabolabpy-0.9.5/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.4/qtmetabolabpy/qtMetaboLabPy.py` & `qtmetabolabpy-0.9.5/qtmetabolabpy/qtMetaboLabPy.py`

 * *Files 0% similar despite different names*

```diff
@@ -867,16 +867,14 @@
         self.show_ph_corr2d()
         self.set_proc_pars()
         self.show_acquisition_parameters()
         self.show_nmr_spectrum()
         # end apply_2d_ph_corr
 
     def autobaseline(self):
-        #print("autobaseline")
-        #print(self.nd.nmrdat[self.nd.s][self.nd.e].dim)
         if self.nd.nmrdat[self.nd.s][self.nd.e].dim == 1:
             self.autobaseline1d()
         elif self.nd.nmrdat[self.nd.s][self.nd.e].dim == 2:
             self.autobaseline2d()
 
         # end autobaseline
 
@@ -5488,14 +5486,15 @@
             self.nd.ft()
             if self.nd.nmrdat[self.nd.s][self.nd.e].dim == 0:
                 self.nd.auto_ref(True)
             else:
                 self.nd.auto_ref(False)
 
             self.nd.e = len(self.nd.nmrdat[self.nd.s]) - 1
+            self.nd.auto_ref()
             self.plot_spc()
             self.w.keepZoom.setChecked(kz)
             self.set_proc_pars()
             self.set_acq_pars()
             self.set_title_file()
             self.set_pulse_program()
             self.w.expBox.setValue(self.nd.e + 1)
@@ -7039,15 +7038,14 @@
 
     def set_ma_echo_time(self):
         if len(self.w.multipletAnalysisEchoTime.text()) > 0:
             echo_time = float(self.w.multipletAnalysisEchoTime.text())
             if self.w.maApplyToAll.isChecked():
                 for k in range(len(self.nd.nmrdat[self.nd.s])):
                     self.nd.nmrdat[self.nd.s][k].hsqc.echo_time = echo_time
-                    hsqc.echo_time = echo_time
 
             self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.echo_time = echo_time
 
     # end set_ma_echo_time
 
     def set_ma_intensity(self):
         hsqc = self.nd.nmrdat[self.nd.s][self.nd.e].hsqc
```

### Comparing `qtmetabolabpy-0.9.4/qtmetabolabpy/ui/metabolabpy_mainwindow.ui` & `qtmetabolabpy-0.9.5/qtmetabolabpy/ui/metabolabpy_mainwindow.ui`

 * *Files 1% similar despite different names*

#### Comparing `qtmetabolabpy-0.9.4/qtmetabolabpy/ui/metabolabpy_mainwindow.ui` & `qtmetabolabpy-0.9.5/qtmetabolabpy/ui/metabolabpy_mainwindow.ui`

```diff
@@ -3514,75 +3514,21 @@
                                     <column>
                                       <property name="text">
                                         <string>[%]</string>
                                       </property>
                                     </column>
                                   </widget>
                                 </item>
-                                <item row="1" column="0">
-                                  <widget class="QCheckBox" name="maAutoScale">
-                                    <property name="text">
-                                      <string>Autoscale</string>
-                                    </property>
-                                    <property name="checked">
-                                      <bool>true</bool>
-                                    </property>
-                                  </widget>
-                                </item>
-                                <item row="2" column="0">
-                                  <widget class="QCheckBox" name="maAutoSim">
-                                    <property name="text">
-                                      <string>Autosim</string>
-                                    </property>
-                                    <property name="checked">
-                                      <bool>false</bool>
-                                    </property>
-                                  </widget>
-                                </item>
                                 <item row="3" column="0" rowspan="2" colspan="7">
                                   <widget class="Line" name="line_2">
                                     <property name="orientation">
                                       <enum>Qt::Horizontal</enum>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="4" column="1" rowspan="2" colspan="2">
-                                  <spacer name="horizontalSpacer_47">
-                                    <property name="orientation">
-                                      <enum>Qt::Horizontal</enum>
-                                    </property>
-                                    <property name="sizeHint" stdset="0">
-                                      <size>
-                                        <width>96</width>
-                                        <height>20</height>
-                                      </size>
-                                    </property>
-                                  </spacer>
-                                </item>
-                                <item row="4" column="3" rowspan="2" colspan="2">
-                                  <widget class="QLabel" name="label_84">
-                                    <property name="text">
-                                      <string>Echo time [ms]:</string>
-                                    </property>
-                                  </widget>
-                                </item>
-                                <item row="5" column="0">
-                                  <widget class="QCheckBox" name="maApplyToAll">
-                                    <property name="text">
-                                      <string>Apply to all</string>
-                                    </property>
-                                  </widget>
-                                </item>
-                                <item row="5" column="5" colspan="2">
-                                  <widget class="QLineEdit" name="multipletAnalysisEchoTime">
-                                    <property name="alignment">
-                                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                                    </property>
-                                  </widget>
-                                </item>
                                 <item row="6" column="0" rowspan="2" colspan="7">
                                   <widget class="Line" name="line">
                                     <property name="orientation">
                                       <enum>Qt::Horizontal</enum>
                                     </property>
                                   </widget>
                                 </item>
@@ -3630,52 +3576,93 @@
                                 <item row="10" column="6">
                                   <widget class="QPushButton" name="maFitButton">
                                     <property name="text">
                                       <string>Fit</string>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="1" column="1" colspan="2">
-                                  <widget class="QLabel" name="label_82">
+                                <item row="10" column="4">
+                                  <widget class="QPushButton" name="exportHsqcData">
                                     <property name="text">
-                                      <string>Intensity:</string>
+                                      <string>Export all</string>
                                     </property>
+                                  </widget>
+                                </item>
+                                <item row="5" column="6">
+                                  <widget class="QLineEdit" name="multipletAnalysisEchoTime">
                                     <property name="alignment">
                                       <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="2" column="1" colspan="2">
-                                  <widget class="QLabel" name="label_83">
+                                <item row="5" column="0" colspan="2">
+                                  <widget class="QCheckBox" name="maApplyToAll">
                                     <property name="text">
-                                      <string>Linewidth [Hz]:</string>
+                                      <string>Apply to all</string>
                                     </property>
-                                    <property name="alignment">
-                                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                  </widget>
+                                </item>
+                                <item row="5" column="4" colspan="2">
+                                  <widget class="QLabel" name="label_84">
+                                    <property name="text">
+                                      <string>Echo time [ms]:</string>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="2" column="3" colspan="4">
+                                <item row="2" column="4" colspan="3">
                                   <widget class="QLineEdit" name="multipletAnalysisR2">
                                     <property name="alignment">
                                       <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="1" column="3" colspan="4">
+                                <item row="1" column="4" colspan="3">
                                   <widget class="QLineEdit" name="multipletAnalysisIntensity">
                                     <property name="alignment">
                                       <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                                     </property>
                                   </widget>
                                 </item>
-                                <item row="10" column="4">
-                                  <widget class="QPushButton" name="exportHsqcData">
+                                <item row="1" column="3">
+                                  <widget class="QLabel" name="label_82">
                                     <property name="text">
-                                      <string>Export all</string>
+                                      <string>Int.:</string>
+                                    </property>
+                                    <property name="alignment">
+                                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item row="2" column="3">
+                                  <widget class="QLabel" name="label_83">
+                                    <property name="text">
+                                      <string>lw [Hz]:</string>
+                                    </property>
+                                    <property name="alignment">
+                                      <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item row="1" column="0" colspan="2">
+                                  <widget class="QCheckBox" name="maAutoScale">
+                                    <property name="text">
+                                      <string>Autoscale</string>
+                                    </property>
+                                    <property name="checked">
+                                      <bool>true</bool>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item row="2" column="0" colspan="2">
+                                  <widget class="QCheckBox" name="maAutoSim">
+                                    <property name="text">
+                                      <string>Autosim</string>
+                                    </property>
+                                    <property name="checked">
+                                      <bool>false</bool>
                                     </property>
                                   </widget>
                                 </item>
                               </layout>
                             </widget>
                             <widget class="QWidget" name="hsqcSetupTab">
                               <attribute name="title">
@@ -3789,15 +3776,15 @@
                                       </property>
                                     </item>
                                   </widget>
                                 </item>
                                 <item row="5" column="0" colspan="3">
                                   <widget class="QLabel" name="label_92">
                                     <property name="text">
-                                      <string>Autoscale 13C range with J-scale (cnst18)</string>
+                                      <string>Scale 13C range with J-scale (cnst18)</string>
                                     </property>
                                   </widget>
                                 </item>
                                 <item row="5" column="4">
                                   <widget class="QComboBox" name="autoscaleCB">
                                     <item>
                                       <property name="text">
@@ -6430,72 +6417,14 @@
               </layout>
             </widget>
             <widget class="QWidget" name="helpTab">
               <attribute name="title">
                 <string>Help</string>
               </attribute>
               <layout class="QGridLayout" name="gridLayout_27">
-                <item row="1" column="5">
-                  <widget class="QCheckBox" name="autoUnzip">
-                    <property name="text">
-                      <string>Auto-unzip downloaded zip files</string>
-                    </property>
-                    <property name="checked">
-                      <bool>true</bool>
-                    </property>
-                  </widget>
-                </item>
-                <item row="1" column="3">
-                  <widget class="QPushButton" name="stopNotebookButton">
-                    <property name="text">
-                      <string>Stop Notebook Server</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="1" column="2">
-                  <widget class="QPushButton" name="startNotebookButton">
-                    <property name="text">
-                      <string>(Re-)Start Notebook Server</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="0" column="0" colspan="6">
-                  <widget class="QWebEngineView2" name="helpView" native="true">
-                    <property name="sizePolicy">
-                      <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
-                        <horstretch>0</horstretch>
-                        <verstretch>0</verstretch>
-                      </sizepolicy>
-                    </property>
-                    <property name="maximumSize">
-                      <size>
-                        <width>16777215</width>
-                        <height>16777215</height>
-                      </size>
-                    </property>
-                    <property name="font">
-                      <font>
-                        <pointsize>8</pointsize>
-                      </font>
-                    </property>
-                  </widget>
-                </item>
-                <item row="1" column="4">
-                  <spacer name="horizontalSpacer_24">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>1208</width>
-                        <height>20</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
                 <item row="1" column="0">
                   <widget class="QComboBox" name="helpComboBox">
                     <item>
                       <property name="text">
                         <string>Help</string>
                       </property>
                     </item>
@@ -6537,28 +6466,72 @@
                     <item>
                       <property name="text">
                         <string>SpinCouple</string>
                       </property>
                     </item>
                   </widget>
                 </item>
+                <item row="1" column="2">
+                  <spacer name="horizontalSpacer_24">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>1208</width>
+                        <height>20</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
                 <item row="1" column="1">
                   <widget class="QComboBox" name="tutorialComboBox">
                     <item>
                       <property name="text">
                         <string>Tutorial 1</string>
                       </property>
                     </item>
                     <item>
                       <property name="text">
                         <string>Tutorial 2</string>
                       </property>
                     </item>
                   </widget>
                 </item>
+                <item row="0" column="0" colspan="4">
+                  <widget class="QWebEngineView2" name="helpView" native="true">
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                    <property name="maximumSize">
+                      <size>
+                        <width>16777215</width>
+                        <height>16777215</height>
+                      </size>
+                    </property>
+                    <property name="font">
+                      <font>
+                        <pointsize>8</pointsize>
+                      </font>
+                    </property>
+                  </widget>
+                </item>
+                <item row="1" column="3">
+                  <widget class="QCheckBox" name="autoUnzip">
+                    <property name="text">
+                      <string>Auto-unzip downloaded zip files</string>
+                    </property>
+                    <property name="checked">
+                      <bool>true</bool>
+                    </property>
+                  </widget>
+                </item>
               </layout>
             </widget>
           </widget>
         </item>
       </layout>
     </widget>
     <widget class="QMenuBar" name="menuBar">
```

### Comparing `qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/PKG-INFO` & `qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.9.4/qtmetabolabpy.egg-info/SOURCES.txt` & `qtmetabolabpy-0.9.5/qtmetabolabpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.9.4/setup.py` & `qtmetabolabpy-0.9.5/setup.py`

 * *Files identical despite different names*

