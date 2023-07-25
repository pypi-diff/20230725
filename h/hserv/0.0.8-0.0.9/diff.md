# Comparing `tmp/hserv-0.0.8.tar.gz` & `tmp/hserv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hserv-0.0.8.tar", last modified: Fri Jul 21 15:51:22 2023, max compression
+gzip compressed data, was "hserv-0.0.9.tar", last modified: Sat Jul 22 12:20:45 2023, max compression
```

## Comparing `hserv-0.0.8.tar` & `hserv-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:22.498094 hserv-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-21 15:51:09.000000 hserv-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-21 15:51:09.000000 hserv-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-21 15:51:22.498094 hserv-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-21 15:51:09.000000 hserv-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:22.498094 hserv-0.0.8/hserv/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5753 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:22.498094 hserv-0.0.8/hserv/supabase/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/supabase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/supabase/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    10742 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/supabase/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:22.498094 hserv-0.0.8/hserv/webproxy/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/webproxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-07-21 15:51:09.000000 hserv-0.0.8/hserv/webproxy/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 15:51:22.498094 hserv-0.0.8/hserv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-21 15:51:22.000000 hserv-0.0.8/hserv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-21 15:51:22.000000 hserv-0.0.8/hserv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 15:51:22.000000 hserv-0.0.8/hserv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-21 15:51:22.000000 hserv-0.0.8/hserv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-21 15:51:22.000000 hserv-0.0.8/hserv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-21 15:51:09.000000 hserv-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 15:51:22.498094 hserv-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-21 15:51:09.000000 hserv-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:20:45.202990 hserv-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-22 12:20:31.000000 hserv-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-22 12:20:31.000000 hserv-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-22 12:20:45.202990 hserv-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-22 12:20:31.000000 hserv-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:20:45.198990 hserv-0.0.9/hserv/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-22 12:20:31.000000 hserv-0.0.9/hserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-22 12:20:31.000000 hserv-0.0.9/hserv/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5753 2023-07-22 12:20:31.000000 hserv-0.0.9/hserv/server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:20:45.202990 hserv-0.0.9/hserv/supabase/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-22 12:20:31.000000 hserv-0.0.9/hserv/supabase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-07-22 12:20:31.000000 hserv-0.0.9/hserv/supabase/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-07-22 12:20:31.000000 hserv-0.0.9/hserv/supabase/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:20:45.202990 hserv-0.0.9/hserv/webproxy/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-22 12:20:31.000000 hserv-0.0.9/hserv/webproxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-07-22 12:20:31.000000 hserv-0.0.9/hserv/webproxy/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 12:20:45.198990 hserv-0.0.9/hserv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-22 12:20:45.000000 hserv-0.0.9/hserv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-22 12:20:45.000000 hserv-0.0.9/hserv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 12:20:45.000000 hserv-0.0.9/hserv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-22 12:20:45.000000 hserv-0.0.9/hserv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-22 12:20:45.000000 hserv-0.0.9/hserv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-22 12:20:31.000000 hserv-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-22 12:20:45.202990 hserv-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-07-22 12:20:31.000000 hserv-0.0.9/setup.py
```

### Comparing `hserv-0.0.8/LICENSE` & `hserv-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hserv-0.0.8/hserv/server.py` & `hserv-0.0.9/hserv/server.py`

 * *Files identical despite different names*

### Comparing `hserv-0.0.8/hserv/supabase/config.py` & `hserv-0.0.9/hserv/supabase/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 import yaml
 
 if TYPE_CHECKING:
     from .controller import SupabaseController
 
 
 ENV_LOOKUP: Dict[str, List[str]] = dict(
-    pg_password=["POSTGRES_PASSWORD"],
+    postgres_password=["POSTGRES_PASSWORD"],
     jwt_secret=["JWT_SECRET"],
     anon_jwt=["ANON_KEY"],
     service_jwt=["SERVICE_ROLE_KEY"],
     public_url=["SITE_URL"],
     site_url=["SITE_URL"],
     api_url=["SUPABASE_PUBLIC_URL", "API_EXTERNAL_URL"],
-    pg_port=["POSTGRES_PORT"],
+    postgres_port=["POSTGRES_PORT"],
     public_port=["STUDIO_PORT"],
     api_port=["KONG_HTTP_PORT"],
 )
 
 @dataclass
 class SupabaseConfig:
     controller: 'SupabaseController' = field(repr=False)
