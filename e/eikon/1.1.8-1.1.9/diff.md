# Comparing `tmp/eikon-1.1.8.tar.gz` & `tmp/eikon-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\eikon-1.1.8.tar", last modified: Wed Nov 25 23:07:15 2020, max compression
+gzip compressed data, was "eikon-1.1.9.tar", last modified: Wed Mar 10 21:45:53 2021, max compression
```

## Comparing `eikon-1.1.8.tar` & `eikon-1.1.9.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxrwx   0        0        0        0 2020-11-25 23:07:15.000000 eikon-1.1.8/
--rw-rw-rw-   0        0        0     2475 2020-11-24 12:20:39.000000 eikon-1.1.8/CHANGES.txt
--rw-rw-rw-   0        0        0      561 2020-09-10 12:47:05.000000 eikon-1.1.8/LICENSE.md
--rw-rw-rw-   0        0        0    14739 2020-11-25 23:07:15.000000 eikon-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     6627 2020-09-10 12:47:05.000000 eikon-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2020-11-25 23:07:14.000000 eikon-1.1.8/eikon/
--rw-rw-rw-   0        0        0    10212 2020-09-25 12:54:38.000000 eikon-1.1.8/eikon/Profile.py
--rw-rw-rw-   0        0        0      685 2020-11-24 08:26:06.000000 eikon-1.1.8/eikon/__init__.py
--rw-rw-rw-   0        0        0     9626 2020-09-10 12:47:05.000000 eikon-1.1.8/eikon/data_grid.py
--rw-rw-rw-   0        0        0      567 2020-09-10 12:47:05.000000 eikon-1.1.8/eikon/eikonError.py
--rw-rw-rw-   0        0        0    11657 2020-11-23 07:31:09.000000 eikon-1.1.8/eikon/json_requests.py
--rw-rw-rw-   0        0        0     7591 2020-11-24 17:52:37.000000 eikon-1.1.8/eikon/news_request.py
-drwxrwxrwx   0        0        0        0 2020-11-25 23:07:15.000000 eikon-1.1.8/eikon/streaming_session/
--rw-rw-rw-   0        0        0      195 2020-09-10 12:47:05.000000 eikon-1.1.8/eikon/streaming_session/__init__.py
--rw-rw-rw-   0        0        0     4257 2020-09-10 12:47:05.000000 eikon-1.1.8/eikon/streaming_session/cache.py
--rw-rw-rw-   0        0        0     9689 2020-11-23 10:00:09.000000 eikon-1.1.8/eikon/streaming_session/desktop_session.py
--rw-rw-rw-   0        0        0     2200 2020-09-10 12:47:05.000000 eikon-1.1.8/eikon/streaming_session/istream_callback.py
--rw-rw-rw-   0        0        0    14937 2020-10-14 07:09:00.000000 eikon-1.1.8/eikon/streaming_session/itemstream.py
--rw-rw-rw-   0        0        0    25763 2020-10-14 07:09:11.000000 eikon-1.1.8/eikon/streaming_session/session.py
--rw-rw-rw-   0        0        0     7879 2020-10-14 07:09:00.000000 eikon-1.1.8/eikon/streaming_session/stream.py
--rw-rw-rw-   0        0        0    19607 2020-09-10 12:47:05.000000 eikon-1.1.8/eikon/streaming_session/stream_connection.py
--rw-rw-rw-   0        0        0      925 2020-09-10 12:47:05.000000 eikon-1.1.8/eikon/streaming_session/streaming_connection_config.py
--rw-rw-rw-   0        0        0    14279 2020-10-14 07:09:00.000000 eikon-1.1.8/eikon/streaming_session/streamingprice.py
--rw-rw-rw-   0        0        0     2252 2020-09-10 12:47:05.000000 eikon-1.1.8/eikon/streaming_session/streamingprice_callback.py
--rw-rw-rw-   0        0        0    13760 2020-10-14 07:09:00.000000 eikon-1.1.8/eikon/streaming_session/streamingprices.py
--rw-rw-rw-   0        0        0     5158 2020-11-23 14:10:52.000000 eikon-1.1.8/eikon/symbology.py
--rw-rw-rw-   0        0        0    14239 2020-11-23 14:16:11.000000 eikon-1.1.8/eikon/time_series.py
--rw-rw-rw-   0        0        0     3864 2020-09-10 12:47:05.000000 eikon-1.1.8/eikon/tools.py
-drwxrwxrwx   0        0        0        0 2020-11-25 23:07:14.000000 eikon-1.1.8/eikon.egg-info/
--rw-rw-rw-   0        0        0    14739 2020-11-25 23:07:13.000000 eikon-1.1.8/eikon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      886 2020-11-25 23:07:13.000000 eikon-1.1.8/eikon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-11-25 23:07:13.000000 eikon-1.1.8/eikon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-09-25 12:56:45.000000 eikon-1.1.8/eikon.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      135 2020-11-25 23:07:13.000000 eikon-1.1.8/eikon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2020-11-25 23:07:13.000000 eikon-1.1.8/eikon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-11-25 23:07:15.000000 eikon-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2282 2020-11-24 18:13:13.000000 eikon-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-03-10 21:45:53.935999 eikon-1.1.9/
+-rw-rw-rw-   0        0        0      561 2020-09-10 12:45:46.000000 eikon-1.1.9/LICENSE.md
+-rw-rw-rw-   0        0        0     8029 2021-03-10 21:45:53.933997 eikon-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6627 2020-09-10 12:45:46.000000 eikon-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2021-03-10 21:45:53.847860 eikon-1.1.9/eikon/
+-rw-rw-rw-   0        0        0    10778 2021-02-05 07:19:46.000000 eikon-1.1.9/eikon/Profile.py
+-rw-rw-rw-   0        0        0      685 2021-03-10 15:32:04.000000 eikon-1.1.9/eikon/__init__.py
+-rw-rw-rw-   0        0        0     9689 2021-02-05 07:19:46.000000 eikon-1.1.9/eikon/data_grid.py
+-rw-rw-rw-   0        0        0      567 2020-04-21 20:10:15.000000 eikon-1.1.9/eikon/eikonError.py
+-rw-rw-rw-   0        0        0    10987 2021-02-05 07:19:46.000000 eikon-1.1.9/eikon/json_requests.py
+-rw-rw-rw-   0        0        0     7591 2021-01-15 06:03:25.000000 eikon-1.1.9/eikon/news_request.py
+drwxrwxrwx   0        0        0        0 2021-03-10 21:45:53.927992 eikon-1.1.9/eikon/streaming_session/
+-rw-rw-rw-   0        0        0      195 2020-04-21 20:10:15.000000 eikon-1.1.9/eikon/streaming_session/__init__.py
+-rw-rw-rw-   0        0        0     4257 2020-04-21 20:10:15.000000 eikon-1.1.9/eikon/streaming_session/cache.py
+-rw-rw-rw-   0        0        0     9689 2021-01-15 06:03:25.000000 eikon-1.1.9/eikon/streaming_session/desktop_session.py
+-rw-rw-rw-   0        0        0     2200 2020-04-21 20:10:15.000000 eikon-1.1.9/eikon/streaming_session/istream_callback.py
+-rw-rw-rw-   0        0        0    14937 2021-01-15 06:02:09.000000 eikon-1.1.9/eikon/streaming_session/itemstream.py
+-rw-rw-rw-   0        0        0    25763 2021-03-10 21:22:22.000000 eikon-1.1.9/eikon/streaming_session/session.py
+-rw-rw-rw-   0        0        0     7879 2021-01-15 06:02:09.000000 eikon-1.1.9/eikon/streaming_session/stream.py
+-rw-rw-rw-   0        0        0    19607 2020-04-21 20:10:15.000000 eikon-1.1.9/eikon/streaming_session/stream_connection.py
+-rw-rw-rw-   0        0        0      925 2020-04-21 20:10:15.000000 eikon-1.1.9/eikon/streaming_session/streaming_connection_config.py
+-rw-rw-rw-   0        0        0    14279 2021-01-15 06:02:09.000000 eikon-1.1.9/eikon/streaming_session/streamingprice.py
+-rw-rw-rw-   0        0        0     2252 2020-04-21 20:10:15.000000 eikon-1.1.9/eikon/streaming_session/streamingprice_callback.py
+-rw-rw-rw-   0        0        0    14507 2021-01-26 21:56:01.000000 eikon-1.1.9/eikon/streaming_session/streamingprices.py
+-rw-rw-rw-   0        0        0     5158 2021-01-15 06:03:25.000000 eikon-1.1.9/eikon/symbology.py
+-rw-rw-rw-   0        0        0    14239 2021-01-15 06:03:25.000000 eikon-1.1.9/eikon/time_series.py
+-rw-rw-rw-   0        0        0     3864 2020-09-10 12:45:46.000000 eikon-1.1.9/eikon/tools.py
+drwxrwxrwx   0        0        0        0 2021-03-10 21:45:53.876998 eikon-1.1.9/eikon.egg-info/
+-rw-rw-rw-   0        0        0     8029 2021-03-10 21:45:53.000000 eikon-1.1.9/eikon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      874 2021-03-10 21:45:53.000000 eikon-1.1.9/eikon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-03-10 21:45:53.000000 eikon-1.1.9/eikon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-01-15 06:09:39.000000 eikon-1.1.9/eikon.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      123 2021-03-10 21:45:53.000000 eikon-1.1.9/eikon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2021-03-10 21:45:53.000000 eikon-1.1.9/eikon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-03-10 21:45:53.936992 eikon-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2255 2021-02-05 07:21:23.000000 eikon-1.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `eikon-1.1.8/LICENSE.md` & `eikon-1.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/README.md` & `eikon-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/Profile.py` & `eikon-1.1.9/eikon/Profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,7 +348,16 @@
     def check_profile(self):
         if self.port is not None:
             self.logger.info('Port {} on local proxy was detected'.format(self.get_port_number()))
         else:
             # port number wasn't identified => raise EikonError exception
             self.logger.error('Port number was not identified.\nCheck if Eikon Desktop or Eikon API Proxy is running.')
             raise EikonError(-1, 'Port number was not identified. Check if Eikon Desktop or Eikon API Proxy is running.')
+
+    def send_request(self, json, timeout=None):
+        response = self._desktop_session.http_request(url=self.get_url(),
+                                                      method="POST",
+                                                      headers={'Content-Type': 'application/json',
+                                                               'x-tr-applicationid': self.get_app_key()},
+                                                      json=json,
+                                                      timeout=timeout)
+        return response
```

