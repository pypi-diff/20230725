# Comparing `tmp/fastq_preprocessor-2023.5.17.tar.gz` & `tmp/fastq_preprocessor-2023.7.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastq_preprocessor-2023.5.17.tar", last modified: Tue May 16 06:14:22 2023, max compression
+gzip compressed data, was "fastq_preprocessor-2023.7.24.tar", last modified: Mon Jul 24 22:41:00 2023, max compression
```

## Comparing `fastq_preprocessor-2023.5.17.tar` & `fastq_preprocessor-2023.7.24.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-05-16 06:14:22.035565 fastq_preprocessor-2023.5.17/
--rw-------   0 jespinoz  (3456) staff       (20)     1750 2020-03-27 17:41:41.000000 fastq_preprocessor-2023.5.17/LICENSE.txt
--rw-------   0 jespinoz  (3456) staff       (20)      151 2022-02-15 23:53:42.000000 fastq_preprocessor-2023.5.17/MANIFEST.in
--rw-r--r--   0 jespinoz  (3456) staff       (20)      302 2023-05-16 06:14:22.035182 fastq_preprocessor-2023.5.17/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)    16608 2023-05-16 06:13:55.000000 fastq_preprocessor-2023.5.17/README.md
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-05-16 06:14:22.031453 fastq_preprocessor-2023.5.17/bin/
--rwxrwxr-x   0 jespinoz  (3456) staff       (20)    23211 2023-05-16 06:08:00.000000 fastq_preprocessor-2023.5.17/bin/fastq_preprocessor
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-05-16 06:14:22.032417 fastq_preprocessor-2023.5.17/fastq_preprocessor/
--rwxrwxr-x   0 jespinoz  (3456) staff       (20)     2476 2023-05-16 06:01:26.000000 fastq_preprocessor-2023.5.17/fastq_preprocessor/__init__.py
--rwxrwxr-x   0 jespinoz  (3456) staff       (20)    23217 2023-05-16 06:10:23.000000 fastq_preprocessor-2023.5.17/fastq_preprocessor/fastq_preprocessor.py
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-05-16 06:14:22.034691 fastq_preprocessor-2023.5.17/fastq_preprocessor.egg-info/
--rw-------   0 jespinoz  (3456) staff       (20)      302 2023-05-16 06:14:21.000000 fastq_preprocessor-2023.5.17/fastq_preprocessor.egg-info/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)      346 2023-05-16 06:14:21.000000 fastq_preprocessor-2023.5.17/fastq_preprocessor.egg-info/SOURCES.txt
--rw-------   0 jespinoz  (3456) staff       (20)        1 2023-05-16 06:14:21.000000 fastq_preprocessor-2023.5.17/fastq_preprocessor.egg-info/dependency_links.txt
--rw-------   0 jespinoz  (3456) staff       (20)       80 2023-05-16 06:14:21.000000 fastq_preprocessor-2023.5.17/fastq_preprocessor.egg-info/requires.txt
--rw-------   0 jespinoz  (3456) staff       (20)       19 2023-05-16 06:14:21.000000 fastq_preprocessor-2023.5.17/fastq_preprocessor.egg-info/top_level.txt
--rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-05-16 06:14:22.035697 fastq_preprocessor-2023.5.17/setup.cfg
--rw-------   0 jespinoz  (3456) staff       (20)      943 2023-05-16 00:08:07.000000 fastq_preprocessor-2023.5.17/setup.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-24 22:41:00.178213 fastq_preprocessor-2023.7.24/
+-rw-------   0 jespinoz  (3456) staff       (20)    34519 2023-06-21 19:49:42.000000 fastq_preprocessor-2023.7.24/LICENSE
+-rw-------   0 jespinoz  (3456) staff       (20)      151 2022-02-15 23:53:42.000000 fastq_preprocessor-2023.7.24/MANIFEST.in
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      326 2023-07-24 22:41:00.177830 fastq_preprocessor-2023.7.24/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)    16636 2023-07-24 22:14:04.000000 fastq_preprocessor-2023.7.24/README.md
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-24 22:41:00.172852 fastq_preprocessor-2023.7.24/bin/
+-rwxrwxr-x   0 jespinoz  (3456) staff       (20)    23137 2023-07-24 22:19:45.000000 fastq_preprocessor-2023.7.24/bin/fastq_preprocessor
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-24 22:41:00.174458 fastq_preprocessor-2023.7.24/fastq_preprocessor/
+-rwxrwxr-x   0 jespinoz  (3456) staff       (20)      492 2023-07-24 22:11:31.000000 fastq_preprocessor-2023.7.24/fastq_preprocessor/__init__.py
+-rwxrwxr-x   0 jespinoz  (3456) staff       (20)    23137 2023-07-24 22:19:26.000000 fastq_preprocessor-2023.7.24/fastq_preprocessor/fastq_preprocessor.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-07-24 22:41:00.177250 fastq_preprocessor-2023.7.24/fastq_preprocessor.egg-info/
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      326 2023-07-24 22:40:59.000000 fastq_preprocessor-2023.7.24/fastq_preprocessor.egg-info/PKG-INFO
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      342 2023-07-24 22:41:00.000000 fastq_preprocessor-2023.7.24/fastq_preprocessor.egg-info/SOURCES.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)        1 2023-07-24 22:40:59.000000 fastq_preprocessor-2023.7.24/fastq_preprocessor.egg-info/dependency_links.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)       80 2023-07-24 22:40:59.000000 fastq_preprocessor-2023.7.24/fastq_preprocessor.egg-info/requires.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)       19 2023-07-24 22:40:59.000000 fastq_preprocessor-2023.7.24/fastq_preprocessor.egg-info/top_level.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-07-24 22:41:00.178339 fastq_preprocessor-2023.7.24/setup.cfg
+-rw-------   0 jespinoz  (3456) staff       (20)      971 2023-07-24 22:13:10.000000 fastq_preprocessor-2023.7.24/setup.py
```

### Comparing `fastq_preprocessor-2023.5.17/README.md` & `fastq_preprocessor-2023.7.24/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 `__cite__ = "TBD"`
 
 `__contact__ = "jespinoz@jcvi.org, jol.espinoz@gmail.com"`
 
 `__developmental__ = True`
 
