# Comparing `tmp/prefect-lakefs-0.1.0.tar.gz` & `tmp/prefect-lakefs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-lakefs/prefect-lakefs/dist/.tmp-91e7597u/prefect-lakefs-0.1.0.tar", last modified: Mon May  8 21:00:56 2023, max compression
+gzip compressed data, was "prefect-lakefs-0.2.0.tar", last modified: Mon Jul 24 22:29:30 2023, max compression
```

## Comparing `prefect-lakefs-0.1.0.tar` & `prefect-lakefs-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/prefect_lakefs/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/prefect_lakefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/prefect_lakefs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/prefect_lakefs/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/prefect_lakefs/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/prefect_lakefs/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/prefect_lakefs/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/prefect_lakefs/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/prefect_lakefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/prefect_lakefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/prefect_lakefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/prefect_lakefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/prefect_lakefs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/prefect_lakefs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/prefect_lakefs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:00:56.000000 prefect-lakefs-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/tests/test_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-08 20:59:29.000000 prefect-lakefs-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:30.597977 prefect-lakefs-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-24 22:29:30.597977 prefect-lakefs-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:30.601976 prefect-lakefs-0.2.0/prefect_lakefs/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 22:29:30.601976 prefect-lakefs-0.2.0/prefect_lakefs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/commits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/prefect_lakefs/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:30.597977 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-24 22:29:30.000000 prefect-lakefs-0.2.0/prefect_lakefs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 22:29:30.601976 prefect-lakefs-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 22:29:30.597977 prefect-lakefs-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_commits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-07-24 22:28:42.000000 prefect-lakefs-0.2.0/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `prefect-lakefs-0.1.0/LICENSE` & `prefect-lakefs-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `prefect-lakefs-0.1.0/PKG-INFO` & `prefect-lakefs-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-lakefs
-Version: 0.1.0
+Version: 0.2.0
 Summary: Prefect integrations for interacting with LakeFS services.
 Home-page: https://github.com/limx0/prefect-lakefs
 Author: limx0
 Author-email: limx0@example.com
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -78,15 +78,15 @@
 
 ```python
 import asyncio
 
 from prefect_lakefs.credentials import LakeFSCredentials
 from prefect_lakefs.tasks import list_branches
 
-# You can configure this while adding a block in the prefect-ui or 
+# You can configure this while adding a block in the prefect-ui or
 #   you can save the block using .save() utility method provided by the block.
 lakefs_creds = LakeFSCredentials(
         endpoint_url="http://localhost:8000/api/v1",
         access_key_id="AKIAIOSFODNN7EXAMPLE",
         secret_access_key="wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY",
     ).save("lakefs-creds")
 
@@ -94,15 +94,15 @@
 @flow
 def list_branches_for_example_repo():
     branches = list_branches(
         lakefs_credentials=LakeFSCredentials.load("lakefs-creds"),
         repository="example",
     )
     print(branches)
- 
+
 
 
 if __name__ == "__main__":
     # run the flow
     asyncio.run(list_branches())
 ```
```

### Comparing `prefect-lakefs-0.1.0/README.md` & `prefect-lakefs-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ```python
 import asyncio
 
 from prefect_lakefs.credentials import LakeFSCredentials
 from prefect_lakefs.tasks import list_branches
 
-# You can configure this while adding a block in the prefect-ui or 
+# You can configure this while adding a block in the prefect-ui or
 #   you can save the block using .save() utility method provided by the block.
 lakefs_creds = LakeFSCredentials(
         endpoint_url="http://localhost:8000/api/v1",
         access_key_id="AKIAIOSFODNN7EXAMPLE",
         secret_access_key="wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY",
     ).save("lakefs-creds")
 
@@ -70,15 +70,15 @@
 @flow
 def list_branches_for_example_repo():
     branches = list_branches(
         lakefs_credentials=LakeFSCredentials.load("lakefs-creds"),
         repository="example",
     )
     print(branches)
- 
+
 
 
 if __name__ == "__main__":
     # run the flow
     asyncio.run(list_branches())
 ```
