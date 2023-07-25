# Comparing `tmp/httplus-0.1.0.tar.gz` & `tmp/httplus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httplus-0.1.0.tar", max compression
+gzip compressed data, was "httplus-0.1.1.tar", max compression
```

## Comparing `httplus-0.1.0.tar` & `httplus-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-05-28 07:57:55.312570 httplus-0.1.0/LICENSE
--rw-r--r--   0        0        0     1267 2023-05-31 08:40:24.812091 httplus-0.1.0/README.md
--rw-r--r--   0        0        0       47 2023-05-30 11:55:36.148288 httplus-0.1.0/httplus/__init__.py
--rw-r--r--   0        0        0     3464 2023-05-30 10:58:20.428873 httplus-0.1.0/httplus/client.py
--rw-r--r--   0        0        0     1872 2023-05-30 09:13:58.586047 httplus-0.1.0/httplus/request.py
--rw-r--r--   0        0        0     1161 2023-05-30 09:17:26.535355 httplus-0.1.0/httplus/response.py
--rw-r--r--   0        0        0      398 2023-05-31 08:38:03.138203 httplus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 httplus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-28 07:57:55.312570 httplus-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1374 2023-05-31 11:47:23.520807 httplus-0.1.1/README.md
+-rw-r--r--   0        0        0       47 2023-05-30 11:55:36.148288 httplus-0.1.1/httplus/__init__.py
+-rw-r--r--   0        0        0     4273 2023-07-25 11:00:03.840090 httplus-0.1.1/httplus/client.py
+-rw-r--r--   0        0        0     2215 2023-07-19 11:08:10.521237 httplus-0.1.1/httplus/request.py
+-rw-r--r--   0        0        0     1174 2023-07-25 11:33:29.457438 httplus-0.1.1/httplus/response.py
+-rw-r--r--   0        0        0      398 2023-07-25 11:25:32.674275 httplus-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 httplus-0.1.1/PKG-INFO
```

### Comparing `httplus-0.1.0/LICENSE` & `httplus-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `httplus-0.1.0/README.md` & `httplus-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # HTTPlus
 
 An HTTP asynchronous client.
 
+[![Stable Version](https://img.shields.io/pypi/v/httplus?label=pypi)](https://pypi.org/project/httplus/)
+
+
 
 ## Instalation
 ```shell
 pip install httplus
 ```
 
 ## Basic Usage
```

### Comparing `httplus-0.1.0/httplus/request.py` & `httplus-0.1.1/httplus/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,42 +8,45 @@
             method: str = 'GET',
             headers: dict = None
     ):
         self.url = url
         self.host = ''
         self.port = 80
         self.uri = ''
-        self.headers = headers or {}
         self.method = method
-        self.version = 'http/1.1'
+        self.version = 'HTTP/1.1'
         self.body: bytes = b''
         self.issecurity = True
         self.prepare_host()
+        self.headers = self.generate_headers(headers or {})
 
     def prepare_host(self):
         if self.url.startswith('http://'):
             self.issecurity = False
             size = 7
+        elif self.url.startswith('www'):
+            size = 0
         else:
             size = 8
         splt = self.url[size:].split('/', maxsplit=1)
         self.uri = f'/{splt[1]}' if len(splt) > 1 else '/'
         host_port_splt = splt[0].split(':')
         if len(host_port_splt) > 1:
             self.port = int(host_port_splt[1])
         else:
-            self.port = 433 if self.issecurity else 80
+            self.port = 443 if self.issecurity else 80
         self.host = host_port_splt[0]
 
     def render(self) -> bytes:
         headers = '\r\n'.join([f'{k}:{v}' for k, v in self.headers.items()])
         content = f'{self.method} {self.uri} {self.version}\r\n{headers}\r\n'
         content = content.encode()
+        content += b'\r\n'
         if self.body:
-            content += b'\r\n' + self.body
+            content += self.body
         return content
 
     def set_data(self, data: ... = None):
         if not data:
             self.body = b''
             return
         if content_type := self.headers.get('Content-Type', ''):
@@ -54,7 +57,16 @@
                 case _:
                     self.body = data
         else:
             body = json.dumps(data)
             self.body = body.encode()
             self.headers['Content-Type'] = 'application/json'
             self.headers['Content-Length'] = len(self.body)
+
+    def generate_headers(self, headers: dict):
+        n_headers = {
+            'Host': self.host,
+            'User-Agent': 'httplus/0.1.1',
+            'Accept': '*/*'
+        }
+        n_headers.update(headers)
+        return n_headers
```

### Comparing `httplus-0.1.0/httplus/response.py` & `httplus-0.1.1/httplus/response.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.status = int(status)
         self.message = message[:-4]
         self.version = version
 
     def set_header_pair(self, line: bytes):
         self.raw += line
         key, value = line.decode().split(':', maxsplit=1)
-        self.headers[key] = value
+        self.headers[key] = value[:-2].strip()
         if key == 'Content-Type':
             self.content_type = value
         elif key == 'Content-Length':
             self.content_length = int(value)
 
     def set_body(self, line: bytes):
         self.body = line
```

