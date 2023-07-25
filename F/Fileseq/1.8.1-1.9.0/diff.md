# Comparing `tmp/Fileseq-1.8.1.zip` & `tmp/Fileseq-1.9.0.zip`

## zipinfo {}

```diff
@@ -1,162 +1,180 @@
-Zip file size: 86299 bytes, number of entries: 160
--rw-rw-r--  2.0 unx       55 b- defN 18-Jan-09 13:41 Fileseq-1.8.1/MANIFEST.in
--rw-rw-r--  2.0 unx     3580 b- defN 18-Jan-09 13:41 Fileseq-1.8.1/README.md
--rw-rw-r--  2.0 unx     1503 b- defN 19-May-15 16:39 Fileseq-1.8.1/setup.py
--rw-rw-r--  2.0 unx     5372 b- defN 19-May-15 16:39 Fileseq-1.8.1/PKG-INFO
--rw-rw-r--  2.0 unx       38 b- defN 19-May-15 16:39 Fileseq-1.8.1/setup.cfg
--rw-rw-r--  2.0 unx     9263 b- defN 19-May-13 16:19 Fileseq-1.8.1/docs/conf.py
--rw-r--r--  2.0 unx     5372 b- defN 19-May-15 16:39 Fileseq-1.8.1/src/Fileseq.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     4199 b- defN 19-May-15 16:39 Fileseq-1.8.1/src/Fileseq.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 19-May-15 16:39 Fileseq-1.8.1/src/Fileseq.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        7 b- defN 19-May-15 16:39 Fileseq-1.8.1/src/Fileseq.egg-info/requires.txt
--rw-r--r--  2.0 unx        8 b- defN 19-May-15 16:39 Fileseq-1.8.1/src/Fileseq.egg-info/top_level.txt
--rw-rw-r--  2.0 unx     1740 b- defN 19-May-15 16:30 Fileseq-1.8.1/src/fileseq/__init__.py
--rw-rw-r--  2.0 unx       22 b- defN 19-May-15 16:35 Fileseq-1.8.1/src/fileseq/__version__.py
--rw-rw-r--  2.0 unx     1412 b- defN 19-May-10 17:55 Fileseq-1.8.1/src/fileseq/constants.py
--rw-rw-r--  2.0 unx      453 b- defN 19-May-10 17:55 Fileseq-1.8.1/src/fileseq/exceptions.py
--rw-rw-r--  2.0 unx    25338 b- defN 19-May-15 16:30 Fileseq-1.8.1/src/fileseq/filesequence.py
--rw-rw-r--  2.0 unx    36882 b- defN 19-May-15 16:30 Fileseq-1.8.1/src/fileseq/frameset.py
--rw-rw-r--  2.0 unx     4482 b- defN 19-May-15 16:30 Fileseq-1.8.1/src/fileseq/utils.py
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/__init__.py
--rw-r--r--  2.0 unx      133 b- defN 19-May-13 16:22 Fileseq-1.8.1/test/__init__.pyc
--rwxrwxr-x  2.0 unx      268 b- defN 18-Mar-19 16:24 Fileseq-1.8.1/test/run.py
--rwxrwxr-x  2.0 unx    55259 b- defN 19-May-15 16:30 Fileseq-1.8.1/test/test_fuzz.py
--rw-rw-r--  2.0 unx    58531 b- defN 18-Apr-12 09:43 Fileseq-1.8.1/test/test_fuzz.pyc
--rwxrwxr-x  2.0 unx    36206 b- defN 19-May-15 16:30 Fileseq-1.8.1/test/test_unit.py
--rw-rw-r--  2.0 unx    34705 b- defN 18-Apr-12 09:43 Fileseq-1.8.1/test/test_unit.pyc
--rw-rw-r--  2.0 unx     1086 b- defN 18-Apr-12 09:43 Fileseq-1.8.1/test/utils.pyc
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/broken_seq/broke.0000.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/broken_seq/broke.0001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/broken_seq/broke.0002.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/broken_seq/broke.0004.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/broken_seq/broke.0006.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/broken_seq/broke.0007.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/broken_seq/broke.0008.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.-0001.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.-001.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.-1.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.00.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.0000.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.00000.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.00001.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.00002.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.00003.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.00004.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.00005.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.0001.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.0002.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.0003.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.0004.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.0005.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.01.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.02.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.03.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.04.ext
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.8.1/test/mixed/seq.05.ext
--rw-r--r--  2.0 unx        0 b- defN 15-Jul-24 11:07 Fileseq-1.8.1/test/seq/0001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Jul-24 11:07 Fileseq-1.8.1/test/seq/0002.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Jul-24 11:07 Fileseq-1.8.1/test/seq/0003.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/bar1000.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/bar1001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/bar1002.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/bar1004.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/bar1005.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/bar1006.exr
--rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.8.1/test/seq/baz_left.0001.exr
--rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.8.1/test/seq/baz_left.0002.exr
--rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.8.1/test/seq/baz_left.0003.exr
--rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.8.1/test/seq/baz_right.0001.exr
--rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.8.1/test/seq/baz_right.0002.exr
--rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.8.1/test/seq/baz_right.0003.exr
--rw-rw-r--  2.0 unx        0 b- defN 19-Mar-25 11:40 Fileseq-1.8.1/test/seq/big.0999.ext
--rw-rw-r--  2.0 unx        0 b- defN 19-Mar-25 11:40 Fileseq-1.8.1/test/seq/big.1000.ext
--rw-rw-r--  2.0 unx        0 b- defN 19-Mar-25 11:40 Fileseq-1.8.1/test/seq/big.1001.ext
--rw-rw-r--  2.0 unx        0 b- defN 19-Mar-25 11:40 Fileseq-1.8.1/test/seq/big.1002.ext
--rw-rw-r--  2.0 unx        0 b- defN 19-Mar-25 11:40 Fileseq-1.8.1/test/seq/big.1003.ext
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/foo.0001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/foo.0001.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/foo.0002.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/foo.0002.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/foo.0003.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/foo.0003.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/foo.0004.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/foo.0004.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/foo.0005.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seq/foo.0005.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-May-08 17:11 Fileseq-1.8.1/test/seq/foo.debug.0001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-May-08 17:11 Fileseq-1.8.1/test/seq/foo.debug.0002.exr
--rw-r--r--  2.0 unx        0 b- defN 15-May-08 17:11 Fileseq-1.8.1/test/seq/foo.debug.0003.exr
--rw-r--r--  2.0 unx        0 b- defN 15-May-08 17:11 Fileseq-1.8.1/test/seq/foo.debug.0004.exr
--rw-r--r--  2.0 unx        0 b- defN 15-May-08 17:11 Fileseq-1.8.1/test/seq/foo.debug.0005.exr
--rw-rw-r--  2.0 unx        0 b- defN 16-Mar-11 17:52 Fileseq-1.8.1/test/seq/foo_0001.exr
--rw-rw-r--  2.0 unx        0 b- defN 18-Apr-12 09:57 Fileseq-1.8.1/test/seq/foo_0001_extra.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.bar1000.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.bar1001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.bar1002.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.bar1004.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.bar1005.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.bar1006.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.foo.0001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.foo.0001.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.foo.0002.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.foo.0002.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.foo.0003.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.foo.0003.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.foo.0004.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.foo.0004.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.foo.0005.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.foo.0005.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/.hidden
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/bar1000.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/bar1001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/bar1002.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/bar1004.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/bar1005.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/bar1006.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/foo.0001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/foo.0001.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/foo.0002.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/foo.0002.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/foo.0003.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/foo.0003.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/foo.0004.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/foo.0004.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/foo.0005.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.8.1/test/seqhidden/foo.0005.jpg
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seqneg/bar.-001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seqneg/bar.0000.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/seqneg/bar.0001.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/0001.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/0002.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/0003.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/bar1000.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/bar1001.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/bar1002.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/bar1004.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/bar1005.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/bar1006.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0001.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0001.jpg
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0002.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0002.jpg
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0003.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0003.jpg
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0004.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0004.jpg
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0005.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0005.jpg
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.debug.0001.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.debug.0002.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.debug.0003.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.debug.0004.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo.debug.0005.exr
--rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.8.1/test/seqsubdirs/sub1/foo_0001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/step_seq/step1.0001.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/step_seq/step1.0005.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/step_seq/step1.0009.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/step_seq/step1.0013.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/step_seq/step1.0014.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/step_seq/step1.0015.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/step_seq/step1.0016.exr
--rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.8.1/test/step_seq/step1.0017.exr
-160 files, 285915 bytes uncompressed, 61519 bytes compressed:  78.5%
+Zip file size: 89119 bytes, number of entries: 178
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/docs/
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/src/
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/test/
+-rw-rw-r--  2.0 unx       55 b- defN 18-Jan-09 13:41 Fileseq-1.9.0/MANIFEST.in
+-rw-rw-r--  2.0 unx     2995 b- defN 20-Feb-25 15:27 Fileseq-1.9.0/README.md
+-rw-rw-r--  2.0 unx     1505 b- defN 19-Oct-08 09:15 Fileseq-1.9.0/setup.py
+-rw-rw-r--  2.0 unx     4725 b- defN 20-Feb-26 09:56 Fileseq-1.9.0/PKG-INFO
+-rw-rw-r--  2.0 unx       38 b- defN 20-Feb-26 09:56 Fileseq-1.9.0/setup.cfg
+-rw-rw-r--  2.0 unx     9258 b- defN 19-Oct-08 09:17 Fileseq-1.9.0/docs/conf.py
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/src/Fileseq.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/src/fileseq/
+-rw-r--r--  2.0 unx     4725 b- defN 20-Feb-26 09:56 Fileseq-1.9.0/src/Fileseq.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     4307 b- defN 20-Feb-26 09:56 Fileseq-1.9.0/src/Fileseq.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 20-Feb-26 09:56 Fileseq-1.9.0/src/Fileseq.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        7 b- defN 20-Feb-26 09:56 Fileseq-1.9.0/src/Fileseq.egg-info/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 20-Feb-26 09:56 Fileseq-1.9.0/src/Fileseq.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx     1798 b- defN 19-Oct-08 09:19 Fileseq-1.9.0/src/fileseq/__init__.py
+-rw-rw-r--  2.0 unx       22 b- defN 20-Feb-26 09:52 Fileseq-1.9.0/src/fileseq/__version__.py
+-rw-rw-r--  2.0 unx     2770 b- defN 20-Feb-25 16:02 Fileseq-1.9.0/src/fileseq/constants.py
+-rw-rw-r--  2.0 unx      453 b- defN 19-May-10 17:55 Fileseq-1.9.0/src/fileseq/exceptions.py
+-rw-rw-r--  2.0 unx    27370 b- defN 20-Feb-25 16:26 Fileseq-1.9.0/src/fileseq/filesequence.py
+-rw-rw-r--  2.0 unx    36882 b- defN 19-May-15 16:30 Fileseq-1.9.0/src/fileseq/frameset.py
+-rw-rw-r--  2.0 unx     4482 b- defN 19-May-15 16:30 Fileseq-1.9.0/src/fileseq/utils.py
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/test/broken_seq/
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/test/mixed/
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/test/multi_range/
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/test/seq/
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/test/seqhidden/
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/test/seqneg/
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/test/seqsubdirs/
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/test/step_seq/
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/__init__.py
+-rw-r--r--  2.0 unx      133 b- defN 19-May-13 16:22 Fileseq-1.9.0/test/__init__.pyc
+-rwxrwxr-x  2.0 unx      308 b- defN 20-Feb-25 16:02 Fileseq-1.9.0/test/run.py
+-rwxrwxr-x  2.0 unx    55259 b- defN 19-May-15 16:30 Fileseq-1.9.0/test/test_fuzz.py
+-rw-rw-r--  2.0 unx    58531 b- defN 18-Apr-12 09:43 Fileseq-1.9.0/test/test_fuzz.pyc
+-rwxrwxr-x  2.0 unx    39293 b- defN 20-Feb-25 16:26 Fileseq-1.9.0/test/test_unit.py
+-rw-rw-r--  2.0 unx    34705 b- defN 18-Apr-12 09:43 Fileseq-1.9.0/test/test_unit.pyc
+-rw-rw-r--  2.0 unx     1086 b- defN 18-Apr-12 09:43 Fileseq-1.9.0/test/utils.pyc
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/broken_seq/broke.0000.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/broken_seq/broke.0001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/broken_seq/broke.0002.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/broken_seq/broke.0004.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/broken_seq/broke.0006.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/broken_seq/broke.0007.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/broken_seq/broke.0008.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.-0001.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.-001.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.-1.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.00.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.0000.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.00000.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.00001.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.00002.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.00003.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.00004.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.00005.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.0001.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.0002.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.0003.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.0004.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.0005.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.01.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.02.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.03.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.04.ext
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:30 Fileseq-1.9.0/test/mixed/seq.05.ext
+-rw-rw-r--  2.0 unx        0 b- defN 20-Feb-25 16:26 Fileseq-1.9.0/test/multi_range/file_0003.0001.exr
+-rw-rw-r--  2.0 unx        0 b- defN 20-Feb-25 16:26 Fileseq-1.9.0/test/multi_range/file_0004.0001.exr
+-rw-rw-r--  2.0 unx        0 b- defN 20-Feb-25 16:26 Fileseq-1.9.0/test/multi_range/file_0005.0001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Jul-24 11:07 Fileseq-1.9.0/test/seq/0001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Jul-24 11:07 Fileseq-1.9.0/test/seq/0002.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Jul-24 11:07 Fileseq-1.9.0/test/seq/0003.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/bar1000.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/bar1001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/bar1002.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/bar1004.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/bar1005.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/bar1006.exr
+-rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.9.0/test/seq/baz_left.0001.exr
+-rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.9.0/test/seq/baz_left.0002.exr
+-rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.9.0/test/seq/baz_left.0003.exr
+-rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.9.0/test/seq/baz_right.0001.exr
+-rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.9.0/test/seq/baz_right.0002.exr
+-rw-rw-r--  2.0 unx        0 b- defN 18-Aug-03 13:12 Fileseq-1.9.0/test/seq/baz_right.0003.exr
+-rw-rw-r--  2.0 unx        0 b- defN 19-Mar-25 11:40 Fileseq-1.9.0/test/seq/big.0999.ext
+-rw-rw-r--  2.0 unx        0 b- defN 19-Mar-25 11:40 Fileseq-1.9.0/test/seq/big.1000.ext
+-rw-rw-r--  2.0 unx        0 b- defN 19-Mar-25 11:40 Fileseq-1.9.0/test/seq/big.1001.ext
+-rw-rw-r--  2.0 unx        0 b- defN 19-Mar-25 11:40 Fileseq-1.9.0/test/seq/big.1002.ext
+-rw-rw-r--  2.0 unx        0 b- defN 19-Mar-25 11:40 Fileseq-1.9.0/test/seq/big.1003.ext
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/foo.0001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/foo.0001.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/foo.0002.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/foo.0002.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/foo.0003.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/foo.0003.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/foo.0004.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/foo.0004.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/foo.0005.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seq/foo.0005.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-May-08 17:11 Fileseq-1.9.0/test/seq/foo.debug.0001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-May-08 17:11 Fileseq-1.9.0/test/seq/foo.debug.0002.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-May-08 17:11 Fileseq-1.9.0/test/seq/foo.debug.0003.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-May-08 17:11 Fileseq-1.9.0/test/seq/foo.debug.0004.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-May-08 17:11 Fileseq-1.9.0/test/seq/foo.debug.0005.exr
+-rw-rw-r--  2.0 unx        0 b- defN 16-Mar-11 17:52 Fileseq-1.9.0/test/seq/foo_0001.exr
+-rw-rw-r--  2.0 unx        0 b- defN 18-Apr-12 09:57 Fileseq-1.9.0/test/seq/foo_0001_extra.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.bar1000.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.bar1001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.bar1002.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.bar1004.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.bar1005.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.bar1006.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.foo.0001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.foo.0001.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.foo.0002.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.foo.0002.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.foo.0003.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.foo.0003.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.foo.0004.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.foo.0004.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.foo.0005.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.foo.0005.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/.hidden
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/bar1000.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/bar1001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/bar1002.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/bar1004.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/bar1005.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/bar1006.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/foo.0001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/foo.0001.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/foo.0002.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/foo.0002.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/foo.0003.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/foo.0003.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/foo.0004.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/foo.0004.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/foo.0005.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-28 15:18 Fileseq-1.9.0/test/seqhidden/foo.0005.jpg
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seqneg/bar.-001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seqneg/bar.0000.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/seqneg/bar.0001.exr
+drwxrwxr-x  2.0 unx        0 b- stor 20-Feb-26 09:56 Fileseq-1.9.0/test/seqsubdirs/sub1/
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/0001.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/0002.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/0003.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/bar1000.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/bar1001.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/bar1002.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/bar1004.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/bar1005.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/bar1006.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0001.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0001.jpg
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0002.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0002.jpg
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0003.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0003.jpg
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0004.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0004.jpg
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0005.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0005.jpg
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.debug.0001.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.debug.0002.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.debug.0003.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.debug.0004.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo.debug.0005.exr
+-rw-rw-r--  2.0 unx        0 b- defN 17-Jul-19 15:22 Fileseq-1.9.0/test/seqsubdirs/sub1/foo_0001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/step_seq/step1.0001.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/step_seq/step1.0005.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/step_seq/step1.0009.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/step_seq/step1.0013.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/step_seq/step1.0014.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/step_seq/step1.0015.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/step_seq/step1.0016.exr
+-rw-r--r--  2.0 unx        0 b- defN 15-Apr-20 13:13 Fileseq-1.9.0/test/step_seq/step1.0017.exr
+178 files, 290716 bytes uncompressed, 61901 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -1,481 +1,535 @@
-Filename: Fileseq-1.8.1/MANIFEST.in
+Filename: Fileseq-1.9.0/
 Comment: 
 
-Filename: Fileseq-1.8.1/README.md
+Filename: Fileseq-1.9.0/docs/
 Comment: 
 
-Filename: Fileseq-1.8.1/setup.py
+Filename: Fileseq-1.9.0/src/
 Comment: 
 
-Filename: Fileseq-1.8.1/PKG-INFO
+Filename: Fileseq-1.9.0/test/
 Comment: 
 
-Filename: Fileseq-1.8.1/setup.cfg
+Filename: Fileseq-1.9.0/MANIFEST.in
 Comment: 
 
-Filename: Fileseq-1.8.1/docs/conf.py
+Filename: Fileseq-1.9.0/README.md
 Comment: 
 
-Filename: Fileseq-1.8.1/src/Fileseq.egg-info/PKG-INFO
+Filename: Fileseq-1.9.0/setup.py
 Comment: 
 
-Filename: Fileseq-1.8.1/src/Fileseq.egg-info/SOURCES.txt
+Filename: Fileseq-1.9.0/PKG-INFO
 Comment: 
 
-Filename: Fileseq-1.8.1/src/Fileseq.egg-info/dependency_links.txt
+Filename: Fileseq-1.9.0/setup.cfg
 Comment: 
 
-Filename: Fileseq-1.8.1/src/Fileseq.egg-info/requires.txt
+Filename: Fileseq-1.9.0/docs/conf.py
 Comment: 
 
-Filename: Fileseq-1.8.1/src/Fileseq.egg-info/top_level.txt
+Filename: Fileseq-1.9.0/src/Fileseq.egg-info/
 Comment: 
 
-Filename: Fileseq-1.8.1/src/fileseq/__init__.py
+Filename: Fileseq-1.9.0/src/fileseq/
 Comment: 
 
-Filename: Fileseq-1.8.1/src/fileseq/__version__.py
+Filename: Fileseq-1.9.0/src/Fileseq.egg-info/PKG-INFO
 Comment: 
 
-Filename: Fileseq-1.8.1/src/fileseq/constants.py
+Filename: Fileseq-1.9.0/src/Fileseq.egg-info/SOURCES.txt
 Comment: 
 
-Filename: Fileseq-1.8.1/src/fileseq/exceptions.py
+Filename: Fileseq-1.9.0/src/Fileseq.egg-info/dependency_links.txt
 Comment: 
 
-Filename: Fileseq-1.8.1/src/fileseq/filesequence.py
+Filename: Fileseq-1.9.0/src/Fileseq.egg-info/requires.txt
 Comment: 
 
-Filename: Fileseq-1.8.1/src/fileseq/frameset.py
+Filename: Fileseq-1.9.0/src/Fileseq.egg-info/top_level.txt
 Comment: 
 
-Filename: Fileseq-1.8.1/src/fileseq/utils.py
+Filename: Fileseq-1.9.0/src/fileseq/__init__.py
 Comment: 
 
-Filename: Fileseq-1.8.1/test/__init__.py
+Filename: Fileseq-1.9.0/src/fileseq/__version__.py
 Comment: 
 
-Filename: Fileseq-1.8.1/test/__init__.pyc
+Filename: Fileseq-1.9.0/src/fileseq/constants.py
 Comment: 
 
-Filename: Fileseq-1.8.1/test/run.py
+Filename: Fileseq-1.9.0/src/fileseq/exceptions.py
 Comment: 
 
-Filename: Fileseq-1.8.1/test/test_fuzz.py
+Filename: Fileseq-1.9.0/src/fileseq/filesequence.py
 Comment: 
 
-Filename: Fileseq-1.8.1/test/test_fuzz.pyc
+Filename: Fileseq-1.9.0/src/fileseq/frameset.py
 Comment: 
 
-Filename: Fileseq-1.8.1/test/test_unit.py
+Filename: Fileseq-1.9.0/src/fileseq/utils.py
 Comment: 
 
-Filename: Fileseq-1.8.1/test/test_unit.pyc
+Filename: Fileseq-1.9.0/test/broken_seq/
 Comment: 
 
-Filename: Fileseq-1.8.1/test/utils.pyc
+Filename: Fileseq-1.9.0/test/mixed/
 Comment: 
 
-Filename: Fileseq-1.8.1/test/broken_seq/broke.0000.exr
+Filename: Fileseq-1.9.0/test/multi_range/
 Comment: 
 
-Filename: Fileseq-1.8.1/test/broken_seq/broke.0001.exr
+Filename: Fileseq-1.9.0/test/seq/
 Comment: 
 
-Filename: Fileseq-1.8.1/test/broken_seq/broke.0002.exr
+Filename: Fileseq-1.9.0/test/seqhidden/
 Comment: 
 
-Filename: Fileseq-1.8.1/test/broken_seq/broke.0004.exr
+Filename: Fileseq-1.9.0/test/seqneg/
 Comment: 
 
-Filename: Fileseq-1.8.1/test/broken_seq/broke.0006.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/
 Comment: 
 
-Filename: Fileseq-1.8.1/test/broken_seq/broke.0007.exr
+Filename: Fileseq-1.9.0/test/step_seq/
 Comment: 
 
-Filename: Fileseq-1.8.1/test/broken_seq/broke.0008.exr
+Filename: Fileseq-1.9.0/test/__init__.py
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.-0001.ext
+Filename: Fileseq-1.9.0/test/__init__.pyc
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.-001.ext
+Filename: Fileseq-1.9.0/test/run.py
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.-1.ext
+Filename: Fileseq-1.9.0/test/test_fuzz.py
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.00.ext
+Filename: Fileseq-1.9.0/test/test_fuzz.pyc
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.0000.ext
+Filename: Fileseq-1.9.0/test/test_unit.py
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.00000.ext
+Filename: Fileseq-1.9.0/test/test_unit.pyc
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.00001.ext
+Filename: Fileseq-1.9.0/test/utils.pyc
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.00002.ext
+Filename: Fileseq-1.9.0/test/broken_seq/broke.0000.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.00003.ext
+Filename: Fileseq-1.9.0/test/broken_seq/broke.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.00004.ext
+Filename: Fileseq-1.9.0/test/broken_seq/broke.0002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.00005.ext
+Filename: Fileseq-1.9.0/test/broken_seq/broke.0004.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.0001.ext
+Filename: Fileseq-1.9.0/test/broken_seq/broke.0006.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.0002.ext
+Filename: Fileseq-1.9.0/test/broken_seq/broke.0007.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.0003.ext
+Filename: Fileseq-1.9.0/test/broken_seq/broke.0008.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.0004.ext
+Filename: Fileseq-1.9.0/test/mixed/seq.-0001.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.0005.ext
+Filename: Fileseq-1.9.0/test/mixed/seq.-001.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.01.ext
+Filename: Fileseq-1.9.0/test/mixed/seq.-1.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.02.ext
+Filename: Fileseq-1.9.0/test/mixed/seq.00.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.03.ext
+Filename: Fileseq-1.9.0/test/mixed/seq.0000.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.04.ext
+Filename: Fileseq-1.9.0/test/mixed/seq.00000.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/mixed/seq.05.ext
+Filename: Fileseq-1.9.0/test/mixed/seq.00001.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/0001.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.00002.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/0002.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.00003.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/0003.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.00004.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/bar1000.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.00005.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/bar1001.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.0001.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/bar1002.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.0002.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/bar1004.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.0003.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/bar1005.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.0004.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/bar1006.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.0005.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/baz_left.0001.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.01.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/baz_left.0002.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.02.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/baz_left.0003.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.03.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/baz_right.0001.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.04.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/baz_right.0002.exr
+Filename: Fileseq-1.9.0/test/mixed/seq.05.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/baz_right.0003.exr
+Filename: Fileseq-1.9.0/test/multi_range/file_0003.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/big.0999.ext
+Filename: Fileseq-1.9.0/test/multi_range/file_0004.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/big.1000.ext
+Filename: Fileseq-1.9.0/test/multi_range/file_0005.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/big.1001.ext
+Filename: Fileseq-1.9.0/test/seq/0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/big.1002.ext
+Filename: Fileseq-1.9.0/test/seq/0002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/big.1003.ext
+Filename: Fileseq-1.9.0/test/seq/0003.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.0001.exr
+Filename: Fileseq-1.9.0/test/seq/bar1000.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.0001.jpg
+Filename: Fileseq-1.9.0/test/seq/bar1001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.0002.exr
+Filename: Fileseq-1.9.0/test/seq/bar1002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.0002.jpg
+Filename: Fileseq-1.9.0/test/seq/bar1004.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.0003.exr
+Filename: Fileseq-1.9.0/test/seq/bar1005.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.0003.jpg
+Filename: Fileseq-1.9.0/test/seq/bar1006.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.0004.exr
+Filename: Fileseq-1.9.0/test/seq/baz_left.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.0004.jpg
+Filename: Fileseq-1.9.0/test/seq/baz_left.0002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.0005.exr
+Filename: Fileseq-1.9.0/test/seq/baz_left.0003.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.0005.jpg
+Filename: Fileseq-1.9.0/test/seq/baz_right.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.debug.0001.exr
+Filename: Fileseq-1.9.0/test/seq/baz_right.0002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.debug.0002.exr
+Filename: Fileseq-1.9.0/test/seq/baz_right.0003.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.debug.0003.exr
+Filename: Fileseq-1.9.0/test/seq/big.0999.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.debug.0004.exr
+Filename: Fileseq-1.9.0/test/seq/big.1000.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo.debug.0005.exr
+Filename: Fileseq-1.9.0/test/seq/big.1001.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo_0001.exr
+Filename: Fileseq-1.9.0/test/seq/big.1002.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seq/foo_0001_extra.exr
+Filename: Fileseq-1.9.0/test/seq/big.1003.ext
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.bar1000.exr
+Filename: Fileseq-1.9.0/test/seq/foo.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.bar1001.exr
+Filename: Fileseq-1.9.0/test/seq/foo.0001.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.bar1002.exr
+Filename: Fileseq-1.9.0/test/seq/foo.0002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.bar1004.exr
+Filename: Fileseq-1.9.0/test/seq/foo.0002.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.bar1005.exr
+Filename: Fileseq-1.9.0/test/seq/foo.0003.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.bar1006.exr
+Filename: Fileseq-1.9.0/test/seq/foo.0003.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.foo.0001.exr
+Filename: Fileseq-1.9.0/test/seq/foo.0004.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.foo.0001.jpg
+Filename: Fileseq-1.9.0/test/seq/foo.0004.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.foo.0002.exr
+Filename: Fileseq-1.9.0/test/seq/foo.0005.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.foo.0002.jpg
+Filename: Fileseq-1.9.0/test/seq/foo.0005.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.foo.0003.exr
+Filename: Fileseq-1.9.0/test/seq/foo.debug.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.foo.0003.jpg
+Filename: Fileseq-1.9.0/test/seq/foo.debug.0002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.foo.0004.exr
+Filename: Fileseq-1.9.0/test/seq/foo.debug.0003.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.foo.0004.jpg
+Filename: Fileseq-1.9.0/test/seq/foo.debug.0004.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.foo.0005.exr
+Filename: Fileseq-1.9.0/test/seq/foo.debug.0005.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.foo.0005.jpg
+Filename: Fileseq-1.9.0/test/seq/foo_0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/.hidden
+Filename: Fileseq-1.9.0/test/seq/foo_0001_extra.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/bar1000.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.bar1000.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/bar1001.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.bar1001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/bar1002.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.bar1002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/bar1004.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.bar1004.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/bar1005.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.bar1005.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/bar1006.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.bar1006.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/foo.0001.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.foo.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/foo.0001.jpg
+Filename: Fileseq-1.9.0/test/seqhidden/.foo.0001.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/foo.0002.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.foo.0002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/foo.0002.jpg
+Filename: Fileseq-1.9.0/test/seqhidden/.foo.0002.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/foo.0003.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.foo.0003.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/foo.0003.jpg
+Filename: Fileseq-1.9.0/test/seqhidden/.foo.0003.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/foo.0004.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.foo.0004.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/foo.0004.jpg
+Filename: Fileseq-1.9.0/test/seqhidden/.foo.0004.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/foo.0005.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.foo.0005.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqhidden/foo.0005.jpg
+Filename: Fileseq-1.9.0/test/seqhidden/.foo.0005.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqneg/bar.-001.exr
+Filename: Fileseq-1.9.0/test/seqhidden/.hidden
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqneg/bar.0000.exr
+Filename: Fileseq-1.9.0/test/seqhidden/bar1000.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqneg/bar.0001.exr
+Filename: Fileseq-1.9.0/test/seqhidden/bar1001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/0001.exr
+Filename: Fileseq-1.9.0/test/seqhidden/bar1002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/0002.exr
+Filename: Fileseq-1.9.0/test/seqhidden/bar1004.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/0003.exr
+Filename: Fileseq-1.9.0/test/seqhidden/bar1005.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/bar1000.exr
+Filename: Fileseq-1.9.0/test/seqhidden/bar1006.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/bar1001.exr
+Filename: Fileseq-1.9.0/test/seqhidden/foo.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/bar1002.exr
+Filename: Fileseq-1.9.0/test/seqhidden/foo.0001.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/bar1004.exr
+Filename: Fileseq-1.9.0/test/seqhidden/foo.0002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/bar1005.exr
+Filename: Fileseq-1.9.0/test/seqhidden/foo.0002.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/bar1006.exr
+Filename: Fileseq-1.9.0/test/seqhidden/foo.0003.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0001.exr
+Filename: Fileseq-1.9.0/test/seqhidden/foo.0003.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0001.jpg
+Filename: Fileseq-1.9.0/test/seqhidden/foo.0004.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0002.exr
+Filename: Fileseq-1.9.0/test/seqhidden/foo.0004.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0002.jpg
+Filename: Fileseq-1.9.0/test/seqhidden/foo.0005.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0003.exr
+Filename: Fileseq-1.9.0/test/seqhidden/foo.0005.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0003.jpg
+Filename: Fileseq-1.9.0/test/seqneg/bar.-001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0004.exr
+Filename: Fileseq-1.9.0/test/seqneg/bar.0000.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0004.jpg
+Filename: Fileseq-1.9.0/test/seqneg/bar.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0005.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.0005.jpg
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.debug.0001.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/0002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.debug.0002.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/0003.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.debug.0003.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/bar1000.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.debug.0004.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/bar1001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo.debug.0005.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/bar1002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/seqsubdirs/sub1/foo_0001.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/bar1004.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/step_seq/step1.0001.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/bar1005.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/step_seq/step1.0005.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/bar1006.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/step_seq/step1.0009.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0001.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/step_seq/step1.0013.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0001.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/step_seq/step1.0014.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0002.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/step_seq/step1.0015.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0002.jpg
 Comment: 
 
-Filename: Fileseq-1.8.1/test/step_seq/step1.0016.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0003.exr
 Comment: 
 
-Filename: Fileseq-1.8.1/test/step_seq/step1.0017.exr
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0003.jpg
+Comment: 
+
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0004.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0004.jpg
+Comment: 
+
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0005.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.0005.jpg
+Comment: 
+
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.debug.0001.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.debug.0002.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.debug.0003.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.debug.0004.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo.debug.0005.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/seqsubdirs/sub1/foo_0001.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/step_seq/step1.0001.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/step_seq/step1.0005.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/step_seq/step1.0009.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/step_seq/step1.0013.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/step_seq/step1.0014.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/step_seq/step1.0015.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/step_seq/step1.0016.exr
+Comment: 
+
+Filename: Fileseq-1.9.0/test/step_seq/step1.0017.exr
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `Fileseq-1.8.1/README.md` & `Fileseq-1.9.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# Fileseq [![Documentation Status](https://readthedocs.org/projects/fileseq/badge/?version=latest)](http://fileseq.readthedocs.io/en/latest/) [![Travis Build Status](https://api.travis-ci.org/sqlboy/fileseq.svg)](https://travis-ci.org/sqlboy/fileseq) [![AppVeyor Build status](https://ci.appveyor.com/api/projects/status/87t3pycl3365lnkd?svg=true)](https://ci.appveyor.com/project/justinfx/fileseq)
+# ![Fileseq](docs/_static/fileseq_large.png) 
 