-`__license__ = "BSD-3"`
+`__license__ = "GNU AFFERO GENERAL PUBLIC LICENSE"`
 
-`__version__ = "2022.5.17"`
+`__version__ = "2023.7.17"`
 
 #### Dependencies: 
 
 ##### Bioinformatics software:
 * bbmap
 * fastp
 * seqkit
```

### Comparing `fastq_preprocessor-2023.5.17/bin/fastq_preprocessor` & `fastq_preprocessor-2023.7.24/bin/fastq_preprocessor`

 * *Files 2% similar despite different names*

```diff
@@ -8,45 +8,48 @@
 # Soothsayer Ecosystem
 from genopype import *
 from soothsayer_utils import *
 
 pd.options.display.max_colwidth = 100
 
 __program__ = os.path.split(sys.argv[0])[-1]
-__version__ = "2023.5.17"
+__version__ = "2023.7.24"
 
 # .............................................................................
 # Primordial
 # .............................................................................
-# Kneaddata
+# Fastp
 def get_fastp_cmd(input_filepaths, output_filepaths, output_directory, directories, opts):
     os.environ["TMPDIR"] = directories["tmp"]
     # Command
     cmd = [
     # fastp
     "(",
+    os.environ["repair.sh"],
+    "out=stdout.fastq",
+    "in1={}".format(input_filepaths[0]),
+    "in2={}".format(input_filepaths[1]),
+    "|",
     os.environ["fastp"],
-    "--in1 {}".format(input_filepaths[0]),
-    "--in2 {}".format(input_filepaths[1]),
+    "--stdin",
     "--stdout",
+    "--interleaved_in",
     "-h {}".format(os.path.join(output_directory, "fastp.html")),
     "-j {}".format(os.path.join(output_directory, "fastp.json")),
     "-l {}".format(opts.minimum_read_length),
     "--thread {}".format(opts.n_jobs),
     {"detect":"--detect_adapter_for_pe"}.get(opts.adapters, "--adapter_fasta {}".format(opts.adapters)), # Use --detect_adapter_for_pe by default unless a fasta path is given
     opts.fastp_options,
-    ")",
     # reformat.sh
     "|",
-    "(",
     os.environ["repair.sh"],
     "in=stdin.fastq",
     "out1={}".format(os.path.join(output_directory, "trimmed_1.fastq.gz")),
     "out2={}".format(os.path.join(output_directory, "trimmed_2.fastq.gz")),
-    "outs={}".format(os.path.join(output_directory, "trimmed_singletons.fastq.gz")),
+    # "outs={}".format(os.path.join(output_directory, "trimmed_singletons.fastq.gz")),
     "overwrite=t",
     ")",
     # Seqkit
     "&&",
     "(",
     os.environ["seqkit"],
     "stats",
@@ -205,15 +208,15 @@
             os.path.join(output_directory,"seqkit_stats.concatenated.tsv"),
             ),
         ]
 
     cmd += [
     "DST={}; (for SRC in {}; do SRC=$(realpath --relative-to $DST $SRC); ln -sf $SRC $DST; done)".format(
         output_directory,
-        input_filepaths, 
+        " ".join(input_filepaths), 
         )
     ]
         
 
     return cmd
 
 # ============
