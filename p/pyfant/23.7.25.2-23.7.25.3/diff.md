# Comparing `tmp/pyfant-23.7.25.2.tar.gz` & `tmp/pyfant-23.7.25.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfant-23.7.25.2.tar", last modified: Tue Jul 25 19:55:16 2023, max compression
+gzip compressed data, was "pyfant-23.7.25.3.tar", last modified: Tue Jul 25 20:02:06 2023, max compression
```

## Comparing `pyfant-23.7.25.2.tar` & `pyfant-23.7.25.3.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.012812 pyfant-23.7.25.2/
--rw-rw-r--   0 j         (1000) j         (1000)       34 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/MANIFEST.in
--rw-rw-r--   0 j         (1000) j         (1000)      445 2023-07-25 19:55:16.012812 pyfant-23.7.25.2/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)      150 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/README.md
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.004812 pyfant-23.7.25.2/pyfant/
--rw-rw-r--   0 j         (1000) j         (1000)     1219 2023-04-12 12:29:24.000000 pyfant-23.7.25.2/pyfant/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     1143 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/_star.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.004812 pyfant-23.7.25.2/pyfant/basic/
--rw-rw-r--   0 j         (1000) j         (1000)      396 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/basic/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      774 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/basic/constants.py
--rw-rw-r--   0 j         (1000) j         (1000)    13736 2023-07-25 19:31:29.000000 pyfant-23.7.25.2/pyfant/basic/conversion.py
--rw-rw-r--   0 j         (1000) j         (1000)      215 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/basic/errors.py
--rw-rw-r--   0 j         (1000) j         (1000)      738 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/basic/misc.py
--rw-rw-r--   0 j         (1000) j         (1000)     2540 2023-07-25 19:51:37.000000 pyfant-23.7.25.2/pyfant/basic/paths.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.004812 pyfant-23.7.25.2/pyfant/convmol/
--rw-rw-r--   0 j         (1000) j         (1000)      281 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/convmol/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     1686 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/convmol/calc_qgbd.py
--rw-rw-r--   0 j         (1000) j         (1000)     9987 2023-07-24 13:55:19.000000 pyfant-23.7.25.2/pyfant/convmol/conv.py
--rw-rw-r--   0 j         (1000) j         (1000)    14275 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/convmol/conv_brooke2014.py
--rw-rw-r--   0 j         (1000) j         (1000)    16508 2023-07-24 13:55:04.000000 pyfant-23.7.25.2/pyfant/convmol/conv_hitran.py
--rw-rw-r--   0 j         (1000) j         (1000)     5402 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/convmol/conv_hitran160.py
--rw-rw-r--   0 j         (1000) j         (1000)     3694 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/convmol/conv_kurucz.py
--rw-rw-r--   0 j         (1000) j         (1000)     3602 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/convmol/conv_plez.py
--rw-rw-r--   0 j         (1000) j         (1000)     3328 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/convmol/conv_vald3.py
--rw-rw-r--   0 j         (1000) j         (1000)     1585 2023-05-31 22:53:51.000000 pyfant-23.7.25.2/pyfant/convmol/convlog.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.004812 pyfant-23.7.25.2/pyfant/data/
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.004812 pyfant-23.7.25.2/pyfant/data/default/
--rw-rw-r--   0 j         (1000) j         (1000)     1163 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/abonds.dat
--rw-rw-r--   0 j         (1000) j         (1000)     2551 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/absoru2.dat
--rw-rw-r--   0 j         (1000) j         (1000)      618 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/abxfwhm.py
--rw-rw-r--   0 j         (1000) j         (1000)      362 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/configconvmol.py
--rw-rw-r--   0 j         (1000) j         (1000)     1353 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/configmolconsts.py
--rw-rw-r--   0 j         (1000) j         (1000)     3628 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/dissoc.dat
--rw-rw-r--   0 j         (1000) j         (1000)    14336 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/hitrandb.sqlite
--rw-rw-r--   0 j         (1000) j         (1000)      381 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/hmap.dat
--rw-rw-r--   0 j         (1000) j         (1000)       89 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/main.dat
--rw-rw-r--   0 j         (1000) j         (1000)     2400 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/modeles.mod
--rw-rw-r--   0 j         (1000) j         (1000)    77824 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/moldb.sqlite
--rw-rw-r--   0 j         (1000) j         (1000)    53356 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/data/default/partit.dat
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.004812 pyfant-23.7.25.2/pyfant/downloaders/
--rw-rw-r--   0 j         (1000) j         (1000)      783 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/downloaders/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     5083 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/downloaders/downhitran.py
--rw-rw-r--   0 j         (1000) j         (1000)     7550 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/downloaders/downnist.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.008812 pyfant-23.7.25.2/pyfant/filetypes/
--rw-rw-r--   0 j         (1000) j         (1000)      699 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/filetypes/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     7533 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/fileabonds.py
--rw-rw-r--   0 j         (1000) j         (1000)      494 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/fileabsoru2.py
--rw-rw-r--   0 j         (1000) j         (1000)     5690 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/fileabxfwhm.py
--rw-rw-r--   0 j         (1000) j         (1000)     9301 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/fileatoms.py
--rw-rw-r--   0 j         (1000) j         (1000)     6927 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/filetypes/filebrooke2014.py
--rw-rw-r--   0 j         (1000) j         (1000)     2220 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/filetypes/filecojm1998.py
--rw-rw-r--   0 j         (1000) j         (1000)      348 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/fileconfconvmol.py
--rw-rw-r--   0 j         (1000) j         (1000)     4346 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/filedissoc.py
--rw-rw-r--   0 j         (1000) j         (1000)    11105 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/filetypes/filehitran160.py
--rw-rw-r--   0 j         (1000) j         (1000)     3964 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/filehitrandb.py
--rw-rw-r--   0 j         (1000) j         (1000)     2360 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/filehmap.py
--rw-rw-r--   0 j         (1000) j         (1000)    17698 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/filetypes/filekuruczmol.py
--rw-rw-r--   0 j         (1000) j         (1000)     4058 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/filemain.py
--rw-rw-r--   0 j         (1000) j         (1000)    17453 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/filemod.py
--rw-rw-r--   0 j         (1000) j         (1000)     1101 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/filemolconsts.py
--rw-rw-r--   0 j         (1000) j         (1000)    14451 2023-05-28 11:43:17.000000 pyfant-23.7.25.2/pyfant/filetypes/filemoldb.py
--rw-rw-r--   0 j         (1000) j         (1000)    18441 2023-07-05 21:06:29.000000 pyfant-23.7.25.2/pyfant/filetypes/filemolecules.py
--rw-rw-r--   0 j         (1000) j         (1000)      980 2023-07-05 21:06:29.000000 pyfant-23.7.25.2/pyfant/filetypes/filemollist.py
--rw-rw-r--   0 j         (1000) j         (1000)     4381 2023-04-14 20:41:53.000000 pyfant-23.7.25.2/pyfant/filetypes/fileoptions.py
--rw-rw-r--   0 j         (1000) j         (1000)      518 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/filepartit.py
--rw-rw-r--   0 j         (1000) j         (1000)    16754 2023-06-30 20:15:22.000000 pyfant-23.7.25.2/pyfant/filetypes/fileplezlinelist.py
--rw-rw-r--   0 j         (1000) j         (1000)    10212 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/filepleztio.py
--rw-rw-r--   0 j         (1000) j         (1000)     3085 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/filetoh.py
--rw-rw-r--   0 j         (1000) j         (1000)    17088 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/filetraprb.py
--rw-rw-r--   0 j         (1000) j         (1000)    10714 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/filevald3.py
--rw-rw-r--   0 j         (1000) j         (1000)     9913 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/filetypes/morespectra.py
--rw-rw-r--   0 j         (1000) j         (1000)     5793 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/from_turbospectrum.py
--rw-rw-r--   0 j         (1000) j         (1000)     6563 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/from_vald.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.008812 pyfant-23.7.25.2/pyfant/gui/
--rw-rw-r--   0 j         (1000) j         (1000)     1768 2023-04-12 13:57:59.000000 pyfant-23.7.25.2/pyfant/gui/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)     3086 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/_shared.py
--rw-rw-r--   0 j         (1000) j         (1000)    13175 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WContinua.py
--rw-rw-r--   0 j         (1000) j         (1000)     5037 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WContinuum.py
--rw-rw-r--   0 j         (1000) j         (1000)     7851 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WDBFCF.py
--rw-rw-r--   0 j         (1000) j         (1000)     5134 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WDBMolecule.py
--rw-rw-r--   0 j         (1000) j         (1000)     4856 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WDBPFANTMol.py
--rw-rw-r--   0 j         (1000) j         (1000)     6533 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WDBState.py
--rw-rw-r--   0 j         (1000) j         (1000)     4791 2023-05-27 11:10:12.000000 pyfant-23.7.25.2/pyfant/gui/a_WDBSystem.py
--rw-rw-r--   0 j         (1000) j         (1000)     3789 2023-05-28 11:36:39.000000 pyfant-23.7.25.2/pyfant/gui/a_WDBSystemPfantmolFCF.py
--rw-rw-r--   0 j         (1000) j         (1000)     7412 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WFileAbXFwhm.py
--rw-rw-r--   0 j         (1000) j         (1000)    11906 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WFileAbonds.py
--rw-rw-r--   0 j         (1000) j         (1000)    14369 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WFileMain.py
--rw-rw-r--   0 j         (1000) j         (1000)     3832 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WFileMolConsts.py
--rw-rw-r--   0 j         (1000) j         (1000)     2312 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WFileMolDB.py
--rw-rw-r--   0 j         (1000) j         (1000)    36626 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/gui/a_WMolecularConstants.py
--rw-rw-r--   0 j         (1000) j         (1000)    33331 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_WOptionsEditor.py
--rw-rw-r--   0 j         (1000) j         (1000)     3059 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XAtomLinesEditor.py
--rw-rw-r--   0 j         (1000) j         (1000)    36371 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XConvMol.py
--rw-rw-r--   0 j         (1000) j         (1000)     5551 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XFileAbonds.py
--rw-rw-r--   0 j         (1000) j         (1000)    15676 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XFileAtoms.py
--rw-rw-r--   0 j         (1000) j         (1000)     3212 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XFileAtomsHistogram.py
--rw-rw-r--   0 j         (1000) j         (1000)     3826 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XFileMain.py
--rw-rw-r--   0 j         (1000) j         (1000)     1874 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XFileMolConsts.py
--rw-rw-r--   0 j         (1000) j         (1000)     1023 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XFileMolDB.py
--rw-rw-r--   0 j         (1000) j         (1000)     3544 2023-04-12 14:29:20.000000 pyfant-23.7.25.2/pyfant/gui/a_XFileMoleculeHistogram.py
--rw-rw-r--   0 j         (1000) j         (1000)    25430 2023-05-05 17:13:54.000000 pyfant-23.7.25.2/pyfant/gui/a_XFileMolecules.py
--rw-rw-r--   0 j         (1000) j         (1000)      936 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XFileOptions.py
--rw-rw-r--   0 j         (1000) j         (1000)    15149 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XMainAbonds.py
--rw-rw-r--   0 j         (1000) j         (1000)     3049 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XMolLinesEditor.py
--rw-rw-r--   0 j         (1000) j         (1000)     7504 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XMulti.py
--rw-rw-r--   0 j         (1000) j         (1000)     4805 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XPFANT.py
--rw-rw-r--   0 j         (1000) j         (1000)    14232 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/gui/a_XRunnableManager.py
--rw-rw-r--   0 j         (1000) j         (1000)    38318 2023-04-15 22:19:35.000000 pyfant-23.7.25.2/pyfant/kovacs.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.008812 pyfant-23.7.25.2/pyfant/misc/
--rw-rw-r--   0 j         (1000) j         (1000)       27 2023-04-12 12:38:10.000000 pyfant-23.7.25.2/pyfant/misc/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      752 2023-04-12 18:08:57.000000 pyfant-23.7.25.2/pyfant/misc/molhistogram.py
--rw-rw-r--   0 j         (1000) j         (1000)    11950 2023-06-12 13:25:51.000000 pyfant-23.7.25.2/pyfant/molconsts.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.012812 pyfant-23.7.25.2/pyfant/run/
--rw-rw-r--   0 j         (1000) j         (1000)      118 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/run/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)    18394 2023-07-05 21:06:29.000000 pyfant-23.7.25.2/pyfant/run/conf.py
--rw-rw-r--   0 j         (1000) j         (1000)     9047 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/run/multirunnable.py
--rw-rw-r--   0 j         (1000) j         (1000)    16962 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/run/rm.py
--rw-rw-r--   0 j         (1000) j         (1000)    18010 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/run/runnables.py
--rw-rw-r--   0 j         (1000) j         (1000)     3725 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/run/traprbclass.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.012812 pyfant-23.7.25.2/pyfant/scripts/
--rwxrwxr-x   0 j         (1000) j         (1000)     2363 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/_copy-from-sessions.py
--rwxrwxr-x   0 j         (1000) j         (1000)     1633 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/_diff-molecules.py
--rwxrwxr-x   0 j         (1000) j         (1000)     4311 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/_plot-innewmarcs-result.py
--rwxrwxr-x   0 j         (1000) j         (1000)      563 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/_recreate-hitrandb.py
--rwxrwxr-x   0 j         (1000) j         (1000)     2216 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/_save-pdf.py
--rwxrwxr-x   0 j         (1000) j         (1000)      625 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/abed.py
--rwxrwxr-x   0 j         (1000) j         (1000)      667 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/ated.py
--rwxrwxr-x   0 j         (1000) j         (1000)     1104 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/convmol.py
--rwxrwxr-x   0 j         (1000) j         (1000)     2791 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/copy-star.py
--rwxrwxr-x   0 j         (1000) j         (1000)     3669 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/create-grid.py
--rwxrwxr-x   0 j         (1000) j         (1000)     1286 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/cut-atoms.py
--rwxrwxr-x   0 j         (1000) j         (1000)     1226 2023-07-05 21:06:29.000000 pyfant-23.7.25.2/pyfant/scripts/cut-molecules.py
--rwxrwxr-x   0 j         (1000) j         (1000)     6811 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/hitran-scraper.py
--rwxrwxr-x   0 j         (1000) j         (1000)     3173 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/link.py
--rwxrwxr-x   0 j         (1000) j         (1000)      636 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/mained.py
--rwxrwxr-x   0 j         (1000) j         (1000)      943 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/mced.py
--rw-rw-r--   0 j         (1000) j         (1000)     2197 2023-07-03 22:19:58.000000 pyfant-23.7.25.2/pyfant/scripts/merge-molecules.py
--rwxrwxr-x   0 j         (1000) j         (1000)      703 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/mled.py
--rwxrwxr-x   0 j         (1000) j         (1000)      912 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/moldbed.py
--rwxrwxr-x   0 j         (1000) j         (1000)     1848 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/nist-scraper.py
--rwxrwxr-x   0 j         (1000) j         (1000)     3879 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/nulbad.py
--rwxrwxr-x   0 j         (1000) j         (1000)      849 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/optionsed.py
--rwxrwxr-x   0 j         (1000) j         (1000)     2113 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/run-multi.py
--rwxrwxr-x   0 j         (1000) j         (1000)     1152 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/run4.py
--rw-rw-r--   0 j         (1000) j         (1000)     2388 2023-07-24 12:50:46.000000 pyfant-23.7.25.2/pyfant/scripts/search-mollines.py
--rw-rw-r--   0 j         (1000) j         (1000)     2298 2023-07-05 21:06:29.000000 pyfant-23.7.25.2/pyfant/scripts/split-molecules.py
--rwxrwxr-x   0 j         (1000) j         (1000)    10219 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/tune-zinf.py
--rwxrwxr-x   0 j         (1000) j         (1000)     2762 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/turbospectrum-to-atoms.py
--rwxrwxr-x   0 j         (1000) j         (1000)     2770 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/vald3-to-atoms.py
--rwxrwxr-x   0 j         (1000) j         (1000)     1101 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/scripts/x.py
--rw-rw-r--   0 j         (1000) j         (1000)    15663 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/util.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.012812 pyfant-23.7.25.2/pyfant/vis/
--rw-rw-r--   0 j         (1000) j         (1000)       67 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/vis/__init__.py
--rw-rw-r--   0 j         (1000) j         (1000)      723 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/vis/modgrid.py
--rw-rw-r--   0 j         (1000) j         (1000)     3073 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/vis/vismany.py
--rw-rw-r--   0 j         (1000) j         (1000)     8273 2020-10-12 00:16:49.000000 pyfant-23.7.25.2/pyfant/vis/vismod.py
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 19:55:16.004812 pyfant-23.7.25.2/pyfant.egg-info/
--rw-rw-r--   0 j         (1000) j         (1000)      445 2023-07-25 19:55:15.000000 pyfant-23.7.25.2/pyfant.egg-info/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)     4194 2023-07-25 19:55:15.000000 pyfant-23.7.25.2/pyfant.egg-info/SOURCES.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2023-07-25 19:55:15.000000 pyfant-23.7.25.2/pyfant.egg-info/dependency_links.txt
--rw-rw-r--   0 j         (1000) j         (1000)      133 2023-07-25 19:55:15.000000 pyfant-23.7.25.2/pyfant.egg-info/requires.txt
--rw-rw-r--   0 j         (1000) j         (1000)        7 2023-07-25 19:55:15.000000 pyfant-23.7.25.2/pyfant.egg-info/top_level.txt
--rw-rw-r--   0 j         (1000) j         (1000)       38 2023-07-25 19:55:16.012812 pyfant-23.7.25.2/setup.cfg
--rw-rw-r--   0 j         (1000) j         (1000)     1583 2023-07-25 19:51:37.000000 pyfant-23.7.25.2/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.570221 pyfant-23.7.25.3/
+-rw-rw-r--   0 j         (1000) j         (1000)       34 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/MANIFEST.in
+-rw-rw-r--   0 j         (1000) j         (1000)      445 2023-07-25 20:02:06.566221 pyfant-23.7.25.3/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      150 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/README.md
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.558221 pyfant-23.7.25.3/pyfant/
+-rw-rw-r--   0 j         (1000) j         (1000)     1219 2023-04-12 12:29:24.000000 pyfant-23.7.25.3/pyfant/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1143 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/_star.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.558221 pyfant-23.7.25.3/pyfant/basic/
+-rw-rw-r--   0 j         (1000) j         (1000)      396 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/basic/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      774 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/basic/constants.py
+-rw-rw-r--   0 j         (1000) j         (1000)    13736 2023-07-25 19:31:29.000000 pyfant-23.7.25.3/pyfant/basic/conversion.py
+-rw-rw-r--   0 j         (1000) j         (1000)      215 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/basic/errors.py
+-rw-rw-r--   0 j         (1000) j         (1000)      738 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/basic/misc.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2533 2023-07-25 20:01:33.000000 pyfant-23.7.25.3/pyfant/basic/paths.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.562221 pyfant-23.7.25.3/pyfant/convmol/
+-rw-rw-r--   0 j         (1000) j         (1000)      281 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/convmol/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1686 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/convmol/calc_qgbd.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9987 2023-07-24 13:55:19.000000 pyfant-23.7.25.3/pyfant/convmol/conv.py
+-rw-rw-r--   0 j         (1000) j         (1000)    14275 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/convmol/conv_brooke2014.py
+-rw-rw-r--   0 j         (1000) j         (1000)    16508 2023-07-24 13:55:04.000000 pyfant-23.7.25.3/pyfant/convmol/conv_hitran.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5402 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/convmol/conv_hitran160.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3694 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/convmol/conv_kurucz.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3602 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/convmol/conv_plez.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3328 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/convmol/conv_vald3.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1585 2023-05-31 22:53:51.000000 pyfant-23.7.25.3/pyfant/convmol/convlog.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.558221 pyfant-23.7.25.3/pyfant/data/
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.562221 pyfant-23.7.25.3/pyfant/data/default/
+-rw-rw-r--   0 j         (1000) j         (1000)     1163 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/abonds.dat
+-rw-rw-r--   0 j         (1000) j         (1000)     2551 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/absoru2.dat
+-rw-rw-r--   0 j         (1000) j         (1000)      618 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/abxfwhm.py
+-rw-rw-r--   0 j         (1000) j         (1000)      362 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/configconvmol.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1353 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/configmolconsts.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3628 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/dissoc.dat
+-rw-rw-r--   0 j         (1000) j         (1000)    14336 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/hitrandb.sqlite
+-rw-rw-r--   0 j         (1000) j         (1000)      381 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/hmap.dat
+-rw-rw-r--   0 j         (1000) j         (1000)       89 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/main.dat
+-rw-rw-r--   0 j         (1000) j         (1000)     2400 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/modeles.mod
+-rw-rw-r--   0 j         (1000) j         (1000)    77824 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/moldb.sqlite
+-rw-rw-r--   0 j         (1000) j         (1000)    53356 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/data/default/partit.dat
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.562221 pyfant-23.7.25.3/pyfant/downloaders/
+-rw-rw-r--   0 j         (1000) j         (1000)      783 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/downloaders/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5083 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/downloaders/downhitran.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7550 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/downloaders/downnist.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.562221 pyfant-23.7.25.3/pyfant/filetypes/
+-rw-rw-r--   0 j         (1000) j         (1000)      699 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/filetypes/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7533 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/fileabonds.py
+-rw-rw-r--   0 j         (1000) j         (1000)      494 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/fileabsoru2.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5690 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/fileabxfwhm.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9301 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/fileatoms.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6927 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/filetypes/filebrooke2014.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2220 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/filetypes/filecojm1998.py
+-rw-rw-r--   0 j         (1000) j         (1000)      348 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/fileconfconvmol.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4346 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/filedissoc.py
+-rw-rw-r--   0 j         (1000) j         (1000)    11105 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/filetypes/filehitran160.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3964 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/filehitrandb.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2360 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/filehmap.py
+-rw-rw-r--   0 j         (1000) j         (1000)    17698 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/filetypes/filekuruczmol.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4058 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/filemain.py
+-rw-rw-r--   0 j         (1000) j         (1000)    17453 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/filemod.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1101 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/filemolconsts.py
+-rw-rw-r--   0 j         (1000) j         (1000)    14451 2023-05-28 11:43:17.000000 pyfant-23.7.25.3/pyfant/filetypes/filemoldb.py
+-rw-rw-r--   0 j         (1000) j         (1000)    18441 2023-07-05 21:06:29.000000 pyfant-23.7.25.3/pyfant/filetypes/filemolecules.py
+-rw-rw-r--   0 j         (1000) j         (1000)      980 2023-07-05 21:06:29.000000 pyfant-23.7.25.3/pyfant/filetypes/filemollist.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4381 2023-04-14 20:41:53.000000 pyfant-23.7.25.3/pyfant/filetypes/fileoptions.py
+-rw-rw-r--   0 j         (1000) j         (1000)      518 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/filepartit.py
+-rw-rw-r--   0 j         (1000) j         (1000)    16754 2023-06-30 20:15:22.000000 pyfant-23.7.25.3/pyfant/filetypes/fileplezlinelist.py
+-rw-rw-r--   0 j         (1000) j         (1000)    10212 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/filepleztio.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3085 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/filetoh.py
+-rw-rw-r--   0 j         (1000) j         (1000)    17088 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/filetraprb.py
+-rw-rw-r--   0 j         (1000) j         (1000)    10714 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/filevald3.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9913 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/filetypes/morespectra.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5793 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/from_turbospectrum.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6563 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/from_vald.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.566221 pyfant-23.7.25.3/pyfant/gui/
+-rw-rw-r--   0 j         (1000) j         (1000)     1768 2023-04-12 13:57:59.000000 pyfant-23.7.25.3/pyfant/gui/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3086 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/_shared.py
+-rw-rw-r--   0 j         (1000) j         (1000)    13175 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WContinua.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5037 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WContinuum.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7851 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WDBFCF.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5134 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WDBMolecule.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4856 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WDBPFANTMol.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6533 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WDBState.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4791 2023-05-27 11:10:12.000000 pyfant-23.7.25.3/pyfant/gui/a_WDBSystem.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3789 2023-05-28 11:36:39.000000 pyfant-23.7.25.3/pyfant/gui/a_WDBSystemPfantmolFCF.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7412 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WFileAbXFwhm.py
+-rw-rw-r--   0 j         (1000) j         (1000)    11906 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WFileAbonds.py
+-rw-rw-r--   0 j         (1000) j         (1000)    14369 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WFileMain.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3832 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WFileMolConsts.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2312 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WFileMolDB.py
+-rw-rw-r--   0 j         (1000) j         (1000)    36626 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/gui/a_WMolecularConstants.py
+-rw-rw-r--   0 j         (1000) j         (1000)    33331 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_WOptionsEditor.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3059 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XAtomLinesEditor.py
+-rw-rw-r--   0 j         (1000) j         (1000)    36371 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XConvMol.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5551 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XFileAbonds.py
+-rw-rw-r--   0 j         (1000) j         (1000)    15676 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XFileAtoms.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3212 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XFileAtomsHistogram.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3826 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XFileMain.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1874 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XFileMolConsts.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1023 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XFileMolDB.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3544 2023-04-12 14:29:20.000000 pyfant-23.7.25.3/pyfant/gui/a_XFileMoleculeHistogram.py
+-rw-rw-r--   0 j         (1000) j         (1000)    25430 2023-05-05 17:13:54.000000 pyfant-23.7.25.3/pyfant/gui/a_XFileMolecules.py
+-rw-rw-r--   0 j         (1000) j         (1000)      936 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XFileOptions.py
+-rw-rw-r--   0 j         (1000) j         (1000)    15149 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XMainAbonds.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3049 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XMolLinesEditor.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7504 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XMulti.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4805 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XPFANT.py
+-rw-rw-r--   0 j         (1000) j         (1000)    14232 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/gui/a_XRunnableManager.py
+-rw-rw-r--   0 j         (1000) j         (1000)    38318 2023-04-15 22:19:35.000000 pyfant-23.7.25.3/pyfant/kovacs.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.566221 pyfant-23.7.25.3/pyfant/misc/
+-rw-rw-r--   0 j         (1000) j         (1000)       27 2023-04-12 12:38:10.000000 pyfant-23.7.25.3/pyfant/misc/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      752 2023-04-12 18:08:57.000000 pyfant-23.7.25.3/pyfant/misc/molhistogram.py
+-rw-rw-r--   0 j         (1000) j         (1000)    11950 2023-06-12 13:25:51.000000 pyfant-23.7.25.3/pyfant/molconsts.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.566221 pyfant-23.7.25.3/pyfant/run/
+-rw-rw-r--   0 j         (1000) j         (1000)      118 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/run/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)    18394 2023-07-05 21:06:29.000000 pyfant-23.7.25.3/pyfant/run/conf.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9047 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/run/multirunnable.py
+-rw-rw-r--   0 j         (1000) j         (1000)    16962 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/run/rm.py
+-rw-rw-r--   0 j         (1000) j         (1000)    18010 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/run/runnables.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3725 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/run/traprbclass.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.566221 pyfant-23.7.25.3/pyfant/scripts/
+-rwxrwxr-x   0 j         (1000) j         (1000)     2363 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/_copy-from-sessions.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1633 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/_diff-molecules.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     4311 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/_plot-innewmarcs-result.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      563 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/_recreate-hitrandb.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     2216 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/_save-pdf.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      625 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/abed.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      667 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/ated.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1104 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/convmol.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     2791 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/copy-star.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     3669 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/create-grid.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1286 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/cut-atoms.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1226 2023-07-05 21:06:29.000000 pyfant-23.7.25.3/pyfant/scripts/cut-molecules.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     6811 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/hitran-scraper.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     3173 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/link.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      636 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/mained.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      943 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/mced.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2197 2023-07-03 22:19:58.000000 pyfant-23.7.25.3/pyfant/scripts/merge-molecules.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      703 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/mled.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      912 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/moldbed.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1848 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/nist-scraper.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     3879 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/nulbad.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      849 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/optionsed.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     2113 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/run-multi.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1152 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/run4.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2388 2023-07-24 12:50:46.000000 pyfant-23.7.25.3/pyfant/scripts/search-mollines.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2298 2023-07-05 21:06:29.000000 pyfant-23.7.25.3/pyfant/scripts/split-molecules.py
+-rwxrwxr-x   0 j         (1000) j         (1000)    10219 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/tune-zinf.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     2762 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/turbospectrum-to-atoms.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     2770 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/vald3-to-atoms.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1101 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/scripts/x.py
+-rw-rw-r--   0 j         (1000) j         (1000)    15663 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/util.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.566221 pyfant-23.7.25.3/pyfant/vis/
+-rw-rw-r--   0 j         (1000) j         (1000)       67 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/vis/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      723 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/vis/modgrid.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3073 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/vis/vismany.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8273 2020-10-12 00:16:49.000000 pyfant-23.7.25.3/pyfant/vis/vismod.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-25 20:02:06.558221 pyfant-23.7.25.3/pyfant.egg-info/
+-rw-rw-r--   0 j         (1000) j         (1000)      445 2023-07-25 20:02:06.000000 pyfant-23.7.25.3/pyfant.egg-info/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)     4194 2023-07-25 20:02:06.000000 pyfant-23.7.25.3/pyfant.egg-info/SOURCES.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2023-07-25 20:02:06.000000 pyfant-23.7.25.3/pyfant.egg-info/dependency_links.txt
+-rw-rw-r--   0 j         (1000) j         (1000)      133 2023-07-25 20:02:06.000000 pyfant-23.7.25.3/pyfant.egg-info/requires.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        7 2023-07-25 20:02:06.000000 pyfant-23.7.25.3/pyfant.egg-info/top_level.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       38 2023-07-25 20:02:06.570221 pyfant-23.7.25.3/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)     1583 2023-07-25 20:01:47.000000 pyfant-23.7.25.3/setup.py
```

### Comparing `pyfant-23.7.25.2/pyfant/__init__.py` & `pyfant-23.7.25.3/pyfant/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/_star.py` & `pyfant-23.7.25.3/pyfant/_star.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/basic/constants.py` & `pyfant-23.7.25.3/pyfant/basic/constants.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/basic/conversion.py` & `pyfant-23.7.25.3/pyfant/basic/conversion.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/basic/misc.py` & `pyfant-23.7.25.3/pyfant/basic/misc.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/basic/paths.py` & `pyfant-23.7.25.3/pyfant/basic/paths.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     Returns: list of a99.ExeInfo
     """
 
     ret = []
 
     flag_bindir = True
     try:
-        bindir = os.path.join(get_pfant_path(), "fortran", "bin")
+        bindir = os.path.join(get_pfant_path(), "fortran")
     except:
         flag_bindir = False
 
     ihpn = ["innewmarcs", "hydro2", "pfant", "nulbad"]
     if max_len is None:
         max_len = max(len(x) for x in ihpn)
```

### Comparing `pyfant-23.7.25.2/pyfant/convmol/calc_qgbd.py` & `pyfant-23.7.25.3/pyfant/convmol/calc_qgbd.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/convmol/conv.py` & `pyfant-23.7.25.3/pyfant/convmol/conv.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/convmol/conv_brooke2014.py` & `pyfant-23.7.25.3/pyfant/convmol/conv_brooke2014.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/convmol/conv_hitran.py` & `pyfant-23.7.25.3/pyfant/convmol/conv_hitran.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/convmol/conv_hitran160.py` & `pyfant-23.7.25.3/pyfant/convmol/conv_hitran160.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/convmol/conv_kurucz.py` & `pyfant-23.7.25.3/pyfant/convmol/conv_kurucz.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/convmol/conv_plez.py` & `pyfant-23.7.25.3/pyfant/convmol/conv_plez.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/convmol/conv_vald3.py` & `pyfant-23.7.25.3/pyfant/convmol/conv_vald3.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/convmol/convlog.py` & `pyfant-23.7.25.3/pyfant/convmol/convlog.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/data/default/abonds.dat` & `pyfant-23.7.25.3/pyfant/data/default/abonds.dat`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/data/default/absoru2.dat` & `pyfant-23.7.25.3/pyfant/data/default/absoru2.dat`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/data/default/abxfwhm.py` & `pyfant-23.7.25.3/pyfant/data/default/abxfwhm.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/data/default/configmolconsts.py` & `pyfant-23.7.25.3/pyfant/data/default/configmolconsts.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/data/default/dissoc.dat` & `pyfant-23.7.25.3/pyfant/data/default/dissoc.dat`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/data/default/hitrandb.sqlite` & `pyfant-23.7.25.3/pyfant/data/default/hitrandb.sqlite`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/data/default/modeles.mod` & `pyfant-23.7.25.3/pyfant/data/default/modeles.mod`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/data/default/moldb.sqlite` & `pyfant-23.7.25.3/pyfant/data/default/moldb.sqlite`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/data/default/partit.dat` & `pyfant-23.7.25.3/pyfant/data/default/partit.dat`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/downloaders/__init__.py` & `pyfant-23.7.25.3/pyfant/downloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/downloaders/downhitran.py` & `pyfant-23.7.25.3/pyfant/downloaders/downhitran.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/downloaders/downnist.py` & `pyfant-23.7.25.3/pyfant/downloaders/downnist.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/__init__.py` & `pyfant-23.7.25.3/pyfant/filetypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/fileabonds.py` & `pyfant-23.7.25.3/pyfant/filetypes/fileabonds.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/fileabxfwhm.py` & `pyfant-23.7.25.3/pyfant/filetypes/fileabxfwhm.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/fileatoms.py` & `pyfant-23.7.25.3/pyfant/filetypes/fileatoms.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filebrooke2014.py` & `pyfant-23.7.25.3/pyfant/filetypes/filebrooke2014.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filecojm1998.py` & `pyfant-23.7.25.3/pyfant/filetypes/filecojm1998.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filedissoc.py` & `pyfant-23.7.25.3/pyfant/filetypes/filedissoc.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filehitran160.py` & `pyfant-23.7.25.3/pyfant/filetypes/filehitran160.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filehitrandb.py` & `pyfant-23.7.25.3/pyfant/filetypes/filehitrandb.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filehmap.py` & `pyfant-23.7.25.3/pyfant/filetypes/filehmap.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filekuruczmol.py` & `pyfant-23.7.25.3/pyfant/filetypes/filekuruczmol.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filemain.py` & `pyfant-23.7.25.3/pyfant/filetypes/filemain.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filemod.py` & `pyfant-23.7.25.3/pyfant/filetypes/filemod.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filemolconsts.py` & `pyfant-23.7.25.3/pyfant/filetypes/filemolconsts.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filemoldb.py` & `pyfant-23.7.25.3/pyfant/filetypes/filemoldb.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filemolecules.py` & `pyfant-23.7.25.3/pyfant/filetypes/filemolecules.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filemollist.py` & `pyfant-23.7.25.3/pyfant/filetypes/filemollist.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/fileoptions.py` & `pyfant-23.7.25.3/pyfant/filetypes/fileoptions.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filepartit.py` & `pyfant-23.7.25.3/pyfant/filetypes/filepartit.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/fileplezlinelist.py` & `pyfant-23.7.25.3/pyfant/filetypes/fileplezlinelist.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filepleztio.py` & `pyfant-23.7.25.3/pyfant/filetypes/filepleztio.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filetoh.py` & `pyfant-23.7.25.3/pyfant/filetypes/filetoh.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filetraprb.py` & `pyfant-23.7.25.3/pyfant/filetypes/filetraprb.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/filevald3.py` & `pyfant-23.7.25.3/pyfant/filetypes/filevald3.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/filetypes/morespectra.py` & `pyfant-23.7.25.3/pyfant/filetypes/morespectra.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/from_turbospectrum.py` & `pyfant-23.7.25.3/pyfant/from_turbospectrum.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/from_vald.py` & `pyfant-23.7.25.3/pyfant/from_vald.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/__init__.py` & `pyfant-23.7.25.3/pyfant/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/_shared.py` & `pyfant-23.7.25.3/pyfant/gui/_shared.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WContinua.py` & `pyfant-23.7.25.3/pyfant/gui/a_WContinua.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WContinuum.py` & `pyfant-23.7.25.3/pyfant/gui/a_WContinuum.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WDBFCF.py` & `pyfant-23.7.25.3/pyfant/gui/a_WDBFCF.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WDBMolecule.py` & `pyfant-23.7.25.3/pyfant/gui/a_WDBMolecule.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WDBPFANTMol.py` & `pyfant-23.7.25.3/pyfant/gui/a_WDBPFANTMol.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WDBState.py` & `pyfant-23.7.25.3/pyfant/gui/a_WDBState.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WDBSystem.py` & `pyfant-23.7.25.3/pyfant/gui/a_WDBSystem.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WDBSystemPfantmolFCF.py` & `pyfant-23.7.25.3/pyfant/gui/a_WDBSystemPfantmolFCF.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WFileAbXFwhm.py` & `pyfant-23.7.25.3/pyfant/gui/a_WFileAbXFwhm.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WFileAbonds.py` & `pyfant-23.7.25.3/pyfant/gui/a_WFileAbonds.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WFileMain.py` & `pyfant-23.7.25.3/pyfant/gui/a_WFileMain.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WFileMolConsts.py` & `pyfant-23.7.25.3/pyfant/gui/a_WFileMolConsts.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WFileMolDB.py` & `pyfant-23.7.25.3/pyfant/gui/a_WFileMolDB.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WMolecularConstants.py` & `pyfant-23.7.25.3/pyfant/gui/a_WMolecularConstants.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_WOptionsEditor.py` & `pyfant-23.7.25.3/pyfant/gui/a_WOptionsEditor.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XAtomLinesEditor.py` & `pyfant-23.7.25.3/pyfant/gui/a_XAtomLinesEditor.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XConvMol.py` & `pyfant-23.7.25.3/pyfant/gui/a_XConvMol.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XFileAbonds.py` & `pyfant-23.7.25.3/pyfant/gui/a_XFileAbonds.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XFileAtoms.py` & `pyfant-23.7.25.3/pyfant/gui/a_XFileAtoms.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XFileAtomsHistogram.py` & `pyfant-23.7.25.3/pyfant/gui/a_XFileAtomsHistogram.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XFileMain.py` & `pyfant-23.7.25.3/pyfant/gui/a_XFileMain.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XFileMolConsts.py` & `pyfant-23.7.25.3/pyfant/gui/a_XFileMolConsts.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XFileMolDB.py` & `pyfant-23.7.25.3/pyfant/gui/a_XFileMolDB.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XFileMoleculeHistogram.py` & `pyfant-23.7.25.3/pyfant/gui/a_XFileMoleculeHistogram.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XFileMolecules.py` & `pyfant-23.7.25.3/pyfant/gui/a_XFileMolecules.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XFileOptions.py` & `pyfant-23.7.25.3/pyfant/gui/a_XFileOptions.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XMainAbonds.py` & `pyfant-23.7.25.3/pyfant/gui/a_XMainAbonds.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XMolLinesEditor.py` & `pyfant-23.7.25.3/pyfant/gui/a_XMolLinesEditor.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XMulti.py` & `pyfant-23.7.25.3/pyfant/gui/a_XMulti.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XPFANT.py` & `pyfant-23.7.25.3/pyfant/gui/a_XPFANT.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/gui/a_XRunnableManager.py` & `pyfant-23.7.25.3/pyfant/gui/a_XRunnableManager.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/kovacs.py` & `pyfant-23.7.25.3/pyfant/kovacs.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/misc/molhistogram.py` & `pyfant-23.7.25.3/pyfant/misc/molhistogram.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/molconsts.py` & `pyfant-23.7.25.3/pyfant/molconsts.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/run/conf.py` & `pyfant-23.7.25.3/pyfant/run/conf.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/run/multirunnable.py` & `pyfant-23.7.25.3/pyfant/run/multirunnable.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/run/rm.py` & `pyfant-23.7.25.3/pyfant/run/rm.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/run/runnables.py` & `pyfant-23.7.25.3/pyfant/run/runnables.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/run/traprbclass.py` & `pyfant-23.7.25.3/pyfant/run/traprbclass.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/_copy-from-sessions.py` & `pyfant-23.7.25.3/pyfant/scripts/_copy-from-sessions.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/_diff-molecules.py` & `pyfant-23.7.25.3/pyfant/scripts/_diff-molecules.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/_plot-innewmarcs-result.py` & `pyfant-23.7.25.3/pyfant/scripts/_plot-innewmarcs-result.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/_recreate-hitrandb.py` & `pyfant-23.7.25.3/pyfant/scripts/_recreate-hitrandb.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/_save-pdf.py` & `pyfant-23.7.25.3/pyfant/scripts/_save-pdf.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/abed.py` & `pyfant-23.7.25.3/pyfant/scripts/abed.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/ated.py` & `pyfant-23.7.25.3/pyfant/scripts/ated.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/convmol.py` & `pyfant-23.7.25.3/pyfant/scripts/convmol.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/copy-star.py` & `pyfant-23.7.25.3/pyfant/scripts/copy-star.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/create-grid.py` & `pyfant-23.7.25.3/pyfant/scripts/create-grid.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/cut-atoms.py` & `pyfant-23.7.25.3/pyfant/scripts/cut-atoms.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/cut-molecules.py` & `pyfant-23.7.25.3/pyfant/scripts/cut-molecules.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/hitran-scraper.py` & `pyfant-23.7.25.3/pyfant/scripts/hitran-scraper.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/link.py` & `pyfant-23.7.25.3/pyfant/scripts/link.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/mained.py` & `pyfant-23.7.25.3/pyfant/scripts/mained.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/mced.py` & `pyfant-23.7.25.3/pyfant/scripts/mced.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/merge-molecules.py` & `pyfant-23.7.25.3/pyfant/scripts/merge-molecules.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/mled.py` & `pyfant-23.7.25.3/pyfant/scripts/mled.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/moldbed.py` & `pyfant-23.7.25.3/pyfant/scripts/moldbed.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/nist-scraper.py` & `pyfant-23.7.25.3/pyfant/scripts/nist-scraper.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/nulbad.py` & `pyfant-23.7.25.3/pyfant/scripts/nulbad.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/optionsed.py` & `pyfant-23.7.25.3/pyfant/scripts/optionsed.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/run-multi.py` & `pyfant-23.7.25.3/pyfant/scripts/run-multi.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/run4.py` & `pyfant-23.7.25.3/pyfant/scripts/run4.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/search-mollines.py` & `pyfant-23.7.25.3/pyfant/scripts/search-mollines.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/split-molecules.py` & `pyfant-23.7.25.3/pyfant/scripts/split-molecules.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/tune-zinf.py` & `pyfant-23.7.25.3/pyfant/scripts/tune-zinf.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/turbospectrum-to-atoms.py` & `pyfant-23.7.25.3/pyfant/scripts/turbospectrum-to-atoms.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/vald3-to-atoms.py` & `pyfant-23.7.25.3/pyfant/scripts/vald3-to-atoms.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/scripts/x.py` & `pyfant-23.7.25.3/pyfant/scripts/x.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/util.py` & `pyfant-23.7.25.3/pyfant/util.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/vis/modgrid.py` & `pyfant-23.7.25.3/pyfant/vis/modgrid.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/vis/vismany.py` & `pyfant-23.7.25.3/pyfant/vis/vismany.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant/vis/vismod.py` & `pyfant-23.7.25.3/pyfant/vis/vismod.py`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/pyfant.egg-info/SOURCES.txt` & `pyfant-23.7.25.3/pyfant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfant-23.7.25.2/setup.py` & `pyfant-23.7.25.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 pkgs = find_packages()
 scripts = find_scripts([PACKAGE_NAME])
 
 setup(
     name=PACKAGE_NAME,
     packages=find_packages(),
     include_package_data=True,
-    version='23.7.25.2',
+    version='23.7.25.3',
     license='GNU GPLv3',
     platforms='any',
     description='Python interface to the PFANT spectral synthesis code, with a varied set of extra tools',
     author='Julio Trevisan',
     author_email='juliotrevisan@gmail.com',
     url='https://github.com/trevisanj/pyfant',
     keywords= ['astronomy', "stellar", "spectroscopy", "spectral", "synthesis",
```