+[![Documentation Status](https://readthedocs.org/projects/fileseq/badge/?version=latest)](http://fileseq.readthedocs.io/en/latest/) [![Travis Build Status](https://api.travis-ci.org/justinfx/fileseq.svg)](https://travis-ci.org/justinfx/fileseq) [![AppVeyor Build status](https://ci.appveyor.com/api/projects/status/87t3pycl3365lnkd?svg=true)](https://ci.appveyor.com/project/justinfx/fileseq)
 
 A Python library for parsing frame ranges and file sequences based on a similar library found in Katana.
 
 ## Frame Range Shorthand
 
 Support for:
 
@@ -11,14 +12,15 @@
 * Comma Delimited: 1-10,10-20
 * Chunked: 1-100x5
 * Filled: 1-100y5
 * Staggered: 1-100:3 (1-100x3, 1-100x2, 1-100)
 * Negative frame numbers: -10-100
 * Padding: #=4 padded, @=single pad
 * Printf Syntax Padding: %04d=4 padded, %01d=1 padded
+* Houdini Syntax Padding: $F4=4 padding, $F=1 padded
 
 ## FrameSets
 
 A FrameSet wraps a sequence of frames in a list list container.
 
 ### Iterate a FrameSet
 ```python
@@ -106,21 +108,11 @@
 fileseq.findSequenceOnDisk('/foo/bar.@@@@@.exr')
 ```
 No: 
 ```python
 fileseq.findSequenceOnDisk('/foo/bar.*.exr')
 ```
 
-## Changes in versions >= 1.0.0
+## Language Ports
 
-From version 1.0.0, a FrameSet allows all the normal Set operations.  It is now an immutable and
-hashable object in its own right, as well.  This means that the order and contents are immutable
-values internally (a tuple and a frozenset, respectively), and that the FrameSet itself can be
-used as a key in a dictionary.
-
-This also means that the null FrameSet (FrameSet('')) is a valid object, and something you should
-expect to receive back from any Set operations that would result in an empty return value.  This
-brings the caveat that the FrameSet.start and FrameSet.end methods on a null FrameSet will raise an
-IndexError if called.
-
-To help avoid confusion, a FrameSet.is_null attribute has been added in 1.0.1, which you can check 
-before calling those methods.
+* Go: https://github.com/justinfx/gofileseq
+* C++: https://github.com/justinfx/gofileseq/tree/master/cpp
```

## Comparing `Fileseq-1.8.1/setup.py` & `Fileseq-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
       author='Matt Chambers',
       author_email='yougotrooted@gmail.com',
 
       maintainer='Justin Israel',
       maintainer_email='justinisrael@gmail.com',
 
-      url='https://github.com/sqlboy/fileseq',
+      url='https://github.com/justinfx/fileseq',
 
       description=descript,
       long_description=long_description,
       long_description_content_type="text/markdown",
 
       license='MIT',
```

## Comparing `Fileseq-1.8.1/PKG-INFO` & `Fileseq-1.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: Fileseq
-Version: 1.8.1
+Version: 1.9.0
 Summary: A Python library for parsing frame ranges and file sequences based on a similar library found in Katana.
-Home-page: https://github.com/sqlboy/fileseq
+Home-page: https://github.com/justinfx/fileseq
 Author: Matt Chambers
 Author-email: yougotrooted@gmail.com
 Maintainer: Justin Israel
 Maintainer-email: justinisrael@gmail.com
 License: MIT
-Description: # Fileseq [![Documentation Status](https://readthedocs.org/projects/fileseq/badge/?version=latest)](http://fileseq.readthedocs.io/en/latest/) [![Travis Build Status](https://api.travis-ci.org/sqlboy/fileseq.svg)](https://travis-ci.org/sqlboy/fileseq) [![AppVeyor Build status](https://ci.appveyor.com/api/projects/status/87t3pycl3365lnkd?svg=true)](https://ci.appveyor.com/project/justinfx/fileseq)
+Description: # ![Fileseq](docs/_static/fileseq_large.png) 
         
+        [![Documentation Status](https://readthedocs.org/projects/fileseq/badge/?version=latest)](http://fileseq.readthedocs.io/en/latest/) [![Travis Build Status](https://api.travis-ci.org/justinfx/fileseq.svg)](https://travis-ci.org/justinfx/fileseq) [![AppVeyor Build status](https://ci.appveyor.com/api/projects/status/87t3pycl3365lnkd?svg=true)](https://ci.appveyor.com/project/justinfx/fileseq)
         
         A Python library for parsing frame ranges and file sequences based on a similar library found in Katana.
         
         ## Frame Range Shorthand
         
         Support for:
         
@@ -21,14 +22,15 @@
         * Comma Delimited: 1-10,10-20
         * Chunked: 1-100x5
         * Filled: 1-100y5
         * Staggered: 1-100:3 (1-100x3, 1-100x2, 1-100)
         * Negative frame numbers: -10-100
         * Padding: #=4 padded, @=single pad
         * Printf Syntax Padding: %04d=4 padded, %01d=1 padded
+        * Houdini Syntax Padding: $F4=4 padding, $F=1 padded
         
         ## FrameSets
         
         A FrameSet wraps a sequence of frames in a list list container.
         
         ### Iterate a FrameSet
         ```python
@@ -116,28 +118,18 @@
         fileseq.findSequenceOnDisk('/foo/bar.@@@@@.exr')
         ```
         No: 
         ```python
         fileseq.findSequenceOnDisk('/foo/bar.*.exr')
         ```
         
-        ## Changes in versions >= 1.0.0
+        ## Language Ports
         
-        From version 1.0.0, a FrameSet allows all the normal Set operations.  It is now an immutable and
-        hashable object in its own right, as well.  This means that the order and contents are immutable
-        values internally (a tuple and a frozenset, respectively), and that the FrameSet itself can be
-        used as a key in a dictionary.
-        
-        This also means that the null FrameSet (FrameSet('')) is a valid object, and something you should
-        expect to receive back from any Set operations that would result in an empty return value.  This
-        brings the caveat that the FrameSet.start and FrameSet.end methods on a null FrameSet will raise an
-        IndexError if called.
-        
-        To help avoid confusion, a FrameSet.is_null attribute has been added in 1.0.1, which you can check 
-        before calling those methods.
+        * Go: https://github.com/justinfx/gofileseq
+        * C++: https://github.com/justinfx/gofileseq/tree/master/cpp
         
 Keywords: vfx visual effects file sequence frames image
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

## Comparing `Fileseq-1.8.1/docs/conf.py` & `Fileseq-1.9.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'Fileseq'
-copyright = u'2015-%d, Matthew Chambers' % datetime.datetime.now().year
+copyright = u'2015, Justin Israel'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = __version__
@@ -125,20 +125,20 @@
 #html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 #html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+html_logo = "_static/fileseq_vertical.png"
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+html_favicon = "_static/fileseq.ico"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
@@ -221,15 +221,15 @@
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
   ('index', 'Fileseq.tex', u'Fileseq Documentation',
-   u'Matthew Chambers', 'manual'),
+   u'Justin Israel', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -251,29 +251,29 @@
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     ('index', 'fileseq', u'Fileseq Documentation',
-     [u'Matthew Chambers'], 1)
+     [u'Justin Israel'], 1)
 ]
 
 # If true, show URL addresses after external links.
 #man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
   ('index', 'Fileseq', u'Fileseq Documentation',
-   u'Matthew Chambers', 'Fileseq', 'One line description of project.',
+   u'Justin Israel', 'Fileseq', 'One line description of project.',
    'Miscellaneous'),
 ]
 
 # Documents to append as an appendix to all manuals.
 #texinfo_appendices = []
 
 # If false, no module index is generated.
```

## Comparing `Fileseq-1.8.1/src/Fileseq.egg-info/PKG-INFO` & `Fileseq-1.9.0/src/Fileseq.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: Fileseq
-Version: 1.8.1
+Version: 1.9.0
 Summary: A Python library for parsing frame ranges and file sequences based on a similar library found in Katana.
-Home-page: https://github.com/sqlboy/fileseq
+Home-page: https://github.com/justinfx/fileseq
 Author: Matt Chambers
 Author-email: yougotrooted@gmail.com
 Maintainer: Justin Israel
 Maintainer-email: justinisrael@gmail.com
 License: MIT
-Description: # Fileseq [![Documentation Status](https://readthedocs.org/projects/fileseq/badge/?version=latest)](http://fileseq.readthedocs.io/en/latest/) [![Travis Build Status](https://api.travis-ci.org/sqlboy/fileseq.svg)](https://travis-ci.org/sqlboy/fileseq) [![AppVeyor Build status](https://ci.appveyor.com/api/projects/status/87t3pycl3365lnkd?svg=true)](https://ci.appveyor.com/project/justinfx/fileseq)
+Description: # ![Fileseq](docs/_static/fileseq_large.png) 
         
+        [![Documentation Status](https://readthedocs.org/projects/fileseq/badge/?version=latest)](http://fileseq.readthedocs.io/en/latest/) [![Travis Build Status](https://api.travis-ci.org/justinfx/fileseq.svg)](https://travis-ci.org/justinfx/fileseq) [![AppVeyor Build status](https://ci.appveyor.com/api/projects/status/87t3pycl3365lnkd?svg=true)](https://ci.appveyor.com/project/justinfx/fileseq)
         
         A Python library for parsing frame ranges and file sequences based on a similar library found in Katana.
         
         ## Frame Range Shorthand
         
         Support for:
         
@@ -21,14 +22,15 @@
         * Comma Delimited: 1-10,10-20
         * Chunked: 1-100x5
         * Filled: 1-100y5
         * Staggered: 1-100:3 (1-100x3, 1-100x2, 1-100)
         * Negative frame numbers: -10-100
         * Padding: #=4 padded, @=single pad
         * Printf Syntax Padding: %04d=4 padded, %01d=1 padded
+        * Houdini Syntax Padding: $F4=4 padding, $F=1 padded
         
         ## FrameSets
         
         A FrameSet wraps a sequence of frames in a list list container.
         
         ### Iterate a FrameSet
         ```python
@@ -116,28 +118,18 @@
         fileseq.findSequenceOnDisk('/foo/bar.@@@@@.exr')
         ```
         No: 
         ```python
         fileseq.findSequenceOnDisk('/foo/bar.*.exr')
         ```
         
-        ## Changes in versions >= 1.0.0
+        ## Language Ports
         
-        From version 1.0.0, a FrameSet allows all the normal Set operations.  It is now an immutable and
-        hashable object in its own right, as well.  This means that the order and contents are immutable
-        values internally (a tuple and a frozenset, respectively), and that the FrameSet itself can be
-        used as a key in a dictionary.
-        
-        This also means that the null FrameSet (FrameSet('')) is a valid object, and something you should
-        expect to receive back from any Set operations that would result in an empty return value.  This
-        brings the caveat that the FrameSet.start and FrameSet.end methods on a null FrameSet will raise an
-        IndexError if called.
-        
-        To help avoid confusion, a FrameSet.is_null attribute has been added in 1.0.1, which you can check 
-        before calling those methods.
+        * Go: https://github.com/justinfx/gofileseq
+        * C++: https://github.com/justinfx/gofileseq/tree/master/cpp
         
 Keywords: vfx visual effects file sequence frames image
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

## Comparing `Fileseq-1.8.1/src/Fileseq.egg-info/SOURCES.txt` & `Fileseq-1.9.0/src/Fileseq.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 test/mixed/seq.0004.ext
 test/mixed/seq.0005.ext
 test/mixed/seq.01.ext
 test/mixed/seq.02.ext
 test/mixed/seq.03.ext
 test/mixed/seq.04.ext
 test/mixed/seq.05.ext
+test/multi_range/file_0003.0001.exr
+test/multi_range/file_0004.0001.exr
+test/multi_range/file_0005.0001.exr
 test/seq/0001.exr
 test/seq/0002.exr
 test/seq/0003.exr
 test/seq/bar1000.exr
 test/seq/bar1001.exr
 test/seq/bar1002.exr
 test/seq/bar1004.exr
```

## Comparing `Fileseq-1.8.1/src/fileseq/__init__.py` & `Fileseq-1.9.0/src/fileseq/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 fileseq - A simple python library for parsing file sequence strings commonly
 used in VFX and Animation applications.
 
 The MIT License (MIT)
 
-Copyright (c) 2015 Matthew Chambers
+Original work Copyright (c) 2015 Matthew Chambers
+
+Modified work Copyright 2015 Justin Israel
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `Fileseq-1.8.1/src/fileseq/filesequence.py` & `Fileseq-1.9.0/src/fileseq/filesequence.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 import re
 import functools
 from glob import iglob
 
 from fileseq.exceptions import ParseException, FileSeqException
-from fileseq.constants import PAD_MAP, DISK_RE, SPLIT_RE, PRINTF_SYNTAX_PADDING_RE
+from fileseq.constants import PAD_MAP, DISK_RE, SPLIT_RE, PRINTF_SYNTAX_PADDING_RE, HOUDINI_SYNTAX_PADDING_RE
 from fileseq.frameset import FrameSet
 from fileseq import utils
 
 
 class FileSequence(object):
     """:class:`FileSequence` represents an ordered sequence of files.
 
@@ -473,47 +473,91 @@
 
     def __eq__(self, other):
         return str(self) == str(other)
 
     def __ne__(self, other):
         return str(self) != str(other)
 
+    def __hash__(self):
+        # TODO: Technically we should be returning None,
+        # as this class is mutable and cannot reliably be hashed.
+        # Python2 allows it without this definition.
+        # Python3 fails with TypeError: unhashable.
+        # For now, preserving the hashing behaviour in py3.
+        return id(self)
+
     @staticmethod
-    def yield_sequences_in_list(paths):
+    def yield_sequences_in_list(paths, using=None):
         """
         Yield the discrete sequences within paths.  This does not try to
         determine if the files actually exist on disk, it assumes you already
         know that.
 
+        A template :obj:`FileSequence` object can also be provided via the
+        ``using`` parameter. Given this template, the dirname, basename, and
+        extension values will be used to extract the frame value from the paths
+        instead of parsing each path from scratch.
+
+        Examples:
+            The ``using`` field can supply a template for extracting the frame
+            component from the paths::
+
+                paths = [
+                    '/dir/file_001.0001.ext',
+                    '/dir/file_002.0001.ext',
+                    '/dir/file_003.0001.ext',
+                ]
+                template = FileSequence('/dir/file_#.0001.ext')
+                seqs = FileSequence.yield_sequences_in_list(paths, using)
+                # [<FileSequence: '/dir/file_1-3@@@.0001.ext'>]
+
         Args:
             paths (list[str]): a list of paths
+            using (:obj:`FileSequence`): Optional sequence to use as template
 
         Yields:
             :obj:`FileSequence`:
         """
         seqs = {}
         _check = DISK_RE.match
 
-        for match in filter(None, map(_check, map(utils.asString, paths))):
-            dirname, basename, frame, ext = match.groups()
-            if not basename and not ext:
-                continue
-            key = (dirname, basename, ext)
-            seqs.setdefault(key, set())
-            if frame:
-                seqs[key].add(frame)
+        using_template = isinstance(using, FileSequence)
+
+        if using_template:
+            key = dirname, basename, ext = using.dirname(), using.basename(), using.extension()
+            head = len(dirname + basename)
+            tail = -len(ext)
+            frames = set()
+
+            for path in filter(None, map(utils.asString, paths)):
+                frame = path[head:tail]
+                try:
+                    int(frame)
+                except ValueError:
+                    continue
+                seqs.setdefault(key, frames).add(frame)
+
+        else:
+            for match in filter(None, map(_check, map(utils.asString, paths))):
+                dirname, basename, frame, ext = match.groups()
+                if not basename and not ext:
+                    continue
+                key = (dirname, basename, ext)
+                seqs.setdefault(key, set())
+                if frame:
+                    seqs[key].add(frame)
 
         for (dirname, basename, ext), frames in iteritems(seqs):
             # build the FileSequence behind the scenes, rather than dupe work
             seq = FileSequence.__new__(FileSequence)
             seq._dir = dirname or ''
             seq._base = basename or ''
             seq._ext = ext or ''
             if frames:
-                seq._frameSet = FrameSet(set(map(int, frames))) if frames else None
+                seq._frameSet = FrameSet({int(f) for f in frames}) if frames else None
                 seq._pad = FileSequence.getPaddingChars(min(map(len, frames)))
             else:
                 seq._frameSet = None
                 seq._pad = ''
             seq.__init__(utils.asString(seq))
             yield seq
 
@@ -686,15 +730,15 @@
         pad = seq.padding()
 
         globbed = iglob(patt)
         if pad and strictPadding:
             globbed = cls._filterByPaddingNum(globbed, seq.zfill())
             pad = cls.conformPadding(pad)
 
-        matches = cls.yield_sequences_in_list(globbed)
+        matches = cls.yield_sequences_in_list(globbed, using=seq)
         for match in matches:
             if match.basename() == basename and match.extension() == ext:
                 if pad and strictPadding:
                     match.setPadding(pad)
                 return match
 
         msg = 'no sequence found on disk matching {0}'
@@ -780,17 +824,19 @@
 
         Returns:
             int:
 
         Raises:
             ValueError: if unsupported padding character is detected
         """
-        match = PRINTF_SYNTAX_PADDING_RE.match(chars)
+        match = PRINTF_SYNTAX_PADDING_RE.match(chars) or HOUDINI_SYNTAX_PADDING_RE.match(chars)
         if match:
-            return int(match.group(1))
+            paddingNumStr = match.group(1)
+            paddingNum = int(paddingNumStr) if paddingNumStr else 1
+            return max(paddingNum, 1)
 
         try:
             rval = 0
             for char in chars:
                 rval += PAD_MAP[char]
             return rval
         except KeyError:
```

## Comparing `Fileseq-1.8.1/src/fileseq/frameset.py` & `Fileseq-1.9.0/src/fileseq/frameset.py`

 * *Files identical despite different names*

## Comparing `Fileseq-1.8.1/src/fileseq/utils.py` & `Fileseq-1.9.0/src/fileseq/utils.py`

 * *Files identical despite different names*

## Comparing `Fileseq-1.8.1/test/test_fuzz.py` & `Fileseq-1.9.0/test/test_fuzz.py`

 * *Files identical despite different names*

## Comparing `Fileseq-1.8.1/test/test_fuzz.pyc` & `Fileseq-1.9.0/test/test_fuzz.pyc`

 * *Files identical despite different names*

## Comparing `Fileseq-1.8.1/test/test_unit.py` & `Fileseq-1.9.0/test/test_unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from __future__ import division
 from __future__ import absolute_import
 
-from future import standard_library
-standard_library.install_aliases()
+import warnings
+with warnings.catch_warnings():
+    warnings.simplefilter('ignore', DeprecationWarning)
+
+    from future import standard_library
+    standard_library.install_aliases()
+
 from builtins import map
 from future.utils import string_types, native_str
 
 try:
     import pickle as pickle
 except ImportError:
     import pickle
@@ -279,14 +284,38 @@
         self.assertEquals("%04d", seq.padding())
         self.assertEquals(".exr", seq.extension())
 
         self.assertEquals("/foo/boo.9999.exr", seq.frame(9999))
         self.assertEquals("/foo/boo.0001.exr", seq[0])
         self.assertEquals("/foo/boo.0001.exr", seq.index(0))
 
+    def testSeqGettersHoudini(self):
+        seq = FileSequence("/foo/boo.1-5$F.exr")
+        self.assertEquals(5, len(seq))
+        self.assertEquals("/foo/", seq.dirname())
+        self.assertEquals("boo.", seq.basename())
+        self.assertEquals("$F", seq.padding())
+        self.assertEquals(".exr", seq.extension())
+
+        self.assertEquals("/foo/boo.9999.exr", seq.frame(9999))
+        self.assertEquals("/foo/boo.1.exr", seq[0])
+        self.assertEquals("/foo/boo.1.exr", seq.index(0))
+
+    def testSeqGettersHoudiniPadded(self):
+        seq = FileSequence("/foo/boo.1-5$F4.exr")
+        self.assertEquals(5, len(seq))
+        self.assertEquals("/foo/", seq.dirname())
+        self.assertEquals("boo.", seq.basename())
+        self.assertEquals("$F4", seq.padding())
+        self.assertEquals(".exr", seq.extension())
+
+        self.assertEquals("/foo/boo.9999.exr", seq.frame(9999))
+        self.assertEquals("/foo/boo.0001.exr", seq[0])
+        self.assertEquals("/foo/boo.0001.exr", seq.index(0))
+
     def testSetDirname(self):
         seq = FileSequence("/foo/bong.1-5@.exr")
         seq.setDirname("/bing/")
         self.assertEquals("/bing/bong.1.exr", seq[0])
 
         seq = FileSequence("/foo/bong.1-5@.exr")
         seq.setDirname("bing")
@@ -503,14 +532,19 @@
         self.assertEquals(seq.padding(), '#')
 
         seq = FileSequence("/path/to/1-5%04d.exr")
         self.assertEquals(seq.basename(), "")
         self.assertEquals(len(seq), 5)
         self.assertEquals(seq.padding(), '%04d')
 
+        seq = FileSequence("/path/to/1-5$F4.exr")
+        self.assertEquals(seq.basename(), "")
+        self.assertEquals(len(seq), 5)
+        self.assertEquals(seq.padding(), "$F4")
+
     def testStringSubclasses(self):
         def sep(p):
             return p.replace("/", os.sep)
 
         tests = [
             ("/path/to/files.0001.ext", sep("/path/to/"), "files."),
             ("/path/to/files.1-100#.ext", sep("/path/to/"), "files."),
@@ -614,14 +648,40 @@
         actual = set(str(fs) for fs in FileSequence.yield_sequences_in_list(paths))
         self.assertEquals(expected, actual)
 
         paths = list(map(_CustomPathString, paths))
         actual = set(str(fs) for fs in FileSequence.yield_sequences_in_list(paths))
         self.assertEquals({str(_CustomPathString(p)) for p in expected}, actual)
 
+    def test_yield_sequences_in_list_using(self):
+        paths = [
+            'seq/file_0003.0001.exr',
+            'seq/file_0005.0001.exr',
+            'seq/file_0007.0001.exr',
+        ]
+
+        expects = [os.path.join("seq", "file_3-7x2#.0001.exr")]
+
+        template = FileSequence('seq/file_@@.0001.exr')
+        actual = {str(fs) for fs in FileSequence.yield_sequences_in_list(paths, using=template)}
+
+        for expect in expects:
+            self.assertIn(expect, actual)
+
+        expects = [
+            "seq/file_0003.1#.exr",
+            "seq/file_0005.1#.exr",
+            "seq/file_0007.1#.exr",
+        ]
+
+        actual = {str(fs) for fs in FileSequence.yield_sequences_in_list(paths)}
+
+        for expect in expects:
+            self.assertIn(expect, actual)
+
     def testIgnoreFrameSetStrings(self):
         for char in "xy:,".split():
             fs = FileSequence("/path/to/file{0}1-1x1#.exr".format(char))
             self.assertEquals(fs.basename(), "file{0}".format(char))
             self.assertEquals(fs.start(), 1)
             self.assertEquals(fs.end(), 1)
             self.assertEquals(fs.padding(), '#')
@@ -751,23 +811,24 @@
             os.path.join = _join
 
 
 class TestFindSequenceOnDisk(TestBase):
 
     def testFindSequenceOnDisk(self):
         tests = [
-            ("seq/bar#.exr", "seq/bar1000-1002,1004-1006#.exr"),
-            ("seq/foo.#.exr", "seq/foo.1-5#.exr"),
-            ("seq/foo.#.jpg", "seq/foo.1-5#.jpg"),
-            ("seq/foo.0002.jpg", "seq/foo.1-5#.jpg"),
-            ("seq/foo.#.exr", "seq/foo.1-5#.exr"),
-            ("seq/foo.debug.#.exr", "seq/foo.debug.1-5#.exr"),
-            ("seq/#.exr", "seq/1-3#.exr"),
-            ("seq/bar1001.exr", "seq/bar1001.exr"),
-            ("seq/foo_0001.exr", "seq/foo_0001.exr"),
+            # ("seq/bar#.exr", "seq/bar1000-1002,1004-1006#.exr"),
+            # ("seq/foo.#.exr", "seq/foo.1-5#.exr"),
+            # ("seq/foo.#.jpg", "seq/foo.1-5#.jpg"),
+            # ("seq/foo.0002.jpg", "seq/foo.1-5#.jpg"),
+            # ("seq/foo.#.exr", "seq/foo.1-5#.exr"),
+            # ("seq/foo.debug.#.exr", "seq/foo.debug.1-5#.exr"),
+            # ("seq/#.exr", "seq/1-3#.exr"),
+            # ("seq/bar1001.exr", "seq/bar1001.exr"),
+            # ("seq/foo_0001.exr", "seq/foo_0001.exr"),
+            ("multi_range/file_#.0001.exr", "multi_range/file_3-5#.0001.exr"),
         ]
 
         for pattern, expected in tests:
             seq = findSequenceOnDisk(pattern, strictPadding=False)
             self.assertTrue(isinstance(seq, FileSequence))
             actual = str(seq)
             self.assertEqual(actual, expected)
@@ -790,19 +851,21 @@
             ("seq/foo_#_extra.exr", None),
             ("seq/foo_##.exr", None),
             ("seq/foo_@.exr", None),
             ("seq/big.#.ext", "seq/big.999-1003#.ext"),
             ("seq/big.@@@.ext", "seq/big.1000-1003@@@.ext"),
             ("seq/big.@.ext", "seq/big.1000-1003@.ext"),
             ("seq/big.#@.ext", None),
+            ("multi_range/file_@@.0001.exr", None),
+            ("multi_range/file_#.0001.exr", "multi_range/file_3-5#.0001.exr"),
         ]
 
         for pattern, expected in tests:
             if expected is None:
-                with self.assertRaises(FileSeqException):
+                with self.assertRaises(FileSeqException, msg=pattern):
                     findSequenceOnDisk(pattern, strictPadding=True)
                 continue
 
             seq = findSequenceOnDisk(pattern, strictPadding=True)
             self.assertTrue(isinstance(seq, FileSequence))
             actual = str(seq)
             self.assertEqual(actual, expected)
@@ -900,25 +963,37 @@
         self.assertEqual(getPaddingNum('#@'), 5)
         self.assertEqual(getPaddingNum('##@@'), 10)
 
         self.assertEqual(getPaddingNum('%01d'), 1)
         self.assertEqual(getPaddingNum('%1d'), 1)
         self.assertEqual(getPaddingNum('%04d'), 4)
         self.assertEqual(getPaddingNum('%10d'), 10)
+        self.assertEqual(getPaddingNum('%00d'), 1)
+        self.assertEqual(getPaddingNum('%0d'), 1)
+        self.assertEqual(getPaddingNum('%d'), 1)
+
+        self.assertEqual(getPaddingNum('$F'), 1)
+        self.assertEqual(getPaddingNum('$F1'), 1)
+        self.assertEqual(getPaddingNum('$F2'), 2)
+        self.assertEqual(getPaddingNum('$F3'), 3)
 
-        allPossibleChars = [s for s in string.printable if s not in list(PAD_MAP.keys())]
+        allPossibleChars = [s for s in string.printable if s not in PAD_MAP]
         for char in allPossibleChars:
             self.assertRaises(ValueError, getPaddingNum, char)
             self.assertRaises(ValueError, getPaddingNum, '#{}'.format(char))
             self.assertRaises(ValueError, getPaddingNum, '@{}'.format(char))
 
-        allPossibleChars = [s for s in string.printable if s not in list(PAD_MAP.keys()) and s not in string.digits]
+        allPossibleChars = [s for s in string.printable if s not in PAD_MAP and s not in string.digits]
         for char in allPossibleChars:
             self.assertRaises(ValueError, getPaddingNum, '%{}d'.format(char))
 
+        allPossibleChars = [s for s in string.printable if s not in PAD_MAP and s not in string.digits]
+        for char in allPossibleChars:
+            self.assertRaises(ValueError, getPaddingNum, '$F{}'.format(char))
+
     def testConformPadding(self):
         """
         Ensure that alternate padding formats are conformed
         to a primary PAD_MAP format
         """
         class Case(object):
             def __init__(self, src, expected, error=False):
@@ -935,14 +1010,21 @@
             Case('@', '@'),
             Case('%08d', '##'),
             Case('%05d', '@@@@@'),
             Case('%04d', '#'),
             Case('%03d', '@@@'),
             Case('%02d', '@@'),
             Case('%01d', '@'),
+            Case('%00d', '@'),
+            Case('%1d', '@'),
+            Case('%d', '@'),
+            Case('$F', '@'),
+            Case('$F1', '@'),
+            Case('$F2', '@@'),
+            Case('$F4', '#'),
             Case('', ''),
             Case('foo', 'foo', error=True),
         ]
 
         for case in tests:
             
             if case.error:
```

## Comparing `Fileseq-1.8.1/test/test_unit.pyc` & `Fileseq-1.9.0/test/test_unit.pyc`

 * *Files identical despite different names*

## Comparing `Fileseq-1.8.1/test/utils.pyc` & `Fileseq-1.9.0/test/utils.pyc`

 * *Files identical despite different names*

