# Comparing `tmp/datawords-0.7.0.tar.gz` & `tmp/datawords-0.7.1.tar.gz`

## Comparing `datawords-0.7.0.tar` & `datawords-0.7.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datawords-0.7.0/.pylintrc
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 datawords-0.7.0/Makefile
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datawords-0.7.0/mypy.ini
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datawords-0.7.0/readthedocs.yml
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/__about__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/_utils.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/constants.py
--rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/indexes.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/install_pytorch.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/models.py
--rw-r--r--   0        0        0    14532 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/parsers.py
--rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/ranking.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/utils.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/deepnlp/__init__.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/deepnlp/core.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/deepnlp/translators.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/deepnlp/translators2.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/deepnlp/utils.py
--rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/files/stop_en.txt
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/files/stop_es.txt
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 datawords-0.7.0/datawords/files/stop_pt.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/make.bat
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api_reference.rst
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/conf.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/index.rst
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/introduction.rst
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api/deepnlp.rst
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api/indexes.rst
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api/models.rst
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api/parsers.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datawords-0.7.0/docs/source/api/ranking.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/shared.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/test_indexes.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/test_models.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/test_parsers.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/test_rankings.py
--rw-r--r--   0        0        0    21956 2020-02-02 00:00:00.000000 datawords-0.7.0/tests/texts.txt
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datawords-0.7.0/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datawords-0.7.0/LICENSE
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 datawords-0.7.0/NOTICE.md
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 datawords-0.7.0/README.md
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 datawords-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 datawords-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    20849 2020-02-02 00:00:00.000000 datawords-0.7.1/.pylintrc
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 datawords-0.7.1/Makefile
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 datawords-0.7.1/mypy.ini
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 datawords-0.7.1/readthedocs.yml
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/__about__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/_utils.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/constants.py
+-rw-r--r--   0        0        0    15202 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/indexes.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/install_pytorch.py
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/models.py
+-rw-r--r--   0        0        0    14532 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/parsers.py
+-rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/ranking.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/utils.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/deepnlp/__init__.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/deepnlp/core.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/deepnlp/translators.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/deepnlp/translators2.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/deepnlp/utils.py
+-rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/files/stop_en.txt
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/files/stop_es.txt
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 datawords-0.7.1/datawords/files/stop_pt.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/make.bat
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api_reference.rst
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/conf.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/index.rst
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/introduction.rst
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api/deepnlp.rst
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api/indexes.rst
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api/models.rst
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api/parsers.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datawords-0.7.1/docs/source/api/ranking.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/shared.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/test_indexes.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/test_models.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/test_parsers.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/test_rankings.py
+-rw-r--r--   0        0        0    21956 2020-02-02 00:00:00.000000 datawords-0.7.1/tests/texts.txt
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 datawords-0.7.1/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 datawords-0.7.1/LICENSE
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 datawords-0.7.1/NOTICE.md
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 datawords-0.7.1/README.md
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 datawords-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 datawords-0.7.1/PKG-INFO
```

### Comparing `datawords-0.7.0/.pylintrc` & `datawords-0.7.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/Makefile` & `datawords-0.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/_utils.py` & `datawords-0.7.1/datawords/_utils.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/constants.py` & `datawords-0.7.1/datawords/constants.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/indexes.py` & `datawords-0.7.1/datawords/indexes.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,20 @@
     """
     Represents a document indexed in the :class:`SQLiteIndex`
     """
 
     id: str
     text: str
 
+    def __hash__(self):
+        return hash(self.id)
+
+    def __eq__(self, other):
+        return self.id == other.id
+
 
 @define
 class TextIndexMeta:
     name: str
     words_model_path: str
     vector_size: int = 100
     ann_trees: int = 10
@@ -256,14 +262,19 @@
         :param stopwords: list of stop words to be used by the parsed.
         :type stopwords: Set[str]
         """
         self.db = sqlite3.connect(sqlite)
         self._create_tables()
         self._stopw = stopwords
 
+    def journal_mode(self):
+        cur = self.db.cursor()
+        cur.execute("PRAGMA jounral_mode=WAL;")
+        cur.close()
+
     def _create_tables(self):
         cur = self.db.cursor()
         cur.execute(
             'create virtual table search_docs using fts5(id, text, tokenize="ascii");'
         )
         cur.execute(
             """CREATE TABLE search_index
@@ -279,14 +290,20 @@
             strip_accents=True,
             lower=True,
             numbers=True,
             parse_urls=False,
         )
         return tokens
 
+    def parse(self, txt) -> List[str]:
+        """
+        Parse a text
+        """
+        return self._parse(txt)
+
     def _insert(self, cur, doc: LiteDoc):
         tokens = self._parse(doc.text)
         words = " ".join(tokens)
         cur.execute(
             "insert into search_index (doc_id) values (?);",
             (doc.id,),
         )
@@ -335,31 +352,26 @@
         sqlite: str = ":memory:",
     ) -> "SQLiteIndex":
         obj = cls(sqlite, stopwords)
         cur = obj.db.cursor()
         tracking = []
         for _id in tqdm(ids, disable=not progress_bar, total=total_ids):
             data = getter(_id)