@@ -495,22 +498,22 @@
     parser_fastp = parser.add_argument_group('Fastp arguments')
     parser_fastp.add_argument("-m", "--minimum_read_length", type=int, default=75, help="Fastp | Minimum read length [Default: 75]")
     parser_fastp.add_argument("-a", "--adapters", type=str, default="detect", help="Fastp | path/to/adapters.fasta [Default: detect]")
     parser_fastp.add_argument("--fastp_options", type=str, default="", help="Fastp | More options (e.g. --arg 1 ) [Default: '']")
 
     # Bowtie
     parser_bowtie2 = parser.add_argument_group('Bowtie2 arguments')
-    parser_bowtie2.add_argument("-x", "--contamination_index", type=str, help="Bowtie2 | path/to/contamination_index\n(e.g., Human GRCh38 from ftp://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/000/001/405/GCA_000001405.15_GRCh38/seqs_for_alignment_pipelines.ucsc_ids//GCA_000001405.15_GRCh38_no_alt_analysis_set.fna.bowtie_index.tar.gz)")
+    parser_bowtie2.add_argument("-x", "--contamination_index", type=str, help="Bowtie2 | path/to/contamination_index\n(e.g., Human T2T assembly from https://genome-idx.s3.amazonaws.com/bt/chm13v2.0.zip)")
     parser_bowtie2.add_argument("--retain_trimmed_reads", default=0, type=int, help = "Retain fastp trimmed fastq after decontamination. 0=No, 1=yes [Default: 0]") 
     parser_bowtie2.add_argument("--retain_contaminated_reads", default=0, type=int, help = "Retain contaminated fastq after decontamination. 0=No, 1=yes [Default: 0]")
     parser_bowtie2.add_argument("--bowtie2_options", type=str, default="", help="Bowtie2 | More options (e.g. --arg 1 ) [Default: '']\nhttp://bowtie-bio.sourceforge.net/bowtie2/manual.shtml")
 
     # BBDuk
     parser_bbduk = parser.add_argument_group('BBDuk arguments')