@@ -34,18 +34,19 @@
         # create buffers for the config
         envBuf = io.StringIO()
         kongBuf = io.StringIO()
 
         # load the config into buffer
         self.controller.server.get(self._env_path, envBuf)
         self.controller.server.get(self._kong_path, kongBuf)
+        kongBuf.seek(0)
 
         # set as attributes
         self._env = envBuf.getvalue()
-        self._kong = yaml.load(kongBuf, Loader=yaml.FullLoader)
+        self._kong = yaml.load(kongBuf, Loader=yaml.Loader)
 
     def save(self):
         # load the current config into buffers
         envBuf = io.StringIO(self._env)
         kongBuf = io.StringIO()
         yaml.dump(self._kong, kongBuf)
 
@@ -84,12 +85,12 @@
         if not all([n in self._env for n in names]):
             raise AttributeError(f"Attribute '{name}' is not a valid environment configuration value.")
         
         # still here means replace the config
         env = self._env
         for n in names:
             # get the current value
-            current_val = getattr(self, n)
+            current_val = self.get(n)
             env.replace(f"{n}={current_val}", f"{n}={value}")
         
         # finally set the new env
         self._env = env
```

### Comparing `hserv-0.0.8/hserv/supabase/controller.py` & `hserv-0.0.9/hserv/supabase/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     project: str
     path: str = field(default=os.path.expanduser('~'))
     docker_path: str = field(init=False, repr=False)
     server: HydrocodeServer = field(default_factory=HydrocodeServer, repr=False)
     quiet: bool = field(default=False, repr=False)
     jwt_secret: str = field(init=False, repr=False)
 
-    pg_password: str = field(init=False, repr=False)
-    pg_port: int = field(init=False, repr=False)
+    postgres_password: str = field(init=False, repr=False)
+    postgres_port: int = field(init=False, repr=False)
 
     # development only, this will be configured later, and derived from the project
     public_url: str = field(default="localhost")
     public_port: int = field(default=3000, repr=False)
     kong_port: int = field(init=False, repr=False)
 
     def __post_init__(self):      
@@ -147,16 +147,16 @@
 
     def reload_config(self):
         # get the config
         config = self.config
 
         # sync the settings
         self.jwt_secret = config['jwt_secret']
-        self.pg_password = config['postgres_password']
-        self.pg_port = config['postgres_port']
+        self.postgres_password = config['postgres_password']
+        self.postgres_port = config['postgres_port']
         self.kong_port = config['kong_port']
         self.public_port = config['public_port']
 
     @property
     def is_downloaded(self):
         # check if the supabase docker folder exists
         return self.server.exists(os.path.join(self.path, 'supabase', 'docker'))
@@ -167,15 +167,15 @@
         envBuf = io.BytesIO()
         self.server.get(os.path.join(self.docker_path, '.env'), envBuf)
         
         # get the conf as string
         conf = envBuf.getvalue().decode()
         
         # make sure the passwords match
-        return self.pg_password in conf and self.jwt_secret in conf
+        return self.postgres_password in conf and self.jwt_secret in conf
 
     @property
     def site_url(self):
         if self.public_port == 80:
             return self.public_url
         else:
             return f"{self.public_url}:{self.public_port}"
@@ -216,16 +216,16 @@
     def update_supabase_config(self, jwt=False, postgres=False, domain=False):
         # instantiate a Config object
         conf = SupabaseConfig(self)
         
         # update the postgres password
         if postgres:
             # set the password
-            conf.set('pg_password',  self.pg_password)
-            conf.set('pg_port', self.pg_port)
+            conf.set('postgres_password',  self.postgres_password)
+            conf.set('postgres_port', self.postgres_port)
         
         # update the jwt secret
         if jwt:
             # replace jwt secret
             conf.set('jwt_secret',  self.jwt_secret)
 
             # repalce the api keys in the environment file
```

### Comparing `hserv-0.0.8/setup.py` & `hserv-0.0.9/setup.py`

 * *Files identical despite different names*

