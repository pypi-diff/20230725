# Comparing `tmp/devchat_ask-0.0.2-py3-none-any.whl.zip` & `tmp/devchat_ask-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 15383 bytes, number of entries: 21
+Zip file size: 15418 bytes, number of entries: 21
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 chat/__init__.py
 -rw-r--r--  2.0 unx      133 b- defN 80-Jan-01 00:00 chat/ask_codebase/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/__init__.py
--rw-r--r--  2.0 unx     1876 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/simple_qa.py
--rw-r--r--  2.0 unx     2445 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/stuff_dc_qa.py
+-rw-r--r--  2.0 unx     1926 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/simple_qa.py
+-rw-r--r--  2.0 unx     2495 b- defN 80-Jan-01 00:00 chat/ask_codebase/chains/stuff_dc_qa.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/__init__.py
 -rw-r--r--  2.0 unx     1821 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/embedding.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/__init__.py
 -rw-r--r--  2.0 unx      259 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/base.py
 -rw-r--r--  2.0 unx     4798 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/file.py
 -rw-r--r--  2.0 unx     5422 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/loader/function.py
 -rw-r--r--  2.0 unx      364 b- defN 80-Jan-01 00:00 chat/ask_codebase/indexing/util.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/__init__.py
 -rw-r--r--  2.0 unx     1254 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/file.py
 -rw-r--r--  2.0 unx     7383 b- defN 80-Jan-01 00:00 chat/ask_codebase/store/qdrant.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 chat/util/__init__.py
 -rw-r--r--  2.0 unx      718 b- defN 80-Jan-01 00:00 chat/util/decorator.py
 -rw-r--r--  2.0 unx     3359 b- defN 80-Jan-01 00:00 chat/util/misc.py
--rw-r--r--  2.0 unx     4085 b- defN 80-Jan-01 00:00 devchat_ask-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 devchat_ask-0.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1821 b- defN 16-Jan-01 00:00 devchat_ask-0.0.2.dist-info/RECORD
-21 files, 35826 bytes uncompressed, 12361 bytes compressed:  65.5%
+-rw-r--r--  2.0 unx     4085 b- defN 80-Jan-01 00:00 devchat_ask-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 devchat_ask-0.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1821 b- defN 16-Jan-01 00:00 devchat_ask-0.0.3.dist-info/RECORD
+21 files, 35926 bytes uncompressed, 12396 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -48,17 +48,17 @@
 
 Filename: chat/util/decorator.py
 Comment: 
 
 Filename: chat/util/misc.py
 Comment: 
 
-Filename: devchat_ask-0.0.2.dist-info/METADATA
+Filename: devchat_ask-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: devchat_ask-0.0.2.dist-info/WHEEL
+Filename: devchat_ask-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: devchat_ask-0.0.2.dist-info/RECORD
+Filename: devchat_ask-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chat/ask_codebase/chains/simple_qa.py

```diff
@@ -17,27 +17,29 @@
     llm: BaseLanguageModel = ChatOpenAI(temperature=0.1, model_name="gpt-4")  # type: ignore
     reduce_llm: BaseLanguageModel = ChatOpenAI(  # type: ignore
         temperature=0.1, model_name="gpt-4"
     )
 
     def __init__(
         self,
-        source_name: str,
-        embedding_cls: Type[Embeddings],
+        # source_name: str,
+        # embedding_cls: Type[Embeddings],
+        q: Q,
     ) -> None:
-        self._source_name = source_name
-        self._embedding_cls = embedding_cls
+        # self._source_name = source_name
+        # self._embedding_cls = embedding_cls
+        self._q = q
 
         self._chain: Optional[Chain] = None
 
     @property
     def chain(self) -> Chain:
         if self._chain is None:
-            q = Q.reuse(self._source_name, self._embedding_cls)
-            retriver = q.qdrant.as_retriever(
+            # q = Q.reuse(self._source_name, self._embedding_cls)
+            retriver = self._q.qdrant.as_retriever(
                 search_type="similarity", search_kwargs={"k": 20}
             )
             chain: BaseRetrievalQA = RetrievalQA.from_chain_type(
                 llm=self.llm,
                 chain_type_kwargs={
                     "reduce_llm": self.reduce_llm,
                 },
```

## chat/ask_codebase/chains/stuff_dc_qa.py