### Comparing `eikon-1.1.8/eikon/__init__.py` & `eikon-1.1.9/eikon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding: utf-8
-__version__ = '1.1.8'
+__version__ = '1.1.9'
 
 """
     Eikon Data API for Python allows your Python applications to access Refinitiv data directly from Eikon.
     Its usage requires:
         - An App Key (you can create it wit App Key Generator in Eikon Desktop)
         - Eikon Desktop or Refinitiv Workspace application running on your local machine
```

### Comparing `eikon-1.1.8/eikon/data_grid.py` & `eikon-1.1.9/eikon/data_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,16 @@
     elif value is dict:
         return value['value']
     else:
         return value
 
 
 def get_data_frame(data_dict, field_name=False):
+    if 'headers' not in data_dict:
+        return None, None
     if field_name:
         headers = [header.get('field', header.get('displayName')) for header in data_dict['headers'][0]]
     else:
         headers = [header['displayName'] for header in data_dict['headers'][0]]
     data = numpy.array([[get_data_value(value) for value in row] for row in data_dict['data']])
     if len(data):
         df = pd.DataFrame(data, columns=headers)
```

### Comparing `eikon-1.1.8/eikon/eikonError.py` & `eikon-1.1.9/eikon/eikonError.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/json_requests.py` & `eikon-1.1.9/eikon/json_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,19 +82,15 @@
             raise e
 
         network_error = False
         try:
             # build the request
             udf_request = {'Entity': {'E': entity, 'W': data} }
             logger.debug('Request:{}'.format(udf_request))
-            response = profile._desktop_session.http_request(url=profile.get_url(),
-                                                             method="POST",
-                                                             headers={'Content-Type': 'application/json',
-                                                                      'x-tr-applicationid': profile.get_app_key()},
-                                                             json=udf_request)
+            response = profile.send_request(json=udf_request)
             try:
                 logger.debug('HTTP Response code: {}'.format(response.status_code))
                 logger.debug('HTTP Response: {}'.format(response.text))
             except UnicodeEncodeError as unicode_error:
                 _response = json.dumps(response.text, ensure_ascii=False).encode('utf8')
                 logger.debug(f'HTTP Response unicode: {_response}')
 
@@ -111,20 +107,15 @@
                     ticket = _check_ticket_async(result)
                     while ticket:
                         ticket_request = {'Entity': {
                                              'E': entity,
                                              'W': {'requests': [{'ticket': ticket}]}
                                          }}
                         logger.debug('Send ticket request:{}'.format(ticket_request))
-                        response = profile._desktop_session.http_request(url=profile.get_url(),
-                                                                         method="POST",
-                                                                         headers={'Content-Type': 'application/json',
-                                                                                  'x-tr-applicationid': profile.get_app_key()},
-                                                                         json=ticket_request,
-                                                                         timeout=(15.0, 15.0))
+                        response = profile.send_request(json=ticket_request, timeout=(15.0, 15.0))
 
                         try:
                             logger.debug(f'HTTP Response: {response.status_code} - {response.text}')
                         except UnicodeEncodeError:
                             _response = json.dumps(response.text, ensure_ascii=False).encode('utf8')
                             logger.debug(f'HTTP Response unicode: {_response}')
                         result = response.json()
@@ -134,25 +125,29 @@
                 return result
             else:
                 _raise_for_status(response)
         except httpx.TimeoutException as timeout_exception:
             error_msg = f'HTTP TimeoutException: {timeout_exception}.'
             logger.error(error_msg)
             raise EikonError(408, error_msg)
+        except EikonError as eikon_err:
+            logger.error(f"HTTP request failed: {type(eikon_err).__name__}-{eikon_err.message}")
+            raise EikonError(eikon_err.code, eikon_err.message)
         except httpx.ConnectTimeout as connect_timeout:
             logger.debug(f'HTTP ConnectTimeout: {connect_timeout}')
             network_error = True
         except httpx.HTTPError as http_error:
             logger.debug(f'HTTP Error: {http_error}')
             network_error = True
         except httpx.DecodingError as decoding_error:
             logger.debug(f'HTTP DecodingError: {decoding_error}')
             network_error = True
         except Exception as e:
-            logger.error(f"HTTP request failed: {type(e).__name__}-{e.message}")
+            message = getattr(e, 'message', None) or e
+            logger.error(f"HTTP request failed: {type(e).__name__}-{message}")
         if network_error:
             error_msg = 'Eikon Proxy not running or cannot be reached. Please read the documentation on troubleshooting'
             logger.error(error_msg)
             raise EikonError(401, error_msg)
 
 
 def _check_ticket_async(server_response):
```

### Comparing `eikon-1.1.8/eikon/news_request.py` & `eikon-1.1.9/eikon/news_request.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/streaming_session/cache.py` & `eikon-1.1.9/eikon/streaming_session/cache.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/streaming_session/desktop_session.py` & `eikon-1.1.9/eikon/streaming_session/desktop_session.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/streaming_session/istream_callback.py` & `eikon-1.1.9/eikon/streaming_session/istream_callback.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/streaming_session/itemstream.py` & `eikon-1.1.9/eikon/streaming_session/itemstream.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/streaming_session/session.py` & `eikon-1.1.9/eikon/streaming_session/session.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/streaming_session/stream.py` & `eikon-1.1.9/eikon/streaming_session/stream.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/streaming_session/stream_connection.py` & `eikon-1.1.9/eikon/streaming_session/stream_connection.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/streaming_session/streaming_connection_config.py` & `eikon-1.1.9/eikon/streaming_session/streaming_connection_config.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/streaming_session/streamingprice.py` & `eikon-1.1.9/eikon/streaming_session/streamingprice.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/streaming_session/streamingprice_callback.py` & `eikon-1.1.9/eikon/streaming_session/streamingprice_callback.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/streaming_session/streamingprices.py` & `eikon-1.1.9/eikon/streaming_session/streamingprices.py`

 * *Files 9% similar despite different names*

```diff
@@ -133,22 +133,25 @@
             self._streaming_prices[name] = StreamingPrice(session=self._session,
                                                           name=name,
                                                           fields=self._fields,
                                                           service=self._service,
                                                           on_refresh=self._on_refresh,
                                                           on_update=self._on_update,
                                                           on_status=self._on_status,
-                                                          on_complete=self._on_complete)
+                                                          on_complete=self._on_complete
+                                                          )
         self._on_refresh_cb = on_refresh
         self._on_status_cb = on_status
         self._on_update_cb = on_update
         self._on_complete_cb = on_complete
 
         self._state = StreamState.Closed
-        self._complete_event_nb = 0
+
+        #   set universe of on_complete 
+        self._on_complete_set = None
 
     @property
     def state(self):
         return self._state
 
     ###################################################
     #  Access to StreamingPrices as a dict            #
@@ -202,15 +205,16 @@
         Open asynchronously the streaming price
         """
         self._session.log(1, f'StreamingPrices : open streaming on {self.params.instruments}')
         if self._state == StreamState.Open:
             return
 
         self._state = StreamState.Pending