-    parser_bbduk.add_argument("-k","--kmer_database", type=str,  help="BBDuk | path/to/kmer_database\n(e.g., ribokmers.fa.gz from https://drive.google.com/file/d/0B3llHR93L14wS2NqRXpXakhFaEk/view?usp=sharing)")
+    parser_bbduk.add_argument("-k","--kmer_database", type=str,  help="BBDuk | path/to/kmer_database\n(e.g., ribokmers.fa.gz from https://figshare.com/ndownloader/files/36220587)")
     parser_bbduk.add_argument("--kmer_size", type=int, default=31, help="BBDuk | k-mer size [Default: 31]")
     parser_bbduk.add_argument("--retain_kmer_hits", default=0, type=int, help = "Retain reads that map to k-mer database. 0=No, 1=yes [Default: 0]")
     parser_bbduk.add_argument("--retain_non_kmer_hits", default=0, type=int, help = "Retain reads that do not map to k-mer database. 0=No, 1=yes [Default: 0]")
     parser_bbduk.add_argument("--bbduk_options", type=str, default="", help="BBDuk | More options (e.g., --arg 1) [Default: '']")
 
     # Options
     opts = parser.parse_args()
@@ -518,15 +521,15 @@
     opts.script_filename = script_filename
 
     # Threads
     if opts.n_jobs == -1:
         from multiprocessing import cpu_count 
         opts.n_jobs = cpu_count()
     assert opts.n_jobs >= 1, "--n_jobs must be ≥ 1.  To select all available threads, use -1."
-    
+
     # Directories
     directories = dict()
     directories["project"] = create_directory(opts.project_directory)
     directories["sample"] = create_directory(os.path.join(directories["project"], opts.name))
     directories["output"] = create_directory(os.path.join(directories["sample"], "output"))
     directories["log"] = create_directory(os.path.join(directories["sample"], "log"))
     directories["tmp"] = create_directory(os.path.join(directories["sample"], "tmp"))
```

### Comparing `fastq_preprocessor-2023.5.17/fastq_preprocessor/fastq_preprocessor.py` & `fastq_preprocessor-2023.7.24/fastq_preprocessor/fastq_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,45 +8,48 @@
 # Soothsayer Ecosystem
 from genopype import *
 from soothsayer_utils import *
 
 pd.options.display.max_colwidth = 100
 
 __program__ = os.path.split(sys.argv[0])[-1]
-__version__ = "2023.5.17"
+__version__ = "2023.7.24"
 
 # .............................................................................
 # Primordial
 # .............................................................................