-            doc = LiteDoc(
-                id=_id,
-                text=data
-            )
+            doc = LiteDoc(id=_id, text=data)
             try:
                 obj._insert(cur, doc)
                 tracking.append(True)
             except sqlite3.IntegrityError:
                 tracking.append(False)
         obj.db.commit()
         cur.close()
         return obj
 
     @classmethod
-    def load(
-        cls, sqlite: str, stopwords=set()
-    ) -> "SQLiteIndex":
+    def load(cls, sqlite: str, stopwords=set()) -> "SQLiteIndex":
         obj = cls(sqlite, stopwords)
         return obj
 
     def add_batch(self, docs: List[LiteDoc]) -> List[bool]:
         """
         Add documents in batch.
 
@@ -380,14 +392,26 @@
         cur.close()
         return tracking
 
     def _list(self, cur, limit=10, offset=0, table="search_index"):
         result = cur.execute(f"select * from {table} LIMIT {offset}, {limit};")
         return result
 
+    def get_doc(self, id: str) -> LiteDoc:
+        cur = self.db.cursor()
+        # row = cur.execute(f"select * from search_docs where search_docs.id={id};").fetchone()
+
+        row = cur.execute(
+                f"""select * from search_docs where text MATCH '{id}'
+                                    limit 1"""
+        ).fetchone()
+
+        cur.close()
+        return LiteDoc(id=row[0], text=row[1])
+
     def list_docs(self, limit=10, offset=0) -> List[LiteDoc]:
         cur = self.db.cursor()
         rows = self._list(cur, limit=limit, offset=offset, table="search_docs")
         docs = [LiteDoc(id=r[0], text=r[1]) for r in rows]
         cur.close()
         return docs
 
@@ -407,15 +431,22 @@
         cur = self.db.cursor()
         res = cur.execute("select count(*) from search_index;").fetchone()
         cur.close()
         return res[0]
 
     def search(self, text: str, top_n: int = 5) -> List[LiteDoc]:
         """
-        Performs a search in the index.
+        Performs a search in the index. It will parse and match
+        the wodos as:
+
+        MATCH '"{words}" *'
+
+        To use a more low level search query use
+        :method:`SQLiteIndex.search_query`
+
 
         :param text: text to search.
         :type text: str
         :param limit: how many results retrieve.
         :type limit: int
         :return: Documents found
         :rtype: List[LiteDoc]
@@ -429,7 +460,33 @@
                                     limit {top_n}"""
             ).fetchall()
 
         except sqlite3.OperationalError:
             result = []
         cur.close()
         return [LiteDoc(id=r[0], text=r[1]) for r in result]
+
+    def search_query(self, query: str, top_n: int = 5) -> List[LiteDoc]:
+        """
+        Performs a search query into the sqlite database.
+
+        'search AND (sqlite OR help)'
+
+        :param query: query to search
+        :type query: str
+        :param limit: how many results retrieve.
+        :type limit: int
+        :return: Documents found
+        :rtype: List[LiteDoc]
+        """
+        # tokens = self._parse(text)
+        cur = self.db.cursor()
+        try:
+            result = cur.execute(
+                f"""select * from search_docs where text MATCH '{query}'
+                                    limit {top_n}"""
+            ).fetchall()
+
+        except sqlite3.OperationalError:
+            result = []
+        cur.close()
+        return [LiteDoc(id=r[0], text=r[1]) for r in result]
```

### Comparing `datawords-0.7.0/datawords/install_pytorch.py` & `datawords-0.7.1/datawords/install_pytorch.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/models.py` & `datawords-0.7.1/datawords/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,18 @@
 
     @property
     def vector_size(self) -> int:
         return self._size
 
     @property
     def wv(self) -> Union[Word2Vec, KeyedVectors]:
-        return self.model
+        if self._using_kv:
+            return self.model
+        else:
+            return self.model.wv
 
     def fit(self, X: Iterable):
         """
         This will train the model. It needs an iterable.
 
         :param X: An iterable which returns plain texts.
         :type X: Iterable
@@ -124,15 +127,15 @@
         """Get a vector from a list of words
         if a sentence has words that don't match in the word2vec model,
         then it fills with zeros
         """
         vectors = []
         for word in sentence:
             try:
-                _vect = self.model.wv[word]
+                _vect = self.wv[word]
                 vectors.append(_vect)
             except KeyError:
                 pass
         if len(vectors) > 0:
             return np.sum(np.array(vectors), axis=0) / (len(vectors) + 0.001)
         return np.zeros((self._size,))
 
@@ -181,15 +184,15 @@
         else:
             model = Word2Vec.load(f"{fp}/{name}.bin")
         with open(f"{fp}/{name}.json", "r") as f:
             jmeta = json.loads(f.read())
             meta = cattrs.structure(jmeta, W2VecMeta)
         phrases = None
         if meta.phrases_model_path:
-            phrases = PhrasesModel.load(meta.phrases_model_path)
+            phrases = parsers.PhrasesModel.load(meta.phrases_model_path)
         obj = cls(
             parser_conf=meta.parser_conf,
             phrases_model=phrases,
             size=meta.size,
             window=meta.window,
             min_count=meta.min_count,
             model=model,
```

### Comparing `datawords-0.7.0/datawords/parsers.py` & `datawords-0.7.1/datawords/parsers.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/ranking.py` & `datawords-0.7.1/datawords/ranking.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/utils.py` & `datawords-0.7.1/datawords/utils.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/deepnlp/core.py` & `datawords-0.7.1/datawords/deepnlp/core.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/deepnlp/translators.py` & `datawords-0.7.1/datawords/deepnlp/translators.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/deepnlp/translators2.py` & `datawords-0.7.1/datawords/deepnlp/translators2.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/files/stop_en.txt` & `datawords-0.7.1/datawords/files/stop_en.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/files/stop_es.txt` & `datawords-0.7.1/datawords/files/stop_es.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/datawords/files/stop_pt.txt` & `datawords-0.7.1/datawords/files/stop_pt.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/docs/Makefile` & `datawords-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/docs/make.bat` & `datawords-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/docs/source/conf.py` & `datawords-0.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/docs/source/index.rst` & `datawords-0.7.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/docs/source/introduction.rst` & `datawords-0.7.1/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/docs/source/api/deepnlp.rst` & `datawords-0.7.1/docs/source/api/deepnlp.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/docs/source/api/indexes.rst` & `datawords-0.7.1/docs/source/api/indexes.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/docs/source/api/parsers.rst` & `datawords-0.7.1/docs/source/api/parsers.rst`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/tests/test_indexes.py` & `datawords-0.7.1/tests/test_indexes.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,34 @@
         texts = f.readlines()
     for t in texts:
         _t = t.strip()
         if _t:
             yield _t
 
 
+def test_indexes_lite_doc():
+    l1 = LiteDoc(id="test", text="pepe")
+    l2 = LiteDoc(id="test", text="other text")
+    l3 = LiteDoc(id="different", text="other text")
+    s = set()
+    s.add(l1)
+    s.add(l2)
+    s.add(l3)
+    assert len(s) == 2
+    assert l1 == l2
+    assert l1 != l3
+
+def test_indexes_sqlite_get():
+    l1 = LiteDoc(id="pepe", text="pepe")
+    ix = SQLiteIndex()
+    ix.add_batch([l1])
+    doc = ix.get_doc("pepe")
+
+    assert doc.text == "pepe"
+
 def test_indexes_words_index():
     texts = open_texts()
     parser_conf = parsers.ParserConf(lang="en")
     # model = PhrasesModel(parser_conf)
     # model.fit(texts)
     elements = {x[0]: x[1] for x in enumerate(list(open_texts()))}
 
@@ -59,7 +79,20 @@
     # docs = [LiteDoc(id=ix, text=t) for ix, t in enumerate(texts[:5])]
     ids = list(elements.keys())
     ix = SQLiteIndex.build(ids=ids, getter=getter, stopwords=stopw)
     total = ix.total
     res = ix.search("coco", top_n=1)
     assert isinstance(res[0], LiteDoc)
     assert total == 5
+
+
+def test_indexes_sqlite_search_query():
+    elements = {x[0]: x[1] for x in enumerate(list(open_texts())[:5])}
+
+    def getter(id_):
+        return elements[id_]
+    stopw = parsers.load_stop2()
+    # docs = [LiteDoc(id=ix, text=t) for ix, t in enumerate(texts[:5])]
+    ids = list(elements.keys())
+    ix = SQLiteIndex.build(ids=ids, getter=getter, stopwords=stopw)
+    res = ix.search_query("cocomelon AND goal", top_n=1)
+    assert isinstance(res[0], LiteDoc)
```

### Comparing `datawords-0.7.0/tests/test_models.py` & `datawords-0.7.1/tests/test_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,10 +17,15 @@
     wv.fit(texts)
     with tempfile.TemporaryDirectory() as tmpdir:
         fp = f"{tmpdir}/tests"
         wv.save(fp)
         wv2 = Word2VecHelper.load(fp)
         kv = Word2VecHelper.load(fp, keyed_vectors=True)
 
+    encoded = kv.encode("hello world")
+
     assert isinstance(wv.model, Word2Vec)
     assert isinstance(wv2.model, Word2Vec)
     assert isinstance(kv.model, KeyedVectors)
+    assert encoded.any()
+
+
```

### Comparing `datawords-0.7.0/tests/test_parsers.py` & `datawords-0.7.1/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/tests/test_rankings.py` & `datawords-0.7.1/tests/test_rankings.py`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/tests/texts.txt` & `datawords-0.7.1/tests/texts.txt`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/.gitignore` & `datawords-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/LICENSE` & `datawords-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/README.md` & `datawords-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/pyproject.toml` & `datawords-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datawords-0.7.0/PKG-INFO` & `datawords-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawords
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library to work with text data
 Project-URL: Documentation, https://github.com/unknown/datawords#readme
 Project-URL: Issues, https://github.com/unknown/datawords/issues
 Project-URL: Source, https://github.com/unknown/datawords
 Author-email: Xavier Petit <nuxion@gmail.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
```