-        self._complete_event_nb = 0
+        self._on_complete_set = set()
+
         task_list = [stream.open_async(with_updates=with_updates) for stream in self._streaming_prices.values()]
         await asyncio.wait(task_list, return_when=asyncio.ALL_COMPLETED)
         self._state = StreamState.Open
         self._session.log(1, f'StreamingPrices : start asynchrously streaming on {self.params.instruments} done')
         return self._state
 
     def close(self):
@@ -312,34 +316,47 @@
                 self._session._loop.call_soon_threadsafe(self._on_refresh_cb, self, stream.name, message)
                 # self._on_refresh_cb(self, name, message)
             except Exception as e:
                 self._session.log(logging.ERROR, f'StreamingPrices on_refresh callback raised exception: {e!r}')
                 self._session.log(1, f'Traceback : {sys.exc_info()[2]}')
 
     def _on_status(self, stream, status):
+
         if self._on_status_cb:
             try:
                 self._session.log(1, 'StreamingPrices : call on_status callback')
                 self._session._loop.call_soon_threadsafe(self._on_status_cb, self, stream.name, status)
             except Exception as e:
                 self._session.log(logging.ERROR, f'StreamingPrices on_status callback raised exception: {e!r}')
                 self._session.log(1, f'Traceback : {sys.exc_info()[2]}')
 