```diff
@@ -29,23 +29,25 @@
 
 
 class StuffDocumentCodeQa:
     llm: BaseLanguageModel = ChatOpenAI(temperature=0.1)  # type: ignore
 
     def __init__(
         self,
-        source_name: str,
-        embedding_cls: Type[Embeddings],
+        # source_name: str,
+        # embedding_cls: Type[Embeddings],
+        q: Q,
     ) -> None:
-        self._source_name = source_name
-        self._embedding_cls = embedding_cls
+        # self._source_name = source_name
+        # self._embedding_cls = embedding_cls
+        self._q = q
 
     def run(self, question: str) -> Tuple[str, List[Document]]:
-        q = Q.reuse(self._source_name, self._embedding_cls)
-        qdrant = q.qdrant
+        # q = Q.reuse(self._source_name, self._embedding_cls)
+        qdrant = self._q.qdrant
 
         potential_found_docs = qdrant.similarity_search(
             question,
             k=50,
         )
 
         enc = tiktoken.encoding_for_model("gpt-4")
```

## Comparing `devchat_ask-0.0.2.dist-info/METADATA` & `devchat_ask-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devchat-ask
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: Hezheng Yin
 Author-email: hezheng@merico.dev
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: instructorembedding (>=1.0.1,<2.0.0)
```

## Comparing `devchat_ask-0.0.2.dist-info/RECORD` & `devchat_ask-0.0.3.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 chat/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chat/ask_codebase/__init__.py,sha256=60EyVGMNUL04Rz8ZeY5jI2cxyLz9Ilyh-uNGCptUNoQ,133
 chat/ask_codebase/chains/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-chat/ask_codebase/chains/simple_qa.py,sha256=Vrt3ifN_lePlV8HtBQwTvl8EFK3RQGlfQiOEO99lZxQ,1876
-chat/ask_codebase/chains/stuff_dc_qa.py,sha256=qhnAo62MlbpXtc_-Ps2Mxj6Hul1o-i89sDoPfsH-Hng,2445
+chat/ask_codebase/chains/simple_qa.py,sha256=uu9f4mErUUoewTiZQ_UjlijUn3B-qo4gc5_9fhaqULM,1926
+chat/ask_codebase/chains/stuff_dc_qa.py,sha256=MHg7BV64DqIdBvA_8S1yQ9Xd18jhxnr1DEMWdxCvymw,2495
 chat/ask_codebase/indexing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chat/ask_codebase/indexing/embedding.py,sha256=kJO6GyXgZDW69zdDT3W5W-A_KMJ2Ag_3w-bDBu3RrZA,1821
 chat/ask_codebase/indexing/loader/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chat/ask_codebase/indexing/loader/base.py,sha256=NM2CYwOC72OIJDp_HKpwdrQNPiWU0U_UUNat77kdYwM,259
 chat/ask_codebase/indexing/loader/file.py,sha256=q_KLUzjJTlElwum2AZmtMaVwp2SwKwhU_58dUJ5yh6Y,4798
 chat/ask_codebase/indexing/loader/function.py,sha256=tli2EQWLh8KOwbVJuVSIFYv-WeIVGiQQR7I_P1U7LHE,5422
 chat/ask_codebase/indexing/util.py,sha256=e03by30E499cTkfdWKPmOQ6RHcXPTjnzRlFRAHKAuYU,364
 chat/ask_codebase/store/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chat/ask_codebase/store/file.py,sha256=UzJhj41pw0OUbWwnNFITfTLrYQFnaFK_Z89IL-_COis,1254
 chat/ask_codebase/store/qdrant.py,sha256=lKtK2eaEMcawAuU9vl3lJXxx2Tbt4ZvZ1_tJAYgofak,7383
 chat/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chat/util/decorator.py,sha256=VPq0NiX_5fc_egGGR6OuUjXkdWwRczmaQOwHyt4qVIk,718
 chat/util/misc.py,sha256=-QlIRZBXF9KjgBAwLnBKeraAzZ9L9Tyt_cn1c7hJFiU,3359
-devchat_ask-0.0.2.dist-info/METADATA,sha256=yupYOtBzlxMdYBu0rTmlX5nkKbMgjG4lG8NI-qcAh28,4085
-devchat_ask-0.0.2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-devchat_ask-0.0.2.dist-info/RECORD,,
+devchat_ask-0.0.3.dist-info/METADATA,sha256=7wSPLfE0kX771Y--hjFTi8EKt_LDE5ogwdOT-n3Jt48,4085
+devchat_ask-0.0.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+devchat_ask-0.0.3.dist-info/RECORD,,
```