-# Kneaddata
+# Fastp
 def get_fastp_cmd(input_filepaths, output_filepaths, output_directory, directories, opts):
     os.environ["TMPDIR"] = directories["tmp"]
     # Command
     cmd = [
     # fastp
     "(",
+    os.environ["repair.sh"],
+    "out=stdout.fastq",
+    "in1={}".format(input_filepaths[0]),
+    "in2={}".format(input_filepaths[1]),
+    "|",
     os.environ["fastp"],
-    "--in1 {}".format(input_filepaths[0]),
-    "--in2 {}".format(input_filepaths[1]),
+    "--stdin",
     "--stdout",
+    "--interleaved_in",
     "-h {}".format(os.path.join(output_directory, "fastp.html")),
     "-j {}".format(os.path.join(output_directory, "fastp.json")),
     "-l {}".format(opts.minimum_read_length),
     "--thread {}".format(opts.n_jobs),
     {"detect":"--detect_adapter_for_pe"}.get(opts.adapters, "--adapter_fasta {}".format(opts.adapters)), # Use --detect_adapter_for_pe by default unless a fasta path is given
     opts.fastp_options,
-    ")",
     # reformat.sh
     "|",
-    "(",
     os.environ["repair.sh"],
     "in=stdin.fastq",
     "out1={}".format(os.path.join(output_directory, "trimmed_1.fastq.gz")),
     "out2={}".format(os.path.join(output_directory, "trimmed_2.fastq.gz")),
-    "outs={}".format(os.path.join(output_directory, "trimmed_singletons.fastq.gz")),
+    # "outs={}".format(os.path.join(output_directory, "trimmed_singletons.fastq.gz")),
     "overwrite=t",
     ")",
     # Seqkit
     "&&",
     "(",
     os.environ["seqkit"],
     "stats",
@@ -495,22 +498,22 @@
     parser_fastp = parser.add_argument_group('Fastp arguments')
     parser_fastp.add_argument("-m", "--minimum_read_length", type=int, default=75, help="Fastp | Minimum read length [Default: 75]")
     parser_fastp.add_argument("-a", "--adapters", type=str, default="detect", help="Fastp | path/to/adapters.fasta [Default: detect]")
     parser_fastp.add_argument("--fastp_options", type=str, default="", help="Fastp | More options (e.g. --arg 1 ) [Default: '']")
 
     # Bowtie
     parser_bowtie2 = parser.add_argument_group('Bowtie2 arguments')
-    parser_bowtie2.add_argument("-x", "--contamination_index", type=str, help="Bowtie2 | path/to/contamination_index\n(e.g., Human GRCh38 from ftp://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/000/001/405/GCA_000001405.15_GRCh38/seqs_for_alignment_pipelines.ucsc_ids//GCA_000001405.15_GRCh38_no_alt_analysis_set.fna.bowtie_index.tar.gz)")
+    parser_bowtie2.add_argument("-x", "--contamination_index", type=str, help="Bowtie2 | path/to/contamination_index\n(e.g., Human T2T assembly from https://genome-idx.s3.amazonaws.com/bt/chm13v2.0.zip)")
     parser_bowtie2.add_argument("--retain_trimmed_reads", default=0, type=int, help = "Retain fastp trimmed fastq after decontamination. 0=No, 1=yes [Default: 0]") 
     parser_bowtie2.add_argument("--retain_contaminated_reads", default=0, type=int, help = "Retain contaminated fastq after decontamination. 0=No, 1=yes [Default: 0]")
     parser_bowtie2.add_argument("--bowtie2_options", type=str, default="", help="Bowtie2 | More options (e.g. --arg 1 ) [Default: '']\nhttp://bowtie-bio.sourceforge.net/bowtie2/manual.shtml")
 
     # BBDuk
     parser_bbduk = parser.add_argument_group('BBDuk arguments')
-    parser_bbduk.add_argument("-k","--kmer_database", type=str,  help="BBDuk | path/to/kmer_database\n(e.g., ribokmers.fa.gz from https://drive.google.com/file/d/0B3llHR93L14wS2NqRXpXakhFaEk/view?usp=sharing)")
+    parser_bbduk.add_argument("-k","--kmer_database", type=str,  help="BBDuk | path/to/kmer_database\n(e.g., ribokmers.fa.gz from https://figshare.com/ndownloader/files/36220587)")
     parser_bbduk.add_argument("--kmer_size", type=int, default=31, help="BBDuk | k-mer size [Default: 31]")
     parser_bbduk.add_argument("--retain_kmer_hits", default=0, type=int, help = "Retain reads that map to k-mer database. 0=No, 1=yes [Default: 0]")
     parser_bbduk.add_argument("--retain_non_kmer_hits", default=0, type=int, help = "Retain reads that do not map to k-mer database. 0=No, 1=yes [Default: 0]")
     parser_bbduk.add_argument("--bbduk_options", type=str, default="", help="BBDuk | More options (e.g., --arg 1) [Default: '']")
 
     # Options
     opts = parser.parse_args()
```

### Comparing `fastq_preprocessor-2023.5.17/setup.py` & `fastq_preprocessor-2023.7.24/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 setup(name='fastq_preprocessor',
       version=version,
       description='Fast short read fastq preprocessor with optional contamination removal',
       url='https://github.com/jolespin/fastq_preprocessor',
       author='Josh L. Espinoza',
       author_email='jespinoz@jcvi.org',
-      license='BSD-3',
+      license='GNU AFFERO GENERAL PUBLIC LICENSE',
       packages=["fastq_preprocessor"],
       install_requires=[
       "genopype >=2023.4.13",
       "soothsayer_utils >=2022.6.24",
       "pandas >=0.24",
       "numpy",
       "tqdm",
```