+        #   check for closed stream when status "Closed", "ClosedRecover", "NonStreaming" or "Redirect"
+        if stream.state == StreamState.Closed and stream.name not in self._on_complete_set:
+            #   this stream has been closed, so it means completed also
+            self._on_complete(stream)
+
     def _on_update(self, stream, update):
         if self._on_update_cb:
             try:
                 self._session.log(1, 'StreamingPrices : call on_update callback')
                 self._session._loop.call_soon_threadsafe(self._on_update_cb, self, stream.name, update)
             except Exception as e:
                 self._session.log(logging.ERROR, f'StreamingPrices on_update callback raised exception: {e!r}')
                 self._session.log(1, f'Traceback : {sys.exc_info()[2]}')
 
     def _on_complete(self, stream):
-        self._complete_event_nb += 1
-        if self._complete_event_nb == len(self.params.instruments):
-            if self._on_complete_cb:
-                try:
-                    self._session.log(1, 'StreamingPrices : call on_complete callback')
-                    self._session._loop.call_soon_threadsafe(self._on_complete_cb, self)
-                except Exception as e:
-                    self._session.log(logging.ERROR, f'StreamingPrices on_complete callback raised exception: {e!r}')
-                    self._session.log(1, f'Traceback : {sys.exc_info()[2]}')
+        assert self._on_complete_set is not None
+
+        #   check for update completed set
+        if stream.name not in self._on_complete_set:
+            #   update the stream to be in complete list
+            self._on_complete_set.update([stream.name, ])
+
+            #   check for complete for all subscribe universe
+            if self._on_complete_set == set(self.params.instruments):
+                if self._on_complete_cb:
+                    try:
+                        self._session.log(1, 'StreamingPrices : call on_complete callback')
+                        self._session._loop.call_soon_threadsafe(self._on_complete_cb, self)
+                    except Exception as e:
+                        self._session.log(logging.ERROR, f'StreamingPrices on_complete callback raised exception: {e!r}')
+                        self._session.log(1, f'Traceback : {sys.exc_info()[2]}')
```

### Comparing `eikon-1.1.8/eikon/symbology.py` & `eikon-1.1.9/eikon/symbology.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/time_series.py` & `eikon-1.1.9/eikon/time_series.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon/tools.py` & `eikon-1.1.9/eikon/tools.py`

 * *Files identical despite different names*

### Comparing `eikon-1.1.8/eikon.egg-info/SOURCES.txt` & `eikon-1.1.9/eikon.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-CHANGES.txt
 LICENSE.md
 README.md
 setup.py
 eikon/Profile.py
 eikon/__init__.py
 eikon/data_grid.py
 eikon/eikonError.py
```

### Comparing `eikon-1.1.8/setup.py` & `eikon-1.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,19 +38,19 @@
       description='Python package for retrieving Eikon data.',
       long_description=read_md('README.md'),
       long_description_content_type=description_content_type,
       url='https://developers.refinitiv.com/eikon-apis/eikon-data-api',
       author='REFINITIV',
       author_email='',
       license='Apache 2.0',
-      data_files=[("", ["LICENSE.md", "CHANGES.txt"])],
+      data_files=[("", ["LICENSE.md"])],
       packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
       zip_safe=False,
-      install_requires=['httpx<0.15',
-                        'nest_asyncio<1.4.0,>=1.3.0',
+      install_requires=['httpx',
+                        'nest_asyncio>=1.5.1',
                         'datetime',
                         'pandas>=1.0.0',
                         'numpy>=1.11.0',
                         'appdirs>=1.4.3',
                         'python-dateutil',
                         'websocket-client',
                         'deprecation'],
```