```

### Comparing `prefect-lakefs-0.1.0/prefect_lakefs/branches.py` & `prefect-lakefs-0.2.0/prefect_lakefs/branches.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
     Args:
         lakefs_credentials: `LakeFSCredentials` block for creating
             authenticated LakeFS API clients.
         repository: name of a lakefs repository.
         branch: name of the branch to apply revert.
         revert_ref: string value of a ref to revert.
         parent_number: number representing parent index(based 1) to pick
-            incase of reverting merge commits. Defaults to 1.
+            in case of reverting merge commits. Defaults to 1.
         **lakefs_kwargs: Optional extra keyword arguments to pass to the LakeFS API.
 
     Returns:
         None
 
     Example:
         revert changes on a branch named `feature` for repository named `example`:
```

### Comparing `prefect-lakefs-0.1.0/prefect_lakefs/credentials.py` & `prefect-lakefs-0.2.0/prefect_lakefs/credentials.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,27 +46,34 @@
         title="LakeFS Access Key Secret",
     )
     endpoint_url: Optional[str] = Field(
         default="http://localhost:8000/api/v1",
         description="A LakeFS URL.",
         title="LakeFS URL",
     )
-
+    repository: Optional[str] = Field(
+        description="Default LakeFS repository to use.",
+        title="Default LakeFS repository",
+    )
+    branch: Optional[str] = Field(
+        description="Default LakeFS branch to use.",
+        title="Default LakeFS branch",
+    )
     _block_type_name = "LakeFS Credentials"
     _block_type_slug = "lakefs-credentials"
     # TODO: add lakefs logo_url
     _logo_url = "https://styles.redditmedia.com/t5_57y5vj/styles/communityIcon_oapa1t4myyu71.png?width=256&v=enabled&s=d3319b91ef0a5eea78e46242e07f2034834f31f7"  # noqa
     # TODO: add LakeFSCredentials doc slug
     _documentation_url = "https://prefecthq.github.io"  # noqa
     _documentation_url = "https://limx0.github.io/prefect-lakefs/credentials/#prefect_lakefs.credentials.LakeFSCredentials"  # noqa
 
     @contextmanager
     def get_client(
         self,
-        client_type: Literal["branches", "commits", "objects"],
+        client_type: Literal["branches", "commits", "objects", "repository"],
     ) -> Generator[LakeFSClient, None, None]:
         """Convenience method for retrieving a LakeFS API client for deployment resources.
 
         Args:
             client_type: The resource-specific type of LakeFS client to retrieve.
 
         Yields:
```

### Comparing `prefect-lakefs-0.1.0/prefect_lakefs/storage.py` & `prefect-lakefs-0.2.0/prefect_lakefs/storage.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from lakefs_client.model.commit_creation import CommitCreation
 from prefect.context import FlowRunContext
 from prefect_aws import S3Bucket
 from pydantic import Field
 
 from prefect_lakefs.credentials import LakeFSCredentials
-from prefect_lakefs.git import commit_sha, get_git_repo
 
 
 class LakeFS(S3Bucket):
     _block_type_name = "LakeFS"
 
     credentials: LakeFSCredentials = Field(
         description="A block containing your credentials to AWS or MinIO.",
@@ -19,52 +18,39 @@
     def _get_s3_client(self):
         # return self.credentials.get_client()
         raise NotImplementedError(
             "Should be using LakeFS client via `self.credentials.get_client()`"
         )
 
     def _write_sync(self, key: str, data: bytes) -> None:
-        client = self.credentials.objects_api
-        branch = self.credentials.ref or commit_sha()
-
-        with io.BytesIO(data) as stream:
-            client.upload_object(
-                repository=self.credentials.repository,
-                branch=branch,
-                path=key,
-                content=stream,
-                metadata={""},
-            )
-        if self.credentials.commit_on_task:
-            self.commit_changes()
+        with self.credentials.get_client("objects") as client:
+            with io.BytesIO(data) as stream:
+                stream.name = key
+                client.upload_object(
+                    repository=self.credentials.repository,
+                    branch=self.credentials.branch,
+                    path=key,
+                    content=stream,
+                )
+        # if self.credentials.commit_on_task:
+        #     self.commit_changes()
 
     def _read_sync(self, key: str) -> None:
         client = self.credentials.objects_api
         data = client.get_object(
             repository=self.credentials.repository,
             ref=self._get_branch(),
             path=key,
         )
         return data
 
     def commit_changes(self):
-        if self.credentials.strict_no_dirty:
-            git_repo = get_git_repo()
-            assert (
-                not git_repo.is_dirty()
-            ), "Repo has uncommitted changes, cannot commit data."
-
         repository = self.credentials.repository
         branch: str = self.credentials.branch
         assert branch, "If committing, `branch` must be set in `LakeFsCredentials`"
         commits_api = self.credentials.commits_api
         run_context: FlowRunContext = FlowRunContext.get()
         metadata = {
             "flow_run_id": run_context.flow.id,
         }
-        if self.credentials.mirror_git_repo:
-            git_repo = get_git_repo()
-            sha = commit_sha(git_repo)
-            metadata = {"git_sha": sha}
-
         commit = CommitCreation("prefect-lakefs commit", metadata=metadata)
         commits_api.commit(repository=repository, branch=branch, commit_creation=commit)
```

### Comparing `prefect-lakefs-0.1.0/prefect_lakefs.egg-info/PKG-INFO` & `prefect-lakefs-0.2.0/prefect_lakefs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-lakefs
-Version: 0.1.0
+Version: 0.2.0
 Summary: Prefect integrations for interacting with LakeFS services.
 Home-page: https://github.com/limx0/prefect-lakefs
 Author: limx0
 Author-email: limx0@example.com
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -78,15 +78,15 @@
 
 ```python
 import asyncio
 
 from prefect_lakefs.credentials import LakeFSCredentials
 from prefect_lakefs.tasks import list_branches
 
-# You can configure this while adding a block in the prefect-ui or 
+# You can configure this while adding a block in the prefect-ui or
 #   you can save the block using .save() utility method provided by the block.
 lakefs_creds = LakeFSCredentials(
         endpoint_url="http://localhost:8000/api/v1",
         access_key_id="AKIAIOSFODNN7EXAMPLE",
         secret_access_key="wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY",
     ).save("lakefs-creds")
 
@@ -94,15 +94,15 @@
 @flow
 def list_branches_for_example_repo():
     branches = list_branches(
         lakefs_credentials=LakeFSCredentials.load("lakefs-creds"),
         repository="example",
     )
     print(branches)
- 
+
 
 
 if __name__ == "__main__":
     # run the flow
     asyncio.run(list_branches())
 ```
```

### Comparing `prefect-lakefs-0.1.0/prefect_lakefs.egg-info/SOURCES.txt` & `prefect-lakefs-0.2.0/prefect_lakefs.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -5,20 +5,24 @@
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 prefect_lakefs/__init__.py
 prefect_lakefs/_version.py
 prefect_lakefs/branches.py
+prefect_lakefs/commits.py
 prefect_lakefs/credentials.py
-prefect_lakefs/git.py
+prefect_lakefs/objects.py
 prefect_lakefs/storage.py
 prefect_lakefs/tasks.py
 prefect_lakefs.egg-info/PKG-INFO
 prefect_lakefs.egg-info/SOURCES.txt
 prefect_lakefs.egg-info/dependency_links.txt
 prefect_lakefs.egg-info/entry_points.txt
 prefect_lakefs.egg-info/requires.txt
 prefect_lakefs.egg-info/top_level.txt
 tests/test_block_standards.py
 tests/test_branches.py
-tests/test_credentials.py
+tests/test_commits.py
+tests/test_credentials.py
+tests/test_objects.py
+tests/test_storage.py
```

### Comparing `prefect-lakefs-0.1.0/setup.cfg` & `prefect-lakefs-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.1.0/setup.py` & `prefect-lakefs-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.1.0/tests/test_block_standards.py` & `prefect-lakefs-0.2.0/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.1.0/tests/test_branches.py` & `prefect-lakefs-0.2.0/tests/test_branches.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.1.0/tests/test_credentials.py` & `prefect-lakefs-0.2.0/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-lakefs-0.1.0/versioneer.py` & `prefect-lakefs-0.2.0/versioneer.py`

 * *Files identical despite different names*

