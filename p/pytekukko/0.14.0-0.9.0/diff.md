# Comparing `tmp/pytekukko-0.14.0.tar.gz` & `tmp/pytekukko-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytekukko-0.14.0.tar", last modified: Tue Jul 25 14:59:21 2023, max compression
+gzip compressed data, was "pytekukko-0.9.0.tar", last modified: Mon Dec  6 09:48:11 2021, max compression
```

## Comparing `pytekukko-0.14.0.tar` & `pytekukko-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:59:21.498803 pytekukko-0.14.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-25 14:59:08.000000 pytekukko-0.14.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-25 14:59:08.000000 pytekukko-0.14.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-25 14:59:08.000000 pytekukko-0.14.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-07-25 14:59:21.498803 pytekukko-0.14.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-25 14:59:08.000000 pytekukko-0.14.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-25 14:59:08.000000 pytekukko-0.14.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:59:21.494804 pytekukko-0.14.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 14:59:08.000000 pytekukko-0.14.0/requirements/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-25 14:59:08.000000 pytekukko-0.14.0/requirements/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:59:21.498803 pytekukko-0.14.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:59:21.490804 pytekukko-0.14.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:59:21.494804 pytekukko-0.14.0/src/pytekukko/
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-07-25 14:59:08.000000 pytekukko-0.14.0/src/pytekukko/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:59:21.494804 pytekukko-0.14.0/src/pytekukko/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-25 14:59:08.000000 pytekukko-0.14.0/src/pytekukko/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1113 2023-07-25 14:59:08.000000 pytekukko-0.14.0/src/pytekukko/examples/print_collection_schedules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-07-25 14:59:08.000000 pytekukko-0.14.0/src/pytekukko/examples/print_invoice_headers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-07-25 14:59:08.000000 pytekukko-0.14.0/src/pytekukko/examples/print_next_collections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6690 2023-07-25 14:59:08.000000 pytekukko-0.14.0/src/pytekukko/examples/update_google_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 14:59:08.000000 pytekukko-0.14.0/src/pytekukko/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-25 14:59:08.000000 pytekukko-0.14.0/src/pytekukko/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:59:08.000000 pytekukko-0.14.0/src/pytekukko/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:59:21.494804 pytekukko-0.14.0/src/pytekukko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-07-25 14:59:21.000000 pytekukko-0.14.0/src/pytekukko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-25 14:59:21.000000 pytekukko-0.14.0/src/pytekukko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:59:21.000000 pytekukko-0.14.0/src/pytekukko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 14:59:21.000000 pytekukko-0.14.0/src/pytekukko.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-25 14:59:21.000000 pytekukko-0.14.0/src/pytekukko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 14:59:21.000000 pytekukko-0.14.0/src/pytekukko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:59:21.498803 pytekukko-0.14.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 14:59:08.000000 pytekukko-0.14.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:59:21.498803 pytekukko-0.14.0/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-25 14:59:08.000000 pytekukko-0.14.0/tests/cassettes/test_get_collection_schedule.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-07-25 14:59:08.000000 pytekukko-0.14.0/tests/cassettes/test_get_invoice_headers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   112493 2023-07-25 14:59:08.000000 pytekukko-0.14.0/tests/cassettes/test_login_logout.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   107146 2023-07-25 14:59:08.000000 pytekukko-0.14.0/tests/cassettes/test_logout.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-25 14:59:08.000000 pytekukko-0.14.0/tests/test_pytekukko.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:48:11.426420 pytekukko-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     3419 2021-12-06 09:48:06.000000 pytekukko-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-12-06 09:48:06.000000 pytekukko-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-06 09:48:06.000000 pytekukko-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2870 2021-12-06 09:48:11.426420 pytekukko-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2071 2021-12-06 09:48:06.000000 pytekukko-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2021-12-06 09:48:06.000000 pytekukko-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2845 2021-12-06 09:48:11.426420 pytekukko-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2021-12-06 09:48:06.000000 pytekukko-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:48:11.422420 pytekukko-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:48:11.422420 pytekukko-0.9.0/src/pytekukko/
+-rw-r--r--   0 runner    (1001) docker     (121)     5976 2021-12-06 09:48:06.000000 pytekukko-0.9.0/src/pytekukko/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:48:11.426420 pytekukko-0.9.0/src/pytekukko/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2342 2021-12-06 09:48:06.000000 pytekukko-0.9.0/src/pytekukko/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1057 2021-12-06 09:48:06.000000 pytekukko-0.9.0/src/pytekukko/examples/print_collection_schedules.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      976 2021-12-06 09:48:06.000000 pytekukko-0.9.0/src/pytekukko/examples/print_invoice_headers.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1000 2021-12-06 09:48:06.000000 pytekukko-0.9.0/src/pytekukko/examples/print_next_collections.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6852 2021-12-06 09:48:06.000000 pytekukko-0.9.0/src/pytekukko/examples/update_google_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2235 2021-12-06 09:48:06.000000 pytekukko-0.9.0/src/pytekukko/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:48:11.422420 pytekukko-0.9.0/src/pytekukko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2870 2021-12-06 09:48:11.000000 pytekukko-0.9.0/src/pytekukko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      787 2021-12-06 09:48:11.000000 pytekukko-0.9.0/src/pytekukko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-06 09:48:11.000000 pytekukko-0.9.0/src/pytekukko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2021-12-06 09:48:11.000000 pytekukko-0.9.0/src/pytekukko.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-12-06 09:48:11.000000 pytekukko-0.9.0/src/pytekukko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-06 09:48:11.000000 pytekukko-0.9.0/src/pytekukko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:48:11.426420 pytekukko-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-06 09:48:06.000000 pytekukko-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 09:48:11.426420 pytekukko-0.9.0/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (121)     6438 2021-12-06 09:48:06.000000 pytekukko-0.9.0/tests/cassettes/test_get_collection_schedule.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     9629 2021-12-06 09:48:06.000000 pytekukko-0.9.0/tests/cassettes/test_get_invoice_headers.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5323 2021-12-06 09:48:06.000000 pytekukko-0.9.0/tests/cassettes/test_login.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   106105 2021-12-06 09:48:06.000000 pytekukko-0.9.0/tests/cassettes/test_logout.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     4088 2021-12-06 09:48:06.000000 pytekukko-0.9.0/tests/test_pytekukko.py
```

### Comparing `pytekukko-0.14.0/LICENSE` & `pytekukko-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytekukko-0.14.0/README.md` & `pytekukko-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 - `pytekukko-next-collections`: output next collection dates in JSON
 - `pytekukko-update-google-calendar`: update Google Calendar with
   events for next collections
 
 ## Disclaimer
 
 This package is not supported by or endorsed by Jätekukko. Do not
-bother them with questions or issues related to it.
+bother them with issues related to it.
```

### Comparing `pytekukko-0.14.0/src/pytekukko/__init__.py` & `pytekukko-0.9.0/src/pytekukko/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 """Jätekukko Omakukko client."""
 
-from contextlib import suppress
-from datetime import date
-from datetime import datetime as dt
+from datetime import date, datetime
 from http import HTTPStatus
-from typing import Any, cast
+from typing import Any, Dict, List, Union, cast
 from urllib.parse import urljoin
-from zoneinfo import ZoneInfo
 
 from aiohttp import ClientResponse, ClientResponseError, ClientSession
 
-from .exceptions import UnexpectedResponseStructureError
 from .models import CustomerData, InvoiceHeader, Service
 
-__version__ = "0.14.0"
+__version__ = "0.9.0"
 DEFAULT_BASE_URL = "https://tilasto.jatekukko.fi/jatekukko/"
 
-SERVICE_TIMEZONE = ZoneInfo("Europe/Helsinki")
-"""Assumed time zone of timestamps in data from service."""
-
 
 class Pytekukko:
     """Client for accessing Jätekukko Omakukko services."""
 
     def __init__(
         self,
         session: ClientSession,
@@ -32,156 +25,146 @@
     ):
         """Set up client."""
         self.session = session
         self.customer_number = customer_number
         self.password = password
         self.base_url = base_url
 
-    async def get_customer_data(self) -> dict[str, list[CustomerData]]:
+    async def get_customer_data(self) -> Dict[str, List[CustomerData]]:
         """Get customer data."""
         url = urljoin(self.base_url, "secure/get_customer_datas.do")
 
         response_data = await self._request_with_retry(method="GET", url=url)
 
         return {
             customer_number: [CustomerData(raw_data=a_data) for a_data in data]
             for customer_number, data in _unmarshal(response_data).items()
         }
 
-    async def get_services(self) -> list[Service]:
+    async def get_services(self) -> List[Service]:
         """Get services."""
         url = urljoin(self.base_url, "secure/get_services_by_customer_numbers.do")
         params = {"customerNumbers[]": self.customer_number}
 
         response_data = await self._request_with_retry(
-            method="GET",
-            url=url,
-            params=params,
+            method="GET", url=url, params=params
         )
-        if not isinstance(response_data, list | tuple):
-            raise UnexpectedResponseStructureError(response_data)
+        assert isinstance(response_data, (list, tuple))
 
         return [Service(raw_data=_unmarshal(service)) for service in response_data]
 
-    async def get_collection_schedule(self, what: Service | int) -> list[date]:
-        """Get collection schedule for a service.
+    async def get_collection_schedule(self, what: Union[Service, int]) -> List[date]:
+        """
+        Get collection schedule for a service.
 
         :param what: the service or a "pos" value of one to get schedule for
         """
         url = urljoin(self.base_url, "get_collection_schedule.do")
         pos = what.pos if isinstance(what, Service) else what
         params = {"customerNumber": self.customer_number, "pos": pos}
 
         response_data = await self._request_with_retry(
-            method="GET",
-            url=url,
-            params=params,
+            method="GET", url=url, params=params
         )
 
-        return cast(list[date], _unmarshal(response_data))
+        return cast(List[date], _unmarshal(response_data))
 
-    async def get_invoice_headers(self) -> list[InvoiceHeader]:
+    async def get_invoice_headers(self) -> List[InvoiceHeader]:
         """Get headers of available invoices."""
         url = urljoin(self.base_url, "secure/get_invoice_headers_for_customer.do")
         params = {
             "customerId": self.customer_number,  # yep, customerId, not *Number here
         }
 
         response_data = await self._request_with_retry(
-            method="GET",
-            url=url,
-            params=params,
+            method="GET", url=url, params=params
         )
-        if not isinstance(response_data, list | tuple):
-            raise UnexpectedResponseStructureError(response_data)
+        assert isinstance(response_data, (list, tuple))
 
         return [
             InvoiceHeader(raw_data=_unmarshal(invoice_header))
             for invoice_header in response_data
         ]
 
-    async def login(self) -> dict[str, str]:
+    async def login(self) -> Dict[str, str]:
         """Log in."""
         url = urljoin(self.base_url, "j_acegi_security_check")
         headers = (("X-Requested-With", "XMLHttpRequest"),)
         params = {"target": "2"}
         data = {"j_username": self.customer_number, "j_password": self.password}
 
         async with self.session.post(
-            url,
-            headers=headers,
-            params=params,
-            data=data,
-            raise_for_status=True,
+            url, headers=headers, params=params, data=data, raise_for_status=True
         ) as response:
-            # NOTE(scop): could check that we got {"response":"OK"}
-            return cast(dict[str, str], await response.json())
+            # TODO(scop): Check we got {"response":"OK"}?
+            return cast(Dict[str, str], await response.json())
 
     async def logout(self) -> None:
         """Log out the current session."""
         url = urljoin(self.base_url, "j_acegi_logout_elcustrap")
 
         async with self.session.get(url, raise_for_status=True) as response:
             await _drain(response)
 
     async def _request_with_retry(self, **request_kwargs: Any) -> Any:
-        """Do a request, with automatic login and retry if session is logged out.
+        """
+        Do a request, with automatic login and retry if session is logged out.
 
         :param raise_for_first_status: whether first unsuccessful status should raise;
             False allows for handling special cases that give errors instead of
             redirecting to login page
         :param request_kwargs: kwargs to pass to self.session.request
         """
         try:
             async with self.session.request(
-                **request_kwargs,
-                raise_for_status=True,
+                **request_kwargs, raise_for_status=True
             ) as response:
                 if response.history and response.url.path.endswith("/login.do"):
                     await _drain(response)
                 else:
                     return await response.json()
         except ClientResponseError as ex:
             if not (
                 ex.status in (HTTPStatus.BAD_REQUEST, HTTPStatus.INTERNAL_SERVER_ERROR)
                 and "get_collection_schedule" in ex.request_info.url.path
             ):
                 raise
 
         _ = await self.login()
         async with self.session.request(
-            **request_kwargs,
-            raise_for_status=True,
+            **request_kwargs, raise_for_status=True
         ) as response:
             return await response.json()
 
 
 def _unmarshal(data: Any) -> Any:
-    """Unmarshal items in parsed JSON to more specific objects.
+    """
+    Unmarshal items in parsed JSON to more specific objects.
 
     :param data: parsed JSON data
     :return: unmarshalled data
     """
     if isinstance(data, dict):
         for key, value in data.items():
             data[key] = _unmarshal(value)
     elif isinstance(data, list):
         for i, value in enumerate(data):
             data[i] = _unmarshal(value)
     elif isinstance(data, str):
         try:
-            parsed = dt.strptime(data, "%Y-%m-%d").replace(tzinfo=SERVICE_TIMEZONE)
-            data = parsed.date()
+            data = datetime.strptime(data, "%Y-%m-%d").date()
         except ValueError:
-            with suppress(ValueError):
-                parsed = dt.strptime(data, "%H:%M").replace(tzinfo=SERVICE_TIMEZONE)
-                data = parsed.time()
+            try:
+                data = datetime.strptime(data, "%H:%M").time()
+            except ValueError:
+                pass
     return data
 
 
 async def _drain(response: ClientResponse) -> None:
-    """Consume and discard response.
+    """
+    Consume and discard response.
 
     Useful for keeping the connection alive without caring about response content.
     """
     async for _ in response.content.iter_chunked(1024):
         pass
```

### Comparing `pytekukko-0.14.0/src/pytekukko/examples/__init__.py` & `pytekukko-0.9.0/src/pytekukko/examples/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,45 @@
 """Pytekukko examples."""
 
 import os
 import sys
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
+from typing import Dict, Optional, Tuple
 
+import dotenv
 from aiohttp import ClientSession, CookieJar
-from dotenv import find_dotenv, load_dotenv
 
 from pytekukko import Pytekukko
 
 
 def arg_environ_default(
-    key: str,
-    *,
-    optional: bool = False,
-    fallback: str | None = None,
-) -> dict[str, str | None]:
+    key: str, optional: bool = False, fallback: Optional[str] = None
+) -> Dict[str, Optional[str]]:
     """Get kwargs for environment backed argument addition."""
     help_text = f"default: ${key} from environment"
     if optional:
         help_text += " (optional)"
     if fallback:
         help_text += f", or {fallback}"
     return {
         "default": os.environ.get(key, fallback),
         "help": help_text,
     }
 
 
-def load_pytekukko_dotenv() -> bool:
-    """Load our .env."""
-    return load_dotenv(os.environ.get("PYTEKUKKO_DOTENV", find_dotenv(usecwd=True)))
-
-
 def example_argparser(description: str) -> ArgumentParser:
     """Set up example argument parser."""
-    _ = load_pytekukko_dotenv()
+    dotenv.load_dotenv()
 
     argparser = ArgumentParser(
         description=description,
         epilog=(
-            "Environment variable defaults are loaded from the path set in "
-            "$PYTEKUKKO_DOTENV in environment, falling back to .env if not set. "
-            "If the path is relative, it is searched in directories starting from the "
-            "current directory, walking towards the file system root."
+            "Environment variable defaults are loaded from .env "
+            "in the current directory."
         ),
     )
     argparser.add_argument(
         "--customer-number",
         type=str,
         **arg_environ_default("PYTEKUKKO_CUSTOMER_NUMBER"),  # type: ignore[arg-type]
     )
@@ -57,29 +48,29 @@
         type=str,
         **arg_environ_default("PYTEKUKKO_PASSWORD"),  # type: ignore[arg-type]
     )
     argparser.add_argument(
         "--cookie-jar-file",
         type=str,
         **arg_environ_default(  # type: ignore[arg-type]
-            "PYTEKUKKO_COOKIE_JAR_FILE",
-            optional=True,
+            "PYTEKUKKO_COOKIE_JAR_FILE", optional=True
         ),
     )
 
     return argparser
 
 
-def example_client(args: Namespace) -> tuple[Pytekukko, CookieJar, Path | None]:
+def example_client(args: Namespace) -> Tuple[Pytekukko, CookieJar, Optional[Path]]:
     """Set up example client."""
+
     if not args.customer_number:
-        print("customer number required", file=sys.stderr)  # noqa: T201
+        print("customer number required", file=sys.stderr)
         sys.exit(2)
     if not args.password:
-        print("password required", file=sys.stderr)  # noqa: T201
+        print("password required", file=sys.stderr)
         sys.exit(2)
     cookie_jar = CookieJar()
     cookie_jar_path = None
     if args.cookie_jar_file:
         cookie_jar_path = Path(args.cookie_jar_file)
         if cookie_jar_path.exists():
             cookie_jar.load(cookie_jar_path)
```

### Comparing `pytekukko-0.14.0/src/pytekukko/examples/print_collection_schedules.py` & `pytekukko-0.9.0/src/pytekukko/examples/print_collection_schedules.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,33 +6,35 @@
 import json
 
 from pytekukko.examples import example_argparser, example_client
 
 
 async def run_example() -> None:
     """Run the example."""
+
     client, cookie_jar, cookie_jar_path = example_client(
-        example_argparser(__doc__).parse_args(),
+        example_argparser(__doc__).parse_args()
     )
 
     data = []
     async with client.session:
         services = await client.get_services()
         for service in services:
-            if schedule := await client.get_collection_schedule(service):
-                data.append(  # noqa: PERF401 # negligible, hairy with list comprehension
+            schedule = await client.get_collection_schedule(service)
+            if schedule:
+                data.append(
                     {
                         "name": service.name,
                         "collection_schedule": [x.isoformat() for x in schedule],
-                    },
+                    }
                 )
         if not cookie_jar_path:
             await client.logout()
 
-    print(json.dumps(data))  # noqa: T201
+    print(json.dumps(data))
 
     if cookie_jar_path:
         cookie_jar.save(cookie_jar_path)
 
 
 def main() -> None:
     """Run example in event loop."""
```

### Comparing `pytekukko-0.14.0/src/pytekukko/examples/print_invoice_headers.py` & `pytekukko-0.9.0/src/pytekukko/examples/print_invoice_headers.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,31 +6,33 @@
 import json
 
 from pytekukko.examples import example_argparser, example_client
 
 
 async def run_example() -> None:
     """Run the example."""
+
     client, cookie_jar, cookie_jar_path = example_client(
-        example_argparser(__doc__).parse_args(),
+        example_argparser(__doc__).parse_args()
     )
 
+    data = []
     async with client.session:
-        data = [
-            {
-                "name": invoice_header.name,
-                "due_date": invoice_header.due_date.isoformat(),
-                "total": invoice_header.total,
-            }
-            for invoice_header in await client.get_invoice_headers()
-        ]
+        for invoice_header in await client.get_invoice_headers():
+            data.append(
+                {
+                    "name": invoice_header.name,
+                    "due_date": invoice_header.due_date.isoformat(),
+                    "total": invoice_header.total,
+                }
+            )
         if not cookie_jar_path:
             await client.logout()
 
-    print(json.dumps(data))  # noqa: T201
+    print(json.dumps(data))
 
     if cookie_jar_path:
         cookie_jar.save(cookie_jar_path)
 
 
 def main() -> None:
     """Run example in event loop."""
```

### Comparing `pytekukko-0.14.0/src/pytekukko/examples/print_next_collections.py` & `pytekukko-0.9.0/src/pytekukko/examples/print_next_collections.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,31 +6,33 @@
 import json
 
 from pytekukko.examples import example_argparser, example_client
 
 
 async def run_example() -> None:
     """Run the example."""
+
     client, cookie_jar, cookie_jar_path = example_client(
-        example_argparser(__doc__).parse_args(),
+        example_argparser(__doc__).parse_args()
     )
 
+    data = []
     async with client.session:
-        data = [
-            {
-                "name": service.name,
-                "collection_date": service.next_collection.isoformat(),
-            }
-            for service in await client.get_services()
-            if service.next_collection
-        ]
+        services = await client.get_services()
+        for service in (x for x in services if x.next_collection):
+            data.append(
+                {
+                    "name": service.name,
+                    "collection_date": service.next_collection.isoformat(),  # type: ignore[union-attr]
+                }
+            )
         if not cookie_jar_path:
             await client.logout()
 
-    print(json.dumps(data))  # noqa: T201
+    print(json.dumps(data))
 
     if cookie_jar_path:
         cookie_jar.save(cookie_jar_path)
 
 
 def main() -> None:
     """Run example in event loop."""
```

### Comparing `pytekukko-0.14.0/src/pytekukko/examples/update_google_calendar.py` & `pytekukko-0.9.0/src/pytekukko/examples/update_google_calendar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 #!/usr/bin/env python3
 
-"""Update Google Calendar with events for next collections.
+"""
+Update Google Calendar with events for next collections.
 
 To get the required service account file, enable the Google Calendar API
 in the Google Cloud console, create service account credentials with
 access to it, and create keys of type JSON.
 
 Calendar id is typically the target Google Calendar account e-mail
 address.
 """
 
 import asyncio
 import datetime
 import logging
 import sys
-import zoneinfo
-from collections.abc import Mapping
-from typing import Any, NamedTuple, cast
+from typing import Any, Dict, Mapping, NamedTuple, cast
+
+try:
+    import zoneinfo  # type: ignore[import]
+except ImportError:  # Python < 3.9
+    from backports import zoneinfo  # type: ignore[import]
 
-from google.oauth2 import service_account  # type: ignore[import]
-from googleapiclient.discovery import build  # type: ignore[import]
+from google.oauth2 import service_account  # type: ignore
+from googleapiclient.discovery import build  # type: ignore
 
 from pytekukko.examples import arg_environ_default, example_argparser, example_client
 
 logging.basicConfig(level=logging.INFO)
 LOGGER = logging.getLogger(__name__)
 
 
@@ -32,15 +36,15 @@
 
     name: str
     date: datetime.date
     location: str
 
 
 # https://developers.google.com/resources/api-libraries/documentation/calendar/v3/python/latest/calendar_v3.events.html
-def update_google_calendar(
+def update_google_calendar(  # pylint: disable=too-many-locals
     credentials: service_account.Credentials,
     calendar_id: str,
     data: Mapping[str, CalendarData],
 ) -> None:
     """Update the calendar."""
     service = build(
         "calendar",
@@ -49,45 +53,48 @@
         # https://github.com/googleapis/google-api-python-client/issues/299
         # https://github.com/googleapis/google-api-python-client/issues/325
         cache_discovery=False,
     )
 
     # Events with only date set are apparently treated as occurring at midnight,
     # start of day in calendar's timezone.
-    calendar = service.calendars().get(calendarId=calendar_id).execute()
+    calendar = (
+        service.calendars()  # pylint: disable=no-member
+        .get(calendarId=calendar_id)
+        .execute()
+    )
     if calendar.get("timeZone"):
         timezone: datetime.tzinfo = zoneinfo.ZoneInfo(calendar["timeZone"])
     else:
         timezone = datetime.timezone.utc
     since = datetime.datetime.now(timezone).replace(hour=0) - datetime.timedelta(
-        hours=1,
+        hours=1
     )
 
     events = (
-        service.events()
+        service.events()  # pylint: disable=no-member
         .list(
             calendarId=calendar_id,
             orderBy="startTime",
             singleEvents=True,
             timeMin=since.isoformat(),
             privateExtendedProperty="pytekukko-managed=true",
         )
         .execute()
     )
 
-    pos_events: dict[str, dict[str, Any]] = {}
+    pos_events: Dict[str, Dict[str, Any]] = {}
     for event in events["items"]:
         # Store first event for each pos for update, delete rest
         pos = event["extendedProperties"]["private"].get("pytekukko-pos")
         if pos and pos in data and not pos_events.get(pos):
             pos_events[pos] = event
         else:
-            service.events().delete(
-                calendarId=calendar_id,
-                eventId=event["id"],
+            service.events().delete(  # pylint: disable=no-member
+                calendarId=calendar_id, eventId=event["id"]
             ).execute()
 
     for pos, pos_event_data in data.items():
         date = pos_event_data.date.isoformat()
         name = pos_event_data.name or ""
         description = f"{name} [pos={pos}]".strip()
         event_data = {
@@ -99,15 +106,15 @@
             # Reminders are "for the authenticated user" per docs.
             # So for the service account, not the calendar owner :(
             # No way to set this for the "actual" calendar user from here,
             # at least while using a service account.
             "reminders": {"useDefault": False},
             "transparency": "transparent",
             "extendedProperties": {
-                "private": {"pytekukko-managed": "true", "pytekukko-pos": pos},
+                "private": {"pytekukko-managed": "true", "pytekukko-pos": pos}
             },
             "source": {
                 "url": "https://tilasto.jatekukko.fi/indexservice2.jsp",
                 "title": "Omakukko",
             },
             "creator": {
                 "displayName": "Pytekukko",
@@ -118,60 +125,57 @@
 
         method = None
         log_level = logging.INFO
         if event:
             for key, value in event_data.items():
                 if event.get(key) != value:
                     action = "updated"
-                    method = service.events().patch(
-                        calendarId=calendar_id,
-                        eventId=event["id"],
-                        body=event_data,
+                    method = service.events().patch(  # pylint: disable=no-member
+                        calendarId=calendar_id, eventId=event["id"], body=event_data
                     )
                     break
             else:
                 action = "unchanged"
                 log_level = logging.DEBUG
         else:
             action = "created"
-            method = service.events().insert(
-                calendarId=calendar_id,
-                body=event_data,
+            method = service.events().insert(  # pylint: disable=no-member
+                calendarId=calendar_id, body=event_data
             )
         if method:
             event = method.execute()
         LOGGER.log(log_level, "Event %s: %s", action, event.get("htmlLink"))
 
 
 async def run_example() -> None:
     """Run the example."""
+
     argparser = example_argparser(__doc__)
     argparser.add_argument(
         "--google-calendar-id",
         type=str,
         **arg_environ_default("PYTEKUKKO_GOOGLE_CALENDAR_ID"),  # type: ignore[arg-type]
     )
     argparser.add_argument(
         "--google-service-account-file",
         type=str,
         **arg_environ_default(  # type: ignore[arg-type]
-            "PYTEKUKKO_GOOGLE_SERVICE_ACCOUNT_FILE",
-            fallback="service_account.json",
+            "PYTEKUKKO_GOOGLE_SERVICE_ACCOUNT_FILE", fallback="service_account.json"
         ),
     )
     args = argparser.parse_args()
 
     if not args.google_calendar_id:
-        print("Google calendar id required", file=sys.stderr)  # noqa: T201
+        print("Google calendar id required", file=sys.stderr)
         sys.exit(2)
 
     client, cookie_jar, cookie_jar_path = example_client(args)
 
     credentials = service_account.Credentials.from_service_account_file(
-        args.google_service_account_file,
+        args.google_service_account_file
     )
 
     async with client.session:
         services = await client.get_services()
         if not cookie_jar_path:
             await client.logout()
 
@@ -190,19 +194,15 @@
                     service.raw_data.get("owner", {}).get("posti"),
                 )
                 if x
             ),
         )
 
     await asyncio.get_event_loop().run_in_executor(
-        None,
-        update_google_calendar,
-        credentials,
-        args.google_calendar_id,
-        data,
+        None, update_google_calendar, credentials, args.google_calendar_id, data
     )
 
 
 def main() -> None:
     """Run example in event loop."""
     asyncio.run(run_example())
```

### Comparing `pytekukko-0.14.0/src/pytekukko/models.py` & `pytekukko-0.9.0/src/pytekukko/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,76 +1,75 @@
 """Pytekukko model objects."""
 
 from dataclasses import dataclass
 from datetime import date
-from typing import Any, cast
+from typing import Any, Dict, Optional, cast
 
 
 @dataclass
 class Service:
-    """Service encapsulates information about parts of a customer relationship.
+    """
+    Service encapsulates information about parts of a customer relationship.
 
     Examples of the kinds of services there are include collections of different kinds
     of waste containers, and yearly base prices for houses.
 
     Some frequently used service attributes are available as individual properties,
     and all data retrieved from the service is available in the ``raw_data`` dict.
     """
 
-    raw_data: dict[str, Any]
+    raw_data: Dict[str, Any]
 
     @property
     def name(self) -> str:
         """Get service name."""
         return cast(str, self.raw_data["ASTNimi"])
 
     @property
     def pos(self) -> int:
         """Get "pos" value."""
         return cast(int, self.raw_data["ASTPos"])
 
     @property
-    def next_collection(self) -> date | None:
-        """Get next collection date.
+    def next_collection(self) -> Optional[date]:
+        """
+        Get next collection date.
 
         :returns: Next collection date, None if not applicable for the service.
         """
         return self.raw_data.get("ASTSeurTyhj")
 
 
 @dataclass
 class CustomerData:
-    """CustomerData encapsulates customer information.
+    """
+    CustomerData encapsulates customer information.
 
     Some frequently used service attributes are available as individual properties,
     and all data retrieved from the service is available in the ``raw_data`` dict.
     """
 
-    raw_data: dict[str, Any]
+    raw_data: Dict[str, Any]
 
     @property
     def customer_number(self) -> str:
         """Get customer number."""
         return cast(str, self.raw_data["asiakasnro"])
 
-    @property
-    def name(self) -> str:
-        """Get customer name."""
-        return cast(str, self.raw_data["nimi"])
-
 
 @dataclass
 class InvoiceHeader:
-    """InvoiceHeader encapsulates basic information of an invoice.
+    """
+    InvoiceHeader encapsulates basic information of an invoice.
 
     Some frequently used service attributes are available as individual properties,
     and all data retrieved from the service is available in the ``raw_data`` dict.
     """
 
-    raw_data: dict[str, Any]
+    raw_data: Dict[str, Any]
 
     @property
     def name(self) -> str:
         """Get customer number."""
         return cast(str, self.raw_data["name"])
 
     @property
```

### Comparing `pytekukko-0.14.0/src/pytekukko.egg-info/SOURCES.txt` & `pytekukko-0.9.0/src/pytekukko.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements/dev-requirements.txt
-requirements/test-requirements.txt
+setup.cfg
+setup.py
 src/pytekukko/__init__.py
-src/pytekukko/exceptions.py
 src/pytekukko/models.py
-src/pytekukko/py.typed
 src/pytekukko.egg-info/PKG-INFO
 src/pytekukko.egg-info/SOURCES.txt
 src/pytekukko.egg-info/dependency_links.txt
 src/pytekukko.egg-info/entry_points.txt
 src/pytekukko.egg-info/requires.txt
 src/pytekukko.egg-info/top_level.txt
 src/pytekukko/examples/__init__.py
@@ -20,9 +18,9 @@
 src/pytekukko/examples/print_invoice_headers.py
 src/pytekukko/examples/print_next_collections.py
 src/pytekukko/examples/update_google_calendar.py
 tests/__init__.py
 tests/test_pytekukko.py
 tests/cassettes/test_get_collection_schedule.yaml
 tests/cassettes/test_get_invoice_headers.yaml
-tests/cassettes/test_login_logout.yaml
+tests/cassettes/test_login.yaml
 tests/cassettes/test_logout.yaml
```

### Comparing `pytekukko-0.14.0/tests/cassettes/test_get_collection_schedule.yaml` & `pytekukko-0.9.0/tests/cassettes/test_get_collection_schedule.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,103 +1,103 @@
 interactions:
 - request:
-    body:
-      j_password: secret
-      j_username: 00-0000000-00
+    body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Content-Length:
       - '78'
       Content-Type:
       - application/x-www-form-urlencoded
       Host:
       - tilasto.jatekukko.fi
       User-Agent:
-      - Python/3.8 aiohttp/3.8.1
+      - Python/3.8 aiohttp/3.7.4.post0
       X-Requested-With:
       - XMLHttpRequest
     method: POST
     uri: https://tilasto.jatekukko.fi/jatekukko/j_acegi_security_check?target=2
   response:
-    body: {}
+    body:
+      string: ''
     headers:
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       Date:
-      - Wed, 31 Aug 2022 19:15:10 GMT
+      - Sun, 05 Sep 2021 08:16:31 GMT
       Location:
       - https://tilasto.jatekukko.fi/jatekukko/secure/welcome.do
       Server:
       - nginx
       Strict-Transport-Security:
       - max-age=63072000
       X-Frame-Options:
       - SAMEORIGIN
       X-Powered-By:
-      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2022.2 #badassfish Java/Eclipse OpenJ9/1.8)'
+      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2021.5 #badassfish Java/Eclipse OpenJ9/1.8)'
     status:
       code: 303
       message: See Other
     url: https://tilasto.jatekukko.fi/jatekukko/j_acegi_security_check?target=2
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Host:
       - tilasto.jatekukko.fi
       User-Agent:
-      - Python/3.8 aiohttp/3.8.1
+      - Python/3.8 aiohttp/3.7.4.post0
       X-Requested-With:
       - XMLHttpRequest
     method: GET
     uri: https://tilasto.jatekukko.fi/jatekukko/secure/welcome.do
   response:
-    body: {}
+    body:
+      string: ''
     headers:
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       Content-Security-Policy:
       - frame-ancestors 'none'
       Date:
-      - Wed, 31 Aug 2022 19:15:10 GMT
+      - Sun, 05 Sep 2021 08:16:31 GMT
       Location:
       - https://tilasto.jatekukko.fi/jatekukko/secure/well.do
       Server:
       - nginx
       Strict-Transport-Security:
       - max-age=63072000
       X-Frame-Options:
       - DENY
       X-Powered-By:
-      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2022.2 #badassfish Java/Eclipse OpenJ9/1.8)'
+      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2021.5 #badassfish Java/Eclipse OpenJ9/1.8)'
     status:
       code: 303
       message: See Other
     url: https://tilasto.jatekukko.fi/jatekukko/secure/welcome.do
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Host:
       - tilasto.jatekukko.fi
       User-Agent:
-      - Python/3.8 aiohttp/3.8.1
+      - Python/3.8 aiohttp/3.7.4.post0
       X-Requested-With:
       - XMLHttpRequest
     method: GET
     uri: https://tilasto.jatekukko.fi/jatekukko/secure/well.do
   response:
     body:
       string: '{ "response":"OK"}'
@@ -132,27 +132,27 @@
       Connection:
       - keep-alive
       Content-Length:
       - '18'
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Wed, 31 Aug 2022 19:15:10 GMT
+      - Sun, 05 Sep 2021 08:16:31 GMT
       Expires:
       - Thu, 01 Jan 1970 00:00:00 GMT
       Pragma:
       - no-cache
       Server:
       - nginx
       Strict-Transport-Security:
       - max-age=63072000
       X-Frame-Options:
       - SAMEORIGIN
       X-Powered-By:
-      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2022.2 #badassfish Java/Eclipse OpenJ9/1.8)'
+      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2021.5 #badassfish Java/Eclipse OpenJ9/1.8)'
     status:
       code: 200
       message: OK
     url: https://tilasto.jatekukko.fi/jatekukko/secure/well.do
 - request:
     body: null
     headers: {}
@@ -165,27 +165,27 @@
       Cache-Control:
       - no-cache, no-store, must-revalidate
       Connection:
       - keep-alive
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Wed, 31 Aug 2022 19:15:10 GMT
+      - Sun, 05 Sep 2021 08:16:31 GMT
       Expires:
       - Thu, 01 Jan 1970 00:00:00 GMT
       Pragma:
       - no-cache
       Server:
       - nginx
       Strict-Transport-Security:
       - max-age=63072000
       Transfer-Encoding:
       - chunked
       X-Frame-Options:
       - SAMEORIGIN
       X-Powered-By:
-      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2022.2 #badassfish Java/Eclipse OpenJ9/1.8)'
+      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2021.5 #badassfish Java/Eclipse OpenJ9/1.8)'
     status:
       code: 200
       message: OK
     url: https://tilasto.jatekukko.fi/jatekukko/get_collection_schedule.do?customerNumber=00-0000000-00&pos=1234
 version: 1
```

### Comparing `pytekukko-0.14.0/tests/cassettes/test_get_invoice_headers.yaml` & `pytekukko-0.9.0/tests/cassettes/test_get_invoice_headers.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -5,55 +5,55 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Host:
       - tilasto.jatekukko.fi
       User-Agent:
-      - Python/3.8 aiohttp/3.8.1
+      - Python/3.8 aiohttp/3.7.4.post0
     method: GET
     uri: https://tilasto.jatekukko.fi/jatekukko/secure/get_invoice_headers_for_customer.do?customerId=00-0000000-00
   response:
     body: {}
     headers:
       Connection:
       - keep-alive
       Content-Language:
       - fi-FI
       Content-Length:
       - '197'
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Wed, 31 Aug 2022 19:15:11 GMT
+      - Mon, 06 Sep 2021 19:09:45 GMT
       Location:
       - https://tilasto.jatekukko.fi/jatekukko/login.do
       Server:
       - nginx
       Strict-Transport-Security:
       - max-age=63072000
       X-Frame-Options:
       - SAMEORIGIN
       X-Powered-By:
-      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2022.2 #badassfish Java/Eclipse OpenJ9/1.8)'
+      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2021.5 #badassfish Java/Eclipse OpenJ9/1.8)'
     status:
       code: 302
       message: Found
     url: https://tilasto.jatekukko.fi/jatekukko/secure/get_invoice_headers_for_customer.do?customerId=00-0000000-00
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Host:
       - tilasto.jatekukko.fi
       User-Agent:
-      - Python/3.8 aiohttp/3.8.1
+      - Python/3.8 aiohttp/3.7.4.post0
     method: GET
     uri: https://tilasto.jatekukko.fi/jatekukko/login.do
   response:
     body:
       string: redacted
     headers:
       Connection:
@@ -63,124 +63,124 @@
       Content-Language:
       - fi-FI
       Content-Security-Policy:
       - frame-ancestors 'none'
       Content-Type:
       - text/html;charset=utf-8
       Date:
-      - Wed, 31 Aug 2022 19:15:11 GMT
+      - Mon, 06 Sep 2021 19:09:45 GMT
       Server:
       - nginx
       Strict-Transport-Security:
       - max-age=63072000
       Transfer-Encoding:
       - chunked
       X-Frame-Options:
       - DENY
       X-Powered-By:
-      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2022.2 #badassfish Java/Eclipse OpenJ9/1.8)'
+      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2021.5 #badassfish Java/Eclipse OpenJ9/1.8)'
     status:
       code: 200
       message: OK
     url: https://tilasto.jatekukko.fi/jatekukko/login.do
 - request:
-    body:
-      j_password: secret
-      j_username: 00-0000000-00
+    body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Content-Length:
       - '78'
       Content-Type:
       - application/x-www-form-urlencoded
       Host:
       - tilasto.jatekukko.fi
       User-Agent:
-      - Python/3.8 aiohttp/3.8.1
+      - Python/3.8 aiohttp/3.7.4.post0
       X-Requested-With:
       - XMLHttpRequest
     method: POST
     uri: https://tilasto.jatekukko.fi/jatekukko/j_acegi_security_check?target=2
   response:
-    body: {}
+    body:
+      string: ''
     headers:
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       Date:
-      - Wed, 31 Aug 2022 19:15:11 GMT
+      - Mon, 06 Sep 2021 19:09:45 GMT
       Location:
       - https://tilasto.jatekukko.fi/jatekukko/secure/welcome.do
       Server:
       - nginx
       Strict-Transport-Security:
       - max-age=63072000
       X-Frame-Options:
       - SAMEORIGIN
       X-Powered-By:
-      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2022.2 #badassfish Java/Eclipse OpenJ9/1.8)'
+      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2021.5 #badassfish Java/Eclipse OpenJ9/1.8)'
     status:
       code: 303
       message: See Other
     url: https://tilasto.jatekukko.fi/jatekukko/j_acegi_security_check?target=2
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Host:
       - tilasto.jatekukko.fi
       User-Agent:
-      - Python/3.8 aiohttp/3.8.1
+      - Python/3.8 aiohttp/3.7.4.post0
       X-Requested-With:
       - XMLHttpRequest
     method: GET
     uri: https://tilasto.jatekukko.fi/jatekukko/secure/welcome.do
   response:
-    body: {}
+    body:
+      string: ''
     headers:
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       Content-Security-Policy:
       - frame-ancestors 'none'
       Date:
-      - Wed, 31 Aug 2022 19:15:11 GMT
+      - Mon, 06 Sep 2021 19:09:46 GMT
       Location:
       - https://tilasto.jatekukko.fi/jatekukko/secure/well.do
       Server:
       - nginx
       Strict-Transport-Security:
       - max-age=63072000
       X-Frame-Options:
       - DENY
       X-Powered-By:
-      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2022.2 #badassfish Java/Eclipse OpenJ9/1.8)'
+      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2021.5 #badassfish Java/Eclipse OpenJ9/1.8)'
     status:
       code: 303
       message: See Other
     url: https://tilasto.jatekukko.fi/jatekukko/secure/welcome.do
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Host:
       - tilasto.jatekukko.fi
       User-Agent:
-      - Python/3.8 aiohttp/3.8.1
+      - Python/3.8 aiohttp/3.7.4.post0
       X-Requested-With:
       - XMLHttpRequest
     method: GET
     uri: https://tilasto.jatekukko.fi/jatekukko/secure/well.do
   response:
     body:
       string: '{ "response":"OK"}'
@@ -215,27 +215,27 @@
       Connection:
       - keep-alive
       Content-Length:
       - '18'
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Wed, 31 Aug 2022 19:15:11 GMT
+      - Mon, 06 Sep 2021 19:09:46 GMT
       Expires:
       - Thu, 01 Jan 1970 00:00:00 GMT
       Pragma:
       - no-cache
       Server:
       - nginx
       Strict-Transport-Security:
       - max-age=63072000
       X-Frame-Options:
       - SAMEORIGIN
       X-Powered-By:
-      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2022.2 #badassfish Java/Eclipse OpenJ9/1.8)'
+      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2021.5 #badassfish Java/Eclipse OpenJ9/1.8)'
     status:
       code: 200
       message: OK
     url: https://tilasto.jatekukko.fi/jatekukko/secure/well.do
 - request:
     body: null
     headers: {}
@@ -250,27 +250,27 @@
       Cache-Control:
       - no-cache, no-store, must-revalidate
       Connection:
       - keep-alive
       Content-Type:
       - application/json;charset=UTF-8
       Date:
-      - Wed, 31 Aug 2022 19:15:11 GMT
+      - Mon, 06 Sep 2021 19:09:46 GMT
       Expires:
       - Thu, 01 Jan 1970 00:00:00 GMT
       Pragma:
       - no-cache
       Server:
       - nginx
       Strict-Transport-Security:
       - max-age=63072000
       Transfer-Encoding:
       - chunked
       X-Frame-Options:
       - SAMEORIGIN
       X-Powered-By:
-      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2022.2 #badassfish Java/Eclipse OpenJ9/1.8)'
+      - 'Servlet/4.0 JSP/2.3 (Payara Server  5.2021.5 #badassfish Java/Eclipse OpenJ9/1.8)'
     status:
       code: 200
       message: OK
     url: https://tilasto.jatekukko.fi/jatekukko/secure/get_invoice_headers_for_customer.do?customerId=00-0000000-00
 version: 1
```

### Comparing `pytekukko-0.14.0/tests/cassettes/test_login_logout.yaml` & `pytekukko-0.9.0/tests/cassettes/test_logout.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,7031 +1,6632 @@
 00000000: 696e 7465 7261 6374 696f 6e73 3a0a 2d20  interactions:.- 
 00000010: 7265 7175 6573 743a 0a20 2020 2062 6f64  request:.    bod
-00000020: 793a 0a20 2020 2020 206a 5f70 6173 7377  y:.      j_passw
-00000030: 6f72 643a 2073 6563 7265 740a 2020 2020  ord: secret.    
-00000040: 2020 6a5f 7573 6572 6e61 6d65 3a20 3030    j_username: 00
-00000050: 2d30 3030 3030 3030 2d30 300a 2020 2020  -0000000-00.    
-00000060: 6865 6164 6572 733a 0a20 2020 2020 2041  headers:.      A
-00000070: 6363 6570 743a 0a20 2020 2020 202d 2027  ccept:.      - '
-00000080: 2a2f 2a27 0a20 2020 2020 2041 6363 6570  */*'.      Accep
-00000090: 742d 456e 636f 6469 6e67 3a0a 2020 2020  t-Encoding:.    
-000000a0: 2020 2d20 677a 6970 2c20 6465 666c 6174    - gzip, deflat
-000000b0: 650a 2020 2020 2020 436f 6e74 656e 742d  e.      Content-
-000000c0: 4c65 6e67 7468 3a0a 2020 2020 2020 2d20  Length:.      - 
-000000d0: 2737 3827 0a20 2020 2020 2043 6f6e 7465  '78'.      Conte
-000000e0: 6e74 2d54 7970 653a 0a20 2020 2020 202d  nt-Type:.      -
-000000f0: 2061 7070 6c69 6361 7469 6f6e 2f78 2d77   application/x-w
-00000100: 7777 2d66 6f72 6d2d 7572 6c65 6e63 6f64  ww-form-urlencod
-00000110: 6564 0a20 2020 2020 2048 6f73 743a 0a20  ed.      Host:. 
-00000120: 2020 2020 202d 2074 696c 6173 746f 2e6a       - tilasto.j
-00000130: 6174 656b 756b 6b6f 2e66 690a 2020 2020  atekukko.fi.    
-00000140: 2020 5573 6572 2d41 6765 6e74 3a0a 2020    User-Agent:.  
-00000150: 2020 2020 2d20 5079 7468 6f6e 2f33 2e31      - Python/3.1
-00000160: 3120 6169 6f68 7474 702f 332e 382e 340a  1 aiohttp/3.8.4.
-00000170: 2020 2020 2020 582d 5265 7175 6573 7465        X-Requeste
-00000180: 642d 5769 7468 3a0a 2020 2020 2020 2d20  d-With:.      - 
-00000190: 584d 4c48 7474 7052 6571 7565 7374 0a20  XMLHttpRequest. 
-000001a0: 2020 206d 6574 686f 643a 2050 4f53 540a     method: POST.
-000001b0: 2020 2020 7572 693a 2068 7474 7073 3a2f      uri: https:/
-000001c0: 2f74 696c 6173 746f 2e6a 6174 656b 756b  /tilasto.jatekuk
-000001d0: 6b6f 2e66 692f 6a61 7465 6b75 6b6b 6f2f  ko.fi/jatekukko/
-000001e0: 6a5f 6163 6567 695f 7365 6375 7269 7479  j_acegi_security
-000001f0: 5f63 6865 636b 3f74 6172 6765 743d 320a  _check?target=2.
-00000200: 2020 7265 7370 6f6e 7365 3a0a 2020 2020    response:.    
-00000210: 626f 6479 3a20 7b7d 0a20 2020 2068 6561  body: {}.    hea
-00000220: 6465 7273 3a0a 2020 2020 2020 436f 6e6e  ders:.      Conn
-00000230: 6563 7469 6f6e 3a0a 2020 2020 2020 2d20  ection:.      - 
-00000240: 6b65 6570 2d61 6c69 7665 0a20 2020 2020  keep-alive.     
-00000250: 2043 6f6e 7465 6e74 2d4c 656e 6774 683a   Content-Length:
-00000260: 0a20 2020 2020 202d 2027 3027 0a20 2020  .      - '0'.   
-00000270: 2020 2044 6174 653a 0a20 2020 2020 202d     Date:.      -
-00000280: 2046 7269 2c20 3236 204d 6179 2032 3032   Fri, 26 May 202
-00000290: 3320 3037 3a35 383a 3036 2047 4d54 0a20  3 07:58:06 GMT. 
-000002a0: 2020 2020 204c 6f63 6174 696f 6e3a 0a20       Location:. 
-000002b0: 2020 2020 202d 2068 7474 7073 3a2f 2f74       - https://t
-000002c0: 696c 6173 746f 2e6a 6174 656b 756b 6b6f  ilasto.jatekukko
-000002d0: 2e66 692f 6a61 7465 6b75 6b6b 6f2f 7365  .fi/jatekukko/se
-000002e0: 6375 7265 2f77 656c 636f 6d65 2e64 6f0a  cure/welcome.do.
-000002f0: 2020 2020 2020 5365 7276 6572 3a0a 2020        Server:.  
-00000300: 2020 2020 2d20 6e67 696e 780a 2020 2020      - nginx.    
-00000310: 2020 5374 7269 6374 2d54 7261 6e73 706f    Strict-Transpo
-00000320: 7274 2d53 6563 7572 6974 793a 0a20 2020  rt-Security:.   
-00000330: 2020 202d 206d 6178 2d61 6765 3d36 3330     - max-age=630
-00000340: 3732 3030 300a 2020 2020 2020 582d 4672  72000.      X-Fr
-00000350: 616d 652d 4f70 7469 6f6e 733a 0a20 2020  ame-Options:.   
-00000360: 2020 202d 2053 414d 454f 5249 4749 4e0a     - SAMEORIGIN.
-00000370: 2020 2020 2020 582d 506f 7765 7265 642d        X-Powered-
-00000380: 4279 3a0a 2020 2020 2020 2d20 2753 6572  By:.      - 'Ser
-00000390: 766c 6574 2f34 2e30 204a 5350 2f32 2e33  vlet/4.0 JSP/2.3
-000003a0: 2028 5061 7961 7261 2053 6572 7665 7220   (Payara Server 
-000003b0: 2035 2e32 3032 322e 3520 2362 6164 6173   5.2022.5 #badas
-000003c0: 7366 6973 6820 4a61 7661 2f45 636c 6970  sfish Java/Eclip
-000003d0: 7365 204f 7065 6e4a 392f 312e 3829 270a  se OpenJ9/1.8)'.
-000003e0: 2020 2020 7374 6174 7573 3a0a 2020 2020      status:.    
-000003f0: 2020 636f 6465 3a20 3330 330a 2020 2020    code: 303.    
-00000400: 2020 6d65 7373 6167 653a 2053 6565 204f    message: See O
-00000410: 7468 6572 0a20 2020 2075 726c 3a20 6874  ther.    url: ht
-00000420: 7470 733a 2f2f 7469 6c61 7374 6f2e 6a61  tps://tilasto.ja
-00000430: 7465 6b75 6b6b 6f2e 6669 2f6a 6174 656b  tekukko.fi/jatek
-00000440: 756b 6b6f 2f6a 5f61 6365 6769 5f73 6563  ukko/j_acegi_sec
-00000450: 7572 6974 795f 6368 6563 6b3f 7461 7267  urity_check?targ
-00000460: 6574 3d32 0a2d 2072 6571 7565 7374 3a0a  et=2.- request:.
-00000470: 2020 2020 626f 6479 3a20 6e75 6c6c 0a20      body: null. 
-00000480: 2020 2068 6561 6465 7273 3a0a 2020 2020     headers:.    
-00000490: 2020 4163 6365 7074 3a0a 2020 2020 2020    Accept:.      
-000004a0: 2d20 272a 2f2a 270a 2020 2020 2020 4163  - '*/*'.      Ac
-000004b0: 6365 7074 2d45 6e63 6f64 696e 673a 0a20  cept-Encoding:. 
-000004c0: 2020 2020 202d 2067 7a69 702c 2064 6566       - gzip, def
-000004d0: 6c61 7465 0a20 2020 2020 2048 6f73 743a  late.      Host:
-000004e0: 0a20 2020 2020 202d 2074 696c 6173 746f  .      - tilasto
-000004f0: 2e6a 6174 656b 756b 6b6f 2e66 690a 2020  .jatekukko.fi.  
-00000500: 2020 2020 5573 6572 2d41 6765 6e74 3a0a      User-Agent:.
-00000510: 2020 2020 2020 2d20 5079 7468 6f6e 2f33        - Python/3
-00000520: 2e31 3120 6169 6f68 7474 702f 332e 382e  .11 aiohttp/3.8.
-00000530: 340a 2020 2020 2020 582d 5265 7175 6573  4.      X-Reques
-00000540: 7465 642d 5769 7468 3a0a 2020 2020 2020  ted-With:.      
-00000550: 2d20 584d 4c48 7474 7052 6571 7565 7374  - XMLHttpRequest
-00000560: 0a20 2020 206d 6574 686f 643a 2047 4554  .    method: GET
-00000570: 0a20 2020 2075 7269 3a20 6874 7470 733a  .    uri: https:
-00000580: 2f2f 7469 6c61 7374 6f2e 6a61 7465 6b75  //tilasto.jateku
-00000590: 6b6b 6f2e 6669 2f6a 6174 656b 756b 6b6f  kko.fi/jatekukko
-000005a0: 2f73 6563 7572 652f 7765 6c63 6f6d 652e  /secure/welcome.
-000005b0: 646f 0a20 2072 6573 706f 6e73 653a 0a20  do.  response:. 
-000005c0: 2020 2062 6f64 793a 207b 7d0a 2020 2020     body: {}.    
-000005d0: 6865 6164 6572 733a 0a20 2020 2020 2043  headers:.      C
-000005e0: 6f6e 6e65 6374 696f 6e3a 0a20 2020 2020  onnection:.     
-000005f0: 202d 206b 6565 702d 616c 6976 650a 2020   - keep-alive.  
-00000600: 2020 2020 436f 6e74 656e 742d 4c65 6e67      Content-Leng
-00000610: 7468 3a0a 2020 2020 2020 2d20 2730 270a  th:.      - '0'.
-00000620: 2020 2020 2020 436f 6e74 656e 742d 5365        Content-Se
-00000630: 6375 7269 7479 2d50 6f6c 6963 793a 0a20  curity-Policy:. 
-00000640: 2020 2020 202d 2066 7261 6d65 2d61 6e63       - frame-anc
-00000650: 6573 746f 7273 2027 6e6f 6e65 270a 2020  estors 'none'.  
-00000660: 2020 2020 4461 7465 3a0a 2020 2020 2020      Date:.      
-00000670: 2d20 4672 692c 2032 3620 4d61 7920 3230  - Fri, 26 May 20
-00000680: 3233 2030 373a 3538 3a30 3620 474d 540a  23 07:58:06 GMT.
-00000690: 2020 2020 2020 4c6f 6361 7469 6f6e 3a0a        Location:.
-000006a0: 2020 2020 2020 2d20 6874 7470 733a 2f2f        - https://
-000006b0: 7469 6c61 7374 6f2e 6a61 7465 6b75 6b6b  tilasto.jatekukk
-000006c0: 6f2e 6669 2f6a 6174 656b 756b 6b6f 2f73  o.fi/jatekukko/s
-000006d0: 6563 7572 652f 7765 6c6c 2e64 6f0a 2020  ecure/well.do.  
-000006e0: 2020 2020 5365 7276 6572 3a0a 2020 2020      Server:.    
-000006f0: 2020 2d20 6e67 696e 780a 2020 2020 2020    - nginx.      
-00000700: 5374 7269 6374 2d54 7261 6e73 706f 7274  Strict-Transport
-00000710: 2d53 6563 7572 6974 793a 0a20 2020 2020  -Security:.     
-00000720: 202d 206d 6178 2d61 6765 3d36 3330 3732   - max-age=63072
-00000730: 3030 300a 2020 2020 2020 582d 4672 616d  000.      X-Fram
-00000740: 652d 4f70 7469 6f6e 733a 0a20 2020 2020  e-Options:.     
-00000750: 202d 2044 454e 590a 2020 2020 2020 582d   - DENY.      X-
-00000760: 506f 7765 7265 642d 4279 3a0a 2020 2020  Powered-By:.    
-00000770: 2020 2d20 2753 6572 766c 6574 2f34 2e30    - 'Servlet/4.0
-00000780: 204a 5350 2f32 2e33 2028 5061 7961 7261   JSP/2.3 (Payara
-00000790: 2053 6572 7665 7220 2035 2e32 3032 322e   Server  5.2022.
-000007a0: 3520 2362 6164 6173 7366 6973 6820 4a61  5 #badassfish Ja
-000007b0: 7661 2f45 636c 6970 7365 204f 7065 6e4a  va/Eclipse OpenJ
-000007c0: 392f 312e 3829 270a 2020 2020 7374 6174  9/1.8)'.    stat
-000007d0: 7573 3a0a 2020 2020 2020 636f 6465 3a20  us:.      code: 
-000007e0: 3330 330a 2020 2020 2020 6d65 7373 6167  303.      messag
-000007f0: 653a 2053 6565 204f 7468 6572 0a20 2020  e: See Other.   
-00000800: 2075 726c 3a20 6874 7470 733a 2f2f 7469   url: https://ti
-00000810: 6c61 7374 6f2e 6a61 7465 6b75 6b6b 6f2e  lasto.jatekukko.
-00000820: 6669 2f6a 6174 656b 756b 6b6f 2f73 6563  fi/jatekukko/sec
-00000830: 7572 652f 7765 6c63 6f6d 652e 646f 0a2d  ure/welcome.do.-
-00000840: 2072 6571 7565 7374 3a0a 2020 2020 626f   request:.    bo
-00000850: 6479 3a20 6e75 6c6c 0a20 2020 2068 6561  dy: null.    hea
-00000860: 6465 7273 3a0a 2020 2020 2020 4163 6365  ders:.      Acce
-00000870: 7074 3a0a 2020 2020 2020 2d20 272a 2f2a  pt:.      - '*/*
-00000880: 270a 2020 2020 2020 4163 6365 7074 2d45  '.      Accept-E
-00000890: 6e63 6f64 696e 673a 0a20 2020 2020 202d  ncoding:.      -
-000008a0: 2067 7a69 702c 2064 6566 6c61 7465 0a20   gzip, deflate. 
-000008b0: 2020 2020 2048 6f73 743a 0a20 2020 2020       Host:.     
-000008c0: 202d 2074 696c 6173 746f 2e6a 6174 656b   - tilasto.jatek
-000008d0: 756b 6b6f 2e66 690a 2020 2020 2020 5573  ukko.fi.      Us
-000008e0: 6572 2d41 6765 6e74 3a0a 2020 2020 2020  er-Agent:.      
-000008f0: 2d20 5079 7468 6f6e 2f33 2e31 3120 6169  - Python/3.11 ai
-00000900: 6f68 7474 702f 332e 382e 340a 2020 2020  ohttp/3.8.4.    
-00000910: 2020 582d 5265 7175 6573 7465 642d 5769    X-Requested-Wi
-00000920: 7468 3a0a 2020 2020 2020 2d20 584d 4c48  th:.      - XMLH
-00000930: 7474 7052 6571 7565 7374 0a20 2020 206d  ttpRequest.    m
-00000940: 6574 686f 643a 2047 4554 0a20 2020 2075  ethod: GET.    u
-00000950: 7269 3a20 6874 7470 733a 2f2f 7469 6c61  ri: https://tila
-00000960: 7374 6f2e 6a61 7465 6b75 6b6b 6f2e 6669  sto.jatekukko.fi
-00000970: 2f6a 6174 656b 756b 6b6f 2f73 6563 7572  /jatekukko/secur
-00000980: 652f 7765 6c6c 2e64 6f0a 2020 7265 7370  e/well.do.  resp
-00000990: 6f6e 7365 3a0a 2020 2020 626f 6479 3a0a  onse:.    body:.
-000009a0: 2020 2020 2020 7374 7269 6e67 3a20 277b        string: '{
-000009b0: 2022 7265 7370 6f6e 7365 223a 224f 4b22   "response":"OK"
-000009c0: 7d27 0a20 2020 2068 6561 6465 7273 3a0a  }'.    headers:.
-000009d0: 2020 2020 2020 4163 6365 7074 2d43 6861        Accept-Cha
-000009e0: 7273 6574 3a0a 2020 2020 2020 2d20 6269  rset:.      - bi
-000009f0: 6735 2c20 6269 6735 2d68 6b73 6373 2c20  g5, big5-hkscs, 
-00000a00: 6365 7375 2d38 2c20 6575 632d 6a70 2c20  cesu-8, euc-jp, 
-00000a10: 6575 632d 6b72 2c20 6762 3138 3033 302c  euc-kr, gb18030,
-00000a20: 2067 6232 3331 322c 2067 626b 2c20 6962   gb2312, gbk, ib
-00000a30: 6d2d 7468 6169 2c0a 2020 2020 2020 2020  m-thai,.        
-00000a40: 6962 6d30 3038 3538 2c20 6962 6d30 3131  ibm00858, ibm011
-00000a50: 3430 2c20 6962 6d30 3131 3431 2c20 6962  40, ibm01141, ib
-00000a60: 6d30 3131 3432 2c20 6962 6d30 3131 3433  m01142, ibm01143
-00000a70: 2c20 6962 6d30 3131 3434 2c20 6962 6d30  , ibm01144, ibm0
-00000a80: 3131 3435 2c20 6962 6d30 3131 3436 2c0a  1145, ibm01146,.
-00000a90: 2020 2020 2020 2020 6962 6d30 3131 3437          ibm01147
-00000aa0: 2c20 6962 6d30 3131 3438 2c20 6962 6d30  , ibm01148, ibm0
-00000ab0: 3131 3439 2c20 6962 6d30 3337 2c20 6962  1149, ibm037, ib
-00000ac0: 6d31 3032 362c 2069 626d 3130 3437 2c20  m1026, ibm1047, 
-00000ad0: 6962 6d32 3733 2c20 6962 6d32 3737 2c20  ibm273, ibm277, 
-00000ae0: 6962 6d32 3738 2c0a 2020 2020 2020 2020  ibm278,.        
-00000af0: 6962 6d32 3830 2c20 6962 6d32 3834 2c20  ibm280, ibm284, 
-00000b00: 6962 6d32 3835 2c20 6962 6d32 3930 2c20  ibm285, ibm290, 
-00000b10: 6962 6d32 3937 2c20 6962 6d34 3230 2c20  ibm297, ibm420, 
-00000b20: 6962 6d34 3234 2c20 6962 6d34 3337 2c20  ibm424, ibm437, 
-00000b30: 6962 6d35 3030 2c20 6962 6d37 3735 2c0a  ibm500, ibm775,.
-00000b40: 2020 2020 2020 2020 6962 6d38 3530 2c20          ibm850, 
-00000b50: 6962 6d38 3532 2c20 6962 6d38 3535 2c20  ibm852, ibm855, 
-00000b60: 6962 6d38 3537 2c20 6962 6d38 3630 2c20  ibm857, ibm860, 
-00000b70: 6962 6d38 3631 2c20 6962 6d38 3632 2c20  ibm861, ibm862, 
-00000b80: 6962 6d38 3633 2c20 6962 6d38 3634 2c20  ibm863, ibm864, 
-00000b90: 6962 6d38 3635 2c0a 2020 2020 2020 2020  ibm865,.        
-00000ba0: 6962 6d38 3636 2c20 6962 6d38 3638 2c20  ibm866, ibm868, 
-00000bb0: 6962 6d38 3639 2c20 6962 6d38 3730 2c20  ibm869, ibm870, 
-00000bc0: 6962 6d38 3731 2c20 6962 6d39 3138 2c20  ibm871, ibm918, 
-00000bd0: 6973 6f2d 3230 3232 2d63 6e2c 2069 736f  iso-2022-cn, iso
-00000be0: 2d32 3032 322d 6a70 2c0a 2020 2020 2020  -2022-jp,.      
-00000bf0: 2020 6973 6f2d 3230 3232 2d6a 702d 322c    iso-2022-jp-2,
-00000c00: 2069 736f 2d32 3032 322d 6b72 2c20 6973   iso-2022-kr, is
-00000c10: 6f2d 3838 3539 2d31 2c20 6973 6f2d 3838  o-8859-1, iso-88
-00000c20: 3539 2d31 332c 2069 736f 2d38 3835 392d  59-13, iso-8859-
-00000c30: 3135 2c20 6973 6f2d 3838 3539 2d32 2c0a  15, iso-8859-2,.
-00000c40: 2020 2020 2020 2020 6973 6f2d 3838 3539          iso-8859
-00000c50: 2d33 2c20 6973 6f2d 3838 3539 2d34 2c20  -3, iso-8859-4, 
-00000c60: 6973 6f2d 3838 3539 2d35 2c20 6973 6f2d  iso-8859-5, iso-
-00000c70: 3838 3539 2d36 2c20 6973 6f2d 3838 3539  8859-6, iso-8859
-00000c80: 2d37 2c20 6973 6f2d 3838 3539 2d38 2c20  -7, iso-8859-8, 
-00000c90: 6973 6f2d 3838 3539 2d39 2c0a 2020 2020  iso-8859-9,.    
-00000ca0: 2020 2020 6a69 735f 7830 3230 312c 206a      jis_x0201, j
-00000cb0: 6973 5f78 3032 3132 2d31 3939 302c 206b  is_x0212-1990, k
-00000cc0: 6f69 382d 722c 206b 6f69 382d 752c 2073  oi8-r, koi8-u, s
-00000cd0: 6869 6674 5f6a 6973 2c20 7469 732d 3632  hift_jis, tis-62
-00000ce0: 302c 2075 732d 6173 6369 692c 2075 7466  0, us-ascii, utf
-00000cf0: 2d31 362c 0a20 2020 2020 2020 2075 7466  -16,.        utf
-00000d00: 2d31 3662 652c 2075 7466 2d31 366c 652c  -16be, utf-16le,
-00000d10: 2075 7466 2d33 322c 2075 7466 2d33 3262   utf-32, utf-32b
-00000d20: 652c 2075 7466 2d33 326c 652c 2075 7466  e, utf-32le, utf
-00000d30: 2d38 2c20 7769 6e64 6f77 732d 3132 3530  -8, windows-1250
-00000d40: 2c20 7769 6e64 6f77 732d 3132 3531 2c0a  , windows-1251,.
-00000d50: 2020 2020 2020 2020 7769 6e64 6f77 732d          windows-
-00000d60: 3132 3532 2c20 7769 6e64 6f77 732d 3132  1252, windows-12
-00000d70: 3533 2c20 7769 6e64 6f77 732d 3132 3534  53, windows-1254
-00000d80: 2c20 7769 6e64 6f77 732d 3132 3535 2c20  , windows-1255, 
-00000d90: 7769 6e64 6f77 732d 3132 3536 2c20 7769  windows-1256, wi
-00000da0: 6e64 6f77 732d 3132 3537 2c0a 2020 2020  ndows-1257,.    
-00000db0: 2020 2020 7769 6e64 6f77 732d 3132 3538      windows-1258
-00000dc0: 2c20 7769 6e64 6f77 732d 3331 6a2c 2078  , windows-31j, x
-00000dd0: 2d62 6967 352d 686b 7363 732d 3230 3031  -big5-hkscs-2001
-00000de0: 2c20 782d 6269 6735 2d73 6f6c 6172 6973  , x-big5-solaris
-00000df0: 2c20 782d 636f 6d70 6f75 6e64 5f74 6578  , x-compound_tex
-00000e00: 742c 0a20 2020 2020 2020 2078 2d65 7563  t,.        x-euc
-00000e10: 2d6a 702d 6c69 6e75 782c 2078 2d65 7563  -jp-linux, x-euc
-00000e20: 2d74 772c 2078 2d65 7563 6a70 2d6f 7065  -tw, x-eucjp-ope
-00000e30: 6e2c 2078 2d69 626d 3130 3036 2c20 782d  n, x-ibm1006, x-
-00000e40: 6962 6d31 3032 352c 2078 2d69 626d 3130  ibm1025, x-ibm10
-00000e50: 3436 2c20 782d 6962 6d31 3039 372c 0a20  46, x-ibm1097,. 
-00000e60: 2020 2020 2020 2078 2d69 626d 3130 3938         x-ibm1098
-00000e70: 2c20 782d 6962 6d31 3131 322c 2078 2d69  , x-ibm1112, x-i
-00000e80: 626d 3131 3232 2c20 782d 6962 6d31 3132  bm1122, x-ibm112
-00000e90: 332c 2078 2d69 626d 3131 3234 2c20 782d  3, x-ibm1124, x-
-00000ea0: 6962 6d31 3136 362c 2078 2d69 626d 3133  ibm1166, x-ibm13
-00000eb0: 3634 2c0a 2020 2020 2020 2020 782d 6962  64,.        x-ib
-00000ec0: 6d31 3338 312c 2078 2d69 626d 3133 3833  m1381, x-ibm1383
-00000ed0: 2c20 782d 6962 6d33 3030 2c20 782d 6962  , x-ibm300, x-ib
-00000ee0: 6d33 3337 3232 2c20 782d 6962 6d37 3337  m33722, x-ibm737
-00000ef0: 2c20 782d 6962 6d38 3333 2c20 782d 6962  , x-ibm833, x-ib
-00000f00: 6d38 3334 2c0a 2020 2020 2020 2020 782d  m834,.        x-
-00000f10: 6962 6d38 3536 2c20 782d 6962 6d38 3734  ibm856, x-ibm874
-00000f20: 2c20 782d 6962 6d38 3735 2c20 782d 6962  , x-ibm875, x-ib
-00000f30: 6d39 3231 2c20 782d 6962 6d39 3232 2c20  m921, x-ibm922, 
-00000f40: 782d 6962 6d39 3330 2c20 782d 6962 6d39  x-ibm930, x-ibm9
-00000f50: 3333 2c20 782d 6962 6d39 3335 2c0a 2020  33, x-ibm935,.  
-00000f60: 2020 2020 2020 782d 6962 6d39 3337 2c20        x-ibm937, 
-00000f70: 782d 6962 6d39 3339 2c20 782d 6962 6d39  x-ibm939, x-ibm9
-00000f80: 3432 2c20 782d 6962 6d39 3432 632c 2078  42, x-ibm942c, x
-00000f90: 2d69 626d 3934 332c 2078 2d69 626d 3934  -ibm943, x-ibm94
-00000fa0: 3363 2c20 782d 6962 6d39 3438 2c20 782d  3c, x-ibm948, x-
-00000fb0: 6962 6d39 3439 2c0a 2020 2020 2020 2020  ibm949,.        
-00000fc0: 782d 6962 6d39 3439 632c 2078 2d69 626d  x-ibm949c, x-ibm
-00000fd0: 3935 302c 2078 2d69 626d 3936 342c 2078  950, x-ibm964, x
-00000fe0: 2d69 626d 3937 302c 2078 2d69 7363 6969  -ibm970, x-iscii
-00000ff0: 3931 2c20 782d 6973 6f2d 3230 3232 2d63  91, x-iso-2022-c
-00001000: 6e2d 636e 732c 2078 2d69 736f 2d32 3032  n-cns, x-iso-202
-00001010: 322d 636e 2d67 622c 0a20 2020 2020 2020  2-cn-gb,.       
-00001020: 2078 2d69 736f 2d38 3835 392d 3131 2c20   x-iso-8859-11, 
-00001030: 782d 6a69 7330 3230 382c 2078 2d6a 6973  x-jis0208, x-jis
-00001040: 6175 746f 6465 7465 6374 2c20 782d 6a6f  autodetect, x-jo
-00001050: 6861 622c 2078 2d6d 6163 6172 6162 6963  hab, x-macarabic
-00001060: 2c20 782d 6d61 6363 656e 7472 616c 6575  , x-maccentraleu
-00001070: 726f 7065 2c0a 2020 2020 2020 2020 782d  rope,.        x-
-00001080: 6d61 6363 726f 6174 6961 6e2c 2078 2d6d  maccroatian, x-m
-00001090: 6163 6379 7269 6c6c 6963 2c20 782d 6d61  accyrillic, x-ma
-000010a0: 6364 696e 6762 6174 2c20 782d 6d61 6367  cdingbat, x-macg
-000010b0: 7265 656b 2c20 782d 6d61 6368 6562 7265  reek, x-machebre
-000010c0: 772c 2078 2d6d 6163 6963 656c 616e 642c  w, x-maciceland,
-000010d0: 0a20 2020 2020 2020 2078 2d6d 6163 726f  .        x-macro
-000010e0: 6d61 6e2c 2078 2d6d 6163 726f 6d61 6e69  man, x-macromani
-000010f0: 612c 2078 2d6d 6163 7379 6d62 6f6c 2c20  a, x-macsymbol, 
-00001100: 782d 6d61 6374 6861 692c 2078 2d6d 6163  x-macthai, x-mac
-00001110: 7475 726b 6973 682c 2078 2d6d 6163 756b  turkish, x-macuk
-00001120: 7261 696e 652c 0a20 2020 2020 2020 2078  raine,.        x
-00001130: 2d6d 7339 3332 5f30 3231 332c 2078 2d6d  -ms932_0213, x-m
-00001140: 7339 3530 2d68 6b73 6373 2c20 782d 6d73  s950-hkscs, x-ms
-00001150: 3935 302d 686b 7363 732d 7870 2c20 782d  950-hkscs-xp, x-
-00001160: 6d73 7769 6e2d 3933 362c 2078 2d70 636b  mswin-936, x-pck
-00001170: 2c20 782d 736a 6973 5f30 3231 332c 0a20  , x-sjis_0213,. 
-00001180: 2020 2020 2020 2078 2d75 7466 2d31 366c         x-utf-16l
-00001190: 652d 626f 6d2c 2078 2d75 7466 2d33 3262  e-bom, x-utf-32b
-000011a0: 652d 626f 6d2c 2078 2d75 7466 2d33 326c  e-bom, x-utf-32l
-000011b0: 652d 626f 6d2c 2078 2d77 696e 646f 7773  e-bom, x-windows
-000011c0: 2d35 3032 3230 2c20 782d 7769 6e64 6f77  -50220, x-window
-000011d0: 732d 3530 3232 312c 0a20 2020 2020 2020  s-50221,.       
-000011e0: 2078 2d77 696e 646f 7773 2d38 3734 2c20   x-windows-874, 
-000011f0: 782d 7769 6e64 6f77 732d 3934 392c 2078  x-windows-949, x
-00001200: 2d77 696e 646f 7773 2d39 3530 2c20 782d  -windows-950, x-
-00001210: 7769 6e64 6f77 732d 6973 6f32 3032 326a  windows-iso2022j
-00001220: 700a 2020 2020 2020 4361 6368 652d 436f  p.      Cache-Co
-00001230: 6e74 726f 6c3a 0a20 2020 2020 202d 206e  ntrol:.      - n
-00001240: 6f2d 6361 6368 652c 206e 6f2d 7374 6f72  o-cache, no-stor
-00001250: 652c 206d 7573 742d 7265 7661 6c69 6461  e, must-revalida
-00001260: 7465 0a20 2020 2020 2043 6f6e 6e65 6374  te.      Connect
-00001270: 696f 6e3a 0a20 2020 2020 202d 206b 6565  ion:.      - kee
-00001280: 702d 616c 6976 650a 2020 2020 2020 436f  p-alive.      Co
-00001290: 6e74 656e 742d 4c65 6e67 7468 3a0a 2020  ntent-Length:.  
-000012a0: 2020 2020 2d20 2731 3827 0a20 2020 2020      - '18'.     
-000012b0: 2043 6f6e 7465 6e74 2d54 7970 653a 0a20   Content-Type:. 
-000012c0: 2020 2020 202d 2061 7070 6c69 6361 7469       - applicati
-000012d0: 6f6e 2f6a 736f 6e3b 6368 6172 7365 743d  on/json;charset=
-000012e0: 5554 462d 380a 2020 2020 2020 4461 7465  UTF-8.      Date
-000012f0: 3a0a 2020 2020 2020 2d20 4672 692c 2032  :.      - Fri, 2
-00001300: 3620 4d61 7920 3230 3233 2030 373a 3538  6 May 2023 07:58
-00001310: 3a30 3620 474d 540a 2020 2020 2020 4578  :06 GMT.      Ex
-00001320: 7069 7265 733a 0a20 2020 2020 202d 2054  pires:.      - T
-00001330: 6875 2c20 3031 204a 616e 2031 3937 3020  hu, 01 Jan 1970 
-00001340: 3030 3a30 303a 3030 2047 4d54 0a20 2020  00:00:00 GMT.   
-00001350: 2020 2050 7261 676d 613a 0a20 2020 2020     Pragma:.     
-00001360: 202d 206e 6f2d 6361 6368 650a 2020 2020   - no-cache.    
-00001370: 2020 5365 7276 6572 3a0a 2020 2020 2020    Server:.      
-00001380: 2d20 6e67 696e 780a 2020 2020 2020 5374  - nginx.      St
-00001390: 7269 6374 2d54 7261 6e73 706f 7274 2d53  rict-Transport-S
-000013a0: 6563 7572 6974 793a 0a20 2020 2020 202d  ecurity:.      -
-000013b0: 206d 6178 2d61 6765 3d36 3330 3732 3030   max-age=6307200
-000013c0: 300a 2020 2020 2020 582d 4672 616d 652d  0.      X-Frame-
-000013d0: 4f70 7469 6f6e 733a 0a20 2020 2020 202d  Options:.      -
-000013e0: 2053 414d 454f 5249 4749 4e0a 2020 2020   SAMEORIGIN.    
-000013f0: 2020 582d 506f 7765 7265 642d 4279 3a0a    X-Powered-By:.
-00001400: 2020 2020 2020 2d20 2753 6572 766c 6574        - 'Servlet
-00001410: 2f34 2e30 204a 5350 2f32 2e33 2028 5061  /4.0 JSP/2.3 (Pa
-00001420: 7961 7261 2053 6572 7665 7220 2035 2e32  yara Server  5.2
-00001430: 3032 322e 3520 2362 6164 6173 7366 6973  022.5 #badassfis
-00001440: 6820 4a61 7661 2f45 636c 6970 7365 204f  h Java/Eclipse O
-00001450: 7065 6e4a 392f 312e 3829 270a 2020 2020  penJ9/1.8)'.    
-00001460: 7374 6174 7573 3a0a 2020 2020 2020 636f  status:.      co
-00001470: 6465 3a20 3230 300a 2020 2020 2020 6d65  de: 200.      me
-00001480: 7373 6167 653a 204f 4b0a 2020 2020 7572  ssage: OK.    ur
-00001490: 6c3a 2068 7474 7073 3a2f 2f74 696c 6173  l: https://tilas
-000014a0: 746f 2e6a 6174 656b 756b 6b6f 2e66 692f  to.jatekukko.fi/
-000014b0: 6a61 7465 6b75 6b6b 6f2f 7365 6375 7265  jatekukko/secure
-000014c0: 2f77 656c 6c2e 646f 0a2d 2072 6571 7565  /well.do.- reque
-000014d0: 7374 3a0a 2020 2020 626f 6479 3a20 6e75  st:.    body: nu
-000014e0: 6c6c 0a20 2020 2068 6561 6465 7273 3a0a  ll.    headers:.
-000014f0: 2020 2020 2020 4163 6365 7074 3a0a 2020        Accept:.  
-00001500: 2020 2020 2d20 272a 2f2a 270a 2020 2020      - '*/*'.    
-00001510: 2020 4163 6365 7074 2d45 6e63 6f64 696e    Accept-Encodin
-00001520: 673a 0a20 2020 2020 202d 2067 7a69 702c  g:.      - gzip,
-00001530: 2064 6566 6c61 7465 0a20 2020 2020 2048   deflate.      H
-00001540: 6f73 743a 0a20 2020 2020 202d 2074 696c  ost:.      - til
-00001550: 6173 746f 2e6a 6174 656b 756b 6b6f 2e66  asto.jatekukko.f
-00001560: 690a 2020 2020 2020 5573 6572 2d41 6765  i.      User-Age
-00001570: 6e74 3a0a 2020 2020 2020 2d20 5079 7468  nt:.      - Pyth
-00001580: 6f6e 2f33 2e31 3120 6169 6f68 7474 702f  on/3.11 aiohttp/
-00001590: 332e 382e 340a 2020 2020 6d65 7468 6f64  3.8.4.    method
-000015a0: 3a20 4745 540a 2020 2020 7572 693a 2068  : GET.    uri: h
-000015b0: 7474 7073 3a2f 2f74 696c 6173 746f 2e6a  ttps://tilasto.j
-000015c0: 6174 656b 756b 6b6f 2e66 692f 6a61 7465  atekukko.fi/jate
-000015d0: 6b75 6b6b 6f2f 6a5f 6163 6567 695f 6c6f  kukko/j_acegi_lo
-000015e0: 676f 7574 5f65 6c63 7573 7472 6170 0a20  gout_elcustrap. 
-000015f0: 2072 6573 706f 6e73 653a 0a20 2020 2062   response:.    b
-00001600: 6f64 793a 207b 7d0a 2020 2020 6865 6164  ody: {}.    head
-00001610: 6572 733a 0a20 2020 2020 2043 6f6e 6e65  ers:.      Conne
-00001620: 6374 696f 6e3a 0a20 2020 2020 202d 206b  ction:.      - k
-00001630: 6565 702d 616c 6976 650a 2020 2020 2020  eep-alive.      
-00001640: 436f 6e74 656e 742d 4c61 6e67 7561 6765  Content-Language
-00001650: 3a0a 2020 2020 2020 2d20 6669 2d46 490a  :.      - fi-FI.
-00001660: 2020 2020 2020 436f 6e74 656e 742d 4c65        Content-Le
-00001670: 6e67 7468 3a0a 2020 2020 2020 2d20 2731  ngth:.      - '1
-00001680: 3938 270a 2020 2020 2020 436f 6e74 656e  98'.      Conten
-00001690: 742d 5479 7065 3a0a 2020 2020 2020 2d20  t-Type:.      - 
-000016a0: 7465 7874 2f68 746d 6c3b 6368 6172 7365  text/html;charse
-000016b0: 743d 5554 462d 380a 2020 2020 2020 4461  t=UTF-8.      Da
-000016c0: 7465 3a0a 2020 2020 2020 2d20 4672 692c  te:.      - Fri,
-000016d0: 2032 3620 4d61 7920 3230 3233 2030 373a   26 May 2023 07:
-000016e0: 3538 3a30 3620 474d 540a 2020 2020 2020  58:06 GMT.      
-000016f0: 4c6f 6361 7469 6f6e 3a0a 2020 2020 2020  Location:.      
-00001700: 2d20 6874 7470 733a 2f2f 7469 6c61 7374  - https://tilast
-00001710: 6f2e 6a61 7465 6b75 6b6b 6f2e 6669 2f6a  o.jatekukko.fi/j
-00001720: 6174 656b 756b 6b6f 2f73 6168 6173 2e6a  atekukko/sahas.j
-00001730: 7370 0a20 2020 2020 2053 6572 7665 723a  sp.      Server:
-00001740: 0a20 2020 2020 202d 206e 6769 6e78 0a20  .      - nginx. 
-00001750: 2020 2020 2053 7472 6963 742d 5472 616e       Strict-Tran
-00001760: 7370 6f72 742d 5365 6375 7269 7479 3a0a  sport-Security:.
-00001770: 2020 2020 2020 2d20 6d61 782d 6167 653d        - max-age=
-00001780: 3633 3037 3230 3030 0a20 2020 2020 2058  63072000.      X
-00001790: 2d46 7261 6d65 2d4f 7074 696f 6e73 3a0a  -Frame-Options:.
-000017a0: 2020 2020 2020 2d20 5341 4d45 4f52 4947        - SAMEORIG
-000017b0: 494e 0a20 2020 2020 2058 2d50 6f77 6572  IN.      X-Power
-000017c0: 6564 2d42 793a 0a20 2020 2020 202d 2027  ed-By:.      - '
-000017d0: 5365 7276 6c65 742f 342e 3020 4a53 502f  Servlet/4.0 JSP/
-000017e0: 322e 3320 2850 6179 6172 6120 5365 7276  2.3 (Payara Serv
-000017f0: 6572 2020 352e 3230 3232 2e35 2023 6261  er  5.2022.5 #ba
-00001800: 6461 7373 6669 7368 204a 6176 612f 4563  dassfish Java/Ec
-00001810: 6c69 7073 6520 4f70 656e 4a39 2f31 2e38  lipse OpenJ9/1.8
-00001820: 2927 0a20 2020 2073 7461 7475 733a 0a20  )'.    status:. 
-00001830: 2020 2020 2063 6f64 653a 2033 3032 0a20       code: 302. 
-00001840: 2020 2020 206d 6573 7361 6765 3a20 466f       message: Fo
-00001850: 756e 640a 2020 2020 7572 6c3a 2068 7474  und.    url: htt
-00001860: 7073 3a2f 2f74 696c 6173 746f 2e6a 6174  ps://tilasto.jat
-00001870: 656b 756b 6b6f 2e66 692f 6a61 7465 6b75  ekukko.fi/jateku
-00001880: 6b6b 6f2f 6a5f 6163 6567 695f 6c6f 676f  kko/j_acegi_logo
-00001890: 7574 5f65 6c63 7573 7472 6170 0a2d 2072  ut_elcustrap.- r
-000018a0: 6571 7565 7374 3a0a 2020 2020 626f 6479  equest:.    body
-000018b0: 3a20 6e75 6c6c 0a20 2020 2068 6561 6465  : null.    heade
-000018c0: 7273 3a0a 2020 2020 2020 4163 6365 7074  rs:.      Accept
-000018d0: 3a0a 2020 2020 2020 2d20 272a 2f2a 270a  :.      - '*/*'.
-000018e0: 2020 2020 2020 4163 6365 7074 2d45 6e63        Accept-Enc
-000018f0: 6f64 696e 673a 0a20 2020 2020 202d 2067  oding:.      - g
-00001900: 7a69 702c 2064 6566 6c61 7465 0a20 2020  zip, deflate.   
-00001910: 2020 2048 6f73 743a 0a20 2020 2020 202d     Host:.      -
-00001920: 2074 696c 6173 746f 2e6a 6174 656b 756b   tilasto.jatekuk
-00001930: 6b6f 2e66 690a 2020 2020 2020 5573 6572  ko.fi.      User
-00001940: 2d41 6765 6e74 3a0a 2020 2020 2020 2d20  -Agent:.      - 
-00001950: 5079 7468 6f6e 2f33 2e31 3120 6169 6f68  Python/3.11 aioh
-00001960: 7474 702f 332e 382e 340a 2020 2020 6d65  ttp/3.8.4.    me
-00001970: 7468 6f64 3a20 4745 540a 2020 2020 7572  thod: GET.    ur
-00001980: 693a 2068 7474 7073 3a2f 2f74 696c 6173  i: https://tilas
-00001990: 746f 2e6a 6174 656b 756b 6b6f 2e66 692f  to.jatekukko.fi/
-000019a0: 6a61 7465 6b75 6b6b 6f2f 7361 6861 732e  jatekukko/sahas.
-000019b0: 6a73 700a 2020 7265 7370 6f6e 7365 3a0a  jsp.  response:.
-000019c0: 2020 2020 626f 6479 3a0a 2020 2020 2020      body:.      
-000019d0: 7374 7269 6e67 3a20 225c 725c 6e5c 725c  string: "\r\n\r\
-000019e0: 6e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  n\r\n\r\n\r\n\r\
-000019f0: 6e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  n\r\n\r\n\r\n\r\
-00001a00: 6e5c 725c 6e5c 725c 6e5c 725c 6e20 2020  n\r\n\r\n\r\n   
-00001a10: 205c 725c 6e20 2020 205c 725c 6e5c 725c   \r\n    \r\n\r\
-00001a20: 6e0a 2020 2020 2020 2020 5c20 2020 3c21  n.        \   <!
-00001a30: 646f 6374 7970 6520 6874 6d6c 3e5c 725c  doctype html>\r\
-00001a40: 6e5c 725c 6e20 2020 203c 6874 6d6c 206c  n\r\n    <html l
-00001a50: 616e 673d 5c22 6669 5f46 495c 223e 5c72  ang=\"fi_FI\">\r
-00001a60: 5c6e 5c72 5c6e 2020 2020 3c68 6561 643e  \n\r\n    <head>
-00001a70: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-00001a80: 2020 2020 203c 6d65 7461 2068 7474 702d       <meta http-
-00001a90: 6571 7569 763d 5c22 582d 5541 2d43 6f6d  equiv=\"X-UA-Com
-00001aa0: 7061 7469 626c 655c 2220 636f 6e74 656e  patible\" conten
-00001ab0: 743d 5c22 4945 3d65 6467 655c 223e 5c72  t=\"IE=edge\">\r
-00001ac0: 5c6e 2020 2020 2020 2020 3c6d 6574 610a  \n        <meta.
-00001ad0: 2020 2020 2020 2020 6368 6172 7365 743d          charset=
-00001ae0: 5c22 7574 662d 385c 223e 5c72 5c6e 2020  \"utf-8\">\r\n  
-00001af0: 2020 2020 2020 3c6d 6574 6120 6e61 6d65        <meta name
-00001b00: 3d5c 2276 6965 7770 6f72 745c 2220 636f  =\"viewport\" co
-00001b10: 6e74 656e 743d 5c22 7769 6474 683d 6465  ntent=\"width=de
-00001b20: 7669 6365 2d77 6964 7468 2c0a 2020 2020  vice-width,.    
-00001b30: 2020 2020 696e 6974 6961 6c2d 7363 616c      initial-scal
-00001b40: 653d 315c 223e 5c72 5c6e 5c72 5c6e 2020  e=1\">\r\n\r\n  
-00001b50: 2020 2020 2020 3c74 6974 6c65 3e4a 5c78        <title>J\x
-00001b60: 4534 7465 6b75 6b6b 6f20 4f79 202d 2053  E4tekukko Oy - S
-00001b70: 5c78 4534 686b 5c78 4636 696e 656e 0a20  \xE4hk\xF6inen. 
-00001b80: 2020 2020 2020 2061 7369 6f69 6e74 693c         asiointi<
-00001b90: 2f74 6974 6c65 3e5c 725c 6e5c 725c 6e20  /title>\r\n\r\n 
-00001ba0: 2020 2020 2020 205c 725c 6e5c 725c 6e20         \r\n\r\n 
-00001bb0: 2020 2020 2020 205c 725c 6e5c 725c 6e20         \r\n\r\n 
-00001bc0: 2020 2020 2020 203c 6c69 6e6b 2072 656c         <link rel
-00001bd0: 3d5c 2269 636f 6e5c 220a 2020 2020 2020  =\"icon\".      
-00001be0: 2020 6872 6566 3d5c 222f 6a61 7465 6b75    href=\"/jateku
-00001bf0: 6b6b 6f2f 696d 6167 6573 2f66 6176 6963  kko/images/favic
-00001c00: 6f6e 2e70 6e67 3f74 696d 6573 7461 6d70  on.png?timestamp
-00001c10: 3d32 3032 3330 3530 352d 3037 3239 5c22  =20230505-0729\"
-00001c20: 2074 7970 653d 5c22 696d 6167 652f 782d   type=\"image/x-
-00001c30: 6963 6f6e 5c22 3e5c 725c 6e0a 2020 2020  icon\">\r\n.    
-00001c40: 2020 2020 5c20 2020 2020 2020 3c6c 696e      \       <lin
-00001c50: 6b20 7265 6c3d 5c22 7368 6f72 7463 7574  k rel=\"shortcut
-00001c60: 2069 636f 6e5c 2220 6872 6566 3d5c 222f   icon\" href=\"/
-00001c70: 6a61 7465 6b75 6b6b 6f2f 696d 6167 6573  jatekukko/images
-00001c80: 2f66 6176 6963 6f6e 2e70 6e67 3f74 696d  /favicon.png?tim
-00001c90: 6573 7461 6d70 3d32 3032 3330 3530 352d  estamp=20230505-
-00001ca0: 3037 3239 5c22 5c72 5c6e 0a20 2020 2020  0729\"\r\n.     
-00001cb0: 2020 205c 2020 2020 2020 2020 2020 2020     \            
-00001cc0: 2074 7970 653d 5c22 696d 6167 652f 782d   type=\"image/x-
-00001cd0: 6963 6f6e 5c22 3e5c 725c 6e20 2020 2020  icon\">\r\n     
-00001ce0: 2020 203c 6c69 6e6b 2072 656c 3d5c 226d     <link rel=\"m
-00001cf0: 616e 6966 6573 745c 2220 6872 6566 3d5c  anifest\" href=\
-00001d00: 226d 616e 6966 6573 742e 6a73 6f6e 5c22  "manifest.json\"
-00001d10: 3e5c 725c 6e5c 725c 6e0a 2020 2020 2020  >\r\n\r\n.      
-00001d20: 2020 5c20 2020 2020 2020 5c72 5c6e 5c72    \       \r\n\r
-00001d30: 5c6e 5c72 5c6e 5c72 5c6e 3c73 7479 6c65  \n\r\n\r\n<style
-00001d40: 2069 643d 5c22 616e 7469 436c 6963 6b6a   id=\"antiClickj
-00001d50: 6163 6b5c 223e 626f 6479 7b64 6973 706c  ack\">body{displ
-00001d60: 6179 3a6e 6f6e 6520 2169 6d70 6f72 7461  ay:none !importa
-00001d70: 6e74 3b7d 3c2f 7374 796c 653e 5c72 5c6e  nt;}</style>\r\n
-00001d80: 5c72 5c6e 3c73 6372 6970 740a 2020 2020  \r\n<script.    
-00001d90: 2020 2020 7479 7065 3d5c 2274 6578 742f      type=\"text/
-00001da0: 6a61 7661 7363 7269 7074 5c22 3e5c 725c  javascript\">\r\
-00001db0: 6e5c 7469 6620 2873 656c 6620 3d3d 3d20  n\tif (self === 
-00001dc0: 746f 7029 207b 5c72 5c6e 5c74 5c74 5c72  top) {\r\n\t\t\r
-00001dd0: 5c6e 5c74 5c74 7661 7220 616e 7469 436c  \n\t\tvar antiCl
-00001de0: 6963 6b6a 6163 6b0a 2020 2020 2020 2020  ickjack.        
-00001df0: 3d20 646f 6375 6d65 6e74 2e67 6574 456c  = document.getEl
-00001e00: 656d 656e 7442 7949 6428 5c22 616e 7469  ementById(\"anti
-00001e10: 436c 6963 6b6a 6163 6b5c 2229 3b5c 725c  Clickjack\");\r\
-00001e20: 6e5c 745c 7461 6e74 6943 6c69 636b 6a61  n\t\tantiClickja
-00001e30: 636b 2e70 6172 656e 744e 6f64 652e 7265  ck.parentNode.re
-00001e40: 6d6f 7665 4368 696c 6428 616e 7469 436c  moveChild(antiCl
-00001e50: 6963 6b6a 6163 6b29 3b5c 725c 6e5c 747d  ickjack);\r\n\t}
-00001e60: 0a20 2020 2020 2020 2065 6c73 6520 7b5c  .        else {\
-00001e70: 725c 6e5c 745c 745c 725c 6e5c 745c 7474  r\n\t\t\r\n\t\tt
-00001e80: 6f70 2e6c 6f63 6174 696f 6e20 3d20 7365  op.location = se
-00001e90: 6c66 2e6c 6f63 6174 696f 6e3b 5c72 5c6e  lf.location;\r\n
-00001ea0: 5c74 7d5c 725c 6e3c 2f73 6372 6970 743e  \t}\r\n</script>
-00001eb0: 5c72 5c6e 5c72 5c6e 0a20 2020 2020 2020  \r\n\r\n.       
-00001ec0: 205c 2020 2020 2020 203c 212d 2d20 4468   \       <!-- Dh
-00001ed0: 746d 6c78 202d 2d3e 2020 2020 5c72 5c6e  tmlx -->    \r\n
-00001ee0: 3c6c 696e 6b20 7265 6c3d 5c22 7374 796c  <link rel=\"styl
-00001ef0: 6573 6865 6574 5c22 2074 7970 653d 5c22  esheet\" type=\"
-00001f00: 7465 7874 2f63 7373 5c22 0a20 2020 2020  text/css\".     
-00001f10: 2020 2068 7265 663d 5c22 2f6a 6174 656b     href=\"/jatek
-00001f20: 756b 6b6f 2f6a 732f 6468 746d 6c78 5375  ukko/js/dhtmlxSu
-00001f30: 6974 652f 636f 6465 6261 7365 2f64 6874  ite/codebase/dht
-00001f40: 6d6c 782e 6373 735c 223e 5c72 5c6e 3c6c  mlx.css\">\r\n<l
-00001f50: 696e 6b20 7265 6c3d 5c22 7374 796c 6573  ink rel=\"styles
-00001f60: 6865 6574 5c22 0a20 2020 2020 2020 2074  heet\".        t
-00001f70: 7970 653d 5c22 7465 7874 2f63 7373 5c22  ype=\"text/css\"
-00001f80: 2068 7265 663d 5c22 6a73 2f64 6874 6d6c   href=\"js/dhtml
-00001f90: 7853 7569 7465 2f73 6b69 6e73 2f74 6572  xSuite/skins/ter
-00001fa0: 7261 6365 2f64 6874 6d6c 782e 6373 735c  race/dhtmlx.css\
-00001fb0: 223e 5c72 5c6e 3c21 2d2d 0a20 2020 2020  ">\r\n<!--.     
-00001fc0: 2020 203c 6c69 6e6b 2072 656c 3d5c 2253     <link rel=\"S
-00001fd0: 5459 4c45 5348 4545 545c 2220 7479 7065  TYLESHEET\" type
-00001fe0: 3d5c 2274 6578 742f 6373 735c 2220 6872  =\"text/css\" hr
-00001ff0: 6566 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  ef=\"/jatekukko/
-00002000: 6a73 2f64 6874 6d6c 7853 7569 7465 2f73  js/dhtmlxSuite/s
-00002010: 6b69 6e73 2f73 6b79 626c 7565 2f64 6874  kins/skyblue/dht
-00002020: 6d6c 782e 6373 735c 223e 0a20 2020 2020  mlx.css\">.     
-00002030: 2020 202d 2d3e 5c72 5c6e 5c72 5c6e 5c72     -->\r\n\r\n\r
-00002040: 5c6e 3c21 2d2d 2041 7263 4749 5320 2d2d  \n<!-- ArcGIS --
-00002050: 3e5c 725c 6e3c 6c69 6e6b 2072 656c 3d5c  >\r\n<link rel=\
-00002060: 2273 7479 6c65 7368 6565 745c 2220 6872  "stylesheet\" hr
-00002070: 6566 3d5c 2268 7474 7073 3a2f 2f6a 732e  ef=\"https://js.
-00002080: 6172 6367 6973 2e63 6f6d 2f33 2e33 392f  arcgis.com/3.39/
-00002090: 6573 7269 2f63 7373 2f65 7372 692e 6373  esri/css/esri.cs
-000020a0: 735c 220a 2020 2020 2020 2020 2f3e 5c72  s\".        />\r
-000020b0: 5c6e 5c72 5c6e 3c21 2d2d 2042 6f6f 7473  \n\r\n<!-- Boots
-000020c0: 7472 6170 202d 2d3e 5c72 5c6e 3c6c 696e  trap -->\r\n<lin
-000020d0: 6b20 7265 6c3d 5c22 7374 796c 6573 6865  k rel=\"styleshe
-000020e0: 6574 5c22 2074 7970 653d 5c22 7465 7874  et\" type=\"text
-000020f0: 2f63 7373 5c22 0a20 2020 2020 2020 2068  /css\".        h
-00002100: 7265 663d 5c22 6373 732f 626f 6f74 7374  ref=\"css/bootst
-00002110: 7261 702f 626f 6f74 7374 7261 702e 6d69  rap/bootstrap.mi
-00002120: 6e2e 6373 735c 223e 5c72 5c6e 5c72 5c6e  n.css\">\r\n\r\n
-00002130: 3c21 2d2d 204b 656e 646f 5549 202d 2d3e  <!-- KendoUI -->
-00002140: 5c72 5c6e 3c6c 696e 6b0a 2020 2020 2020  \r\n<link.      
-00002150: 2020 7265 6c3d 5c22 7374 796c 6573 6865    rel=\"styleshe
-00002160: 6574 5c22 2074 7970 653d 5c22 7465 7874  et\" type=\"text
-00002170: 2f63 7373 5c22 2068 7265 663d 5c22 2f6a  /css\" href=\"/j
-00002180: 6174 656b 756b 6b6f 2f63 7373 2f6b 656e  atekukko/css/ken
-00002190: 646f 7569 2f6b 656e 646f 2e63 6f6d 6d6f  doui/kendo.commo
-000021a0: 6e2d 626f 6f74 7374 7261 702e 6d69 6e2e  n-bootstrap.min.
-000021b0: 6373 735c 223e 5c72 5c6e 3c6c 696e 6b0a  css\">\r\n<link.
-000021c0: 2020 2020 2020 2020 7265 6c3d 5c22 7374          rel=\"st
-000021d0: 796c 6573 6865 6574 5c22 2074 7970 653d  ylesheet\" type=
-000021e0: 5c22 7465 7874 2f63 7373 5c22 2068 7265  \"text/css\" hre
-000021f0: 663d 5c22 2f6a 6174 656b 756b 6b6f 2f63  f=\"/jatekukko/c
-00002200: 7373 2f6b 656e 646f 7569 2f6b 656e 646f  ss/kendoui/kendo
-00002210: 2e62 6f6f 7473 7472 6170 2e6d 696e 2e63  .bootstrap.min.c
-00002220: 7373 5c22 3e5c 725c 6e3c 6c69 6e6b 0a20  ss\">\r\n<link. 
-00002230: 2020 2020 2020 2072 656c 3d5c 2273 7479         rel=\"sty
-00002240: 6c65 7368 6565 745c 2220 7479 7065 3d5c  lesheet\" type=\
-00002250: 2274 6578 742f 6373 735c 2220 6872 6566  "text/css\" href
-00002260: 3d5c 2263 7373 2f6b 656e 646f 7569 2f6b  =\"css/kendoui/k
-00002270: 656e 646f 2e6d 6f62 696c 652e 616c 6c2e  endo.mobile.all.
-00002280: 6d69 6e2e 6373 735c 223e 5c72 5c6e 5c72  min.css\">\r\n\r
-00002290: 5c6e 3c21 2d2d 0a20 2020 2020 2020 2053  \n<!--.        S
-000022a0: 7479 6c65 7320 2d2d 3e5c 725c 6e3c 6c69  tyles -->\r\n<li
-000022b0: 6e6b 2072 656c 3d5c 2273 7479 6c65 7368  nk rel=\"stylesh
-000022c0: 6565 745c 2220 6872 6566 3d5c 2263 7373  eet\" href=\"css
-000022d0: 2f73 6861 7265 645f 6261 7365 2e63 7373  /shared_base.css
-000022e0: 3f74 696d 6573 7461 6d70 3d32 3032 3330  ?timestamp=20230
-000022f0: 3530 352d 3037 3239 5c22 3e5c 725c 6e3c  505-0729\">\r\n<
-00002300: 6c69 6e6b 0a20 2020 2020 2020 2072 656c  link.        rel
-00002310: 3d5c 2273 7479 6c65 7368 6565 745c 2220  =\"stylesheet\" 
-00002320: 6872 6566 3d5c 2263 7373 2f73 6168 6173  href=\"css/sahas
-00002330: 2f6d 6169 6e5f 6261 7365 2e63 7373 3f74  /main_base.css?t
-00002340: 696d 6573 7461 6d70 3d32 3032 3330 3530  imestamp=2023050
-00002350: 352d 3037 3239 5c22 3e5c 725c 6e5c 725c  5-0729\">\r\n\r\
-00002360: 6e3c 6c69 6e6b 0a20 2020 2020 2020 2072  n<link.        r
-00002370: 656c 3d5c 2273 7479 6c65 7368 6565 745c  el=\"stylesheet\
-00002380: 2220 6872 6566 3d5c 2263 7373 2f73 6861  " href=\"css/sha
-00002390: 7265 642e 6373 733f 7469 6d65 7374 616d  red.css?timestam
-000023a0: 703d 3230 3233 3035 3035 2d30 3732 395c  p=20230505-0729\
-000023b0: 223e 5c72 5c6e 3c6c 696e 6b0a 2020 2020  ">\r\n<link.    
-000023c0: 2020 2020 7265 6c3d 5c22 7374 796c 6573      rel=\"styles
-000023d0: 6865 6574 5c22 2068 7265 663d 5c22 6373  heet\" href=\"cs
-000023e0: 732f 7361 6861 732f 6d61 696e 2e63 7373  s/sahas/main.css
-000023f0: 3f74 696d 6573 7461 6d70 3d32 3032 3330  ?timestamp=20230
-00002400: 3530 352d 3037 3239 5c22 3e5c 725c 6e5c  505-0729\">\r\n\
-00002410: 725c 6e5c 725c 6e0a 2020 2020 2020 2020  r\n\r\n.        
-00002420: 5c20 2020 2020 2020 5c72 5c6e 5c72 5c6e  \       \r\n\r\n
-00002430: 3c6c 696e 6b20 6872 6566 3d27 6874 7470  <link href='http
-00002440: 733a 2f2f 666f 6e74 732e 676f 6f67 6c65  s://fonts.google
-00002450: 6170 6973 2e63 6f6d 2f63 7373 3f66 616d  apis.com/css?fam
-00002460: 696c 793d 4c61 746f 3a33 3030 2c33 3030  ily=Lato:300,300
-00002470: 4974 616c 6963 2c34 3030 2c34 3030 6974  Italic,400,400it
-00002480: 616c 6963 2c37 3030 2c37 3030 6974 616c  alic,700,700ital
-00002490: 6963 270a 2020 2020 2020 2020 7265 6c3d  ic'.        rel=
-000024a0: 2773 7479 6c65 7368 6565 7427 2074 7970  'stylesheet' typ
-000024b0: 653d 2774 6578 742f 6373 7327 2f3e 5c72  e='text/css'/>\r
-000024c0: 5c6e 3c6c 696e 6b20 7265 6c3d 5c22 7374  \n<link rel=\"st
-000024d0: 796c 6573 6865 6574 5c22 2074 7970 653d  ylesheet\" type=
-000024e0: 5c22 7465 7874 2f63 7373 5c22 0a20 2020  \"text/css\".   
-000024f0: 2020 2020 2068 7265 663d 5c22 6874 7470       href=\"http
-00002500: 733a 2f2f 666f 6e74 732e 676f 6f67 6c65  s://fonts.google
-00002510: 6170 6973 2e63 6f6d 2f63 7373 3f66 616d  apis.com/css?fam
-00002520: 696c 793d 5054 2b53 616e 735c 222f 3e5c  ily=PT+Sans\"/>\
-00002530: 725c 6e3c 6c69 6e6b 2068 7265 663d 5c22  r\n<link href=\"
-00002540: 6874 7470 733a 2f2f 666f 6e74 732e 676f  https://fonts.go
-00002550: 6f67 6c65 6170 6973 2e63 6f6d 2f63 7373  ogleapis.com/css
-00002560: 3f66 616d 696c 793d 5369 676e 696b 613a  ?family=Signika:
-00002570: 3330 302c 3430 305c 220a 2020 2020 2020  300,400\".      
-00002580: 2020 7265 6c3d 5c22 7374 796c 6573 6865    rel=\"styleshe
-00002590: 6574 5c22 2f3e 5c72 5c6e 2020 2020 3c2f  et\"/>\r\n    </
-000025a0: 6865 6164 3e5c 725c 6e5c 725c 6e20 2020  head>\r\n\r\n   
-000025b0: 203c 626f 6479 2069 643d 5c22 7361 6861   <body id=\"saha
-000025c0: 735c 2220 636c 6173 733d 5c22 6c6f 6769  s\" class=\"logi
-000025d0: 6e5c 223e 5c72 5c6e 0a20 2020 2020 2020  n\">\r\n.       
-000025e0: 205c 2020 205c 725c 6e20 2020 203c 6865   \   \r\n    <he
-000025f0: 6164 6572 3e5c 725c 6e20 2020 2020 2020  ader>\r\n       
-00002600: 203c 6469 7620 6964 3d5c 2262 726f 7773   <div id=\"brows
-00002610: 6572 2d69 6e63 6f6d 7061 7469 626c 652d  er-incompatible-
-00002620: 6d65 7373 6167 655c 2220 636c 6173 733d  message\" class=
-00002630: 5c22 616c 6572 740a 2020 2020 2020 2020  \"alert.        
-00002640: 616c 6572 742d 6461 6e67 6572 2074 6578  alert-danger tex
-00002650: 742d 6365 6e74 6572 5c22 2073 7479 6c65  t-center\" style
-00002660: 3d5c 2264 6973 706c 6179 3a20 6e6f 6e65  =\"display: none
-00002670: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
-00002680: 2020 2053 656c 6169 6e76 6572 7369 6f73     Selainversios
-00002690: 690a 2020 2020 2020 2020 6569 206f 6c65  i.        ei ole
-000026a0: 2076 6572 6b6b 6f70 616c 7665 6c75 6e20   verkkopalvelun 
-000026b0: 7475 6574 7475 6a65 6e20 7365 6c61 696e  tuettujen selain
-000026c0: 7465 6e20 6c69 7374 616c 6c61 2e20 5665  ten listalla. Ve
-000026d0: 726b 6b6f 7061 6c76 656c 7520 6569 2076  rkkopalvelu ei v
-000026e0: 5c78 4534 6c74 745c 7845 346d 5c78 4534  \xE4ltt\xE4m\xE4
-000026f0: 7474 5c78 4534 0a20 2020 2020 2020 2074  tt\xE4.        t
-00002700: 6f69 6d69 206f 696b 6569 6e2e 5c72 5c6e  oimi oikein.\r\n
-00002710: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-00002720: 5c6e 5c72 5c6e 2020 2020 2020 2020 5c72  \n\r\n        \r
-00002730: 5c6e 5c72 5c6e 2020 2020 2020 2020 3c6e  \n\r\n        <n
-00002740: 6176 2063 6c61 7373 3d5c 226e 6176 6261  av class=\"navba
-00002750: 725c 223e 5c72 5c6e 0a20 2020 2020 2020  r\">\r\n.       
-00002760: 205c 2020 2020 2020 2020 2020 203c 6469   \           <di
-00002770: 7620 636c 6173 733d 5c22 636f 6e74 6169  v class=\"contai
-00002780: 6e65 725c 223e 5c72 5c6e 2020 2020 2020  ner\">\r\n      
-00002790: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-000027a0: 6c61 7373 3d5c 226e 6176 6261 722d 6865  lass=\"navbar-he
-000027b0: 6164 6572 5c22 3e5c 725c 6e0a 2020 2020  ader\">\r\n.    
-000027c0: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-000027d0: 2020 2020 2020 2020 3c62 7574 746f 6e20          <button 
-000027e0: 7479 7065 3d5c 2262 7574 746f 6e5c 2220  type=\"button\" 
-000027f0: 636c 6173 733d 5c22 6e61 7662 6172 2d74  class=\"navbar-t
-00002800: 6f67 676c 6520 636f 6c6c 6170 7365 645c  oggle collapsed\
-00002810: 220a 2020 2020 2020 2020 6461 7461 2d74  ".        data-t
-00002820: 6f67 676c 653d 5c22 636f 6c6c 6170 7365  oggle=\"collapse
-00002830: 5c22 5c72 5c6e 2020 2020 2020 2020 2020  \"\r\n          
-00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002850: 2020 6461 7461 2d74 6172 6765 743d 5c22    data-target=\"
-00002860: 236e 6176 6261 722d 636f 6c6c 6170 7365  #navbar-collapse
-00002870: 5c22 0a20 2020 2020 2020 2061 7269 612d  \".        aria-
-00002880: 6578 7061 6e64 6564 3d5c 2266 616c 7365  expanded=\"false
-00002890: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
-000028a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000028b0: 7370 616e 2063 6c61 7373 3d5c 2273 722d  span class=\"sr-
-000028c0: 6f6e 6c79 5c22 3e41 7661 610a 2020 2020  only\">Avaa.    
-000028d0: 2020 2020 7661 6c69 6b6b 6f3c 2f73 7061      valikko</spa
-000028e0: 6e3e 5c72 5c6e 2020 2020 2020 2020 2020  n>\r\n          
-000028f0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00002900: 7061 6e20 636c 6173 733d 5c22 6963 6f6e  pan class=\"icon
-00002910: 2d62 6172 5c22 3e3c 2f73 7061 6e3e 5c72  -bar\"></span>\r
-00002920: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002940: 2020 203c 7370 616e 2063 6c61 7373 3d5c     <span class=\
-00002950: 2269 636f 6e2d 6261 725c 223e 3c2f 7370  "icon-bar\"></sp
-00002960: 616e 3e5c 725c 6e20 2020 2020 2020 2020  an>\r\n         
-00002970: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002980: 7370 616e 0a20 2020 2020 2020 2063 6c61  span.        cla
-00002990: 7373 3d5c 2269 636f 6e2d 6261 725c 223e  ss=\"icon-bar\">
-000029a0: 3c2f 7370 616e 3e5c 725c 6e20 2020 2020  </span>\r\n     
-000029b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000029c0: 2f62 7574 746f 6e3e 5c72 5c6e 2020 2020  /button>\r\n    
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a00: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a20: 2020 2020 203c 6120 6872 6566 3d5c 2268       <a href=\"h
-00002a30: 7474 7073 3a2f 2f77 7777 2e6a 6174 656b  ttps://www.jatek
-00002a40: 756b 6b6f 2e66 692f 5c22 3e5c 725c 6e0a  ukko.fi/\">\r\n.
-00002a50: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
-00002a80: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 696d  =\"/jatekukko/im
-00002a90: 6167 6573 2f6a 6174 656b 756b 6b6f 2d6c  ages/jatekukko-l
-00002aa0: 6f67 6f2d 7465 6b73 7469 2e70 6e67 5c22  ogo-teksti.png\"
-00002ab0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ae0: 2020 616c 743d 5c22 4a5c 7845 3474 656b    alt=\"J\xE4tek
-00002af0: 756b 6b6f 204f 795c 2220 636c 6173 733d  ukko Oy\" class=
-00002b00: 5c22 6e61 7662 6172 2d62 7261 6e64 5c22  \"navbar-brand\"
-00002b10: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 2020 2020 2020 3c2f 613e 5c72            </a>\r
-00002b40: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00002b50: 2020 2020 2020 2020 2020 5c72 5c6e 2020            \r\n  
-00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b70: 2020 2020 2020 5c72 5c6e 0a20 2020 2020        \r\n.     
-00002b80: 2020 205c 2020 2020 2020 2020 2020 2020     \            
-00002b90: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
-00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 2020 205c 725c 6e20 2020 2020 2020 2020     \r\n         
-00002bc0: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
-00002bd0: 6e5c 725c 6e0a 2020 2020 2020 2020 5c20  n\r\n.        \ 
-00002be0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00002bf0: 6976 2063 6c61 7373 3d5c 2263 6f6c 6c61  iv class=\"colla
-00002c00: 7073 6520 6e61 7662 6172 2d63 6f6c 6c61  pse navbar-colla
-00002c10: 7073 655c 2220 6964 3d5c 226e 6176 6261  pse\" id=\"navba
-00002c20: 722d 636f 6c6c 6170 7365 5c22 3e5c 725c  r-collapse\">\r\
-00002c30: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-00002c40: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00002c50: 6976 2063 6c61 7373 3d5c 226e 6176 6261  iv class=\"navba
-00002c60: 722d 7269 6768 745c 223e 5c72 5c6e 2020  r-right\">\r\n  
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2020 2020 2020 5c72 5c6e 0a20 2020 2020        \r\n.     
-00002c90: 2020 205c 2020 2020 2020 2020 2020 2020     \            
-00002ca0: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cc0: 2020 2020 2020 205c 725c 6e20 2020 2020         \r\n     
-00002cd0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002ce0: 2f64 6976 3e5c 725c 6e0a 2020 2020 2020  /div>\r\n.      
-00002cf0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-00002d00: 2020 3c2f 6469 763e 5c72 5c6e 2020 2020    </div>\r\n    
-00002d10: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-00002d20: 5c6e 2020 2020 2020 2020 3c2f 6e61 763e  \n        </nav>
-00002d30: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
-00002d40: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-00002d50: 203c 2f68 6561 6465 723e 5c72 5c6e 5c72   </header>\r\n\r
-00002d60: 5c6e 2020 2020 3c6d 6169 6e3e 5c72 5c6e  \n    <main>\r\n
-00002d70: 2020 2020 2020 2020 3c64 6976 2064 6174          <div dat
-00002d80: 612d 726f 6c65 3d5c 226d 6169 6e2d 7461  a-role=\"main-ta
-00002d90: 6262 6172 5c22 3e5c 725c 6e0a 2020 2020  bbar\">\r\n.    
-00002da0: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-00002db0: 3c68 6561 6465 7220 636c 6173 733d 5c22  <header class=\"
-00002dc0: 636f 6e74 6169 6e65 725c 2220 7374 796c  container\" styl
-00002dd0: 653d 5c22 6469 7370 6c61 793a 6e6f 6e65  e=\"display:none
-00002de0: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
-00002df0: 2020 2020 2020 203c 6469 760a 2020 2020         <div.    
-00002e00: 2020 2020 636c 6173 733d 5c22 726f 775c      class=\"row\
-00002e10: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
-00002e20: 2020 2020 2020 2020 2020 3c75 6c20 636c            <ul cl
-00002e30: 6173 733d 5c22 6e61 7620 6e61 7662 6172  ass=\"nav navbar
-00002e40: 2d6e 6176 206e 6176 6261 722d 7269 6768  -nav navbar-righ
-00002e50: 740a 2020 2020 2020 2020 7461 622d 6c69  t.        tab-li
-00002e60: 7374 5c22 2064 6174 612d 726f 6c65 3d5c  st\" data-role=\
-00002e70: 2274 6162 2d6c 6973 745c 225c 725c 6e20  "tab-list\"\r\n 
-00002e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e90: 2020 2020 2020 2073 7479 6c65 3d5c 2264         style=\"d
-00002ea0: 6973 706c 6179 3a6e 6f6e 655c 223e 5c72  isplay:none\">\r
-00002eb0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ed0: 2020 203c 6c69 2063 6c61 7373 3d5c 226c     <li class=\"l
-00002ee0: 6f67 696e 2061 6374 6976 655c 223e 3c61  ogin active\"><a
-00002ef0: 2068 7265 663d 5c22 236c 6f67 696e 5c22   href=\"#login\"
-00002f00: 3e4b 6972 6a61 7564 753c 2f61 3e3c 2f6c  >Kirjaudu</a></l
-00002f10: 693e 5c72 5c6e 0a20 2020 2020 2020 205c  i>\r\n.        \
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 2020 2020 2020 203c 6c69 2063 6c61 7373         <li class
-00002f40: 3d5c 2273 6572 7669 6365 735c 223e 3c61  =\"services\"><a
-00002f50: 2068 7265 663d 5c22 2373 6572 7669 6365   href=\"#service
-00002f60: 735c 223e 5061 6c76 656c 7574 3c2f 613e  s\">Palvelut</a>
-00002f70: 3c2f 6c69 3e5c 725c 6e0a 2020 2020 2020  </li>\r\n.      
-00002f80: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-00002f90: 2020 2020 2020 2020 2020 5c72 5c6e 2020            \r\n  
-00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fb0: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
-00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fd0: 2020 2020 2020 3c6c 690a 2020 2020 2020        <li.      
-00002fe0: 2020 636c 6173 733d 5c22 6375 7374 6f6d    class=\"custom
-00002ff0: 6572 2d64 6174 615c 223e 3c61 2068 7265  er-data\"><a hre
-00003000: 663d 5c22 2363 7573 746f 6d65 722d 6461  f=\"#customer-da
-00003010: 7461 5c22 3e4b 6f68 7465 656e 2074 6965  ta\">Kohteen tie
-00003020: 646f 743c 2f61 3e3c 2f6c 693e 5c72 5c6e  dot</a></li>\r\n
-00003030: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003050: 205c 725c 6e20 2020 2020 2020 2020 2020   \r\n           
-00003060: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
-00003070: 2063 6c61 7373 3d5c 2275 7365 722d 6465   class=\"user-de
-00003080: 7461 696c 735c 223e 3c61 0a20 2020 2020  tails\"><a.     
-00003090: 2020 2068 7265 663d 5c22 2375 7365 722d     href=\"#user-
-000030a0: 6465 7461 696c 735c 223e 4f6d 6174 2074  details\">Omat t
-000030b0: 6965 646f 743c 2f61 3e3c 2f6c 693e 5c72  iedot</a></li>\r
-000030c0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-000030d0: 2020 2020 2020 2020 2020 5c72 5c6e 0a20            \r\n. 
-000030e0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-000030f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003100: 2020 203c 6c69 2063 6c61 7373 3d5c 2269     <li class=\"i
-00003110: 6e76 6f69 6365 735c 223e 3c61 2068 7265  nvoices\"><a hre
-00003120: 663d 5c22 2369 6e76 6f69 6365 735c 223e  f=\"#invoices\">
-00003130: 4c61 736b 7574 3c2f 613e 3c2f 6c69 3e5c  Laskut</a></li>\
-00003140: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00000020: 793a 206e 756c 6c0a 2020 2020 6865 6164  y: null.    head
+00000030: 6572 733a 0a20 2020 2020 2041 6363 6570  ers:.      Accep
+00000040: 743a 0a20 2020 2020 202d 2027 2a2f 2a27  t:.      - '*/*'
+00000050: 0a20 2020 2020 2041 6363 6570 742d 456e  .      Accept-En
+00000060: 636f 6469 6e67 3a0a 2020 2020 2020 2d20  coding:.      - 
+00000070: 677a 6970 2c20 6465 666c 6174 650a 2020  gzip, deflate.  
+00000080: 2020 2020 486f 7374 3a0a 2020 2020 2020      Host:.      
+00000090: 2d20 7469 6c61 7374 6f2e 6a61 7465 6b75  - tilasto.jateku
+000000a0: 6b6b 6f2e 6669 0a20 2020 2020 2055 7365  kko.fi.      Use
+000000b0: 722d 4167 656e 743a 0a20 2020 2020 202d  r-Agent:.      -
+000000c0: 2050 7974 686f 6e2f 332e 3920 6169 6f68   Python/3.9 aioh
+000000d0: 7474 702f 332e 372e 342e 706f 7374 300a  ttp/3.7.4.post0.
+000000e0: 2020 2020 6d65 7468 6f64 3a20 4745 540a      method: GET.
+000000f0: 2020 2020 7572 693a 2068 7474 7073 3a2f      uri: https:/
+00000100: 2f74 696c 6173 746f 2e6a 6174 656b 756b  /tilasto.jatekuk
+00000110: 6b6f 2e66 692f 6a61 7465 6b75 6b6b 6f2f  ko.fi/jatekukko/
+00000120: 6a5f 6163 6567 695f 6c6f 676f 7574 5f65  j_acegi_logout_e
+00000130: 6c63 7573 7472 6170 0a20 2072 6573 706f  lcustrap.  respo
+00000140: 6e73 653a 0a20 2020 2062 6f64 793a 207b  nse:.    body: {
+00000150: 7d0a 2020 2020 6865 6164 6572 733a 0a20  }.    headers:. 
+00000160: 2020 2020 2043 6f6e 6e65 6374 696f 6e3a       Connection:
+00000170: 0a20 2020 2020 202d 206b 6565 702d 616c  .      - keep-al
+00000180: 6976 650a 2020 2020 2020 436f 6e74 656e  ive.      Conten
+00000190: 742d 4c61 6e67 7561 6765 3a0a 2020 2020  t-Language:.    
+000001a0: 2020 2d20 6669 2d46 490a 2020 2020 2020    - fi-FI.      
+000001b0: 436f 6e74 656e 742d 4c65 6e67 7468 3a0a  Content-Length:.
+000001c0: 2020 2020 2020 2d20 2731 3938 270a 2020        - '198'.  
+000001d0: 2020 2020 436f 6e74 656e 742d 5479 7065      Content-Type
+000001e0: 3a0a 2020 2020 2020 2d20 7465 7874 2f68  :.      - text/h
+000001f0: 746d 6c3b 6368 6172 7365 743d 5554 462d  tml;charset=UTF-
+00000200: 380a 2020 2020 2020 4461 7465 3a0a 2020  8.      Date:.  
+00000210: 2020 2020 2d20 5361 742c 2030 3420 5365      - Sat, 04 Se
+00000220: 7020 3230 3231 2030 383a 3538 3a33 3020  p 2021 08:58:30 
+00000230: 474d 540a 2020 2020 2020 4c6f 6361 7469  GMT.      Locati
+00000240: 6f6e 3a0a 2020 2020 2020 2d20 6874 7470  on:.      - http
+00000250: 733a 2f2f 7469 6c61 7374 6f2e 6a61 7465  s://tilasto.jate
+00000260: 6b75 6b6b 6f2e 6669 2f6a 6174 656b 756b  kukko.fi/jatekuk
+00000270: 6b6f 2f73 6168 6173 2e6a 7370 0a20 2020  ko/sahas.jsp.   
+00000280: 2020 2053 6572 7665 723a 0a20 2020 2020     Server:.     
+00000290: 202d 206e 6769 6e78 0a20 2020 2020 2053   - nginx.      S
+000002a0: 7472 6963 742d 5472 616e 7370 6f72 742d  trict-Transport-
+000002b0: 5365 6375 7269 7479 3a0a 2020 2020 2020  Security:.      
+000002c0: 2d20 6d61 782d 6167 653d 3633 3037 3230  - max-age=630720
+000002d0: 3030 0a20 2020 2020 2058 2d46 7261 6d65  00.      X-Frame
+000002e0: 2d4f 7074 696f 6e73 3a0a 2020 2020 2020  -Options:.      
+000002f0: 2d20 5341 4d45 4f52 4947 494e 0a20 2020  - SAMEORIGIN.   
+00000300: 2020 2058 2d50 6f77 6572 6564 2d42 793a     X-Powered-By:
+00000310: 0a20 2020 2020 202d 2027 5365 7276 6c65  .      - 'Servle
+00000320: 742f 342e 3020 4a53 502f 322e 3320 2850  t/4.0 JSP/2.3 (P
+00000330: 6179 6172 6120 5365 7276 6572 2020 352e  ayara Server  5.
+00000340: 3230 3231 2e35 2023 6261 6461 7373 6669  2021.5 #badassfi
+00000350: 7368 204a 6176 612f 4563 6c69 7073 6520  sh Java/Eclipse 
+00000360: 4f70 656e 4a39 2f31 2e38 2927 0a20 2020  OpenJ9/1.8)'.   
+00000370: 2073 7461 7475 733a 0a20 2020 2020 2063   status:.      c
+00000380: 6f64 653a 2033 3032 0a20 2020 2020 206d  ode: 302.      m
+00000390: 6573 7361 6765 3a20 466f 756e 640a 2020  essage: Found.  
+000003a0: 2020 7572 6c3a 2068 7474 7073 3a2f 2f74    url: https://t
+000003b0: 696c 6173 746f 2e6a 6174 656b 756b 6b6f  ilasto.jatekukko
+000003c0: 2e66 692f 6a61 7465 6b75 6b6b 6f2f 6a5f  .fi/jatekukko/j_
+000003d0: 6163 6567 695f 6c6f 676f 7574 5f65 6c63  acegi_logout_elc
+000003e0: 7573 7472 6170 0a2d 2072 6571 7565 7374  ustrap.- request
+000003f0: 3a0a 2020 2020 626f 6479 3a20 6e75 6c6c  :.    body: null
+00000400: 0a20 2020 2068 6561 6465 7273 3a0a 2020  .    headers:.  
+00000410: 2020 2020 4163 6365 7074 3a0a 2020 2020      Accept:.    
+00000420: 2020 2d20 272a 2f2a 270a 2020 2020 2020    - '*/*'.      
+00000430: 4163 6365 7074 2d45 6e63 6f64 696e 673a  Accept-Encoding:
+00000440: 0a20 2020 2020 202d 2067 7a69 702c 2064  .      - gzip, d
+00000450: 6566 6c61 7465 0a20 2020 2020 2048 6f73  eflate.      Hos
+00000460: 743a 0a20 2020 2020 202d 2074 696c 6173  t:.      - tilas
+00000470: 746f 2e6a 6174 656b 756b 6b6f 2e66 690a  to.jatekukko.fi.
+00000480: 2020 2020 2020 5573 6572 2d41 6765 6e74        User-Agent
+00000490: 3a0a 2020 2020 2020 2d20 5079 7468 6f6e  :.      - Python
+000004a0: 2f33 2e39 2061 696f 6874 7470 2f33 2e37  /3.9 aiohttp/3.7
+000004b0: 2e34 2e70 6f73 7430 0a20 2020 206d 6574  .4.post0.    met
+000004c0: 686f 643a 2047 4554 0a20 2020 2075 7269  hod: GET.    uri
+000004d0: 3a20 6874 7470 733a 2f2f 7469 6c61 7374  : https://tilast
+000004e0: 6f2e 6a61 7465 6b75 6b6b 6f2e 6669 2f6a  o.jatekukko.fi/j
+000004f0: 6174 656b 756b 6b6f 2f73 6168 6173 2e6a  atekukko/sahas.j
+00000500: 7370 0a20 2072 6573 706f 6e73 653a 0a20  sp.  response:. 
+00000510: 2020 2062 6f64 793a 0a20 2020 2020 2073     body:.      s
+00000520: 7472 696e 673a 2022 5c72 5c6e 5c72 5c6e  tring: "\r\n\r\n
+00000530: 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e  \r\n\r\n\r\n\r\n
+00000540: 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e  \r\n\r\n\r\n\r\n
+00000550: 5c72 5c6e 5c72 5c6e 5c72 5c6e 2020 2020  \r\n\r\n\r\n    
+00000560: 5c72 5c6e 2020 2020 5c72 5c6e 5c72 5c6e  \r\n    \r\n\r\n
+00000570: 0a20 2020 2020 2020 205c 2020 203c 2164  .        \   <!d
+00000580: 6f63 7479 7065 2068 746d 6c3e 5c72 5c6e  octype html>\r\n
+00000590: 5c72 5c6e 2020 2020 3c68 746d 6c20 6c61  \r\n    <html la
+000005a0: 6e67 3d5c 2266 695f 4649 5c22 3e5c 725c  ng=\"fi_FI\">\r\
+000005b0: 6e5c 725c 6e20 2020 203c 6865 6164 3e5c  n\r\n    <head>\
+000005c0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+000005d0: 2020 2020 3c6d 6574 6120 6874 7470 2d65      <meta http-e
+000005e0: 7175 6976 3d5c 2258 2d55 412d 436f 6d70  quiv=\"X-UA-Comp
+000005f0: 6174 6962 6c65 5c22 2063 6f6e 7465 6e74  atible\" content
+00000600: 3d5c 2249 453d 6564 6765 5c22 3e5c 725c  =\"IE=edge\">\r\
+00000610: 6e20 2020 2020 2020 203c 6d65 7461 0a20  n        <meta. 
+00000620: 2020 2020 2020 2063 6861 7273 6574 3d5c         charset=\
+00000630: 2275 7466 2d38 5c22 3e5c 725c 6e20 2020  "utf-8\">\r\n   
+00000640: 2020 2020 203c 6d65 7461 206e 616d 653d       <meta name=
+00000650: 5c22 7669 6577 706f 7274 5c22 2063 6f6e  \"viewport\" con
+00000660: 7465 6e74 3d5c 2277 6964 7468 3d64 6576  tent=\"width=dev
+00000670: 6963 652d 7769 6474 682c 0a20 2020 2020  ice-width,.     
+00000680: 2020 2069 6e69 7469 616c 2d73 6361 6c65     initial-scale
+00000690: 3d31 5c22 3e5c 725c 6e5c 725c 6e20 2020  =1\">\r\n\r\n   
+000006a0: 2020 2020 203c 7469 746c 653e 4a5c 7845       <title>J\xE
+000006b0: 3474 656b 756b 6b6f 204f 7920 2d20 535c  4tekukko Oy - S\
+000006c0: 7845 3468 6b5c 7846 3669 6e65 6e0a 2020  xE4hk\xF6inen.  
+000006d0: 2020 2020 2020 6173 696f 696e 7469 3c2f        asiointi</
+000006e0: 7469 746c 653e 5c72 5c6e 5c72 5c6e 2020  title>\r\n\r\n  
+000006f0: 2020 2020 2020 5c72 5c6e 5c72 5c6e 2020        \r\n\r\n  
+00000700: 2020 2020 2020 5c72 5c6e 5c72 5c6e 2020        \r\n\r\n  
+00000710: 2020 2020 2020 3c6c 696e 6b20 7265 6c3d        <link rel=
+00000720: 5c22 6963 6f6e 5c22 0a20 2020 2020 2020  \"icon\".       
+00000730: 2068 7265 663d 5c22 2f6a 6174 656b 756b   href=\"/jatekuk
+00000740: 6b6f 2f69 6d61 6765 732f 6661 7669 636f  ko/images/favico
+00000750: 6e2e 706e 673f 7469 6d65 7374 616d 703d  n.png?timestamp=
+00000760: 3230 3231 3037 3139 2d31 3433 365c 2220  20210719-1436\" 
+00000770: 7479 7065 3d5c 2269 6d61 6765 2f78 2d69  type=\"image/x-i
+00000780: 636f 6e5c 223e 5c72 5c6e 0a20 2020 2020  con\">\r\n.     
+00000790: 2020 205c 2020 2020 2020 203c 6c69 6e6b     \       <link
+000007a0: 2072 656c 3d5c 2273 686f 7274 6375 7420   rel=\"shortcut 
+000007b0: 6963 6f6e 5c22 2068 7265 663d 5c22 2f6a  icon\" href=\"/j
+000007c0: 6174 656b 756b 6b6f 2f69 6d61 6765 732f  atekukko/images/
+000007d0: 6661 7669 636f 6e2e 706e 673f 7469 6d65  favicon.png?time
+000007e0: 7374 616d 703d 3230 3231 3037 3139 2d31  stamp=20210719-1
+000007f0: 3433 365c 225c 725c 6e0a 2020 2020 2020  436\"\r\n.      
+00000800: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+00000810: 7479 7065 3d5c 2269 6d61 6765 2f78 2d69  type=\"image/x-i
+00000820: 636f 6e5c 223e 5c72 5c6e 2020 2020 2020  con\">\r\n      
+00000830: 2020 3c6c 696e 6b20 7265 6c3d 5c22 6d61    <link rel=\"ma
+00000840: 6e69 6665 7374 5c22 2068 7265 663d 5c22  nifest\" href=\"
+00000850: 6d61 6e69 6665 7374 2e6a 736f 6e5c 223e  manifest.json\">
+00000860: 5c72 5c6e 5c72 5c6e 0a20 2020 2020 2020  \r\n\r\n.       
+00000870: 205c 2020 2020 2020 205c 725c 6e5c 725c   \       \r\n\r\
+00000880: 6e5c 725c 6e5c 725c 6e3c 7374 796c 6520  n\r\n\r\n<style 
+00000890: 6964 3d5c 2261 6e74 6943 6c69 636b 6a61  id=\"antiClickja
+000008a0: 636b 5c22 3e62 6f64 797b 6469 7370 6c61  ck\">body{displa
+000008b0: 793a 6e6f 6e65 2021 696d 706f 7274 616e  y:none !importan
+000008c0: 743b 7d3c 2f73 7479 6c65 3e5c 725c 6e5c  t;}</style>\r\n\
+000008d0: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
+000008e0: 2020 2074 7970 653d 5c22 7465 7874 2f6a     type=\"text/j
+000008f0: 6176 6173 6372 6970 745c 223e 5c72 5c6e  avascript\">\r\n
+00000900: 5c74 6966 2028 7365 6c66 203d 3d3d 2074  \tif (self === t
+00000910: 6f70 2920 7b5c 725c 6e5c 745c 745c 725c  op) {\r\n\t\t\r\
+00000920: 6e5c 745c 7476 6172 2061 6e74 6943 6c69  n\t\tvar antiCli
+00000930: 636b 6a61 636b 0a20 2020 2020 2020 203d  ckjack.        =
+00000940: 2064 6f63 756d 656e 742e 6765 7445 6c65   document.getEle
+00000950: 6d65 6e74 4279 4964 285c 2261 6e74 6943  mentById(\"antiC
+00000960: 6c69 636b 6a61 636b 5c22 293b 5c72 5c6e  lickjack\");\r\n
+00000970: 5c74 5c74 616e 7469 436c 6963 6b6a 6163  \t\tantiClickjac
+00000980: 6b2e 7061 7265 6e74 4e6f 6465 2e72 656d  k.parentNode.rem
+00000990: 6f76 6543 6869 6c64 2861 6e74 6943 6c69  oveChild(antiCli
+000009a0: 636b 6a61 636b 293b 5c72 5c6e 5c74 7d0a  ckjack);\r\n\t}.
+000009b0: 2020 2020 2020 2020 656c 7365 207b 5c72          else {\r
+000009c0: 5c6e 5c74 5c74 5c72 5c6e 5c74 5c74 746f  \n\t\t\r\n\t\tto
+000009d0: 702e 6c6f 6361 7469 6f6e 203d 2073 656c  p.location = sel
+000009e0: 662e 6c6f 6361 7469 6f6e 3b5c 725c 6e5c  f.location;\r\n\
+000009f0: 747d 5c72 5c6e 3c2f 7363 7269 7074 3e5c  t}\r\n</script>\
+00000a00: 725c 6e5c 725c 6e0a 2020 2020 2020 2020  r\n\r\n.        
+00000a10: 5c20 2020 2020 2020 3c21 2d2d 2044 6874  \       <!-- Dht
+00000a20: 6d6c 7820 2d2d 3e20 2020 205c 725c 6e3c  mlx -->    \r\n<
+00000a30: 6c69 6e6b 2072 656c 3d5c 2273 7479 6c65  link rel=\"style
+00000a40: 7368 6565 745c 2220 7479 7065 3d5c 2274  sheet\" type=\"t
+00000a50: 6578 742f 6373 735c 220a 2020 2020 2020  ext/css\".      
+00000a60: 2020 6872 6566 3d5c 222f 6a61 7465 6b75    href=\"/jateku
+00000a70: 6b6b 6f2f 6a73 2f64 6874 6d6c 7853 7569  kko/js/dhtmlxSui
+00000a80: 7465 2f63 6f64 6562 6173 652f 6468 746d  te/codebase/dhtm
+00000a90: 6c78 2e63 7373 5c22 3e5c 725c 6e3c 6c69  lx.css\">\r\n<li
+00000aa0: 6e6b 2072 656c 3d5c 2273 7479 6c65 7368  nk rel=\"stylesh
+00000ab0: 6565 745c 220a 2020 2020 2020 2020 7479  eet\".        ty
+00000ac0: 7065 3d5c 2274 6578 742f 6373 735c 2220  pe=\"text/css\" 
+00000ad0: 6872 6566 3d5c 226a 732f 6468 746d 6c78  href=\"js/dhtmlx
+00000ae0: 5375 6974 652f 736b 696e 732f 7465 7272  Suite/skins/terr
+00000af0: 6163 652f 6468 746d 6c78 2e63 7373 5c22  ace/dhtmlx.css\"
+00000b00: 3e5c 725c 6e3c 212d 2d0a 2020 2020 2020  >\r\n<!--.      
+00000b10: 2020 3c6c 696e 6b20 7265 6c3d 5c22 5354    <link rel=\"ST
+00000b20: 594c 4553 4845 4554 5c22 2074 7970 653d  YLESHEET\" type=
+00000b30: 5c22 7465 7874 2f63 7373 5c22 2068 7265  \"text/css\" hre
+00000b40: 663d 5c22 2f6a 6174 656b 756b 6b6f 2f6a  f=\"/jatekukko/j
+00000b50: 732f 6468 746d 6c78 5375 6974 652f 736b  s/dhtmlxSuite/sk
+00000b60: 696e 732f 736b 7962 6c75 652f 6468 746d  ins/skyblue/dhtm
+00000b70: 6c78 2e63 7373 5c22 3e0a 2020 2020 2020  lx.css\">.      
+00000b80: 2020 2d2d 3e5c 725c 6e5c 725c 6e5c 725c    -->\r\n\r\n\r\
+00000b90: 6e3c 212d 2d20 4172 6347 4953 202d 2d3e  n<!-- ArcGIS -->
+00000ba0: 5c72 5c6e 3c6c 696e 6b20 7265 6c3d 5c22  \r\n<link rel=\"
+00000bb0: 7374 796c 6573 6865 6574 5c22 2068 7265  stylesheet\" hre
+00000bc0: 663d 5c22 6874 7470 733a 2f2f 6a73 2e61  f=\"https://js.a
+00000bd0: 7263 6769 732e 636f 6d2f 332e 3333 2f65  rcgis.com/3.33/e
+00000be0: 7372 692f 6373 732f 6573 7269 2e63 7373  sri/css/esri.css
+00000bf0: 5c22 0a20 2020 2020 2020 202f 3e5c 725c  \".        />\r\
+00000c00: 6e5c 725c 6e3c 212d 2d20 426f 6f74 7374  n\r\n<!-- Bootst
+00000c10: 7261 7020 2d2d 3e5c 725c 6e3c 6c69 6e6b  rap -->\r\n<link
+00000c20: 2072 656c 3d5c 2273 7479 6c65 7368 6565   rel=\"styleshee
+00000c30: 745c 2220 7479 7065 3d5c 2274 6578 742f  t\" type=\"text/
+00000c40: 6373 735c 220a 2020 2020 2020 2020 6872  css\".        hr
+00000c50: 6566 3d5c 2263 7373 2f62 6f6f 7473 7472  ef=\"css/bootstr
+00000c60: 6170 2f62 6f6f 7473 7472 6170 2e6d 696e  ap/bootstrap.min
+00000c70: 2e63 7373 5c22 3e5c 725c 6e5c 725c 6e3c  .css\">\r\n\r\n<
+00000c80: 212d 2d20 4b65 6e64 6f55 4920 2d2d 3e5c  !-- KendoUI -->\
+00000c90: 725c 6e3c 6c69 6e6b 0a20 2020 2020 2020  r\n<link.       
+00000ca0: 2072 656c 3d5c 2273 7479 6c65 7368 6565   rel=\"styleshee
+00000cb0: 745c 2220 7479 7065 3d5c 2274 6578 742f  t\" type=\"text/
+00000cc0: 6373 735c 2220 6872 6566 3d5c 222f 6a61  css\" href=\"/ja
+00000cd0: 7465 6b75 6b6b 6f2f 6373 732f 6b65 6e64  tekukko/css/kend
+00000ce0: 6f75 692f 6b65 6e64 6f2e 636f 6d6d 6f6e  oui/kendo.common
+00000cf0: 2d62 6f6f 7473 7472 6170 2e6d 696e 2e63  -bootstrap.min.c
+00000d00: 7373 5c22 3e5c 725c 6e3c 6c69 6e6b 0a20  ss\">\r\n<link. 
+00000d10: 2020 2020 2020 2072 656c 3d5c 2273 7479         rel=\"sty
+00000d20: 6c65 7368 6565 745c 2220 7479 7065 3d5c  lesheet\" type=\
+00000d30: 2274 6578 742f 6373 735c 2220 6872 6566  "text/css\" href
+00000d40: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6373  =\"/jatekukko/cs
+00000d50: 732f 6b65 6e64 6f75 692f 6b65 6e64 6f2e  s/kendoui/kendo.
+00000d60: 626f 6f74 7374 7261 702e 6d69 6e2e 6373  bootstrap.min.cs
+00000d70: 735c 223e 5c72 5c6e 3c6c 696e 6b0a 2020  s\">\r\n<link.  
+00000d80: 2020 2020 2020 7265 6c3d 5c22 7374 796c        rel=\"styl
+00000d90: 6573 6865 6574 5c22 2074 7970 653d 5c22  esheet\" type=\"
+00000da0: 7465 7874 2f63 7373 5c22 2068 7265 663d  text/css\" href=
+00000db0: 5c22 6373 732f 6b65 6e64 6f75 692f 6b65  \"css/kendoui/ke
+00000dc0: 6e64 6f2e 6d6f 6269 6c65 2e61 6c6c 2e6d  ndo.mobile.all.m
+00000dd0: 696e 2e63 7373 5c22 3e5c 725c 6e5c 725c  in.css\">\r\n\r\
+00000de0: 6e3c 212d 2d0a 2020 2020 2020 2020 5374  n<!--.        St
+00000df0: 796c 6573 202d 2d3e 5c72 5c6e 3c6c 696e  yles -->\r\n<lin
+00000e00: 6b20 7265 6c3d 5c22 7374 796c 6573 6865  k rel=\"styleshe
+00000e10: 6574 5c22 2068 7265 663d 5c22 6373 732f  et\" href=\"css/
+00000e20: 7368 6172 6564 5f62 6173 652e 6373 733f  shared_base.css?
+00000e30: 7469 6d65 7374 616d 703d 3230 3231 3037  timestamp=202107
+00000e40: 3139 2d31 3433 365c 223e 5c72 5c6e 3c6c  19-1436\">\r\n<l
+00000e50: 696e 6b0a 2020 2020 2020 2020 7265 6c3d  ink.        rel=
+00000e60: 5c22 7374 796c 6573 6865 6574 5c22 2068  \"stylesheet\" h
+00000e70: 7265 663d 5c22 6373 732f 7361 6861 732f  ref=\"css/sahas/
+00000e80: 6d61 696e 5f62 6173 652e 6373 733f 7469  main_base.css?ti
+00000e90: 6d65 7374 616d 703d 3230 3231 3037 3139  mestamp=20210719
+00000ea0: 2d31 3433 365c 223e 5c72 5c6e 5c72 5c6e  -1436\">\r\n\r\n
+00000eb0: 3c6c 696e 6b0a 2020 2020 2020 2020 7265  <link.        re
+00000ec0: 6c3d 5c22 7374 796c 6573 6865 6574 5c22  l=\"stylesheet\"
+00000ed0: 2068 7265 663d 5c22 6373 732f 7368 6172   href=\"css/shar
+00000ee0: 6564 2e63 7373 3f74 696d 6573 7461 6d70  ed.css?timestamp
+00000ef0: 3d32 3032 3130 3731 392d 3134 3336 5c22  =20210719-1436\"
+00000f00: 3e5c 725c 6e3c 6c69 6e6b 0a20 2020 2020  >\r\n<link.     
+00000f10: 2020 2072 656c 3d5c 2273 7479 6c65 7368     rel=\"stylesh
+00000f20: 6565 745c 2220 6872 6566 3d5c 2263 7373  eet\" href=\"css
+00000f30: 2f73 6168 6173 2f6d 6169 6e2e 6373 733f  /sahas/main.css?
+00000f40: 7469 6d65 7374 616d 703d 3230 3231 3037  timestamp=202107
+00000f50: 3139 2d31 3433 365c 223e 5c72 5c6e 5c72  19-1436\">\r\n\r
+00000f60: 5c6e 5c72 5c6e 0a20 2020 2020 2020 205c  \n\r\n.        \
+00000f70: 2020 2020 2020 205c 725c 6e5c 725c 6e3c         \r\n\r\n<
+00000f80: 6c69 6e6b 2068 7265 663d 2768 7474 7073  link href='https
+00000f90: 3a2f 2f66 6f6e 7473 2e67 6f6f 676c 6561  ://fonts.googlea
+00000fa0: 7069 732e 636f 6d2f 6373 733f 6661 6d69  pis.com/css?fami
+00000fb0: 6c79 3d4c 6174 6f3a 3330 302c 3330 3049  ly=Lato:300,300I
+00000fc0: 7461 6c69 632c 3430 302c 3430 3069 7461  talic,400,400ita
+00000fd0: 6c69 632c 3730 302c 3730 3069 7461 6c69  lic,700,700itali
+00000fe0: 6327 0a20 2020 2020 2020 2072 656c 3d27  c'.        rel='
+00000ff0: 7374 796c 6573 6865 6574 2720 7479 7065  stylesheet' type
+00001000: 3d27 7465 7874 2f63 7373 272f 3e5c 725c  ='text/css'/>\r\
+00001010: 6e3c 6c69 6e6b 2072 656c 3d5c 2273 7479  n<link rel=\"sty
+00001020: 6c65 7368 6565 745c 2220 7479 7065 3d5c  lesheet\" type=\
+00001030: 2274 6578 742f 6373 735c 220a 2020 2020  "text/css\".    
+00001040: 2020 2020 6872 6566 3d5c 2268 7474 7073      href=\"https
+00001050: 3a2f 2f66 6f6e 7473 2e67 6f6f 676c 6561  ://fonts.googlea
+00001060: 7069 732e 636f 6d2f 6373 733f 6661 6d69  pis.com/css?fami
+00001070: 6c79 3d50 542b 5361 6e73 5c22 2f3e 5c72  ly=PT+Sans\"/>\r
+00001080: 5c6e 3c6c 696e 6b20 6872 6566 3d5c 2268  \n<link href=\"h
+00001090: 7474 7073 3a2f 2f66 6f6e 7473 2e67 6f6f  ttps://fonts.goo
+000010a0: 676c 6561 7069 732e 636f 6d2f 6373 733f  gleapis.com/css?
+000010b0: 6661 6d69 6c79 3d53 6967 6e69 6b61 3a33  family=Signika:3
+000010c0: 3030 2c34 3030 5c22 0a20 2020 2020 2020  00,400\".       
+000010d0: 2072 656c 3d5c 2273 7479 6c65 7368 6565   rel=\"styleshee
+000010e0: 745c 222f 3e5c 725c 6e20 2020 203c 2f68  t\"/>\r\n    </h
+000010f0: 6561 643e 5c72 5c6e 5c72 5c6e 2020 2020  ead>\r\n\r\n    
+00001100: 3c62 6f64 7920 6964 3d5c 2273 6168 6173  <body id=\"sahas
+00001110: 5c22 2063 6c61 7373 3d5c 226c 6f67 696e  \" class=\"login
+00001120: 5c22 3e5c 725c 6e0a 2020 2020 2020 2020  \">\r\n.        
+00001130: 5c20 2020 5c72 5c6e 2020 2020 3c68 6561  \   \r\n    <hea
+00001140: 6465 723e 5c72 5c6e 2020 2020 2020 2020  der>\r\n        
+00001150: 3c64 6976 2069 643d 5c22 6272 6f77 7365  <div id=\"browse
+00001160: 722d 696e 636f 6d70 6174 6962 6c65 2d6d  r-incompatible-m
+00001170: 6573 7361 6765 5c22 2063 6c61 7373 3d5c  essage\" class=\
+00001180: 2261 6c65 7274 0a20 2020 2020 2020 2061  "alert.        a
+00001190: 6c65 7274 2d64 616e 6765 7220 7465 7874  lert-danger text
+000011a0: 2d63 656e 7465 725c 2220 7374 796c 653d  -center\" style=
+000011b0: 5c22 6469 7370 6c61 793a 206e 6f6e 655c  \"display: none\
+000011c0: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
+000011d0: 2020 5365 6c61 696e 7665 7273 696f 7369    Selainversiosi
+000011e0: 0a20 2020 2020 2020 2065 6920 6f6c 6520  .        ei ole 
+000011f0: 7665 726b 6b6f 7061 6c76 656c 756e 2074  verkkopalvelun t
+00001200: 7565 7474 756a 656e 2073 656c 6169 6e74  uettujen selaint
+00001210: 656e 206c 6973 7461 6c6c 612e 2056 6572  en listalla. Ver
+00001220: 6b6b 6f70 616c 7665 6c75 2065 6920 765c  kkopalvelu ei v\
+00001230: 7845 346c 7474 5c78 4534 6d5c 7845 3474  xE4ltt\xE4m\xE4t
+00001240: 745c 7845 340a 2020 2020 2020 2020 746f  t\xE4.        to
+00001250: 696d 6920 6f69 6b65 696e 2e5c 725c 6e20  imi oikein.\r\n 
+00001260: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
+00001270: 6e5c 725c 6e20 2020 2020 2020 205c 725c  n\r\n        \r\
+00001280: 6e5c 725c 6e20 2020 2020 2020 203c 6e61  n\r\n        <na
+00001290: 7620 636c 6173 733d 5c22 6e61 7662 6172  v class=\"navbar
+000012a0: 5c22 3e5c 725c 6e0a 2020 2020 2020 2020  \">\r\n.        
+000012b0: 5c20 2020 2020 2020 2020 2020 3c64 6976  \           <div
+000012c0: 2063 6c61 7373 3d5c 2263 6f6e 7461 696e   class=\"contain
+000012d0: 6572 5c22 3e5c 725c 6e20 2020 2020 2020  er\">\r\n       
+000012e0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+000012f0: 6173 733d 5c22 6e61 7662 6172 2d68 6561  ass=\"navbar-hea
+00001300: 6465 725c 223e 5c72 5c6e 0a20 2020 2020  der\">\r\n.     
+00001310: 2020 205c 2020 2020 2020 2020 2020 2020     \            
+00001320: 2020 2020 2020 203c 6275 7474 6f6e 2074         <button t
+00001330: 7970 653d 5c22 6275 7474 6f6e 5c22 2063  ype=\"button\" c
+00001340: 6c61 7373 3d5c 226e 6176 6261 722d 746f  lass=\"navbar-to
+00001350: 6767 6c65 2063 6f6c 6c61 7073 6564 5c22  ggle collapsed\"
+00001360: 0a20 2020 2020 2020 2064 6174 612d 746f  .        data-to
+00001370: 6767 6c65 3d5c 2263 6f6c 6c61 7073 655c  ggle=\"collapse\
+00001380: 225c 725c 6e20 2020 2020 2020 2020 2020  "\r\n           
+00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013a0: 2064 6174 612d 7461 7267 6574 3d5c 2223   data-target=\"#
+000013b0: 6e61 7662 6172 2d63 6f6c 6c61 7073 655c  navbar-collapse\
+000013c0: 220a 2020 2020 2020 2020 6172 6961 2d65  ".        aria-e
+000013d0: 7870 616e 6465 643d 5c22 6661 6c73 655c  xpanded=\"false\
+000013e0: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
+000013f0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00001400: 7061 6e20 636c 6173 733d 5c22 7372 2d6f  pan class=\"sr-o
+00001410: 6e6c 795c 223e 4176 6161 0a20 2020 2020  nly\">Avaa.     
+00001420: 2020 2076 616c 696b 6b6f 3c2f 7370 616e     valikko</span
+00001430: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+00001440: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
+00001450: 616e 2063 6c61 7373 3d5c 2269 636f 6e2d  an class=\"icon-
+00001460: 6261 725c 223e 3c2f 7370 616e 3e5c 725c  bar\"></span>\r\
+00001470: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001490: 2020 3c73 7061 6e20 636c 6173 733d 5c22    <span class=\"
+000014a0: 6963 6f6e 2d62 6172 5c22 3e3c 2f73 7061  icon-bar\"></spa
+000014b0: 6e3e 5c72 5c6e 2020 2020 2020 2020 2020  n>\r\n          
+000014c0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+000014d0: 7061 6e0a 2020 2020 2020 2020 636c 6173  pan.        clas
+000014e0: 733d 5c22 6963 6f6e 2d62 6172 5c22 3e3c  s=\"icon-bar\"><
+000014f0: 2f73 7061 6e3e 5c72 5c6e 2020 2020 2020  /span>\r\n      
+00001500: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001510: 6275 7474 6f6e 3e5c 725c 6e20 2020 2020  button>\r\n     
+00001520: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00001530: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001550: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 2020 2020 3c61 2068 7265 663d 5c22 6874      <a href=\"ht
+00001580: 7470 733a 2f2f 7777 772e 6a61 7465 6b75  tps://www.jateku
+00001590: 6b6b 6f2e 6669 2f5c 223e 5c72 5c6e 0a20  kko.fi/\">\r\n. 
+000015a0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+000015d0: 5c22 2f6a 6174 656b 756b 6b6f 2f69 6d61  \"/jatekukko/ima
+000015e0: 6765 732f 6a61 7465 6b75 6b6b 6f2d 6c6f  ges/jatekukko-lo
+000015f0: 676f 2d74 656b 7374 692e 706e 675c 225c  go-teksti.png\"\
+00001600: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001630: 2061 6c74 3d5c 224a 5c78 4534 7465 6b75   alt=\"J\xE4teku
+00001640: 6b6b 6f20 4f79 5c22 2063 6c61 7373 3d5c  kko Oy\" class=\
+00001650: 226e 6176 6261 722d 6272 616e 645c 223e  "navbar-brand\">
+00001660: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001680: 2020 2020 2020 2020 203c 2f61 3e5c 725c           </a>\r\
+00001690: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+000016a0: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
+000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016c0: 2020 2020 205c 725c 6e0a 2020 2020 2020       \r\n.      
+000016d0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+000016e0: 2020 2020 2020 2020 2020 5c72 5c6e 2020            \r\n  
+000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001700: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
+00001710: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
+00001720: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+00001730: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00001740: 7620 636c 6173 733d 5c22 636f 6c6c 6170  v class=\"collap
+00001750: 7365 206e 6176 6261 722d 636f 6c6c 6170  se navbar-collap
+00001760: 7365 5c22 2069 643d 5c22 6e61 7662 6172  se\" id=\"navbar
+00001770: 2d63 6f6c 6c61 7073 655c 223e 5c72 5c6e  -collapse\">\r\n
+00001780: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+00001790: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+000017a0: 7620 636c 6173 733d 5c22 6e61 7662 6172  v class=\"navbar
+000017b0: 2d72 6967 6874 5c22 3e5c 725c 6e20 2020  -right\">\r\n   
+000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017d0: 2020 2020 205c 725c 6e0a 2020 2020 2020       \r\n.      
+000017e0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+000017f0: 2020 2020 2020 2020 2020 5c72 5c6e 2020            \r\n  
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
+00001820: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001830: 6469 763e 5c72 5c6e 0a20 2020 2020 2020  div>\r\n.       
+00001840: 205c 2020 2020 2020 2020 2020 2020 2020   \              
+00001850: 203c 2f64 6976 3e5c 725c 6e20 2020 2020   </div>\r\n     
+00001860: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
+00001870: 6e20 2020 2020 2020 203c 2f6e 6176 3e5c  n        </nav>\
+00001880: 725c 6e5c 725c 6e20 2020 2020 2020 205c  r\n\r\n        \
+00001890: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+000018a0: 3c2f 6865 6164 6572 3e5c 725c 6e5c 725c  </header>\r\n\r\
+000018b0: 6e20 2020 203c 6d61 696e 3e5c 725c 6e20  n    <main>\r\n 
+000018c0: 2020 2020 2020 203c 6469 7620 6461 7461         <div data
+000018d0: 2d72 6f6c 653d 5c22 6d61 696e 2d74 6162  -role=\"main-tab
+000018e0: 6261 725c 223e 5c72 5c6e 0a20 2020 2020  bar\">\r\n.     
+000018f0: 2020 205c 2020 2020 2020 2020 2020 203c     \           <
+00001900: 6865 6164 6572 2063 6c61 7373 3d5c 2263  header class=\"c
+00001910: 6f6e 7461 696e 6572 5c22 2073 7479 6c65  ontainer\" style
+00001920: 3d5c 2264 6973 706c 6179 3a6e 6f6e 655c  =\"display:none\
+00001930: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
+00001940: 2020 2020 2020 3c64 6976 0a20 2020 2020        <div.     
+00001950: 2020 2063 6c61 7373 3d5c 2272 6f77 5c22     class=\"row\"
+00001960: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+00001970: 2020 2020 2020 2020 203c 756c 2063 6c61           <ul cla
+00001980: 7373 3d5c 226e 6176 206e 6176 6261 722d  ss=\"nav navbar-
+00001990: 6e61 7620 6e61 7662 6172 2d72 6967 6874  nav navbar-right
+000019a0: 0a20 2020 2020 2020 2074 6162 2d6c 6973  .        tab-lis
+000019b0: 745c 2220 6461 7461 2d72 6f6c 653d 5c22  t\" data-role=\"
+000019c0: 7461 622d 6c69 7374 5c22 5c72 5c6e 2020  tab-list\"\r\n  
+000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019e0: 2020 2020 2020 7374 796c 653d 5c22 6469        style=\"di
+000019f0: 7370 6c61 793a 6e6f 6e65 5c22 3e5c 725c  splay:none\">\r\
+00001a00: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a20: 2020 3c6c 6920 636c 6173 733d 5c22 6c6f    <li class=\"lo
+00001a30: 6769 6e20 6163 7469 7665 5c22 3e3c 6120  gin active\"><a 
+00001a40: 6872 6566 3d5c 2223 6c6f 6769 6e5c 223e  href=\"#login\">
+00001a50: 4b69 726a 6175 6475 3c2f 613e 3c2f 6c69  Kirjaudu</a></li
+00001a60: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
+00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a80: 2020 2020 2020 3c6c 6920 636c 6173 733d        <li class=
+00001a90: 5c22 7365 7276 6963 6573 5c22 3e3c 6120  \"services\"><a 
+00001aa0: 6872 6566 3d5c 2223 7365 7276 6963 6573  href=\"#services
+00001ab0: 5c22 3e50 616c 7665 6c75 743c 2f61 3e3c  \">Palvelut</a><
+00001ac0: 2f6c 693e 5c72 5c6e 0a20 2020 2020 2020  /li>\r\n.       
+00001ad0: 205c 2020 2020 2020 2020 2020 2020 2020   \              
+00001ae0: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
+00001af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b00: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
+00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b20: 2020 2020 203c 6c69 0a20 2020 2020 2020       <li.       
+00001b30: 2063 6c61 7373 3d5c 2263 7573 746f 6d65   class=\"custome
+00001b40: 722d 6461 7461 5c22 3e3c 6120 6872 6566  r-data\"><a href
+00001b50: 3d5c 2223 6375 7374 6f6d 6572 2d64 6174  =\"#customer-dat
+00001b60: 615c 223e 4b6f 6874 6565 6e20 7469 6564  a\">Kohteen tied
+00001b70: 6f74 3c2f 613e 3c2f 6c69 3e5c 725c 6e0a  ot</a></li>\r\n.
+00001b80: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ba0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00001bb0: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
+00001bc0: 636c 6173 733d 5c22 7573 6572 2d64 6574  class=\"user-det
+00001bd0: 6169 6c73 5c22 3e3c 610a 2020 2020 2020  ails\"><a.      
+00001be0: 2020 6872 6566 3d5c 2223 7573 6572 2d64    href=\"#user-d
+00001bf0: 6574 6169 6c73 5c22 3e4f 6d61 7420 7469  etails\">Omat ti
+00001c00: 6564 6f74 3c2f 613e 3c2f 6c69 3e5c 725c  edot</a></li>\r\
+00001c10: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00001c20: 2020 2020 2020 2020 205c 725c 6e0a 2020           \r\n.  
+00001c30: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c50: 2020 3c6c 6920 636c 6173 733d 5c22 696e    <li class=\"in
+00001c60: 766f 6963 6573 5c22 3e3c 6120 6872 6566  voices\"><a href
+00001c70: 3d5c 2223 696e 766f 6963 6573 5c22 3e4c  =\"#invoices\">L
+00001c80: 6173 6b75 743c 2f61 3e3c 2f6c 693e 5c72  askut</a></li>\r
+00001c90: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cb0: 2020 205c 725c 6e20 2020 2020 2020 2020     \r\n         
+00001cc0: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00001cd0: 725c 6e5c 725c 6e20 2020 2020 2020 2020  r\n\r\n         
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cf0: 2020 205c 725c 6e0a 2020 2020 2020 2020     \r\n.        
+00001d00: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+00001d10: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
+00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d50: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
+00001d60: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2020 2020 205c 725c 6e5c 725c 6e20 2020       \r\n\r\n   
+00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001da0: 2020 2020 2020 2020 205c 725c 6e5c 725c           \r\n\r\
+00001db0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dd0: 205c 725c 6e0a 2020 2020 2020 2020 5c20   \r\n.        \ 
+00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001df0: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+00001e00: 5c6e 5c72 5c6e 2020 2020 2020 2020 2020  \n\r\n          
+00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e20: 2020 2020 2020 2020 2020 5c72 5c6e 5c72            \r\n\r
+00001e30: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001e60: 6c69 2063 6c61 7373 3d5c 2266 6565 6462  li class=\"feedb
+00001e70: 6163 6b5c 223e 3c61 5c72 5c6e 2020 2020  ack\"><a\r\n    
+00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ea0: 2020 2020 2020 2020 6872 6566 3d5c 2223          href=\"#
+00001eb0: 6665 6564 6261 636b 5c22 3e50 616c 6175  feedback\">Palau
+00001ec0: 7465 3c2f 613e 3c2f 6c69 3e5c 725c 6e5c  te</a></li>\r\n\
+00001ed0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f00: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
+00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f20: 2020 2020 2020 2020 5c72 5c6e 0a20 2020          \r\n.   
+00001f30: 2020 2020 205c 2020 2020 2020 2020 2020       \          
+00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f50: 205c 725c 6e5c 725c 6e20 2020 2020 2020   \r\n\r\n       
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f70: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
+00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f90: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
+00001fa0: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+00001fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fc0: 2020 2020 2020 5c72 5c6e 5c72 5c6e 2020        \r\n\r\n  
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fe0: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+00001ff0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002010: 2020 5c72 5c6e 0a20 2020 2020 2020 205c    \r\n.        \
+00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002030: 2020 2020 2020 2020 2020 205c 725c 6e5c             \r\n\
+00002040: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00002050: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
+00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002070: 2020 2020 2020 203c 6c69 0a20 2020 2020         <li.     
+00002080: 2020 2063 6c61 7373 3d5c 226c 6f67 6f75     class=\"logou
+00002090: 745c 223e 3c61 2068 7265 663d 5c22 236c  t\"><a href=\"#l
+000020a0: 6f67 6f75 745c 225c 725c 6e20 2020 2020  ogout\"\r\n     
+000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020d0: 2020 2020 2020 2020 206f 6e63 6c69 636b           onclick
+000020e0: 3d5c 2277 696e 646f 772e 6c6f 6361 7469  =\"window.locati
+000020f0: 6f6e 3d62 6173 6575 726c 0a20 2020 2020  on=baseurl.     
+00002100: 2020 202b 2027 2f6a 5f61 6365 6769 5f6c     + '/j_acegi_l
+00002110: 6f67 6f75 745f 656c 6375 7374 7261 7027  ogout_elcustrap'
+00002120: 5c22 3e4b 6972 6a61 7564 7520 756c 6f73  \">Kirjaudu ulos
+00002130: 3c2f 613e 3c2f 6c69 3e5c 725c 6e20 2020  </a></li>\r\n   
+00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002150: 2020 2020 205c 725c 6e0a 2020 2020 2020       \r\n.      
+00002160: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+00002170: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+00002180: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00002190: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+000021a0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+000021b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021c0: 2020 5c72 5c6e 0a20 2020 2020 2020 205c    \r\n.        \
+000021d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021e0: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
+000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002200: 2020 2020 2020 2020 2020 203c 6c69 2063             <li c
+00002210: 6c61 7373 3d5c 2265 7869 7475 7365 725c  lass=\"exituser\
+00002220: 223e 3c61 0a20 2020 2020 2020 2068 7265  "><a.        hre
+00002230: 663d 5c22 2365 7869 7475 7365 725c 225c  f=\"#exituser\"\
+00002240: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002270: 2020 2020 2020 206f 6e63 6c69 636b 3d5c         onclick=\
+00002280: 2277 696e 646f 772e 6c6f 6361 7469 6f6e  "window.location
+00002290: 3d62 6173 6575 726c 0a20 2020 2020 2020  =baseurl.       
+000022a0: 202b 2027 2f6a 6174 656b 756b 6b6f 2f6a   + '/jatekukko/j
+000022b0: 5f61 6365 6769 5f65 7869 745f 7573 6572  _acegi_exit_user
+000022c0: 3f72 6564 6972 6563 743d 2f73 6563 7572  ?redirect=/secur
+000022d0: 652f 6164 6d69 6e2f 7573 6572 732e 646f  e/admin/users.do
+000022e0: 275c 223e 4c6f 7065 7461 0a20 2020 2020  '\">Lopeta.     
+000022f0: 2020 2070 6569 6c61 7573 3c2f 613e 3c2f     peilaus</a></
+00002300: 6c69 3e5c 725c 6e20 2020 2020 2020 2020  li>\r\n         
+00002310: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00002320: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00002330: 2020 2020 2020 203c 2f75 6c3e 5c72 5c6e         </ul>\r\n
+00002340: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+00002350: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
+00002360: 725c 6e5c 725c 6e20 2020 2020 2020 2020  r\n\r\n         
+00002370: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00002380: 733d 5c22 726f 775c 223e 5c72 5c6e 2020  s=\"row\">\r\n  
+00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023a0: 2020 3c64 6976 0a20 2020 2020 2020 2063    <div.        c
+000023b0: 6c61 7373 3d5c 2263 6f6c 2d6c 672d 6f66  lass=\"col-lg-of
+000023c0: 6673 6574 2d32 2063 6f6c 2d6c 672d 385c  fset-2 col-lg-8\
+000023d0: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
+000023e0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+000023f0: 6976 2069 643d 5c22 7365 7276 6963 652d  iv id=\"service-
+00002400: 7365 6c65 6374 6f72 5c22 0a20 2020 2020  selector\".     
+00002410: 2020 2063 6c61 7373 3d5c 2273 6572 7669     class=\"servi
+00002420: 6365 2d73 656c 6563 746f 725c 2220 7374  ce-selector\" st
+00002430: 796c 653d 5c22 6469 7370 6c61 793a 6e6f  yle=\"display:no
+00002440: 6e65 5c22 3e3c 2f64 6976 3e5c 725c 6e20  ne\"></div>\r\n 
+00002450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002460: 2020 203c 2f64 6976 3e5c 725c 6e0a 2020     </div>\r\n.  
+00002470: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+00002480: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
+00002490: 2020 2020 2020 2020 2020 2020 3c2f 6865              </he
+000024a0: 6164 6572 3e5c 725c 6e5c 725c 6e20 2020  ader>\r\n\r\n   
+000024b0: 2020 2020 2020 2020 203c 7365 6374 696f           <sectio
+000024c0: 6e0a 2020 2020 2020 2020 6964 3d5c 226c  n.        id=\"l
+000024d0: 6f67 696e 5c22 2063 6c61 7373 3d5c 226c  ogin\" class=\"l
+000024e0: 6f67 696e 2063 6f6e 7461 696e 6572 5c22  ogin container\"
+000024f0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+00002500: 2020 2020 205c 725c 6e5c 725c 6e5c 725c       \r\n\r\n\r\
+00002510: 6e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  n\r\n\r\n\r\n\r\
+00002520: 6e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  n\r\n\r\n\r\n\r\
+00002530: 6e5c 725c 6e5c 725c 6e5c 725c 6e3c 6469  n\r\n\r\n\r\n<di
+00002540: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
+00002550: 5c22 7461 622d 636f 6e74 656e 745c 223e  \"tab-content\">
+00002560: 5c72 5c6e 5c74 5c72 5c6e 5c74 5c74 5c72  \r\n\t\r\n\t\t\r
+00002570: 5c6e 5c74 5c74 5c72 5c6e 5c74 5c74 5c72  \n\t\t\r\n\t\t\r
+00002580: 5c6e 5c72 5c6e 5c74 5c74 5c72 5c6e 5c72  \n\r\n\t\t\r\n\r
+00002590: 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e 3c64  \n\r\n\r\n\r\n<d
+000025a0: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+000025b0: 3d5c 2274 6162 2d70 616e 6520 6163 7469  =\"tab-pane acti
+000025c0: 7665 5c22 2072 6f6c 653d 5c22 7461 6270  ve\" role=\"tabp
+000025d0: 616e 656c 5c22 2069 643d 5c22 6c6f 6769  anel\" id=\"logi
+000025e0: 6e2d 6765 6e65 7261 6c5c 223e 5c72 5c6e  n-general\">\r\n
+000025f0: 2020 2020 3c64 6976 0a20 2020 2020 2020      <div.       
+00002600: 2063 6c61 7373 3d5c 2272 6f77 5c22 3e5c   class=\"row\">\
+00002610: 725c 6e20 2020 2020 2020 205c 725c 6e20  r\n        \r\n 
+00002620: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
+00002630: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
+00002640: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00002650: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00002660: 2020 2020 2020 2020 5c72 5c6e 2020 2020          \r\n    
+00002670: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
+00002680: 3c64 6976 2063 6c61 7373 3d5c 2263 6f6c  <div class=\"col
+00002690: 2d73 6d2d 3620 636f 6c2d 6d64 2d36 206c  -sm-6 col-md-6 l
+000026a0: 6f67 696e 2d70 6167 652d 6d65 7373 6167  ogin-page-messag
+000026b0: 655c 223e 5c72 5c6e 0a20 2020 2020 2020  e\">\r\n.       
+000026c0: 205c 2020 2020 2020 2020 2020 203c 7020   \           <p 
+000026d0: 636c 6173 733d 5c22 6c65 6164 5c22 3e54  class=\"lead\">T
+000026e0: 6572 7665 7475 6c6f 6120 4f6d 616b 756b  ervetuloa Omakuk
+000026f0: 6b6f 6f6e 203c 6272 3e3c 7370 616e 2073  koon <br><span s
+00002700: 7479 6c65 3d5c 2266 6f6e 742d 7369 7a65  tyle=\"font-size
+00002710: 3a0a 2020 2020 2020 2020 302e 3865 6d5c  :.        0.8em\
+00002720: 223e 2623 3832 3132 204a 5c78 4534 7465  ">&#8212 J\xE4te
+00002730: 6b75 6b6f 6e20 735c 7845 3468 6b5c 7846  kukon s\xE4hk\xF
+00002740: 3669 7365 656e 2061 7369 6f69 6e74 6969  6iseen asiointii
+00002750: 6e3c 2f73 7061 6e3e 3c2f 703e 5c72 5c6e  n</span></p>\r\n
+00002760: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+00002770: 2020 2020 2020 2020 205c 725c 6e5c 725c           \r\n\r\
+00002780: 6e20 2020 2020 2020 2020 2020 205c 725c  n            \r\
+00002790: 6e20 2020 2020 2020 2020 2020 205c 725c  n            \r\
+000027a0: 6e20 2020 2020 2020 2020 2020 203c 6469  n            <di
+000027b0: 7620 636c 6173 733d 5c22 616c 6572 740a  v class=\"alert.
+000027c0: 2020 2020 2020 2020 616c 6572 742d 6461          alert-da
+000027d0: 6e67 6572 5c22 2064 6174 612d 726f 6c65  nger\" data-role
+000027e0: 3d5c 226c 6f67 696e 2d61 6c65 7274 5c22  =\"login-alert\"
+000027f0: 3e3c 2f64 6976 3e5c 725c 6e20 2020 2020  ></div>\r\n     
+00002800: 2020 2020 2020 203c 666f 726d 2069 643d         <form id=
+00002810: 5c22 6c6f 6769 6e2d 666f 726d 2d67 656e  \"login-form-gen
+00002820: 6572 616c 5c22 0a20 2020 2020 2020 2064  eral\".        d
+00002830: 6174 612d 726f 6c65 3d5c 226c 6f67 696e  ata-role=\"login
+00002840: 2d66 6f72 6d5c 2220 6d65 7468 6f64 3d5c  -form\" method=\
+00002850: 2250 4f53 545c 2220 6175 746f 636f 6d70  "POST\" autocomp
+00002860: 6c65 7465 3d5c 226f 6666 5c22 3e5c 725c  lete=\"off\">\r\
+00002870: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00002880: 203c 6469 760a 2020 2020 2020 2020 636c   <div.        cl
+00002890: 6173 733d 5c22 666f 726d 2d67 726f 7570  ass=\"form-group
+000028a0: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
+000028b0: 2020 2020 2020 2020 2020 203c 6c61 6265             <labe
+000028c0: 6c20 666f 723d 5c22 6a5f 7573 6572 6e61  l for=\"j_userna
+000028d0: 6d65 2d67 656e 6572 616c 5c22 3e5c 725c  me-general\">\r\
+000028e0: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002900: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
+00002910: 2020 2020 2020 2020 2020 3c2f 6c61 6265            </labe
+00002920: 6c3e 5c72 5c6e 5c72 5c6e 2020 2020 2020  l>\r\n\r\n      
+00002930: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+00002940: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00002950: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00002960: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00002970: 2020 2020 2020 203c 7370 616e 2063 6c61         <span cla
+00002980: 7373 3d5c 2267 6c79 7068 6963 6f6e 2067  ss=\"glyphicon g
+00002990: 6c79 7068 6963 6f6e 2d71 7565 7374 696f  lyphicon-questio
+000029a0: 6e2d 7369 676e 0a20 2020 2020 2020 2073  n-sign.        s
+000029b0: 6d61 6c6c 5c22 2064 6174 612d 746f 6767  mall\" data-togg
+000029c0: 6c65 3d5c 2270 6f70 6f76 6572 5c22 5c72  le=\"popover\"\r
+000029d0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+000029e0: 2020 2020 2020 2020 2020 7461 6269 6e64            tabind
+000029f0: 6578 3d5c 222d 315c 220a 2020 2020 2020  ex=\"-1\".      
+00002a00: 2020 6461 7461 2d70 6c61 6365 6d65 6e74    data-placement
+00002a10: 3d5c 2261 7574 6f20 7269 6768 745c 225c  =\"auto right\"\
+00002a20: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00002a30: 2020 2020 2020 2020 2020 2064 6174 612d             data-
+00002a40: 6f72 6967 696e 616c 2d74 6974 6c65 3d5c  original-title=\
+00002a50: 224b 5c78 4534 7974 745c 7845 346a 5c78  "K\xE4ytt\xE4j\x
+00002a60: 4534 7475 6e6e 756b 7365 6e61 0a20 2020  E4tunnuksena.   
+00002a70: 2020 2020 2074 6f69 6d69 6920 6173 6961       toimii asia
+00002a80: 6b61 736e 756d 6572 6f73 6920 2878 782d  kasnumerosi (xx-
+00002a90: 7878 7878 7878 782d 7878 292e 204a 6f73  xxxxxxx-xx). Jos
+00002aa0: 206f 6c65 7420 6973 5c78 4534 6e6e 5c78   olet is\xE4nn\x
+00002ab0: 4636 6974 7369 6a5c 7845 3420 7461 690a  F6itsij\xE4 tai.
+00002ac0: 2020 2020 2020 2020 7972 6974 7973 2c20          yritys, 
+00002ad0: 766f 6974 2073 6161 6461 204a 5c78 4534  voit saada J\xE4
+00002ae0: 7465 6b75 6b6f 6c74 6120 6572 696c 6c69  tekukolta erilli
+00002af0: 7365 6e20 7475 6e6e 756b 7365 6e2c 206a  sen tunnuksen, j
+00002b00: 6f6e 6b61 2061 7675 6c6c 6120 6e5c 7845  onka avulla n\xE
+00002b10: 3465 740a 2020 2020 2020 2020 6b61 696b  4et.        kaik
+00002b20: 6b69 656e 206b 6f68 7465 6964 6573 6920  kien kohteidesi 
+00002b30: 6a5c 7845 3474 6568 756f 6c6c 6f6e 2e5c  j\xE4tehuollon.\
+00002b40: 2220 6461 7461 2d74 7269 6767 6572 3d5c  " data-trigger=\
+00002b50: 2266 6f63 7573 5c22 3e3c 2f73 7061 6e3e  "focus\"></span>
+00002b60: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00002b70: 2020 2020 2020 2020 5c72 5c6e 5c72 5c6e          \r\n\r\n
+00002b80: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+00002b90: 2020 2020 2020 2020 2020 2020 203c 696e               <in
+00002ba0: 7075 7420 636c 6173 733d 5c22 666f 726d  put class=\"form
+00002bb0: 2d63 6f6e 7472 6f6c 5c22 2074 7970 653d  -control\" type=
+00002bc0: 5c22 7465 7874 5c22 2069 643d 5c22 6a5f  \"text\" id=\"j_
+00002bd0: 7573 6572 6e61 6d65 2d67 656e 6572 616c  username-general
+00002be0: 5c22 5c72 5c6e 0a20 2020 2020 2020 205c  \"\r\n.        \
+00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c00: 2020 2020 2020 206e 616d 653d 5c22 6a5f         name=\"j_
+00002c10: 7573 6572 6e61 6d65 5c22 2070 6c61 6365  username\" place
+00002c20: 686f 6c64 6572 3d5c 224b 5c78 4534 7974  holder=\"K\xE4yt
+00002c30: 745c 7845 346a 5c78 4534 7475 6e6e 7573  t\xE4j\xE4tunnus
+00002c40: 5c22 3e5c 725c 6e0a 2020 2020 2020 2020  \">\r\n.        
+00002c50: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+00002c60: 3c2f 6469 763e 5c72 5c6e 2020 2020 2020  </div>\r\n      
+00002c70: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00002c80: 6c61 7373 3d5c 2266 6f72 6d2d 6772 6f75  lass=\"form-grou
+00002c90: 705c 223e 5c72 5c6e 2020 2020 2020 2020  p\">\r\n        
+00002ca0: 2020 2020 2020 2020 2020 2020 3c6c 6162              <lab
+00002cb0: 656c 0a20 2020 2020 2020 2066 6f72 3d5c  el.        for=\
+00002cc0: 226a 5f70 6173 7377 6f72 642d 6765 6e65  "j_password-gene
+00002cd0: 7261 6c5c 223e 5c72 5c6e 2020 2020 2020  ral\">\r\n      
+00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cf0: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
+00002d00: 2020 2020 2020 2020 2020 3c2f 6c61 6265            </labe
+00002d10: 6c3e 5c72 5c6e 5c72 5c6e 0a20 2020 2020  l>\r\n\r\n.     
+00002d20: 2020 205c 2020 2020 2020 2020 2020 2020     \            
+00002d30: 2020 2020 2020 205c 725c 6e20 2020 2020         \r\n     
+00002d40: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00002d50: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00002d60: 2020 2020 2020 203c 7370 616e 0a20 2020         <span.   
+00002d70: 2020 2020 2063 6c61 7373 3d5c 2267 6c79       class=\"gly
+00002d80: 7068 6963 6f6e 2067 6c79 7068 6963 6f6e  phicon glyphicon
+00002d90: 2d71 7565 7374 696f 6e2d 7369 676e 2073  -question-sign s
+00002da0: 6d61 6c6c 5c22 2064 6174 612d 746f 6767  mall\" data-togg
+00002db0: 6c65 3d5c 2270 6f70 6f76 6572 5c22 5c72  le=\"popover\"\r
+00002dc0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002de0: 2020 2074 6162 696e 6465 783d 5c22 2d31     tabindex=\"-1
+00002df0: 5c22 2064 6174 612d 706c 6163 656d 656e  \" data-placemen
+00002e00: 743d 5c22 6175 746f 2072 6967 6874 5c22  t=\"auto right\"
+00002e10: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e30: 2020 2020 2064 6174 612d 6f72 6967 696e       data-origin
+00002e40: 616c 2d74 6974 6c65 3d5c 2245 6e73 696d  al-title=\"Ensim
+00002e50: 6d5c 7845 3469 7365 6c6c 5c78 4534 206b  m\xE4isell\xE4 k
+00002e60: 6972 6a61 7574 756d 6973 6b65 7272 616c  irjautumiskerral
+00002e70: 6c61 0a20 2020 2020 2020 2073 616c 6173  la.        salas
+00002e80: 616e 6120 6f6e 206c 6173 6b75 6e20 6e75  ana on laskun nu
+00002e90: 6d65 726f 2074 6169 206c 6173 6b75 7475  mero tai laskutu
+00002ea0: 736f 736f 6974 7465 6573 692e 2045 6e73  sosoitteesi. Ens
+00002eb0: 696d 6d5c 7845 3469 7365 6e20 6b69 726a  imm\xE4isen kirj
+00002ec0: 6175 7475 6d69 7365 6e0a 2020 2020 2020  autumisen.      
+00002ed0: 2020 6a5c 7845 346c 6b65 656e 2070 5c78    j\xE4lkeen p\x
+00002ee0: 4534 5c78 4534 7365 7420 6d75 7574 7461  E4\xE4set muutta
+00002ef0: 6d61 616e 2073 616c 6173 616e 6173 692e  maan salasanasi.
+00002f00: 5c22 2064 6174 612d 7472 6967 6765 723d  \" data-trigger=
+00002f10: 5c22 666f 6375 735c 223e 3c2f 7370 616e  \"focus\"></span
+00002f20: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
+00002f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f40: 2020 5c72 5c6e 5c72 5c6e 2020 2020 2020    \r\n\r\n      
+00002f50: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
+00002f60: 6e70 7574 2063 6c61 7373 3d5c 2266 6f72  nput class=\"for
+00002f70: 6d2d 636f 6e74 726f 6c5c 220a 2020 2020  m-control\".    
+00002f80: 2020 2020 7479 7065 3d5c 2270 6173 7377      type=\"passw
+00002f90: 6f72 645c 2220 6964 3d5c 226a 5f70 6173  ord\" id=\"j_pas
+00002fa0: 7377 6f72 642d 6765 6e65 7261 6c5c 225c  sword-general\"\
+00002fb0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00002fc0: 2020 2020 2020 2020 2020 6e61 6d65 3d5c            name=\
+00002fd0: 226a 5f70 6173 7377 6f72 645c 220a 2020  "j_password\".  
+00002fe0: 2020 2020 2020 6175 746f 636f 6d70 6c65        autocomple
+00002ff0: 7465 3d5c 226f 6666 5c22 5c72 5c6e 2020  te=\"off\"\r\n  
+00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003010: 2020 2020 2070 6c61 6365 686f 6c64 6572       placeholder
+00003020: 3d5c 2253 616c 6173 616e 615c 223e 5c72  =\"Salasana\">\r
+00003030: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00003040: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00003050: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00003060: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00003070: 733d 5c22 666f 726d 2d67 726f 7570 5c22  s=\"form-group\"
+00003080: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
+00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030a0: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
+000030b0: 653d 5c22 7061 7373 776f 7264 5c22 2069  e=\"password\" i
+000030c0: 643d 5c22 6870 2d67 656e 6572 616c 5c22  d=\"hp-general\"
+000030d0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030f0: 2020 2073 7479 6c65 3d5c 2264 6973 706c     style=\"displ
+00003100: 6179 3a6e 6f6e 655c 225c 725c 6e0a 2020  ay:none\"\r\n.  
+00003110: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003130: 2020 2020 2063 6c61 7373 3d5c 2266 6f72       class=\"for
+00003140: 6d2d 636f 6e74 726f 6c5c 225c 725c 6e20  m-control\"\r\n 
 00003150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003160: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
-00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031a0: 2020 2020 5c72 5c6e 0a20 2020 2020 2020      \r\n.       
-000031b0: 205c 2020 2020 2020 2020 2020 2020 2020   \              
-000031c0: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
-000031d0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-000031e0: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
-000031f0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00003200: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
-00003210: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003230: 2020 2020 2020 5c72 5c6e 5c72 5c6e 2020        \r\n\r\n  
+00003160: 2020 2020 2020 2020 2020 2020 2020 6175                au
+00003170: 746f 636f 6d70 6c65 7465 3d5c 226f 6666  tocomplete=\"off
+00003180: 5c22 0a20 2020 2020 2020 2076 616c 7565  \".        value
+00003190: 3d5c 2264 6f6e 6f74 7361 7665 5c22 202f  =\"donotsave\" /
+000031a0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+000031b0: 2020 2020 2020 2020 2020 2020 203c 696e               <in
+000031c0: 7075 7420 7479 7065 3d5c 2270 6173 7377  put type=\"passw
+000031d0: 6f72 645c 220a 2020 2020 2020 2020 6964  ord\".        id
+000031e0: 3d5c 2268 7032 2d67 656e 6572 616c 5c22  =\"hp2-general\"
+000031f0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003210: 2020 2073 7479 6c65 3d5c 2264 6973 706c     style=\"displ
+00003220: 6179 3a6e 6f6e 655c 225c 725c 6e0a 2020  ay:none\"\r\n.  
+00003230: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
 00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003250: 2020 2020 2020 2020 2020 5c72 5c6e 5c72            \r\n\r
-00003260: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00003250: 2020 2020 2063 6c61 7373 3d5c 2266 6f72       class=\"for
+00003260: 6d2d 636f 6e74 726f 6c5c 225c 725c 6e20  m-control\"\r\n 
 00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003280: 2020 5c72 5c6e 0a20 2020 2020 2020 205c    \r\n.        \
-00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032a0: 2020 2020 2020 2020 2020 2020 2020 205c                 \
-000032b0: 725c 6e5c 725c 6e20 2020 2020 2020 2020  r\n\r\n         
-000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032d0: 2020 2020 2020 2020 2020 205c 725c 6e5c             \r\n\
-000032e0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003310: 3c6c 6920 636c 6173 733d 5c22 6665 6564  <li class=\"feed
-00003320: 6261 636b 5c22 3e3c 615c 725c 6e20 2020  back\"><a\r\n   
-00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 2020 2020 2020 2020 2068 7265 663d 5c22           href=\"
-00003360: 2366 6565 6462 6163 6b5c 223e 5061 6c61  #feedback\">Pala
-00003370: 7574 653c 2f61 3e3c 2f6c 693e 5c72 5c6e  ute</a></li>\r\n
-00003380: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-00003390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033b0: 205c 725c 6e5c 725c 6e20 2020 2020 2020   \r\n\r\n       
-000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033d0: 2020 2020 2020 2020 205c 725c 6e0a 2020           \r\n.  
-000033e0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2020 5c72 5c6e 5c72 5c6e 2020 2020 2020    \r\n\r\n      
+00003280: 2020 2020 2020 2020 2020 2020 2020 6175                au
+00003290: 746f 636f 6d70 6c65 7465 3d5c 226f 6666  tocomplete=\"off
+000032a0: 5c22 0a20 2020 2020 2020 2076 616c 7565  \".        value
+000032b0: 3d5c 2264 6f6e 6f74 7361 7665 325c 2220  =\"donotsave2\" 
+000032c0: 2f3e 5c72 5c6e 2020 2020 2020 2020 2020  />\r\n          
+000032d0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+000032e0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+000032f0: 2020 2020 2020 2020 5c72 5c6e 0a20 2020          \r\n.   
+00003300: 2020 2020 205c 2020 2020 2020 2020 2020       \          
+00003310: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00003320: 6173 733d 5c22 6368 6563 6b62 6f78 5c22  ass=\"checkbox\"
+00003330: 2073 7479 6c65 3d5c 2264 6973 706c 6179   style=\"display
+00003340: 3a6e 6f6e 655c 223e 5c72 5c6e 2020 2020  :none\">\r\n    
+00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003360: 2020 2020 3c6c 6162 656c 3e5c 725c 6e0a      <label>\r\n.
+00003370: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003390: 2020 2020 3c69 6e70 7574 2074 7970 653d      <input type=
+000033a0: 5c22 6368 6563 6b62 6f78 5c22 2069 643d  \"checkbox\" id=
+000033b0: 5c22 7265 6d65 6d62 6572 2d6d 655c 2220  \"remember-me\" 
+000033c0: 6e61 6d65 3d5c 2272 656d 656d 6265 722d  name=\"remember-
+000033d0: 6d65 5c22 3e5c 725c 6e0a 2020 2020 2020  me\">\r\n.      
+000033e0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+000033f0: 2020 2020 2020 2020 2020 2020 2020 4d75                Mu
+00003400: 6973 7461 206d 696e 7574 5c72 5c6e 2020  ista minut\r\n  
 00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003420: 2020 2020 2020 2020 2020 5c72 5c6e 2020            \r\n  
-00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003440: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
-00003450: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 2020 2020 2020 205c 725c 6e5c 725c 6e20         \r\n\r\n 
-00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003490: 2020 2020 2020 2020 2020 2020 2020 205c                 \
-000034a0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00003420: 2020 2020 2020 3c2f 6c61 6265 6c3e 5c72        </label>\r
+00003430: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00003440: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00003450: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
+00003460: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
+00003470: 725c 6e5c 725c 6e20 2020 2020 2020 2020  r\n\r\n         
+00003480: 2020 2020 2020 203c 6469 760a 2020 2020         <div.    
+00003490: 2020 2020 636c 6173 733d 5c22 666f 726d      class=\"form
+000034a0: 2d67 726f 7570 5c22 3e5c 725c 6e20 2020  -group\">\r\n   
 000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034c0: 2020 205c 725c 6e0a 2020 2020 2020 2020     \r\n.        
-000034d0: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-000034e0: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
-000034f0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00003500: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 2020 2020 2020 3c6c 690a 2020 2020          <li.    
-00003530: 2020 2020 636c 6173 733d 5c22 6c6f 676f      class=\"logo
-00003540: 7574 5c22 3e3c 6120 6872 6566 3d5c 2223  ut\"><a href=\"#
-00003550: 6c6f 676f 7574 5c22 5c72 5c6e 2020 2020  logout\"\r\n    
+000034c0: 203c 6275 7474 6f6e 2074 7970 653d 5c22   <button type=\"
+000034d0: 6275 7474 6f6e 5c22 2064 6174 612d 6163  button\" data-ac
+000034e0: 7469 6f6e 3d5c 2266 6f72 676f 7474 656e  tion=\"forgotten
+000034f0: 2d70 6173 7377 6f72 645c 220a 2020 2020  -password\".    
+00003500: 2020 2020 636c 6173 733d 5c22 6274 6e20      class=\"btn 
+00003510: 6274 6e2d 6c69 6e6b 5c22 3e5c 725c 6e20  btn-link\">\r\n 
+00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003530: 2020 2020 2020 2054 696c 6161 2075 6e6f         Tilaa uno
+00003540: 6874 756e 7574 2073 616c 6173 616e 615c  htunut salasana\
+00003550: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
 00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003580: 2020 2020 2020 2020 2020 6f6e 636c 6963            onclic
-00003590: 6b3d 5c22 7769 6e64 6f77 2e6c 6f63 6174  k=\"window.locat
-000035a0: 696f 6e3d 6261 7365 7572 6c0a 2020 2020  ion=baseurl.    
-000035b0: 2020 2020 2b20 272f 6a5f 6163 6567 695f      + '/j_acegi_
-000035c0: 6c6f 676f 7574 5f65 6c63 7573 7472 6170  logout_elcustrap
-000035d0: 275c 223e 4b69 726a 6175 6475 2075 6c6f  '\">Kirjaudu ulo
-000035e0: 733c 2f61 3e3c 2f6c 693e 5c72 5c6e 2020  s</a></li>\r\n  
-000035f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003600: 2020 2020 2020 5c72 5c6e 0a20 2020 2020        \r\n.     
-00003610: 2020 205c 2020 2020 2020 2020 2020 2020     \            
-00003620: 2020 2020 2020 2020 2020 2020 2020 205c                 \
-00003630: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-00003640: 2020 2020 2020 2020 2020 2020 2020 205c                 \
-00003650: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00003570: 3c2f 6275 7474 6f6e 3e5c 725c 6e20 2020  </button>\r\n   
+00003580: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00003590: 6976 3e5c 725c 6e20 2020 2020 2020 2020  iv>\r\n         
+000035a0: 2020 2020 2020 203c 6469 760a 2020 2020         <div.    
+000035b0: 2020 2020 636c 6173 733d 5c22 666f 726d      class=\"form
+000035c0: 2d67 726f 7570 5c22 2069 643d 5c22 6c6f  -group\" id=\"lo
+000035d0: 6769 6e2d 6275 7474 6f6e 2d67 726f 7570  gin-button-group
+000035e0: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
+000035f0: 2020 2020 2020 2020 2020 203c 6275 7474             <butt
+00003600: 6f6e 0a20 2020 2020 2020 2074 7970 653d  on.        type=
+00003610: 5c22 7375 626d 6974 5c22 2063 6c61 7373  \"submit\" class
+00003620: 3d5c 2262 746e 2062 746e 2d70 7269 6d61  =\"btn btn-prima
+00003630: 7279 5c22 2069 643d 5c22 6c6f 6769 6e2d  ry\" id=\"login-
+00003640: 6275 7474 6f6e 2d67 656e 6572 616c 5c22  button-general\"
+00003650: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
 00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003670: 2020 205c 725c 6e0a 2020 2020 2020 2020     \r\n.        
-00003680: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-00003690: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
-000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036b0: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
-000036c0: 636c 6173 733d 5c22 6578 6974 7573 6572  class=\"exituser
-000036d0: 5c22 3e3c 610a 2020 2020 2020 2020 6872  \"><a.        hr
-000036e0: 6566 3d5c 2223 6578 6974 7573 6572 5c22  ef=\"#exituser\"
-000036f0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00003700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003720: 2020 2020 2020 2020 6f6e 636c 6963 6b3d          onclick=
-00003730: 5c22 7769 6e64 6f77 2e6c 6f63 6174 696f  \"window.locatio
-00003740: 6e3d 6261 7365 7572 6c0a 2020 2020 2020  n=baseurl.      
-00003750: 2020 2b20 272f 6a61 7465 6b75 6b6b 6f2f    + '/jatekukko/
-00003760: 6a5f 6163 6567 695f 6578 6974 5f75 7365  j_acegi_exit_use
-00003770: 723f 7265 6469 7265 6374 3d2f 7365 6375  r?redirect=/secu
-00003780: 7265 2f61 646d 696e 2f75 7365 7273 2e64  re/admin/users.d
-00003790: 6f27 5c22 3e4c 6f70 6574 610a 2020 2020  o'\">Lopeta.    
-000037a0: 2020 2020 7065 696c 6175 733c 2f61 3e3c      peilaus</a><
-000037b0: 2f6c 693e 5c72 5c6e 2020 2020 2020 2020  /li>\r\n        
-000037c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037d0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-000037e0: 2020 2020 2020 2020 3c2f 756c 3e5c 725c          </ul>\r\
-000037f0: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-00003800: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00003810: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
-00003820: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00003830: 7373 3d5c 2272 6f77 5c22 3e5c 725c 6e20  ss=\"row\">\r\n 
-00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003850: 2020 203c 6469 760a 2020 2020 2020 2020     <div.        
-00003860: 636c 6173 733d 5c22 636f 6c2d 6c67 2d6f  class=\"col-lg-o
-00003870: 6666 7365 742d 3220 636f 6c2d 6c67 2d38  ffset-2 col-lg-8
-00003880: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
-00003890: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000038a0: 6469 7620 6964 3d5c 2273 6572 7669 6365  div id=\"service
-000038b0: 2d73 656c 6563 746f 725c 220a 2020 2020  -selector\".    
-000038c0: 2020 2020 636c 6173 733d 5c22 7365 7276      class=\"serv
-000038d0: 6963 652d 7365 6c65 6374 6f72 5c22 2073  ice-selector\" s
-000038e0: 7479 6c65 3d5c 2264 6973 706c 6179 3a6e  tyle=\"display:n
-000038f0: 6f6e 655c 223e 3c2f 6469 763e 5c72 5c6e  one\"></div>\r\n
-00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003910: 2020 2020 3c2f 6469 763e 5c72 5c6e 0a20      </div>\r\n. 
-00003920: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-00003930: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
-00003940: 6e20 2020 2020 2020 2020 2020 203c 2f68  n            </h
-00003950: 6561 6465 723e 5c72 5c6e 5c72 5c6e 2020  eader>\r\n\r\n  
-00003960: 2020 2020 2020 2020 2020 3c73 6563 7469            <secti
-00003970: 6f6e 0a20 2020 2020 2020 2069 643d 5c22  on.        id=\"
-00003980: 6c6f 6769 6e5c 2220 636c 6173 733d 5c22  login\" class=\"
-00003990: 6c6f 6769 6e20 636f 6e74 6169 6e65 725c  login container\
-000039a0: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
-000039b0: 2020 2020 2020 5c72 5c6e 5c72 5c6e 5c72        \r\n\r\n\r
-000039c0: 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72  \n\r\n\r\n\r\n\r
-000039d0: 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72  \n\r\n\r\n\r\n\r
-000039e0: 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e 3c64  \n\r\n\r\n\r\n<d
-000039f0: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
-00003a00: 3d5c 2274 6162 2d63 6f6e 7465 6e74 5c22  =\"tab-content\"
-00003a10: 3e5c 725c 6e5c 745c 725c 6e5c 745c 745c  >\r\n\t\r\n\t\t\
-00003a20: 725c 6e5c 745c 745c 725c 6e5c 745c 745c  r\n\t\t\r\n\t\t\
-00003a30: 725c 6e5c 725c 6e5c 745c 745c 725c 6e5c  r\n\r\n\t\t\r\n\
-00003a40: 725c 6e5c 725c 6e5c 725c 6e5c 725c 6e3c  r\n\r\n\r\n\r\n<
-00003a50: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-00003a60: 733d 5c22 7461 622d 7061 6e65 2061 6374  s=\"tab-pane act
-00003a70: 6976 655c 2220 726f 6c65 3d5c 2274 6162  ive\" role=\"tab
-00003a80: 7061 6e65 6c5c 2220 6964 3d5c 226c 6f67  panel\" id=\"log
-00003a90: 696e 2d67 656e 6572 616c 5c22 3e5c 725c  in-general\">\r\
-00003aa0: 6e20 2020 203c 6469 760a 2020 2020 2020  n    <div.      
-00003ab0: 2020 636c 6173 733d 5c22 726f 775c 223e    class=\"row\">
-00003ac0: 5c72 5c6e 2020 2020 2020 2020 5c72 5c6e  \r\n        \r\n
-00003ad0: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
-00003ae0: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
-00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b00: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-00003b10: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
-00003b20: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
-00003b30: 203c 6469 7620 636c 6173 733d 5c22 636f   <div class=\"co
-00003b40: 6c2d 736d 2d36 2063 6f6c 2d6d 642d 3620  l-sm-6 col-md-6 
-00003b50: 6c6f 6769 6e2d 7061 6765 2d6d 6573 7361  login-page-messa
-00003b60: 6765 5c22 3e5c 725c 6e0a 2020 2020 2020  ge\">\r\n.      
-00003b70: 2020 5c20 2020 2020 2020 2020 2020 3c70    \           <p
-00003b80: 2063 6c61 7373 3d5c 226c 6561 645c 223e   class=\"lead\">
-00003b90: 5465 7276 6574 756c 6f61 204f 6d61 6b75  Tervetuloa Omaku
-00003ba0: 6b6b 6f6f 6e20 3c62 723e 3c73 7061 6e20  kkoon <br><span 
-00003bb0: 7374 796c 653d 5c22 666f 6e74 2d73 697a  style=\"font-siz
-00003bc0: 653a 0a20 2020 2020 2020 2030 2e38 656d  e:.        0.8em
-00003bd0: 5c22 3e26 2338 3231 3220 4a5c 7845 3474  \">&#8212 J\xE4t
-00003be0: 656b 756b 6f6e 2073 5c78 4534 686b 5c78  ekukon s\xE4hk\x
-00003bf0: 4636 6973 6565 6e20 6173 696f 696e 7469  F6iseen asiointi
-00003c00: 696e 3c2f 7370 616e 3e3c 2f70 3e5c 725c  in</span></p>\r\
-00003c10: 6e5c 725c 6e0a 2020 2020 2020 2020 5c20  n\r\n.        \ 
-00003c20: 2020 2020 2020 2020 2020 5c72 5c6e 5c72            \r\n\r
-00003c30: 5c6e 2020 2020 2020 2020 2020 2020 5c72  \n            \r
-00003c40: 5c6e 2020 2020 2020 2020 2020 2020 5c72  \n            \r
-00003c50: 5c6e 2020 2020 2020 2020 2020 2020 3c64  \n            <d
-00003c60: 6976 2063 6c61 7373 3d5c 2261 6c65 7274  iv class=\"alert
-00003c70: 0a20 2020 2020 2020 2061 6c65 7274 2d64  .        alert-d
-00003c80: 616e 6765 725c 2220 6461 7461 2d72 6f6c  anger\" data-rol
-00003c90: 653d 5c22 6c6f 6769 6e2d 616c 6572 745c  e=\"login-alert\
-00003ca0: 223e 3c2f 6469 763e 5c72 5c6e 2020 2020  "></div>\r\n    
-00003cb0: 2020 2020 2020 2020 3c66 6f72 6d20 6964          <form id
-00003cc0: 3d5c 226c 6f67 696e 2d66 6f72 6d2d 6765  =\"login-form-ge
-00003cd0: 6e65 7261 6c5c 220a 2020 2020 2020 2020  neral\".        
-00003ce0: 6461 7461 2d72 6f6c 653d 5c22 6c6f 6769  data-role=\"logi
-00003cf0: 6e2d 666f 726d 5c22 206d 6574 686f 643d  n-form\" method=
-00003d00: 5c22 504f 5354 5c22 2061 7574 6f63 6f6d  \"POST\" autocom
-00003d10: 706c 6574 653d 5c22 6f66 665c 223e 5c72  plete=\"off\">\r
-00003d20: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00003d30: 2020 3c64 6976 0a20 2020 2020 2020 2063    <div.        c
-00003d40: 6c61 7373 3d5c 2266 6f72 6d2d 6772 6f75  lass=\"form-grou
-00003d50: 705c 223e 5c72 5c6e 2020 2020 2020 2020  p\">\r\n        
-00003d60: 2020 2020 2020 2020 2020 2020 3c6c 6162              <lab
-00003d70: 656c 2066 6f72 3d5c 226a 5f75 7365 726e  el for=\"j_usern
-00003d80: 616d 652d 6765 6e65 7261 6c5c 223e 5c72  ame-general\">\r
-00003d90: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003db0: 2020 205c 725c 6e20 2020 2020 2020 2020     \r\n         
-00003dc0: 2020 2020 2020 2020 2020 203c 2f6c 6162             </lab
-00003dd0: 656c 3e5c 725c 6e5c 725c 6e20 2020 2020  el>\r\n\r\n     
-00003de0: 2020 2020 2020 2020 2020 2020 2020 205c                 \
-00003df0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e10: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00003e20: 2020 2020 2020 2020 3c73 7061 6e20 636c          <span cl
-00003e30: 6173 733d 5c22 676c 7970 6869 636f 6e20  ass=\"glyphicon 
-00003e40: 676c 7970 6869 636f 6e2d 7175 6573 7469  glyphicon-questi
-00003e50: 6f6e 2d73 6967 6e0a 2020 2020 2020 2020  on-sign.        
-00003e60: 736d 616c 6c5c 2220 6461 7461 2d74 6f67  small\" data-tog
-00003e70: 676c 653d 5c22 706f 706f 7665 725c 225c  gle=\"popover\"\
-00003e80: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-00003e90: 2020 2020 2020 2020 2020 2074 6162 696e             tabin
-00003ea0: 6465 783d 5c22 2d31 5c22 0a20 2020 2020  dex=\"-1\".     
-00003eb0: 2020 2064 6174 612d 706c 6163 656d 656e     data-placemen
-00003ec0: 743d 5c22 6175 746f 2072 6967 6874 5c22  t=\"auto right\"
-00003ed0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00003ee0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00003ef0: 2d6f 7269 6769 6e61 6c2d 7469 746c 653d  -original-title=
-00003f00: 5c22 4b5c 7845 3479 7474 5c78 4534 6a5c  \"K\xE4ytt\xE4j\
-00003f10: 7845 3474 756e 6e75 6b73 656e 610a 2020  xE4tunnuksena.  
-00003f20: 2020 2020 2020 746f 696d 6969 2061 7369        toimii asi
-00003f30: 616b 6173 6e75 6d65 726f 7369 2028 7878  akasnumerosi (xx
-00003f40: 2d78 7878 7878 7878 2d78 7829 2e20 4a6f  -xxxxxxx-xx). Jo
-00003f50: 7320 6f6c 6574 2069 735c 7845 346e 6e5c  s olet is\xE4nn\
-00003f60: 7846 3669 7473 696a 5c78 4534 2074 6169  xF6itsij\xE4 tai
-00003f70: 0a20 2020 2020 2020 2079 7269 7479 732c  .        yritys,
-00003f80: 2076 6f69 7420 7361 6164 6120 4a5c 7845   voit saada J\xE
-00003f90: 3474 656b 756b 6f6c 7461 2065 7269 6c6c  4tekukolta erill
-00003fa0: 6973 656e 2074 756e 6e75 6b73 656e 2c20  isen tunnuksen, 
-00003fb0: 6a6f 6e6b 6120 6176 756c 6c61 206e 5c78  jonka avulla n\x
-00003fc0: 4534 6574 0a20 2020 2020 2020 206b 6169  E4et.        kai
-00003fd0: 6b6b 6965 6e20 6b6f 6874 6569 6465 7369  kkien kohteidesi
-00003fe0: 206a 5c78 4534 7465 6875 6f6c 6c6f 6e2e   j\xE4tehuollon.
-00003ff0: 5c22 2064 6174 612d 7472 6967 6765 723d  \" data-trigger=
-00004000: 5c22 666f 6375 735c 223e 3c2f 7370 616e  \"focus\"></span
-00004010: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-00004020: 2020 2020 2020 2020 205c 725c 6e5c 725c           \r\n\r\
-00004030: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-00004040: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00004050: 6e70 7574 2063 6c61 7373 3d5c 2266 6f72  nput class=\"for
-00004060: 6d2d 636f 6e74 726f 6c5c 2220 7479 7065  m-control\" type
-00004070: 3d5c 2274 6578 745c 2220 6964 3d5c 226a  =\"text\" id=\"j
-00004080: 5f75 7365 726e 616d 652d 6765 6e65 7261  _username-genera
-00004090: 6c5c 225c 725c 6e0a 2020 2020 2020 2020  l\"\r\n.        
-000040a0: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-000040b0: 2020 2020 2020 2020 6e61 6d65 3d5c 226a          name=\"j
-000040c0: 5f75 7365 726e 616d 655c 2220 706c 6163  _username\" plac
-000040d0: 6568 6f6c 6465 723d 5c22 4b5c 7845 3479  eholder=\"K\xE4y
-000040e0: 7474 5c78 4534 6a5c 7845 3474 756e 6e75  tt\xE4j\xE4tunnu
-000040f0: 735c 223e 5c72 5c6e 0a20 2020 2020 2020  s\">\r\n.       
-00004100: 205c 2020 2020 2020 2020 2020 2020 2020   \              
-00004110: 203c 2f64 6976 3e5c 725c 6e20 2020 2020   </div>\r\n     
-00004120: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00004130: 636c 6173 733d 5c22 666f 726d 2d67 726f  class=\"form-gro
-00004140: 7570 5c22 3e5c 725c 6e20 2020 2020 2020  up\">\r\n       
-00004150: 2020 2020 2020 2020 2020 2020 203c 6c61               <la
-00004160: 6265 6c0a 2020 2020 2020 2020 666f 723d  bel.        for=
-00004170: 5c22 6a5f 7061 7373 776f 7264 2d67 656e  \"j_password-gen
-00004180: 6572 616c 5c22 3e5c 725c 6e20 2020 2020  eral\">\r\n     
-00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041a0: 2020 205c 725c 6e20 2020 2020 2020 2020     \r\n         
-000041b0: 2020 2020 2020 2020 2020 203c 2f6c 6162             </lab
-000041c0: 656c 3e5c 725c 6e5c 725c 6e0a 2020 2020  el>\r\n\r\n.    
-000041d0: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-000041e0: 2020 2020 2020 2020 5c72 5c6e 2020 2020          \r\n    
-000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004200: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00004210: 2020 2020 2020 2020 3c73 7061 6e0a 2020          <span.  
-00004220: 2020 2020 2020 636c 6173 733d 5c22 676c        class=\"gl
-00004230: 7970 6869 636f 6e20 676c 7970 6869 636f  yphicon glyphico
-00004240: 6e2d 7175 6573 7469 6f6e 2d73 6967 6e20  n-question-sign 
-00004250: 736d 616c 6c5c 2220 6461 7461 2d74 6f67  small\" data-tog
-00004260: 676c 653d 5c22 706f 706f 7665 725c 225c  gle=\"popover\"\
-00004270: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-00004280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004290: 2020 2020 7461 6269 6e64 6578 3d5c 222d      tabindex=\"-
-000042a0: 315c 2220 6461 7461 2d70 6c61 6365 6d65  1\" data-placeme
-000042b0: 6e74 3d5c 2261 7574 6f20 7269 6768 745c  nt=\"auto right\
-000042c0: 225c 725c 6e0a 2020 2020 2020 2020 5c20  "\r\n.        \ 
-000042d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042e0: 2020 2020 2020 6461 7461 2d6f 7269 6769        data-origi
-000042f0: 6e61 6c2d 7469 746c 653d 5c22 456e 7369  nal-title=\"Ensi
-00004300: 6d6d 5c78 4534 6973 656c 6c5c 7845 3420  mm\xE4isell\xE4 
-00004310: 6b69 726a 6175 7475 6d69 736b 6572 7261  kirjautumiskerra
-00004320: 6c6c 610a 2020 2020 2020 2020 7361 6c61  lla.        sala
-00004330: 7361 6e61 206f 6e20 6c61 736b 756e 206e  sana on laskun n
-00004340: 756d 6572 6f20 7461 6920 6c61 736b 7574  umero tai laskut
-00004350: 7573 6f73 6f69 7474 6565 7369 2e20 456e  usosoitteesi. En
-00004360: 7369 6d6d 5c78 4534 6973 656e 206b 6972  simm\xE4isen kir
-00004370: 6a61 7574 756d 6973 656e 0a20 2020 2020  jautumisen.     
-00004380: 2020 206a 5c78 4534 6c6b 6565 6e20 705c     j\xE4lkeen p\
-00004390: 7845 345c 7845 3473 6574 206d 7575 7474  xE4\xE4set muutt
-000043a0: 616d 6161 6e20 7361 6c61 7361 6e61 7369  amaan salasanasi
-000043b0: 2e5c 2220 6461 7461 2d74 7269 6767 6572  .\" data-trigger
-000043c0: 3d5c 2266 6f63 7573 5c22 3e3c 2f73 7061  =\"focus\"></spa
-000043d0: 6e3e 5c72 5c6e 0a20 2020 2020 2020 205c  n>\r\n.        \
-000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043f0: 2020 205c 725c 6e5c 725c 6e20 2020 2020     \r\n\r\n     
-00004400: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00004410: 696e 7075 7420 636c 6173 733d 5c22 666f  input class=\"fo
-00004420: 726d 2d63 6f6e 7472 6f6c 5c22 0a20 2020  rm-control\".   
-00004430: 2020 2020 2074 7970 653d 5c22 7061 7373       type=\"pass
-00004440: 776f 7264 5c22 2069 643d 5c22 6a5f 7061  word\" id=\"j_pa
-00004450: 7373 776f 7264 2d67 656e 6572 616c 5c22  ssword-general\"
-00004460: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00004470: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-00004480: 5c22 6a5f 7061 7373 776f 7264 5c22 0a20  \"j_password\". 
-00004490: 2020 2020 2020 2061 7574 6f63 6f6d 706c         autocompl
-000044a0: 6574 653d 5c22 6f66 665c 225c 725c 6e20  ete=\"off\"\r\n 
-000044b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044c0: 2020 2020 2020 706c 6163 6568 6f6c 6465        placeholde
-000044d0: 723d 5c22 5361 6c61 7361 6e61 5c22 3e5c  r=\"Salasana\">\
-000044e0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004500: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00004510: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00004520: 7373 3d5c 2266 6f72 6d2d 6772 6f75 705c  ss=\"form-group\
-00004530: 223e 5c72 5c6e 0a20 2020 2020 2020 205c  ">\r\n.        \
+00003670: 2020 2020 2020 4b69 726a 6175 6475 5c72        Kirjaudu\r
+00003680: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00003690: 2020 2020 2020 3c2f 6275 7474 6f6e 3e5c        </button>\
+000036a0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+000036b0: 2020 2020 2020 205c 725c 6e0a 2020 2020         \r\n.    
+000036c0: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
+000036d0: 2020 2020 2020 2020 3c62 7574 746f 6e20          <button 
+000036e0: 7479 7065 3d5c 2262 7574 746f 6e5c 2220  type=\"button\" 
+000036f0: 6461 7461 2d61 6374 696f 6e3d 5c22 7172  data-action=\"qr
+00003700: 2d72 6561 6465 725c 2220 636c 6173 733d  -reader\" class=
+00003710: 5c22 6274 6e0a 2020 2020 2020 2020 6274  \"btn.        bt
+00003720: 6e2d 7072 696d 6172 795c 223e 5c72 5c6e  n-primary\">\r\n
+00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003740: 2020 2020 2020 2020 4c75 6520 5152 2d6b          Lue QR-k
+00003750: 6f6f 6469 5c72 5c6e 2020 2020 2020 2020  oodi\r\n        
+00003760: 2020 2020 2020 2020 2020 2020 3c2f 6275              </bu
+00003770: 7474 6f6e 3e5c 725c 6e0a 2020 2020 2020  tton>\r\n.      
+00003780: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+00003790: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
+000037a0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+000037b0: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
+000037c0: 2020 2020 2020 2020 5c72 5c6e 5c72 5c6e          \r\n\r\n
+000037d0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+000037e0: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
+000037f0: 2020 2020 2020 2020 203c 2f66 6f72 6d3e           </form>
+00003800: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
+00003810: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
+00003820: 2020 2020 2020 2020 3c21 2d2d 0a20 2020          <!--.   
+00003830: 2020 2020 2041 6c65 7274 206d 7573 7420       Alert must 
+00003840: 6e6f 7420 636f 6e74 6169 6e20 616e 7920  not contain any 
+00003850: 6578 7472 6120 6368 6172 6163 7465 7273  extra characters
+00003860: 2c20 6576 656e 2077 6869 7465 7370 6163  , even whitespac
+00003870: 652c 2066 6f72 2068 6964 696e 6720 746f  e, for hiding to
+00003880: 0a20 2020 2020 2020 2077 6f72 6b20 7072  .        work pr
+00003890: 6f70 6572 6c79 2e20 2d2d 3e5c 725c 6e20  operly. -->\r\n 
+000038a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000038b0: 6272 3e5c 725c 6e20 2020 2020 2020 2020  br>\r\n         
+000038c0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+000038d0: 733d 5c22 6572 726f 722d 6275 6c6c 6574  s=\"error-bullet
+000038e0: 696e 0a20 2020 2020 2020 2061 6c65 7274  in.        alert
+000038f0: 2061 6c65 7274 2d69 6e66 6f5c 223e 3c2f   alert-info\"></
+00003900: 6469 763e 5c72 5c6e 2020 2020 2020 2020  div>\r\n        
+00003910: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
+00003920: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
+00003930: 2020 2020 5c72 5c6e 0a20 2020 2020 2020      \r\n.       
+00003940: 205c 2020 2020 2020 203c 2f64 6976 3e5c   \       </div>\
+00003950: 725c 6e5c 725c 6e20 2020 2020 2020 205c  r\n\r\n        \
+00003960: 725c 6e20 2020 2020 2020 203c 6469 7620  r\n        <div 
+00003970: 636c 6173 733d 5c22 636f 6c2d 736d 2d36  class=\"col-sm-6
+00003980: 2063 6f6c 2d6d 642d 365c 223e 5c72 5c6e   col-md-6\">\r\n
+00003990: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+000039a0: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
+000039b0: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
+000039c0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+000039d0: 5c22 726f 7720 6c6f 6769 6e2d 7061 6765  \"row login-page
+000039e0: 2d61 6374 696f 6e73 5c22 3e5c 725c 6e0a  -actions\">\r\n.
+000039f0: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+00003a00: 2020 2020 2020 2020 5c72 5c6e 5c72 5c6e          \r\n\r\n
+00003a10: 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e  \r\n\r\n\r\n\r\n
+00003a20: 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c74 3c64  \r\n\r\n\r\n\t<d
+00003a30: 6976 2063 6c61 7373 3d5c 2272 6f77 5c22  iv class=\"row\"
+00003a40: 3e5c 725c 6e5c 745c 745c 725c 6e5c 745c  >\r\n\t\t\r\n\t\
+00003a50: 745c 725c 6e5c 745c 745c 745c 725c 6e5c  t\r\n\t\t\t\r\n\
+00003a60: 745c 745c 725c 6e5c 745c 743c 6275 7474  t\t\r\n\t\t<butt
+00003a70: 6f6e 0a20 2020 2020 2020 2074 7970 653d  on.        type=
+00003a80: 5c22 6275 7474 6f6e 5c22 2063 6c61 7373  \"button\" class
+00003a90: 3d5c 2262 746e 2062 746e 2d70 7269 6d61  =\"btn btn-prima
+00003aa0: 7279 2062 746e 2d62 6c6f 636b 206c 6f6e  ry btn-block lon
+00003ab0: 672d 7465 7874 2d62 7574 746f 6e5c 2220  g-text-button\" 
+00003ac0: 6461 7461 2d61 6374 696f 6e3d 5c22 6a6f  data-action=\"jo
+00003ad0: 696e 2d77 6173 7465 2d63 6f6c 6c65 6374  in-waste-collect
+00003ae0: 696f 6e5c 223e 5c72 5c6e 5c74 5c74 5c74  ion\">\r\n\t\t\t
+00003af0: 4c69 6974 790a 2020 2020 2020 2020 6a5c  Liity.        j\
+00003b00: 7845 3474 6568 756f 6c74 6f6f 6e5c 725c  xE4tehuoltoon\r\
+00003b10: 6e5c 745c 743c 2f62 7574 746f 6e3e 5c72  n\t\t</button>\r
+00003b20: 5c6e 5c74 5c74 5c72 5c6e 5c74 3c2f 6469  \n\t\t\r\n\t</di
+00003b30: 763e 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72  v>\r\n\r\n\r\n\r
+00003b40: 5c6e 5c74 3c64 6976 0a20 2020 2020 2020  \n\t<div.       
+00003b50: 2063 6c61 7373 3d5c 2272 6f77 5c22 3e5c   class=\"row\">\
+00003b60: 725c 6e5c 745c 743c 6834 3e3c 2f68 343e  r\n\t\t<h4></h4>
+00003b70: 5c72 5c6e 5c74 5c74 5c72 5c6e 5c74 5c74  \r\n\t\t\r\n\t\t
+00003b80: 5c74 5c72 5c6e 5c74 5c74 5c72 5c6e 5c74  \t\r\n\t\t\r\n\t
+00003b90: 5c74 3c62 7574 746f 6e20 7479 7065 3d5c  \t<button type=\
+00003ba0: 2262 7574 746f 6e5c 220a 2020 2020 2020  "button\".      
+00003bb0: 2020 636c 6173 733d 5c22 6274 6e20 6274    class=\"btn bt
+00003bc0: 6e2d 7072 696d 6172 7920 6274 6e2d 626c  n-primary btn-bl
+00003bd0: 6f63 6b20 6c6f 6e67 2d74 6578 742d 6275  ock long-text-bu
+00003be0: 7474 6f6e 5c22 2064 6174 612d 6163 7469  tton\" data-acti
+00003bf0: 6f6e 3d5c 226d 616b 652d 636f 6d70 6f73  on=\"make-compos
+00003c00: 742d 6e6f 7469 6365 5c22 3e5c 725c 6e5c  t-notice\">\r\n\
+00003c10: 745c 745c 7454 5c78 4534 7974 5c78 4534  t\t\tT\xE4yt\xE4
+00003c20: 0a20 2020 2020 2020 206b 6f6d 706f 7374  .        kompost
+00003c30: 6f69 6e74 692d 696c 6d6f 6974 7573 5c72  ointi-ilmoitus\r
+00003c40: 5c6e 5c74 5c74 3c2f 6275 7474 6f6e 3e5c  \n\t\t</button>\
+00003c50: 725c 6e5c 745c 745c 725c 6e5c 743c 2f64  r\n\t\t\r\n\t</d
+00003c60: 6976 3e5c 725c 6e5c 725c 6e5c 725c 6e5c  iv>\r\n\r\n\r\n\
+00003c70: 725c 6e5c 725c 6e5c 745c 725c 6e5c 745c  r\n\r\n\t\r\n\t\
+00003c80: 725c 6e5c 745c 725c 6e5c 745c 725c 6e5c  r\n\t\r\n\t\r\n\
+00003c90: 745c 725c 6e5c 725c 6e5c 745c 725c 6e5c  t\r\n\r\n\t\r\n\
+00003ca0: 725c 6e5c 745c 725c 6e5c 745c 725c 6e5c  r\n\t\r\n\t\r\n\
+00003cb0: 725c 6e5c 745c 725c 6e5c 745c 725c 6e5c  r\n\t\r\n\t\r\n\
+00003cc0: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
+00003cd0: 6173 733d 5c22 726f 775c 223e 5c72 5c6e  ass=\"row\">\r\n
+00003ce0: 5c74 5c74 3c68 343e 3c2f 6834 3e5c 725c  \t\t<h4></h4>\r\
+00003cf0: 6e5c 745c 745c 725c 6e5c 745c 745c 745c  n\t\t\r\n\t\t\t\
+00003d00: 725c 6e5c 745c 745c 725c 6e5c 745c 743c  r\n\t\t\r\n\t\t<
+00003d10: 6275 7474 6f6e 2074 7970 653d 5c22 6275  button type=\"bu
+00003d20: 7474 6f6e 5c22 0a20 2020 2020 2020 2063  tton\".        c
+00003d30: 6c61 7373 3d5c 2262 746e 2062 746e 2d70  lass=\"btn btn-p
+00003d40: 7269 6d61 7279 2062 746e 2d62 6c6f 636b  rimary btn-block
+00003d50: 206c 6f6e 672d 7465 7874 2d62 7574 746f   long-text-butto
+00003d60: 6e5c 2220 6461 7461 2d61 6374 696f 6e3d  n\" data-action=
+00003d70: 5c22 6769 7665 2d66 6565 6462 6163 6b5c  \"give-feedback\
+00003d80: 220a 2020 2020 2020 2020 6461 7461 2d66  ".        data-f
+00003d90: 6565 6462 6163 6b2d 7769 6e64 6f77 2d69  eedback-window-i
+00003da0: 643d 5c22 305c 223e 5c72 5c6e 5c74 5c74  d=\"0\">\r\n\t\t
+00003db0: 5c74 416e 6e61 2070 616c 6175 7465 7474  \tAnna palautett
+00003dc0: 615c 725c 6e5c 745c 743c 2f62 7574 746f  a\r\n\t\t</butto
+00003dd0: 6e3e 5c72 5c6e 5c74 5c74 5c72 5c6e 5c74  n>\r\n\t\t\r\n\t
+00003de0: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 5c74  </div>\r\n\r\n\t
+00003df0: 5c72 5c6e 5c72 5c6e 5c74 5c72 5c6e 5c72  \r\n\r\n\t\r\n\r
+00003e00: 5c6e 5c74 5c72 5c6e 5c72 5c6e 5c74 5c72  \n\t\r\n\r\n\t\r
+00003e10: 5c6e 5c74 5c72 5c6e 5c72 5c6e 5c74 5c72  \n\t\r\n\r\n\t\r
+00003e20: 5c6e 5c72 5c6e 5c74 5c72 5c6e 5c74 5c72  \n\r\n\t\r\n\t\r
+00003e30: 5c6e 5c72 5c6e 5c74 5c72 5c6e 5c72 5c6e  \n\r\n\t\r\n\r\n
+00003e40: 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e  \r\n\r\n\r\n\r\n
+00003e50: 5c72 5c6e 5c72 5c6e 5c72 5c6e 0a20 2020  \r\n\r\n\r\n.   
+00003e60: 2020 2020 205c 2020 2020 2020 2020 2020       \          
+00003e70: 203c 2f64 6976 3e5c 725c 6e20 2020 2020   </div>\r\n     
+00003e80: 2020 2020 2020 205c 725c 6e20 2020 2020         \r\n     
+00003e90: 2020 203c 2f64 6976 3e5c 725c 6e20 2020     </div>\r\n   
+00003ea0: 205c 725c 6e5c 725c 6e20 2020 203c 2f64   \r\n\r\n    </d
+00003eb0: 6976 3e5c 725c 6e0a 2020 2020 2020 2020  iv>\r\n.        
+00003ec0: 5c20 2020 5c72 5c6e 2020 2020 3c64 6976  \   \r\n    <div
+00003ed0: 2069 643d 5c22 6c6f 6769 6e2d 666f 6f74   id=\"login-foot
+00003ee0: 6572 5c22 2063 6c61 7373 3d5c 2272 6f77  er\" class=\"row
+00003ef0: 5c22 3e5c 725c 6e20 2020 2020 2020 203c  \">\r\n        <
+00003f00: 6469 7620 636c 6173 733d 5c22 636f 6e74  div class=\"cont
+00003f10: 6163 742d 696e 666f 5c22 3e5c 725c 6e0a  act-info\">\r\n.
+00003f20: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+00003f30: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
+00003f40: 2263 6f6c 2d73 6d2d 3620 636f 6c2d 6d64  "col-sm-6 col-md
+00003f50: 2d36 5c22 3e5c 725c 6e20 2020 2020 2020  -6\">\r\n       
+00003f60: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00003f70: 6173 733d 5c22 6c6f 6769 6e2d 666f 6f74  ass=\"login-foot
+00003f80: 6572 2d74 6578 745c 223e 5c72 5c6e 0a20  er-text\">\r\n. 
+00003f90: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+00003fa0: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
+00003fb0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00003fc0: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
+00003fd0: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
+00003fe0: 2020 2020 2020 2020 2020 203c 6469 760a             <div.
+00003ff0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+00004000: 636f 6c2d 736d 2d36 2063 6f6c 2d6d 642d  col-sm-6 col-md-
+00004010: 365c 223e 5c72 5c6e 2020 2020 2020 2020  6\">\r\n        
+00004020: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
+00004030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004040: 205c 725c 6e0a 2020 2020 2020 2020 5c20   \r\n.        \ 
+00004050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004060: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
+00004070: 2020 2020 2020 2020 2020 5c72 5c6e 2020            \r\n  
+00004080: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+00004090: 5c6e 2020 2020 2020 2020 2020 2020 203c  \n             <
+000040a0: 2f64 6976 3e5c 725c 6e0a 2020 2020 2020  /div>\r\n.      
+000040b0: 2020 5c20 2020 2020 2020 3c2f 6469 763e    \       </div>
+000040c0: 5c72 5c6e 2020 2020 3c2f 6469 763e 5c72  \r\n    </div>\r
+000040d0: 5c6e 3c2f 6469 763e 5c72 5c6e 5c74 5c72  \n</div>\r\n\t\r
+000040e0: 5c6e 3c2f 6469 763e 5c72 5c6e 5c72 5c6e  \n</div>\r\n\r\n
+000040f0: 5c72 5c6e 5c72 5c6e 5c72 5c6e 0a20 2020  \r\n\r\n\r\n.   
+00004100: 2020 2020 205c 2020 2020 2020 2020 2020       \          
+00004110: 203c 2f73 6563 7469 6f6e 3e5c 725c 6e5c   </section>\r\n\
+00004120: 725c 6e20 2020 2020 2020 2020 2020 203c  r\n            <
+00004130: 7365 6374 696f 6e20 6964 3d5c 2273 6572  section id=\"ser
+00004140: 7669 6365 2d6c 6973 745c 2220 636c 6173  vice-list\" clas
+00004150: 733d 5c22 7365 7276 6963 6573 0a20 2020  s=\"services.   
+00004160: 2020 2020 2063 6f6e 7461 696e 6572 5c22       container\"
+00004170: 2073 7479 6c65 3d5c 2264 6973 706c 6179   style=\"display
+00004180: 3a6e 6f6e 655c 223e 5c72 5c6e 2020 2020  :none\">\r\n    
+00004190: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+000041a0: 2063 6c61 7373 3d5c 2265 6d70 7479 2d70   class=\"empty-p
+000041b0: 6167 655c 223e 5c72 5c6e 0a20 2020 2020  age\">\r\n.     
+000041c0: 2020 205c 2020 2020 2020 2020 2020 2020     \            
+000041d0: 2020 2020 2020 203c 7020 636c 6173 733d         <p class=
+000041e0: 5c22 6c65 6164 2074 6578 742d 6365 6e74  \"lead text-cent
+000041f0: 6572 5c22 3e56 616c 6974 7365 206b 6f68  er\">Valitse koh
+00004200: 6465 206f 696b 6561 6e20 796c 5c78 4534  de oikean yl\xE4
+00004210: 6b75 6c6d 616e 0a20 2020 2020 2020 2076  kulman.        v
+00004220: 616c 696b 6f73 7461 2e3c 2f70 3e5c 725c  alikosta.</p>\r\
+00004230: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00004240: 203c 2f64 6976 3e5c 725c 6e5c 725c 6e20   </div>\r\n\r\n 
+00004250: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00004260: 6469 7620 636c 6173 733d 5c22 636f 6e74  div class=\"cont
+00004270: 656e 740a 2020 2020 2020 2020 726f 775c  ent.        row\
+00004280: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
+00004290: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+000042a0: 6c61 7373 3d5c 2263 6f6c 2d6c 672d 3130  lass=\"col-lg-10
+000042b0: 2063 6f6c 2d6c 672d 6f66 6673 6574 2d31   col-lg-offset-1
+000042c0: 5c22 3e5c 725c 6e0a 2020 2020 2020 2020  \">\r\n.        
+000042d0: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+000042e0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000042f0: 7373 3d5c 2264 6f2d 6e6f 742d 7368 6f77  ss=\"do-not-show
+00004300: 5c22 2069 643d 5c22 646f 2d6e 6f74 2d73  \" id=\"do-not-s
+00004310: 686f 775c 223e 4875 6f6d 6173 6974 6861  how\">Huomasitha
+00004320: 6e2c 0a20 2020 2020 2020 2065 7474 5c78  n,.        ett\x
+00004330: 4534 205c 2254 696c 6161 2079 6c69 6d5c  E4 \"Tilaa ylim\
+00004340: 7845 345c 7845 3472 5c78 4534 696e 656e  xE4\xE4r\xE4inen
+00004350: 2074 7968 6a65 6e6e 7973 5c22 202d 746f   tyhjennys\" -to
+00004360: 696d 696e 746f 206c 5c78 4636 7974 7979  iminto l\xF6ytyy
+00004370: 206e 796b 7969 7369 6e0a 2020 2020 2020   nykyisin.      
+00004380: 2020 5c22 5465 6520 6d75 7574 6f6b 7369    \"Tee muutoksi
+00004390: 6120 7061 6c76 656c 7575 6e5c 222d 7061  a palveluun\"-pa
+000043a0: 696e 696b 6b65 656e 2061 6c74 612e 203c  inikkeen alta. <
+000043b0: 6120 6872 6566 3d5c 2223 5c22 2064 6174  a href=\"#\" dat
+000043c0: 612d 6163 7469 6f6e 3d5c 2263 6f6d 706f  a-action=\"compo
+000043d0: 7374 2d6e 6f74 6963 655c 223e 4b6f 6d70  st-notice\">Komp
+000043e0: 6f73 746f 696e 7469 2d69 6c6d 6f69 7475  ostointi-ilmoitu
+000043f0: 6b73 6565 6e0a 2020 2020 2020 2020 705c  kseen.        p\
+00004400: 7845 345c 7845 3473 6574 2074 5c78 4534  xE4\xE4set t\xE4
+00004410: 7374 5c78 4534 3c2f 613e 2e3c 2f64 6976  st\xE4</a>.</div
+00004420: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+00004430: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
+00004440: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00004450: 2020 2020 2020 2020 203c 6469 760a 2020           <div.  
+00004460: 2020 2020 2020 636c 6173 733d 5c22 7365        class=\"se
+00004470: 7276 6963 6573 5c22 3e5c 725c 6e20 2020  rvices\">\r\n   
+00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004490: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
+000044a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044b0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+000044c0: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
+000044d0: 5c22 666f 726d 2d62 7574 746f 6e73 2074  \"form-buttons t
+000044e0: 6578 742d 6365 6e74 6572 2061 6374 696f  ext-center actio
+000044f0: 6e2d 6275 7474 6f6e 732d 626c 6f63 6b5c  n-buttons-block\
+00004500: 2220 6461 7461 2d72 6f6c 653d 5c22 6163  " data-role=\"ac
+00004510: 7469 6f6e 2d62 7574 746f 6e73 5c22 3e5c  tion-buttons\">\
+00004520: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00004530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004550: 2020 2020 2020 203c 696e 7075 7420 7479         <input ty
-00004560: 7065 3d5c 2270 6173 7377 6f72 645c 2220  pe=\"password\" 
-00004570: 6964 3d5c 2268 702d 6765 6e65 7261 6c5c  id=\"hp-general\
-00004580: 225c 725c 6e20 2020 2020 2020 2020 2020  "\r\n           
-00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045a0: 2020 2020 7374 796c 653d 5c22 6469 7370      style=\"disp
-000045b0: 6c61 793a 6e6f 6e65 5c22 5c72 5c6e 0a20  lay:none\"\r\n. 
-000045c0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045e0: 2020 2020 2020 636c 6173 733d 5c22 666f        class=\"fo
-000045f0: 726d 2d63 6f6e 7472 6f6c 5c22 5c72 5c6e  rm-control\"\r\n
-00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004610: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00004620: 7574 6f63 6f6d 706c 6574 653d 5c22 6f66  utocomplete=\"of
-00004630: 665c 220a 2020 2020 2020 2020 7661 6c75  f\".        valu
-00004640: 653d 5c22 646f 6e6f 7473 6176 655c 2220  e=\"donotsave\" 
-00004650: 2f3e 5c72 5c6e 2020 2020 2020 2020 2020  />\r\n          
-00004660: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00004670: 6e70 7574 2074 7970 653d 5c22 7061 7373  nput type=\"pass
-00004680: 776f 7264 5c22 0a20 2020 2020 2020 2069  word\".        i
-00004690: 643d 5c22 6870 322d 6765 6e65 7261 6c5c  d=\"hp2-general\
-000046a0: 225c 725c 6e20 2020 2020 2020 2020 2020  "\r\n           
-000046b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046c0: 2020 2020 7374 796c 653d 5c22 6469 7370      style=\"disp
-000046d0: 6c61 793a 6e6f 6e65 5c22 5c72 5c6e 0a20  lay:none\"\r\n. 
-000046e0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004700: 2020 2020 2020 636c 6173 733d 5c22 666f        class=\"fo
-00004710: 726d 2d63 6f6e 7472 6f6c 5c22 5c72 5c6e  rm-control\"\r\n
+00004550: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00004580: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+00004590: 2273 6572 7669 6365 2d69 7465 6d20 6f72  "service-item or
+000045a0: 6465 722d 6e65 772d 626f 785c 223e 5c72  der-new-box\">\r
+000045b0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+000045c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045d0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+000045e0: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+000045f0: 3d5c 2276 6572 7469 6361 6c2d 6365 6e74  =\"vertical-cent
+00004600: 6572 696e 672d 7772 6170 7065 7220 7465  ering-wrapper te
+00004610: 7874 2d63 656e 7465 725c 223e 5c72 5c6e  xt-center\">\r\n
+00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004650: 3c61 0a20 2020 2020 2020 2068 7265 663d  <a.        href=
+00004660: 5c22 5c22 2063 6c61 7373 3d5c 226f 7264  \"\" class=\"ord
+00004670: 6572 2d6e 6577 2063 7265 6174 652d 7365  er-new create-se
+00004680: 7276 6963 652d 6275 7474 6f6e 5c22 3e54  rvice-button\">T
+00004690: 696c 6161 2075 7573 6920 7061 6c76 656c  ilaa uusi palvel
+000046a0: 753c 7370 616e 5c72 5c6e 0a20 2020 2020  u<span\r\n.     
+000046b0: 2020 205c 2020 2020 2020 2020 2020 2020     \            
+000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2020 2020 2020 2020 2020 2063 6c61 7373             class
+000046f0: 3d5c 2272 6f75 6e64 6564 2d6c 696e 6b5c  =\"rounded-link\
+00004700: 223e 2b3c 2f73 7061 6e3e 3c2f 613e 5c72  ">+</span></a>\r
+00004710: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
 00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004730: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00004740: 7574 6f63 6f6d 706c 6574 653d 5c22 6f66  utocomplete=\"of
-00004750: 665c 220a 2020 2020 2020 2020 7661 6c75  f\".        valu
-00004760: 653d 5c22 646f 6e6f 7473 6176 6532 5c22  e=\"donotsave2\"
-00004770: 202f 3e5c 725c 6e20 2020 2020 2020 2020   />\r\n         
-00004780: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00004790: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-000047a0: 2020 2020 2020 2020 205c 725c 6e0a 2020           \r\n.  
-000047b0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-000047c0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-000047d0: 6c61 7373 3d5c 2263 6865 636b 626f 785c  lass=\"checkbox\
-000047e0: 2220 7374 796c 653d 5c22 6469 7370 6c61  " style=\"displa
-000047f0: 793a 6e6f 6e65 5c22 3e5c 725c 6e20 2020  y:none\">\r\n   
+00004730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004740: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
+00004750: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004770: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
+00004780: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00004790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
+000047c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047d0: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
+000047e0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004810: 2020 2020 203c 6c61 6265 6c3e 5c72 5c6e       <label>\r\n
-00004820: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-00004830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004840: 2020 2020 203c 696e 7075 7420 7479 7065       <input type
-00004850: 3d5c 2263 6865 636b 626f 785c 2220 6964  =\"checkbox\" id
-00004860: 3d5c 2272 656d 656d 6265 722d 6d65 5c22  =\"remember-me\"
-00004870: 206e 616d 653d 5c22 7265 6d65 6d62 6572   name=\"remember
-00004880: 2d6d 655c 223e 5c72 5c6e 0a20 2020 2020  -me\">\r\n.     
-00004890: 2020 205c 2020 2020 2020 2020 2020 2020     \            
-000048a0: 2020 2020 2020 2020 2020 2020 2020 204d                 M
-000048b0: 7569 7374 6120 6d69 6e75 745c 725c 6e20  uista minut\r\n 
+00004810: 205c 725c 6e5c 725c 6e20 2020 2020 2020   \r\n\r\n       
+00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004830: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
+00004840: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+00004850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004860: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00004870: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004890: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+000048a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048b0: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
 000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048d0: 2020 2020 2020 203c 2f6c 6162 656c 3e5c         </label>\
-000048e0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004900: 3c2f 6469 763e 5c72 5c6e 2020 2020 2020  </div>\r\n      
-00004910: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00004920: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
-00004930: 2020 2020 2020 2020 3c64 6976 0a20 2020          <div.   
-00004940: 2020 2020 2063 6c61 7373 3d5c 2266 6f72       class=\"for
-00004950: 6d2d 6772 6f75 705c 223e 5c72 5c6e 2020  m-group\">\r\n  
-00004960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004970: 2020 3c62 7574 746f 6e20 7479 7065 3d5c    <button type=\
-00004980: 2262 7574 746f 6e5c 2220 6461 7461 2d61  "button\" data-a
-00004990: 6374 696f 6e3d 5c22 666f 7267 6f74 7465  ction=\"forgotte
-000049a0: 6e2d 7061 7373 776f 7264 5c22 0a20 2020  n-password\".   
-000049b0: 2020 2020 2063 6c61 7373 3d5c 2262 746e       class=\"btn
-000049c0: 2062 746e 2d6c 696e 6b5c 223e 5c72 5c6e   btn-link\">\r\n
-000049d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049e0: 2020 2020 2020 2020 5469 6c61 6120 756e          Tilaa un
-000049f0: 6f68 7475 6e75 7420 7361 6c61 7361 6e61  ohtunut salasana
-00004a00: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a20: 203c 2f62 7574 746f 6e3e 5c72 5c6e 2020   </button>\r\n  
-00004a30: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00004a40: 6469 763e 5c72 5c6e 2020 2020 2020 2020  div>\r\n        
-00004a50: 2020 2020 2020 2020 3c64 6976 0a20 2020          <div.   
-00004a60: 2020 2020 2063 6c61 7373 3d5c 2266 6f72       class=\"for
-00004a70: 6d2d 6772 6f75 705c 2220 6964 3d5c 226c  m-group\" id=\"l
-00004a80: 6f67 696e 2d62 7574 746f 6e2d 6772 6f75  ogin-button-grou
-00004a90: 705c 223e 5c72 5c6e 2020 2020 2020 2020  p\">\r\n        
-00004aa0: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
-00004ab0: 746f 6e0a 2020 2020 2020 2020 7479 7065  ton.        type
-00004ac0: 3d5c 2273 7562 6d69 745c 2220 636c 6173  =\"submit\" clas
-00004ad0: 733d 5c22 6274 6e20 6274 6e2d 7072 696d  s=\"btn btn-prim
-00004ae0: 6172 795c 2220 6964 3d5c 226c 6f67 696e  ary\" id=\"login
-00004af0: 2d62 7574 746f 6e2d 6765 6e65 7261 6c5c  -button-general\
-00004b00: 223e 5c72 5c6e 0a20 2020 2020 2020 205c  ">\r\n.        \
-00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b20: 2020 2020 2020 204b 6972 6a61 7564 755c         Kirjaudu\
-00004b30: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-00004b40: 2020 2020 2020 203c 2f62 7574 746f 6e3e         </button>
-00004b50: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00004b60: 2020 2020 2020 2020 5c72 5c6e 0a20 2020          \r\n.   
-00004b70: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-00004b80: 2020 2020 2020 2020 203c 6275 7474 6f6e           <button
-00004b90: 2074 7970 653d 5c22 6275 7474 6f6e 5c22   type=\"button\"
-00004ba0: 2064 6174 612d 6163 7469 6f6e 3d5c 2271   data-action=\"q
-00004bb0: 722d 7265 6164 6572 5c22 2063 6c61 7373  r-reader\" class
-00004bc0: 3d5c 2262 746e 0a20 2020 2020 2020 2062  =\"btn.        b
-00004bd0: 746e 2d70 7269 6d61 7279 5c22 3e5c 725c  tn-primary\">\r\
-00004be0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00004bf0: 2020 2020 2020 2020 204c 7565 2051 522d           Lue QR-
-00004c00: 6b6f 6f64 695c 725c 6e20 2020 2020 2020  koodi\r\n       
-00004c10: 2020 2020 2020 2020 2020 2020 203c 2f62               </b
-00004c20: 7574 746f 6e3e 5c72 5c6e 0a20 2020 2020  utton>\r\n.     
-00004c30: 2020 205c 2020 2020 2020 2020 2020 2020     \            
-00004c40: 2020 2020 2020 205c 725c 6e20 2020 2020         \r\n     
-00004c50: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00004c60: 3e5c 725c 6e5c 725c 6e20 2020 2020 2020  >\r\n\r\n       
-00004c70: 2020 2020 2020 2020 205c 725c 6e5c 725c           \r\n\r\
-00004c80: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-00004c90: 2020 2020 2020 2020 2020 5c72 5c6e 2020            \r\n  
-00004ca0: 2020 2020 2020 2020 2020 3c2f 666f 726d            </form
-00004cb0: 3e5c 725c 6e5c 725c 6e20 2020 2020 2020  >\r\n\r\n       
-00004cc0: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
-00004cd0: 2020 2020 2020 2020 203c 212d 2d0a 2020           <!--.  
-00004ce0: 2020 2020 2020 416c 6572 7420 6d75 7374        Alert must
-00004cf0: 206e 6f74 2063 6f6e 7461 696e 2061 6e79   not contain any
-00004d00: 2065 7874 7261 2063 6861 7261 6374 6572   extra character
-00004d10: 732c 2065 7665 6e20 7768 6974 6573 7061  s, even whitespa
-00004d20: 6365 2c20 666f 7220 6869 6469 6e67 2074  ce, for hiding t
-00004d30: 6f0a 2020 2020 2020 2020 776f 726b 2070  o.        work p
-00004d40: 726f 7065 726c 792e 202d 2d3e 5c72 5c6e  roperly. -->\r\n
+000048d0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+000048e0: 733d 5c22 636c 6561 7266 6978 5c22 3e3c  s=\"clearfix\"><
+000048f0: 2f64 6976 3e5c 725c 6e0a 2020 2020 2020  /div>\r\n.      
+00004900: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+00004910: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
+00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004930: 3c2f 6469 763e 5c72 5c6e 2020 2020 2020  </div>\r\n      
+00004940: 2020 2020 2020 3c2f 7365 6374 696f 6e3e        </section>
+00004950: 5c72 5c6e 5c72 5c6e 0a20 2020 2020 2020  \r\n\r\n.       
+00004960: 205c 2020 2020 2020 2020 2020 205c 725c   \           \r\
+00004970: 6e5c 725c 6e20 2020 2020 2020 2020 2020  n\r\n           
+00004980: 205c 725c 6e20 2020 2020 2020 2020 2020   \r\n           
+00004990: 2020 2020 203c 7365 6374 696f 6e20 6964       <section id
+000049a0: 3d5c 2263 7573 746f 6d65 722d 6461 7461  =\"customer-data
+000049b0: 5c22 0a20 2020 2020 2020 2063 6c61 7373  \".        class
+000049c0: 3d5c 2263 7573 746f 6d65 722d 6461 7461  =\"customer-data
+000049d0: 2063 6f6e 7461 696e 6572 5c22 2073 7479   container\" sty
+000049e0: 6c65 3d5c 2264 6973 706c 6179 3a6e 6f6e  le=\"display:non
+000049f0: 655c 223e 5c72 5c6e 2020 2020 2020 2020  e\">\r\n        
+00004a00: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00004a10: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+00004a20: 2272 6f77 5c22 3e5c 725c 6e20 2020 2020  "row\">\r\n     
+00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a40: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
+00004a50: 636f 6c2d 6d64 2d31 325c 223e 5c72 5c6e  col-md-12\">\r\n
+00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a70: 2020 2020 2020 2020 2020 2020 3c75 6c0a              <ul.
+00004a80: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+00004a90: 6c69 7374 2d69 6e6c 696e 6520 7465 7874  list-inline text
+00004aa0: 2d63 656e 7465 725c 2220 6461 7461 2d72  -center\" data-r
+00004ab0: 6f6c 653d 5c22 6163 7469 6f6e 2d62 7574  ole=\"action-but
+00004ac0: 746f 6e73 5c22 3e5c 725c 6e20 2020 2020  tons\">\r\n     
+00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ae0: 2020 2020 2020 2020 2020 205c 725c 6e0a             \r\n.
+00004af0: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b10: 2020 2020 2020 2020 2020 2020 3c6c 693e              <li>
+00004b20: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b40: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
+00004b50: 746f 6e0a 2020 2020 2020 2020 636c 6173  ton.        clas
+00004b60: 733d 5c22 6274 6e20 6274 6e2d 7072 696d  s=\"btn btn-prim
+00004b70: 6172 795c 2220 6461 7461 2d61 6374 696f  ary\" data-actio
+00004b80: 6e3d 5c22 636f 6d70 6f73 742d 6e6f 7469  n=\"compost-noti
+00004b90: 6365 5c22 3e5c 725c 6e20 2020 2020 2020  ce\">\r\n       
+00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bc0: 2020 2020 2054 6565 0a20 2020 2020 2020       Tee.       
+00004bd0: 206b 6f6d 706f 7374 6f69 6e74 692d 696c   kompostointi-il
+00004be0: 6d6f 6974 7573 5c72 5c6e 2020 2020 2020  moitus\r\n      
+00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c10: 2020 3c2f 6275 7474 6f6e 3e5c 725c 6e0a    </button>\r\n.
+00004c20: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+00004c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c50: 3c64 6976 2064 6174 612d 726f 6c65 3d5c  <div data-role=\
+00004c60: 2263 6f6d 706f 7374 2d6e 6f74 6963 652d  "compost-notice-
+00004c70: 696e 666f 726d 6174 696f 6e5c 223e 3c2f  information\"></
+00004c80: 6469 763e 5c72 5c6e 0a20 2020 2020 2020  div>\r\n.       
+00004c90: 205c 2020 2020 2020 2020 2020 2020 2020   \              
+00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cb0: 2020 2020 203c 2f6c 693e 5c72 5c6e 2020       </li>\r\n  
+00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cd0: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+00004ce0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d00: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
+00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d30: 2020 203c 6c69 3e5c 725c 6e0a 2020 2020     <li>\r\n.    
+00004d40: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
 00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d60: 3c62 723e 5c72 5c6e 2020 2020 2020 2020  <br>\r\n        
-00004d70: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00004d80: 7373 3d5c 2265 7272 6f72 2d62 756c 6c65  ss=\"error-bulle
-00004d90: 7469 6e0a 2020 2020 2020 2020 616c 6572  tin.        aler
-00004da0: 7420 616c 6572 742d 696e 666f 5c22 3e3c  t alert-info\"><
-00004db0: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
-00004dc0: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
-00004dd0: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
-00004de0: 2020 2020 205c 725c 6e0a 2020 2020 2020       \r\n.      
-00004df0: 2020 5c20 2020 2020 2020 3c2f 6469 763e    \       </div>
-00004e00: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
-00004e10: 5c72 5c6e 2020 2020 2020 2020 3c64 6976  \r\n        <div
-00004e20: 2063 6c61 7373 3d5c 2263 6f6c 2d73 6d2d   class=\"col-sm-
-00004e30: 3620 636f 6c2d 6d64 2d36 5c22 3e5c 725c  6 col-md-6\">\r\
-00004e40: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-00004e50: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
-00004e60: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
-00004e70: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00004e80: 3d5c 2272 6f77 206c 6f67 696e 2d70 6167  =\"row login-pag
-00004e90: 652d 6163 7469 6f6e 735c 223e 5c72 5c6e  e-actions\">\r\n
-00004ea0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-00004eb0: 2020 2020 2020 2020 205c 725c 6e5c 725c           \r\n\r\
-00004ec0: 6e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  n\r\n\r\n\r\n\r\
-00004ed0: 6e5c 725c 6e5c 725c 6e5c 725c 6e5c 743c  n\r\n\r\n\r\n\t<
-00004ee0: 6469 7620 636c 6173 733d 5c22 726f 775c  div class=\"row\
-00004ef0: 223e 5c72 5c6e 5c74 5c74 5c72 5c6e 5c74  ">\r\n\t\t\r\n\t
-00004f00: 5c74 5c72 5c6e 5c74 5c74 5c74 5c72 5c6e  \t\r\n\t\t\t\r\n
-00004f10: 5c74 5c74 5c72 5c6e 5c74 5c74 3c62 7574  \t\t\r\n\t\t<but
-00004f20: 746f 6e0a 2020 2020 2020 2020 7479 7065  ton.        type
-00004f30: 3d5c 2262 7574 746f 6e5c 2220 636c 6173  =\"button\" clas
-00004f40: 733d 5c22 6274 6e20 6274 6e2d 7072 696d  s=\"btn btn-prim
-00004f50: 6172 7920 6274 6e2d 626c 6f63 6b20 6c6f  ary btn-block lo
-00004f60: 6e67 2d74 6578 742d 6275 7474 6f6e 5c22  ng-text-button\"
-00004f70: 2064 6174 612d 6163 7469 6f6e 3d5c 226a   data-action=\"j
-00004f80: 6f69 6e2d 7761 7374 652d 636f 6c6c 6563  oin-waste-collec
-00004f90: 7469 6f6e 5c22 3e5c 725c 6e5c 745c 745c  tion\">\r\n\t\t\
-00004fa0: 744c 6969 7479 0a20 2020 2020 2020 206a  tLiity.        j
-00004fb0: 5c78 4534 7465 6875 6f6c 746f 6f6e 5c72  \xE4tehuoltoon\r
-00004fc0: 5c6e 5c74 5c74 3c2f 6275 7474 6f6e 3e5c  \n\t\t</button>\
-00004fd0: 725c 6e5c 745c 745c 725c 6e5c 743c 2f64  r\n\t\t\r\n\t</d
-00004fe0: 6976 3e5c 725c 6e5c 725c 6e5c 725c 6e5c  iv>\r\n\r\n\r\n\
-00004ff0: 725c 6e5c 743c 6469 760a 2020 2020 2020  r\n\t<div.      
-00005000: 2020 636c 6173 733d 5c22 726f 775c 223e    class=\"row\">
-00005010: 5c72 5c6e 5c74 5c74 3c68 343e 3c2f 6834  \r\n\t\t<h4></h4
-00005020: 3e5c 725c 6e5c 745c 745c 725c 6e5c 745c  >\r\n\t\t\r\n\t\
-00005030: 745c 745c 725c 6e5c 745c 745c 725c 6e5c  t\t\r\n\t\t\r\n\
-00005040: 745c 743c 6275 7474 6f6e 2074 7970 653d  t\t<button type=
-00005050: 5c22 6275 7474 6f6e 5c22 0a20 2020 2020  \"button\".     
-00005060: 2020 2063 6c61 7373 3d5c 2262 746e 2062     class=\"btn b
-00005070: 746e 2d70 7269 6d61 7279 2062 746e 2d62  tn-primary btn-b
-00005080: 6c6f 636b 206c 6f6e 672d 7465 7874 2d62  lock long-text-b
-00005090: 7574 746f 6e20 636f 6d70 6f73 742d 6e6f  utton compost-no
-000050a0: 7465 5c22 2064 6174 612d 6163 7469 6f6e  te\" data-action
-000050b0: 3d5c 226d 616b 652d 636f 6d70 6f73 742d  =\"make-compost-
-000050c0: 6e6f 7469 6365 5c22 3e5c 725c 6e5c 745c  notice\">\r\n\t\
-000050d0: 745c 7454 5c78 4534 7974 5c78 4534 0a20  t\tT\xE4yt\xE4. 
-000050e0: 2020 2020 2020 206b 6f6d 706f 7374 6f69         kompostoi
-000050f0: 6e74 692d 696c 6d6f 6974 7573 5c72 5c6e  nti-ilmoitus\r\n
-00005100: 5c74 5c74 3c2f 6275 7474 6f6e 3e5c 725c  \t\t</button>\r\
-00005110: 6e5c 745c 745c 725c 6e5c 743c 2f64 6976  n\t\t\r\n\t</div
-00005120: 3e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  >\r\n\r\n\r\n\r\
-00005130: 6e5c 725c 6e5c 745c 725c 6e5c 745c 725c  n\r\n\t\r\n\t\r\
-00005140: 6e5c 745c 725c 6e5c 745c 725c 6e5c 745c  n\t\r\n\t\r\n\t\
-00005150: 725c 6e5c 725c 6e5c 745c 725c 6e5c 725c  r\n\r\n\t\r\n\r\
-00005160: 6e5c 745c 725c 6e5c 745c 725c 6e5c 725c  n\t\r\n\t\r\n\r\
-00005170: 6e5c 745c 725c 6e5c 745c 725c 6e5c 743c  n\t\r\n\t\r\n\t<
-00005180: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-00005190: 733d 5c22 726f 775c 223e 5c72 5c6e 5c74  s=\"row\">\r\n\t
-000051a0: 5c74 3c68 343e 3c2f 6834 3e5c 725c 6e5c  \t<h4></h4>\r\n\
-000051b0: 745c 745c 725c 6e5c 745c 745c 745c 725c  t\t\r\n\t\t\t\r\
-000051c0: 6e5c 745c 745c 725c 6e5c 745c 743c 6275  n\t\t\r\n\t\t<bu
-000051d0: 7474 6f6e 2074 7970 653d 5c22 6275 7474  tton type=\"butt
-000051e0: 6f6e 5c22 0a20 2020 2020 2020 2063 6c61  on\".        cla
-000051f0: 7373 3d5c 2262 746e 2062 746e 2d70 7269  ss=\"btn btn-pri
-00005200: 6d61 7279 2062 746e 2d62 6c6f 636b 206c  mary btn-block l
-00005210: 6f6e 672d 7465 7874 2d62 7574 746f 6e5c  ong-text-button\
-00005220: 2220 6461 7461 2d61 6374 696f 6e3d 5c22  " data-action=\"
-00005230: 6769 7665 2d66 6565 6462 6163 6b5c 220a  give-feedback\".
-00005240: 2020 2020 2020 2020 6461 7461 2d66 6565          data-fee
-00005250: 6462 6163 6b2d 7769 6e64 6f77 2d69 643d  dback-window-id=
-00005260: 5c22 305c 223e 5c72 5c6e 5c74 5c74 5c74  \"0\">\r\n\t\t\t
-00005270: 416e 6e61 2070 616c 6175 7465 7474 615c  Anna palautetta\
-00005280: 725c 6e5c 745c 743c 2f62 7574 746f 6e3e  r\n\t\t</button>
-00005290: 5c72 5c6e 5c74 5c74 5c72 5c6e 5c74 3c2f  \r\n\t\t\r\n\t</
-000052a0: 6469 763e 5c72 5c6e 5c72 5c6e 5c74 5c72  div>\r\n\r\n\t\r
-000052b0: 5c6e 5c72 5c6e 5c74 5c72 5c6e 5c72 5c6e  \n\r\n\t\r\n\r\n
-000052c0: 5c74 5c72 5c6e 5c72 5c6e 5c74 5c72 5c6e  \t\r\n\r\n\t\r\n
-000052d0: 5c74 5c72 5c6e 5c72 5c6e 5c74 5c72 5c6e  \t\r\n\r\n\t\r\n
-000052e0: 5c72 5c6e 5c74 5c72 5c6e 5c74 5c72 5c6e  \r\n\t\r\n\t\r\n
-000052f0: 5c72 5c6e 5c74 5c72 5c6e 5c72 5c6e 5c72  \r\n\t\r\n\r\n\r
-00005300: 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72  \n\r\n\r\n\r\n\r
-00005310: 5c6e 5c72 5c6e 5c72 5c6e 0a20 2020 2020  \n\r\n\r\n.     
-00005320: 2020 205c 2020 2020 2020 2020 2020 203c     \           <
-00005330: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
-00005340: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
-00005350: 203c 2f64 6976 3e5c 725c 6e20 2020 205c   </div>\r\n    \
-00005360: 725c 6e5c 725c 6e20 2020 203c 2f64 6976  r\n\r\n    </div
-00005370: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
-00005380: 2020 5c72 5c6e 2020 2020 3c64 6976 2069    \r\n    <div i
-00005390: 643d 5c22 6c6f 6769 6e2d 666f 6f74 6572  d=\"login-footer
-000053a0: 5c22 2063 6c61 7373 3d5c 2272 6f77 5c22  \" class=\"row\"
-000053b0: 3e5c 725c 6e20 2020 2020 2020 203c 6469  >\r\n        <di
-000053c0: 7620 636c 6173 733d 5c22 636f 6e74 6163  v class=\"contac
-000053d0: 742d 696e 666f 5c22 3e5c 725c 6e0a 2020  t-info\">\r\n.  
-000053e0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-000053f0: 2020 3c64 6976 2063 6c61 7373 3d5c 2263    <div class=\"c
-00005400: 6f6c 2d73 6d2d 3620 636f 6c2d 6d64 2d36  ol-sm-6 col-md-6
-00005410: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
-00005420: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00005430: 733d 5c22 6c6f 6769 6e2d 666f 6f74 6572  s=\"login-footer
-00005440: 2d74 6578 745c 223e 5c72 5c6e 0a20 2020  -text\">\r\n.   
-00005450: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-00005460: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
-00005470: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00005480: 6976 3e5c 725c 6e20 2020 2020 2020 2020  iv>\r\n         
-00005490: 2020 203c 2f64 6976 3e5c 725c 6e20 2020     </div>\r\n   
-000054a0: 2020 2020 2020 2020 203c 6469 760a 2020           <div.  
-000054b0: 2020 2020 2020 636c 6173 733d 5c22 636f        class=\"co
-000054c0: 6c2d 736d 2d36 2063 6f6c 2d6d 642d 365c  l-sm-6 col-md-6\
-000054d0: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
-000054e0: 2020 2020 2020 205c 725c 6e20 2020 2020         \r\n     
-000054f0: 2020 2020 2020 2020 2020 2020 2020 205c                 \
-00005500: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00005530: 2020 2020 2020 2020 5c72 5c6e 2020 2020          \r\n    
-00005540: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
-00005550: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00005560: 6976 3e5c 725c 6e0a 2020 2020 2020 2020  iv>\r\n.        
-00005570: 5c20 2020 2020 2020 3c2f 6469 763e 5c72  \       </div>\r
-00005580: 5c6e 2020 2020 3c2f 6469 763e 5c72 5c6e  \n    </div>\r\n
-00005590: 3c2f 6469 763e 5c72 5c6e 5c74 5c72 5c6e  </div>\r\n\t\r\n
-000055a0: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 5c72  </div>\r\n\r\n\r
-000055b0: 5c6e 5c72 5c6e 5c72 5c6e 0a20 2020 2020  \n\r\n\r\n.     
-000055c0: 2020 205c 2020 2020 2020 2020 2020 203c     \           <
-000055d0: 2f73 6563 7469 6f6e 3e5c 725c 6e5c 725c  /section>\r\n\r\
-000055e0: 6e20 2020 2020 2020 2020 2020 203c 7365  n            <se
-000055f0: 6374 696f 6e20 6964 3d5c 2273 6572 7669  ction id=\"servi
-00005600: 6365 2d6c 6973 745c 2220 636c 6173 733d  ce-list\" class=
-00005610: 5c22 7365 7276 6963 6573 0a20 2020 2020  \"services.     
-00005620: 2020 2063 6f6e 7461 696e 6572 5c22 2073     container\" s
-00005630: 7479 6c65 3d5c 2264 6973 706c 6179 3a6e  tyle=\"display:n
-00005640: 6f6e 655c 223e 5c72 5c6e 2020 2020 2020  one\">\r\n      
-00005650: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00005660: 6c61 7373 3d5c 2265 6d70 7479 2d70 6167  lass=\"empty-pag
-00005670: 655c 223e 5c72 5c6e 0a20 2020 2020 2020  e\">\r\n.       
-00005680: 205c 2020 2020 2020 2020 2020 2020 2020   \              
-00005690: 2020 2020 203c 7020 636c 6173 733d 5c22       <p class=\"
-000056a0: 6c65 6164 2074 6578 742d 6365 6e74 6572  lead text-center
-000056b0: 5c22 3e56 616c 6974 7365 206b 6f68 6465  \">Valitse kohde
-000056c0: 206f 696b 6561 6e20 796c 5c78 4534 6b75   oikean yl\xE4ku
-000056d0: 6c6d 616e 0a20 2020 2020 2020 2076 616c  lman.        val
-000056e0: 696b 6f73 7461 2e3c 2f70 3e5c 725c 6e20  ikosta.</p>\r\n 
-000056f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00005700: 2f64 6976 3e5c 725c 6e5c 725c 6e20 2020  /div>\r\n\r\n   
-00005710: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00005720: 7620 636c 6173 733d 5c22 636f 6e74 656e  v class=\"conten
-00005730: 740a 2020 2020 2020 2020 726f 775c 223e  t.        row\">
-00005740: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00005750: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00005760: 7373 3d5c 2263 6f6c 2d6c 672d 3130 2063  ss=\"col-lg-10 c
-00005770: 6f6c 2d6c 672d 6f66 6673 6574 2d31 5c22  ol-lg-offset-1\"
-00005780: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
+00004d60: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
+00004d70: 746f 6e20 636c 6173 733d 5c22 6274 6e20  ton class=\"btn 
+00004d80: 6274 6e2d 7072 696d 6172 795c 220a 2020  btn-primary\".  
+00004d90: 2020 2020 2020 6461 7461 2d61 6374 696f        data-actio
+00004da0: 6e3d 5c22 6368 616e 6765 2d6a 6f69 6e2d  n=\"change-join-
+00004db0: 7479 7065 5c22 3e5c 725c 6e20 2020 2020  type\">\r\n     
+00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004de0: 2020 2020 2020 2056 6169 6864 610a 2020         Vaihda.  
+00004df0: 2020 2020 2020 6a5c 7845 3474 6568 756f        j\xE4tehuo
+00004e00: 6c6c 6f6e 206c 6969 7474 796d 6973 7461  llon liittymista
+00004e10: 7061 615c 725c 6e20 2020 2020 2020 2020  paa\r\n         
+00004e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00004e40: 2f62 7574 746f 6e3e 5c72 5c6e 0a20 2020  /button>\r\n.   
+00004e50: 2020 2020 205c 2020 2020 2020 2020 2020       \          
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 2020 2020 2020 2020 203c 2f6c 693e 5c72           </li>\r
+00004e80: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00004e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ea0: 2020 5c72 5c6e 0a20 2020 2020 2020 205c    \r\n.        \
+00004eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ec0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00004ed0: 6c69 3e5c 725c 6e20 2020 2020 2020 2020  li>\r\n         
+00004ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ef0: 2020 2020 2020 2020 2020 203c 6275 7474             <butt
+00004f00: 6f6e 0a20 2020 2020 2020 2063 6c61 7373  on.        class
+00004f10: 3d5c 2262 746e 2062 746e 2d70 7269 6d61  =\"btn btn-prima
+00004f20: 7279 5c22 2064 6174 612d 6163 7469 6f6e  ry\" data-action
+00004f30: 3d5c 2274 6572 6d69 6e61 7465 2d73 6572  =\"terminate-ser
+00004f40: 7669 6365 5c22 3e5c 725c 6e20 2020 2020  vice\">\r\n     
+00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f70: 2020 2050 5c78 4534 5c78 4534 745c 7845     P\xE4\xE4t\xE
+00004f80: 340a 2020 2020 2020 2020 6b6f 6874 6565  4.        kohtee
+00004f90: 6e20 6a5c 7845 3474 6568 756f 6c74 6f5c  n j\xE4tehuolto\
+00004fa0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fc0: 2020 2020 2020 203c 2f62 7574 746f 6e3e         </button>
+00004fd0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+00004fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ff0: 2020 2020 2020 2020 2020 2020 203c 2f6c               </l
+00005000: 693e 5c72 5c6e 2020 2020 2020 2020 2020  i>\r\n          
+00005010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005020: 2020 3c2f 756c 3e5c 725c 6e0a 2020 2020    </ul>\r\n.    
+00005030: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
+00005040: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00005050: 763e 5c72 5c6e 2020 2020 2020 2020 2020  v>\r\n          
+00005060: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00005070: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00005080: 2020 2020 2020 2020 3c64 6976 0a20 2020          <div.   
+00005090: 2020 2020 2063 6c61 7373 3d5c 2272 6f77       class=\"row
+000050a0: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
+000050b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000050c0: 6469 7620 636c 6173 733d 5c22 636f 6c2d  div class=\"col-
+000050d0: 6d64 2d31 3220 636f 6c2d 6d64 2d6f 6666  md-12 col-md-off
+000050e0: 7365 742d 300a 2020 2020 2020 2020 7061  set-0.        pa
+000050f0: 6e65 6c20 7061 6e65 6c2d 666f 726d 5c22  nel panel-form\"
+00005100: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005120: 203c 6469 7620 636c 6173 733d 5c22 666f   <div class=\"fo
+00005130: 726d 5c22 3e3c 2f64 6976 3e5c 725c 6e0a  rm\"></div>\r\n.
+00005140: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005160: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
+00005170: 2267 6c6f 6261 6c2d 7661 6c69 6461 7469  "global-validati
+00005180: 6f6e 2d65 7272 6f72 2061 6c65 7274 2061  on-error alert a
+00005190: 6c65 7274 2d64 616e 6765 725c 220a 2020  lert-danger\".  
+000051a0: 2020 2020 2020 7374 796c 653d 5c22 6469        style=\"di
+000051b0: 7370 6c61 793a 6e6f 6e65 5c22 3e5c 725c  splay:none\">\r\
+000051c0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051e0: 2054 5c78 4534 7974 5c78 4534 2070 7575   T\xE4yt\xE4 puu
+000051f0: 7474 7576 6174 0a20 2020 2020 2020 206b  ttuvat.        k
+00005200: 656e 745c 7845 3474 5c72 5c6e 2020 2020  ent\xE4t\r\n    
+00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005220: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
+00005230: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00005240: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00005250: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005270: 203c 2f64 6976 3e5c 725c 6e20 2020 2020   </div>\r\n     
+00005280: 2020 2020 2020 2020 2020 203c 2f73 6563             </sec
+00005290: 7469 6f6e 3e5c 725c 6e20 2020 2020 2020  tion>\r\n       
+000052a0: 2020 2020 205c 725c 6e5c 725c 6e0a 2020       \r\n\r\n.  
+000052b0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+000052c0: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
+000052d0: 2020 2020 2020 3c73 6563 7469 6f6e 2069        <section i
+000052e0: 643d 5c22 696e 766f 6963 6573 5c22 2063  d=\"invoices\" c
+000052f0: 6c61 7373 3d5c 2269 6e76 6f69 6365 730a  lass=\"invoices.
+00005300: 2020 2020 2020 2020 636f 6e74 6169 6e65          containe
+00005310: 725c 2220 7374 796c 653d 5c22 6469 7370  r\" style=\"disp
+00005320: 6c61 793a 6e6f 6e65 5c22 3e5c 725c 6e20  lay:none\">\r\n 
+00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005340: 2020 205c 725c 6e20 2020 2020 2020 2020     \r\n         
+00005350: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005360: 703e 4c61 7461 612d 7061 696e 696b 6b65  p>Lataa-painikke
+00005370: 6573 7461 0a20 2020 2020 2020 2070 5c78  esta.        p\x
+00005380: 4534 5c78 4534 7365 7420 6b61 7473 6f6d  E4\xE4set katsom
+00005390: 6161 6e20 6f6d 6961 206c 6173 6b75 6a61  aan omia laskuja
+000053a0: 7369 2076 756f 6465 7374 6120 3230 3138  si vuodesta 2018
+000053b0: 206c 5c78 4534 6874 6965 6e20 7064 662d   l\xE4htien pdf-
+000053c0: 6d75 6f64 6f73 7361 2e3c 2f70 3e5c 725c  muodossa.</p>\r\
+000053d0: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+000053e0: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+000053f0: 5c6e 5c72 5c6e 2020 2020 2020 2020 2020  \n\r\n          
+00005400: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00005410: 6c61 7373 3d5c 2272 6f77 5c22 3e5c 725c  lass=\"row\">\r\
+00005420: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00005430: 2020 2020 2020 2020 203c 6469 760a 2020           <div.  
+00005440: 2020 2020 2020 636c 6173 733d 5c22 636f        class=\"co
+00005450: 6c2d 6d64 2d31 3220 7061 6e65 6c20 7061  l-md-12 panel pa
+00005460: 6e65 6c2d 666f 726d 5c22 3e5c 725c 6e20  nel-form\">\r\n 
+00005470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005480: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00005490: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+000054a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054b0: 2020 2020 2020 2020 3c21 2d2d 2044 6973          <!-- Dis
+000054c0: 6162 6c65 2045 6467 6520 6272 6f77 7365  able Edge browse
+000054d0: 7220 616e 6e6f 7969 6e67 2062 6c75 6520  r annoying blue 
+000054e0: 6e75 6d62 6572 730a 2020 2020 2020 2020  numbers.        
+000054f0: 2d2d 3e5c 725c 6e20 2020 2020 2020 2020  -->\r\n         
+00005500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005510: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
+00005520: 7461 626c 652d 7265 7370 6f6e 7369 7665  table-responsive
+00005530: 5c22 2078 2d6d 732d 666f 726d 6174 2d64  \" x-ms-format-d
+00005540: 6574 6563 7469 6f6e 3d5c 226e 6f6e 655c  etection=\"none\
+00005550: 223e 5c72 5c6e 0a20 2020 2020 2020 205c  ">\r\n.        \
+00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005570: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005580: 6469 7620 6964 3d5c 2269 6e76 6f69 6365  div id=\"invoice
+00005590: 732d 6772 6964 626f 785c 223e 3c2f 6469  s-gridbox\"></di
+000055a0: 763e 5c72 5c6e 2020 2020 2020 2020 2020  v>\r\n          
+000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055c0: 2020 3c2f 6469 763e 5c72 5c6e 5c72 5c6e    </div>\r\n\r\n
+000055d0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2020 2020 203c 6469 7620 6964 3d5c 2269       <div id=\"i
+00005600: 6e76 6f69 6365 732d 6c6f 6164 696e 675c  nvoices-loading\
+00005610: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
+00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005630: 2020 2020 2020 3c70 3e5c 725c 6e0a 2020        <p>\r\n.  
+00005640: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+00005650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005660: 2020 2020 2020 2020 2020 3c69 6d67 2063            <img c
+00005670: 6c61 7373 3d5c 226c 6f61 6469 6e67 2d69  lass=\"loading-i
+00005680: 6d61 6765 5c22 2073 7263 3d5c 222f 6a61  mage\" src=\"/ja
+00005690: 7465 6b75 6b6b 6f2f 696d 6167 6573 2f61  tekukko/images/a
+000056a0: 6a61 782d 6c6f 6164 6572 2e67 6966 5c22  jax-loader.gif\"
+000056b0: 2f3e 5c72 5c6e 0a20 2020 2020 2020 205c  />\r\n.        \
+000056c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000056e0: 2f70 3e5c 725c 6e20 2020 2020 2020 2020  /p>\r\n         
+000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005700: 2020 2020 2020 203c 700a 2020 2020 2020         <p.      
+00005710: 2020 636c 6173 733d 5c22 7465 7874 2d63    class=\"text-c
+00005720: 656e 7465 7220 6d75 7465 645c 223e 4c61  enter muted\">La
+00005730: 7461 7573 2076 6f69 206b 6573 745c 7845  taus voi kest\xE
+00005740: 345c 7845 3420 7573 6569 7461 206d 696e  4\xE4 useita min
+00005750: 7575 7474 656a 6121 3c2f 703e 5c72 5c6e  uutteja!</p>\r\n
+00005760: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005780: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
 00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057a0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000057b0: 3d5c 2264 6f2d 6e6f 742d 7368 6f77 5c22  =\"do-not-show\"
-000057c0: 2069 643d 5c22 646f 2d6e 6f74 2d73 686f   id=\"do-not-sho
-000057d0: 775c 223e 4875 6f6d 6173 6974 6861 6e2c  w\">Huomasithan,
-000057e0: 0a20 2020 2020 2020 2065 7474 5c78 4534  .        ett\xE4
-000057f0: 205c 2254 696c 6161 2079 6c69 6d5c 7845   \"Tilaa ylim\xE
-00005800: 345c 7845 3472 5c78 4534 696e 656e 2074  4\xE4r\xE4inen t
-00005810: 7968 6a65 6e6e 7973 5c22 202d 746f 696d  yhjennys\" -toim
-00005820: 696e 746f 206c 5c78 4636 7974 7979 206e  into l\xF6ytyy n
-00005830: 796b 7969 7369 6e0a 2020 2020 2020 2020  ykyisin.        
-00005840: 5c22 5465 6520 6d75 7574 6f6b 7369 6120  \"Tee muutoksia 
-00005850: 7061 6c76 656c 7575 6e5c 222d 7061 696e  palveluun\"-pain
-00005860: 696b 6b65 656e 2061 6c74 612e 203c 6120  ikkeen alta. <a 
-00005870: 6872 6566 3d5c 2223 5c22 2064 6174 612d  href=\"#\" data-
-00005880: 6163 7469 6f6e 3d5c 2263 6f6d 706f 7374  action=\"compost
-00005890: 2d6e 6f74 6963 655c 223e 4b6f 6d70 6f73  -notice\">Kompos
-000058a0: 746f 696e 7469 2d69 6c6d 6f69 7475 6b73  tointi-ilmoituks
-000058b0: 6565 6e0a 2020 2020 2020 2020 705c 7845  een.        p\xE
-000058c0: 345c 7845 3473 6574 2074 5c78 4534 7374  4\xE4set t\xE4st
-000058d0: 5c78 4534 3c2f 613e 2e3c 2f64 6976 3e5c  \xE4</a>.</div>\
-000058e0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-000058f0: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
-00005900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005910: 2020 2020 2020 203c 6469 760a 2020 2020         <div.    
-00005920: 2020 2020 636c 6173 733d 5c22 7365 7276      class=\"serv
-00005930: 6963 6573 5c22 3e5c 725c 6e20 2020 2020  ices\">\r\n     
-00005940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005950: 2020 2020 2020 205c 725c 6e20 2020 2020         \r\n     
-00005960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005970: 2020 2020 2020 2020 2020 203c 6469 760a             <div.
-00005980: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-00005990: 666f 726d 2d62 7574 746f 6e73 2074 6578  form-buttons tex
-000059a0: 742d 6365 6e74 6572 2061 6374 696f 6e2d  t-center action-
-000059b0: 6275 7474 6f6e 732d 626c 6f63 6b5c 2220  buttons-block\" 
-000059c0: 6461 7461 2d72 6f6c 653d 5c22 6163 7469  data-role=\"acti
-000059d0: 6f6e 2d62 7574 746f 6e73 5c22 3e5c 725c  on-buttons\">\r\
-000059e0: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+000057a0: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
+000057b0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+000057c0: 2020 2020 203c 2f64 6976 3e5c 725c 6e0a       </div>\r\n.
+000057d0: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+000057e0: 2020 2020 2020 2020 3c2f 7365 6374 696f          </sectio
+000057f0: 6e3e 5c72 5c6e 2020 2020 2020 2020 2020  n>\r\n          
+00005800: 2020 5c72 5c6e 5c72 5c6e 2020 2020 2020    \r\n\r\n      
+00005810: 2020 2020 2020 5c72 5c6e 5c72 5c6e 2020        \r\n\r\n  
+00005820: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+00005830: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00005840: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
+00005850: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00005860: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00005870: 2020 205c 725c 6e20 2020 2020 2020 2020     \r\n         
+00005880: 2020 2020 2020 205c 725c 6e5c 725c 6e0a         \r\n\r\n.
+00005890: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+000058a0: 2020 2020 2020 2020 5c72 5c6e 5c72 5c6e          \r\n\r\n
+000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058c0: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
+000058d0: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
+000058e0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005900: 2020 2020 205c 725c 6e5c 725c 6e20 2020       \r\n\r\n   
+00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005920: 2020 2020 203c 7365 6374 696f 6e20 6964       <section id
+00005930: 3d5c 2266 6565 6462 6163 6b5c 225c 725c  =\"feedback\"\r\
+00005940: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005960: 2020 2020 2020 2020 2020 2064 6174 612d             data-
+00005970: 6665 6564 6261 636b 2d77 696e 646f 772d  feedback-window-
+00005980: 6964 3d5c 2230 5c22 5c72 5c6e 2020 2020  id=\"0\"\r\n    
+00005990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059a0: 2020 2020 2020 2020 2020 2020 2063 6c61               cla
+000059b0: 7373 3d5c 2266 6565 6462 6163 6b0a 2020  ss=\"feedback.  
+000059c0: 2020 2020 2020 636f 6e74 6169 6e65 725c        container\
+000059d0: 2220 7374 796c 653d 5c22 6469 7370 6c61  " style=\"displa
+000059e0: 793a 6e6f 6e65 5c22 3e5c 725c 6e20 2020  y:none\">\r\n   
 000059f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a00: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
-00005a10: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00005a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a30: 2020 2020 2020 2020 2020 3c64 6976 0a20            <div. 
-00005a40: 2020 2020 2020 2063 6c61 7373 3d5c 2273         class=\"s
-00005a50: 6572 7669 6365 2d69 7465 6d20 6f72 6465  ervice-item orde
-00005a60: 722d 6e65 772d 626f 785c 223e 5c72 5c6e  r-new-box\">\r\n
-00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00005aa0: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
-00005ab0: 2276 6572 7469 6361 6c2d 6365 6e74 6572  "vertical-center
-00005ac0: 696e 672d 7772 6170 7065 7220 7465 7874  ing-wrapper text
-00005ad0: 2d63 656e 7465 725c 223e 5c72 5c6e 2020  -center\">\r\n  
-00005ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b00: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
-00005b10: 0a20 2020 2020 2020 2068 7265 663d 5c22  .        href=\"
-00005b20: 5c22 2063 6c61 7373 3d5c 226f 7264 6572  \" class=\"order
-00005b30: 2d6e 6577 2063 7265 6174 652d 7365 7276  -new create-serv
-00005b40: 6963 652d 6275 7474 6f6e 5c22 3e54 696c  ice-button\">Til
-00005b50: 6161 2075 7573 6920 7061 6c76 656c 753c  aa uusi palvelu<
-00005b60: 7370 616e 5c72 5c6e 0a20 2020 2020 2020  span\r\n.       
-00005b70: 205c 2020 2020 2020 2020 2020 2020 2020   \              
-00005b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a00: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00005a10: 6173 733d 5c22 726f 775c 223e 5c72 5c6e  ass=\"row\">\r\n
+00005a20: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a40: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00005a50: 6173 733d 5c22 636f 6c2d 6d64 2d36 2063  ass=\"col-md-6 c
+00005a60: 6f6c 2d6d 642d 6f66 6673 6574 2d33 2070  ol-md-offset-3 p
+00005a70: 616e 656c 0a20 2020 2020 2020 2070 616e  anel.        pan
+00005a80: 656c 2d66 6f72 6d5c 223e 5c72 5c6e 2020  el-form\">\r\n  
+00005a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ab0: 2020 5c72 5c6e 5c72 5c6e 2020 2020 2020    \r\n\r\n      
+00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ad0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00005ae0: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+00005af0: 3d5c 2266 6f72 6d5c 223e 3c2f 6469 763e  =\"form\"></div>
+00005b00: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b20: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00005b30: 7373 3d5c 2267 6c6f 6261 6c2d 7661 6c69  ss=\"global-vali
+00005b40: 6461 7469 6f6e 2d65 7272 6f72 0a20 2020  dation-error.   
+00005b50: 2020 2020 2061 6c65 7274 2061 6c65 7274       alert alert
+00005b60: 2d64 616e 6765 725c 2220 7374 796c 653d  -danger\" style=
+00005b70: 5c22 6469 7370 6c61 793a 6e6f 6e65 5c22  \"display:none\"
+00005b80: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
 00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ba0: 2020 2020 2020 2020 2063 6c61 7373 3d5c           class=\
-00005bb0: 2272 6f75 6e64 6564 2d6c 696e 6b5c 223e  "rounded-link\">
-00005bc0: 2b3c 2f73 7061 6e3e 3c2f 613e 5c72 5c6e  +</span></a>\r\n
-00005bd0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+00005ba0: 2020 2020 2020 2020 2020 2020 2054 5c78               T\x
+00005bb0: 4534 7974 5c78 4534 0a20 2020 2020 2020  E4yt\xE4.       
+00005bc0: 2070 7575 7474 7576 6174 206b 656e 745c   puuttuvat kent\
+00005bd0: 7845 3474 5c72 5c6e 2020 2020 2020 2020  xE4t\r\n        
 00005be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c00: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
+00005bf0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00005c00: 763e 5c72 5c6e 2020 2020 2020 2020 2020  v>\r\n          
 00005c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c30: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
-00005c40: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-00005c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c60: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
-00005c70: 5c6e 5c72 5c6e 2020 2020 2020 2020 2020  \n\r\n          
-00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c90: 2020 2020 2020 2020 2020 5c72 5c6e 5c72            \r\n\r
-00005ca0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2020 2020 2020 2020 2020 2020 2020 205c                 \
-00005cd0: 725c 6e5c 725c 6e20 2020 2020 2020 2020  r\n\r\n         
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cf0: 2020 2020 2020 2020 2020 205c 725c 6e0a             \r\n.
-00005d00: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d20: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-00005d30: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00005d40: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
-00005d50: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d70: 2020 203c 2f64 6976 3e5c 725c 6e20 2020     </div>\r\n   
-00005d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d90: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00005da0: 5c22 636c 6561 7266 6978 5c22 3e3c 2f64  \"clearfix\"></d
-00005db0: 6976 3e5c 725c 6e0a 2020 2020 2020 2020  iv>\r\n.        
-00005dc0: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-00005dd0: 2020 2020 3c2f 6469 763e 5c72 5c6e 2020      </div>\r\n  
-00005de0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00005df0: 6469 763e 5c72 5c6e 2020 2020 2020 2020  div>\r\n        
-00005e00: 2020 2020 3c2f 7365 6374 696f 6e3e 5c72      </section>\r
-00005e10: 5c6e 5c72 5c6e 0a20 2020 2020 2020 205c  \n\r\n.        \
-00005e20: 2020 2020 2020 2020 2020 205c 725c 6e5c             \r\n\
-00005e30: 725c 6e20 2020 2020 2020 2020 2020 205c  r\n            \
-00005e40: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-00005e50: 2020 203c 7365 6374 696f 6e20 6964 3d5c     <section id=\
-00005e60: 2263 7573 746f 6d65 722d 6461 7461 5c22  "customer-data\"
-00005e70: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
-00005e80: 2263 7573 746f 6d65 722d 6461 7461 2063  "customer-data c
-00005e90: 6f6e 7461 696e 6572 5c22 2073 7479 6c65  ontainer\" style
-00005ea0: 3d5c 2264 6973 706c 6179 3a6e 6f6e 655c  =\"display:none\
-00005eb0: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
-00005ec0: 2020 2020 2020 2020 2020 3c64 6976 0a20            <div. 
-00005ed0: 2020 2020 2020 2063 6c61 7373 3d5c 2272         class=\"r
-00005ee0: 6f77 5c22 3e5c 725c 6e20 2020 2020 2020  ow\">\r\n       
-00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f00: 203c 6469 7620 636c 6173 733d 5c22 636f   <div class=\"co
-00005f10: 6c2d 6d64 2d31 325c 223e 5c72 5c6e 2020  l-md-12\">\r\n  
-00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f30: 2020 2020 2020 2020 2020 3c75 6c0a 2020            <ul.  
-00005f40: 2020 2020 2020 636c 6173 733d 5c22 6c69        class=\"li
-00005f50: 7374 2d69 6e6c 696e 6520 7465 7874 2d63  st-inline text-c
-00005f60: 656e 7465 725c 2220 6461 7461 2d72 6f6c  enter\" data-rol
-00005f70: 653d 5c22 6163 7469 6f6e 2d62 7574 746f  e=\"action-butto
-00005f80: 6e73 5c22 3e5c 725c 6e20 2020 2020 2020  ns\">\r\n       
+00005c20: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
+00005c30: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+00005c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c50: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
+00005c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c70: 2020 2020 2020 203c 2f73 6563 7469 6f6e         </section
+00005c80: 3e5c 725c 6e5c 725c 6e0a 2020 2020 2020  >\r\n\r\n.      
+00005c90: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+00005ca0: 2020 2020 2020 2020 2020 5c72 5c6e 5c72            \r\n\r
+00005cb0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00005cc0: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
+00005cd0: 2020 2020 2020 2020 2020 5c72 5c6e 5c72            \r\n\r
+00005ce0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00005cf0: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00005d00: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00005d10: 2020 2020 2020 205c 725c 6e20 2020 2020         \r\n     
+00005d20: 2020 2020 2020 2020 2020 205c 725c 6e5c             \r\n\
+00005d30: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00005d40: 2020 2020 2020 205c 725c 6e0a 2020 2020         \r\n.    
+00005d50: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
+00005d60: 2020 2020 2020 2020 5c72 5c6e 2020 2020          \r\n    
+00005d70: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
+00005d80: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00005d90: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
+00005da0: 2020 2020 3c73 6563 7469 6f6e 0a20 2020      <section.   
+00005db0: 2020 2020 2069 643d 5c22 7573 6572 2d64       id=\"user-d
+00005dc0: 6574 6169 6c73 5c22 2063 6c61 7373 3d5c  etails\" class=\
+00005dd0: 2275 7365 722d 6465 7461 696c 7320 636f  "user-details co
+00005de0: 6e74 6169 6e65 725c 2220 7374 796c 653d  ntainer\" style=
+00005df0: 5c22 6469 7370 6c61 793a 6e6f 6e65 5c22  \"display:none\"
+00005e00: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
+00005e10: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00005e20: 6976 2063 6c61 7373 3d5c 2272 6f77 5c22  iv class=\"row\"
+00005e30: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+00005e40: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00005e50: 6173 733d 5c22 636f 6c2d 6d64 2d36 0a20  ass=\"col-md-6. 
+00005e60: 2020 2020 2020 2063 6f6c 2d6d 642d 6f66         col-md-of
+00005e70: 6673 6574 2d33 2070 616e 656c 2070 616e  fset-3 panel pan
+00005e80: 656c 2d66 6f72 6d5c 223e 5c72 5c6e 2020  el-form\">\r\n  
+00005e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ea0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00005eb0: 3d5c 2266 6f72 6d5c 223e 3c2f 6469 763e  =\"form\"></div>
+00005ec0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+00005ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ee0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00005ef0: 5c22 676c 6f62 616c 2d76 616c 6964 6174  \"global-validat
+00005f00: 696f 6e2d 6572 726f 7220 616c 6572 7420  ion-error alert 
+00005f10: 616c 6572 742d 6461 6e67 6572 5c22 0a20  alert-danger\". 
+00005f20: 2020 2020 2020 2073 7479 6c65 3d5c 2264         style=\"d
+00005f30: 6973 706c 6179 3a6e 6f6e 655c 223e 5c72  isplay:none\">\r
+00005f40: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00005f50: 2020 2020 2020 2020 2020 2020 2020 545c                T\
+00005f60: 7845 3479 745c 7845 3420 7075 7574 7475  xE4yt\xE4 puuttu
+00005f70: 7661 740a 2020 2020 2020 2020 6b65 6e74  vat.        kent
+00005f80: 5c78 4534 745c 725c 6e20 2020 2020 2020  \xE4t\r\n       
 00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fa0: 2020 2020 2020 2020 205c 725c 6e0a 2020           \r\n.  
-00005fb0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fd0: 2020 2020 2020 2020 2020 3c6c 693e 5c72            <li>\r
-00005fe0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006000: 2020 2020 2020 2020 2020 3c62 7574 746f            <butto
-00006010: 6e0a 2020 2020 2020 2020 636c 6173 733d  n.        class=
-00006020: 5c22 6274 6e20 6274 6e2d 7072 696d 6172  \"btn btn-primar
-00006030: 795c 2220 6461 7461 2d61 6374 696f 6e3d  y\" data-action=
-00006040: 5c22 636f 6d70 6f73 742d 6e6f 7469 6365  \"compost-notice
-00006050: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
-00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006080: 2020 2054 6565 0a20 2020 2020 2020 206b     Tee.        k
-00006090: 6f6d 706f 7374 6f69 6e74 692d 696c 6d6f  ompostointi-ilmo
-000060a0: 6974 7573 5c72 5c6e 2020 2020 2020 2020  itus\r\n        
-000060b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060d0: 3c2f 6275 7474 6f6e 3e5c 725c 6e0a 2020  </button>\r\n.  
-000060e0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006100: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00006110: 6976 2064 6174 612d 726f 6c65 3d5c 2263  iv data-role=\"c
-00006120: 6f6d 706f 7374 2d6e 6f74 6963 652d 696e  ompost-notice-in
-00006130: 666f 726d 6174 696f 6e5c 223e 3c2f 6469  formation\"></di
-00006140: 763e 5c72 5c6e 0a20 2020 2020 2020 205c  v>\r\n.        \
-00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006170: 2020 203c 2f6c 693e 5c72 5c6e 2020 2020     </li>\r\n    
-00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006190: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
-000061a0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-000061b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061c0: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061f0: 203c 6c69 3e5c 725c 6e0a 2020 2020 2020   <li>\r\n.      
-00006200: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006220: 2020 2020 2020 2020 2020 3c62 7574 746f            <butto
-00006230: 6e20 636c 6173 733d 5c22 6274 6e20 6274  n class=\"btn bt
-00006240: 6e2d 7072 696d 6172 795c 220a 2020 2020  n-primary\".    
-00006250: 2020 2020 6461 7461 2d61 6374 696f 6e3d      data-action=
-00006260: 5c22 6368 616e 6765 2d6a 6f69 6e2d 7479  \"change-join-ty
-00006270: 7065 5c22 3e5c 725c 6e20 2020 2020 2020  pe\">\r\n       
-00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062a0: 2020 2020 2056 6169 6864 610a 2020 2020       Vaihda.    
-000062b0: 2020 2020 6a5c 7845 3474 6568 756f 6c6c      j\xE4tehuoll
-000062c0: 6f6e 206c 6969 7474 796d 6973 7461 7061  on liittymistapa
-000062d0: 615c 725c 6e20 2020 2020 2020 2020 2020  a\r\n           
-000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062f0: 2020 2020 2020 2020 2020 2020 203c 2f62               </b
-00006300: 7574 746f 6e3e 5c72 5c6e 0a20 2020 2020  utton>\r\n.     
-00006310: 2020 205c 2020 2020 2020 2020 2020 2020     \            
-00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006330: 2020 2020 2020 203c 2f6c 693e 5c72 5c6e         </li>\r\n
-00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006360: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006380: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
-00006390: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063b0: 2020 2020 2020 2020 203c 6275 7474 6f6e           <button
-000063c0: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
-000063d0: 2262 746e 2062 746e 2d70 7269 6d61 7279  "btn btn-primary
-000063e0: 5c22 2064 6174 612d 6163 7469 6f6e 3d5c  \" data-action=\
-000063f0: 2274 6572 6d69 6e61 7465 2d73 6572 7669  "terminate-servi
-00006400: 6365 5c22 3e5c 725c 6e20 2020 2020 2020  ce\">\r\n       
-00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006430: 2050 5c78 4534 5c78 4534 745c 7845 340a   P\xE4\xE4t\xE4.
-00006440: 2020 2020 2020 2020 6b6f 6874 6565 6e20          kohteen 
-00006450: 6a5c 7845 3474 6568 756f 6c74 6f5c 725c  j\xE4tehuolto\r\
-00006460: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006480: 2020 2020 203c 2f62 7574 746f 6e3e 5c72       </button>\r
-00006490: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064b0: 2020 2020 2020 2020 2020 203c 2f6c 693e             </li>
-000064c0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064e0: 3c2f 756c 3e5c 725c 6e0a 2020 2020 2020  </ul>\r\n.      
-000064f0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-00006500: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00006510: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00006520: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-00006530: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00006540: 2020 2020 2020 3c64 6976 0a20 2020 2020        <div.     
-00006550: 2020 2063 6c61 7373 3d5c 2272 6f77 5c22     class=\"row\"
-00006560: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-00006570: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00006580: 7620 636c 6173 733d 5c22 636f 6c2d 6d64  v class=\"col-md
-00006590: 2d31 3220 636f 6c2d 6d64 2d6f 6666 7365  -12 col-md-offse
-000065a0: 742d 300a 2020 2020 2020 2020 7061 6e65  t-0.        pane
-000065b0: 6c20 7061 6e65 6c2d 666f 726d 5c22 3e5c  l panel-form\">\
-000065c0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-000065d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000065e0: 6469 7620 636c 6173 733d 5c22 666f 726d  div class=\"form
-000065f0: 5c22 3e3c 2f64 6976 3e5c 725c 6e0a 2020  \"></div>\r\n.  
-00006600: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006620: 2020 3c64 6976 2063 6c61 7373 3d5c 2267    <div class=\"g
-00006630: 6c6f 6261 6c2d 7661 6c69 6461 7469 6f6e  lobal-validation
-00006640: 2d65 7272 6f72 2061 6c65 7274 2061 6c65  -error alert ale
-00006650: 7274 2d64 616e 6765 725c 220a 2020 2020  rt-danger\".    
-00006660: 2020 2020 7374 796c 653d 5c22 6469 7370      style=\"disp
-00006670: 6c61 793a 6e6f 6e65 5c22 3e5c 725c 6e20  lay:none\">\r\n 
-00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006690: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-000066a0: 5c78 4534 7974 5c78 4534 2070 7575 7474  \xE4yt\xE4 puutt
-000066b0: 7576 6174 0a20 2020 2020 2020 206b 656e  uvat.        ken
-000066c0: 745c 7845 3474 5c72 5c6e 2020 2020 2020  t\xE4t\r\n      
-000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
-000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-00006710: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-00006720: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00006730: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
-00006740: 2020 2020 2020 2020 203c 2f73 6563 7469           </secti
-00006750: 6f6e 3e5c 725c 6e20 2020 2020 2020 2020  on>\r\n         
-00006760: 2020 205c 725c 6e5c 725c 6e0a 2020 2020     \r\n\r\n.    
-00006770: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-00006780: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00006790: 2020 2020 3c73 6563 7469 6f6e 2069 643d      <section id=
-000067a0: 5c22 696e 766f 6963 6573 5c22 2063 6c61  \"invoices\" cla
-000067b0: 7373 3d5c 2269 6e76 6f69 6365 730a 2020  ss=\"invoices.  
-000067c0: 2020 2020 2020 636f 6e74 6169 6e65 725c        container\
-000067d0: 2220 7374 796c 653d 5c22 6469 7370 6c61  " style=\"displa
-000067e0: 793a 6e6f 6e65 5c22 3e5c 725c 6e20 2020  y:none\">\r\n   
-000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006800: 205c 725c 6e20 2020 2020 2020 2020 2020   \r\n           
-00006810: 2020 2020 2020 2020 2020 2020 203c 703e               <p>
-00006820: 4c61 7461 612d 7061 696e 696b 6b65 6573  Lataa-painikkees
-00006830: 7461 0a20 2020 2020 2020 2070 5c78 4534  ta.        p\xE4
-00006840: 5c78 4534 7365 7420 6b61 7473 6f6d 6161  \xE4set katsomaa
-00006850: 6e20 6f6d 6961 206c 6173 6b75 6a61 7369  n omia laskujasi
-00006860: 2076 756f 6465 7374 6120 3230 3138 206c   vuodesta 2018 l
-00006870: 5c78 4534 6874 6965 6e20 7064 662d 6d75  \xE4htien pdf-mu
-00006880: 6f64 6f73 7361 2e3c 2f70 3e5c 725c 6e0a  odossa.</p>\r\n.
-00006890: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-000068a0: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
-000068b0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-000068c0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000068d0: 7373 3d5c 2272 6f77 5c22 3e5c 725c 6e20  ss=\"row\">\r\n 
-000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068f0: 2020 2020 2020 203c 6469 760a 2020 2020         <div.    
-00006900: 2020 2020 636c 6173 733d 5c22 636f 6c2d      class=\"col-
-00006910: 6d64 2d31 3220 7061 6e65 6c20 7061 6e65  md-12 panel pane
-00006920: 6c2d 666f 726d 5c22 3e5c 725c 6e20 2020  l-form\">\r\n   
-00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006940: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
-00006950: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006970: 2020 2020 2020 3c21 2d2d 2044 6973 6162        <!-- Disab
-00006980: 6c65 2045 6467 6520 6272 6f77 7365 7220  le Edge browser 
-00006990: 616e 6e6f 7969 6e67 2062 6c75 6520 6e75  annoying blue nu
-000069a0: 6d62 6572 730a 2020 2020 2020 2020 2d2d  mbers.        --
-000069b0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069d0: 203c 6469 7620 636c 6173 733d 5c22 7461   <div class=\"ta
-000069e0: 626c 652d 7265 7370 6f6e 7369 7665 5c22  ble-responsive\"
-000069f0: 2078 2d6d 732d 666f 726d 6174 2d64 6574   x-ms-format-det
-00006a00: 6563 7469 6f6e 3d5c 226e 6f6e 655c 223e  ection=\"none\">
-00006a10: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a30: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00006a40: 7620 6964 3d5c 2269 6e76 6f69 6365 732d  v id=\"invoices-
-00006a50: 6772 6964 626f 785c 223e 3c2f 6469 763e  gridbox\"></div>
-00006a60: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a80: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 0a20  </div>\r\n\r\n. 
-00006a90: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ab0: 2020 203c 6469 7620 6964 3d5c 2269 6e76     <div id=\"inv
-00006ac0: 6f69 6365 732d 6c6f 6164 696e 675c 223e  oices-loading\">
-00006ad0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006af0: 2020 2020 3c70 3e5c 725c 6e0a 2020 2020      <p>\r\n.    
-00006b00: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b20: 2020 2020 2020 2020 3c69 6d67 2063 6c61          <img cla
-00006b30: 7373 3d5c 226c 6f61 6469 6e67 2d69 6d61  ss=\"loading-ima
-00006b40: 6765 5c22 2073 7263 3d5c 222f 6a61 7465  ge\" src=\"/jate
-00006b50: 6b75 6b6b 6f2f 696d 6167 6573 2f61 6a61  kukko/images/aja
-00006b60: 782d 6c6f 6164 6572 2e67 6966 5c22 2f3e  x-loader.gif\"/>
-00006b70: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b90: 2020 2020 2020 2020 2020 2020 203c 2f70               </p
-00006ba0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-00006bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bc0: 2020 2020 203c 700a 2020 2020 2020 2020       <p.        
-00006bd0: 636c 6173 733d 5c22 7465 7874 2d63 656e  class=\"text-cen
-00006be0: 7465 7220 6d75 7465 645c 223e 4c61 7461  ter muted\">Lata
-00006bf0: 7573 2076 6f69 206b 6573 745c 7845 345c  us voi kest\xE4\
-00006c00: 7845 3420 7573 6569 7461 206d 696e 7575  xE4 useita minuu
-00006c10: 7474 656a 6121 3c2f 703e 5c72 5c6e 0a20  tteja!</p>\r\n. 
-00006c20: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c40: 2020 203c 2f64 6976 3e5c 725c 6e20 2020     </div>\r\n   
-00006c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c60: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
-00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c80: 2020 203c 2f64 6976 3e5c 725c 6e0a 2020     </div>\r\n.  
-00006c90: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-00006ca0: 2020 2020 2020 3c2f 7365 6374 696f 6e3e        </section>
-00006cb0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00006cc0: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
-00006cd0: 2020 2020 5c72 5c6e 5c72 5c6e 2020 2020      \r\n\r\n    
-00006ce0: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
-00006cf0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-00006d00: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
-00006d10: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
-00006d20: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00006d30: 205c 725c 6e20 2020 2020 2020 2020 2020   \r\n           
-00006d40: 2020 2020 205c 725c 6e5c 725c 6e0a 2020       \r\n\r\n.  
-00006d50: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-00006d60: 2020 2020 2020 5c72 5c6e 5c72 5c6e 2020        \r\n\r\n  
-00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d80: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
-00006d90: 2020 2020 2020 2020 2020 5c72 5c6e 5c72            \r\n\r
-00006da0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-00006db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dc0: 2020 205c 725c 6e5c 725c 6e20 2020 2020     \r\n\r\n     
-00006dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006de0: 2020 203c 7365 6374 696f 6e20 6964 3d5c     <section id=\
-00006df0: 2266 6565 6462 6163 6b5c 225c 725c 6e0a  "feedback\"\r\n.
-00006e00: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-00006e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e20: 2020 2020 2020 2020 2064 6174 612d 6665           data-fe
-00006e30: 6564 6261 636b 2d77 696e 646f 772d 6964  edback-window-id
-00006e40: 3d5c 2230 5c22 5c72 5c6e 2020 2020 2020  =\"0\"\r\n      
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 2020 2020 2020 2020 2020 2063 6c61 7373             class
-00006e70: 3d5c 2266 6565 6462 6163 6b0a 2020 2020  =\"feedback.    
-00006e80: 2020 2020 636f 6e74 6169 6e65 725c 2220      container\" 
-00006e90: 7374 796c 653d 5c22 6469 7370 6c61 793a  style=\"display:
-00006ea0: 6e6f 6e65 5c22 3e5c 725c 6e20 2020 2020  none\">\r\n     
-00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ec0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00006ed0: 733d 5c22 726f 775c 223e 5c72 5c6e 0a20  s=\"row\">\r\n. 
-00006ee0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f00: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00006f10: 733d 5c22 636f 6c2d 6d64 2d36 2063 6f6c  s=\"col-md-6 col
-00006f20: 2d6d 642d 6f66 6673 6574 2d33 2070 616e  -md-offset-3 pan
-00006f30: 656c 0a20 2020 2020 2020 2070 616e 656c  el.        panel
-00006f40: 2d66 6f72 6d5c 223e 5c72 5c6e 2020 2020  -form\">\r\n    
-00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f70: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
-00006f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f90: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00006fa0: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
-00006fb0: 2266 6f72 6d5c 223e 3c2f 6469 763e 5c72  "form\"></div>\r
-00006fc0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fe0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00006ff0: 3d5c 2267 6c6f 6261 6c2d 7661 6c69 6461  =\"global-valida
-00007000: 7469 6f6e 2d65 7272 6f72 0a20 2020 2020  tion-error.     
-00007010: 2020 2061 6c65 7274 2061 6c65 7274 2d64     alert alert-d
-00007020: 616e 6765 725c 2220 7374 796c 653d 5c22  anger\" style=\"
-00007030: 6469 7370 6c61 793a 6e6f 6e65 5c22 3e5c  display:none\">\
-00007040: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-00007050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007060: 2020 2020 2020 2020 2020 2054 5c78 4534             T\xE4
-00007070: 7974 5c78 4534 0a20 2020 2020 2020 2070  yt\xE4.        p
-00007080: 7575 7474 7576 6174 206b 656e 745c 7845  uuttuvat kent\xE
-00007090: 3474 5c72 5c6e 2020 2020 2020 2020 2020  4t\r\n          
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-000070c0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070e0: 2020 2020 3c2f 6469 763e 5c72 5c6e 0a20      </div>\r\n. 
-000070f0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007110: 2020 203c 2f64 6976 3e5c 725c 6e20 2020     </div>\r\n   
-00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007130: 2020 2020 203c 2f73 6563 7469 6f6e 3e5c       </section>\
-00007140: 725c 6e5c 725c 6e0a 2020 2020 2020 2020  r\n\r\n.        
-00007150: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-00007160: 2020 2020 2020 2020 5c72 5c6e 5c72 5c6e          \r\n\r\n
-00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007180: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
-00007190: 2020 2020 2020 2020 5c72 5c6e 5c72 5c6e          \r\n\r\n
-000071a0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-000071b0: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
-000071c0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-000071d0: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
-000071e0: 2020 2020 2020 2020 205c 725c 6e5c 725c           \r\n\r\
-000071f0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00007200: 2020 2020 205c 725c 6e0a 2020 2020 2020       \r\n.      
-00007210: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-00007220: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
-00007230: 2020 2020 2020 2020 2020 5c72 5c6e 5c72            \r\n\r
-00007240: 5c6e 2020 2020 2020 2020 2020 2020 5c72  \n            \r
-00007250: 5c6e 5c72 5c6e 2020 2020 2020 2020 2020  \n\r\n          
-00007260: 2020 3c73 6563 7469 6f6e 0a20 2020 2020    <section.     
-00007270: 2020 2069 643d 5c22 7573 6572 2d64 6574     id=\"user-det
-00007280: 6169 6c73 5c22 2063 6c61 7373 3d5c 2275  ails\" class=\"u
-00007290: 7365 722d 6465 7461 696c 7320 636f 6e74  ser-details cont
-000072a0: 6169 6e65 725c 2220 7374 796c 653d 5c22  ainer\" style=\"
-000072b0: 6469 7370 6c61 793a 6e6f 6e65 5c22 3e5c  display:none\">\
-000072c0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-000072d0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-000072e0: 2063 6c61 7373 3d5c 2272 6f77 5c22 3e5c   class=\"row\">\
-000072f0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-00007300: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00007310: 733d 5c22 636f 6c2d 6d64 2d36 0a20 2020  s=\"col-md-6.   
-00007320: 2020 2020 2063 6f6c 2d6d 642d 6f66 6673       col-md-offs
-00007330: 6574 2d33 2070 616e 656c 2070 616e 656c  et-3 panel panel
-00007340: 2d66 6f72 6d5c 223e 5c72 5c6e 2020 2020  -form\">\r\n    
-00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007360: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
-00007370: 2266 6f72 6d5c 223e 3c2f 6469 763e 5c72  "form\"></div>\r
-00007380: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073a0: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
-000073b0: 676c 6f62 616c 2d76 616c 6964 6174 696f  global-validatio
-000073c0: 6e2d 6572 726f 7220 616c 6572 7420 616c  n-error alert al
-000073d0: 6572 742d 6461 6e67 6572 5c22 0a20 2020  ert-danger\".   
-000073e0: 2020 2020 2073 7479 6c65 3d5c 2264 6973       style=\"dis
-000073f0: 706c 6179 3a6e 6f6e 655c 223e 5c72 5c6e  play:none\">\r\n
-00007400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007410: 2020 2020 2020 2020 2020 2020 545c 7845              T\xE
-00007420: 3479 745c 7845 3420 7075 7574 7475 7661  4yt\xE4 puuttuva
-00007430: 740a 2020 2020 2020 2020 6b65 6e74 5c78  t.        kent\x
-00007440: 4534 745c 725c 6e20 2020 2020 2020 2020  E4t\r\n         
-00007450: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00007460: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
-00007470: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00007480: 6976 3e5c 725c 6e0a 2020 2020 2020 2020  iv>\r\n.        
-00007490: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-000074a0: 3c2f 6469 763e 5c72 5c6e 2020 2020 2020  </div>\r\n      
-000074b0: 2020 2020 2020 3c2f 7365 6374 696f 6e3e        </section>
-000074c0: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
-000074d0: 2020 2020 3c73 6563 7469 6f6e 0a20 2020      <section.   
-000074e0: 2020 2020 2069 643d 5c22 6c6f 676f 7574       id=\"logout
-000074f0: 5c22 2063 6c61 7373 3d5c 226c 6f67 6f75  \" class=\"logou
-00007500: 745c 223e 3c2f 7365 6374 696f 6e3e 5c72  t\"></section>\r
-00007510: 5c6e 2020 2020 2020 2020 3c2f 6469 763e  \n        </div>
-00007520: 5c72 5c6e 2020 2020 3c2f 6d61 696e 3e5c  \r\n    </main>\
-00007530: 725c 6e5c 725c 6e0a 2020 2020 2020 2020  r\n\r\n.        
-00007540: 5c20 2020 3c64 6976 3e5c 725c 6e20 2020  \   <div>\r\n   
-00007550: 2020 2020 205c 725c 6e5c 725c 6e5c 725c       \r\n\r\n\r\
-00007560: 6e3c 6469 7620 6964 3d5c 2274 6572 6d73  n<div id=\"terms
-00007570: 2d6d 6f64 616c 5c22 2063 6c61 7373 3d5c  -modal\" class=\
-00007580: 226d 6f64 616c 5c22 2073 7479 6c65 3d5c  "modal\" style=\
-00007590: 2264 6973 706c 6179 3a6e 6f6e 655c 223e  "display:none\">
-000075a0: 5c72 5c6e 5c74 3c64 6976 0a20 2020 2020  \r\n\t<div.     
-000075b0: 2020 2063 6c61 7373 3d5c 226d 6f64 616c     class=\"modal
-000075c0: 2d64 6961 6c6f 6720 6d6f 6461 6c2d 6c67  -dialog modal-lg
-000075d0: 5c22 3e5c 725c 6e5c 745c 743c 6469 7620  \">\r\n\t\t<div 
-000075e0: 636c 6173 733d 5c22 6d6f 6461 6c2d 636f  class=\"modal-co
-000075f0: 6e74 656e 745c 223e 5c72 5c6e 5c74 5c74  ntent\">\r\n\t\t
-00007600: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
-00007610: 6c61 7373 3d5c 226d 6f64 616c 2d62 6f64  lass=\"modal-bod
-00007620: 795c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  y\">\r\n\t\t\t\t
-00007630: 3c64 6976 2063 6c61 7373 3d5c 2274 6578  <div class=\"tex
-00007640: 745c 223e 3c2f 6469 763e 5c72 5c6e 5c74  t\"></div>\r\n\t
-00007650: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 5c74  \t\t\r\n\t\t\t\t
-00007660: 3c64 6976 0a20 2020 2020 2020 2064 6174  <div.        dat
-00007670: 612d 726f 6c65 3d5c 2263 6f6e 6669 726d  a-role=\"confirm
-00007680: 2d62 7574 746f 6e73 5c22 2063 6c61 7373  -buttons\" class
-00007690: 3d5c 2266 6f72 6d2d 6275 7474 6f6e 7320  =\"form-buttons 
-000076a0: 7465 7874 2d63 656e 7465 725c 223e 5c72  text-center\">\r
-000076b0: 5c6e 5c74 5c74 5c74 5c74 5c74 3c62 7574  \n\t\t\t\t\t<but
-000076c0: 746f 6e0a 2020 2020 2020 2020 7479 7065  ton.        type
-000076d0: 3d5c 2262 7574 746f 6e5c 2220 636c 6173  =\"button\" clas
-000076e0: 733d 5c22 6274 6e20 6274 6e2d 6465 6661  s=\"btn btn-defa
-000076f0: 756c 7420 6361 6e63 656c 5c22 2064 6174  ult cancel\" dat
-00007700: 612d 6469 736d 6973 733d 5c22 6d6f 6461  a-dismiss=\"moda
-00007710: 6c5c 223e 456e 0a20 2020 2020 2020 2068  l\">En.        h
-00007720: 7976 5c78 4534 6b73 7920 6568 746f 6a61  yv\xE4ksy ehtoja
-00007730: 3c2f 6275 7474 6f6e 3e5c 725c 6e5c 745c  </button>\r\n\t\
-00007740: 745c 745c 745c 743c 6275 7474 6f6e 2074  t\t\t\t<button t
-00007750: 7970 653d 5c22 6275 7474 6f6e 5c22 2063  ype=\"button\" c
-00007760: 6c61 7373 3d5c 2262 746e 0a20 2020 2020  lass=\"btn.     
-00007770: 2020 2062 746e 2d70 7269 6d61 7279 2061     btn-primary a
-00007780: 6363 6570 745c 2220 6461 7461 2d64 6973  ccept\" data-dis
-00007790: 6d69 7373 3d5c 226d 6f64 616c 5c22 3e48  miss=\"modal\">H
-000077a0: 7976 5c78 4534 6b73 796e 2065 6864 6f74  yv\xE4ksyn ehdot
-000077b0: 3c2f 6275 7474 6f6e 3e5c 725c 6e5c 745c  </button>\r\n\t\
-000077c0: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
-000077d0: 745c 745c 745c 743c 6469 760a 2020 2020  t\t\t\t<div.    
-000077e0: 2020 2020 6461 7461 2d72 6f6c 653d 5c22      data-role=\"
-000077f0: 6469 7370 6c61 792d 6275 7474 6f6e 735c  display-buttons\
-00007800: 2220 636c 6173 733d 5c22 666f 726d 2d62  " class=\"form-b
-00007810: 7574 746f 6e73 2074 6578 742d 6365 6e74  uttons text-cent
-00007820: 6572 5c22 3e5c 725c 6e5c 745c 745c 745c  er\">\r\n\t\t\t\
-00007830: 745c 743c 6275 7474 6f6e 0a20 2020 2020  t\t<button.     
-00007840: 2020 2074 7970 653d 5c22 6275 7474 6f6e     type=\"button
-00007850: 5c22 2063 6c61 7373 3d5c 2262 746e 2062  \" class=\"btn b
-00007860: 746e 2d70 7269 6d61 7279 5c22 2064 6174  tn-primary\" dat
-00007870: 612d 6469 736d 6973 733d 5c22 6d6f 6461  a-dismiss=\"moda
-00007880: 6c5c 2220 6461 7461 2d61 6374 696f 6e3d  l\" data-action=
-00007890: 5c22 6469 7370 6c61 792d 6f6b 5c22 3e4f  \"display-ok\">O
-000078a0: 4b3c 2f62 7574 746f 6e3e 5c72 5c6e 5c74  K</button>\r\n\t
-000078b0: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
-000078c0: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
-000078d0: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-000078e0: 3c2f 6469 763e 5c72 5c6e 3c2f 6469 763e  </div>\r\n</div>
-000078f0: 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e  \r\n\r\n\r\n\r\n
-00007900: 3c64 6976 0a20 2020 2020 2020 2069 643d  <div.        id=
-00007910: 5c22 6f72 6465 722d 666f 726d 2d6d 6f64  \"order-form-mod
-00007920: 616c 5c22 2063 6c61 7373 3d5c 226d 6f64  al\" class=\"mod
-00007930: 616c 5c22 2073 7479 6c65 3d5c 2264 6973  al\" style=\"dis
-00007940: 706c 6179 3a6e 6f6e 655c 2220 726f 6c65  play:none\" role
-00007950: 3d5c 2264 6961 6c6f 675c 220a 2020 2020  =\"dialog\".    
-00007960: 2020 2020 6172 6961 2d68 6964 6465 6e3d      aria-hidden=
-00007970: 5c22 7472 7565 5c22 3e5c 725c 6e5c 743c  \"true\">\r\n\t<
-00007980: 6469 7620 636c 6173 733d 5c22 6d6f 6461  div class=\"moda
-00007990: 6c2d 6469 616c 6f67 5c22 3e5c 725c 6e5c  l-dialog\">\r\n\
-000079a0: 745c 743c 6469 7620 636c 6173 733d 5c22  t\t<div class=\"
-000079b0: 6d6f 6461 6c2d 636f 6e74 656e 745c 223e  modal-content\">
-000079c0: 5c72 5c6e 5c74 5c74 5c74 3c64 6976 0a20  \r\n\t\t\t<div. 
-000079d0: 2020 2020 2020 2063 6c61 7373 3d5c 226d         class=\"m
-000079e0: 6f64 616c 2d62 6f64 795c 223e 5c72 5c6e  odal-body\">\r\n
-000079f0: 5c74 5c74 5c74 5c74 3c64 6976 2063 6c61  \t\t\t\t<div cla
-00007a00: 7373 3d5c 2270 6167 652d 6865 6164 6572  ss=\"page-header
-00007a10: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
-00007a20: 745c 725c 6e5c 745c 745c 745c 745c 743c  t\r\n\t\t\t\t\t<
-00007a30: 6275 7474 6f6e 0a20 2020 2020 2020 2063  button.        c
-00007a40: 6c61 7373 3d5c 2270 756c 6c2d 7269 6768  lass=\"pull-righ
-00007a50: 7420 6274 6e2d 6469 736d 6973 735c 2220  t btn-dismiss\" 
-00007a60: 6172 6961 2d6c 6162 656c 3d5c 2253 756c  aria-label=\"Sul
-00007a70: 6a65 5c22 2064 6174 612d 6163 7469 6f6e  je\" data-action
-00007a80: 3d5c 2263 616e 6365 6c2d 616c 6c5c 223e  =\"cancel-all\">
-00007a90: 3c2f 6275 7474 6f6e 3e5c 725c 6e0a 2020  </button>\r\n.  
-00007aa0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-00007ab0: 2020 2020 2020 2020 2020 3c68 313e 5469            <h1>Ti
-00007ac0: 6c61 6120 796c 696d 5c78 4534 5c78 4534  laa ylim\xE4\xE4
-00007ad0: 725c 7845 3469 6e65 6e20 7479 686a 656e  r\xE4inen tyhjen
-00007ae0: 6e79 733c 2f68 313e 5c72 5c6e 5c74 5c74  nys</h1>\r\n\t\t
-00007af0: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-00007b00: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
-00007b10: 2020 2063 6c61 7373 3d5c 2266 6f72 6d5c     class=\"form\
-00007b20: 223e 3c2f 6469 763e 5c72 5c6e 5c74 5c74  "></div>\r\n\t\t
-00007b30: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
-00007b40: 2267 6c6f 6261 6c2d 7661 6c69 6461 7469  "global-validati
-00007b50: 6f6e 2d65 7272 6f72 2061 6c65 7274 0a20  on-error alert. 
-00007b60: 2020 2020 2020 2061 6c65 7274 2d64 616e         alert-dan
-00007b70: 6765 725c 2220 7374 796c 653d 5c22 6469  ger\" style=\"di
-00007b80: 7370 6c61 793a 6e6f 6e65 5c22 3e5c 725c  splay:none\">\r\
-00007b90: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00007ba0: 2020 2020 2054 5c78 4534 7974 5c78 4534       T\xE4yt\xE4
-00007bb0: 0a20 2020 2020 2020 2070 7575 7474 7576  .        puuttuv
-00007bc0: 6174 206b 656e 745c 7845 3474 5c72 5c6e  at kent\xE4t\r\n
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
-00007bf0: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 3c2f  </div>\r\n\t\t</
-00007c00: 6469 763e 5c72 5c6e 5c74 3c2f 6469 763e  div>\r\n\t</div>
-00007c10: 5c72 5c6e 3c2f 6469 763e 5c72 5c6e 5c72  \r\n</div>\r\n\r
-00007c20: 5c6e 5c72 5c6e 5c72 5c6e 3c64 6976 0a20  \n\r\n\r\n<div. 
-00007c30: 2020 2020 2020 2069 643d 5c22 6372 6561         id=\"crea
-00007c40: 7465 2d6e 6577 2d75 7365 722d 6d6f 6461  te-new-user-moda
-00007c50: 6c5c 2220 636c 6173 733d 5c22 6d6f 6461  l\" class=\"moda
-00007c60: 6c5c 2220 7374 796c 653d 5c22 6469 7370  l\" style=\"disp
-00007c70: 6c61 793a 6e6f 6e65 5c22 3e5c 725c 6e5c  lay:none\">\r\n\
-00007c80: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
-00007c90: 6173 733d 5c22 6d6f 6461 6c2d 6469 616c  ass=\"modal-dial
-00007ca0: 6f67 5c22 3e5c 725c 6e5c 745c 743c 6469  og\">\r\n\t\t<di
-00007cb0: 7620 636c 6173 733d 5c22 6d6f 6461 6c2d  v class=\"modal-
-00007cc0: 636f 6e74 656e 745c 223e 5c72 5c6e 5c74  content\">\r\n\t
-00007cd0: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-00007ce0: 2063 6c61 7373 3d5c 226d 6f64 616c 2d62   class=\"modal-b
-00007cf0: 6f64 795c 223e 5c72 5c6e 5c74 5c74 5c74  ody\">\r\n\t\t\t
-00007d00: 5c74 3c64 6976 2063 6c61 7373 3d5c 2270  \t<div class=\"p
-00007d10: 6167 652d 6865 6164 6572 5c22 3e5c 725c  age-header\">\r\
-00007d20: 6e5c 745c 745c 745c 745c 745c 725c 6e5c  n\t\t\t\t\t\r\n\
-00007d30: 745c 745c 745c 745c 743c 6831 3e4c 756f  t\t\t\t\t<h1>Luo
-00007d40: 0a20 2020 2020 2020 2075 7573 6920 7475  .        uusi tu
-00007d50: 6e6e 7573 3c2f 6831 3e5c 725c 6e5c 745c  nnus</h1>\r\n\t\
-00007d60: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
-00007d70: 725c 6e5c 745c 745c 745c 743c 6469 7620  r\n\t\t\t\t<div 
-00007d80: 636c 6173 733d 5c22 666f 726d 2066 6f72  class=\"form for
-00007d90: 6d43 6f6c 5c22 3e3c 2f64 6976 3e5c 725c  mCol\"></div>\r\
-00007da0: 6e5c 745c 745c 743c 2f64 6976 3e5c 725c  n\t\t\t</div>\r\
-00007db0: 6e5c 745c 743c 2f64 6976 3e5c 725c 6e5c  n\t\t</div>\r\n\
-00007dc0: 743c 2f64 6976 3e5c 725c 6e3c 2f64 6976  t</div>\r\n</div
-00007dd0: 3e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  >\r\n\r\n\r\n\r\
-00007de0: 6e3c 6469 760a 2020 2020 2020 2020 6964  n<div.        id
-00007df0: 3d5c 2265 6d61 696c 2d70 686f 6e65 2d6d  =\"email-phone-m
-00007e00: 6f64 616c 5c22 2063 6c61 7373 3d5c 226d  odal\" class=\"m
-00007e10: 6f64 616c 5c22 2073 7479 6c65 3d5c 2264  odal\" style=\"d
-00007e20: 6973 706c 6179 3a6e 6f6e 655c 223e 5c72  isplay:none\">\r
-00007e30: 5c6e 5c74 3c64 6976 0a20 2020 2020 2020  \n\t<div.       
-00007e40: 2063 6c61 7373 3d5c 226d 6f64 616c 2d64   class=\"modal-d
-00007e50: 6961 6c6f 675c 223e 5c72 5c6e 5c74 5c74  ialog\">\r\n\t\t
-00007e60: 3c64 6976 2063 6c61 7373 3d5c 226d 6f64  <div class=\"mod
-00007e70: 616c 2d63 6f6e 7465 6e74 5c22 3e5c 725c  al-content\">\r\
-00007e80: 6e5c 745c 745c 743c 6469 760a 2020 2020  n\t\t\t<div.    
-00007e90: 2020 2020 636c 6173 733d 5c22 6d6f 6461      class=\"moda
-00007ea0: 6c2d 626f 6479 5c22 3e5c 725c 6e5c 745c  l-body\">\r\n\t\
-00007eb0: 745c 745c 743c 6469 7620 636c 6173 733d  t\t\t<div class=
-00007ec0: 5c22 7061 6765 2d68 6561 6465 725c 223e  \"page-header\">
-00007ed0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c72  \r\n\t\t\t\t\t\r
-00007ee0: 5c6e 5c74 5c74 5c74 5c74 5c74 3c68 313e  \n\t\t\t\t\t<h1>
-00007ef0: 416e 6e61 0a20 2020 2020 2020 2073 5c78  Anna.        s\x
-00007f00: 4534 686b 5c78 4636 706f 7374 6920 6a61  E4hk\xF6posti ja
-00007f10: 2070 7568 656c 696e 6e75 6d65 726f 3c2f   puhelinnumero</
-00007f20: 6831 3e5c 725c 6e5c 745c 745c 745c 743c  h1>\r\n\t\t\t\t<
-00007f30: 2f64 6976 3e5c 725c 6e5c 725c 6e5c 745c  /div>\r\n\r\n\t\
-00007f40: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
-00007f50: 2020 636c 6173 733d 5c22 666f 726d 2066    class=\"form f
-00007f60: 6f72 6d43 6f6c 5c22 3e3c 2f64 6976 3e5c  ormCol\"></div>\
-00007f70: 725c 6e5c 745c 745c 743c 2f64 6976 3e5c  r\n\t\t\t</div>\
-00007f80: 725c 6e5c 745c 743c 2f64 6976 3e5c 725c  r\n\t\t</div>\r\
-00007f90: 6e5c 743c 2f64 6976 3e5c 725c 6e3c 2f64  n\t</div>\r\n</d
-00007fa0: 6976 3e5c 725c 6e5c 725c 6e5c 725c 6e5c  iv>\r\n\r\n\r\n\
-00007fb0: 725c 6e3c 6469 760a 2020 2020 2020 2020  r\n<div.        
-00007fc0: 6964 3d5c 2263 7265 6174 652d 6e65 772d  id=\"create-new-
-00007fd0: 7365 7276 6963 652d 6d6f 6461 6c5c 2220  service-modal\" 
-00007fe0: 636c 6173 733d 5c22 6d6f 6461 6c5c 2220  class=\"modal\" 
-00007ff0: 7374 796c 653d 5c22 6469 7370 6c61 793a  style=\"display:
-00008000: 6e6f 6e65 5c22 3e5c 725c 6e5c 743c 6469  none\">\r\n\t<di
-00008010: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
-00008020: 5c22 6d6f 6461 6c2d 6469 616c 6f67 206d  \"modal-dialog m
-00008030: 6f64 616c 2d6c 675c 223e 5c72 5c6e 5c74  odal-lg\">\r\n\t
-00008040: 5c74 3c64 6976 2063 6c61 7373 3d5c 226d  \t<div class=\"m
-00008050: 6f64 616c 2d63 6f6e 7465 6e74 5c22 3e5c  odal-content\">\
-00008060: 725c 6e5c 745c 745c 743c 6469 760a 2020  r\n\t\t\t<div.  
-00008070: 2020 2020 2020 636c 6173 733d 5c22 6d6f        class=\"mo
-00008080: 6461 6c2d 626f 6479 5c22 3e5c 725c 6e5c  dal-body\">\r\n\
-00008090: 745c 745c 745c 743c 6469 7620 636c 6173  t\t\t\t<div clas
-000080a0: 733d 5c22 7061 6765 2d68 6561 6465 725c  s=\"page-header\
-000080b0: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
-000080c0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c62  \r\n\t\t\t\t\t<b
-000080d0: 7574 746f 6e0a 2020 2020 2020 2020 636c  utton.        cl
-000080e0: 6173 733d 5c22 7075 6c6c 2d72 6967 6874  ass=\"pull-right
-000080f0: 2062 746e 2d64 6973 6d69 7373 5c22 2061   btn-dismiss\" a
-00008100: 7269 612d 6c61 6265 6c3d 5c22 5375 6c6a  ria-label=\"Sulj
-00008110: 655c 2220 6461 7461 2d61 6374 696f 6e3d  e\" data-action=
-00008120: 5c22 6361 6e63 656c 2d61 6c6c 5c22 3e3c  \"cancel-all\"><
-00008130: 2f62 7574 746f 6e3e 5c72 5c6e 0a20 2020  /button>\r\n.   
-00008140: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-00008150: 2020 2020 2020 2020 203c 6831 3e55 7564           <h1>Uud
-00008160: 656e 2070 616c 7665 6c75 6e20 7469 6c61  en palvelun tila
-00008170: 7573 3c2f 6831 3e5c 725c 6e5c 745c 745c  us</h1>\r\n\t\t\
-00008180: 745c 743c 2f64 6976 3e5c 725c 6e20 2020  t\t</div>\r\n   
-00008190: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
-000081a0: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-000081b0: 2020 2020 2020 2020 2020 3c68 333e 5479            <h3>Ty
-000081c0: 686a 656e 6e79 736b 6f68 6465 3c2f 6833  hjennyskohde</h3
-000081d0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-000081e0: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
-000081f0: 2020 2020 2020 2020 203c 6164 6472 6573           <addres
-00008200: 733e 5c72 5c6e 0a20 2020 2020 2020 205c  s>\r\n.        \
-00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008220: 2020 203c 7374 726f 6e67 3e3c 7370 616e     <strong><span
-00008230: 2064 6174 612d 726f 6c65 3d5c 226e 616d   data-role=\"nam
-00008240: 655c 223e 3c2f 7370 616e 3e3c 2f73 7472  e\"></span></str
-00008250: 6f6e 673e 3c62 723e 5c72 5c6e 0a20 2020  ong><br>\r\n.   
-00008260: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-00008270: 2020 2020 2020 2020 203c 7370 616e 2064           <span d
-00008280: 6174 612d 726f 6c65 3d5c 2261 6464 7265  ata-role=\"addre
-00008290: 7373 5c22 3e3c 2f73 7061 6e3e 3c62 723e  ss\"></span><br>
-000082a0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-000082b0: 2020 2020 2020 2020 3c73 7061 6e0a 2020          <span.  
-000082c0: 2020 2020 2020 6461 7461 2d72 6f6c 653d        data-role=
-000082d0: 5c22 706f 7374 5c22 3e3c 2f73 7061 6e3e  \"post\"></span>
-000082e0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-000082f0: 2020 2020 3c2f 6164 6472 6573 733e 5c72      </address>\r
-00008300: 5c6e 5c72 5c6e 5c74 5c74 5c74 5c74 3c64  \n\r\n\t\t\t\t<d
-00008310: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
-00008320: 3d5c 2266 6f72 6d5c 223e 3c2f 6469 763e  =\"form\"></div>
-00008330: 5c72 5c6e 5c72 5c6e 5c74 5c74 5c74 5c74  \r\n\r\n\t\t\t\t
-00008340: 3c64 6976 2063 6c61 7373 3d5c 2267 6c6f  <div class=\"glo
-00008350: 6261 6c2d 7661 6c69 6461 7469 6f6e 2d65  bal-validation-e
-00008360: 7272 6f72 0a20 2020 2020 2020 2061 6c65  rror.        ale
-00008370: 7274 2061 6c65 7274 2d64 616e 6765 725c  rt alert-danger\
-00008380: 2220 7374 796c 653d 5c22 6469 7370 6c61  " style=\"displa
-00008390: 793a 6e6f 6e65 5c22 3e5c 725c 6e5c 745c  y:none\">\r\n\t\
-000083a0: 7420 2020 205c 745c 7454 5c78 4534 7974  t    \t\tT\xE4yt
-000083b0: 5c78 4534 2070 7575 7474 7576 6174 0a20  \xE4 puuttuvat. 
-000083c0: 2020 2020 2020 206b 656e 745c 7845 3474         kent\xE4t
-000083d0: 5c72 5c6e 5c74 5c74 2020 2020 5c74 3c2f  \r\n\t\t    \t</
-000083e0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 3c2f  div>\r\n\t\t\t</
-000083f0: 6469 763e 5c72 5c6e 5c74 5c74 3c2f 6469  div>\r\n\t\t</di
-00008400: 763e 5c72 5c6e 5c74 3c2f 6469 763e 5c72  v>\r\n\t</div>\r
-00008410: 5c6e 3c2f 6469 763e 5c72 5c6e 5c72 5c6e  \n</div>\r\n\r\n
-00008420: 5c72 5c6e 5c72 5c6e 3c64 6976 0a20 2020  \r\n\r\n<div.   
-00008430: 2020 2020 2069 643d 5c22 6368 616e 6765       id=\"change
-00008440: 2d70 6173 7377 6f72 642d 6d6f 6461 6c5c  -password-modal\
-00008450: 2220 636c 6173 733d 5c22 6d6f 6461 6c5c  " class=\"modal\
-00008460: 2220 7374 796c 653d 5c22 6469 7370 6c61  " style=\"displa
-00008470: 793a 6e6f 6e65 5c22 3e5c 725c 6e5c 743c  y:none\">\r\n\t<
-00008480: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-00008490: 733d 5c22 6d6f 6461 6c2d 6469 616c 6f67  s=\"modal-dialog
-000084a0: 5c22 3e5c 725c 6e5c 745c 743c 6469 7620  \">\r\n\t\t<div 
-000084b0: 636c 6173 733d 5c22 6d6f 6461 6c2d 636f  class=\"modal-co
-000084c0: 6e74 656e 745c 223e 5c72 5c6e 5c74 5c74  ntent\">\r\n\t\t
-000084d0: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
-000084e0: 6c61 7373 3d5c 226d 6f64 616c 2d68 6561  lass=\"modal-hea
-000084f0: 6465 725c 223e 5c72 5c6e 5c74 5c74 5c74  der\">\r\n\t\t\t
-00008500: 5c74 5661 6968 6461 2073 616c 6173 616e  \tVaihda salasan
-00008510: 615c 725c 6e5c 745c 745c 743c 2f64 6976  a\r\n\t\t\t</div
-00008520: 3e5c 725c 6e5c 745c 745c 743c 6469 760a  >\r\n\t\t\t<div.
-00008530: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-00008540: 6d6f 6461 6c2d 626f 6479 5c22 3e5c 725c  modal-body\">\r\
-00008550: 6e5c 745c 745c 745c 743c 6469 7620 636c  n\t\t\t\t<div cl
-00008560: 6173 733d 5c22 666f 726d 2066 6f72 6d43  ass=\"form formC
-00008570: 6f6c 5c22 3e3c 2f64 6976 3e5c 725c 6e5c  ol\"></div>\r\n\
-00008580: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
-00008590: 745c 743c 2f64 6976 3e5c 725c 6e5c 743c  t\t</div>\r\n\t<
-000085a0: 2f64 6976 3e5c 725c 6e3c 2f64 6976 3e5c  /div>\r\n</div>\
-000085b0: 725c 6e5c 725c 6e5c 725c 6e5c 725c 6e3c  r\n\r\n\r\n\r\n<
-000085c0: 6469 760a 2020 2020 2020 2020 6964 3d5c  div.        id=\
-000085d0: 2263 6861 6e67 652d 7365 7276 6963 652d  "change-service-
-000085e0: 6d6f 6461 6c5c 2220 636c 6173 733d 5c22  modal\" class=\"
-000085f0: 6d6f 6461 6c5c 2220 7374 796c 653d 5c22  modal\" style=\"
-00008600: 6469 7370 6c61 793a 6e6f 6e65 5c22 3e5c  display:none\">\
-00008610: 725c 6e5c 743c 6469 760a 2020 2020 2020  r\n\t<div.      
-00008620: 2020 636c 6173 733d 5c22 6d6f 6461 6c2d    class=\"modal-
-00008630: 6469 616c 6f67 5c22 3e5c 725c 6e5c 745c  dialog\">\r\n\t\
-00008640: 743c 6469 7620 636c 6173 733d 5c22 6d6f  t<div class=\"mo
-00008650: 6461 6c2d 636f 6e74 656e 745c 223e 5c72  dal-content\">\r
-00008660: 5c6e 5c74 5c74 5c74 3c64 6976 0a20 2020  \n\t\t\t<div.   
-00008670: 2020 2020 2063 6c61 7373 3d5c 226d 6f64       class=\"mod
-00008680: 616c 2d62 6f64 795c 223e 5c72 5c6e 5c74  al-body\">\r\n\t
-00008690: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
-000086a0: 3d5c 2270 6167 652d 6865 6164 6572 5c22  =\"page-header\"
-000086b0: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-000086c0: 725c 6e5c 745c 745c 745c 745c 743c 6275  r\n\t\t\t\t\t<bu
-000086d0: 7474 6f6e 0a20 2020 2020 2020 2063 6c61  tton.        cla
-000086e0: 7373 3d5c 2270 756c 6c2d 7269 6768 7420  ss=\"pull-right 
-000086f0: 6274 6e2d 6469 736d 6973 735c 2220 6172  btn-dismiss\" ar
-00008700: 6961 2d6c 6162 656c 3d5c 2253 756c 6a65  ia-label=\"Sulje
-00008710: 5c22 2064 6174 612d 6163 7469 6f6e 3d5c  \" data-action=\
-00008720: 2263 616e 6365 6c2d 616c 6c5c 223e 3c2f  "cancel-all\"></
-00008730: 6275 7474 6f6e 3e5c 725c 6e0a 2020 2020  button>\r\n.    
-00008740: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-00008750: 2020 2020 2020 2020 3c68 313e 5061 6c76          <h1>Palv
-00008760: 656c 756d 7575 746f 733c 2f68 313e 5c72  elumuutos</h1>\r
-00008770: 5c6e 5c74 5c74 5c74 5c74 3c2f 6469 763e  \n\t\t\t\t</div>
-00008780: 5c72 5c6e 5c74 5c74 5c74 5c74 3c64 6976  \r\n\t\t\t\t<div
-00008790: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
-000087a0: 2266 6f72 6d5c 223e 3c2f 6469 763e 5c72  "form\"></div>\r
-000087b0: 5c6e 5c74 5c74 5c74 5c74 3c64 6976 2063  \n\t\t\t\t<div c
-000087c0: 6c61 7373 3d5c 2267 6c6f 6261 6c2d 7661  lass=\"global-va
-000087d0: 6c69 6461 7469 6f6e 2d65 7272 6f72 2061  lidation-error a
-000087e0: 6c65 7274 0a20 2020 2020 2020 2061 6c65  lert.        ale
-000087f0: 7274 2d64 616e 6765 725c 2220 7374 796c  rt-danger\" styl
-00008800: 653d 5c22 6469 7370 6c61 793a 6e6f 6e65  e=\"display:none
-00008810: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
-00008820: 2020 2020 2020 2020 2020 2054 5c78 4534             T\xE4
-00008830: 7974 5c78 4534 0a20 2020 2020 2020 2070  yt\xE4.        p
-00008840: 7575 7474 7576 6174 206b 656e 745c 7845  uuttuvat kent\xE
-00008850: 3474 5c72 5c6e 2020 2020 2020 2020 2020  4t\r\n          
-00008860: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
-00008870: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
-00008880: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-00008890: 3c2f 6469 763e 5c72 5c6e 3c2f 6469 763e  </div>\r\n</div>
-000088a0: 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e  \r\n\r\n\r\n\r\n
-000088b0: 3c64 6976 0a20 2020 2020 2020 2069 643d  <div.        id=
-000088c0: 5c22 6372 6561 7465 2d6b 696d 7070 612d  \"create-kimppa-
-000088d0: 6d6f 6461 6c5c 2220 636c 6173 733d 5c22  modal\" class=\"
-000088e0: 6d6f 6461 6c5c 2220 7374 796c 653d 5c22  modal\" style=\"
-000088f0: 6469 7370 6c61 793a 6e6f 6e65 5c22 3e5c  display:none\">\
-00008900: 725c 6e5c 743c 6469 760a 2020 2020 2020  r\n\t<div.      
-00008910: 2020 636c 6173 733d 5c22 6d6f 6461 6c2d    class=\"modal-
-00008920: 6469 616c 6f67 206d 6f64 616c 2d6c 675c  dialog modal-lg\
-00008930: 223e 5c72 5c6e 5c74 5c74 3c64 6976 2063  ">\r\n\t\t<div c
-00008940: 6c61 7373 3d5c 226d 6f64 616c 2d63 6f6e  lass=\"modal-con
-00008950: 7465 6e74 5c22 3e5c 725c 6e5c 745c 745c  tent\">\r\n\t\t\
-00008960: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
-00008970: 6173 733d 5c22 6d6f 6461 6c2d 626f 6479  ass=\"modal-body
-00008980: 5c22 3e5c 725c 6e5c 745c 745c 745c 743c  \">\r\n\t\t\t\t<
-00008990: 6469 7620 636c 6173 733d 5c22 7061 6765  div class=\"page
-000089a0: 2d68 6561 6465 725c 223e 5c72 5c6e 5c74  -header\">\r\n\t
-000089b0: 5c74 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \t\t\t\t\r\n\t\t
-000089c0: 5c74 5c74 5c74 3c62 7574 746f 6e0a 2020  \t\t\t<button.  
-000089d0: 2020 2020 2020 636c 6173 733d 5c22 7075        class=\"pu
-000089e0: 6c6c 2d72 6967 6874 2062 746e 2d64 6973  ll-right btn-dis
-000089f0: 6d69 7373 5c22 2061 7269 612d 6c61 6265  miss\" aria-labe
-00008a00: 6c3d 5c22 5375 6c6a 655c 2220 6461 7461  l=\"Sulje\" data
-00008a10: 2d61 6374 696f 6e3d 5c22 6361 6e63 656c  -action=\"cancel
-00008a20: 2d61 6c6c 5c22 3e3c 2f62 7574 746f 6e3e  -all\"></button>
-00008a30: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c68  \r\n\t\t\t\t\t<h
-00008a40: 313e 5061 6c76 656c 7573 7461 0a20 2020  1>Palvelusta.   
-00008a50: 2020 2020 206b 696d 7061 6b73 693c 2f68       kimpaksi</h
-00008a60: 313e 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f  1>\r\n\t\t\t\t</
-00008a70: 6469 763e 5c72 5c6e 5c72 5c6e 5c74 5c74  div>\r\n\r\n\t\t
-00008a80: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
-00008a90: 2274 6578 742d 7269 6768 745c 223e 5c72  "text-right\">\r
-00008aa0: 5c6e 5c74 5c74 5c74 5c74 5c74 3c62 7574  \n\t\t\t\t\t<but
-00008ab0: 746f 6e0a 2020 2020 2020 2020 636c 6173  ton.        clas
-00008ac0: 733d 5c22 6274 6e20 6274 6e2d 6c69 6e6b  s=\"btn btn-link
-00008ad0: 5c22 2064 6174 612d 6163 7469 6f6e 3d5c  \" data-action=\
-00008ae0: 2270 7269 6e74 5c22 3e54 756c 6f73 7461  "print\">Tulosta
-00008af0: 206b 696d 7070 616c 7565 7474 656c 6f20   kimppaluettelo 
-00008b00: 3c73 7061 6e0a 2020 2020 2020 2020 636c  <span.        cl
-00008b10: 6173 733d 5c22 676c 7970 6869 636f 6e20  ass=\"glyphicon 
-00008b20: 676c 7970 6869 636f 6e2d 7072 696e 745c  glyphicon-print\
-00008b30: 223e 3c2f 7370 616e 3e3c 2f62 7574 746f  "></span></butto
-00008b40: 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f  n>\r\n\t\t\t\t</
-00008b50: 6469 763e 5c72 5c6e 5c72 5c6e 5c74 5c74  div>\r\n\r\n\t\t
-00008b60: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-00008b70: 2063 6c61 7373 3d5c 226b 696d 7070 615c   class=\"kimppa\
-00008b80: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
-00008b90: 3c73 7479 6c65 2073 636f 7065 643e 5c72  <style scoped>\r
-00008ba0: 5c6e 5c74 5c74 5c74 5c74 5c74 2e6b 696d  \n\t\t\t\t\t.kim
-00008bb0: 7070 6120 7370 616e 2e69 7361 6e74 613a  ppa span.isanta:
-00008bc0: 6265 666f 7265 0a20 2020 2020 2020 207b  before.        {
-00008bd0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-00008be0: 636f 6e74 656e 743a 2027 4b69 6d70 7061  content: 'Kimppa
-00008bf0: 6973 5c78 4534 6e74 5c78 4534 273b 5c72  is\xE4nt\xE4';\r
-00008c00: 5c6e 5c74 5c74 5c74 5c74 5c74 7d5c 725c  \n\t\t\t\t\t}\r\
-00008c10: 6e5c 745c 745c 745c 745c 743c 2f73 7479  n\t\t\t\t\t</sty
-00008c20: 6c65 3e5c 725c 6e5c 745c 745c 745c 745c  le>\r\n\t\t\t\t\
-00008c30: 745c 725c 6e5c 745c 745c 745c 745c 743c  t\r\n\t\t\t\t\t<
-00008c40: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-00008c50: 733d 5c22 6772 6964 5c22 3e3c 2f64 6976  s=\"grid\"></div
-00008c60: 3e5c 725c 6e5c 725c 6e5c 745c 745c 745c  >\r\n\r\n\t\t\t\
-00008c70: 745c 743c 7363 7269 7074 2069 643d 5c22  t\t<script id=\"
-00008c80: 6b69 6d70 7061 2d65 6469 742d 6d65 6e75  kimppa-edit-menu
-00008c90: 2d74 656d 706c 6174 655c 220a 2020 2020  -template\".    
-00008ca0: 2020 2020 7479 7065 3d5c 2274 6578 742f      type=\"text/
-00008cb0: 782d 7465 6d70 6c61 7465 5c22 3e5c 725c  x-template\">\r\
-00008cc0: 6e5c 745c 745c 745c 745c 743c 6469 7620  n\t\t\t\t\t<div 
-00008cd0: 636c 6173 733d 5c22 6d65 6e75 2065 6469  class=\"menu edi
-00008ce0: 742d 6d65 6e75 5c22 2064 6174 612d 726f  t-menu\" data-ro
-00008cf0: 6c65 3d5c 2265 6469 742d 6d65 6e75 5c22  le=\"edit-menu\"
-00008d00: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-00008d10: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
-00008d20: 6173 733d 5c22 726f 775c 223e 5c72 5c6e  ass=\"row\">\r\n
-00008d30: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c64  \t\t\t\t\t\t\t<d
-00008d40: 6976 2063 6c61 7373 3d5c 2263 6f6c 2d78  iv class=\"col-x
-00008d50: 732d 345c 223e 3c62 7574 746f 6e20 7479  s-4\"><button ty
-00008d60: 7065 3d5c 2262 7574 746f 6e5c 220a 2020  pe=\"button\".  
-00008d70: 2020 2020 2020 6461 7461 2d61 6374 696f        data-actio
-00008d80: 6e3d 5c22 6564 6974 2d6f 7361 6b61 735c  n=\"edit-osakas\
-00008d90: 2220 636c 6173 733d 5c22 6274 6e20 6274  " class=\"btn bt
-00008da0: 6e2d 7072 696d 6172 7920 6274 6e2d 626c  n-primary btn-bl
-00008db0: 6f63 6b5c 223e 5c72 5c6e 5c74 5c74 5c74  ock\">\r\n\t\t\t
-00008dc0: 5c74 5c74 5c74 5c74 5c74 4d75 6f6b 6b61  \t\t\t\t\tMuokka
-00008dd0: 615c 725c 6e5c 745c 745c 745c 745c 745c  a\r\n\t\t\t\t\t\
-00008de0: 745c 743c 2f62 7574 746f 6e3e 3c2f 6469  t\t</button></di
-00008df0: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  v>\r\n\t\t\t\t\t
-00008e00: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-00008e10: 2063 6c61 7373 3d5c 2263 6f6c 2d78 732d   class=\"col-xs-
-00008e20: 345c 223e 3c62 7574 746f 6e20 7479 7065  4\"><button type
-00008e30: 3d5c 2262 7574 746f 6e5c 2220 6461 7461  =\"button\" data
-00008e40: 2d61 6374 696f 6e3d 5c22 636c 6f73 652d  -action=\"close-
-00008e50: 6d65 6e75 5c22 2063 6c61 7373 3d5c 2262  menu\" class=\"b
-00008e60: 746e 0a20 2020 2020 2020 2062 746e 2d70  tn.        btn-p
-00008e70: 7269 6d61 7279 2062 746e 2d62 6c6f 636b  rimary btn-block
-00008e80: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
-00008e90: 745c 745c 745c 7450 6572 7575 7461 5c72  t\t\t\tPeruuta\r
-00008ea0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-00008eb0: 3c2f 6275 7474 6f6e 3e3c 2f64 6976 3e5c  </button></div>\
-00008ec0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
-00008ed0: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
-00008ee0: 6173 733d 5c22 636f 6c2d 7873 2d34 5c22  ass=\"col-xs-4\"
-00008ef0: 3e3c 6275 7474 6f6e 2074 7970 653d 5c22  ><button type=\"
-00008f00: 6275 7474 6f6e 5c22 2064 6174 612d 6163  button\" data-ac
-00008f10: 7469 6f6e 3d5c 2264 656c 6574 652d 726f  tion=\"delete-ro
-00008f20: 775c 2220 636c 6173 733d 5c22 6274 6e0a  w\" class=\"btn.
-00008f30: 2020 2020 2020 2020 6274 6e2d 7072 696d          btn-prim
-00008f40: 6172 7920 6274 6e2d 626c 6f63 6b5c 223e  ary btn-block\">
-00008f50: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-00008f60: 5c74 5c74 506f 6973 7461 5c72 5c6e 5c74  \t\tPoista\r\n\t
-00008f70: 5c74 5c74 5c74 5c74 5c74 5c74 3c2f 6275  \t\t\t\t\t\t</bu
-00008f80: 7474 6f6e 3e3c 2f64 6976 3e5c 725c 6e5c  tton></div>\r\n\
-00008f90: 745c 745c 745c 745c 745c 743c 2f64 6976  t\t\t\t\t\t</div
-00008fa0: 3e5c 725c 6e5c 745c 745c 745c 745c 743c  >\r\n\t\t\t\t\t<
-00008fb0: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
-00008fc0: 745c 743c 2f73 6372 6970 743e 5c72 5c6e  t\t</script>\r\n
-00008fd0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c73  \r\n\t\t\t\t\t<s
-00008fe0: 6372 6970 740a 2020 2020 2020 2020 6964  cript.        id
-00008ff0: 3d5c 226b 696d 7070 612d 7061 696e 6f2d  =\"kimppa-paino-
-00009000: 6d65 6e75 2d74 656d 706c 6174 655c 2220  menu-template\" 
-00009010: 7479 7065 3d5c 2274 6578 742f 782d 7465  type=\"text/x-te
-00009020: 6d70 6c61 7465 5c22 3e5c 725c 6e5c 745c  mplate\">\r\n\t\
-00009030: 745c 745c 745c 743c 6469 760a 2020 2020  t\t\t\t<div.    
-00009040: 2020 2020 636c 6173 733d 5c22 6d65 6e75      class=\"menu
-00009050: 2070 6169 6e6f 2d6d 656e 755c 2220 6461   paino-menu\" da
-00009060: 7461 2d72 6f6c 653d 5c22 7061 696e 6f2d  ta-role=\"paino-
-00009070: 6d65 6e75 5c22 3e5c 725c 6e5c 745c 745c  menu\">\r\n\t\t\
-00009080: 745c 745c 745c 743c 6469 7620 636c 6173  t\t\t\t<div clas
-00009090: 733d 5c22 726f 770a 2020 2020 2020 2020  s=\"row.        
-000090a0: 726f 772d 6365 6e74 6572 6564 5c22 3e5c  row-centered\">\
-000090b0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
-000090c0: 743c 6469 7620 636c 6173 733d 5c22 636f  t<div class=\"co
-000090d0: 6c2d 7873 2d34 2063 6f6c 2d63 656e 7465  l-xs-4 col-cente
-000090e0: 7265 645c 223e 3c62 7574 746f 6e0a 2020  red\"><button.  
-000090f0: 2020 2020 2020 7479 7065 3d5c 2262 7574        type=\"but
-00009100: 746f 6e5c 2220 6461 7461 2d61 6374 696f  ton\" data-actio
-00009110: 6e3d 5c22 7365 742d 7061 696e 6f5c 2220  n=\"set-paino\" 
-00009120: 6461 7461 2d76 616c 7565 3d5c 2230 5c22  data-value=\"0\"
-00009130: 2063 6c61 7373 3d5c 2262 746e 2062 746e   class=\"btn btn
-00009140: 2d70 7269 6d61 7279 0a20 2020 2020 2020  -primary.       
-00009150: 2062 746e 2d62 6c6f 636b 5c22 3e5c 725c   btn-block\">\r\
-00009160: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
-00009170: 7445 6920 6c61 736b 7574 6574 615c 725c  tEi laskuteta\r\
-00009180: 6e5c 745c 745c 745c 745c 745c 745c 743c  n\t\t\t\t\t\t\t<
-00009190: 2f62 7574 746f 6e3e 3c2f 6469 763e 5c72  /button></div>\r
-000091a0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-000091b0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-000091c0: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
-000091d0: 6c61 7373 3d5c 2263 6f6c 2d78 732d 3420  lass=\"col-xs-4 
-000091e0: 636f 6c2d 6365 6e74 6572 6564 5c22 3e3c  col-centered\"><
-000091f0: 6275 7474 6f6e 2074 7970 653d 5c22 6275  button type=\"bu
-00009200: 7474 6f6e 5c22 2064 6174 612d 6163 7469  tton\" data-acti
-00009210: 6f6e 3d5c 2273 6574 2d70 6169 6e6f 5c22  on=\"set-paino\"
-00009220: 0a20 2020 2020 2020 2064 6174 612d 7661  .        data-va
-00009230: 6c75 653d 5c22 325c 2220 636c 6173 733d  lue=\"2\" class=
-00009240: 5c22 6274 6e20 6274 6e2d 7072 696d 6172  \"btn btn-primar
-00009250: 7920 6274 6e2d 626c 6f63 6b5c 223e 5c72  y btn-block\">\r
-00009260: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-00009270: 5c74 5661 6b69 7475 6973 656e 0a20 2020  \tVakituisen.   
-00009280: 2020 2020 206d 756b 6169 7365 7374 695c       mukaisesti\
-00009290: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
-000092a0: 743c 2f62 7574 746f 6e3e 3c2f 6469 763e  t</button></div>
-000092b0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-000092c0: 5c74 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  \t\r\n\t\t\t\t\t
-000092d0: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-000092e0: 2063 6c61 7373 3d5c 2263 6f6c 2d78 732d   class=\"col-xs-
-000092f0: 3420 636f 6c2d 6365 6e74 6572 6564 5c22  4 col-centered\"
-00009300: 3e3c 6275 7474 6f6e 2074 7970 653d 5c22  ><button type=\"
-00009310: 6275 7474 6f6e 5c22 2064 6174 612d 6163  button\" data-ac
-00009320: 7469 6f6e 3d5c 2273 6574 2d70 6169 6e6f  tion=\"set-paino
-00009330: 5c22 0a20 2020 2020 2020 2064 6174 612d  \".        data-
-00009340: 7661 6c75 653d 5c22 315c 2220 636c 6173  value=\"1\" clas
-00009350: 733d 5c22 6274 6e20 6274 6e2d 7072 696d  s=\"btn btn-prim
-00009360: 6172 7920 6274 6e2d 626c 6f63 6b5c 223e  ary btn-block\">
-00009370: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-00009380: 5c74 5c74 5661 7061 612d 616a 616e 0a20  \t\tVapaa-ajan. 
-00009390: 2020 2020 2020 206d 756b 6169 7365 7374         mukaisest
-000093a0: 695c 725c 6e5c 745c 745c 745c 745c 745c  i\r\n\t\t\t\t\t\
-000093b0: 745c 743c 2f62 7574 746f 6e3e 3c2f 6469  t\t</button></di
-000093c0: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  v>\r\n\t\t\t\t\t
-000093d0: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
-000093e0: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
-000093f0: 5c74 5c74 5c74 5c74 5c74 3c2f 7363 7269  \t\t\t\t\t</scri
-00009400: 7074 3e5c 725c 6e5c 725c 6e5c 745c 745c  pt>\r\n\r\n\t\t\
-00009410: 745c 745c 743c 703e 4c61 736b 7574 7573  t\t\t<p>Laskutus
-00009420: 6f73 7575 6b73 6965 6e0a 2020 2020 2020  osuuksien.      
-00009430: 2020 7375 6d6d 6120 745c 7845 3479 7479    summa t\xE4yty
-00009440: 7920 6f6c 6c61 2031 3030 2025 2e20 566f  y olla 100 %. Vo
-00009450: 6974 206a 616b 6161 206b 696d 7061 6e20  it jakaa kimpan 
-00009460: 6c61 736b 7574 7573 6f73 7575 6465 7420  laskutusosuudet 
-00009470: 6175 746f 6d61 6174 7469 7365 7374 690a  automaattisesti.
-00009480: 2020 2020 2020 2020 616c 6c61 206f 6c65          alla ole
-00009490: 7661 6c6c 6120 7061 696e 696b 6b65 656c  valla painikkeel
-000094a0: 6c61 2c20 6a6f 6c6c 6f69 6e20 6c61 736b  la, jolloin lask
-000094b0: 7574 7573 6f73 7575 6465 7420 6a61 6574  utusosuudet jaet
-000094c0: 6161 6e20 6b69 696e 7465 6973 745c 7846  aan kiinteist\xF
-000094d0: 366e 0a20 2020 2020 2020 206b 5c78 4534  6n.        k\xE4
-000094e0: 7974 745c 7846 3674 6172 6b6f 6974 756b  ytt\xF6tarkoituk
-000094f0: 7365 6e20 6d75 6b61 616e 2e20 566f 6974  sen mukaan. Voit
-00009500: 206d 795c 7846 3673 2068 616c 7574 6573   my\xF6s halutes
-00009510: 7361 7369 2073 795c 7846 3674 745c 7845  sasi sy\xF6tt\xE
-00009520: 345c 7845 340a 2020 2020 2020 2020 6c61  4\xE4.        la
-00009530: 736b 7574 7573 6f73 7575 6465 7420 6b5c  skutusosuudet k\
-00009540: 7845 3473 696e 2079 6c6c 5c78 4534 6f6c  xE4sin yll\xE4ol
-00009550: 6576 6969 6e20 6b65 6e74 7469 696e 2e3c  eviin kenttiin.<
-00009560: 2f70 3e5c 725c 6e5c 725c 6e5c 745c 745c  /p>\r\n\r\n\t\t\
-00009570: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
-00009580: 2020 636c 6173 733d 5c22 7465 7874 2d63    class=\"text-c
-00009590: 656e 7465 725c 223e 5c72 5c6e 5c74 5c74  enter\">\r\n\t\t
-000095a0: 5c74 5c74 5c74 5c74 3c62 7574 746f 6e20  \t\t\t\t<button 
-000095b0: 7479 7065 3d5c 2262 7574 746f 6e5c 2220  type=\"button\" 
-000095c0: 636c 6173 733d 5c22 6274 6e0a 2020 2020  class=\"btn.    
-000095d0: 2020 2020 6274 6e2d 6465 6661 756c 745c      btn-default\
-000095e0: 2220 6461 7461 2d61 6374 696f 6e3d 5c22  " data-action=\"
-000095f0: 6469 7374 7269 6275 7465 2d65 7665 6e6c  distribute-evenl
-00009600: 795c 223e 4a61 6120 6c61 736b 7574 7573  y\">Jaa laskutus
-00009610: 2d25 2074 6173 616e 3c2f 6275 7474 6f6e  -% tasan</button
-00009620: 3e5c 725c 6e5c 745c 745c 745c 745c 743c  >\r\n\t\t\t\t\t<
-00009630: 2f64 6976 3e5c 725c 6e5c 725c 6e5c 745c  /div>\r\n\r\n\t\
-00009640: 745c 745c 745c 743c 6469 760a 2020 2020  t\t\t\t<div.    
-00009650: 2020 2020 636c 6173 733d 5c22 666f 726d      class=\"form
-00009660: 2d67 726f 7570 5c22 3e5c 725c 6e5c 745c  -group\">\r\n\t\
-00009670: 745c 745c 745c 745c 743c 6c61 6265 6c20  t\t\t\t\t<label 
-00009680: 666f 723d 5c22 4b49 4d43 6f6d 6d5c 223e  for=\"KIMComm\">
-00009690: 4d75 7574 6f6b 7365 6e20 7379 793c 2f6c  Muutoksen syy</l
-000096a0: 6162 656c 3e5c 725c 6e5c 745c 745c 745c  abel>\r\n\t\t\t\
-000096b0: 745c 745c 743c 7465 7874 6172 6561 0a20  t\t\t<textarea. 
-000096c0: 2020 2020 2020 2069 643d 5c22 4b49 4d43         id=\"KIMC
-000096d0: 6f6d 6d5c 2220 6e61 6d65 3d5c 224b 494d  omm\" name=\"KIM
-000096e0: 436f 6d6d 5c22 2063 6c61 7373 3d5c 2266  Comm\" class=\"f
-000096f0: 6f72 6d2d 636f 6e74 726f 6c5c 223e 3c2f  orm-control\"></
-00009700: 7465 7874 6172 6561 3e5c 725c 6e5c 745c  textarea>\r\n\t\
-00009710: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
-00009720: 6e5c 725c 6e5c 745c 745c 745c 745c 743c  n\r\n\t\t\t\t\t<
-00009730: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-00009740: 733d 5c22 666f 726d 2d67 726f 7570 205c  s=\"form-group \
-00009750: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
-00009760: 5c74 3c6c 6162 656c 2066 6f72 3d5c 224b  \t<label for=\"K
-00009770: 4952 5076 6d5c 223e 4d75 7574 6f6b 7365  IRPvm\">Muutokse
-00009780: 7420 7475 6c65 7661 740a 2020 2020 2020  t tulevat.      
-00009790: 2020 766f 696d 6161 6e3c 2f6c 6162 656c    voimaan</label
-000097a0: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-000097b0: 743c 696e 7075 7420 6e61 6d65 3d5c 224b  t<input name=\"K
-000097c0: 4952 5076 6d5c 2220 636c 6173 733d 5c22  IRPvm\" class=\"
-000097d0: 666f 726d 2d63 6f6e 7472 6f6c 5c22 0a20  form-control\". 
-000097e0: 2020 2020 2020 203e 5c72 5c6e 5c74 5c74         >\r\n\t\t
-000097f0: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
-00009800: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00009810: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00009820: 7373 3d5c 2266 6f72 6d2d 6772 6f75 705c  ss=\"form-group\
-00009830: 223e 5c72 5c6e 0a20 2020 2020 2020 205c  ">\r\n.        \
-00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009850: 2020 2020 2020 203c 6c61 6265 6c20 666f         <label fo
-00009860: 723d 5c22 6e6f 7469 6669 6572 7068 6f6e  r=\"notifierphon
-00009870: 655c 223e 496c 6d6f 6974 7461 6a61 6e20  e\">Ilmoittajan 
-00009880: 7075 6865 6c69 6e6e 756d 6572 6f3c 2f6c  puhelinnumero</l
-00009890: 6162 656c 3e5c 725c 6e0a 2020 2020 2020  abel>\r\n.      
-000098a0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-000098b0: 2020 2020 2020 2020 2020 3c69 6e70 7574            <input
-000098c0: 206e 616d 653d 5c22 6e6f 7469 6669 6572   name=\"notifier
-000098d0: 7068 6f6e 655c 2220 7479 7065 3d5c 2274  phone\" type=\"t
-000098e0: 656c 5c22 2063 6c61 7373 3d5c 2266 6f72  el\" class=\"for
-000098f0: 6d2d 636f 6e74 726f 6c5c 220a 2020 2020  m-control\".    
-00009900: 2020 2020 7061 7474 6572 6e3d 5c22 5e5c      pattern=\"^\
-00009910: 5c73 2a5c 5c2b 3f28 5c5c 647c 5c5c 737c  \s*\\+?(\\d|\\s|
-00009920: 2d29 2b24 5c22 2070 6c61 6365 686f 6c64  -)+$\" placehold
-00009930: 6572 3d5c 225c 223e 5c72 5c6e 2020 2020  er=\"\">\r\n    
-00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 0a20  </div>\r\n\r\n. 
-00009960: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-00009970: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00009980: 636c 6173 733d 5c22 666f 726d 2d67 726f  class=\"form-gro
-00009990: 7570 5c22 3e5c 725c 6e20 2020 2020 2020  up\">\r\n       
-000099a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099b0: 203c 6c61 6265 6c0a 2020 2020 2020 2020   <label.        
-000099c0: 666f 723d 5c22 6e6f 7469 6669 6572 656d  for=\"notifierem
-000099d0: 6169 6c5c 223e 496c 6d6f 6974 7461 6a61  ail\">Ilmoittaja
-000099e0: 6e20 735c 7845 3468 6b5c 7846 3670 6f73  n s\xE4hk\xF6pos
-000099f0: 7469 6f73 6f69 7465 3c2f 6c61 6265 6c3e  tiosoite</label>
-00009a00: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00009a10: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
-00009a20: 7574 0a20 2020 2020 2020 206e 616d 653d  ut.        name=
-00009a30: 5c22 6e6f 7469 6669 6572 656d 6169 6c5c  \"notifieremail\
-00009a40: 2220 7479 7065 3d5c 2265 6d61 696c 5c22  " type=\"email\"
-00009a50: 2063 6c61 7373 3d5c 2266 6f72 6d2d 636f   class=\"form-co
-00009a60: 6e74 726f 6c5c 223e 5c72 5c6e 2020 2020  ntrol\">\r\n    
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
-00009a90: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
-00009aa0: 5c74 3c2f 6469 763e 5c72 5c6e 5c72 5c6e  \t</div>\r\n\r\n
-00009ab0: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
-00009ac0: 2020 2063 6c61 7373 3d5c 226d 6f64 616c     class=\"modal
-00009ad0: 2d66 6f6f 7465 725c 223e 5c72 5c6e 5c74  -footer\">\r\n\t
-00009ae0: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
-00009af0: 3d5c 2266 6f72 6d2d 6772 6f75 705c 223e  =\"form-group\">
-00009b00: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c64  \r\n\t\t\t\t\t<d
-00009b10: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
-00009b20: 3d5c 2263 6865 636b 626f 7820 7465 7874  =\"checkbox text
-00009b30: 2d6c 6566 745c 223e 5c72 5c6e 5c74 5c74  -left\">\r\n\t\t
-00009b40: 5c74 5c74 5c74 5c74 3c6c 6162 656c 3e3c  \t\t\t\t<label><
-00009b50: 696e 7075 7420 7479 7065 3d5c 2263 6865  input type=\"che
-00009b60: 636b 626f 785c 220a 2020 2020 2020 2020  ckbox\".        
-00009b70: 6e61 6d65 3d5c 2263 6f6e 6669 726d 2d63  name=\"confirm-c
-00009b80: 6861 6e67 6573 5c22 3e20 4f6c 656e 2074  hanges\"> Olen t
-00009b90: 6172 6b69 7374 616e 7574 206b 696d 7061  arkistanut kimpa
-00009ba0: 6e20 6c61 736b 7574 7573 6f73 7575 6465  n laskutusosuude
-00009bb0: 7420 6a61 2074 6965 646f 740a 2020 2020  t ja tiedot.    
-00009bc0: 2020 2020 6f76 6174 206f 696b 6569 6e2e      ovat oikein.
-00009bd0: 3c2f 6c61 6265 6c3e 5c72 5c6e 5c74 5c74  </label>\r\n\t\t
-00009be0: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
-00009bf0: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
-00009c00: 5c6e 5c74 5c74 5c74 5c74 3c64 6976 0a20  \n\t\t\t\t<div. 
-00009c10: 2020 2020 2020 2063 6c61 7373 3d5c 2266         class=\"f
-00009c20: 6f72 6d2d 6275 7474 6f6e 7320 7465 7874  orm-buttons text
-00009c30: 2d63 656e 7465 725c 223e 5c72 5c6e 5c74  -center\">\r\n\t
-00009c40: 5c74 5c74 5c74 5c74 3c62 7574 746f 6e20  \t\t\t\t<button 
-00009c50: 636c 6173 733d 5c22 6274 6e20 6274 6e2d  class=\"btn btn-
-00009c60: 7072 696d 6172 795c 220a 2020 2020 2020  primary\".      
-00009c70: 2020 6461 7461 2d61 6374 696f 6e3d 5c22    data-action=\"
-00009c80: 7361 7665 2d6b 696d 7070 615c 2220 6469  save-kimppa\" di
-00009c90: 7361 626c 6564 3e4c 5c78 4534 6865 745c  sabled>L\xE4het\
-00009ca0: 7845 3420 6d75 7574 6f6b 7365 743c 2f62  xE4 muutokset</b
-00009cb0: 7574 746f 6e3e 5c72 5c6e 5c74 5c74 5c74  utton>\r\n\t\t\t
-00009cc0: 5c74 5c74 3c62 7574 746f 6e0a 2020 2020  \t\t<button.    
-00009cd0: 2020 2020 636c 6173 733d 5c22 6274 6e20      class=\"btn 
-00009ce0: 6274 6e2d 7072 696d 6172 795c 2220 6461  btn-primary\" da
-00009cf0: 7461 2d61 6374 696f 6e3d 5c22 6361 6e63  ta-action=\"canc
-00009d00: 656c 2d61 6c6c 5c22 3e50 6572 7575 7461  el-all\">Peruuta
-00009d10: 206d 7575 746f 6b73 6574 3c2f 6275 7474   muutokset</butt
-00009d20: 6f6e 3e5c 725c 6e5c 745c 745c 745c 743c  on>\r\n\t\t\t\t<
-00009d30: 2f64 6976 3e5c 725c 6e5c 745c 745c 743c  /div>\r\n\t\t\t<
-00009d40: 2f64 6976 3e5c 725c 6e5c 745c 743c 2f64  /div>\r\n\t\t</d
-00009d50: 6976 3e5c 725c 6e5c 743c 2f64 6976 3e5c  iv>\r\n\t</div>\
-00009d60: 725c 6e3c 2f64 6976 3e5c 725c 6e5c 725c  r\n</div>\r\n\r\
-00009d70: 6e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  n\r\n\r\n\r\n\r\
-00009d80: 6e3c 6469 760a 2020 2020 2020 2020 6964  n<div.        id
-00009d90: 3d5c 2265 6469 742d 6b69 6d70 7061 2d6d  =\"edit-kimppa-m
-00009da0: 6f64 616c 5c22 2063 6c61 7373 3d5c 226d  odal\" class=\"m
-00009db0: 6f64 616c 5c22 2073 7479 6c65 3d5c 2264  odal\" style=\"d
-00009dc0: 6973 706c 6179 3a6e 6f6e 655c 223e 5c72  isplay:none\">\r
-00009dd0: 5c6e 5c74 3c64 6976 0a20 2020 2020 2020  \n\t<div.       
-00009de0: 2063 6c61 7373 3d5c 226d 6f64 616c 2d64   class=\"modal-d
-00009df0: 6961 6c6f 6720 6d6f 6461 6c2d 6c67 5c22  ialog modal-lg\"
-00009e00: 3e5c 725c 6e5c 745c 743c 6469 7620 636c  >\r\n\t\t<div cl
-00009e10: 6173 733d 5c22 6d6f 6461 6c2d 636f 6e74  ass=\"modal-cont
-00009e20: 656e 745c 223e 5c72 5c6e 5c74 5c74 5c74  ent\">\r\n\t\t\t
-00009e30: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
-00009e40: 7373 3d5c 226d 6f64 616c 2d62 6f64 795c  ss=\"modal-body\
-00009e50: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 3c64  ">\r\n\t\t\t\t<d
-00009e60: 6976 2063 6c61 7373 3d5c 2270 6167 652d  iv class=\"page-
-00009e70: 6865 6164 6572 5c22 3e5c 725c 6e5c 745c  header\">\r\n\t\
-00009e80: 745c 745c 745c 745c 725c 6e5c 745c 745c  t\t\t\t\r\n\t\t\
-00009e90: 745c 745c 743c 6275 7474 6f6e 0a20 2020  t\t\t<button.   
-00009ea0: 2020 2020 2063 6c61 7373 3d5c 2270 756c       class=\"pul
-00009eb0: 6c2d 7269 6768 7420 6274 6e2d 6469 736d  l-right btn-dism
-00009ec0: 6973 735c 2220 6172 6961 2d6c 6162 656c  iss\" aria-label
-00009ed0: 3d5c 2253 756c 6a65 5c22 2064 6174 612d  =\"Sulje\" data-
-00009ee0: 6163 7469 6f6e 3d5c 2263 616e 6365 6c2d  action=\"cancel-
-00009ef0: 616c 6c5c 223e 3c2f 6275 7474 6f6e 3e5c  all\"></button>\
-00009f00: 725c 6e5c 745c 745c 745c 745c 743c 6831  r\n\t\t\t\t\t<h1
-00009f10: 3e4d 756f 6b6b 6161 0a20 2020 2020 2020  >Muokkaa.       
-00009f20: 206b 696d 7070 6161 3c2f 6831 3e5c 725c   kimppaa</h1>\r\
-00009f30: 6e5c 745c 745c 745c 743c 2f64 6976 3e5c  n\t\t\t\t</div>\
-00009f40: 725c 6e5c 745c 745c 745c 745c 725c 6e5c  r\n\t\t\t\t\r\n\
-00009f50: 745c 745c 745c 743c 6469 7620 636c 6173  t\t\t\t<div clas
-00009f60: 733d 5c22 7465 7874 2d72 6967 6874 5c22  s=\"text-right\"
-00009f70: 3e5c 725c 6e5c 745c 745c 745c 745c 743c  >\r\n\t\t\t\t\t<
-00009f80: 6275 7474 6f6e 0a20 2020 2020 2020 2063  button.        c
-00009f90: 6c61 7373 3d5c 2262 746e 2062 746e 2d6c  lass=\"btn btn-l
-00009fa0: 696e 6b5c 2220 6461 7461 2d61 6374 696f  ink\" data-actio
-00009fb0: 6e3d 5c22 7072 696e 745c 223e 5475 6c6f  n=\"print\">Tulo
-00009fc0: 7374 6120 6b69 6d70 7061 6c75 6574 7465  sta kimppaluette
-00009fd0: 6c6f 203c 7370 616e 0a20 2020 2020 2020  lo <span.       
-00009fe0: 2063 6c61 7373 3d5c 2267 6c79 7068 6963   class=\"glyphic
-00009ff0: 6f6e 2067 6c79 7068 6963 6f6e 2d70 7269  on glyphicon-pri
-0000a000: 6e74 5c22 3e3c 2f73 7061 6e3e 3c2f 6275  nt\"></span></bu
-0000a010: 7474 6f6e 3e5c 725c 6e5c 745c 745c 745c  tton>\r\n\t\t\t\
-0000a020: 743c 2f64 6976 3e5c 725c 6e5c 725c 6e5c  t</div>\r\n\r\n\
-0000a030: 745c 745c 745c 743c 6469 760a 2020 2020  t\t\t\t<div.    
-0000a040: 2020 2020 636c 6173 733d 5c22 6b69 6d70      class=\"kimp
-0000a050: 7061 5c22 3e5c 725c 6e5c 745c 745c 745c  pa\">\r\n\t\t\t\
-0000a060: 745c 743c 7374 796c 6520 7363 6f70 6564  t\t<style scoped
-0000a070: 3e5c 725c 6e5c 745c 745c 745c 745c 742e  >\r\n\t\t\t\t\t.
-0000a080: 6b69 6d70 7061 2073 7061 6e2e 6973 616e  kimppa span.isan
-0000a090: 7461 3a62 6566 6f72 650a 2020 2020 2020  ta:before.      
-0000a0a0: 2020 7b5c 725c 6e5c 745c 745c 745c 745c    {\r\n\t\t\t\t\
-0000a0b0: 745c 7463 6f6e 7465 6e74 3a20 274b 696d  t\tcontent: 'Kim
-0000a0c0: 7070 6169 735c 7845 346e 745c 7845 3427  ppais\xE4nt\xE4'
-0000a0d0: 3b5c 725c 6e5c 745c 745c 745c 745c 747d  ;\r\n\t\t\t\t\t}
-0000a0e0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c2f  \r\n\t\t\t\t\t</
-0000a0f0: 7374 796c 653e 5c72 5c6e 5c72 5c6e 5c74  style>\r\n\r\n\t
-0000a100: 5c74 5c74 5c74 5c74 3c64 6976 0a20 2020  \t\t\t\t<div.   
-0000a110: 2020 2020 2063 6c61 7373 3d5c 2267 7269       class=\"gri
-0000a120: 645c 223e 3c2f 6469 763e 5c72 5c6e 5c72  d\"></div>\r\n\r
-0000a130: 5c6e 5c74 5c74 5c74 5c74 5c74 3c73 6372  \n\t\t\t\t\t<scr
-0000a140: 6970 7420 6964 3d5c 226b 696d 7070 612d  ipt id=\"kimppa-
-0000a150: 6564 6974 2d6d 656e 752d 7465 6d70 6c61  edit-menu-templa
-0000a160: 7465 5c22 0a20 2020 2020 2020 2074 7970  te\".        typ
-0000a170: 653d 5c22 7465 7874 2f78 2d74 656d 706c  e=\"text/x-templ
-0000a180: 6174 655c 223e 5c72 5c6e 5c74 5c74 5c74  ate\">\r\n\t\t\t
-0000a190: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
-0000a1a0: 3d5c 226d 656e 7520 6564 6974 2d6d 656e  =\"menu edit-men
-0000a1b0: 755c 2220 6461 7461 2d72 6f6c 653d 5c22  u\" data-role=\"
-0000a1c0: 6564 6974 2d6d 656e 755c 223e 5c72 5c6e  edit-menu\">\r\n
-0000a1d0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c64  \t\t\t\t\t\t\t<d
-0000a1e0: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
-0000a1f0: 3d5c 2272 6f77 5c22 3e5c 725c 6e5c 745c  =\"row\">\r\n\t\
-0000a200: 745c 745c 745c 745c 745c 745c 743c 6469  t\t\t\t\t\t\t<di
-0000a210: 7620 636c 6173 733d 5c22 636f 6c2d 7873  v class=\"col-xs
-0000a220: 2d34 5c22 3e5c 725c 6e5c 745c 745c 745c  -4\">\r\n\t\t\t\
-0000a230: 745c 745c 745c 745c 745c 743c 6275 7474  t\t\t\t\t\t<butt
-0000a240: 6f6e 0a20 2020 2020 2020 2074 7970 653d  on.        type=
-0000a250: 5c22 6275 7474 6f6e 5c22 2064 6174 612d  \"button\" data-
-0000a260: 6163 7469 6f6e 3d5c 2265 6469 742d 6f73  action=\"edit-os
-0000a270: 616b 6173 5c22 2063 6c61 7373 3d5c 2262  akas\" class=\"b
-0000a280: 746e 2062 746e 2d70 7269 6d61 7279 2062  tn btn-primary b
-0000a290: 746e 2d62 6c6f 636b 5c22 3e5c 725c 6e5c  tn-block\">\r\n\
-0000a2a0: 745c 745c 745c 745c 745c 745c 745c 745c  t\t\t\t\t\t\t\t\
-0000a2b0: 745c 744d 756f 6b6b 6161 5c72 5c6e 5c74  t\tMuokkaa\r\n\t
-0000a2c0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-0000a2d0: 3c2f 6275 7474 6f6e 3e5c 725c 6e5c 745c  </button>\r\n\t\
-0000a2e0: 745c 745c 745c 745c 745c 745c 743c 2f64  t\t\t\t\t\t\t</d
-0000a2f0: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
-0000a300: 745c 745c 745c 743c 6469 760a 2020 2020  t\t\t\t<div.    
-0000a310: 2020 2020 636c 6173 733d 5c22 636f 6c2d      class=\"col-
-0000a320: 7873 2d34 5c22 3e5c 725c 6e5c 745c 745c  xs-4\">\r\n\t\t\
-0000a330: 745c 745c 745c 745c 745c 745c 743c 6275  t\t\t\t\t\t\t<bu
-0000a340: 7474 6f6e 2074 7970 653d 5c22 6275 7474  tton type=\"butt
-0000a350: 6f6e 5c22 2064 6174 612d 6163 7469 6f6e  on\" data-action
-0000a360: 3d5c 2263 6c6f 7365 2d6d 656e 755c 220a  =\"close-menu\".
-0000a370: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-0000a380: 6274 6e20 6274 6e2d 7072 696d 6172 7920  btn btn-primary 
-0000a390: 6274 6e2d 626c 6f63 6b5c 223e 5c72 5c6e  btn-block\">\r\n
-0000a3a0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-0000a3b0: 5c74 5c74 5065 7275 7574 615c 725c 6e5c  \t\tPeruuta\r\n\
-0000a3c0: 745c 745c 745c 745c 745c 745c 745c 745c  t\t\t\t\t\t\t\t\
-0000a3d0: 743c 2f62 7574 746f 6e3e 5c72 5c6e 5c74  t</button>\r\n\t
-0000a3e0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \t\t\t\t\t\t\t</
-0000a3f0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
-0000a400: 5c74 5c74 5c74 5c74 3c64 6976 0a20 2020  \t\t\t\t<div.   
-0000a410: 2020 2020 2063 6c61 7373 3d5c 2263 6f6c       class=\"col
-0000a420: 2d78 732d 345c 223e 5c72 5c6e 5c74 5c74  -xs-4\">\r\n\t\t
-0000a430: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c62  \t\t\t\t\t\t\t<b
-0000a440: 7574 746f 6e20 7479 7065 3d5c 2262 7574  utton type=\"but
-0000a450: 746f 6e5c 2220 6461 7461 2d61 6374 696f  ton\" data-actio
-0000a460: 6e3d 5c22 6465 6c65 7465 2d72 6f77 5c22  n=\"delete-row\"
-0000a470: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
-0000a480: 2262 746e 2062 746e 2d70 7269 6d61 7279  "btn btn-primary
-0000a490: 2062 746e 2d62 6c6f 636b 5c22 3e5c 725c   btn-block\">\r\
-0000a4a0: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
-0000a4b0: 745c 745c 7450 6f69 7374 615c 725c 6e5c  t\t\tPoista\r\n\
-0000a4c0: 745c 745c 745c 745c 745c 745c 745c 745c  t\t\t\t\t\t\t\t\
-0000a4d0: 743c 2f62 7574 746f 6e3e 5c72 5c6e 5c74  t</button>\r\n\t
-0000a4e0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \t\t\t\t\t\t\t</
-0000a4f0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
-0000a500: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
-0000a510: 5c74 5c74 5c74 5c74 5c74 5c74 3c2f 6469  \t\t\t\t\t\t</di
-0000a520: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  v>\r\n\t\t\t\t\t
-0000a530: 3c2f 7363 7269 7074 3e5c 725c 6e5c 725c  </script>\r\n\r\
-0000a540: 6e5c 745c 745c 745c 745c 743c 7363 7269  n\t\t\t\t\t<scri
-0000a550: 7074 0a20 2020 2020 2020 2069 643d 5c22  pt.        id=\"
-0000a560: 6b69 6d70 7061 2d70 6169 6e6f 2d6d 656e  kimppa-paino-men
-0000a570: 752d 7465 6d70 6c61 7465 5c22 2074 7970  u-template\" typ
-0000a580: 653d 5c22 7465 7874 2f78 2d74 656d 706c  e=\"text/x-templ
-0000a590: 6174 655c 223e 5c72 5c6e 5c74 5c74 5c74  ate\">\r\n\t\t\t
-0000a5a0: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-0000a5b0: 2063 6c61 7373 3d5c 226d 656e 7520 7061   class=\"menu pa
-0000a5c0: 696e 6f2d 6d65 6e75 5c22 2064 6174 612d  ino-menu\" data-
-0000a5d0: 726f 6c65 3d5c 2270 6169 6e6f 2d6d 656e  role=\"paino-men
-0000a5e0: 755c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  u\">\r\n\t\t\t\t
-0000a5f0: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
-0000a600: 2272 6f77 0a20 2020 2020 2020 2072 6f77  "row.        row
-0000a610: 2d63 656e 7465 7265 645c 223e 5c72 5c6e  -centered\">\r\n
-0000a620: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c64  \t\t\t\t\t\t\t<d
-0000a630: 6976 2063 6c61 7373 3d5c 2263 6f6c 2d78  iv class=\"col-x
-0000a640: 732d 3420 636f 6c2d 6365 6e74 6572 6564  s-4 col-centered
-0000a650: 5c22 3e3c 6275 7474 6f6e 0a20 2020 2020  \"><button.     
-0000a660: 2020 2074 7970 653d 5c22 6275 7474 6f6e     type=\"button
-0000a670: 5c22 2064 6174 612d 6163 7469 6f6e 3d5c  \" data-action=\
-0000a680: 2273 6574 2d70 6169 6e6f 5c22 2064 6174  "set-paino\" dat
-0000a690: 612d 7661 6c75 653d 5c22 305c 2220 636c  a-value=\"0\" cl
-0000a6a0: 6173 733d 5c22 6274 6e20 6274 6e2d 7072  ass=\"btn btn-pr
-0000a6b0: 696d 6172 790a 2020 2020 2020 2020 6274  imary.        bt
-0000a6c0: 6e2d 626c 6f63 6b5c 223e 5c72 5c6e 5c74  n-block\">\r\n\t
-0000a6d0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 4569  \t\t\t\t\t\t\tEi
-0000a6e0: 206c 6173 6b75 7465 7461 5c72 5c6e 5c74   laskuteta\r\n\t
-0000a6f0: 5c74 5c74 5c74 5c74 5c74 5c74 3c2f 6275  \t\t\t\t\t\t</bu
-0000a700: 7474 6f6e 3e3c 2f64 6976 3e5c 725c 6e5c  tton></div>\r\n\
-0000a710: 745c 745c 745c 745c 745c 745c 745c 725c  t\t\t\t\t\t\t\r\
-0000a720: 6e5c 745c 745c 745c 745c 745c 745c 743c  n\t\t\t\t\t\t\t<
-0000a730: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-0000a740: 733d 5c22 636f 6c2d 7873 2d34 2063 6f6c  s=\"col-xs-4 col
-0000a750: 2d63 656e 7465 7265 645c 223e 3c62 7574  -centered\"><but
-0000a760: 746f 6e20 7479 7065 3d5c 2262 7574 746f  ton type=\"butto
-0000a770: 6e5c 2220 6461 7461 2d61 6374 696f 6e3d  n\" data-action=
-0000a780: 5c22 7365 742d 7061 696e 6f5c 220a 2020  \"set-paino\".  
-0000a790: 2020 2020 2020 6461 7461 2d76 616c 7565        data-value
-0000a7a0: 3d5c 2232 5c22 2063 6c61 7373 3d5c 2262  =\"2\" class=\"b
-0000a7b0: 746e 2062 746e 2d70 7269 6d61 7279 2062  tn btn-primary b
-0000a7c0: 746e 2d62 6c6f 636b 5c22 3e5c 725c 6e5c  tn-block\">\r\n\
-0000a7d0: 745c 745c 745c 745c 745c 745c 745c 7456  t\t\t\t\t\t\t\tV
-0000a7e0: 616b 6974 7569 7365 6e0a 2020 2020 2020  akituisen.      
-0000a7f0: 2020 6d75 6b61 6973 6573 7469 5c72 5c6e    mukaisesti\r\n
-0000a800: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \t\t\t\t\t\t\t</
-0000a810: 6275 7474 6f6e 3e3c 2f64 6976 3e5c 725c  button></div>\r\
-0000a820: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
-0000a830: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
-0000a840: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
-0000a850: 6173 733d 5c22 636f 6c2d 7873 2d34 2063  ass=\"col-xs-4 c
-0000a860: 6f6c 2d63 656e 7465 7265 645c 223e 3c62  ol-centered\"><b
-0000a870: 7574 746f 6e20 7479 7065 3d5c 2262 7574  utton type=\"but
-0000a880: 746f 6e5c 2220 6461 7461 2d61 6374 696f  ton\" data-actio
-0000a890: 6e3d 5c22 7365 742d 7061 696e 6f5c 220a  n=\"set-paino\".
-0000a8a0: 2020 2020 2020 2020 6461 7461 2d76 616c          data-val
-0000a8b0: 7565 3d5c 2231 5c22 2063 6c61 7373 3d5c  ue=\"1\" class=\
-0000a8c0: 2262 746e 2062 746e 2d70 7269 6d61 7279  "btn btn-primary
-0000a8d0: 2062 746e 2d62 6c6f 636b 5c22 3e5c 725c   btn-block\">\r\
-0000a8e0: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
-0000a8f0: 7456 6170 6161 2d61 6a61 6e0a 2020 2020  tVapaa-ajan.    
-0000a900: 2020 2020 6d75 6b61 6973 6573 7469 5c72      mukaisesti\r
-0000a910: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-0000a920: 3c2f 6275 7474 6f6e 3e3c 2f64 6976 3e5c  </button></div>\
-0000a930: 725c 6e5c 745c 745c 745c 745c 745c 743c  r\n\t\t\t\t\t\t<
-0000a940: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
-0000a950: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
-0000a960: 745c 745c 745c 743c 2f73 6372 6970 743e  t\t\t\t</script>
-0000a970: 5c72 5c6e 5c72 5c6e 5c74 5c74 5c74 5c74  \r\n\r\n\t\t\t\t
-0000a980: 5c74 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  \t\r\n\t\t\t\t\t
-0000a990: 5c74 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  \t\r\n\t\t\t\t\t
-0000a9a0: 5c74 5c74 3c70 3e4a 6f73 0a20 2020 2020  \t\t<p>Jos.     
-0000a9b0: 2020 206b 696d 7061 6e20 6f73 616b 6169     kimpan osakai
-0000a9c0: 7373 6120 6f6e 2074 6170 6168 7475 6e75  ssa on tapahtunu
-0000a9d0: 7420 6d75 7574 6f6b 7369 612c 2070 6f69  t muutoksia, poi
-0000a9e0: 7374 6120 6f73 616b 6173 206a 6120 6c75  sta osakas ja lu
-0000a9f0: 6f20 7575 7369 2e3c 2f70 3e5c 725c 6e5c  o uusi.</p>\r\n\
-0000aa00: 745c 745c 745c 745c 745c 745c 725c 6e5c  t\t\t\t\t\t\r\n\
-0000aa10: 725c 6e5c 745c 745c 745c 745c 745c 743c  r\n\t\t\t\t\t\t<
-0000aa20: 703e 4c61 736b 7574 7573 6f73 7575 6b73  p>Laskutusosuuks
-0000aa30: 6965 6e0a 2020 2020 2020 2020 7375 6d6d  ien.        summ
-0000aa40: 6120 745c 7845 3479 7479 7920 6f6c 6c61  a t\xE4ytyy olla
-0000aa50: 2031 3030 2025 2e20 566f 6974 206a 616b   100 %. Voit jak
-0000aa60: 6161 206b 696d 7061 6e20 6c61 736b 7574  aa kimpan laskut
-0000aa70: 7573 6f73 7575 6465 7420 6175 746f 6d61  usosuudet automa
-0000aa80: 6174 7469 7365 7374 690a 2020 2020 2020  attisesti.      
-0000aa90: 2020 616c 6c61 206f 6c65 7661 6c6c 6120    alla olevalla 
-0000aaa0: 7061 696e 696b 6b65 656c 6c61 2c20 6a6f  painikkeella, jo
-0000aab0: 6c6c 6f69 6e20 6c61 736b 7574 7573 6f73  lloin laskutusos
-0000aac0: 7575 6465 7420 6a61 6574 6161 6e20 6b69  uudet jaetaan ki
-0000aad0: 696e 7465 6973 745c 7846 366e 0a20 2020  inteist\xF6n.   
-0000aae0: 2020 2020 206b 5c78 4534 7974 745c 7846       k\xE4ytt\xF
-0000aaf0: 3674 6172 6b6f 6974 756b 7365 6e20 6d75  6tarkoituksen mu
-0000ab00: 6b61 616e 2e20 566f 6974 206d 795c 7846  kaan. Voit my\xF
-0000ab10: 3673 2068 616c 7574 6573 7361 7369 2073  6s halutessasi s
-0000ab20: 795c 7846 3674 745c 7845 345c 7845 340a  y\xF6tt\xE4\xE4.
-0000ab30: 2020 2020 2020 2020 6c61 736b 7574 7573          laskutus
-0000ab40: 6f73 7575 6465 7420 6b5c 7845 3473 696e  osuudet k\xE4sin
-0000ab50: 2079 6c6c 5c78 4534 6f6c 6576 6969 6e20   yll\xE4oleviin 
-0000ab60: 6b65 6e74 7469 696e 2e3c 2f70 3e5c 725c  kenttiin.</p>\r\
-0000ab70: 6e5c 725c 6e5c 745c 745c 745c 745c 745c  n\r\n\t\t\t\t\t\
-0000ab80: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
-0000ab90: 6173 733d 5c22 7465 7874 2d63 656e 7465  ass=\"text-cente
-0000aba0: 725c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  r\">\r\n\t\t\t\t
-0000abb0: 5c74 5c74 5c74 3c62 7574 746f 6e20 7479  \t\t\t<button ty
-0000abc0: 7065 3d5c 2262 7574 746f 6e5c 2220 636c  pe=\"button\" cl
-0000abd0: 6173 733d 5c22 6274 6e0a 2020 2020 2020  ass=\"btn.      
-0000abe0: 2020 6274 6e2d 6465 6661 756c 745c 2220    btn-default\" 
-0000abf0: 6461 7461 2d61 6374 696f 6e3d 5c22 6469  data-action=\"di
-0000ac00: 7374 7269 6275 7465 2d65 7665 6e6c 795c  stribute-evenly\
-0000ac10: 223e 4a61 6120 6c61 736b 7574 7573 2d25  ">Jaa laskutus-%
-0000ac20: 2074 6173 616e 3c2f 6275 7474 6f6e 3e5c   tasan</button>\
-0000ac30: 725c 6e5c 745c 745c 745c 745c 745c 743c  r\n\t\t\t\t\t\t<
-0000ac40: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
-0000ac50: 745c 745c 725c 6e5c 745c 745c 745c 745c  t\t\r\n\t\t\t\t\
-0000ac60: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
-0000ac70: 636c 6173 733d 5c22 666f 726d 2d67 726f  class=\"form-gro
-0000ac80: 7570 5c22 3e5c 725c 6e5c 745c 745c 745c  up\">\r\n\t\t\t\
-0000ac90: 745c 745c 745c 743c 6c61 6265 6c20 666f  t\t\t\t<label fo
-0000aca0: 723d 5c22 4b49 4d43 6f6d 6d5c 223e 4d75  r=\"KIMComm\">Mu
-0000acb0: 7574 6f6b 7365 6e20 7379 793c 2f6c 6162  utoksen syy</lab
-0000acc0: 656c 3e5c 725c 6e5c 745c 745c 745c 745c  el>\r\n\t\t\t\t\
-0000acd0: 745c 745c 743c 7465 7874 6172 6561 0a20  t\t\t<textarea. 
-0000ace0: 2020 2020 2020 2069 643d 5c22 4b49 4d43         id=\"KIMC
-0000acf0: 6f6d 6d5c 2220 6e61 6d65 3d5c 224b 494d  omm\" name=\"KIM
-0000ad00: 436f 6d6d 5c22 2063 6c61 7373 3d5c 2266  Comm\" class=\"f
-0000ad10: 6f72 6d2d 636f 6e74 726f 6c5c 223e 3c2f  orm-control\"></
-0000ad20: 7465 7874 6172 6561 3e5c 725c 6e5c 745c  textarea>\r\n\t\
-0000ad30: 745c 745c 745c 745c 743c 2f64 6976 3e5c  t\t\t\t\t</div>\
-0000ad40: 725c 6e5c 745c 745c 745c 745c 745c 725c  r\n\t\t\t\t\t\r\
-0000ad50: 6e5c 745c 745c 745c 745c 745c 743c 6469  n\t\t\t\t\t\t<di
-0000ad60: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
-0000ad70: 5c22 666f 726d 2d67 726f 7570 205c 223e  \"form-group \">
-0000ad80: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-0000ad90: 5c74 3c6c 6162 656c 2066 6f72 3d5c 224b  \t<label for=\"K
-0000ada0: 4952 5076 6d5c 223e 4d75 7574 6f6b 7365  IRPvm\">Muutokse
-0000adb0: 7420 7475 6c65 7661 740a 2020 2020 2020  t tulevat.      
-0000adc0: 2020 766f 696d 6161 6e3c 2f6c 6162 656c    voimaan</label
-0000add0: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-0000ade0: 745c 743c 696e 7075 7420 6e61 6d65 3d5c  t\t<input name=\
-0000adf0: 224b 4952 5076 6d5c 2220 636c 6173 733d  "KIRPvm\" class=
-0000ae00: 5c22 666f 726d 2d63 6f6e 7472 6f6c 5c22  \"form-control\"
-0000ae10: 0a20 2020 2020 2020 203e 5c72 5c6e 5c74  .        >\r\n\t
-0000ae20: 5c74 5c74 5c74 5c74 5c74 3c2f 6469 763e  \t\t\t\t\t</div>
-0000ae30: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-0000ae40: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-0000ae50: 3c64 6976 2063 6c61 7373 3d5c 2266 6f72  <div class=\"for
-0000ae60: 6d2d 6772 6f75 705c 223e 5c72 5c6e 5c74  m-group\">\r\n\t
-0000ae70: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae90: 203c 6c61 6265 6c20 666f 723d 5c22 6e6f   <label for=\"no
-0000aea0: 7469 6669 6572 7068 6f6e 655c 223e 496c  tifierphone\">Il
-0000aeb0: 6d6f 6974 7461 6a61 6e20 7075 6865 6c69  moittajan puheli
-0000aec0: 6e6e 756d 6572 6f3c 2f6c 6162 656c 3e5c  nnumero</label>\
-0000aed0: 725c 6e5c 740a 2020 2020 2020 2020 5c20  r\n\t.        \ 
-0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aef0: 2020 2020 2020 3c69 6e70 7574 206e 616d        <input nam
-0000af00: 653d 5c22 6e6f 7469 6669 6572 7068 6f6e  e=\"notifierphon
-0000af10: 655c 2220 7479 7065 3d5c 2274 656c 5c22  e\" type=\"tel\"
-0000af20: 2063 6c61 7373 3d5c 2266 6f72 6d2d 636f   class=\"form-co
-0000af30: 6e74 726f 6c5c 220a 2020 2020 2020 2020  ntrol\".        
-0000af40: 7061 7474 6572 6e3d 5c22 5e5c 5c73 2a5c  pattern=\"^\\s*\
-0000af50: 5c2b 3f28 5c5c 647c 5c5c 737c 2d29 2b24  \+?(\\d|\\s|-)+$
-0000af60: 5c22 2070 6c61 6365 686f 6c64 6572 3d5c  \" placeholder=\
-0000af70: 225c 223e 5c72 5c6e 5c74 2020 2020 2020  "\">\r\n\t      
-0000af80: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0000af90: 6469 763e 5c72 5c6e 5c72 5c6e 5c74 0a20  div>\r\n\r\n\t. 
-0000afa0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-0000afb0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000afc0: 636c 6173 733d 5c22 666f 726d 2d67 726f  class=\"form-gro
-0000afd0: 7570 5c22 3e5c 725c 6e5c 7420 2020 2020  up\">\r\n\t     
-0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aff0: 2020 203c 6c61 6265 6c0a 2020 2020 2020     <label.      
-0000b000: 2020 666f 723d 5c22 6e6f 7469 6669 6572    for=\"notifier
-0000b010: 656d 6169 6c5c 223e 496c 6d6f 6974 7461  email\">Ilmoitta
-0000b020: 6a61 6e20 735c 7845 3468 6b5c 7846 3670  jan s\xE4hk\xF6p
-0000b030: 6f73 7469 6f73 6f69 7465 3c2f 6c61 6265  ostiosoite</labe
-0000b040: 6c3e 5c72 5c6e 5c74 2020 2020 2020 2020  l>\r\n\t        
-0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b060: 3c69 6e70 7574 0a20 2020 2020 2020 206e  <input.        n
-0000b070: 616d 653d 5c22 6e6f 7469 6669 6572 656d  ame=\"notifierem
-0000b080: 6169 6c5c 2220 7479 7065 3d5c 2265 6d61  ail\" type=\"ema
-0000b090: 696c 5c22 2063 6c61 7373 3d5c 2266 6f72  il\" class=\"for
-0000b0a0: 6d2d 636f 6e74 726f 6c5c 223e 5c72 5c6e  m-control\">\r\n
-0000b0b0: 5c74 2020 2020 2020 2020 2020 2020 2020  \t              
-0000b0c0: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
-0000b0d0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-0000b0e0: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
-0000b0f0: 6e5c 745c 745c 745c 743c 2f64 6976 3e5c  n\t\t\t\t</div>\
-0000b100: 725c 6e5c 745c 745c 743c 2f64 6976 3e5c  r\n\t\t\t</div>\
-0000b110: 725c 6e5c 725c 6e5c 745c 745c 743c 6469  r\n\r\n\t\t\t<di
-0000b120: 7620 636c 6173 733d 5c22 6d6f 6461 6c2d  v class=\"modal-
-0000b130: 666f 6f74 6572 5c22 3e5c 725c 6e5c 745c  footer\">\r\n\t\
-0000b140: 745c 745c 745c 725c 6e5c 745c 745c 745c  t\t\t\r\n\t\t\t\
-0000b150: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
-0000b160: 636c 6173 733d 5c22 666f 726d 2d67 726f  class=\"form-gro
-0000b170: 7570 5c22 3e5c 725c 6e5c 745c 745c 745c  up\">\r\n\t\t\t\
-0000b180: 745c 745c 743c 6469 7620 636c 6173 733d  t\t\t<div class=
-0000b190: 5c22 6368 6563 6b62 6f78 2074 6578 742d  \"checkbox text-
-0000b1a0: 6c65 6674 5c22 3e5c 725c 6e5c 745c 745c  left\">\r\n\t\t\
-0000b1b0: 745c 745c 745c 745c 743c 6c61 6265 6c3e  t\t\t\t\t<label>
-0000b1c0: 3c69 6e70 7574 0a20 2020 2020 2020 2074  <input.        t
-0000b1d0: 7970 653d 5c22 6368 6563 6b62 6f78 5c22  ype=\"checkbox\"
-0000b1e0: 206e 616d 653d 5c22 636f 6e66 6972 6d2d   name=\"confirm-
-0000b1f0: 6368 616e 6765 735c 223e 204f 6c65 6e20  changes\"> Olen 
-0000b200: 7461 726b 6973 7461 6e75 7420 6b69 6d70  tarkistanut kimp
-0000b210: 616e 206c 6173 6b75 7475 736f 7375 7564  an laskutusosuud
-0000b220: 6574 0a20 2020 2020 2020 206a 6120 7469  et.        ja ti
-0000b230: 6564 6f74 206f 7661 7420 6f69 6b65 696e  edot ovat oikein
-0000b240: 2e3c 2f6c 6162 656c 3e5c 725c 6e5c 745c  .</label>\r\n\t\
-0000b250: 745c 745c 745c 745c 743c 2f64 6976 3e5c  t\t\t\t\t</div>\
-0000b260: 725c 6e5c 745c 745c 745c 745c 743c 2f64  r\n\t\t\t\t\t</d
-0000b270: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
-0000b280: 725c 6e5c 725c 6e5c 745c 745c 745c 743c  r\n\r\n\t\t\t\t<
-0000b290: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-0000b2a0: 733d 5c22 666f 726d 2d62 7574 746f 6e73  s=\"form-buttons
-0000b2b0: 2074 6578 742d 6365 6e74 6572 5c22 3e5c   text-center\">\
-0000b2c0: 725c 6e5c 745c 745c 745c 745c 745c 725c  r\n\t\t\t\t\t\r\
-0000b2d0: 6e5c 745c 745c 745c 745c 745c 743c 6275  n\t\t\t\t\t\t<bu
-0000b2e0: 7474 6f6e 2063 6c61 7373 3d5c 2262 746e  tton class=\"btn
-0000b2f0: 0a20 2020 2020 2020 2062 746e 2d70 7269  .        btn-pri
-0000b300: 6d61 7279 5c22 2064 6174 612d 6163 7469  mary\" data-acti
-0000b310: 6f6e 3d5c 2273 6176 652d 6b69 6d70 7061  on=\"save-kimppa
-0000b320: 5c22 2064 6973 6162 6c65 643e 5c72 5c6e  \" disabled>\r\n
-0000b330: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 4c5c  \t\t\t\t\t\t\tL\
-0000b340: 7845 3468 6574 5c78 4534 0a20 2020 2020  xE4het\xE4.     
-0000b350: 2020 206d 7575 746f 6b73 6574 5c72 5c6e     muutokset\r\n
-0000b360: 5c74 5c74 5c74 5c74 5c74 5c74 3c2f 6275  \t\t\t\t\t\t</bu
-0000b370: 7474 6f6e 3e5c 725c 6e5c 745c 745c 745c  tton>\r\n\t\t\t\
-0000b380: 745c 745c 725c 6e5c 745c 745c 745c 745c  t\t\r\n\t\t\t\t\
-0000b390: 743c 6275 7474 6f6e 2063 6c61 7373 3d5c  t<button class=\
-0000b3a0: 2262 746e 0a20 2020 2020 2020 2062 746e  "btn.        btn
-0000b3b0: 2d70 7269 6d61 7279 5c22 2064 6174 612d  -primary\" data-
-0000b3c0: 6163 7469 6f6e 3d5c 2263 616e 6365 6c2d  action=\"cancel-
-0000b3d0: 616c 6c5c 223e 5c72 5c6e 5c74 5c74 5c74  all\">\r\n\t\t\t
-0000b3e0: 5c74 5c74 5c74 5065 7275 7574 6120 6d75  \t\t\tPeruuta mu
-0000b3f0: 7574 6f6b 7365 745c 725c 6e5c 745c 745c  utokset\r\n\t\t\
-0000b400: 745c 745c 743c 2f62 7574 746f 6e3e 5c72  t\t\t</button>\r
-0000b410: 5c6e 5c74 5c74 5c74 5c74 3c2f 6469 763e  \n\t\t\t\t</div>
-0000b420: 5c72 5c6e 5c74 5c74 5c74 3c2f 6469 763e  \r\n\t\t\t</div>
-0000b430: 5c72 5c6e 5c74 5c74 3c2f 6469 763e 5c72  \r\n\t\t</div>\r
-0000b440: 5c6e 5c74 3c2f 6469 763e 5c72 5c6e 3c2f  \n\t</div>\r\n</
-0000b450: 6469 763e 5c72 5c6e 5c72 5c6e 3c73 6372  div>\r\n\r\n<scr
-0000b460: 6970 740a 2020 2020 2020 2020 6964 3d5c  ipt.        id=\
-0000b470: 226b 696d 7070 612d 7072 696e 742d 7465  "kimppa-print-te
-0000b480: 6d70 6c61 7465 5c22 2074 7970 653d 5c22  mplate\" type=\"
-0000b490: 7465 7874 2f78 2d6b 656e 646f 2d74 656d  text/x-kendo-tem
-0000b4a0: 706c 6174 655c 223e 5c72 5c6e 5c74 3c6c  plate\">\r\n\t<l
-0000b4b0: 696e 6b20 7265 6c3d 5c22 7374 796c 6573  ink rel=\"styles
-0000b4c0: 6865 6574 5c22 0a20 2020 2020 2020 2068  heet\".        h
-0000b4d0: 7265 663d 5c22 2f6a 6174 656b 756b 6b6f  ref=\"/jatekukko
-0000b4e0: 2f63 7373 2f73 6168 6173 2f6b 696d 7070  /css/sahas/kimpp
-0000b4f0: 612d 7072 696e 742e 6373 735c 223e 5c72  a-print.css\">\r
-0000b500: 5c6e 5c72 5c6e 5c74 3c68 6561 6465 723e  \n\r\n\t<header>
-0000b510: 5c72 5c6e 5c74 5c74 3c68 313e 3c64 6976  \r\n\t\t<h1><div
-0000b520: 3e4a 5c78 4534 7465 6b75 6b6b 6f0a 2020  >J\xE4tekukko.  
-0000b530: 2020 2020 2020 4f79 3c2f 6469 763e 266e        Oy</div>&n
-0000b540: 6273 703b 266e 6273 703b 266e 6273 703b  bsp;&nbsp;&nbsp;
-0000b550: 266e 6273 703b 266e 6273 703b 266e 6273  &nbsp;&nbsp;&nbs
-0000b560: 703b 3c64 6976 3e4b 494d 5050 4120 233a  p;<div>KIMPPA #:
-0000b570: 206e 616d 6520 233c 2f64 6976 3e3c 2f68   name #</div></h
-0000b580: 313e 3c64 6976 0a20 2020 2020 2020 2063  1><div.        c
-0000b590: 6c61 7373 3d5c 2264 6174 655c 223e 233a  lass=\"date\">#:
-0000b5a0: 2064 6174 6520 233c 2f64 6976 3e5c 725c   date #</div>\r\
-0000b5b0: 6e5c 743c 2f68 6561 6465 723e 5c72 5c6e  n\t</header>\r\n
-0000b5c0: 5c74 3c74 6162 6c65 3e5c 725c 6e5c 745c  \t<table>\r\n\t\
-0000b5d0: 743c 7468 6561 643e 5c72 5c6e 5c74 5c74  t<thead>\r\n\t\t
-0000b5e0: 5c74 3c74 723e 5c72 5c6e 5c74 5c74 5c74  \t<tr>\r\n\t\t\t
-0000b5f0: 5c74 5c72 5c6e 5c74 5c74 5c74 5c74 3c74  \t\r\n\t\t\t\t<t
-0000b600: 683e 4e69 6d69 3c2f 7468 3e5c 725c 6e5c  h>Nimi</th>\r\n\
-0000b610: 745c 745c 745c 743c 7468 3e4c 5c78 4534  t\t\t\t<th>L\xE4
-0000b620: 6869 6f73 6f69 7465 3c2f 7468 3e5c 725c  hiosoite</th>\r\
-0000b630: 6e5c 745c 745c 745c 743c 7468 3e4c 6173  n\t\t\t\t<th>Las
-0000b640: 6b75 7475 736f 736f 6974 653c 2f74 683e  kutusosoite</th>
-0000b650: 5c72 5c6e 5c74 5c74 5c74 5c74 3c74 680a  \r\n\t\t\t\t<th.
-0000b660: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-0000b670: 6e75 6d65 7269 635c 223e 5061 6c76 656c  numeric\">Palvel
-0000b680: 752f 5072 6f73 2e6f 7375 7573 3c2f 7468  u/Pros.osuus</th
-0000b690: 3e5c 725c 6e5c 745c 745c 743c 2f74 723e  >\r\n\t\t\t</tr>
-0000b6a0: 5c72 5c6e 5c74 5c74 3c2f 7468 6561 643e  \r\n\t\t</thead>
-0000b6b0: 5c72 5c6e 5c74 5c74 3c74 626f 6479 3e5c  \r\n\t\t<tbody>\
-0000b6c0: 725c 6e5c 745c 7423 0a20 2020 2020 2020  r\n\t\t#.       
-0000b6d0: 2066 6f72 2876 6172 2069 203d 2030 3b20   for(var i = 0; 
-0000b6e0: 6920 3c20 726f 7773 2e6c 656e 6774 683b  i < rows.length;
-0000b6f0: 202b 2b69 2920 7b20 7661 7220 726f 7720   ++i) { var row 
-0000b700: 3d20 726f 7773 5b69 5d3b 2023 5c72 5c6e  = rows[i]; #\r\n
-0000b710: 5c74 5c74 5c74 3c74 723e 5c72 5c6e 5c74  \t\t\t<tr>\r\n\t
-0000b720: 5c74 5c74 5c74 5c72 5c6e 5c74 5c74 5c74  \t\t\t\r\n\t\t\t
-0000b730: 5c74 3c74 643e 233a 0a20 2020 2020 2020  \t<td>#:.       
-0000b740: 2072 6f77 2e6f 7361 6b61 732e 6e69 6d69   row.osakas.nimi
-0000b750: 2023 3c2f 7464 3e5c 725c 6e5c 745c 745c   #</td>\r\n\t\t\
-0000b760: 745c 743c 7464 3e23 3a20 726f 772e 6f73  t\t<td>#: row.os
-0000b770: 616b 6173 2e6b 6174 7520 233c 6272 3e23  akas.katu #<br>#
-0000b780: 3a20 726f 772e 6f73 616b 6173 2e70 6f73  : row.osakas.pos
-0000b790: 7469 0a20 2020 2020 2020 2023 3c2f 7464  ti.        #</td
-0000b7a0: 3e5c 725c 6e5c 745c 745c 745c 743c 7464  >\r\n\t\t\t\t<td
-0000b7b0: 3e23 3a20 726f 772e 6f73 616b 6173 2e6c  >#: row.osakas.l
-0000b7c0: 6173 6b75 7475 736b 6174 7520 233c 6272  askutuskatu #<br
-0000b7d0: 3e23 3a20 726f 772e 6f73 616b 6173 2e6c  >#: row.osakas.l
-0000b7e0: 6173 6b75 7475 7370 6f73 7469 0a20 2020  askutusposti.   
-0000b7f0: 2020 2020 2023 3c2f 7464 3e5c 725c 6e5c       #</td>\r\n\
-0000b800: 745c 745c 745c 743c 7464 2063 6c61 7373  t\t\t\t<td class
-0000b810: 3d5c 226e 756d 6572 6963 5c22 3e23 3a20  =\"numeric\">#: 
-0000b820: 6b65 6e64 6f2e 746f 5374 7269 6e67 2872  kendo.toString(r
-0000b830: 6f77 2e4b 4952 5072 6f73 2c20 276e 2729  ow.KIRPros, 'n')
-0000b840: 0a20 2020 2020 2020 2023 2025 3c2f 7464  .        # %</td
-0000b850: 3e5c 725c 6e5c 745c 745c 743c 2f74 723e  >\r\n\t\t\t</tr>
-0000b860: 5c72 5c6e 5c74 5c74 2320 7d20 235c 725c  \r\n\t\t# } #\r\
-0000b870: 6e5c 745c 743c 2f74 626f 6479 3e5c 725c  n\t\t</tbody>\r\
-0000b880: 6e5c 745c 743c 7466 6f6f 7465 723e 5c72  n\t\t<tfooter>\r
-0000b890: 5c6e 5c74 5c74 5c74 3c74 723e 5c72 5c6e  \n\t\t\t<tr>\r\n
-0000b8a0: 5c74 5c74 5c74 5c74 3c74 643e 3c2f 7464  \t\t\t\t<td></td
-0000b8b0: 3e5c 725c 6e5c 745c 745c 745c 743c 7464  >\r\n\t\t\t\t<td
-0000b8c0: 3e3c 2f74 643e 5c72 5c6e 5c74 5c74 5c74  ></td>\r\n\t\t\t
-0000b8d0: 5c74 3c74 643e 3c2f 7464 3e5c 725c 6e5c  \t<td></td>\r\n\
-0000b8e0: 745c 745c 745c 743c 7464 0a20 2020 2020  t\t\t\t<td.     
-0000b8f0: 2020 2063 6c61 7373 3d5c 226e 756d 6572     class=\"numer
-0000b900: 6963 5c22 3e59 6874 6565 6e73 5c78 4534  ic\">Yhteens\xE4
-0000b910: 3c2f 7464 3e5c 725c 6e5c 745c 745c 745c  </td>\r\n\t\t\t\
-0000b920: 743c 7464 2063 6c61 7373 3d5c 226e 756d  t<td class=\"num
-0000b930: 6572 6963 5c22 3e3c 7374 726f 6e67 3e23  eric\"><strong>#
-0000b940: 3a0a 2020 2020 2020 2020 6b65 6e64 6f2e  :.        kendo.
-0000b950: 746f 5374 7269 6e67 2870 6572 6365 6e74  toString(percent
-0000b960: 5375 6d2c 2027 6e27 2920 2320 253c 2f73  Sum, 'n') # %</s
-0000b970: 7472 6f6e 673e 3c2f 7464 3e5c 725c 6e5c  trong></td>\r\n\
-0000b980: 745c 745c 743c 2f74 723e 5c72 5c6e 5c74  t\t\t</tr>\r\n\t
-0000b990: 5c74 3c2f 7466 6f6f 7465 723e 5c72 5c6e  \t</tfooter>\r\n
-0000b9a0: 5c74 3c2f 7461 626c 653e 5c72 5c6e 3c2f  \t</table>\r\n</
-0000b9b0: 7363 7269 7074 3e5c 725c 6e5c 725c 6e3c  script>\r\n\r\n<
-0000b9c0: 6966 7261 6d65 0a20 2020 2020 2020 206e  iframe.        n
-0000b9d0: 616d 653d 5c22 6b69 6d70 7061 2d70 7269  ame=\"kimppa-pri
-0000b9e0: 6e74 5c22 2077 6964 7468 3d5c 2230 5c22  nt\" width=\"0\"
-0000b9f0: 2068 6569 6768 743d 5c22 305c 2220 6672   height=\"0\" fr
-0000ba00: 616d 6562 6f72 6465 723d 5c22 305c 2220  ameborder=\"0\" 
-0000ba10: 7372 633d 5c22 6162 6f75 743a 626c 616e  src=\"about:blan
-0000ba20: 6b5c 223e 3c2f 6966 7261 6d65 3e5c 725c  k\"></iframe>\r\
-0000ba30: 6e5c 725c 6e5c 725c 6e5c 725c 6e3c 6469  n\r\n\r\n\r\n<di
-0000ba40: 760a 2020 2020 2020 2020 6964 3d5c 2272  v.        id=\"r
-0000ba50: 6573 6967 6e2d 6b69 6d70 7061 2d6d 6f64  esign-kimppa-mod
-0000ba60: 616c 5c22 2063 6c61 7373 3d5c 226d 6f64  al\" class=\"mod
-0000ba70: 616c 5c22 2073 7479 6c65 3d5c 2264 6973  al\" style=\"dis
-0000ba80: 706c 6179 3a6e 6f6e 655c 223e 5c72 5c6e  play:none\">\r\n
-0000ba90: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
-0000baa0: 6c61 7373 3d5c 226d 6f64 616c 2d64 6961  lass=\"modal-dia
-0000bab0: 6c6f 6720 6d6f 6461 6c2d 6c67 5c22 3e5c  log modal-lg\">\
-0000bac0: 725c 6e5c 745c 743c 6469 7620 636c 6173  r\n\t\t<div clas
-0000bad0: 733d 5c22 6d6f 6461 6c2d 636f 6e74 656e  s=\"modal-conten
-0000bae0: 745c 223e 5c72 5c6e 5c74 5c74 5c74 3c64  t\">\r\n\t\t\t<d
-0000baf0: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
-0000bb00: 3d5c 226d 6f64 616c 2d62 6f64 795c 223e  =\"modal-body\">
-0000bb10: 5c72 5c6e 5c74 5c74 5c74 5c74 3c64 6976  \r\n\t\t\t\t<div
-0000bb20: 2063 6c61 7373 3d5c 2270 6167 652d 6865   class=\"page-he
-0000bb30: 6164 6572 206c 696e 652d 7374 796c 655c  ader line-style\
-0000bb40: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
-0000bb50: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c62  \r\n\t\t\t\t\t<b
-0000bb60: 7574 746f 6e0a 2020 2020 2020 2020 636c  utton.        cl
-0000bb70: 6173 733d 5c22 7075 6c6c 2d72 6967 6874  ass=\"pull-right
-0000bb80: 2062 746e 2d64 6973 6d69 7373 5c22 2061   btn-dismiss\" a
-0000bb90: 7269 612d 6c61 6265 6c3d 5c22 5375 6c6a  ria-label=\"Sulj
-0000bba0: 655c 2220 6461 7461 2d61 6374 696f 6e3d  e\" data-action=
-0000bbb0: 5c22 6361 6e63 656c 2d61 6c6c 5c22 3e3c  \"cancel-all\"><
-0000bbc0: 2f62 7574 746f 6e3e 5c72 5c6e 0a20 2020  /button>\r\n.   
-0000bbd0: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-0000bbe0: 2020 2020 2020 2020 203c 6832 3e45 726f           <h2>Ero
-0000bbf0: 6120 6b69 6d70 6173 7461 3c2f 6832 3e5c  a kimpasta</h2>\
-0000bc00: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-0000bc10: 2020 203c 2f64 6976 3e5c 725c 6e5c 725c     </div>\r\n\r\
-0000bc20: 6e5c 745c 745c 745c 743c 6469 760a 2020  n\t\t\t\t<div.  
-0000bc30: 2020 2020 2020 636c 6173 733d 5c22 666f        class=\"fo
-0000bc40: 726d 5c22 3e3c 2f64 6976 3e5c 725c 6e5c  rm\"></div>\r\n\
-0000bc50: 745c 745c 745c 743c 6469 7620 636c 6173  t\t\t\t<div clas
-0000bc60: 733d 5c22 676c 6f62 616c 2d76 616c 6964  s=\"global-valid
-0000bc70: 6174 696f 6e2d 6572 726f 7220 616c 6572  ation-error aler
-0000bc80: 740a 2020 2020 2020 2020 616c 6572 742d  t.        alert-
-0000bc90: 6461 6e67 6572 5c22 2073 7479 6c65 3d5c  danger\" style=\
-0000bca0: 2264 6973 706c 6179 3a6e 6f6e 655c 223e  "display:none\">
-0000bcb0: 545c 7845 3479 745c 7845 3420 7075 7574  T\xE4yt\xE4 puut
-0000bcc0: 7475 7661 7420 6b65 6e74 5c78 4534 743c  tuvat kent\xE4t<
-0000bcd0: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
-0000bce0: 745c 725c 6e5c 745c 745c 745c 743c 6469  t\r\n\t\t\t\t<di
-0000bcf0: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
-0000bd00: 5c22 616b 705c 223e 3c2f 6469 763e 5c72  \"akp\"></div>\r
-0000bd10: 5c6e 5c74 5c74 5c74 5c74 3c64 6976 2063  \n\t\t\t\t<div c
-0000bd20: 6c61 7373 3d5c 2261 6b70 2d69 6e66 6f5c  lass=\"akp-info\
-0000bd30: 223e 3c2f 6469 763e 5c72 5c6e 5c74 5c74  "></div>\r\n\t\t
-0000bd40: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
-0000bd50: 3c2f 6469 763e 5c72 5c6e 5c74 3c2f 6469  </div>\r\n\t</di
-0000bd60: 763e 5c72 5c6e 3c2f 6469 763e 5c72 5c6e  v>\r\n</div>\r\n
-0000bd70: 5c72 5c6e 5c72 5c6e 5c72 5c6e 3c64 6976  \r\n\r\n\r\n<div
-0000bd80: 0a20 2020 2020 2020 2069 643d 5c22 616b  .        id=\"ak
-0000bd90: 702d 6c6f 6361 7469 6f6e 2d6d 6f64 616c  p-location-modal
-0000bda0: 5c22 2063 6c61 7373 3d5c 226d 6f64 616c  \" class=\"modal
-0000bdb0: 5c22 2073 7479 6c65 3d5c 2264 6973 706c  \" style=\"displ
-0000bdc0: 6179 3a6e 6f6e 655c 223e 5c72 5c6e 5c74  ay:none\">\r\n\t
-0000bdd0: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
-0000bde0: 7373 3d5c 226d 6f64 616c 2d64 6961 6c6f  ss=\"modal-dialo
-0000bdf0: 6720 6d6f 6461 6c2d 6c67 5c22 3e5c 725c  g modal-lg\">\r\
-0000be00: 6e5c 745c 743c 6469 7620 636c 6173 733d  n\t\t<div class=
-0000be10: 5c22 6d6f 6461 6c2d 636f 6e74 656e 745c  \"modal-content\
-0000be20: 223e 5c72 5c6e 5c74 5c74 5c74 3c64 6976  ">\r\n\t\t\t<div
-0000be30: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
-0000be40: 226d 6f64 616c 2d68 6561 6465 725c 223e  "modal-header\">
-0000be50: 5c72 5c6e 5c74 5c74 5c74 5c74 5069 7374  \r\n\t\t\t\tPist
-0000be60: 6565 6e20 7369 6a61 696e 7469 202f 2056  een sijainti / V
-0000be70: 6169 6864 6120 7069 7374 6574 745c 7845  aihda pistett\xE
-0000be80: 345c 725c 6e5c 745c 745c 743c 2f64 6976  4\r\n\t\t\t</div
-0000be90: 3e5c 725c 6e5c 745c 745c 743c 6469 760a  >\r\n\t\t\t<div.
-0000bea0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-0000beb0: 6d6f 6461 6c2d 626f 6479 5c22 3e5c 725c  modal-body\">\r\
-0000bec0: 6e5c 745c 745c 745c 743c 6469 7620 636c  n\t\t\t\t<div cl
-0000bed0: 6173 733d 5c22 616b 705c 223e 3c2f 6469  ass=\"akp\"></di
-0000bee0: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 3c64  v>\r\n\t\t\t\t<d
-0000bef0: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
-0000bf00: 3d5c 2261 6b70 2d69 6e66 6f5c 223e 3c2f  =\"akp-info\"></
-0000bf10: 6469 763e 5c72 5c6e 5c74 5c74 5c74 3c2f  div>\r\n\t\t\t</
-0000bf20: 6469 763e 5c72 5c6e 5c74 5c74 3c2f 6469  div>\r\n\t\t</di
-0000bf30: 763e 5c72 5c6e 5c74 3c2f 6469 763e 5c72  v>\r\n\t</div>\r
-0000bf40: 5c6e 3c2f 6469 763e 5c72 5c6e 5c72 5c6e  \n</div>\r\n\r\n
-0000bf50: 5c72 5c6e 5c72 5c6e 3c64 6976 0a20 2020  \r\n\r\n<div.   
-0000bf60: 2020 2020 2069 643d 5c22 7265 7369 676e       id=\"resign
-0000bf70: 2d61 6b70 2d6d 6f64 616c 5c22 2063 6c61  -akp-modal\" cla
-0000bf80: 7373 3d5c 226d 6f64 616c 5c22 2073 7479  ss=\"modal\" sty
-0000bf90: 6c65 3d5c 2264 6973 706c 6179 3a6e 6f6e  le=\"display:non
-0000bfa0: 655c 223e 5c72 5c6e 5c74 3c64 6976 0a20  e\">\r\n\t<div. 
-0000bfb0: 2020 2020 2020 2063 6c61 7373 3d5c 226d         class=\"m
-0000bfc0: 6f64 616c 2d64 6961 6c6f 6720 6d6f 6461  odal-dialog moda
-0000bfd0: 6c2d 6c67 5c22 3e5c 725c 6e5c 745c 743c  l-lg\">\r\n\t\t<
-0000bfe0: 6469 7620 636c 6173 733d 5c22 6d6f 6461  div class=\"moda
-0000bff0: 6c2d 636f 6e74 656e 745c 223e 5c72 5c6e  l-content\">\r\n
-0000c000: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
-0000c010: 2020 2063 6c61 7373 3d5c 226d 6f64 616c     class=\"modal
-0000c020: 2d68 6561 6465 725c 223e 5c72 5c6e 5c74  -header\">\r\n\t
-0000c030: 5c74 5c74 5c74 4c6f 7065 7461 2070 6973  \t\t\tLopeta pis
-0000c040: 7465 656e 206b 5c78 4534 7974 745c 7846  teen k\xE4ytt\xF
-0000c050: 365c 725c 6e5c 745c 745c 743c 2f64 6976  6\r\n\t\t\t</div
-0000c060: 3e5c 725c 6e5c 745c 745c 743c 6469 760a  >\r\n\t\t\t<div.
-0000c070: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-0000c080: 6d6f 6461 6c2d 626f 6479 5c22 3e5c 725c  modal-body\">\r\
-0000c090: 6e5c 745c 745c 745c 743c 6469 7620 636c  n\t\t\t\t<div cl
-0000c0a0: 6173 733d 5c22 666f 726d 5c22 3e3c 2f64  ass=\"form\"></d
-0000c0b0: 6976 3e5c 725c 6e5c 745c 745c 743c 2f64  iv>\r\n\t\t\t</d
-0000c0c0: 6976 3e5c 725c 6e5c 745c 743c 2f64 6976  iv>\r\n\t\t</div
-0000c0d0: 3e5c 725c 6e5c 743c 2f64 6976 3e5c 725c  >\r\n\t</div>\r\
-0000c0e0: 6e3c 2f64 6976 3e5c 725c 6e5c 725c 6e5c  n</div>\r\n\r\n\
-0000c0f0: 725c 6e5c 725c 6e3c 6469 760a 2020 2020  r\n\r\n<div.    
-0000c100: 2020 2020 6964 3d5c 2274 6572 6d69 6e61      id=\"termina
-0000c110: 7465 2d73 6572 7669 6365 2d6d 6f64 616c  te-service-modal
-0000c120: 5c22 2063 6c61 7373 3d5c 226d 6f64 616c  \" class=\"modal
-0000c130: 5c22 2073 7479 6c65 3d5c 2264 6973 706c  \" style=\"displ
-0000c140: 6179 3a6e 6f6e 655c 223e 5c72 5c6e 5c74  ay:none\">\r\n\t
-0000c150: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
-0000c160: 7373 3d5c 226d 6f64 616c 2d64 6961 6c6f  ss=\"modal-dialo
-0000c170: 675c 223e 5c72 5c6e 5c74 5c74 3c64 6976  g\">\r\n\t\t<div
-0000c180: 2063 6c61 7373 3d5c 226d 6f64 616c 2d63   class=\"modal-c
-0000c190: 6f6e 7465 6e74 5c22 3e5c 725c 6e5c 745c  ontent\">\r\n\t\
-0000c1a0: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
-0000c1b0: 636c 6173 733d 5c22 6d6f 6461 6c2d 626f  class=\"modal-bo
-0000c1c0: 6479 5c22 3e5c 725c 6e5c 745c 745c 745c  dy\">\r\n\t\t\t\
-0000c1d0: 745c 725c 6e5c 745c 745c 745c 743c 6275  t\r\n\t\t\t\t<bu
-0000c1e0: 7474 6f6e 2063 6c61 7373 3d5c 2270 756c  tton class=\"pul
-0000c1f0: 6c2d 7269 6768 7420 6274 6e2d 6469 736d  l-right btn-dism
-0000c200: 6973 735c 220a 2020 2020 2020 2020 6172  iss\".        ar
-0000c210: 6961 2d6c 6162 656c 3d5c 2253 756c 6a65  ia-label=\"Sulje
-0000c220: 5c22 2064 6174 612d 6163 7469 6f6e 3d5c  \" data-action=\
-0000c230: 2263 616e 6365 6c2d 616c 6c5c 223e 3c2f  "cancel-all\"></
-0000c240: 6275 7474 6f6e 3e5c 725c 6e20 2020 2020  button>\r\n     
-0000c250: 2020 2020 2020 2020 2020 203c 6469 760a             <div.
-0000c260: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-0000c270: 666f 726d 5c22 3e3c 2f64 6976 3e5c 725c  form\"></div>\r\
-0000c280: 6e5c 745c 745c 745c 743c 6469 7620 636c  n\t\t\t\t<div cl
-0000c290: 6173 733d 5c22 676c 6f62 616c 2d76 616c  ass=\"global-val
-0000c2a0: 6964 6174 696f 6e2d 6572 726f 7220 616c  idation-error al
-0000c2b0: 6572 740a 2020 2020 2020 2020 616c 6572  ert.        aler
-0000c2c0: 742d 6461 6e67 6572 5c22 2073 7479 6c65  t-danger\" style
-0000c2d0: 3d5c 2264 6973 706c 6179 3a6e 6f6e 655c  =\"display:none\
-0000c2e0: 223e 5c72 5c6e 5c74 5c74 2020 2020 5c74  ">\r\n\t\t    \t
-0000c2f0: 5c74 545c 7845 3479 745c 7845 3420 7075  \tT\xE4yt\xE4 pu
-0000c300: 7574 7475 7661 740a 2020 2020 2020 2020  uttuvat.        
-0000c310: 6b65 6e74 5c78 4534 745c 725c 6e5c 745c  kent\xE4t\r\n\t\
-0000c320: 7420 2020 205c 743c 2f64 6976 3e5c 725c  t    \t</div>\r\
-0000c330: 6e5c 745c 745c 743c 2f64 6976 3e5c 725c  n\t\t\t</div>\r\
-0000c340: 6e5c 745c 743c 2f64 6976 3e5c 725c 6e5c  n\t\t</div>\r\n\
-0000c350: 743c 2f64 6976 3e5c 725c 6e3c 2f64 6976  t</div>\r\n</div
-0000c360: 3e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  >\r\n\r\n\r\n\r\
-0000c370: 6e3c 6469 760a 2020 2020 2020 2020 6964  n<div.        id
-0000c380: 3d5c 2263 6861 6e67 652d 6a6f 696e 2d74  =\"change-join-t
-0000c390: 7970 652d 6d6f 6461 6c5c 2220 636c 6173  ype-modal\" clas
-0000c3a0: 733d 5c22 6d6f 6461 6c5c 2220 7374 796c  s=\"modal\" styl
-0000c3b0: 653d 5c22 6469 7370 6c61 793a 6e6f 6e65  e=\"display:none
-0000c3c0: 5c22 3e5c 725c 6e5c 743c 6469 760a 2020  \">\r\n\t<div.  
-0000c3d0: 2020 2020 2020 636c 6173 733d 5c22 6d6f        class=\"mo
-0000c3e0: 6461 6c2d 6469 616c 6f67 206d 6f64 616c  dal-dialog modal
-0000c3f0: 2d6c 675c 223e 5c72 5c6e 5c74 5c74 3c64  -lg\">\r\n\t\t<d
-0000c400: 6976 2063 6c61 7373 3d5c 226d 6f64 616c  iv class=\"modal
-0000c410: 2d63 6f6e 7465 6e74 5c22 3e5c 725c 6e5c  -content\">\r\n\
-0000c420: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
-0000c430: 2020 636c 6173 733d 5c22 6d6f 6461 6c2d    class=\"modal-
-0000c440: 626f 6479 5c22 3e5c 725c 6e5c 745c 745c  body\">\r\n\t\t\
-0000c450: 745c 743c 6469 7620 636c 6173 733d 5c22  t\t<div class=\"
-0000c460: 7061 6765 2d68 6561 6465 725c 223e 5c72  page-header\">\r
-0000c470: 5c6e 5c74 5c74 5c74 5c74 5c74 5c72 5c6e  \n\t\t\t\t\t\r\n
-0000c480: 5c74 5c74 5c74 5c74 5c74 3c62 7574 746f  \t\t\t\t\t<butto
-0000c490: 6e0a 2020 2020 2020 2020 636c 6173 733d  n.        class=
-0000c4a0: 5c22 7075 6c6c 2d72 6967 6874 2062 746e  \"pull-right btn
-0000c4b0: 2d64 6973 6d69 7373 5c22 2061 7269 612d  -dismiss\" aria-
-0000c4c0: 6c61 6265 6c3d 5c22 5375 6c6a 655c 2220  label=\"Sulje\" 
-0000c4d0: 6461 7461 2d61 6374 696f 6e3d 5c22 6361  data-action=\"ca
-0000c4e0: 6e63 656c 2d61 6c6c 5c22 3e3c 2f62 7574  ncel-all\"></but
-0000c4f0: 746f 6e3e 5c72 5c6e 0a20 2020 2020 2020  ton>\r\n.       
-0000c500: 205c 2020 2020 2020 2020 2020 2020 2020   \              
-0000c510: 2020 2020 203c 6832 3e56 6169 6864 6120       <h2>Vaihda 
-0000c520: 6a5c 7845 3474 6568 756f 6c6c 6f6e 206c  j\xE4tehuollon l
-0000c530: 6969 7474 796d 6973 7461 7061 613c 2f68  iittymistapaa</h
-0000c540: 323e 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f  2>\r\n\t\t\t\t</
-0000c550: 6469 763e 5c72 5c6e 5c72 5c6e 0a20 2020  div>\r\n\r\n.   
-0000c560: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-0000c570: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000c580: 5c22 666f 726d 2d67 656e 6572 616c 2d69  \"form-general-i
-0000c590: 6e66 6f5c 223e 3c2f 6469 763e 5c72 5c6e  nfo\"></div>\r\n
-0000c5a0: 5c74 5c74 5c74 5c74 3c64 6976 2063 6c61  \t\t\t\t<div cla
-0000c5b0: 7373 3d5c 2266 6f72 6d5c 223e 3c2f 6469  ss=\"form\"></di
-0000c5c0: 763e 5c72 5c6e 0a20 2020 2020 2020 205c  v>\r\n.        \
-0000c5d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000c5e0: 6469 7620 636c 6173 733d 5c22 666f 726d  div class=\"form
-0000c5f0: 2d69 6e66 6f72 6d61 6e74 5c22 3e3c 2f64  -informant\"></d
-0000c600: 6976 3e5c 725c 6e5c 745c 745c 745c 743c  iv>\r\n\t\t\t\t<
-0000c610: 6469 7620 636c 6173 733d 5c22 616b 702d  div class=\"akp-
-0000c620: 726f 6f74 5c22 3e5c 725c 6e5c 745c 745c  root\">\r\n\t\t\
-0000c630: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
-0000c640: 2020 636c 6173 733d 5c22 616b 705c 223e    class=\"akp\">
-0000c650: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
-0000c660: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
-0000c670: 2261 6b70 2d69 6e66 6f5c 223e 3c2f 6469  "akp-info\"></di
-0000c680: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f  v>\r\n\t\t\t\t</
-0000c690: 6469 763e 5c72 5c6e 5c74 5c74 5c74 3c2f  div>\r\n\t\t\t</
-0000c6a0: 6469 763e 5c72 5c6e 5c74 5c74 3c2f 6469  div>\r\n\t\t</di
-0000c6b0: 763e 5c72 5c6e 5c74 3c2f 6469 763e 5c72  v>\r\n\t</div>\r
-0000c6c0: 5c6e 3c2f 6469 763e 5c72 5c6e 5c72 5c6e  \n</div>\r\n\r\n
-0000c6d0: 5c72 5c6e 5c72 5c6e 3c64 6976 0a20 2020  \r\n\r\n<div.   
-0000c6e0: 2020 2020 2069 643d 5c22 6f72 6465 722d       id=\"order-
-0000c6f0: 6d6f 6461 6c5c 2220 636c 6173 733d 5c22  modal\" class=\"
-0000c700: 6d6f 6461 6c5c 2220 7374 796c 653d 5c22  modal\" style=\"
-0000c710: 6469 7370 6c61 793a 6e6f 6e65 5c22 3e5c  display:none\">\
-0000c720: 725c 6e20 2020 203c 6469 7620 636c 6173  r\n    <div clas
-0000c730: 733d 5c22 6d6f 6461 6c2d 6469 616c 6f67  s=\"modal-dialog
-0000c740: 0a20 2020 2020 2020 206d 6f64 616c 2d6c  .        modal-l
-0000c750: 675c 223e 5c72 5c6e 2020 2020 2020 2020  g\">\r\n        
-0000c760: 3c64 6976 2063 6c61 7373 3d5c 226d 6f64  <div class=\"mod
-0000c770: 616c 2d63 6f6e 7465 6e74 5c22 3e5c 725c  al-content\">\r\
-0000c780: 6e20 2020 2020 2020 2020 2020 203c 6469  n            <di
-0000c790: 7620 636c 6173 733d 5c22 6d6f 6461 6c2d  v class=\"modal-
-0000c7a0: 626f 6479 5c22 3e5c 725c 6e5c 725c 6e0a  body\">\r\n\r\n.
-0000c7b0: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-0000c7c0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000c7d0: 7373 3d5c 2270 6167 652d 6865 6164 6572  ss=\"page-header
-0000c7e0: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
-0000c7f0: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
-0000c800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c810: 2020 203c 6275 7474 6f6e 0a20 2020 2020     <button.     
-0000c820: 2020 2063 6c61 7373 3d5c 2270 756c 6c2d     class=\"pull-
-0000c830: 7269 6768 7420 6274 6e2d 6469 736d 6973  right btn-dismis
-0000c840: 735c 2220 6172 6961 2d6c 6162 656c 3d5c  s\" aria-label=\
-0000c850: 2253 756c 6a65 5c22 2064 6174 612d 6163  "Sulje\" data-ac
-0000c860: 7469 6f6e 3d5c 2263 616e 6365 6c2d 616c  tion=\"cancel-al
-0000c870: 6c5c 223e 3c2f 6275 7474 6f6e 3e5c 725c  l\"></button>\r\
-0000c880: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-0000c890: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
-0000c8a0: 313e 4a5c 7845 3474 6568 756f 6c74 6f6f  1>J\xE4tehuoltoo
-0000c8b0: 6e20 6c69 6974 7479 6d69 6e65 6e3c 2f68  n liittyminen</h
-0000c8c0: 313e 5c72 5c6e 2020 2020 2020 2020 2020  1>\r\n          
-0000c8d0: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
-0000c8e0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-0000c8f0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000c900: 7620 636c 6173 733d 5c22 6c6f 6164 696e  v class=\"loadin
-0000c910: 672d 6963 6f6e 5c22 3e3c 2f64 6976 3e5c  g-icon\"></div>\
-0000c920: 725c 6e5c 725c 6e20 2020 2020 2020 2020  r\n\r\n         
-0000c930: 2020 2020 2020 203c 6469 760a 2020 2020         <div.    
-0000c940: 2020 2020 636c 6173 733d 5c22 7461 6262      class=\"tabb
-0000c950: 6172 5c22 3e5c 725c 6e20 2020 2020 2020  ar\">\r\n       
-0000c960: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
-0000c970: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0000c980: 2020 2020 203c 756c 2063 6c61 7373 3d5c       <ul class=\
-0000c990: 2274 6162 2d6c 6973 740a 2020 2020 2020  "tab-list.      
-0000c9a0: 2020 6c69 7374 2d69 6e6c 696e 655c 2220    list-inline\" 
-0000c9b0: 6461 7461 2d72 6f6c 653d 5c22 7461 622d  data-role=\"tab-
-0000c9c0: 6c69 7374 5c22 3e5c 725c 6e20 2020 2020  list\">\r\n     
-0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9e0: 2020 203c 6c69 2063 6c61 7373 3d5c 2261     <li class=\"a
-0000c9f0: 310a 2020 2020 2020 2020 6e75 6d62 6572  1.        number
-0000ca00: 2d62 7265 6164 6372 756d 625c 223e 3c61  -breadcrumb\"><a
-0000ca10: 2068 7265 663d 5c22 2361 315c 223e 313c   href=\"#a1\">1<
-0000ca20: 2f61 3e3c 2f6c 693e 5c72 5c6e 2020 2020  /a></li>\r\n    
-0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca40: 2020 2020 3c6c 690a 2020 2020 2020 2020      <li.        
-0000ca50: 636c 6173 733d 5c22 6131 5f35 206e 756d  class=\"a1_5 num
-0000ca60: 6265 722d 6272 6561 6463 7275 6d62 5c22  ber-breadcrumb\"
-0000ca70: 3e3c 6120 6872 6566 3d5c 2223 6131 2e35  ><a href=\"#a1.5
-0000ca80: 5c22 3e32 3c2f 613e 3c2f 6c69 3e5c 725c  \">2</a></li>\r\
-0000ca90: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0000caa0: 2020 2020 2020 2020 205c 725c 6e0a 2020           \r\n.  
-0000cab0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-0000cac0: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
-0000cad0: 6920 636c 6173 733d 5c22 616b 7020 6e75  i class=\"akp nu
-0000cae0: 6d62 6572 2d62 7265 6164 6372 756d 625c  mber-breadcrumb\
-0000caf0: 223e 3c61 2068 7265 663d 5c22 2361 6b70  "><a href=\"#akp
-0000cb00: 5c22 3e33 3c2f 613e 3c2f 6c69 3e5c 725c  \">3</a></li>\r\
-0000cb10: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-0000cb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb30: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
-0000cb40: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
-0000cb50: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0000cb60: 2020 2020 2020 2020 2020 3c6c 690a 2020            <li.  
-0000cb70: 2020 2020 2020 636c 6173 733d 5c22 7761        class=\"wa
-0000cb80: 7374 652d 7761 7465 7220 6e75 6d62 6572  ste-water number
-0000cb90: 2d62 7265 6164 6372 756d 625c 223e 3c61  -breadcrumb\"><a
-0000cba0: 2068 7265 663d 5c22 2377 6173 7465 2d77   href=\"#waste-w
-0000cbb0: 6174 6572 5c22 3e34 3c2f 613e 3c2f 6c69  ater\">4</a></li
-0000cbc0: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
+00005fa0: 203c 2f64 6976 3e5c 725c 6e20 2020 2020   </div>\r\n     
+00005fb0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00005fc0: 2f64 6976 3e5c 725c 6e0a 2020 2020 2020  /div>\r\n.      
+00005fd0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+00005fe0: 2020 3c2f 6469 763e 5c72 5c6e 2020 2020    </div>\r\n    
+00005ff0: 2020 2020 2020 2020 3c2f 7365 6374 696f          </sectio
+00006000: 6e3e 5c72 5c6e 5c72 5c6e 2020 2020 2020  n>\r\n\r\n      
+00006010: 2020 2020 2020 3c73 6563 7469 6f6e 0a20        <section. 
+00006020: 2020 2020 2020 2069 643d 5c22 6c6f 676f         id=\"logo
+00006030: 7574 5c22 2063 6c61 7373 3d5c 226c 6f67  ut\" class=\"log
+00006040: 6f75 745c 223e 3c2f 7365 6374 696f 6e3e  out\"></section>
+00006050: 5c72 5c6e 2020 2020 2020 2020 3c2f 6469  \r\n        </di
+00006060: 763e 5c72 5c6e 2020 2020 3c2f 6d61 696e  v>\r\n    </main
+00006070: 3e5c 725c 6e5c 725c 6e0a 2020 2020 2020  >\r\n\r\n.      
+00006080: 2020 5c20 2020 3c64 6976 3e5c 725c 6e20    \   <div>\r\n 
+00006090: 2020 2020 2020 205c 725c 6e5c 725c 6e5c         \r\n\r\n\
+000060a0: 725c 6e3c 6469 7620 6964 3d5c 2274 6572  r\n<div id=\"ter
+000060b0: 6d73 2d6d 6f64 616c 5c22 2063 6c61 7373  ms-modal\" class
+000060c0: 3d5c 226d 6f64 616c 5c22 2073 7479 6c65  =\"modal\" style
+000060d0: 3d5c 2264 6973 706c 6179 3a6e 6f6e 655c  =\"display:none\
+000060e0: 223e 5c72 5c6e 5c74 3c64 6976 0a20 2020  ">\r\n\t<div.   
+000060f0: 2020 2020 2063 6c61 7373 3d5c 226d 6f64       class=\"mod
+00006100: 616c 2d64 6961 6c6f 6720 6d6f 6461 6c2d  al-dialog modal-
+00006110: 6c67 5c22 3e5c 725c 6e5c 745c 743c 6469  lg\">\r\n\t\t<di
+00006120: 7620 636c 6173 733d 5c22 6d6f 6461 6c2d  v class=\"modal-
+00006130: 636f 6e74 656e 745c 223e 5c72 5c6e 5c74  content\">\r\n\t
+00006140: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
+00006150: 2063 6c61 7373 3d5c 226d 6f64 616c 2d62   class=\"modal-b
+00006160: 6f64 795c 223e 5c72 5c6e 5c74 5c74 5c74  ody\">\r\n\t\t\t
+00006170: 5c74 3c64 6976 2063 6c61 7373 3d5c 2274  \t<div class=\"t
+00006180: 6578 745c 223e 3c2f 6469 763e 5c72 5c6e  ext\"></div>\r\n
+00006190: 5c74 5c74 5c74 5c72 5c6e 5c74 5c74 5c74  \t\t\t\r\n\t\t\t
+000061a0: 5c74 3c64 6976 0a20 2020 2020 2020 2064  \t<div.        d
+000061b0: 6174 612d 726f 6c65 3d5c 2263 6f6e 6669  ata-role=\"confi
+000061c0: 726d 2d62 7574 746f 6e73 5c22 2063 6c61  rm-buttons\" cla
+000061d0: 7373 3d5c 2266 6f72 6d2d 6275 7474 6f6e  ss=\"form-button
+000061e0: 7320 7465 7874 2d63 656e 7465 725c 223e  s text-center\">
+000061f0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c62  \r\n\t\t\t\t\t<b
+00006200: 7574 746f 6e0a 2020 2020 2020 2020 7479  utton.        ty
+00006210: 7065 3d5c 2262 7574 746f 6e5c 2220 636c  pe=\"button\" cl
+00006220: 6173 733d 5c22 6274 6e20 6274 6e2d 6465  ass=\"btn btn-de
+00006230: 6661 756c 7420 6361 6e63 656c 5c22 2064  fault cancel\" d
+00006240: 6174 612d 6469 736d 6973 733d 5c22 6d6f  ata-dismiss=\"mo
+00006250: 6461 6c5c 223e 456e 0a20 2020 2020 2020  dal\">En.       
+00006260: 2068 7976 5c78 4534 6b73 7920 6568 746f   hyv\xE4ksy ehto
+00006270: 6a61 3c2f 6275 7474 6f6e 3e5c 725c 6e5c  ja</button>\r\n\
+00006280: 745c 745c 745c 745c 743c 6275 7474 6f6e  t\t\t\t\t<button
+00006290: 2074 7970 653d 5c22 6275 7474 6f6e 5c22   type=\"button\"
+000062a0: 2063 6c61 7373 3d5c 2262 746e 0a20 2020   class=\"btn.   
+000062b0: 2020 2020 2062 746e 2d70 7269 6d61 7279       btn-primary
+000062c0: 2061 6363 6570 745c 2220 6461 7461 2d64   accept\" data-d
+000062d0: 6973 6d69 7373 3d5c 226d 6f64 616c 5c22  ismiss=\"modal\"
+000062e0: 3e48 7976 5c78 4534 6b73 796e 2065 6864  >Hyv\xE4ksyn ehd
+000062f0: 6f74 3c2f 6275 7474 6f6e 3e5c 725c 6e5c  ot</button>\r\n\
+00006300: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
+00006310: 6e5c 745c 745c 745c 743c 6469 760a 2020  n\t\t\t\t<div.  
+00006320: 2020 2020 2020 6461 7461 2d72 6f6c 653d        data-role=
+00006330: 5c22 6469 7370 6c61 792d 6275 7474 6f6e  \"display-button
+00006340: 735c 2220 636c 6173 733d 5c22 666f 726d  s\" class=\"form
+00006350: 2d62 7574 746f 6e73 2074 6578 742d 6365  -buttons text-ce
+00006360: 6e74 6572 5c22 3e5c 725c 6e5c 745c 745c  nter\">\r\n\t\t\
+00006370: 745c 745c 743c 6275 7474 6f6e 0a20 2020  t\t\t<button.   
+00006380: 2020 2020 2074 7970 653d 5c22 6275 7474       type=\"butt
+00006390: 6f6e 5c22 2063 6c61 7373 3d5c 2262 746e  on\" class=\"btn
+000063a0: 2062 746e 2d70 7269 6d61 7279 5c22 2064   btn-primary\" d
+000063b0: 6174 612d 6469 736d 6973 733d 5c22 6d6f  ata-dismiss=\"mo
+000063c0: 6461 6c5c 2220 6461 7461 2d61 6374 696f  dal\" data-actio
+000063d0: 6e3d 5c22 6469 7370 6c61 792d 6f6b 5c22  n=\"display-ok\"
+000063e0: 3e4f 4b3c 2f62 7574 746f 6e3e 5c72 5c6e  >OK</button>\r\n
+000063f0: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
+00006400: 5c6e 5c74 5c74 5c74 3c2f 6469 763e 5c72  \n\t\t\t</div>\r
+00006410: 5c6e 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \n\t\t</div>\r\n
+00006420: 5c74 3c2f 6469 763e 5c72 5c6e 3c2f 6469  \t</div>\r\n</di
+00006430: 763e 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72  v>\r\n\r\n\r\n\r
+00006440: 5c6e 3c64 6976 0a20 2020 2020 2020 2069  \n<div.        i
+00006450: 643d 5c22 6f72 6465 722d 666f 726d 2d6d  d=\"order-form-m
+00006460: 6f64 616c 5c22 2063 6c61 7373 3d5c 226d  odal\" class=\"m
+00006470: 6f64 616c 5c22 2073 7479 6c65 3d5c 2264  odal\" style=\"d
+00006480: 6973 706c 6179 3a6e 6f6e 655c 2220 726f  isplay:none\" ro
+00006490: 6c65 3d5c 2264 6961 6c6f 675c 220a 2020  le=\"dialog\".  
+000064a0: 2020 2020 2020 6172 6961 2d68 6964 6465        aria-hidde
+000064b0: 6e3d 5c22 7472 7565 5c22 3e5c 725c 6e5c  n=\"true\">\r\n\
+000064c0: 743c 6469 7620 636c 6173 733d 5c22 6d6f  t<div class=\"mo
+000064d0: 6461 6c2d 6469 616c 6f67 5c22 3e5c 725c  dal-dialog\">\r\
+000064e0: 6e5c 745c 743c 6469 7620 636c 6173 733d  n\t\t<div class=
+000064f0: 5c22 6d6f 6461 6c2d 636f 6e74 656e 745c  \"modal-content\
+00006500: 223e 5c72 5c6e 5c74 5c74 5c74 3c64 6976  ">\r\n\t\t\t<div
+00006510: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+00006520: 226d 6f64 616c 2d62 6f64 795c 223e 5c72  "modal-body\">\r
+00006530: 5c6e 5c74 5c74 5c74 5c74 3c64 6976 2063  \n\t\t\t\t<div c
+00006540: 6c61 7373 3d5c 2270 6167 652d 6865 6164  lass=\"page-head
+00006550: 6572 5c22 3e5c 725c 6e5c 745c 745c 745c  er\">\r\n\t\t\t\
+00006560: 745c 745c 725c 6e5c 745c 745c 745c 745c  t\t\r\n\t\t\t\t\
+00006570: 743c 6275 7474 6f6e 0a20 2020 2020 2020  t<button.       
+00006580: 2063 6c61 7373 3d5c 2270 756c 6c2d 7269   class=\"pull-ri
+00006590: 6768 7420 6274 6e2d 6469 736d 6973 735c  ght btn-dismiss\
+000065a0: 2220 6172 6961 2d6c 6162 656c 3d5c 2253  " aria-label=\"S
+000065b0: 756c 6a65 5c22 2064 6174 612d 6163 7469  ulje\" data-acti
+000065c0: 6f6e 3d5c 2263 616e 6365 6c2d 616c 6c5c  on=\"cancel-all\
+000065d0: 223e 3c2f 6275 7474 6f6e 3e5c 725c 6e0a  "></button>\r\n.
+000065e0: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+000065f0: 2020 2020 2020 2020 2020 2020 3c68 313e              <h1>
+00006600: 5469 6c61 6120 796c 696d 5c78 4534 5c78  Tilaa ylim\xE4\x
+00006610: 4534 725c 7845 3469 6e65 6e20 7479 686a  E4r\xE4inen tyhj
+00006620: 656e 6e79 733c 2f68 313e 5c72 5c6e 5c74  ennys</h1>\r\n\t
+00006630: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
+00006640: 5c74 5c74 5c74 5c74 3c64 6976 0a20 2020  \t\t\t\t<div.   
+00006650: 2020 2020 2063 6c61 7373 3d5c 2266 6f72       class=\"for
+00006660: 6d5c 223e 3c2f 6469 763e 5c72 5c6e 5c74  m\"></div>\r\n\t
+00006670: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
+00006680: 3d5c 2267 6c6f 6261 6c2d 7661 6c69 6461  =\"global-valida
+00006690: 7469 6f6e 2d65 7272 6f72 2061 6c65 7274  tion-error alert
+000066a0: 0a20 2020 2020 2020 2061 6c65 7274 2d64  .        alert-d
+000066b0: 616e 6765 725c 2220 7374 796c 653d 5c22  anger\" style=\"
+000066c0: 6469 7370 6c61 793a 6e6f 6e65 5c22 3e5c  display:none\">\
+000066d0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+000066e0: 2020 2020 2020 2054 5c78 4534 7974 5c78         T\xE4yt\x
+000066f0: 4534 0a20 2020 2020 2020 2070 7575 7474  E4.        puutt
+00006700: 7576 6174 206b 656e 745c 7845 3474 5c72  uvat kent\xE4t\r
+00006710: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00006720: 2020 3c2f 6469 763e 5c72 5c6e 5c74 5c74    </div>\r\n\t\t
+00006730: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
+00006740: 3c2f 6469 763e 5c72 5c6e 5c74 3c2f 6469  </div>\r\n\t</di
+00006750: 763e 5c72 5c6e 3c2f 6469 763e 5c72 5c6e  v>\r\n</div>\r\n
+00006760: 5c72 5c6e 5c72 5c6e 5c72 5c6e 3c64 6976  \r\n\r\n\r\n<div
+00006770: 0a20 2020 2020 2020 2069 643d 5c22 6372  .        id=\"cr
+00006780: 6561 7465 2d6e 6577 2d75 7365 722d 6d6f  eate-new-user-mo
+00006790: 6461 6c5c 2220 636c 6173 733d 5c22 6d6f  dal\" class=\"mo
+000067a0: 6461 6c5c 2220 7374 796c 653d 5c22 6469  dal\" style=\"di
+000067b0: 7370 6c61 793a 6e6f 6e65 5c22 3e5c 725c  splay:none\">\r\
+000067c0: 6e5c 743c 6469 760a 2020 2020 2020 2020  n\t<div.        
+000067d0: 636c 6173 733d 5c22 6d6f 6461 6c2d 6469  class=\"modal-di
+000067e0: 616c 6f67 5c22 3e5c 725c 6e5c 745c 743c  alog\">\r\n\t\t<
+000067f0: 6469 7620 636c 6173 733d 5c22 6d6f 6461  div class=\"moda
+00006800: 6c2d 636f 6e74 656e 745c 223e 5c72 5c6e  l-content\">\r\n
+00006810: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
+00006820: 2020 2063 6c61 7373 3d5c 226d 6f64 616c     class=\"modal
+00006830: 2d62 6f64 795c 223e 5c72 5c6e 5c74 5c74  -body\">\r\n\t\t
+00006840: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
+00006850: 2270 6167 652d 6865 6164 6572 5c22 3e5c  "page-header\">\
+00006860: 725c 6e5c 745c 745c 745c 745c 745c 725c  r\n\t\t\t\t\t\r\
+00006870: 6e5c 745c 745c 745c 745c 743c 6831 3e4c  n\t\t\t\t\t<h1>L
+00006880: 756f 0a20 2020 2020 2020 2075 7573 6920  uo.        uusi 
+00006890: 7475 6e6e 7573 3c2f 6831 3e5c 725c 6e5c  tunnus</h1>\r\n\
+000068a0: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
+000068b0: 6e5c 725c 6e5c 745c 745c 745c 743c 6469  n\r\n\t\t\t\t<di
+000068c0: 7620 636c 6173 733d 5c22 666f 726d 2066  v class=\"form f
+000068d0: 6f72 6d43 6f6c 5c22 3e3c 2f64 6976 3e5c  ormCol\"></div>\
+000068e0: 725c 6e5c 745c 745c 743c 2f64 6976 3e5c  r\n\t\t\t</div>\
+000068f0: 725c 6e5c 745c 743c 2f64 6976 3e5c 725c  r\n\t\t</div>\r\
+00006900: 6e5c 743c 2f64 6976 3e5c 725c 6e3c 2f64  n\t</div>\r\n</d
+00006910: 6976 3e5c 725c 6e5c 725c 6e5c 725c 6e5c  iv>\r\n\r\n\r\n\
+00006920: 725c 6e3c 6469 760a 2020 2020 2020 2020  r\n<div.        
+00006930: 6964 3d5c 2265 6d61 696c 2d70 686f 6e65  id=\"email-phone
+00006940: 2d6d 6f64 616c 5c22 2063 6c61 7373 3d5c  -modal\" class=\
+00006950: 226d 6f64 616c 5c22 2073 7479 6c65 3d5c  "modal\" style=\
+00006960: 2264 6973 706c 6179 3a6e 6f6e 655c 223e  "display:none\">
+00006970: 5c72 5c6e 5c74 3c64 6976 0a20 2020 2020  \r\n\t<div.     
+00006980: 2020 2063 6c61 7373 3d5c 226d 6f64 616c     class=\"modal
+00006990: 2d64 6961 6c6f 675c 223e 5c72 5c6e 5c74  -dialog\">\r\n\t
+000069a0: 5c74 3c64 6976 2063 6c61 7373 3d5c 226d  \t<div class=\"m
+000069b0: 6f64 616c 2d63 6f6e 7465 6e74 5c22 3e5c  odal-content\">\
+000069c0: 725c 6e5c 745c 745c 743c 6469 760a 2020  r\n\t\t\t<div.  
+000069d0: 2020 2020 2020 636c 6173 733d 5c22 6d6f        class=\"mo
+000069e0: 6461 6c2d 626f 6479 5c22 3e5c 725c 6e5c  dal-body\">\r\n\
+000069f0: 745c 745c 745c 743c 6469 7620 636c 6173  t\t\t\t<div clas
+00006a00: 733d 5c22 7061 6765 2d68 6561 6465 725c  s=\"page-header\
+00006a10: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
+00006a20: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c68  \r\n\t\t\t\t\t<h
+00006a30: 313e 416e 6e61 0a20 2020 2020 2020 2073  1>Anna.        s
+00006a40: 5c78 4534 686b 5c78 4636 706f 7374 6920  \xE4hk\xF6posti 
+00006a50: 6a61 2070 7568 656c 696e 6e75 6d65 726f  ja puhelinnumero
+00006a60: 3c2f 6831 3e5c 725c 6e5c 745c 745c 745c  </h1>\r\n\t\t\t\
+00006a70: 743c 2f64 6976 3e5c 725c 6e5c 725c 6e5c  t</div>\r\n\r\n\
+00006a80: 745c 745c 745c 743c 6469 760a 2020 2020  t\t\t\t<div.    
+00006a90: 2020 2020 636c 6173 733d 5c22 666f 726d      class=\"form
+00006aa0: 2066 6f72 6d43 6f6c 5c22 3e3c 2f64 6976   formCol\"></div
+00006ab0: 3e5c 725c 6e5c 745c 745c 743c 2f64 6976  >\r\n\t\t\t</div
+00006ac0: 3e5c 725c 6e5c 745c 743c 2f64 6976 3e5c  >\r\n\t\t</div>\
+00006ad0: 725c 6e5c 743c 2f64 6976 3e5c 725c 6e3c  r\n\t</div>\r\n<
+00006ae0: 2f64 6976 3e5c 725c 6e5c 725c 6e5c 725c  /div>\r\n\r\n\r\
+00006af0: 6e5c 725c 6e3c 6469 760a 2020 2020 2020  n\r\n<div.      
+00006b00: 2020 6964 3d5c 2263 7265 6174 652d 6e65    id=\"create-ne
+00006b10: 772d 7365 7276 6963 652d 6d6f 6461 6c5c  w-service-modal\
+00006b20: 2220 636c 6173 733d 5c22 6d6f 6461 6c5c  " class=\"modal\
+00006b30: 2220 7374 796c 653d 5c22 6469 7370 6c61  " style=\"displa
+00006b40: 793a 6e6f 6e65 5c22 3e5c 725c 6e5c 743c  y:none\">\r\n\t<
+00006b50: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
+00006b60: 733d 5c22 6d6f 6461 6c2d 6469 616c 6f67  s=\"modal-dialog
+00006b70: 206d 6f64 616c 2d6c 675c 223e 5c72 5c6e   modal-lg\">\r\n
+00006b80: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
+00006b90: 226d 6f64 616c 2d63 6f6e 7465 6e74 5c22  "modal-content\"
+00006ba0: 3e5c 725c 6e5c 745c 745c 743c 6469 760a  >\r\n\t\t\t<div.
+00006bb0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+00006bc0: 6d6f 6461 6c2d 626f 6479 5c22 3e5c 725c  modal-body\">\r\
+00006bd0: 6e5c 745c 745c 745c 743c 6469 7620 636c  n\t\t\t\t<div cl
+00006be0: 6173 733d 5c22 7061 6765 2d68 6561 6465  ass=\"page-heade
+00006bf0: 725c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  r\">\r\n\t\t\t\t
+00006c00: 5c74 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  \t\r\n\t\t\t\t\t
+00006c10: 3c62 7574 746f 6e0a 2020 2020 2020 2020  <button.        
+00006c20: 636c 6173 733d 5c22 7075 6c6c 2d72 6967  class=\"pull-rig
+00006c30: 6874 2062 746e 2d64 6973 6d69 7373 5c22  ht btn-dismiss\"
+00006c40: 2061 7269 612d 6c61 6265 6c3d 5c22 5375   aria-label=\"Su
+00006c50: 6c6a 655c 2220 6461 7461 2d61 6374 696f  lje\" data-actio
+00006c60: 6e3d 5c22 6361 6e63 656c 2d61 6c6c 5c22  n=\"cancel-all\"
+00006c70: 3e3c 2f62 7574 746f 6e3e 5c72 5c6e 0a20  ></button>\r\n. 
+00006c80: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+00006c90: 2020 2020 2020 2020 2020 203c 6831 3e55             <h1>U
+00006ca0: 7564 656e 2070 616c 7665 6c75 6e20 7469  uden palvelun ti
+00006cb0: 6c61 7573 3c2f 6831 3e5c 725c 6e5c 745c  laus</h1>\r\n\t\
+00006cc0: 745c 745c 743c 2f64 6976 3e5c 725c 6e20  t\t\t</div>\r\n 
+00006cd0: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00006ce0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00006cf0: 2020 2020 2020 2020 2020 2020 3c68 333e              <h3>
+00006d00: 5479 686a 656e 6e79 736b 6f68 6465 3c2f  Tyhjennyskohde</
+00006d10: 6833 3e5c 725c 6e20 2020 2020 2020 2020  h3>\r\n         
+00006d20: 2020 2020 2020 205c 725c 6e20 2020 2020         \r\n     
+00006d30: 2020 2020 2020 2020 2020 203c 6164 6472             <addr
+00006d40: 6573 733e 5c72 5c6e 0a20 2020 2020 2020  ess>\r\n.       
+00006d50: 205c 2020 2020 2020 2020 2020 2020 2020   \              
+00006d60: 2020 2020 203c 7374 726f 6e67 3e3c 7370       <strong><sp
+00006d70: 616e 2064 6174 612d 726f 6c65 3d5c 226e  an data-role=\"n
+00006d80: 616d 655c 223e 3c2f 7370 616e 3e3c 2f73  ame\"></span></s
+00006d90: 7472 6f6e 673e 3c62 723e 5c72 5c6e 0a20  trong><br>\r\n. 
+00006da0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+00006db0: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+00006dc0: 2064 6174 612d 726f 6c65 3d5c 2261 6464   data-role=\"add
+00006dd0: 7265 7373 5c22 3e3c 2f73 7061 6e3e 3c62  ress\"></span><b
+00006de0: 723e 5c72 5c6e 2020 2020 2020 2020 2020  r>\r\n          
+00006df0: 2020 2020 2020 2020 2020 3c73 7061 6e0a            <span.
+00006e00: 2020 2020 2020 2020 6461 7461 2d72 6f6c          data-rol
+00006e10: 653d 5c22 706f 7374 5c22 3e3c 2f73 7061  e=\"post\"></spa
+00006e20: 6e3e 5c72 5c6e 2020 2020 2020 2020 2020  n>\r\n          
+00006e30: 2020 2020 2020 3c2f 6164 6472 6573 733e        </address>
+00006e40: 5c72 5c6e 5c72 5c6e 5c74 5c74 5c74 5c74  \r\n\r\n\t\t\t\t
+00006e50: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
+00006e60: 7373 3d5c 2266 6f72 6d5c 223e 3c2f 6469  ss=\"form\"></di
+00006e70: 763e 5c72 5c6e 5c72 5c6e 5c74 5c74 5c74  v>\r\n\r\n\t\t\t
+00006e80: 5c74 3c64 6976 2063 6c61 7373 3d5c 2267  \t<div class=\"g
+00006e90: 6c6f 6261 6c2d 7661 6c69 6461 7469 6f6e  lobal-validation
+00006ea0: 2d65 7272 6f72 0a20 2020 2020 2020 2061  -error.        a
+00006eb0: 6c65 7274 2061 6c65 7274 2d64 616e 6765  lert alert-dange
+00006ec0: 725c 2220 7374 796c 653d 5c22 6469 7370  r\" style=\"disp
+00006ed0: 6c61 793a 6e6f 6e65 5c22 3e5c 725c 6e5c  lay:none\">\r\n\
+00006ee0: 745c 7420 2020 205c 745c 7454 5c78 4534  t\t    \t\tT\xE4
+00006ef0: 7974 5c78 4534 2070 7575 7474 7576 6174  yt\xE4 puuttuvat
+00006f00: 0a20 2020 2020 2020 206b 656e 745c 7845  .        kent\xE
+00006f10: 3474 5c72 5c6e 5c74 5c74 2020 2020 5c74  4t\r\n\t\t    \t
+00006f20: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
+00006f30: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 3c2f  </div>\r\n\t\t</
+00006f40: 6469 763e 5c72 5c6e 5c74 3c2f 6469 763e  div>\r\n\t</div>
+00006f50: 5c72 5c6e 3c2f 6469 763e 5c72 5c6e 5c72  \r\n</div>\r\n\r
+00006f60: 5c6e 5c72 5c6e 5c72 5c6e 3c64 6976 0a20  \n\r\n\r\n<div. 
+00006f70: 2020 2020 2020 2069 643d 5c22 6368 616e         id=\"chan
+00006f80: 6765 2d70 6173 7377 6f72 642d 6d6f 6461  ge-password-moda
+00006f90: 6c5c 2220 636c 6173 733d 5c22 6d6f 6461  l\" class=\"moda
+00006fa0: 6c5c 2220 7374 796c 653d 5c22 6469 7370  l\" style=\"disp
+00006fb0: 6c61 793a 6e6f 6e65 5c22 3e5c 725c 6e5c  lay:none\">\r\n\
+00006fc0: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
+00006fd0: 6173 733d 5c22 6d6f 6461 6c2d 6469 616c  ass=\"modal-dial
+00006fe0: 6f67 5c22 3e5c 725c 6e5c 745c 743c 6469  og\">\r\n\t\t<di
+00006ff0: 7620 636c 6173 733d 5c22 6d6f 6461 6c2d  v class=\"modal-
+00007000: 636f 6e74 656e 745c 223e 5c72 5c6e 5c74  content\">\r\n\t
+00007010: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
+00007020: 2063 6c61 7373 3d5c 226d 6f64 616c 2d68   class=\"modal-h
+00007030: 6561 6465 725c 223e 5c72 5c6e 5c74 5c74  eader\">\r\n\t\t
+00007040: 5c74 5c74 5661 6968 6461 2073 616c 6173  \t\tVaihda salas
+00007050: 616e 615c 725c 6e5c 745c 745c 743c 2f64  ana\r\n\t\t\t</d
+00007060: 6976 3e5c 725c 6e5c 745c 745c 743c 6469  iv>\r\n\t\t\t<di
+00007070: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
+00007080: 5c22 6d6f 6461 6c2d 626f 6479 5c22 3e5c  \"modal-body\">\
+00007090: 725c 6e5c 745c 745c 745c 743c 6469 7620  r\n\t\t\t\t<div 
+000070a0: 636c 6173 733d 5c22 666f 726d 2066 6f72  class=\"form for
+000070b0: 6d43 6f6c 5c22 3e3c 2f64 6976 3e5c 725c  mCol\"></div>\r\
+000070c0: 6e5c 745c 745c 743c 2f64 6976 3e5c 725c  n\t\t\t</div>\r\
+000070d0: 6e5c 745c 743c 2f64 6976 3e5c 725c 6e5c  n\t\t</div>\r\n\
+000070e0: 743c 2f64 6976 3e5c 725c 6e3c 2f64 6976  t</div>\r\n</div
+000070f0: 3e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  >\r\n\r\n\r\n\r\
+00007100: 6e3c 6469 760a 2020 2020 2020 2020 6964  n<div.        id
+00007110: 3d5c 2263 6861 6e67 652d 7365 7276 6963  =\"change-servic
+00007120: 652d 6d6f 6461 6c5c 2220 636c 6173 733d  e-modal\" class=
+00007130: 5c22 6d6f 6461 6c5c 2220 7374 796c 653d  \"modal\" style=
+00007140: 5c22 6469 7370 6c61 793a 6e6f 6e65 5c22  \"display:none\"
+00007150: 3e5c 725c 6e5c 743c 6469 760a 2020 2020  >\r\n\t<div.    
+00007160: 2020 2020 636c 6173 733d 5c22 6d6f 6461      class=\"moda
+00007170: 6c2d 6469 616c 6f67 5c22 3e5c 725c 6e5c  l-dialog\">\r\n\
+00007180: 745c 743c 6469 7620 636c 6173 733d 5c22  t\t<div class=\"
+00007190: 6d6f 6461 6c2d 636f 6e74 656e 745c 223e  modal-content\">
+000071a0: 5c72 5c6e 5c74 5c74 5c74 3c64 6976 0a20  \r\n\t\t\t<div. 
+000071b0: 2020 2020 2020 2063 6c61 7373 3d5c 226d         class=\"m
+000071c0: 6f64 616c 2d62 6f64 795c 223e 5c72 5c6e  odal-body\">\r\n
+000071d0: 5c74 5c74 5c74 5c74 3c64 6976 2063 6c61  \t\t\t\t<div cla
+000071e0: 7373 3d5c 2270 6167 652d 6865 6164 6572  ss=\"page-header
+000071f0: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
+00007200: 745c 725c 6e5c 745c 745c 745c 745c 743c  t\r\n\t\t\t\t\t<
+00007210: 6275 7474 6f6e 0a20 2020 2020 2020 2063  button.        c
+00007220: 6c61 7373 3d5c 2270 756c 6c2d 7269 6768  lass=\"pull-righ
+00007230: 7420 6274 6e2d 6469 736d 6973 735c 2220  t btn-dismiss\" 
+00007240: 6172 6961 2d6c 6162 656c 3d5c 2253 756c  aria-label=\"Sul
+00007250: 6a65 5c22 2064 6174 612d 6163 7469 6f6e  je\" data-action
+00007260: 3d5c 2263 616e 6365 6c2d 616c 6c5c 223e  =\"cancel-all\">
+00007270: 3c2f 6275 7474 6f6e 3e5c 725c 6e0a 2020  </button>\r\n.  
+00007280: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+00007290: 2020 2020 2020 2020 2020 3c68 313e 5061            <h1>Pa
+000072a0: 6c76 656c 756d 7575 746f 733c 2f68 313e  lvelumuutos</h1>
+000072b0: 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f 6469  \r\n\t\t\t\t</di
+000072c0: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 3c64  v>\r\n\t\t\t\t<d
+000072d0: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+000072e0: 3d5c 2266 6f72 6d5c 223e 3c2f 6469 763e  =\"form\"></div>
+000072f0: 5c72 5c6e 5c74 5c74 5c74 5c74 3c64 6976  \r\n\t\t\t\t<div
+00007300: 2063 6c61 7373 3d5c 2267 6c6f 6261 6c2d   class=\"global-
+00007310: 7661 6c69 6461 7469 6f6e 2d65 7272 6f72  validation-error
+00007320: 2061 6c65 7274 0a20 2020 2020 2020 2061   alert.        a
+00007330: 6c65 7274 2d64 616e 6765 725c 2220 7374  lert-danger\" st
+00007340: 796c 653d 5c22 6469 7370 6c61 793a 6e6f  yle=\"display:no
+00007350: 6e65 5c22 3e5c 725c 6e20 2020 2020 2020  ne\">\r\n       
+00007360: 2020 2020 2020 2020 2020 2020 2054 5c78               T\x
+00007370: 4534 7974 5c78 4534 0a20 2020 2020 2020  E4yt\xE4.       
+00007380: 2070 7575 7474 7576 6174 206b 656e 745c   puuttuvat kent\
+00007390: 7845 3474 5c72 5c6e 2020 2020 2020 2020  xE4t\r\n        
+000073a0: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
+000073b0: 5c6e 5c74 5c74 5c74 3c2f 6469 763e 5c72  \n\t\t\t</div>\r
+000073c0: 5c6e 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \n\t\t</div>\r\n
+000073d0: 5c74 3c2f 6469 763e 5c72 5c6e 3c2f 6469  \t</div>\r\n</di
+000073e0: 763e 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72  v>\r\n\r\n\r\n\r
+000073f0: 5c6e 3c64 6976 0a20 2020 2020 2020 2069  \n<div.        i
+00007400: 643d 5c22 6372 6561 7465 2d6b 696d 7070  d=\"create-kimpp
+00007410: 612d 6d6f 6461 6c5c 2220 636c 6173 733d  a-modal\" class=
+00007420: 5c22 6d6f 6461 6c5c 2220 7374 796c 653d  \"modal\" style=
+00007430: 5c22 6469 7370 6c61 793a 6e6f 6e65 5c22  \"display:none\"
+00007440: 3e5c 725c 6e5c 743c 6469 760a 2020 2020  >\r\n\t<div.    
+00007450: 2020 2020 636c 6173 733d 5c22 6d6f 6461      class=\"moda
+00007460: 6c2d 6469 616c 6f67 206d 6f64 616c 2d6c  l-dialog modal-l
+00007470: 675c 223e 5c72 5c6e 5c74 5c74 3c64 6976  g\">\r\n\t\t<div
+00007480: 2063 6c61 7373 3d5c 226d 6f64 616c 2d63   class=\"modal-c
+00007490: 6f6e 7465 6e74 5c22 3e5c 725c 6e5c 745c  ontent\">\r\n\t\
+000074a0: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
+000074b0: 636c 6173 733d 5c22 6d6f 6461 6c2d 626f  class=\"modal-bo
+000074c0: 6479 5c22 3e5c 725c 6e5c 745c 745c 745c  dy\">\r\n\t\t\t\
+000074d0: 743c 6469 7620 636c 6173 733d 5c22 7061  t<div class=\"pa
+000074e0: 6765 2d68 6561 6465 725c 223e 5c72 5c6e  ge-header\">\r\n
+000074f0: 5c74 5c74 5c74 5c74 5c74 5c72 5c6e 5c74  \t\t\t\t\t\r\n\t
+00007500: 5c74 5c74 5c74 5c74 3c62 7574 746f 6e0a  \t\t\t\t<button.
+00007510: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+00007520: 7075 6c6c 2d72 6967 6874 2062 746e 2d64  pull-right btn-d
+00007530: 6973 6d69 7373 5c22 2061 7269 612d 6c61  ismiss\" aria-la
+00007540: 6265 6c3d 5c22 5375 6c6a 655c 2220 6461  bel=\"Sulje\" da
+00007550: 7461 2d61 6374 696f 6e3d 5c22 6361 6e63  ta-action=\"canc
+00007560: 656c 2d61 6c6c 5c22 3e3c 2f62 7574 746f  el-all\"></butto
+00007570: 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  n>\r\n\t\t\t\t\t
+00007580: 3c68 313e 5061 6c76 656c 7573 7461 0a20  <h1>Palvelusta. 
+00007590: 2020 2020 2020 206b 696d 7061 6b73 693c         kimpaksi<
+000075a0: 2f68 313e 5c72 5c6e 5c74 5c74 5c74 5c74  /h1>\r\n\t\t\t\t
+000075b0: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 5c74  </div>\r\n\r\n\t
+000075c0: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
+000075d0: 3d5c 2274 6578 742d 7269 6768 745c 223e  =\"text-right\">
+000075e0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c62  \r\n\t\t\t\t\t<b
+000075f0: 7574 746f 6e0a 2020 2020 2020 2020 636c  utton.        cl
+00007600: 6173 733d 5c22 6274 6e20 6274 6e2d 6c69  ass=\"btn btn-li
+00007610: 6e6b 5c22 2064 6174 612d 6163 7469 6f6e  nk\" data-action
+00007620: 3d5c 2270 7269 6e74 5c22 3e54 756c 6f73  =\"print\">Tulos
+00007630: 7461 206b 696d 7070 616c 7565 7474 656c  ta kimppaluettel
+00007640: 6f20 3c73 7061 6e0a 2020 2020 2020 2020  o <span.        
+00007650: 636c 6173 733d 5c22 676c 7970 6869 636f  class=\"glyphico
+00007660: 6e20 676c 7970 6869 636f 6e2d 7072 696e  n glyphicon-prin
+00007670: 745c 223e 3c2f 7370 616e 3e3c 2f62 7574  t\"></span></but
+00007680: 746f 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74  ton>\r\n\t\t\t\t
+00007690: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 5c74  </div>\r\n\r\n\t
+000076a0: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
+000076b0: 2020 2063 6c61 7373 3d5c 226b 696d 7070     class=\"kimpp
+000076c0: 615c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  a\">\r\n\t\t\t\t
+000076d0: 5c74 3c73 7479 6c65 2073 636f 7065 643e  \t<style scoped>
+000076e0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 2e6b  \r\n\t\t\t\t\t.k
+000076f0: 696d 7070 6120 7370 616e 2e69 7361 6e74  imppa span.isant
+00007700: 613a 6265 666f 7265 0a20 2020 2020 2020  a:before.       
+00007710: 207b 5c72 5c6e 5c74 5c74 5c74 5c74 5c74   {\r\n\t\t\t\t\t
+00007720: 5c74 636f 6e74 656e 743a 2027 4b69 6d70  \tcontent: 'Kimp
+00007730: 7061 6973 5c78 4534 6e74 5c78 4534 273b  pais\xE4nt\xE4';
+00007740: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 7d5c  \r\n\t\t\t\t\t}\
+00007750: 725c 6e5c 745c 745c 745c 745c 743c 2f73  r\n\t\t\t\t\t</s
+00007760: 7479 6c65 3e5c 725c 6e5c 745c 745c 745c  tyle>\r\n\t\t\t\
+00007770: 745c 745c 725c 6e5c 745c 745c 745c 745c  t\t\r\n\t\t\t\t\
+00007780: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
+00007790: 6173 733d 5c22 6772 6964 5c22 3e3c 2f64  ass=\"grid\"></d
+000077a0: 6976 3e5c 725c 6e5c 725c 6e5c 745c 745c  iv>\r\n\r\n\t\t\
+000077b0: 745c 745c 743c 7363 7269 7074 2069 643d  t\t\t<script id=
+000077c0: 5c22 6b69 6d70 7061 2d65 6469 742d 6d65  \"kimppa-edit-me
+000077d0: 6e75 2d74 656d 706c 6174 655c 220a 2020  nu-template\".  
+000077e0: 2020 2020 2020 7479 7065 3d5c 2274 6578        type=\"tex
+000077f0: 742f 782d 7465 6d70 6c61 7465 5c22 3e5c  t/x-template\">\
+00007800: 725c 6e5c 745c 745c 745c 745c 743c 6469  r\n\t\t\t\t\t<di
+00007810: 7620 636c 6173 733d 5c22 6d65 6e75 2065  v class=\"menu e
+00007820: 6469 742d 6d65 6e75 5c22 2064 6174 612d  dit-menu\" data-
+00007830: 726f 6c65 3d5c 2265 6469 742d 6d65 6e75  role=\"edit-menu
+00007840: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
+00007850: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
+00007860: 636c 6173 733d 5c22 726f 775c 223e 5c72  class=\"row\">\r
+00007870: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
+00007880: 3c64 6976 2063 6c61 7373 3d5c 2263 6f6c  <div class=\"col
+00007890: 2d78 732d 345c 223e 3c62 7574 746f 6e20  -xs-4\"><button 
+000078a0: 7479 7065 3d5c 2262 7574 746f 6e5c 220a  type=\"button\".
+000078b0: 2020 2020 2020 2020 6461 7461 2d61 6374          data-act
+000078c0: 696f 6e3d 5c22 6564 6974 2d6f 7361 6b61  ion=\"edit-osaka
+000078d0: 735c 2220 636c 6173 733d 5c22 6274 6e20  s\" class=\"btn 
+000078e0: 6274 6e2d 7072 696d 6172 7920 6274 6e2d  btn-primary btn-
+000078f0: 626c 6f63 6b5c 223e 5c72 5c6e 5c74 5c74  block\">\r\n\t\t
+00007900: 5c74 5c74 5c74 5c74 5c74 5c74 4d75 6f6b  \t\t\t\t\t\tMuok
+00007910: 6b61 615c 725c 6e5c 745c 745c 745c 745c  kaa\r\n\t\t\t\t\
+00007920: 745c 745c 743c 2f62 7574 746f 6e3e 3c2f  t\t\t</button></
+00007930: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
+00007940: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
+00007950: 2020 2063 6c61 7373 3d5c 2263 6f6c 2d78     class=\"col-x
+00007960: 732d 345c 223e 3c62 7574 746f 6e20 7479  s-4\"><button ty
+00007970: 7065 3d5c 2262 7574 746f 6e5c 2220 6461  pe=\"button\" da
+00007980: 7461 2d61 6374 696f 6e3d 5c22 636c 6f73  ta-action=\"clos
+00007990: 652d 6d65 6e75 5c22 2063 6c61 7373 3d5c  e-menu\" class=\
+000079a0: 2262 746e 0a20 2020 2020 2020 2062 746e  "btn.        btn
+000079b0: 2d70 7269 6d61 7279 2062 746e 2d62 6c6f  -primary btn-blo
+000079c0: 636b 5c22 3e5c 725c 6e5c 745c 745c 745c  ck\">\r\n\t\t\t\
+000079d0: 745c 745c 745c 745c 7450 6572 7575 7461  t\t\t\t\tPeruuta
+000079e0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+000079f0: 5c74 3c2f 6275 7474 6f6e 3e3c 2f64 6976  \t</button></div
+00007a00: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00007a10: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
+00007a20: 636c 6173 733d 5c22 636f 6c2d 7873 2d34  class=\"col-xs-4
+00007a30: 5c22 3e3c 6275 7474 6f6e 2074 7970 653d  \"><button type=
+00007a40: 5c22 6275 7474 6f6e 5c22 2064 6174 612d  \"button\" data-
+00007a50: 6163 7469 6f6e 3d5c 2264 656c 6574 652d  action=\"delete-
+00007a60: 726f 775c 2220 636c 6173 733d 5c22 6274  row\" class=\"bt
+00007a70: 6e0a 2020 2020 2020 2020 6274 6e2d 7072  n.        btn-pr
+00007a80: 696d 6172 7920 6274 6e2d 626c 6f63 6b5c  imary btn-block\
+00007a90: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
+00007aa0: 5c74 5c74 5c74 506f 6973 7461 5c72 5c6e  \t\t\tPoista\r\n
+00007ab0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \t\t\t\t\t\t\t</
+00007ac0: 6275 7474 6f6e 3e3c 2f64 6976 3e5c 725c  button></div>\r\
+00007ad0: 6e5c 745c 745c 745c 745c 745c 743c 2f64  n\t\t\t\t\t\t</d
+00007ae0: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
+00007af0: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
+00007b00: 745c 745c 743c 2f73 6372 6970 743e 5c72  t\t\t</script>\r
+00007b10: 5c6e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  \n\r\n\t\t\t\t\t
+00007b20: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
+00007b30: 6964 3d5c 226b 696d 7070 612d 7061 696e  id=\"kimppa-pain
+00007b40: 6f2d 6d65 6e75 2d74 656d 706c 6174 655c  o-menu-template\
+00007b50: 2220 7479 7065 3d5c 2274 6578 742f 782d  " type=\"text/x-
+00007b60: 7465 6d70 6c61 7465 5c22 3e5c 725c 6e5c  template\">\r\n\
+00007b70: 745c 745c 745c 745c 743c 6469 760a 2020  t\t\t\t\t<div.  
+00007b80: 2020 2020 2020 636c 6173 733d 5c22 6d65        class=\"me
+00007b90: 6e75 2070 6169 6e6f 2d6d 656e 755c 2220  nu paino-menu\" 
+00007ba0: 6461 7461 2d72 6f6c 653d 5c22 7061 696e  data-role=\"pain
+00007bb0: 6f2d 6d65 6e75 5c22 3e5c 725c 6e5c 745c  o-menu\">\r\n\t\
+00007bc0: 745c 745c 745c 745c 743c 6469 7620 636c  t\t\t\t\t<div cl
+00007bd0: 6173 733d 5c22 726f 770a 2020 2020 2020  ass=\"row.      
+00007be0: 2020 726f 772d 6365 6e74 6572 6564 5c22    row-centered\"
+00007bf0: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00007c00: 745c 743c 6469 7620 636c 6173 733d 5c22  t\t<div class=\"
+00007c10: 636f 6c2d 7873 2d34 2063 6f6c 2d63 656e  col-xs-4 col-cen
+00007c20: 7465 7265 645c 223e 3c62 7574 746f 6e0a  tered\"><button.
+00007c30: 2020 2020 2020 2020 7479 7065 3d5c 2262          type=\"b
+00007c40: 7574 746f 6e5c 2220 6461 7461 2d61 6374  utton\" data-act
+00007c50: 696f 6e3d 5c22 7365 742d 7061 696e 6f5c  ion=\"set-paino\
+00007c60: 2220 6461 7461 2d76 616c 7565 3d5c 2230  " data-value=\"0
+00007c70: 5c22 2063 6c61 7373 3d5c 2262 746e 2062  \" class=\"btn b
+00007c80: 746e 2d70 7269 6d61 7279 0a20 2020 2020  tn-primary.     
+00007c90: 2020 2062 746e 2d62 6c6f 636b 5c22 3e5c     btn-block\">\
+00007ca0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+00007cb0: 745c 7445 6920 6c61 736b 7574 6574 615c  t\tEi laskuteta\
+00007cc0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+00007cd0: 743c 2f62 7574 746f 6e3e 3c2f 6469 763e  t</button></div>
+00007ce0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+00007cf0: 5c74 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  \t\r\n\t\t\t\t\t
+00007d00: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
+00007d10: 2063 6c61 7373 3d5c 2263 6f6c 2d78 732d   class=\"col-xs-
+00007d20: 3420 636f 6c2d 6365 6e74 6572 6564 5c22  4 col-centered\"
+00007d30: 3e3c 6275 7474 6f6e 2074 7970 653d 5c22  ><button type=\"
+00007d40: 6275 7474 6f6e 5c22 2064 6174 612d 6163  button\" data-ac
+00007d50: 7469 6f6e 3d5c 2273 6574 2d70 6169 6e6f  tion=\"set-paino
+00007d60: 5c22 0a20 2020 2020 2020 2064 6174 612d  \".        data-
+00007d70: 7661 6c75 653d 5c22 325c 2220 636c 6173  value=\"2\" clas
+00007d80: 733d 5c22 6274 6e20 6274 6e2d 7072 696d  s=\"btn btn-prim
+00007d90: 6172 7920 6274 6e2d 626c 6f63 6b5c 223e  ary btn-block\">
+00007da0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+00007db0: 5c74 5c74 5661 6b69 7475 6973 656e 0a20  \t\tVakituisen. 
+00007dc0: 2020 2020 2020 206d 756b 6169 7365 7374         mukaisest
+00007dd0: 695c 725c 6e5c 745c 745c 745c 745c 745c  i\r\n\t\t\t\t\t\
+00007de0: 745c 743c 2f62 7574 746f 6e3e 3c2f 6469  t\t</button></di
+00007df0: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  v>\r\n\t\t\t\t\t
+00007e00: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 5c74  \t\t\r\n\t\t\t\t
+00007e10: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
+00007e20: 2020 2063 6c61 7373 3d5c 2263 6f6c 2d78     class=\"col-x
+00007e30: 732d 3420 636f 6c2d 6365 6e74 6572 6564  s-4 col-centered
+00007e40: 5c22 3e3c 6275 7474 6f6e 2074 7970 653d  \"><button type=
+00007e50: 5c22 6275 7474 6f6e 5c22 2064 6174 612d  \"button\" data-
+00007e60: 6163 7469 6f6e 3d5c 2273 6574 2d70 6169  action=\"set-pai
+00007e70: 6e6f 5c22 0a20 2020 2020 2020 2064 6174  no\".        dat
+00007e80: 612d 7661 6c75 653d 5c22 315c 2220 636c  a-value=\"1\" cl
+00007e90: 6173 733d 5c22 6274 6e20 6274 6e2d 7072  ass=\"btn btn-pr
+00007ea0: 696d 6172 7920 6274 6e2d 626c 6f63 6b5c  imary btn-block\
+00007eb0: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
+00007ec0: 5c74 5c74 5c74 5661 7061 612d 616a 616e  \t\t\tVapaa-ajan
+00007ed0: 0a20 2020 2020 2020 206d 756b 6169 7365  .        mukaise
+00007ee0: 7374 695c 725c 6e5c 745c 745c 745c 745c  sti\r\n\t\t\t\t\
+00007ef0: 745c 745c 743c 2f62 7574 746f 6e3e 3c2f  t\t\t</button></
+00007f00: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
+00007f10: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
+00007f20: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
+00007f30: 5c6e 5c74 5c74 5c74 5c74 5c74 3c2f 7363  \n\t\t\t\t\t</sc
+00007f40: 7269 7074 3e5c 725c 6e5c 725c 6e5c 745c  ript>\r\n\r\n\t\
+00007f50: 745c 745c 745c 743c 703e 4c61 736b 7574  t\t\t\t<p>Laskut
+00007f60: 7573 6f73 7575 6b73 6965 6e0a 2020 2020  usosuuksien.    
+00007f70: 2020 2020 7375 6d6d 6120 745c 7845 3479      summa t\xE4y
+00007f80: 7479 7920 6f6c 6c61 2031 3030 2025 2e20  tyy olla 100 %. 
+00007f90: 566f 6974 206a 616b 6161 206b 696d 7061  Voit jakaa kimpa
+00007fa0: 6e20 6c61 736b 7574 7573 6f73 7575 6465  n laskutusosuude
+00007fb0: 7420 6175 746f 6d61 6174 7469 7365 7374  t automaattisest
+00007fc0: 690a 2020 2020 2020 2020 616c 6c61 206f  i.        alla o
+00007fd0: 6c65 7661 6c6c 6120 7061 696e 696b 6b65  levalla painikke
+00007fe0: 656c 6c61 2c20 6a6f 6c6c 6f69 6e20 6c61  ella, jolloin la
+00007ff0: 736b 7574 7573 6f73 7575 6465 7420 6a61  skutusosuudet ja
+00008000: 6574 6161 6e20 6b69 696e 7465 6973 745c  etaan kiinteist\
+00008010: 7846 366e 0a20 2020 2020 2020 206b 5c78  xF6n.        k\x
+00008020: 4534 7974 745c 7846 3674 6172 6b6f 6974  E4ytt\xF6tarkoit
+00008030: 756b 7365 6e20 6d75 6b61 616e 2e20 566f  uksen mukaan. Vo
+00008040: 6974 206d 795c 7846 3673 2068 616c 7574  it my\xF6s halut
+00008050: 6573 7361 7369 2073 795c 7846 3674 745c  essasi sy\xF6tt\
+00008060: 7845 345c 7845 340a 2020 2020 2020 2020  xE4\xE4.        
+00008070: 6c61 736b 7574 7573 6f73 7575 6465 7420  laskutusosuudet 
+00008080: 6b5c 7845 3473 696e 2079 6c6c 5c78 4534  k\xE4sin yll\xE4
+00008090: 6f6c 6576 6969 6e20 6b65 6e74 7469 696e  oleviin kenttiin
+000080a0: 2e3c 2f70 3e5c 725c 6e5c 725c 6e5c 745c  .</p>\r\n\r\n\t\
+000080b0: 745c 745c 745c 743c 6469 760a 2020 2020  t\t\t\t<div.    
+000080c0: 2020 2020 636c 6173 733d 5c22 7465 7874      class=\"text
+000080d0: 2d63 656e 7465 725c 223e 5c72 5c6e 5c74  -center\">\r\n\t
+000080e0: 5c74 5c74 5c74 5c74 5c74 3c62 7574 746f  \t\t\t\t\t<butto
+000080f0: 6e20 7479 7065 3d5c 2262 7574 746f 6e5c  n type=\"button\
+00008100: 2220 636c 6173 733d 5c22 6274 6e0a 2020  " class=\"btn.  
+00008110: 2020 2020 2020 6274 6e2d 6465 6661 756c        btn-defaul
+00008120: 745c 2220 6461 7461 2d61 6374 696f 6e3d  t\" data-action=
+00008130: 5c22 6469 7374 7269 6275 7465 2d65 7665  \"distribute-eve
+00008140: 6e6c 795c 223e 4a61 6120 6c61 736b 7574  nly\">Jaa laskut
+00008150: 7573 2d25 2074 6173 616e 3c2f 6275 7474  us-% tasan</butt
+00008160: 6f6e 3e5c 725c 6e5c 745c 745c 745c 745c  on>\r\n\t\t\t\t\
+00008170: 743c 2f64 6976 3e5c 725c 6e5c 725c 6e5c  t</div>\r\n\r\n\
+00008180: 745c 745c 745c 745c 743c 6469 760a 2020  t\t\t\t\t<div.  
+00008190: 2020 2020 2020 636c 6173 733d 5c22 666f        class=\"fo
+000081a0: 726d 2d67 726f 7570 5c22 3e5c 725c 6e5c  rm-group\">\r\n\
+000081b0: 745c 745c 745c 745c 745c 743c 6c61 6265  t\t\t\t\t\t<labe
+000081c0: 6c20 666f 723d 5c22 4b49 4d43 6f6d 6d5c  l for=\"KIMComm\
+000081d0: 223e 4d75 7574 6f6b 7365 6e20 7379 793c  ">Muutoksen syy<
+000081e0: 2f6c 6162 656c 3e5c 725c 6e5c 745c 745c  /label>\r\n\t\t\
+000081f0: 745c 745c 745c 743c 7465 7874 6172 6561  t\t\t\t<textarea
+00008200: 0a20 2020 2020 2020 2069 643d 5c22 4b49  .        id=\"KI
+00008210: 4d43 6f6d 6d5c 2220 6e61 6d65 3d5c 224b  MComm\" name=\"K
+00008220: 494d 436f 6d6d 5c22 2063 6c61 7373 3d5c  IMComm\" class=\
+00008230: 2266 6f72 6d2d 636f 6e74 726f 6c5c 223e  "form-control\">
+00008240: 3c2f 7465 7874 6172 6561 3e5c 725c 6e5c  </textarea>\r\n\
+00008250: 745c 745c 745c 745c 743c 2f64 6976 3e5c  t\t\t\t\t</div>\
+00008260: 725c 6e5c 725c 6e5c 745c 745c 745c 745c  r\n\r\n\t\t\t\t\
+00008270: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
+00008280: 6173 733d 5c22 666f 726d 2d67 726f 7570  ass=\"form-group
+00008290: 205c 223e 5c72 5c6e 5c74 5c74 5c74 5c74   \">\r\n\t\t\t\t
+000082a0: 5c74 5c74 3c6c 6162 656c 2066 6f72 3d5c  \t\t<label for=\
+000082b0: 224b 4952 5076 6d5c 223e 4d75 7574 6f6b  "KIRPvm\">Muutok
+000082c0: 7365 7420 7475 6c65 7661 740a 2020 2020  set tulevat.    
+000082d0: 2020 2020 766f 696d 6161 6e3c 2f6c 6162      voimaan</lab
+000082e0: 656c 3e5c 725c 6e5c 745c 745c 745c 745c  el>\r\n\t\t\t\t\
+000082f0: 745c 743c 696e 7075 7420 6e61 6d65 3d5c  t\t<input name=\
+00008300: 224b 4952 5076 6d5c 2220 636c 6173 733d  "KIRPvm\" class=
+00008310: 5c22 666f 726d 2d63 6f6e 7472 6f6c 5c22  \"form-control\"
+00008320: 0a20 2020 2020 2020 203e 5c72 5c6e 5c74  .        >\r\n\t
+00008330: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
+00008340: 5c6e 5c72 5c6e 2020 2020 2020 2020 2020  \n\r\n          
+00008350: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00008360: 6c61 7373 3d5c 2266 6f72 6d2d 6772 6f75  lass=\"form-grou
+00008370: 705c 223e 5c72 5c6e 0a20 2020 2020 2020  p\">\r\n.       
+00008380: 205c 2020 2020 2020 2020 2020 2020 2020   \              
+00008390: 2020 2020 2020 2020 203c 6c61 6265 6c20           <label 
+000083a0: 666f 723d 5c22 6e6f 7469 6669 6572 7068  for=\"notifierph
+000083b0: 6f6e 655c 223e 496c 6d6f 6974 7461 6a61  one\">Ilmoittaja
+000083c0: 6e20 7075 6865 6c69 6e6e 756d 6572 6f3c  n puhelinnumero<
+000083d0: 2f6c 6162 656c 3e5c 725c 6e0a 2020 2020  /label>\r\n.    
+000083e0: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
+000083f0: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
+00008400: 7574 206e 616d 653d 5c22 6e6f 7469 6669  ut name=\"notifi
+00008410: 6572 7068 6f6e 655c 2220 7479 7065 3d5c  erphone\" type=\
+00008420: 2274 656c 5c22 2063 6c61 7373 3d5c 2266  "tel\" class=\"f
+00008430: 6f72 6d2d 636f 6e74 726f 6c5c 220a 2020  orm-control\".  
+00008440: 2020 2020 2020 7061 7474 6572 6e3d 5c22        pattern=\"
+00008450: 5e5c 5c73 2a5c 5c2b 3f28 5c5c 647c 5c5c  ^\\s*\\+?(\\d|\\
+00008460: 737c 2d29 2b24 5c22 2070 6c61 6365 686f  s|-)+$\" placeho
+00008470: 6c64 6572 3d5c 225c 223e 5c72 5c6e 2020  lder=\"\">\r\n  
+00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008490: 2020 3c2f 6469 763e 5c72 5c6e 5c72 5c6e    </div>\r\n\r\n
+000084a0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+000084b0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+000084c0: 7620 636c 6173 733d 5c22 666f 726d 2d67  v class=\"form-g
+000084d0: 726f 7570 5c22 3e5c 725c 6e20 2020 2020  roup\">\r\n     
+000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084f0: 2020 203c 6c61 6265 6c0a 2020 2020 2020     <label.      
+00008500: 2020 666f 723d 5c22 6e6f 7469 6669 6572    for=\"notifier
+00008510: 656d 6169 6c5c 223e 496c 6d6f 6974 7461  email\">Ilmoitta
+00008520: 6a61 6e20 735c 7845 3468 6b5c 7846 3670  jan s\xE4hk\xF6p
+00008530: 6f73 7469 6f73 6f69 7465 3c2f 6c61 6265  ostiosoite</labe
+00008540: 6c3e 5c72 5c6e 2020 2020 2020 2020 2020  l>\r\n          
+00008550: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
+00008560: 6e70 7574 0a20 2020 2020 2020 206e 616d  nput.        nam
+00008570: 653d 5c22 6e6f 7469 6669 6572 656d 6169  e=\"notifieremai
+00008580: 6c5c 2220 7479 7065 3d5c 2265 6d61 696c  l\" type=\"email
+00008590: 5c22 2063 6c61 7373 3d5c 2266 6f72 6d2d  \" class=\"form-
+000085a0: 636f 6e74 726f 6c5c 223e 5c72 5c6e 2020  control\">\r\n  
+000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085c0: 2020 3c2f 6469 763e 5c72 5c6e 5c74 5c74    </div>\r\n\t\t
+000085d0: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
+000085e0: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c72  \t\t</div>\r\n\r
+000085f0: 5c6e 5c74 5c74 5c74 3c64 6976 0a20 2020  \n\t\t\t<div.   
+00008600: 2020 2020 2063 6c61 7373 3d5c 226d 6f64       class=\"mod
+00008610: 616c 2d66 6f6f 7465 725c 223e 5c72 5c6e  al-footer\">\r\n
+00008620: 5c74 5c74 5c74 5c74 3c64 6976 2063 6c61  \t\t\t\t<div cla
+00008630: 7373 3d5c 2266 6f72 6d2d 6772 6f75 705c  ss=\"form-group\
+00008640: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
+00008650: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
+00008660: 7373 3d5c 2263 6865 636b 626f 7820 7465  ss=\"checkbox te
+00008670: 7874 2d6c 6566 745c 223e 5c72 5c6e 5c74  xt-left\">\r\n\t
+00008680: 5c74 5c74 5c74 5c74 5c74 3c6c 6162 656c  \t\t\t\t\t<label
+00008690: 3e3c 696e 7075 7420 7479 7065 3d5c 2263  ><input type=\"c
+000086a0: 6865 636b 626f 785c 220a 2020 2020 2020  heckbox\".      
+000086b0: 2020 6e61 6d65 3d5c 2263 6f6e 6669 726d    name=\"confirm
+000086c0: 2d63 6861 6e67 6573 5c22 3e20 4f6c 656e  -changes\"> Olen
+000086d0: 2074 6172 6b69 7374 616e 7574 206b 696d   tarkistanut kim
+000086e0: 7061 6e20 6c61 736b 7574 7573 6f73 7575  pan laskutusosuu
+000086f0: 6465 7420 6a61 2074 6965 646f 740a 2020  det ja tiedot.  
+00008700: 2020 2020 2020 6f76 6174 206f 696b 6569        ovat oikei
+00008710: 6e2e 3c2f 6c61 6265 6c3e 5c72 5c6e 5c74  n.</label>\r\n\t
+00008720: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
+00008730: 5c6e 5c74 5c74 5c74 5c74 3c2f 6469 763e  \n\t\t\t\t</div>
+00008740: 5c72 5c6e 5c74 5c74 5c74 5c74 3c64 6976  \r\n\t\t\t\t<div
+00008750: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+00008760: 2266 6f72 6d2d 6275 7474 6f6e 7320 7465  "form-buttons te
+00008770: 7874 2d63 656e 7465 725c 223e 5c72 5c6e  xt-center\">\r\n
+00008780: 5c74 5c74 5c74 5c74 5c74 3c62 7574 746f  \t\t\t\t\t<butto
+00008790: 6e20 636c 6173 733d 5c22 6274 6e20 6274  n class=\"btn bt
+000087a0: 6e2d 7072 696d 6172 795c 220a 2020 2020  n-primary\".    
+000087b0: 2020 2020 6461 7461 2d61 6374 696f 6e3d      data-action=
+000087c0: 5c22 7361 7665 2d6b 696d 7070 615c 2220  \"save-kimppa\" 
+000087d0: 6469 7361 626c 6564 3e4c 5c78 4534 6865  disabled>L\xE4he
+000087e0: 745c 7845 3420 6d75 7574 6f6b 7365 743c  t\xE4 muutokset<
+000087f0: 2f62 7574 746f 6e3e 5c72 5c6e 5c74 5c74  /button>\r\n\t\t
+00008800: 5c74 5c74 5c74 3c62 7574 746f 6e0a 2020  \t\t\t<button.  
+00008810: 2020 2020 2020 636c 6173 733d 5c22 6274        class=\"bt
+00008820: 6e20 6274 6e2d 7072 696d 6172 795c 2220  n btn-primary\" 
+00008830: 6461 7461 2d61 6374 696f 6e3d 5c22 6361  data-action=\"ca
+00008840: 6e63 656c 2d61 6c6c 5c22 3e50 6572 7575  ncel-all\">Peruu
+00008850: 7461 206d 7575 746f 6b73 6574 3c2f 6275  ta muutokset</bu
+00008860: 7474 6f6e 3e5c 725c 6e5c 745c 745c 745c  tton>\r\n\t\t\t\
+00008870: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
+00008880: 743c 2f64 6976 3e5c 725c 6e5c 745c 743c  t</div>\r\n\t\t<
+00008890: 2f64 6976 3e5c 725c 6e5c 743c 2f64 6976  /div>\r\n\t</div
+000088a0: 3e5c 725c 6e3c 2f64 6976 3e5c 725c 6e5c  >\r\n</div>\r\n\
+000088b0: 725c 6e5c 725c 6e5c 725c 6e5c 725c 6e5c  r\n\r\n\r\n\r\n\
+000088c0: 725c 6e3c 6469 760a 2020 2020 2020 2020  r\n<div.        
+000088d0: 6964 3d5c 2265 6469 742d 6b69 6d70 7061  id=\"edit-kimppa
+000088e0: 2d6d 6f64 616c 5c22 2063 6c61 7373 3d5c  -modal\" class=\
+000088f0: 226d 6f64 616c 5c22 2073 7479 6c65 3d5c  "modal\" style=\
+00008900: 2264 6973 706c 6179 3a6e 6f6e 655c 223e  "display:none\">
+00008910: 5c72 5c6e 5c74 3c64 6976 0a20 2020 2020  \r\n\t<div.     
+00008920: 2020 2063 6c61 7373 3d5c 226d 6f64 616c     class=\"modal
+00008930: 2d64 6961 6c6f 6720 6d6f 6461 6c2d 6c67  -dialog modal-lg
+00008940: 5c22 3e5c 725c 6e5c 745c 743c 6469 7620  \">\r\n\t\t<div 
+00008950: 636c 6173 733d 5c22 6d6f 6461 6c2d 636f  class=\"modal-co
+00008960: 6e74 656e 745c 223e 5c72 5c6e 5c74 5c74  ntent\">\r\n\t\t
+00008970: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
+00008980: 6c61 7373 3d5c 226d 6f64 616c 2d62 6f64  lass=\"modal-bod
+00008990: 795c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  y\">\r\n\t\t\t\t
+000089a0: 3c64 6976 2063 6c61 7373 3d5c 2270 6167  <div class=\"pag
+000089b0: 652d 6865 6164 6572 5c22 3e5c 725c 6e5c  e-header\">\r\n\
+000089c0: 745c 745c 745c 745c 745c 725c 6e5c 745c  t\t\t\t\t\r\n\t\
+000089d0: 745c 745c 745c 743c 6275 7474 6f6e 0a20  t\t\t\t<button. 
+000089e0: 2020 2020 2020 2063 6c61 7373 3d5c 2270         class=\"p
+000089f0: 756c 6c2d 7269 6768 7420 6274 6e2d 6469  ull-right btn-di
+00008a00: 736d 6973 735c 2220 6172 6961 2d6c 6162  smiss\" aria-lab
+00008a10: 656c 3d5c 2253 756c 6a65 5c22 2064 6174  el=\"Sulje\" dat
+00008a20: 612d 6163 7469 6f6e 3d5c 2263 616e 6365  a-action=\"cance
+00008a30: 6c2d 616c 6c5c 223e 3c2f 6275 7474 6f6e  l-all\"></button
+00008a40: 3e5c 725c 6e5c 745c 745c 745c 745c 743c  >\r\n\t\t\t\t\t<
+00008a50: 6831 3e4d 756f 6b6b 6161 0a20 2020 2020  h1>Muokkaa.     
+00008a60: 2020 206b 696d 7070 6161 3c2f 6831 3e5c     kimppaa</h1>\
+00008a70: 725c 6e5c 745c 745c 745c 743c 2f64 6976  r\n\t\t\t\t</div
+00008a80: 3e5c 725c 6e5c 745c 745c 745c 745c 725c  >\r\n\t\t\t\t\r\
+00008a90: 6e5c 745c 745c 745c 743c 6469 7620 636c  n\t\t\t\t<div cl
+00008aa0: 6173 733d 5c22 7465 7874 2d72 6967 6874  ass=\"text-right
+00008ab0: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
+00008ac0: 743c 6275 7474 6f6e 0a20 2020 2020 2020  t<button.       
+00008ad0: 2063 6c61 7373 3d5c 2262 746e 2062 746e   class=\"btn btn
+00008ae0: 2d6c 696e 6b5c 2220 6461 7461 2d61 6374  -link\" data-act
+00008af0: 696f 6e3d 5c22 7072 696e 745c 223e 5475  ion=\"print\">Tu
+00008b00: 6c6f 7374 6120 6b69 6d70 7061 6c75 6574  losta kimppaluet
+00008b10: 7465 6c6f 203c 7370 616e 0a20 2020 2020  telo <span.     
+00008b20: 2020 2063 6c61 7373 3d5c 2267 6c79 7068     class=\"glyph
+00008b30: 6963 6f6e 2067 6c79 7068 6963 6f6e 2d70  icon glyphicon-p
+00008b40: 7269 6e74 5c22 3e3c 2f73 7061 6e3e 3c2f  rint\"></span></
+00008b50: 6275 7474 6f6e 3e5c 725c 6e5c 745c 745c  button>\r\n\t\t\
+00008b60: 745c 743c 2f64 6976 3e5c 725c 6e5c 725c  t\t</div>\r\n\r\
+00008b70: 6e5c 745c 745c 745c 743c 6469 760a 2020  n\t\t\t\t<div.  
+00008b80: 2020 2020 2020 636c 6173 733d 5c22 6b69        class=\"ki
+00008b90: 6d70 7061 5c22 3e5c 725c 6e5c 745c 745c  mppa\">\r\n\t\t\
+00008ba0: 745c 745c 743c 7374 796c 6520 7363 6f70  t\t\t<style scop
+00008bb0: 6564 3e5c 725c 6e5c 745c 745c 745c 745c  ed>\r\n\t\t\t\t\
+00008bc0: 742e 6b69 6d70 7061 2073 7061 6e2e 6973  t.kimppa span.is
+00008bd0: 616e 7461 3a62 6566 6f72 650a 2020 2020  anta:before.    
+00008be0: 2020 2020 7b5c 725c 6e5c 745c 745c 745c      {\r\n\t\t\t\
+00008bf0: 745c 745c 7463 6f6e 7465 6e74 3a20 274b  t\t\tcontent: 'K
+00008c00: 696d 7070 6169 735c 7845 346e 745c 7845  imppais\xE4nt\xE
+00008c10: 3427 3b5c 725c 6e5c 745c 745c 745c 745c  4';\r\n\t\t\t\t\
+00008c20: 747d 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  t}\r\n\t\t\t\t\t
+00008c30: 3c2f 7374 796c 653e 5c72 5c6e 5c72 5c6e  </style>\r\n\r\n
+00008c40: 5c74 5c74 5c74 5c74 5c74 3c64 6976 0a20  \t\t\t\t\t<div. 
+00008c50: 2020 2020 2020 2063 6c61 7373 3d5c 2267         class=\"g
+00008c60: 7269 645c 223e 3c2f 6469 763e 5c72 5c6e  rid\"></div>\r\n
+00008c70: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c73  \r\n\t\t\t\t\t<s
+00008c80: 6372 6970 7420 6964 3d5c 226b 696d 7070  cript id=\"kimpp
+00008c90: 612d 6564 6974 2d6d 656e 752d 7465 6d70  a-edit-menu-temp
+00008ca0: 6c61 7465 5c22 0a20 2020 2020 2020 2074  late\".        t
+00008cb0: 7970 653d 5c22 7465 7874 2f78 2d74 656d  ype=\"text/x-tem
+00008cc0: 706c 6174 655c 223e 5c72 5c6e 5c74 5c74  plate\">\r\n\t\t
+00008cd0: 5c74 5c74 5c74 5c74 3c64 6976 2063 6c61  \t\t\t\t<div cla
+00008ce0: 7373 3d5c 226d 656e 7520 6564 6974 2d6d  ss=\"menu edit-m
+00008cf0: 656e 755c 2220 6461 7461 2d72 6f6c 653d  enu\" data-role=
+00008d00: 5c22 6564 6974 2d6d 656e 755c 223e 5c72  \"edit-menu\">\r
+00008d10: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
+00008d20: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
+00008d30: 7373 3d5c 2272 6f77 5c22 3e5c 725c 6e5c  ss=\"row\">\r\n\
+00008d40: 745c 745c 745c 745c 745c 745c 745c 743c  t\t\t\t\t\t\t\t<
+00008d50: 6469 7620 636c 6173 733d 5c22 636f 6c2d  div class=\"col-
+00008d60: 7873 2d34 5c22 3e5c 725c 6e5c 745c 745c  xs-4\">\r\n\t\t\
+00008d70: 745c 745c 745c 745c 745c 745c 743c 6275  t\t\t\t\t\t\t<bu
+00008d80: 7474 6f6e 0a20 2020 2020 2020 2074 7970  tton.        typ
+00008d90: 653d 5c22 6275 7474 6f6e 5c22 2064 6174  e=\"button\" dat
+00008da0: 612d 6163 7469 6f6e 3d5c 2265 6469 742d  a-action=\"edit-
+00008db0: 6f73 616b 6173 5c22 2063 6c61 7373 3d5c  osakas\" class=\
+00008dc0: 2262 746e 2062 746e 2d70 7269 6d61 7279  "btn btn-primary
+00008dd0: 2062 746e 2d62 6c6f 636b 5c22 3e5c 725c   btn-block\">\r\
+00008de0: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
+00008df0: 745c 745c 744d 756f 6b6b 6161 5c72 5c6e  t\t\tMuokkaa\r\n
+00008e00: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+00008e10: 5c74 3c2f 6275 7474 6f6e 3e5c 725c 6e5c  \t</button>\r\n\
+00008e20: 745c 745c 745c 745c 745c 745c 745c 743c  t\t\t\t\t\t\t\t<
+00008e30: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
+00008e40: 745c 745c 745c 745c 743c 6469 760a 2020  t\t\t\t\t<div.  
+00008e50: 2020 2020 2020 636c 6173 733d 5c22 636f        class=\"co
+00008e60: 6c2d 7873 2d34 5c22 3e5c 725c 6e5c 745c  l-xs-4\">\r\n\t\
+00008e70: 745c 745c 745c 745c 745c 745c 745c 743c  t\t\t\t\t\t\t\t<
+00008e80: 6275 7474 6f6e 2074 7970 653d 5c22 6275  button type=\"bu
+00008e90: 7474 6f6e 5c22 2064 6174 612d 6163 7469  tton\" data-acti
+00008ea0: 6f6e 3d5c 2263 6c6f 7365 2d6d 656e 755c  on=\"close-menu\
+00008eb0: 220a 2020 2020 2020 2020 636c 6173 733d  ".        class=
+00008ec0: 5c22 6274 6e20 6274 6e2d 7072 696d 6172  \"btn btn-primar
+00008ed0: 7920 6274 6e2d 626c 6f63 6b5c 223e 5c72  y btn-block\">\r
+00008ee0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
+00008ef0: 5c74 5c74 5c74 5065 7275 7574 615c 725c  \t\t\tPeruuta\r\
+00008f00: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
+00008f10: 745c 743c 2f62 7574 746f 6e3e 5c72 5c6e  t\t</button>\r\n
+00008f20: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+00008f30: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
+00008f40: 5c74 5c74 5c74 5c74 5c74 3c64 6976 0a20  \t\t\t\t\t<div. 
+00008f50: 2020 2020 2020 2063 6c61 7373 3d5c 2263         class=\"c
+00008f60: 6f6c 2d78 732d 345c 223e 5c72 5c6e 5c74  ol-xs-4\">\r\n\t
+00008f70: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+00008f80: 3c62 7574 746f 6e20 7479 7065 3d5c 2262  <button type=\"b
+00008f90: 7574 746f 6e5c 2220 6461 7461 2d61 6374  utton\" data-act
+00008fa0: 696f 6e3d 5c22 6465 6c65 7465 2d72 6f77  ion=\"delete-row
+00008fb0: 5c22 0a20 2020 2020 2020 2063 6c61 7373  \".        class
+00008fc0: 3d5c 2262 746e 2062 746e 2d70 7269 6d61  =\"btn btn-prima
+00008fd0: 7279 2062 746e 2d62 6c6f 636b 5c22 3e5c  ry btn-block\">\
+00008fe0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+00008ff0: 745c 745c 745c 7450 6f69 7374 615c 725c  t\t\t\tPoista\r\
+00009000: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
+00009010: 745c 743c 2f62 7574 746f 6e3e 5c72 5c6e  t\t</button>\r\n
+00009020: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+00009030: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
+00009040: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
+00009050: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \n\t\t\t\t\t\t</
+00009060: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
+00009070: 5c74 3c2f 7363 7269 7074 3e5c 725c 6e5c  \t</script>\r\n\
+00009080: 725c 6e5c 745c 745c 745c 745c 743c 7363  r\n\t\t\t\t\t<sc
+00009090: 7269 7074 0a20 2020 2020 2020 2069 643d  ript.        id=
+000090a0: 5c22 6b69 6d70 7061 2d70 6169 6e6f 2d6d  \"kimppa-paino-m
+000090b0: 656e 752d 7465 6d70 6c61 7465 5c22 2074  enu-template\" t
+000090c0: 7970 653d 5c22 7465 7874 2f78 2d74 656d  ype=\"text/x-tem
+000090d0: 706c 6174 655c 223e 5c72 5c6e 5c74 5c74  plate\">\r\n\t\t
+000090e0: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
+000090f0: 2020 2063 6c61 7373 3d5c 226d 656e 7520     class=\"menu 
+00009100: 7061 696e 6f2d 6d65 6e75 5c22 2064 6174  paino-menu\" dat
+00009110: 612d 726f 6c65 3d5c 2270 6169 6e6f 2d6d  a-role=\"paino-m
+00009120: 656e 755c 223e 5c72 5c6e 5c74 5c74 5c74  enu\">\r\n\t\t\t
+00009130: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
+00009140: 3d5c 2272 6f77 0a20 2020 2020 2020 2072  =\"row.        r
+00009150: 6f77 2d63 656e 7465 7265 645c 223e 5c72  ow-centered\">\r
+00009160: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
+00009170: 3c64 6976 2063 6c61 7373 3d5c 2263 6f6c  <div class=\"col
+00009180: 2d78 732d 3420 636f 6c2d 6365 6e74 6572  -xs-4 col-center
+00009190: 6564 5c22 3e3c 6275 7474 6f6e 0a20 2020  ed\"><button.   
+000091a0: 2020 2020 2074 7970 653d 5c22 6275 7474       type=\"butt
+000091b0: 6f6e 5c22 2064 6174 612d 6163 7469 6f6e  on\" data-action
+000091c0: 3d5c 2273 6574 2d70 6169 6e6f 5c22 2064  =\"set-paino\" d
+000091d0: 6174 612d 7661 6c75 653d 5c22 305c 2220  ata-value=\"0\" 
+000091e0: 636c 6173 733d 5c22 6274 6e20 6274 6e2d  class=\"btn btn-
+000091f0: 7072 696d 6172 790a 2020 2020 2020 2020  primary.        
+00009200: 6274 6e2d 626c 6f63 6b5c 223e 5c72 5c6e  btn-block\">\r\n
+00009210: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+00009220: 4569 206c 6173 6b75 7465 7461 5c72 5c6e  Ei laskuteta\r\n
+00009230: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \t\t\t\t\t\t\t</
+00009240: 6275 7474 6f6e 3e3c 2f64 6976 3e5c 725c  button></div>\r\
+00009250: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
+00009260: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+00009270: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
+00009280: 6173 733d 5c22 636f 6c2d 7873 2d34 2063  ass=\"col-xs-4 c
+00009290: 6f6c 2d63 656e 7465 7265 645c 223e 3c62  ol-centered\"><b
+000092a0: 7574 746f 6e20 7479 7065 3d5c 2262 7574  utton type=\"but
+000092b0: 746f 6e5c 2220 6461 7461 2d61 6374 696f  ton\" data-actio
+000092c0: 6e3d 5c22 7365 742d 7061 696e 6f5c 220a  n=\"set-paino\".
+000092d0: 2020 2020 2020 2020 6461 7461 2d76 616c          data-val
+000092e0: 7565 3d5c 2232 5c22 2063 6c61 7373 3d5c  ue=\"2\" class=\
+000092f0: 2262 746e 2062 746e 2d70 7269 6d61 7279  "btn btn-primary
+00009300: 2062 746e 2d62 6c6f 636b 5c22 3e5c 725c   btn-block\">\r\
+00009310: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
+00009320: 7456 616b 6974 7569 7365 6e0a 2020 2020  tVakituisen.    
+00009330: 2020 2020 6d75 6b61 6973 6573 7469 5c72      mukaisesti\r
+00009340: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
+00009350: 3c2f 6275 7474 6f6e 3e3c 2f64 6976 3e5c  </button></div>\
+00009360: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+00009370: 745c 725c 6e5c 745c 745c 745c 745c 745c  t\r\n\t\t\t\t\t\
+00009380: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
+00009390: 636c 6173 733d 5c22 636f 6c2d 7873 2d34  class=\"col-xs-4
+000093a0: 2063 6f6c 2d63 656e 7465 7265 645c 223e   col-centered\">
+000093b0: 3c62 7574 746f 6e20 7479 7065 3d5c 2262  <button type=\"b
+000093c0: 7574 746f 6e5c 2220 6461 7461 2d61 6374  utton\" data-act
+000093d0: 696f 6e3d 5c22 7365 742d 7061 696e 6f5c  ion=\"set-paino\
+000093e0: 220a 2020 2020 2020 2020 6461 7461 2d76  ".        data-v
+000093f0: 616c 7565 3d5c 2231 5c22 2063 6c61 7373  alue=\"1\" class
+00009400: 3d5c 2262 746e 2062 746e 2d70 7269 6d61  =\"btn btn-prima
+00009410: 7279 2062 746e 2d62 6c6f 636b 5c22 3e5c  ry btn-block\">\
+00009420: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+00009430: 745c 7456 6170 6161 2d61 6a61 6e0a 2020  t\tVapaa-ajan.  
+00009440: 2020 2020 2020 6d75 6b61 6973 6573 7469        mukaisesti
+00009450: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+00009460: 5c74 3c2f 6275 7474 6f6e 3e3c 2f64 6976  \t</button></div
+00009470: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00009480: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
+00009490: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
+000094a0: 745c 745c 745c 745c 743c 2f73 6372 6970  t\t\t\t\t</scrip
+000094b0: 743e 5c72 5c6e 5c72 5c6e 5c74 5c74 5c74  t>\r\n\r\n\t\t\t
+000094c0: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 5c74  \t\t\r\n\t\t\t\t
+000094d0: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 5c74  \t\t\r\n\t\t\t\t
+000094e0: 5c74 5c74 5c74 3c70 3e4a 6f73 0a20 2020  \t\t\t<p>Jos.   
+000094f0: 2020 2020 206b 696d 7061 6e20 6f73 616b       kimpan osak
+00009500: 6169 7373 6120 6f6e 2074 6170 6168 7475  aissa on tapahtu
+00009510: 6e75 7420 6d75 7574 6f6b 7369 612c 2070  nut muutoksia, p
+00009520: 6f69 7374 6120 6f73 616b 6173 206a 6120  oista osakas ja 
+00009530: 6c75 6f20 7575 7369 2e3c 2f70 3e5c 725c  luo uusi.</p>\r\
+00009540: 6e5c 745c 745c 745c 745c 745c 745c 725c  n\t\t\t\t\t\t\r\
+00009550: 6e5c 725c 6e5c 745c 745c 745c 745c 745c  n\r\n\t\t\t\t\t\
+00009560: 743c 703e 4c61 736b 7574 7573 6f73 7575  t<p>Laskutusosuu
+00009570: 6b73 6965 6e0a 2020 2020 2020 2020 7375  ksien.        su
+00009580: 6d6d 6120 745c 7845 3479 7479 7920 6f6c  mma t\xE4ytyy ol
+00009590: 6c61 2031 3030 2025 2e20 566f 6974 206a  la 100 %. Voit j
+000095a0: 616b 6161 206b 696d 7061 6e20 6c61 736b  akaa kimpan lask
+000095b0: 7574 7573 6f73 7575 6465 7420 6175 746f  utusosuudet auto
+000095c0: 6d61 6174 7469 7365 7374 690a 2020 2020  maattisesti.    
+000095d0: 2020 2020 616c 6c61 206f 6c65 7661 6c6c      alla olevall
+000095e0: 6120 7061 696e 696b 6b65 656c 6c61 2c20  a painikkeella, 
+000095f0: 6a6f 6c6c 6f69 6e20 6c61 736b 7574 7573  jolloin laskutus
+00009600: 6f73 7575 6465 7420 6a61 6574 6161 6e20  osuudet jaetaan 
+00009610: 6b69 696e 7465 6973 745c 7846 366e 0a20  kiinteist\xF6n. 
+00009620: 2020 2020 2020 206b 5c78 4534 7974 745c         k\xE4ytt\
+00009630: 7846 3674 6172 6b6f 6974 756b 7365 6e20  xF6tarkoituksen 
+00009640: 6d75 6b61 616e 2e20 566f 6974 206d 795c  mukaan. Voit my\
+00009650: 7846 3673 2068 616c 7574 6573 7361 7369  xF6s halutessasi
+00009660: 2073 795c 7846 3674 745c 7845 345c 7845   sy\xF6tt\xE4\xE
+00009670: 340a 2020 2020 2020 2020 6c61 736b 7574  4.        laskut
+00009680: 7573 6f73 7575 6465 7420 6b5c 7845 3473  usosuudet k\xE4s
+00009690: 696e 2079 6c6c 5c78 4534 6f6c 6576 6969  in yll\xE4olevii
+000096a0: 6e20 6b65 6e74 7469 696e 2e3c 2f70 3e5c  n kenttiin.</p>\
+000096b0: 725c 6e5c 725c 6e5c 745c 745c 745c 745c  r\n\r\n\t\t\t\t\
+000096c0: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
+000096d0: 636c 6173 733d 5c22 7465 7874 2d63 656e  class=\"text-cen
+000096e0: 7465 725c 223e 5c72 5c6e 5c74 5c74 5c74  ter\">\r\n\t\t\t
+000096f0: 5c74 5c74 5c74 5c74 3c62 7574 746f 6e20  \t\t\t\t<button 
+00009700: 7479 7065 3d5c 2262 7574 746f 6e5c 2220  type=\"button\" 
+00009710: 636c 6173 733d 5c22 6274 6e0a 2020 2020  class=\"btn.    
+00009720: 2020 2020 6274 6e2d 6465 6661 756c 745c      btn-default\
+00009730: 2220 6461 7461 2d61 6374 696f 6e3d 5c22  " data-action=\"
+00009740: 6469 7374 7269 6275 7465 2d65 7665 6e6c  distribute-evenl
+00009750: 795c 223e 4a61 6120 6c61 736b 7574 7573  y\">Jaa laskutus
+00009760: 2d25 2074 6173 616e 3c2f 6275 7474 6f6e  -% tasan</button
+00009770: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00009780: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
+00009790: 745c 745c 745c 725c 6e5c 745c 745c 745c  t\t\t\r\n\t\t\t\
+000097a0: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+000097b0: 2020 636c 6173 733d 5c22 666f 726d 2d67    class=\"form-g
+000097c0: 726f 7570 5c22 3e5c 725c 6e5c 745c 745c  roup\">\r\n\t\t\
+000097d0: 745c 745c 745c 745c 743c 6c61 6265 6c20  t\t\t\t\t<label 
+000097e0: 666f 723d 5c22 4b49 4d43 6f6d 6d5c 223e  for=\"KIMComm\">
+000097f0: 4d75 7574 6f6b 7365 6e20 7379 793c 2f6c  Muutoksen syy</l
+00009800: 6162 656c 3e5c 725c 6e5c 745c 745c 745c  abel>\r\n\t\t\t\
+00009810: 745c 745c 745c 743c 7465 7874 6172 6561  t\t\t\t<textarea
+00009820: 0a20 2020 2020 2020 2069 643d 5c22 4b49  .        id=\"KI
+00009830: 4d43 6f6d 6d5c 2220 6e61 6d65 3d5c 224b  MComm\" name=\"K
+00009840: 494d 436f 6d6d 5c22 2063 6c61 7373 3d5c  IMComm\" class=\
+00009850: 2266 6f72 6d2d 636f 6e74 726f 6c5c 223e  "form-control\">
+00009860: 3c2f 7465 7874 6172 6561 3e5c 725c 6e5c  </textarea>\r\n\
+00009870: 745c 745c 745c 745c 745c 743c 2f64 6976  t\t\t\t\t\t</div
+00009880: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00009890: 725c 6e5c 745c 745c 745c 745c 745c 743c  r\n\t\t\t\t\t\t<
+000098a0: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
+000098b0: 733d 5c22 666f 726d 2d67 726f 7570 205c  s=\"form-group \
+000098c0: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
+000098d0: 5c74 5c74 3c6c 6162 656c 2066 6f72 3d5c  \t\t<label for=\
+000098e0: 224b 4952 5076 6d5c 223e 4d75 7574 6f6b  "KIRPvm\">Muutok
+000098f0: 7365 7420 7475 6c65 7661 740a 2020 2020  set tulevat.    
+00009900: 2020 2020 766f 696d 6161 6e3c 2f6c 6162      voimaan</lab
+00009910: 656c 3e5c 725c 6e5c 745c 745c 745c 745c  el>\r\n\t\t\t\t\
+00009920: 745c 745c 743c 696e 7075 7420 6e61 6d65  t\t\t<input name
+00009930: 3d5c 224b 4952 5076 6d5c 2220 636c 6173  =\"KIRPvm\" clas
+00009940: 733d 5c22 666f 726d 2d63 6f6e 7472 6f6c  s=\"form-control
+00009950: 5c22 0a20 2020 2020 2020 203e 5c72 5c6e  \".        >\r\n
+00009960: 5c74 5c74 5c74 5c74 5c74 5c74 3c2f 6469  \t\t\t\t\t\t</di
+00009970: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  v>\r\n\t\t\t\t\t
+00009980: 5c74 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  \t\r\n\t\t\t\t\t
+00009990: 5c74 3c64 6976 2063 6c61 7373 3d5c 2266  \t<div class=\"f
+000099a0: 6f72 6d2d 6772 6f75 705c 223e 5c72 5c6e  orm-group\">\r\n
+000099b0: 5c74 0a20 2020 2020 2020 205c 2020 2020  \t.        \    
+000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099d0: 2020 203c 6c61 6265 6c20 666f 723d 5c22     <label for=\"
+000099e0: 6e6f 7469 6669 6572 7068 6f6e 655c 223e  notifierphone\">
+000099f0: 496c 6d6f 6974 7461 6a61 6e20 7075 6865  Ilmoittajan puhe
+00009a00: 6c69 6e6e 756d 6572 6f3c 2f6c 6162 656c  linnumero</label
+00009a10: 3e5c 725c 6e5c 740a 2020 2020 2020 2020  >\r\n\t.        
+00009a20: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+00009a30: 2020 2020 2020 2020 3c69 6e70 7574 206e          <input n
+00009a40: 616d 653d 5c22 6e6f 7469 6669 6572 7068  ame=\"notifierph
+00009a50: 6f6e 655c 2220 7479 7065 3d5c 2274 656c  one\" type=\"tel
+00009a60: 5c22 2063 6c61 7373 3d5c 2266 6f72 6d2d  \" class=\"form-
+00009a70: 636f 6e74 726f 6c5c 220a 2020 2020 2020  control\".      
+00009a80: 2020 7061 7474 6572 6e3d 5c22 5e5c 5c73    pattern=\"^\\s
+00009a90: 2a5c 5c2b 3f28 5c5c 647c 5c5c 737c 2d29  *\\+?(\\d|\\s|-)
+00009aa0: 2b24 5c22 2070 6c61 6365 686f 6c64 6572  +$\" placeholder
+00009ab0: 3d5c 225c 223e 5c72 5c6e 5c74 2020 2020  =\"\">\r\n\t    
+00009ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ad0: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 5c74  </div>\r\n\r\n\t
+00009ae0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+00009af0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00009b00: 7620 636c 6173 733d 5c22 666f 726d 2d67  v class=\"form-g
+00009b10: 726f 7570 5c22 3e5c 725c 6e5c 7420 2020  roup\">\r\n\t   
+00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b30: 2020 2020 203c 6c61 6265 6c0a 2020 2020       <label.    
+00009b40: 2020 2020 666f 723d 5c22 6e6f 7469 6669      for=\"notifi
+00009b50: 6572 656d 6169 6c5c 223e 496c 6d6f 6974  eremail\">Ilmoit
+00009b60: 7461 6a61 6e20 735c 7845 3468 6b5c 7846  tajan s\xE4hk\xF
+00009b70: 3670 6f73 7469 6f73 6f69 7465 3c2f 6c61  6postiosoite</la
+00009b80: 6265 6c3e 5c72 5c6e 5c74 2020 2020 2020  bel>\r\n\t      
+00009b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ba0: 2020 3c69 6e70 7574 0a20 2020 2020 2020    <input.       
+00009bb0: 206e 616d 653d 5c22 6e6f 7469 6669 6572   name=\"notifier
+00009bc0: 656d 6169 6c5c 2220 7479 7065 3d5c 2265  email\" type=\"e
+00009bd0: 6d61 696c 5c22 2063 6c61 7373 3d5c 2266  mail\" class=\"f
+00009be0: 6f72 6d2d 636f 6e74 726f 6c5c 223e 5c72  orm-control\">\r
+00009bf0: 5c6e 5c74 2020 2020 2020 2020 2020 2020  \n\t            
+00009c00: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
+00009c10: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00009c20: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+00009c30: 725c 6e5c 745c 745c 745c 743c 2f64 6976  r\n\t\t\t\t</div
+00009c40: 3e5c 725c 6e5c 745c 745c 743c 2f64 6976  >\r\n\t\t\t</div
+00009c50: 3e5c 725c 6e5c 725c 6e5c 745c 745c 743c  >\r\n\r\n\t\t\t<
+00009c60: 6469 7620 636c 6173 733d 5c22 6d6f 6461  div class=\"moda
+00009c70: 6c2d 666f 6f74 6572 5c22 3e5c 725c 6e5c  l-footer\">\r\n\
+00009c80: 745c 745c 745c 745c 725c 6e5c 745c 745c  t\t\t\t\r\n\t\t\
+00009c90: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+00009ca0: 2020 636c 6173 733d 5c22 666f 726d 2d67    class=\"form-g
+00009cb0: 726f 7570 5c22 3e5c 725c 6e5c 745c 745c  roup\">\r\n\t\t\
+00009cc0: 745c 745c 745c 743c 6469 7620 636c 6173  t\t\t\t<div clas
+00009cd0: 733d 5c22 6368 6563 6b62 6f78 2074 6578  s=\"checkbox tex
+00009ce0: 742d 6c65 6674 5c22 3e5c 725c 6e5c 745c  t-left\">\r\n\t\
+00009cf0: 745c 745c 745c 745c 745c 743c 6c61 6265  t\t\t\t\t\t<labe
+00009d00: 6c3e 3c69 6e70 7574 0a20 2020 2020 2020  l><input.       
+00009d10: 2074 7970 653d 5c22 6368 6563 6b62 6f78   type=\"checkbox
+00009d20: 5c22 206e 616d 653d 5c22 636f 6e66 6972  \" name=\"confir
+00009d30: 6d2d 6368 616e 6765 735c 223e 204f 6c65  m-changes\"> Ole
+00009d40: 6e20 7461 726b 6973 7461 6e75 7420 6b69  n tarkistanut ki
+00009d50: 6d70 616e 206c 6173 6b75 7475 736f 7375  mpan laskutusosu
+00009d60: 7564 6574 0a20 2020 2020 2020 206a 6120  udet.        ja 
+00009d70: 7469 6564 6f74 206f 7661 7420 6f69 6b65  tiedot ovat oike
+00009d80: 696e 2e3c 2f6c 6162 656c 3e5c 725c 6e5c  in.</label>\r\n\
+00009d90: 745c 745c 745c 745c 745c 743c 2f64 6976  t\t\t\t\t\t</div
+00009da0: 3e5c 725c 6e5c 745c 745c 745c 745c 743c  >\r\n\t\t\t\t\t<
+00009db0: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
+00009dc0: 745c 725c 6e5c 725c 6e5c 745c 745c 745c  t\r\n\r\n\t\t\t\
+00009dd0: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
+00009de0: 6173 733d 5c22 666f 726d 2d62 7574 746f  ass=\"form-butto
+00009df0: 6e73 2074 6578 742d 6365 6e74 6572 5c22  ns text-center\"
+00009e00: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00009e10: 725c 6e5c 745c 745c 745c 745c 745c 743c  r\n\t\t\t\t\t\t<
+00009e20: 6275 7474 6f6e 2063 6c61 7373 3d5c 2262  button class=\"b
+00009e30: 746e 0a20 2020 2020 2020 2062 746e 2d70  tn.        btn-p
+00009e40: 7269 6d61 7279 5c22 2064 6174 612d 6163  rimary\" data-ac
+00009e50: 7469 6f6e 3d5c 2273 6176 652d 6b69 6d70  tion=\"save-kimp
+00009e60: 7061 5c22 2064 6973 6162 6c65 643e 5c72  pa\" disabled>\r
+00009e70: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
+00009e80: 4c5c 7845 3468 6574 5c78 4534 0a20 2020  L\xE4het\xE4.   
+00009e90: 2020 2020 206d 7575 746f 6b73 6574 5c72       muutokset\r
+00009ea0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \n\t\t\t\t\t\t</
+00009eb0: 6275 7474 6f6e 3e5c 725c 6e5c 745c 745c  button>\r\n\t\t\
+00009ec0: 745c 745c 745c 725c 6e5c 745c 745c 745c  t\t\t\r\n\t\t\t\
+00009ed0: 745c 743c 6275 7474 6f6e 2063 6c61 7373  t\t<button class
+00009ee0: 3d5c 2262 746e 0a20 2020 2020 2020 2062  =\"btn.        b
+00009ef0: 746e 2d70 7269 6d61 7279 5c22 2064 6174  tn-primary\" dat
+00009f00: 612d 6163 7469 6f6e 3d5c 2263 616e 6365  a-action=\"cance
+00009f10: 6c2d 616c 6c5c 223e 5c72 5c6e 5c74 5c74  l-all\">\r\n\t\t
+00009f20: 5c74 5c74 5c74 5c74 5065 7275 7574 6120  \t\t\t\tPeruuta 
+00009f30: 6d75 7574 6f6b 7365 745c 725c 6e5c 745c  muutokset\r\n\t\
+00009f40: 745c 745c 745c 743c 2f62 7574 746f 6e3e  t\t\t\t</button>
+00009f50: 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f 6469  \r\n\t\t\t\t</di
+00009f60: 763e 5c72 5c6e 5c74 5c74 5c74 3c2f 6469  v>\r\n\t\t\t</di
+00009f70: 763e 5c72 5c6e 5c74 5c74 3c2f 6469 763e  v>\r\n\t\t</div>
+00009f80: 5c72 5c6e 5c74 3c2f 6469 763e 5c72 5c6e  \r\n\t</div>\r\n
+00009f90: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 3c73  </div>\r\n\r\n<s
+00009fa0: 6372 6970 740a 2020 2020 2020 2020 6964  cript.        id
+00009fb0: 3d5c 226b 696d 7070 612d 7072 696e 742d  =\"kimppa-print-
+00009fc0: 7465 6d70 6c61 7465 5c22 2074 7970 653d  template\" type=
+00009fd0: 5c22 7465 7874 2f78 2d6b 656e 646f 2d74  \"text/x-kendo-t
+00009fe0: 656d 706c 6174 655c 223e 5c72 5c6e 5c74  emplate\">\r\n\t
+00009ff0: 3c6c 696e 6b20 7265 6c3d 5c22 7374 796c  <link rel=\"styl
+0000a000: 6573 6865 6574 5c22 0a20 2020 2020 2020  esheet\".       
+0000a010: 2068 7265 663d 5c22 2f6a 6174 656b 756b   href=\"/jatekuk
+0000a020: 6b6f 2f63 7373 2f73 6168 6173 2f6b 696d  ko/css/sahas/kim
+0000a030: 7070 612d 7072 696e 742e 6373 735c 223e  ppa-print.css\">
+0000a040: 5c72 5c6e 5c72 5c6e 5c74 3c68 6561 6465  \r\n\r\n\t<heade
+0000a050: 723e 5c72 5c6e 5c74 5c74 3c68 313e 3c64  r>\r\n\t\t<h1><d
+0000a060: 6976 3e4a 5c78 4534 7465 6b75 6b6b 6f0a  iv>J\xE4tekukko.
+0000a070: 2020 2020 2020 2020 4f79 3c2f 6469 763e          Oy</div>
+0000a080: 266e 6273 703b 266e 6273 703b 266e 6273  &nbsp;&nbsp;&nbs
+0000a090: 703b 266e 6273 703b 266e 6273 703b 266e  p;&nbsp;&nbsp;&n
+0000a0a0: 6273 703b 3c64 6976 3e4b 494d 5050 4120  bsp;<div>KIMPPA 
+0000a0b0: 233a 206e 616d 6520 233c 2f64 6976 3e3c  #: name #</div><
+0000a0c0: 2f68 313e 3c64 6976 0a20 2020 2020 2020  /h1><div.       
+0000a0d0: 2063 6c61 7373 3d5c 2264 6174 655c 223e   class=\"date\">
+0000a0e0: 233a 2064 6174 6520 233c 2f64 6976 3e5c  #: date #</div>\
+0000a0f0: 725c 6e5c 743c 2f68 6561 6465 723e 5c72  r\n\t</header>\r
+0000a100: 5c6e 5c74 3c74 6162 6c65 3e5c 725c 6e5c  \n\t<table>\r\n\
+0000a110: 745c 743c 7468 6561 643e 5c72 5c6e 5c74  t\t<thead>\r\n\t
+0000a120: 5c74 5c74 3c74 723e 5c72 5c6e 5c74 5c74  \t\t<tr>\r\n\t\t
+0000a130: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 5c74  \t\t\r\n\t\t\t\t
+0000a140: 3c74 683e 4e69 6d69 3c2f 7468 3e5c 725c  <th>Nimi</th>\r\
+0000a150: 6e5c 745c 745c 745c 743c 7468 3e4c 5c78  n\t\t\t\t<th>L\x
+0000a160: 4534 6869 6f73 6f69 7465 3c2f 7468 3e5c  E4hiosoite</th>\
+0000a170: 725c 6e5c 745c 745c 745c 743c 7468 3e4c  r\n\t\t\t\t<th>L
+0000a180: 6173 6b75 7475 736f 736f 6974 653c 2f74  askutusosoite</t
+0000a190: 683e 5c72 5c6e 5c74 5c74 5c74 5c74 3c74  h>\r\n\t\t\t\t<t
+0000a1a0: 680a 2020 2020 2020 2020 636c 6173 733d  h.        class=
+0000a1b0: 5c22 6e75 6d65 7269 635c 223e 5061 6c76  \"numeric\">Palv
+0000a1c0: 656c 752f 5072 6f73 2e6f 7375 7573 3c2f  elu/Pros.osuus</
+0000a1d0: 7468 3e5c 725c 6e5c 745c 745c 743c 2f74  th>\r\n\t\t\t</t
+0000a1e0: 723e 5c72 5c6e 5c74 5c74 3c2f 7468 6561  r>\r\n\t\t</thea
+0000a1f0: 643e 5c72 5c6e 5c74 5c74 3c74 626f 6479  d>\r\n\t\t<tbody
+0000a200: 3e5c 725c 6e5c 745c 7423 0a20 2020 2020  >\r\n\t\t#.     
+0000a210: 2020 2066 6f72 2876 6172 2069 203d 2030     for(var i = 0
+0000a220: 3b20 6920 3c20 726f 7773 2e6c 656e 6774  ; i < rows.lengt
+0000a230: 683b 202b 2b69 2920 7b20 7661 7220 726f  h; ++i) { var ro
+0000a240: 7720 3d20 726f 7773 5b69 5d3b 2023 5c72  w = rows[i]; #\r
+0000a250: 5c6e 5c74 5c74 5c74 3c74 723e 5c72 5c6e  \n\t\t\t<tr>\r\n
+0000a260: 5c74 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \t\t\t\t\r\n\t\t
+0000a270: 5c74 5c74 3c74 643e 233a 0a20 2020 2020  \t\t<td>#:.     
+0000a280: 2020 2072 6f77 2e6f 7361 6b61 732e 6e69     row.osakas.ni
+0000a290: 6d69 2023 3c2f 7464 3e5c 725c 6e5c 745c  mi #</td>\r\n\t\
+0000a2a0: 745c 745c 743c 7464 3e23 3a20 726f 772e  t\t\t<td>#: row.
+0000a2b0: 6f73 616b 6173 2e6b 6174 7520 233c 6272  osakas.katu #<br
+0000a2c0: 3e23 3a20 726f 772e 6f73 616b 6173 2e70  >#: row.osakas.p
+0000a2d0: 6f73 7469 0a20 2020 2020 2020 2023 3c2f  osti.        #</
+0000a2e0: 7464 3e5c 725c 6e5c 745c 745c 745c 743c  td>\r\n\t\t\t\t<
+0000a2f0: 7464 3e23 3a20 726f 772e 6f73 616b 6173  td>#: row.osakas
+0000a300: 2e6c 6173 6b75 7475 736b 6174 7520 233c  .laskutuskatu #<
+0000a310: 6272 3e23 3a20 726f 772e 6f73 616b 6173  br>#: row.osakas
+0000a320: 2e6c 6173 6b75 7475 7370 6f73 7469 0a20  .laskutusposti. 
+0000a330: 2020 2020 2020 2023 3c2f 7464 3e5c 725c         #</td>\r\
+0000a340: 6e5c 745c 745c 745c 743c 7464 2063 6c61  n\t\t\t\t<td cla
+0000a350: 7373 3d5c 226e 756d 6572 6963 5c22 3e23  ss=\"numeric\">#
+0000a360: 3a20 6b65 6e64 6f2e 746f 5374 7269 6e67  : kendo.toString
+0000a370: 2872 6f77 2e4b 4952 5072 6f73 2c20 276e  (row.KIRPros, 'n
+0000a380: 2729 0a20 2020 2020 2020 2023 2025 3c2f  ').        # %</
+0000a390: 7464 3e5c 725c 6e5c 745c 745c 743c 2f74  td>\r\n\t\t\t</t
+0000a3a0: 723e 5c72 5c6e 5c74 5c74 2320 7d20 235c  r>\r\n\t\t# } #\
+0000a3b0: 725c 6e5c 745c 743c 2f74 626f 6479 3e5c  r\n\t\t</tbody>\
+0000a3c0: 725c 6e5c 745c 743c 7466 6f6f 7465 723e  r\n\t\t<tfooter>
+0000a3d0: 5c72 5c6e 5c74 5c74 5c74 3c74 723e 5c72  \r\n\t\t\t<tr>\r
+0000a3e0: 5c6e 5c74 5c74 5c74 5c74 3c74 643e 3c2f  \n\t\t\t\t<td></
+0000a3f0: 7464 3e5c 725c 6e5c 745c 745c 745c 743c  td>\r\n\t\t\t\t<
+0000a400: 7464 3e3c 2f74 643e 5c72 5c6e 5c74 5c74  td></td>\r\n\t\t
+0000a410: 5c74 5c74 3c74 643e 3c2f 7464 3e5c 725c  \t\t<td></td>\r\
+0000a420: 6e5c 745c 745c 745c 743c 7464 0a20 2020  n\t\t\t\t<td.   
+0000a430: 2020 2020 2063 6c61 7373 3d5c 226e 756d       class=\"num
+0000a440: 6572 6963 5c22 3e59 6874 6565 6e73 5c78  eric\">Yhteens\x
+0000a450: 4534 3c2f 7464 3e5c 725c 6e5c 745c 745c  E4</td>\r\n\t\t\
+0000a460: 745c 743c 7464 2063 6c61 7373 3d5c 226e  t\t<td class=\"n
+0000a470: 756d 6572 6963 5c22 3e3c 7374 726f 6e67  umeric\"><strong
+0000a480: 3e23 3a0a 2020 2020 2020 2020 6b65 6e64  >#:.        kend
+0000a490: 6f2e 746f 5374 7269 6e67 2870 6572 6365  o.toString(perce
+0000a4a0: 6e74 5375 6d2c 2027 6e27 2920 2320 253c  ntSum, 'n') # %<
+0000a4b0: 2f73 7472 6f6e 673e 3c2f 7464 3e5c 725c  /strong></td>\r\
+0000a4c0: 6e5c 745c 745c 743c 2f74 723e 5c72 5c6e  n\t\t\t</tr>\r\n
+0000a4d0: 5c74 5c74 3c2f 7466 6f6f 7465 723e 5c72  \t\t</tfooter>\r
+0000a4e0: 5c6e 5c74 3c2f 7461 626c 653e 5c72 5c6e  \n\t</table>\r\n
+0000a4f0: 3c2f 7363 7269 7074 3e5c 725c 6e5c 725c  </script>\r\n\r\
+0000a500: 6e3c 6966 7261 6d65 0a20 2020 2020 2020  n<iframe.       
+0000a510: 206e 616d 653d 5c22 6b69 6d70 7061 2d70   name=\"kimppa-p
+0000a520: 7269 6e74 5c22 2077 6964 7468 3d5c 2230  rint\" width=\"0
+0000a530: 5c22 2068 6569 6768 743d 5c22 305c 2220  \" height=\"0\" 
+0000a540: 6672 616d 6562 6f72 6465 723d 5c22 305c  frameborder=\"0\
+0000a550: 2220 7372 633d 5c22 6162 6f75 743a 626c  " src=\"about:bl
+0000a560: 616e 6b5c 223e 3c2f 6966 7261 6d65 3e5c  ank\"></iframe>\
+0000a570: 725c 6e5c 725c 6e5c 725c 6e5c 725c 6e3c  r\n\r\n\r\n\r\n<
+0000a580: 6469 760a 2020 2020 2020 2020 6964 3d5c  div.        id=\
+0000a590: 2272 6573 6967 6e2d 6b69 6d70 7061 2d6d  "resign-kimppa-m
+0000a5a0: 6f64 616c 5c22 2063 6c61 7373 3d5c 226d  odal\" class=\"m
+0000a5b0: 6f64 616c 5c22 2073 7479 6c65 3d5c 2264  odal\" style=\"d
+0000a5c0: 6973 706c 6179 3a6e 6f6e 655c 223e 5c72  isplay:none\">\r
+0000a5d0: 5c6e 5c74 3c64 6976 0a20 2020 2020 2020  \n\t<div.       
+0000a5e0: 2063 6c61 7373 3d5c 226d 6f64 616c 2d64   class=\"modal-d
+0000a5f0: 6961 6c6f 6720 6d6f 6461 6c2d 6c67 5c22  ialog modal-lg\"
+0000a600: 3e5c 725c 6e5c 745c 743c 6469 7620 636c  >\r\n\t\t<div cl
+0000a610: 6173 733d 5c22 6d6f 6461 6c2d 636f 6e74  ass=\"modal-cont
+0000a620: 656e 745c 223e 5c72 5c6e 5c74 5c74 5c74  ent\">\r\n\t\t\t
+0000a630: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
+0000a640: 7373 3d5c 226d 6f64 616c 2d62 6f64 795c  ss=\"modal-body\
+0000a650: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 3c64  ">\r\n\t\t\t\t<d
+0000a660: 6976 2063 6c61 7373 3d5c 2270 6167 652d  iv class=\"page-
+0000a670: 6865 6164 6572 206c 696e 652d 7374 796c  header line-styl
+0000a680: 655c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  e\">\r\n\t\t\t\t
+0000a690: 5c74 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  \t\r\n\t\t\t\t\t
+0000a6a0: 3c62 7574 746f 6e0a 2020 2020 2020 2020  <button.        
+0000a6b0: 636c 6173 733d 5c22 7075 6c6c 2d72 6967  class=\"pull-rig
+0000a6c0: 6874 2062 746e 2d64 6973 6d69 7373 5c22  ht btn-dismiss\"
+0000a6d0: 2061 7269 612d 6c61 6265 6c3d 5c22 5375   aria-label=\"Su
+0000a6e0: 6c6a 655c 2220 6461 7461 2d61 6374 696f  lje\" data-actio
+0000a6f0: 6e3d 5c22 6361 6e63 656c 2d61 6c6c 5c22  n=\"cancel-all\"
+0000a700: 3e3c 2f62 7574 746f 6e3e 5c72 5c6e 0a20  ></button>\r\n. 
+0000a710: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+0000a720: 2020 2020 2020 2020 2020 203c 6832 3e45             <h2>E
+0000a730: 726f 6120 6b69 6d70 6173 7461 3c2f 6832  roa kimpasta</h2
+0000a740: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+0000a750: 2020 2020 203c 2f64 6976 3e5c 725c 6e5c       </div>\r\n\
+0000a760: 725c 6e5c 745c 745c 745c 743c 6469 760a  r\n\t\t\t\t<div.
+0000a770: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+0000a780: 666f 726d 5c22 3e3c 2f64 6976 3e5c 725c  form\"></div>\r\
+0000a790: 6e5c 745c 745c 745c 743c 6469 7620 636c  n\t\t\t\t<div cl
+0000a7a0: 6173 733d 5c22 676c 6f62 616c 2d76 616c  ass=\"global-val
+0000a7b0: 6964 6174 696f 6e2d 6572 726f 7220 616c  idation-error al
+0000a7c0: 6572 740a 2020 2020 2020 2020 616c 6572  ert.        aler
+0000a7d0: 742d 6461 6e67 6572 5c22 2073 7479 6c65  t-danger\" style
+0000a7e0: 3d5c 2264 6973 706c 6179 3a6e 6f6e 655c  =\"display:none\
+0000a7f0: 223e 545c 7845 3479 745c 7845 3420 7075  ">T\xE4yt\xE4 pu
+0000a800: 7574 7475 7661 7420 6b65 6e74 5c78 4534  uttuvat kent\xE4
+0000a810: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
+0000a820: 745c 745c 725c 6e5c 745c 745c 745c 743c  t\t\r\n\t\t\t\t<
+0000a830: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
+0000a840: 733d 5c22 616b 705c 223e 3c2f 6469 763e  s=\"akp\"></div>
+0000a850: 5c72 5c6e 5c74 5c74 5c74 5c74 3c64 6976  \r\n\t\t\t\t<div
+0000a860: 2063 6c61 7373 3d5c 2261 6b70 2d69 6e66   class=\"akp-inf
+0000a870: 6f5c 223e 3c2f 6469 763e 5c72 5c6e 5c74  o\"></div>\r\n\t
+0000a880: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
+0000a890: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 3c2f  \t</div>\r\n\t</
+0000a8a0: 6469 763e 5c72 5c6e 3c2f 6469 763e 5c72  div>\r\n</div>\r
+0000a8b0: 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e 3c64  \n\r\n\r\n\r\n<d
+0000a8c0: 6976 0a20 2020 2020 2020 2069 643d 5c22  iv.        id=\"
+0000a8d0: 616b 702d 6c6f 6361 7469 6f6e 2d6d 6f64  akp-location-mod
+0000a8e0: 616c 5c22 2063 6c61 7373 3d5c 226d 6f64  al\" class=\"mod
+0000a8f0: 616c 5c22 2073 7479 6c65 3d5c 2264 6973  al\" style=\"dis
+0000a900: 706c 6179 3a6e 6f6e 655c 223e 5c72 5c6e  play:none\">\r\n
+0000a910: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
+0000a920: 6c61 7373 3d5c 226d 6f64 616c 2d64 6961  lass=\"modal-dia
+0000a930: 6c6f 6720 6d6f 6461 6c2d 6c67 5c22 3e5c  log modal-lg\">\
+0000a940: 725c 6e5c 745c 743c 6469 7620 636c 6173  r\n\t\t<div clas
+0000a950: 733d 5c22 6d6f 6461 6c2d 636f 6e74 656e  s=\"modal-conten
+0000a960: 745c 223e 5c72 5c6e 5c74 5c74 5c74 3c64  t\">\r\n\t\t\t<d
+0000a970: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+0000a980: 3d5c 226d 6f64 616c 2d68 6561 6465 725c  =\"modal-header\
+0000a990: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5069  ">\r\n\t\t\t\tPi
+0000a9a0: 7374 6565 6e20 7369 6a61 696e 7469 202f  steen sijainti /
+0000a9b0: 2056 6169 6864 6120 7069 7374 6574 745c   Vaihda pistett\
+0000a9c0: 7845 345c 725c 6e5c 745c 745c 743c 2f64  xE4\r\n\t\t\t</d
+0000a9d0: 6976 3e5c 725c 6e5c 745c 745c 743c 6469  iv>\r\n\t\t\t<di
+0000a9e0: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
+0000a9f0: 5c22 6d6f 6461 6c2d 626f 6479 5c22 3e5c  \"modal-body\">\
+0000aa00: 725c 6e5c 745c 745c 745c 743c 6469 7620  r\n\t\t\t\t<div 
+0000aa10: 636c 6173 733d 5c22 616b 705c 223e 3c2f  class=\"akp\"></
+0000aa20: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
+0000aa30: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
+0000aa40: 7373 3d5c 2261 6b70 2d69 6e66 6f5c 223e  ss=\"akp-info\">
+0000aa50: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
+0000aa60: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 3c2f  </div>\r\n\t\t</
+0000aa70: 6469 763e 5c72 5c6e 5c74 3c2f 6469 763e  div>\r\n\t</div>
+0000aa80: 5c72 5c6e 3c2f 6469 763e 5c72 5c6e 5c72  \r\n</div>\r\n\r
+0000aa90: 5c6e 5c72 5c6e 5c72 5c6e 3c64 6976 0a20  \n\r\n\r\n<div. 
+0000aaa0: 2020 2020 2020 2069 643d 5c22 7265 7369         id=\"resi
+0000aab0: 676e 2d61 6b70 2d6d 6f64 616c 5c22 2063  gn-akp-modal\" c
+0000aac0: 6c61 7373 3d5c 226d 6f64 616c 5c22 2073  lass=\"modal\" s
+0000aad0: 7479 6c65 3d5c 2264 6973 706c 6179 3a6e  tyle=\"display:n
+0000aae0: 6f6e 655c 223e 5c72 5c6e 5c74 3c64 6976  one\">\r\n\t<div
+0000aaf0: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+0000ab00: 226d 6f64 616c 2d64 6961 6c6f 6720 6d6f  "modal-dialog mo
+0000ab10: 6461 6c2d 6c67 5c22 3e5c 725c 6e5c 745c  dal-lg\">\r\n\t\
+0000ab20: 743c 6469 7620 636c 6173 733d 5c22 6d6f  t<div class=\"mo
+0000ab30: 6461 6c2d 636f 6e74 656e 745c 223e 5c72  dal-content\">\r
+0000ab40: 5c6e 5c74 5c74 5c74 3c64 6976 0a20 2020  \n\t\t\t<div.   
+0000ab50: 2020 2020 2063 6c61 7373 3d5c 226d 6f64       class=\"mod
+0000ab60: 616c 2d68 6561 6465 725c 223e 5c72 5c6e  al-header\">\r\n
+0000ab70: 5c74 5c74 5c74 5c74 4c6f 7065 7461 2070  \t\t\t\tLopeta p
+0000ab80: 6973 7465 656e 206b 5c78 4534 7974 745c  isteen k\xE4ytt\
+0000ab90: 7846 365c 725c 6e5c 745c 745c 743c 2f64  xF6\r\n\t\t\t</d
+0000aba0: 6976 3e5c 725c 6e5c 745c 745c 743c 6469  iv>\r\n\t\t\t<di
+0000abb0: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
+0000abc0: 5c22 6d6f 6461 6c2d 626f 6479 5c22 3e5c  \"modal-body\">\
+0000abd0: 725c 6e5c 745c 745c 745c 743c 6469 7620  r\n\t\t\t\t<div 
+0000abe0: 636c 6173 733d 5c22 666f 726d 5c22 3e3c  class=\"form\"><
+0000abf0: 2f64 6976 3e5c 725c 6e5c 745c 745c 743c  /div>\r\n\t\t\t<
+0000ac00: 2f64 6976 3e5c 725c 6e5c 745c 743c 2f64  /div>\r\n\t\t</d
+0000ac10: 6976 3e5c 725c 6e5c 743c 2f64 6976 3e5c  iv>\r\n\t</div>\
+0000ac20: 725c 6e3c 2f64 6976 3e5c 725c 6e5c 725c  r\n</div>\r\n\r\
+0000ac30: 6e5c 725c 6e5c 725c 6e3c 6469 760a 2020  n\r\n\r\n<div.  
+0000ac40: 2020 2020 2020 6964 3d5c 2274 6572 6d69        id=\"termi
+0000ac50: 6e61 7465 2d73 6572 7669 6365 2d6d 6f64  nate-service-mod
+0000ac60: 616c 5c22 2063 6c61 7373 3d5c 226d 6f64  al\" class=\"mod
+0000ac70: 616c 5c22 2073 7479 6c65 3d5c 2264 6973  al\" style=\"dis
+0000ac80: 706c 6179 3a6e 6f6e 655c 223e 5c72 5c6e  play:none\">\r\n
+0000ac90: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
+0000aca0: 6c61 7373 3d5c 226d 6f64 616c 2d64 6961  lass=\"modal-dia
+0000acb0: 6c6f 675c 223e 5c72 5c6e 5c74 5c74 3c64  log\">\r\n\t\t<d
+0000acc0: 6976 2063 6c61 7373 3d5c 226d 6f64 616c  iv class=\"modal
+0000acd0: 2d63 6f6e 7465 6e74 5c22 3e5c 725c 6e5c  -content\">\r\n\
+0000ace0: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+0000acf0: 2020 636c 6173 733d 5c22 6d6f 6461 6c2d    class=\"modal-
+0000ad00: 626f 6479 5c22 3e5c 725c 6e5c 745c 745c  body\">\r\n\t\t\
+0000ad10: 745c 745c 725c 6e5c 745c 745c 745c 743c  t\t\r\n\t\t\t\t<
+0000ad20: 6275 7474 6f6e 2063 6c61 7373 3d5c 2270  button class=\"p
+0000ad30: 756c 6c2d 7269 6768 7420 6274 6e2d 6469  ull-right btn-di
+0000ad40: 736d 6973 735c 220a 2020 2020 2020 2020  smiss\".        
+0000ad50: 6172 6961 2d6c 6162 656c 3d5c 2253 756c  aria-label=\"Sul
+0000ad60: 6a65 5c22 2064 6174 612d 6163 7469 6f6e  je\" data-action
+0000ad70: 3d5c 2263 616e 6365 6c2d 616c 6c5c 223e  =\"cancel-all\">
+0000ad80: 3c2f 6275 7474 6f6e 3e5c 725c 6e20 2020  </button>\r\n   
+0000ad90: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000ada0: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
+0000adb0: 5c22 666f 726d 5c22 3e3c 2f64 6976 3e5c  \"form\"></div>\
+0000adc0: 725c 6e5c 745c 745c 745c 743c 6469 7620  r\n\t\t\t\t<div 
+0000add0: 636c 6173 733d 5c22 676c 6f62 616c 2d76  class=\"global-v
+0000ade0: 616c 6964 6174 696f 6e2d 6572 726f 7220  alidation-error 
+0000adf0: 616c 6572 740a 2020 2020 2020 2020 616c  alert.        al
+0000ae00: 6572 742d 6461 6e67 6572 5c22 2073 7479  ert-danger\" sty
+0000ae10: 6c65 3d5c 2264 6973 706c 6179 3a6e 6f6e  le=\"display:non
+0000ae20: 655c 223e 5c72 5c6e 5c74 5c74 2020 2020  e\">\r\n\t\t    
+0000ae30: 5c74 5c74 545c 7845 3479 745c 7845 3420  \t\tT\xE4yt\xE4 
+0000ae40: 7075 7574 7475 7661 740a 2020 2020 2020  puuttuvat.      
+0000ae50: 2020 6b65 6e74 5c78 4534 745c 725c 6e5c    kent\xE4t\r\n\
+0000ae60: 745c 7420 2020 205c 743c 2f64 6976 3e5c  t\t    \t</div>\
+0000ae70: 725c 6e5c 745c 745c 743c 2f64 6976 3e5c  r\n\t\t\t</div>\
+0000ae80: 725c 6e5c 745c 743c 2f64 6976 3e5c 725c  r\n\t\t</div>\r\
+0000ae90: 6e5c 743c 2f64 6976 3e5c 725c 6e3c 2f64  n\t</div>\r\n</d
+0000aea0: 6976 3e5c 725c 6e5c 725c 6e5c 725c 6e5c  iv>\r\n\r\n\r\n\
+0000aeb0: 725c 6e3c 6469 760a 2020 2020 2020 2020  r\n<div.        
+0000aec0: 6964 3d5c 2263 6861 6e67 652d 6a6f 696e  id=\"change-join
+0000aed0: 2d74 7970 652d 6d6f 6461 6c5c 2220 636c  -type-modal\" cl
+0000aee0: 6173 733d 5c22 6d6f 6461 6c5c 2220 7374  ass=\"modal\" st
+0000aef0: 796c 653d 5c22 6469 7370 6c61 793a 6e6f  yle=\"display:no
+0000af00: 6e65 5c22 3e5c 725c 6e5c 743c 6469 760a  ne\">\r\n\t<div.
+0000af10: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+0000af20: 6d6f 6461 6c2d 6469 616c 6f67 206d 6f64  modal-dialog mod
+0000af30: 616c 2d6c 675c 223e 5c72 5c6e 5c74 5c74  al-lg\">\r\n\t\t
+0000af40: 3c64 6976 2063 6c61 7373 3d5c 226d 6f64  <div class=\"mod
+0000af50: 616c 2d63 6f6e 7465 6e74 5c22 3e5c 725c  al-content\">\r\
+0000af60: 6e5c 745c 745c 743c 6469 760a 2020 2020  n\t\t\t<div.    
+0000af70: 2020 2020 636c 6173 733d 5c22 6d6f 6461      class=\"moda
+0000af80: 6c2d 626f 6479 5c22 3e5c 725c 6e5c 745c  l-body\">\r\n\t\
+0000af90: 745c 745c 743c 6469 7620 636c 6173 733d  t\t\t<div class=
+0000afa0: 5c22 7061 6765 2d68 6561 6465 725c 223e  \"page-header\">
+0000afb0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c72  \r\n\t\t\t\t\t\r
+0000afc0: 5c6e 5c74 5c74 5c74 5c74 5c74 3c62 7574  \n\t\t\t\t\t<but
+0000afd0: 746f 6e0a 2020 2020 2020 2020 636c 6173  ton.        clas
+0000afe0: 733d 5c22 7075 6c6c 2d72 6967 6874 2062  s=\"pull-right b
+0000aff0: 746e 2d64 6973 6d69 7373 5c22 2061 7269  tn-dismiss\" ari
+0000b000: 612d 6c61 6265 6c3d 5c22 5375 6c6a 655c  a-label=\"Sulje\
+0000b010: 2220 6461 7461 2d61 6374 696f 6e3d 5c22  " data-action=\"
+0000b020: 6361 6e63 656c 2d61 6c6c 5c22 3e3c 2f62  cancel-all\"></b
+0000b030: 7574 746f 6e3e 5c72 5c6e 0a20 2020 2020  utton>\r\n.     
+0000b040: 2020 205c 2020 2020 2020 2020 2020 2020     \            
+0000b050: 2020 2020 2020 203c 6832 3e56 6169 6864         <h2>Vaihd
+0000b060: 6120 6a5c 7845 3474 6568 756f 6c6c 6f6e  a j\xE4tehuollon
+0000b070: 206c 6969 7474 796d 6973 7461 7061 613c   liittymistapaa<
+0000b080: 2f68 323e 5c72 5c6e 5c74 5c74 5c74 5c74  /h2>\r\n\t\t\t\t
+0000b090: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 0a20  </div>\r\n\r\n. 
+0000b0a0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+0000b0b0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000b0c0: 733d 5c22 666f 726d 2d67 656e 6572 616c  s=\"form-general
+0000b0d0: 2d69 6e66 6f5c 223e 3c2f 6469 763e 5c72  -info\"></div>\r
+0000b0e0: 5c6e 5c74 5c74 5c74 5c74 3c64 6976 2063  \n\t\t\t\t<div c
+0000b0f0: 6c61 7373 3d5c 2266 6f72 6d5c 223e 3c2f  lass=\"form\"></
+0000b100: 6469 763e 5c72 5c6e 0a20 2020 2020 2020  div>\r\n.       
+0000b110: 205c 2020 2020 2020 2020 2020 2020 2020   \              
+0000b120: 203c 6469 7620 636c 6173 733d 5c22 666f   <div class=\"fo
+0000b130: 726d 2d69 6e66 6f72 6d61 6e74 5c22 3e3c  rm-informant\"><
+0000b140: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
+0000b150: 743c 6469 7620 636c 6173 733d 5c22 616b  t<div class=\"ak
+0000b160: 702d 726f 6f74 5c22 3e5c 725c 6e5c 745c  p-root\">\r\n\t\
+0000b170: 745c 745c 745c 743c 6469 760a 2020 2020  t\t\t\t<div.    
+0000b180: 2020 2020 636c 6173 733d 5c22 616b 705c      class=\"akp\
+0000b190: 223e 3c2f 6469 763e 5c72 5c6e 5c74 5c74  "></div>\r\n\t\t
+0000b1a0: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
+0000b1b0: 3d5c 2261 6b70 2d69 6e66 6f5c 223e 3c2f  =\"akp-info\"></
+0000b1c0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
+0000b1d0: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
+0000b1e0: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 3c2f  </div>\r\n\t\t</
+0000b1f0: 6469 763e 5c72 5c6e 5c74 3c2f 6469 763e  div>\r\n\t</div>
+0000b200: 5c72 5c6e 3c2f 6469 763e 5c72 5c6e 5c72  \r\n</div>\r\n\r
+0000b210: 5c6e 5c72 5c6e 5c72 5c6e 3c64 6976 0a20  \n\r\n\r\n<div. 
+0000b220: 2020 2020 2020 2069 643d 5c22 6f72 6465         id=\"orde
+0000b230: 722d 6d6f 6461 6c5c 2220 636c 6173 733d  r-modal\" class=
+0000b240: 5c22 6d6f 6461 6c5c 2220 7374 796c 653d  \"modal\" style=
+0000b250: 5c22 6469 7370 6c61 793a 6e6f 6e65 5c22  \"display:none\"
+0000b260: 3e5c 725c 6e20 2020 203c 6469 7620 636c  >\r\n    <div cl
+0000b270: 6173 733d 5c22 6d6f 6461 6c2d 6469 616c  ass=\"modal-dial
+0000b280: 6f67 0a20 2020 2020 2020 206d 6f64 616c  og.        modal
+0000b290: 2d6c 675c 223e 5c72 5c6e 2020 2020 2020  -lg\">\r\n      
+0000b2a0: 2020 3c64 6976 2063 6c61 7373 3d5c 226d    <div class=\"m
+0000b2b0: 6f64 616c 2d63 6f6e 7465 6e74 5c22 3e5c  odal-content\">\
+0000b2c0: 725c 6e20 2020 2020 2020 2020 2020 203c  r\n            <
+0000b2d0: 6469 7620 636c 6173 733d 5c22 6d6f 6461  div class=\"moda
+0000b2e0: 6c2d 626f 6479 5c22 3e5c 725c 6e5c 725c  l-body\">\r\n\r\
+0000b2f0: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+0000b300: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000b310: 6c61 7373 3d5c 2270 6167 652d 6865 6164  lass=\"page-head
+0000b320: 6572 5c22 3e5c 725c 6e20 2020 2020 2020  er\">\r\n       
+0000b330: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
+0000b340: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0000b350: 2020 2020 203c 6275 7474 6f6e 0a20 2020       <button.   
+0000b360: 2020 2020 2063 6c61 7373 3d5c 2270 756c       class=\"pul
+0000b370: 6c2d 7269 6768 7420 6274 6e2d 6469 736d  l-right btn-dism
+0000b380: 6973 735c 2220 6172 6961 2d6c 6162 656c  iss\" aria-label
+0000b390: 3d5c 2253 756c 6a65 5c22 2064 6174 612d  =\"Sulje\" data-
+0000b3a0: 6163 7469 6f6e 3d5c 2263 616e 6365 6c2d  action=\"cancel-
+0000b3b0: 616c 6c5c 223e 3c2f 6275 7474 6f6e 3e5c  all\"></button>\
+0000b3c0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3e0: 3c68 313e 4a5c 7845 3474 6568 756f 6c74  <h1>J\xE4tehuolt
+0000b3f0: 6f6f 6e20 6c69 6974 7479 6d69 6e65 6e3c  oon liittyminen<
+0000b400: 2f68 313e 5c72 5c6e 2020 2020 2020 2020  /h1>\r\n        
+0000b410: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
+0000b420: 5c6e 5c72 5c6e 0a20 2020 2020 2020 205c  \n\r\n.        \
+0000b430: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000b440: 6469 7620 636c 6173 733d 5c22 6c6f 6164  div class=\"load
+0000b450: 696e 672d 6963 6f6e 5c22 3e3c 2f64 6976  ing-icon\"></div
+0000b460: 3e5c 725c 6e5c 725c 6e20 2020 2020 2020  >\r\n\r\n       
+0000b470: 2020 2020 2020 2020 203c 6469 760a 2020           <div.  
+0000b480: 2020 2020 2020 636c 6173 733d 5c22 7461        class=\"ta
+0000b490: 6262 6172 5c22 3e5c 725c 6e20 2020 2020  bbar\">\r\n     
+0000b4a0: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+0000b4b0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+0000b4c0: 2020 2020 2020 203c 756c 2063 6c61 7373         <ul class
+0000b4d0: 3d5c 2274 6162 2d6c 6973 740a 2020 2020  =\"tab-list.    
+0000b4e0: 2020 2020 6c69 7374 2d69 6e6c 696e 655c      list-inline\
+0000b4f0: 2220 6461 7461 2d72 6f6c 653d 5c22 7461  " data-role=\"ta
+0000b500: 622d 6c69 7374 5c22 3e5c 725c 6e20 2020  b-list\">\r\n   
+0000b510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b520: 2020 2020 203c 6c69 2063 6c61 7373 3d5c       <li class=\
+0000b530: 2261 310a 2020 2020 2020 2020 6e75 6d62  "a1.        numb
+0000b540: 6572 2d62 7265 6164 6372 756d 625c 223e  er-breadcrumb\">
+0000b550: 3c61 2068 7265 663d 5c22 2361 315c 223e  <a href=\"#a1\">
+0000b560: 313c 2f61 3e3c 2f6c 693e 5c72 5c6e 2020  1</a></li>\r\n  
+0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b580: 2020 2020 2020 3c6c 690a 2020 2020 2020        <li.      
+0000b590: 2020 636c 6173 733d 5c22 6131 5f35 206e    class=\"a1_5 n
+0000b5a0: 756d 6265 722d 6272 6561 6463 7275 6d62  umber-breadcrumb
+0000b5b0: 5c22 3e3c 6120 6872 6566 3d5c 2223 6131  \"><a href=\"#a1
+0000b5c0: 2e35 5c22 3e32 3c2f 613e 3c2f 6c69 3e5c  .5\">2</a></li>\
+0000b5d0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+0000b5e0: 2020 2020 2020 2020 2020 205c 725c 6e0a             \r\n.
+0000b5f0: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b610: 3c6c 6920 636c 6173 733d 5c22 616b 7020  <li class=\"akp 
+0000b620: 6e75 6d62 6572 2d62 7265 6164 6372 756d  number-breadcrum
+0000b630: 625c 223e 3c61 2068 7265 663d 5c22 2361  b\"><a href=\"#a
+0000b640: 6b70 5c22 3e33 3c2f 613e 3c2f 6c69 3e5c  kp\">3</a></li>\
+0000b650: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+0000b660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b670: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
+0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b690: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+0000b6a0: 2020 2020 2020 2020 2020 2020 3c6c 690a              <li.
+0000b6b0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+0000b6c0: 7761 7374 652d 7761 7465 7220 6e75 6d62  waste-water numb
+0000b6d0: 6572 2d62 7265 6164 6372 756d 625c 223e  er-breadcrumb\">
+0000b6e0: 3c61 2068 7265 663d 5c22 2377 6173 7465  <a href=\"#waste
+0000b6f0: 2d77 6174 6572 5c22 3e34 3c2f 613e 3c2f  -water\">4</a></
+0000b700: 6c69 3e5c 725c 6e0a 2020 2020 2020 2020  li>\r\n.        
+0000b710: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+0000b720: 2020 2020 2020 2020 5c72 5c6e 2020 2020          \r\n    
+0000b730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b740: 2020 2020 3c6c 6920 636c 6173 733d 5c22      <li class=\"
+0000b750: 6132 206e 756d 6265 722d 6272 6561 6463  a2 number-breadc
+0000b760: 7275 6d62 5c22 3e3c 610a 2020 2020 2020  rumb\"><a.      
+0000b770: 2020 6872 6566 3d5c 2223 6132 5c22 3e35    href=\"#a2\">5
+0000b780: 3c2f 613e 3c2f 6c69 3e5c 725c 6e20 2020  </a></li>\r\n   
+0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7a0: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
+0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7c0: 203c 6c69 0a20 2020 2020 2020 2063 6c61   <li.        cla
+0000b7d0: 7373 3d5c 2261 3320 6e75 6d62 6572 2d62  ss=\"a3 number-b
+0000b7e0: 7265 6164 6372 756d 625c 223e 3c61 2068  readcrumb\"><a h
+0000b7f0: 7265 663d 5c22 2361 335c 223e 363c 2f61  ref=\"#a3\">6</a
+0000b800: 3e3c 2f6c 693e 5c72 5c6e 2020 2020 2020  ></li>\r\n      
+0000b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b820: 2020 3c6c 690a 2020 2020 2020 2020 636c    <li.        cl
+0000b830: 6173 733d 5c22 6134 206e 756d 6265 722d  ass=\"a4 number-
+0000b840: 6272 6561 6463 7275 6d62 5c22 3e3c 6120  breadcrumb\"><a 
+0000b850: 6872 6566 3d5c 2223 6134 5c22 3e37 3c2f  href=\"#a4\">7</
+0000b860: 613e 3c2f 6c69 3e5c 725c 6e20 2020 2020  a></li>\r\n     
+0000b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b880: 2020 203c 6c69 0a20 2020 2020 2020 2063     <li.        c
+0000b890: 6c61 7373 3d5c 2261 3520 6e75 6d62 6572  lass=\"a5 number
+0000b8a0: 2d62 7265 6164 6372 756d 625c 223e 3c61  -breadcrumb\"><a
+0000b8b0: 2068 7265 663d 5c22 2361 355c 223e 383c   href=\"#a5\">8<
+0000b8c0: 2f61 3e3c 2f6c 693e 5c72 5c6e 2020 2020  /a></li>\r\n    
+0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8e0: 3c2f 756c 3e5c 725c 6e5c 725c 6e0a 2020  </ul>\r\n\r\n.  
+0000b8f0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+0000b900: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000b910: 6c61 7373 3d5c 2261 315c 223e 3c2f 6469  lass=\"a1\"></di
+0000b920: 763e 5c72 5c6e 2020 2020 2020 2020 2020  v>\r\n          
+0000b930: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000b940: 6c61 7373 3d5c 2261 315f 355c 223e 3c2f  lass=\"a1_5\"></
+0000b950: 6469 763e 5c72 5c6e 0a20 2020 2020 2020  div>\r\n.       
+0000b960: 205c 2020 2020 2020 2020 2020 2020 2020   \              
+0000b970: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
+0000b980: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000b990: 7620 636c 6173 733d 5c22 616b 705c 223e  v class=\"akp\">
+0000b9a0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+0000b9b0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000b9c0: 0a20 2020 2020 2020 2064 6174 612d 726f  .        data-ro
+0000b9d0: 6c65 3d5c 2261 6b70 2d70 6167 655c 223e  le=\"akp-page\">
+0000b9e0: 3c2f 6469 763e 5c72 5c6e 2020 2020 2020  </div>\r\n      
+0000b9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba00: 2020 3c64 6976 2064 6174 612d 726f 6c65    <div data-role
+0000ba10: 3d5c 2262 7574 746f 6e73 5c22 3e3c 2f64  =\"buttons\"></d
+0000ba20: 6976 3e5c 725c 6e0a 2020 2020 2020 2020  iv>\r\n.        
+0000ba30: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+0000ba40: 2020 2020 3c2f 6469 763e 5c72 5c6e 2020      </div>\r\n  
+0000ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba60: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
+0000ba70: 2020 2020 2020 2020 2020 5c72 5c6e 0a20            \r\n. 
+0000ba80: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+0000ba90: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000baa0: 6461 7461 2d72 6f6c 653d 5c22 7761 7374  data-role=\"wast
+0000bab0: 652d 7761 7465 725c 2220 636c 6173 733d  e-water\" class=
+0000bac0: 5c22 7761 7374 652d 7761 7465 725c 223e  \"waste-water\">
+0000bad0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+0000bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000baf0: 2020 2020 203c 6469 7620 6461 7461 2d72       <div data-r
+0000bb00: 6f6c 653d 5c22 7461 6262 6172 5c22 3e5c  ole=\"tabbar\">\
+0000bb10: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000bb30: 756c 0a20 2020 2020 2020 2063 6c61 7373  ul.        class
+0000bb40: 3d5c 2274 6162 2d6c 6973 7420 6c69 7374  =\"tab-list list
+0000bb50: 2d69 6e6c 696e 655c 223e 5c72 5c6e 2020  -inline\">\r\n  
+0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb70: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
+0000bb80: 6920 636c 6173 733d 5c22 6163 7469 7665  i class=\"active
+0000bb90: 0a20 2020 2020 2020 2061 315c 223e 3c61  .        a1\"><a
+0000bba0: 2068 7265 663d 5c22 2361 315c 223e 4131   href=\"#a1\">A1
+0000bbb0: 3c2f 613e 3c2f 6c69 3e3c 6c69 2063 6c61  </a></li><li cla
+0000bbc0: 7373 3d5c 2261 3220 6469 7361 626c 6564  ss=\"a2 disabled
+0000bbd0: 5c22 3e3c 6120 6872 6566 3d5c 2223 6132  \"><a href=\"#a2
+0000bbe0: 5c22 3e41 323c 2f61 3e3c 2f6c 693e 3c6c  \">A2</a></li><l
+0000bbf0: 690a 2020 2020 2020 2020 636c 6173 733d  i.        class=
+0000bc00: 5c22 6133 2064 6973 6162 6c65 645c 223e  \"a3 disabled\">
+0000bc10: 3c61 2068 7265 663d 5c22 2361 335c 223e  <a href=\"#a3\">
+0000bc20: 4133 3c2f 613e 3c2f 6c69 3e3c 6c69 2063  A3</a></li><li c
+0000bc30: 6c61 7373 3d5c 2261 3420 6469 7361 626c  lass=\"a4 disabl
+0000bc40: 6564 5c22 3e3c 610a 2020 2020 2020 2020  ed\"><a.        
+0000bc50: 6872 6566 3d5c 2223 6134 5c22 3e41 343c  href=\"#a4\">A4<
+0000bc60: 2f61 3e3c 2f6c 693e 3c6c 6920 636c 6173  /a></li><li clas
+0000bc70: 733d 5c22 6135 2064 6973 6162 6c65 645c  s=\"a5 disabled\
+0000bc80: 223e 3c61 2068 7265 663d 5c22 2361 355c  "><a href=\"#a5\
+0000bc90: 223e 4135 3c2f 613e 3c2f 6c69 3e3c 6c69  ">A5</a></li><li
+0000bca0: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+0000bcb0: 2261 3620 6469 7361 626c 6564 5c22 3e3c  "a6 disabled\"><
+0000bcc0: 6120 6872 6566 3d5c 2223 6136 5c22 3e41  a href=\"#a6\">A
+0000bcd0: 363c 2f61 3e3c 2f6c 693e 5c72 5c6e 2020  6</a></li>\r\n  
+0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcf0: 2020 2020 2020 2020 2020 3c2f 756c 3e5c            </ul>\
+0000bd00: 725c 6e5c 725c 6e0a 2020 2020 2020 2020  r\n\r\n.        
+0000bd10: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+0000bd20: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000bd30: 2063 6c61 7373 3d5c 2261 315c 223e 3c2f   class=\"a1\"></
+0000bd40: 6469 763e 5c72 5c6e 2020 2020 2020 2020  div>\r\n        
+0000bd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd60: 2020 2020 3c64 6976 0a20 2020 2020 2020      <div.       
+0000bd70: 2063 6c61 7373 3d5c 2261 325c 223e 3c2f   class=\"a2\"></
+0000bd80: 6469 763e 5c72 5c6e 2020 2020 2020 2020  div>\r\n        
+0000bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bda0: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
+0000bdb0: 2261 335c 223e 3c2f 6469 763e 5c72 5c6e  "a3\"></div>\r\n
+0000bdc0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bde0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000bdf0: 5c22 6134 5c22 3e3c 2f64 6976 3e5c 725c  \"a4\"></div>\r\
+0000be00: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0000be10: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000be20: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
+0000be30: 5c22 6135 5c22 3e3c 2f64 6976 3e5c 725c  \"a5\"></div>\r\
+0000be40: 6e5c 725c 6e20 2020 2020 2020 2020 2020  n\r\n           
+0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be60: 203c 6469 7620 636c 6173 733d 5c22 6136   <div class=\"a6
+0000be70: 5c22 3e5c 725c 6e0a 2020 2020 2020 2020  \">\r\n.        
+0000be80: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bea0: 3c64 6976 2063 6c61 7373 3d5c 226d 6170  <div class=\"map
+0000beb0: 2d69 6e66 6f5c 223e 5c72 5c6e 2020 2020  -info\">\r\n    
+0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bee0: 3c64 6976 3e4b 6172 7474 6161 0a20 2020  <div>Karttaa.   
+0000bef0: 2020 2020 2076 6f69 2073 6969 7274 5c78       voi siirt\x
+0000bf00: 4534 5c78 4534 2068 6969 7265 6c6c 5c78  E4\xE4 hiirell\x
+0000bf10: 4534 2072 6161 6861 616d 616c 6c61 2e20  E4 raahaamalla. 
+0000bf20: 4b6c 696b 6b61 6120 5061 696b 6b61 202d  Klikkaa Paikka -
+0000bf30: 7061 696e 696b 6574 7461 206a 6120 7669  painiketta ja vi
+0000bf40: 650a 2020 2020 2020 2020 6869 6972 6920  e.        hiiri 
+0000bf50: 6b61 7274 616c 6c61 206b 6f68 7461 616e  kartalla kohtaan
+0000bf60: 2c20 6a6f 7373 6120 6b61 6976 6f20 6f6e  , jossa kaivo on
+0000bf70: 2e20 4f68 6a65 6c6d 6120 7661 726d 6973  . Ohjelma varmis
+0000bf80: 7461 6120 7669 656c 5c78 4534 2076 616c  taa viel\xE4 val
+0000bf90: 696e 6e61 6e0a 2020 2020 2020 2020 6f69  innan.        oi
+0000bfa0: 6b65 616b 7369 203c 2f64 6976 3e5c 725c  keaksi </div>\r\
+0000bfb0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfd0: 2020 2020 203c 6275 7474 6f6e 2064 6174       <button dat
+0000bfe0: 612d 6163 7469 6f6e 3d5c 226d 6172 6b2d  a-action=\"mark-
+0000bff0: 7765 6c6c 5c22 3e50 6169 6b6b 613c 2f62  well\">Paikka</b
+0000c000: 7574 746f 6e3e 5c72 5c6e 0a20 2020 2020  utton>\r\n.     
+0000c010: 2020 205c 2020 2020 2020 2020 2020 2020     \            
+0000c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c030: 2020 203c 2f64 6976 3e5c 725c 6e20 2020     </div>\r\n   
+0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c050: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000c060: 760a 2020 2020 2020 2020 6461 7461 2d72  v.        data-r
+0000c070: 6f6c 653d 5c22 6b61 7274 7461 5c22 2063  ole=\"kartta\" c
+0000c080: 6c61 7373 3d5c 226d 6170 5c22 3e3c 2f64  lass=\"map\"></d
+0000c090: 6976 3e5c 725c 6e20 2020 2020 2020 2020  iv>\r\n         
+0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0b0: 2020 203c 2f64 6976 3e5c 725c 6e0a 2020     </div>\r\n.  
+0000c0c0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+0000c0d0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+0000c0e0: 6469 763e 5c72 5c6e 5c72 5c6e 2020 2020  div>\r\n\r\n    
+0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c100: 2020 2020 3c64 6976 2064 6174 612d 726f      <div data-ro
+0000c110: 6c65 3d5c 2262 7574 746f 6e73 5c22 3e3c  le=\"buttons\"><
+0000c120: 2f64 6976 3e5c 725c 6e0a 2020 2020 2020  /div>\r\n.      
+0000c130: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+0000c140: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
+0000c150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c160: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
+0000c170: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000c180: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+0000c190: 2261 325c 223e 3c2f 6469 763e 5c72 5c6e  "a2\"></div>\r\n
+0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1b0: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
+0000c1c0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000c1d0: 2063 6c61 7373 3d5c 2261 335c 223e 3c2f   class=\"a3\"></
+0000c1e0: 6469 763e 5c72 5c6e 0a20 2020 2020 2020  div>\r\n.       
+0000c1f0: 205c 2020 2020 2020 2020 2020 2020 2020   \              
+0000c200: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000c210: 5c22 6134 5c22 3e3c 2f64 6976 3e5c 725c  \"a4\"></div>\r\
+0000c220: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0000c230: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000c240: 5c22 6135 5c22 3e3c 2f64 6976 3e5c 725c  \"a5\"></div>\r\
+0000c250: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+0000c260: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+0000c270: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
+0000c280: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000c290: 7373 3d5c 2267 6c6f 6261 6c2d 7661 6c69  ss=\"global-vali
+0000c2a0: 6461 7469 6f6e 2d65 7272 6f72 0a20 2020  dation-error.   
+0000c2b0: 2020 2020 2061 6c65 7274 2061 6c65 7274       alert alert
+0000c2c0: 2d64 616e 6765 725c 2220 7374 796c 653d  -danger\" style=
+0000c2d0: 5c22 6469 7370 6c61 793a 6e6f 6e65 5c22  \"display:none\"
+0000c2e0: 3e54 5c78 4534 7974 5c78 4534 2070 7575  >T\xE4yt\xE4 puu
+0000c2f0: 7474 7576 6174 206b 656e 745c 7845 3474  ttuvat kent\xE4t
+0000c300: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 0a20  </div>\r\n\r\n. 
+0000c310: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+0000c320: 2020 203c 2f64 6976 3e5c 725c 6e20 2020     </div>\r\n   
+0000c330: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
+0000c340: 2020 203c 2f64 6976 3e5c 725c 6e3c 2f64     </div>\r\n</d
+0000c350: 6976 3e5c 725c 6e5c 725c 6e5c 725c 6e5c  iv>\r\n\r\n\r\n\
+0000c360: 725c 6e5c 725c 6e3c 6469 760a 2020 2020  r\n\r\n<div.    
+0000c370: 2020 2020 6964 3d5c 2263 6f6d 706f 7374      id=\"compost
+0000c380: 2d6d 6f64 616c 5c22 2063 6c61 7373 3d5c  -modal\" class=\
+0000c390: 226d 6f64 616c 5c22 2073 7479 6c65 3d5c  "modal\" style=\
+0000c3a0: 2264 6973 706c 6179 3a6e 6f6e 655c 223e  "display:none\">
+0000c3b0: 5c72 5c6e 5c74 3c64 6976 2063 6c61 7373  \r\n\t<div class
+0000c3c0: 3d5c 226d 6f64 616c 2d64 6961 6c6f 670a  =\"modal-dialog.
+0000c3d0: 2020 2020 2020 2020 6d6f 6461 6c2d 6c67          modal-lg
+0000c3e0: 5c22 3e5c 725c 6e5c 745c 743c 6469 7620  \">\r\n\t\t<div 
+0000c3f0: 636c 6173 733d 5c22 6d6f 6461 6c2d 636f  class=\"modal-co
+0000c400: 6e74 656e 745c 223e 5c72 5c6e 5c74 5c74  ntent\">\r\n\t\t
+0000c410: 5c74 3c64 6976 2063 6c61 7373 3d5c 226d  \t<div class=\"m
+0000c420: 6f64 616c 2d62 6f64 795c 223e 5c72 5c6e  odal-body\">\r\n
+0000c430: 5c72 5c6e 5c74 5c74 5c74 5c74 3c64 6976  \r\n\t\t\t\t<div
+0000c440: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+0000c450: 2270 6167 652d 6865 6164 6572 5c22 3e5c  "page-header\">\
+0000c460: 725c 6e5c 745c 745c 745c 745c 745c 725c  r\n\t\t\t\t\t\r\
+0000c470: 6e5c 745c 745c 745c 745c 743c 6275 7474  n\t\t\t\t\t<butt
+0000c480: 6f6e 2063 6c61 7373 3d5c 2270 756c 6c2d  on class=\"pull-
+0000c490: 7269 6768 740a 2020 2020 2020 2020 6274  right.        bt
+0000c4a0: 6e2d 6469 736d 6973 735c 2220 6172 6961  n-dismiss\" aria
+0000c4b0: 2d6c 6162 656c 3d5c 2253 756c 6a65 5c22  -label=\"Sulje\"
+0000c4c0: 2064 6174 612d 6163 7469 6f6e 3d5c 2263   data-action=\"c
+0000c4d0: 616e 6365 6c2d 616c 6c5c 223e 3c2f 6275  ancel-all\"></bu
+0000c4e0: 7474 6f6e 3e5c 725c 6e0a 2020 2020 2020  tton>\r\n.      
+0000c4f0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+0000c500: 2020 2020 2020 3c68 313e 4b6f 6d70 6f73        <h1>Kompos
+0000c510: 746f 696e 7469 2d69 6c6d 6f69 7475 733c  tointi-ilmoitus<
+0000c520: 2f68 313e 5c72 5c6e 5c74 5c74 5c74 5c74  /h1>\r\n\t\t\t\t
+0000c530: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 0a20  </div>\r\n\t\t. 
+0000c540: 2020 2020 2020 205c 2020 205c 745c 725c         \   \t\r\
+0000c550: 6e5c 745c 7420 2020 205c 743c 6469 7620  n\t\t    \t<div 
+0000c560: 636c 6173 733d 5c22 666f 726d 5c22 3e3c  class=\"form\"><
+0000c570: 2f64 6976 3e5c 725c 6e5c 725c 6e5c 745c  /div>\r\n\r\n\t\
+0000c580: 7420 2020 205c 743c 6469 7620 636c 6173  t    \t<div clas
+0000c590: 733d 5c22 676c 6f62 616c 2d76 616c 6964  s=\"global-valid
+0000c5a0: 6174 696f 6e2d 6572 726f 720a 2020 2020  ation-error.    
+0000c5b0: 2020 2020 616c 6572 7420 616c 6572 742d      alert alert-
+0000c5c0: 6461 6e67 6572 5c22 2073 7479 6c65 3d5c  danger\" style=\
+0000c5d0: 2264 6973 706c 6179 3a6e 6f6e 655c 223e  "display:none\">
+0000c5e0: 5c72 5c6e 5c74 5c74 2020 2020 5c74 5c74  \r\n\t\t    \t\t
+0000c5f0: 545c 7845 3479 745c 7845 3420 7075 7574  T\xE4yt\xE4 puut
+0000c600: 7475 7661 740a 2020 2020 2020 2020 6b65  tuvat.        ke
+0000c610: 6e74 5c78 4534 745c 725c 6e5c 745c 7420  nt\xE4t\r\n\t\t 
+0000c620: 2020 205c 743c 2f64 6976 3e5c 725c 6e5c     \t</div>\r\n\
+0000c630: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
+0000c640: 745c 743c 2f64 6976 3e5c 725c 6e5c 743c  t\t</div>\r\n\t<
+0000c650: 2f64 6976 3e5c 725c 6e3c 2f64 6976 3e5c  /div>\r\n</div>\
+0000c660: 725c 6e5c 725c 6e5c 725c 6e5c 725c 6e3c  r\n\r\n\r\n\r\n<
+0000c670: 6469 760a 2020 2020 2020 2020 6964 3d5c  div.        id=\
+0000c680: 2272 6567 6973 7465 722d 6d6f 6461 6c5c  "register-modal\
+0000c690: 2220 636c 6173 733d 5c22 6d6f 6461 6c5c  " class=\"modal\
+0000c6a0: 2220 7374 796c 653d 5c22 6469 7370 6c61  " style=\"displa
+0000c6b0: 793a 6e6f 6e65 5c22 3e5c 725c 6e5c 743c  y:none\">\r\n\t<
+0000c6c0: 6469 7620 636c 6173 733d 5c22 6d6f 6461  div class=\"moda
+0000c6d0: 6c2d 6469 616c 6f67 0a20 2020 2020 2020  l-dialog.       
+0000c6e0: 206d 6f64 616c 2d6c 675c 223e 5c72 5c6e   modal-lg\">\r\n
+0000c6f0: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
+0000c700: 226d 6f64 616c 2d63 6f6e 7465 6e74 5c22  "modal-content\"
+0000c710: 3e5c 725c 6e5c 745c 745c 743c 6469 7620  >\r\n\t\t\t<div 
+0000c720: 636c 6173 733d 5c22 6d6f 6461 6c2d 626f  class=\"modal-bo
+0000c730: 6479 5c22 3e5c 725c 6e5c 745c 745c 745c  dy\">\r\n\t\t\t\
+0000c740: 725c 6e5c 745c 745c 745c 743c 6469 760a  r\n\t\t\t\t<div.
+0000c750: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+0000c760: 7061 6765 2d68 6561 6465 725c 223e 5c72  page-header\">\r
+0000c770: 5c6e 5c74 5c74 5c74 5c74 5c74 3c68 313e  \n\t\t\t\t\t<h1>
+0000c780: 5469 6c61 6120 6b5c 7845 3479 7474 5c78  Tilaa k\xE4ytt\x
+0000c790: 4534 6a5c 7845 3474 756e 6e75 733c 2f68  E4j\xE4tunnus</h
+0000c7a0: 313e 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f  1>\r\n\t\t\t\t</
+0000c7b0: 6469 763e 5c72 5c6e 5c72 5c6e 5c74 5c74  div>\r\n\r\n\t\t
+0000c7c0: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
+0000c7d0: 2063 6c61 7373 3d5c 2266 6f72 6d5c 223e   class=\"form\">
+0000c7e0: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 5c74  </div>\r\n\r\n\t
+0000c7f0: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
+0000c800: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 3c2f  \t</div>\r\n\t</
+0000c810: 6469 763e 5c72 5c6e 3c2f 6469 763e 5c72  div>\r\n</div>\r
+0000c820: 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e 3c64  \n\r\n\r\n\r\n<d
+0000c830: 6976 0a20 2020 2020 2020 2069 643d 5c22  iv.        id=\"
+0000c840: 626f 6f6b 7570 2d6d 6f64 616c 5c22 2063  bookup-modal\" c
+0000c850: 6c61 7373 3d5c 226d 6f64 616c 5c22 2073  lass=\"modal\" s
+0000c860: 7479 6c65 3d5c 2264 6973 706c 6179 3a6e  tyle=\"display:n
+0000c870: 6f6e 655c 223e 5c72 5c6e 2020 2020 3c64  one\">\r\n    <d
+0000c880: 6976 2063 6c61 7373 3d5c 226d 6f64 616c  iv class=\"modal
+0000c890: 2d64 6961 6c6f 670a 2020 2020 2020 2020  -dialog.        
+0000c8a0: 6d6f 6461 6c2d 6c67 5c22 3e5c 725c 6e20  modal-lg\">\r\n 
+0000c8b0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000c8c0: 733d 5c22 6d6f 6461 6c2d 636f 6e74 656e  s=\"modal-conten
+0000c8d0: 745c 223e 5c72 5c6e 2020 2020 2020 2020  t\">\r\n        
+0000c8e0: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
+0000c8f0: 226d 6f64 616c 2d62 6f64 795c 223e 5c72  "modal-body\">\r
+0000c900: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+0000c910: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000c920: 636c 6173 733d 5c22 7061 6765 2d68 6561  class=\"page-hea
+0000c930: 6465 725c 223e 5c72 5c6e 2020 2020 2020  der\">\r\n      
+0000c940: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
+0000c950: 7574 746f 6e0a 2020 2020 2020 2020 636c  utton.        cl
+0000c960: 6173 733d 5c22 7075 6c6c 2d72 6967 6874  ass=\"pull-right
+0000c970: 2062 746e 2d64 6973 6d69 7373 2063 616e   btn-dismiss can
+0000c980: 6365 6c5c 223e 3c2f 6275 7474 6f6e 3e5c  cel\"></button>\
+0000c990: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+0000c9a0: 2020 2020 2020 203c 6831 3e54 696c 6161         <h1>Tilaa
+0000c9b0: 0a20 2020 2020 2020 2070 616c 7665 6c75  .        palvelu
+0000c9c0: 6974 613c 2f68 313e 5c72 5c6e 2020 2020  ita</h1>\r\n    
+0000c9d0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+0000c9e0: 763e 5c72 5c6e 5c72 5c6e 2020 2020 2020  v>\r\n\r\n      
+0000c9f0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0000ca00: 6c61 7373 3d5c 2263 6f6d 6d75 6e69 7479  lass=\"community
+0000ca10: 2d66 6f72 6d5c 223e 5c72 5c6e 0a20 2020  -form\">\r\n.   
+0000ca20: 2020 2020 205c 2020 2020 2020 2020 2020       \          
+0000ca30: 2020 2020 2020 2020 203c 666f 726d 3e5c           <form>\
+0000ca40: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+0000ca50: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000ca60: 636c 6173 733d 5c22 666f 726d 2d67 726f  class=\"form-gro
+0000ca70: 7570 5c22 3e5c 725c 6e0a 2020 2020 2020  up\">\r\n.      
+0000ca80: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+0000ca90: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
+0000caa0: 6162 656c 2066 6f72 3d5c 2263 6f6d 6d75  abel for=\"commu
+0000cab0: 6e69 7479 2d73 656c 6563 745c 2220 636c  nity-select\" cl
+0000cac0: 6173 733d 5c22 636f 6e74 726f 6c2d 6c61  ass=\"control-la
+0000cad0: 6265 6c5c 223e 5661 6c69 7473 650a 2020  bel\">Valitse.  
+0000cae0: 2020 2020 2020 6b75 6e74 612c 206a 6f73        kunta, jos
+0000caf0: 7361 2061 7375 743c 2f6c 6162 656c 3e5c  sa asut</label>\
+0000cb00: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+0000cb10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000cb20: 7365 6c65 6374 2069 643d 5c22 636f 6d6d  select id=\"comm
+0000cb30: 756e 6974 792d 7365 6c65 6374 5c22 0a20  unity-select\". 
+0000cb40: 2020 2020 2020 206e 616d 653d 5c22 636f         name=\"co
+0000cb50: 6d6d 756e 6974 792d 7365 6c65 6374 5c22  mmunity-select\"
+0000cb60: 2064 6174 612d 726f 6c65 3d5c 2263 6f6d   data-role=\"com
+0000cb70: 6d75 6e69 7479 2d73 656c 6563 745c 2220  munity-select\" 
+0000cb80: 636c 6173 733d 5c22 666f 726d 2d63 6f6e  class=\"form-con
+0000cb90: 7472 6f6c 5c22 3e3c 2f73 656c 6563 743e  trol\"></select>
+0000cba0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbc0: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
 0000cbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbe0: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
-0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc00: 2020 3c6c 6920 636c 6173 733d 5c22 6132    <li class=\"a2
-0000cc10: 206e 756d 6265 722d 6272 6561 6463 7275   number-breadcru
-0000cc20: 6d62 5c22 3e3c 610a 2020 2020 2020 2020  mb\"><a.        
-0000cc30: 6872 6566 3d5c 2223 6132 5c22 3e35 3c2f  href=\"#a2\">5</
-0000cc40: 613e 3c2f 6c69 3e5c 725c 6e20 2020 2020  a></li>\r\n     
-0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc60: 2020 205c 725c 6e20 2020 2020 2020 2020     \r\n         
-0000cc70: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000cc80: 6c69 0a20 2020 2020 2020 2063 6c61 7373  li.        class
-0000cc90: 3d5c 2261 3320 6e75 6d62 6572 2d62 7265  =\"a3 number-bre
-0000cca0: 6164 6372 756d 625c 223e 3c61 2068 7265  adcrumb\"><a hre
-0000ccb0: 663d 5c22 2361 335c 223e 363c 2f61 3e3c  f=\"#a3\">6</a><
-0000ccc0: 2f6c 693e 5c72 5c6e 2020 2020 2020 2020  /li>\r\n        
-0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cce0: 3c6c 690a 2020 2020 2020 2020 636c 6173  <li.        clas
-0000ccf0: 733d 5c22 6134 206e 756d 6265 722d 6272  s=\"a4 number-br
-0000cd00: 6561 6463 7275 6d62 5c22 3e3c 6120 6872  eadcrumb\"><a hr
-0000cd10: 6566 3d5c 2223 6134 5c22 3e37 3c2f 613e  ef=\"#a4\">7</a>
-0000cd20: 3c2f 6c69 3e5c 725c 6e20 2020 2020 2020  </li>\r\n       
-0000cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd40: 203c 6c69 0a20 2020 2020 2020 2063 6c61   <li.        cla
-0000cd50: 7373 3d5c 2261 3520 6e75 6d62 6572 2d62  ss=\"a5 number-b
-0000cd60: 7265 6164 6372 756d 625c 223e 3c61 2068  readcrumb\"><a h
-0000cd70: 7265 663d 5c22 2361 355c 223e 383c 2f61  ref=\"#a5\">8</a
-0000cd80: 3e3c 2f6c 693e 5c72 5c6e 2020 2020 2020  ></li>\r\n      
-0000cd90: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0000cda0: 756c 3e5c 725c 6e5c 725c 6e0a 2020 2020  ul>\r\n\r\n.    
-0000cdb0: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-0000cdc0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000cdd0: 7373 3d5c 2261 315c 223e 3c2f 6469 763e  ss=\"a1\"></div>
-0000cde0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-0000cdf0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000ce00: 7373 3d5c 2261 315f 355c 223e 3c2f 6469  ss=\"a1_5\"></di
-0000ce10: 763e 5c72 5c6e 0a20 2020 2020 2020 205c  v>\r\n.        \
-0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce30: 2020 205c 725c 6e20 2020 2020 2020 2020     \r\n         
-0000ce40: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000ce50: 636c 6173 733d 5c22 616b 705c 223e 5c72  class=\"akp\">\r
-0000ce60: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0000ce70: 2020 2020 2020 2020 2020 3c64 6976 0a20            <div. 
-0000ce80: 2020 2020 2020 2064 6174 612d 726f 6c65         data-role
-0000ce90: 3d5c 2261 6b70 2d70 6167 655c 223e 3c2f  =\"akp-page\"></
-0000cea0: 6469 763e 5c72 5c6e 2020 2020 2020 2020  div>\r\n        
-0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cec0: 3c64 6976 2064 6174 612d 726f 6c65 3d5c  <div data-role=\
-0000ced0: 2262 7574 746f 6e73 5c22 3e3c 2f64 6976  "buttons\"></div
-0000cee0: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
-0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf00: 2020 3c2f 6469 763e 5c72 5c6e 2020 2020    </div>\r\n    
-0000cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf20: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-0000cf30: 2020 2020 2020 2020 5c72 5c6e 0a20 2020          \r\n.   
-0000cf40: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-0000cf50: 2020 2020 2020 2020 203c 6469 7620 6461           <div da
-0000cf60: 7461 2d72 6f6c 653d 5c22 7761 7374 652d  ta-role=\"waste-
-0000cf70: 7761 7465 725c 2220 636c 6173 733d 5c22  water\" class=\"
-0000cf80: 7761 7374 652d 7761 7465 725c 223e 5c72  waste-water\">\r
-0000cf90: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfb0: 2020 203c 6469 7620 6461 7461 2d72 6f6c     <div data-rol
-0000cfc0: 653d 5c22 7461 6262 6172 5c22 3e5c 725c  e=\"tabbar\">\r\
-0000cfd0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0000cfe0: 2020 2020 2020 2020 2020 2020 203c 756c               <ul
-0000cff0: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
-0000d000: 2274 6162 2d6c 6973 7420 6c69 7374 2d69  "tab-list list-i
-0000d010: 6e6c 696e 655c 223e 5c72 5c6e 2020 2020  nline\">\r\n    
-0000d020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d030: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
-0000d040: 636c 6173 733d 5c22 6163 7469 7665 0a20  class=\"active. 
-0000d050: 2020 2020 2020 2061 315c 223e 3c61 2068         a1\"><a h
-0000d060: 7265 663d 5c22 2361 315c 223e 4131 3c2f  ref=\"#a1\">A1</
-0000d070: 613e 3c2f 6c69 3e3c 6c69 2063 6c61 7373  a></li><li class
-0000d080: 3d5c 2261 3220 6469 7361 626c 6564 5c22  =\"a2 disabled\"
-0000d090: 3e3c 6120 6872 6566 3d5c 2223 6132 5c22  ><a href=\"#a2\"
-0000d0a0: 3e41 323c 2f61 3e3c 2f6c 693e 3c6c 690a  >A2</a></li><li.
-0000d0b0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-0000d0c0: 6133 2064 6973 6162 6c65 645c 223e 3c61  a3 disabled\"><a
-0000d0d0: 2068 7265 663d 5c22 2361 335c 223e 4133   href=\"#a3\">A3
-0000d0e0: 3c2f 613e 3c2f 6c69 3e3c 6c69 2063 6c61  </a></li><li cla
-0000d0f0: 7373 3d5c 2261 3420 6469 7361 626c 6564  ss=\"a4 disabled
-0000d100: 5c22 3e3c 610a 2020 2020 2020 2020 6872  \"><a.        hr
-0000d110: 6566 3d5c 2223 6134 5c22 3e41 343c 2f61  ef=\"#a4\">A4</a
-0000d120: 3e3c 2f6c 693e 3c6c 6920 636c 6173 733d  ></li><li class=
-0000d130: 5c22 6135 2064 6973 6162 6c65 645c 223e  \"a5 disabled\">
-0000d140: 3c61 2068 7265 663d 5c22 2361 355c 223e  <a href=\"#a5\">
-0000d150: 4135 3c2f 613e 3c2f 6c69 3e3c 6c69 0a20  A5</a></li><li. 
-0000d160: 2020 2020 2020 2063 6c61 7373 3d5c 2261         class=\"a
-0000d170: 3620 6469 7361 626c 6564 5c22 3e3c 6120  6 disabled\"><a 
-0000d180: 6872 6566 3d5c 2223 6136 5c22 3e41 363c  href=\"#a6\">A6<
-0000d190: 2f61 3e3c 2f6c 693e 5c72 5c6e 2020 2020  /a></li>\r\n    
-0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1b0: 2020 2020 2020 2020 3c2f 756c 3e5c 725c          </ul>\r\
-0000d1c0: 6e5c 725c 6e0a 2020 2020 2020 2020 5c20  n\r\n.        \ 
-0000d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1e0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0000d1f0: 6c61 7373 3d5c 2261 315c 223e 3c2f 6469  lass=\"a1\"></di
-0000d200: 763e 5c72 5c6e 2020 2020 2020 2020 2020  v>\r\n          
+0000cbe0: 2020 2020 2020 203c 6469 7620 6964 3d5c         <div id=\
+0000cbf0: 2265 7874 7261 2d6e 6f74 655c 220a 2020  "extra-note\".  
+0000cc00: 2020 2020 2020 636c 6173 733d 5c22 666f        class=\"fo
+0000cc10: 726d 2d67 726f 7570 5c22 3e5c 725c 6e20  rm-group\">\r\n 
+0000cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc30: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
+0000cc40: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0000cc50: 2020 2020 2020 2020 203c 6469 760a 2020           <div.  
+0000cc60: 2020 2020 2020 636c 6173 733d 5c22 666f        class=\"fo
+0000cc70: 726d 2d67 726f 7570 5c22 3e5c 725c 6e20  rm-group\">\r\n 
+0000cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc90: 2020 2020 2020 2020 2020 203c 6275 7474             <butt
+0000cca0: 6f6e 2074 7970 653d 5c22 6275 7474 6f6e  on type=\"button
+0000ccb0: 5c22 0a20 2020 2020 2020 2063 6c61 7373  \".        class
+0000ccc0: 3d5c 2262 746e 2062 746e 2d70 7269 6d61  =\"btn btn-prima
+0000ccd0: 7279 2064 6973 6162 6c65 645c 2220 6461  ry disabled\" da
+0000cce0: 7461 2d61 6374 696f 6e3d 5c22 7365 6c65  ta-action=\"sele
+0000ccf0: 6374 2d63 6f6d 6d75 6e69 7479 5c22 3e4f  ct-community\">O
+0000cd00: 6b3c 2f62 7574 746f 6e3e 5c72 5c6e 0a20  k</button>\r\n. 
+0000cd10: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+0000cd20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000cd30: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
+0000cd40: 2020 2020 2020 2020 2020 2020 203c 2f66               </f
+0000cd50: 6f72 6d3e 5c72 5c6e 2020 2020 2020 2020  orm>\r\n        
+0000cd60: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
+0000cd70: 5c6e 5c72 5c6e 0a20 2020 2020 2020 205c  \n\r\n.        \
+0000cd80: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000cd90: 6469 7620 636c 6173 733d 5c22 7368 6f70  div class=\"shop
+0000cda0: 7069 6e67 2d70 6167 655c 2220 7374 796c  ping-page\" styl
+0000cdb0: 653d 5c22 6469 7370 6c61 793a 6e6f 6e65  e=\"display:none
+0000cdc0: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
+0000cdd0: 2020 2020 2020 2020 2020 203c 6469 760a             <div.
+0000cde0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+0000cdf0: 7368 6f70 7069 6e67 2d63 6172 742d 636f  shopping-cart-co
+0000ce00: 6e74 656e 745c 2220 7374 796c 653d 5c22  ntent\" style=\"
+0000ce10: 6469 7370 6c61 793a 6e6f 6e65 5c22 3e5c  display:none\">\
+0000ce20: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+0000ce30: 2020 2020 2020 2020 2020 203c 6469 760a             <div.
+0000ce40: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+0000ce50: 666f 726d 5c22 3e3c 2f64 6976 3e5c 725c  form\"></div>\r\
+0000ce60: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0000ce70: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0000ce80: 6173 733d 5c22 676c 6f62 616c 2d76 616c  ass=\"global-val
+0000ce90: 6964 6174 696f 6e2d 6572 726f 720a 2020  idation-error.  
+0000cea0: 2020 2020 2020 616c 6572 7420 616c 6572        alert aler
+0000ceb0: 742d 6461 6e67 6572 5c22 2073 7479 6c65  t-danger\" style
+0000cec0: 3d5c 2264 6973 706c 6179 3a6e 6f6e 655c  =\"display:none\
+0000ced0: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
+0000cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cef0: 2020 545c 7845 3479 745c 7845 340a 2020    T\xE4yt\xE4.  
+0000cf00: 2020 2020 2020 7075 7574 7475 7661 7420        puuttuvat 
+0000cf10: 6b65 6e74 5c78 4534 745c 725c 6e20 2020  kent\xE4t\r\n   
+0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf30: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
+0000cf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf50: 2020 203c 2f64 6976 3e5c 725c 6e5c 725c     </div>\r\n\r\
+0000cf60: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+0000cf70: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+0000cf80: 6976 2063 6c61 7373 3d5c 2272 6f77 5c22  iv class=\"row\"
+0000cf90: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+0000cfa0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000cfb0: 7620 636c 6173 733d 5c22 636f 6c2d 6d64  v class=\"col-md
+0000cfc0: 2d31 320a 2020 2020 2020 2020 7465 7874  -12.        text
+0000cfd0: 2d63 656e 7465 725c 223e 5c72 5c6e 2020  -center\">\r\n  
+0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cff0: 2020 2020 2020 2020 2020 3c64 6976 2064            <div d
+0000d000: 6174 612d 726f 6c65 3d5c 2274 6f6f 6c62  ata-role=\"toolb
+0000d010: 6172 5c22 3e3c 2f64 6976 3e5c 725c 6e0a  ar\"></div>\r\n.
+0000d020: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+0000d030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d040: 3c2f 6469 763e 5c72 5c6e 2020 2020 2020  </div>\r\n      
+0000d050: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+0000d060: 6469 763e 5c72 5c6e 5c72 5c6e 2020 2020  div>\r\n\r\n    
+0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d080: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
+0000d090: 7373 3d5c 2273 686f 7070 696e 672d 7061  ss=\"shopping-pa
+0000d0a0: 6765 2d63 6f6e 7465 6e74 5c22 3e5c 725c  ge-content\">\r\
+0000d0b0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0000d0c0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0000d0d0: 6173 733d 5c22 726f 775c 223e 5c72 5c6e  ass=\"row\">\r\n
+0000d0e0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d100: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000d110: 5c22 636f 6c2d 6d64 2d31 325c 223e 5c72  \"col-md-12\">\r
+0000d120: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d140: 2020 3c6c 6162 656c 0a20 2020 2020 2020    <label.       
+0000d150: 2064 6174 612d 726f 6c65 3d5c 2273 7562   data-role=\"sub
+0000d160: 6361 7465 676f 7279 2d68 6561 6465 725c  category-header\
+0000d170: 223e 416c 696b 6174 6567 6f72 6961 3c2f  ">Alikategoria</
+0000d180: 6c61 6265 6c3e 5c72 5c6e 2020 2020 2020  label>\r\n      
+0000d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1a0: 2020 2020 2020 2020 2020 3c64 6976 0a20            <div. 
+0000d1b0: 2020 2020 2020 2063 6c61 7373 3d5c 2273         class=\"s
+0000d1c0: 7562 6361 7465 676f 7279 2d74 6f6f 6c62  ubcategory-toolb
+0000d1d0: 6172 5c22 2064 6174 612d 726f 6c65 3d5c  ar\" data-role=\
+0000d1e0: 2273 7562 6361 7465 676f 7279 2d74 6f6f  "subcategory-too
+0000d1f0: 6c62 6172 5c22 3e3c 2f64 6976 3e5c 725c  lbar\"></div>\r\
+0000d200: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
 0000d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d220: 2020 3c64 6976 0a20 2020 2020 2020 2063    <div.        c
-0000d230: 6c61 7373 3d5c 2261 325c 223e 3c2f 6469  lass=\"a2\"></di
-0000d240: 763e 5c72 5c6e 2020 2020 2020 2020 2020  v>\r\n          
-0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d260: 2020 3c64 6976 2063 6c61 7373 3d5c 2261    <div class=\"a
-0000d270: 335c 223e 3c2f 6469 763e 5c72 5c6e 0a20  3\"></div>\r\n. 
-0000d280: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+0000d220: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
+0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d240: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
+0000d250: 5c6e 5c72 5c6e 0a20 2020 2020 2020 205c  \n\r\n.        \
+0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d270: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000d280: 733d 5c22 726f 775c 223e 5c72 5c6e 2020  s=\"row\">\r\n  
 0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2a0: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
-0000d2b0: 6134 5c22 3e3c 2f64 6976 3e5c 725c 6e20  a4\"></div>\r\n 
-0000d2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2d0: 2020 2020 2020 2020 2020 203c 6469 760a             <div.
-0000d2e0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-0000d2f0: 6135 5c22 3e3c 2f64 6976 3e5c 725c 6e5c  a5\"></div>\r\n\
-0000d300: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-0000d310: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000d320: 6469 7620 636c 6173 733d 5c22 6136 5c22  div class=\"a6\"
-0000d330: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
-0000d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d350: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0000d360: 6976 2063 6c61 7373 3d5c 226d 6170 2d69  iv class=\"map-i
-0000d370: 6e66 6f5c 223e 5c72 5c6e 2020 2020 2020  nfo\">\r\n      
-0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d390: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0000d3a0: 6976 3e4b 6172 7474 6161 0a20 2020 2020  iv>Karttaa.     
-0000d3b0: 2020 2076 6f69 2073 6969 7274 5c78 4534     voi siirt\xE4
-0000d3c0: 5c78 4534 2068 6969 7265 6c6c 5c78 4534  \xE4 hiirell\xE4
-0000d3d0: 2072 6161 6861 616d 616c 6c61 2e20 4b6c   raahaamalla. Kl
-0000d3e0: 696b 6b61 6120 5061 696b 6b61 202d 7061  ikkaa Paikka -pa
-0000d3f0: 696e 696b 6574 7461 206a 6120 7669 650a  iniketta ja vie.
-0000d400: 2020 2020 2020 2020 6869 6972 6920 6b61          hiiri ka
-0000d410: 7274 616c 6c61 206b 6f68 7461 616e 2c20  rtalla kohtaan, 
-0000d420: 6a6f 7373 6120 6b61 6976 6f20 6f6e 2e20  jossa kaivo on. 
-0000d430: 4f68 6a65 6c6d 6120 7661 726d 6973 7461  Ohjelma varmista
-0000d440: 6120 7669 656c 5c78 4534 2076 616c 696e  a viel\xE4 valin
-0000d450: 6e61 6e0a 2020 2020 2020 2020 6f69 6b65  nan.        oike
-0000d460: 616b 7369 203c 2f64 6976 3e5c 725c 6e20  aksi </div>\r\n 
-0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d490: 2020 203c 6275 7474 6f6e 2064 6174 612d     <button data-
-0000d4a0: 6163 7469 6f6e 3d5c 226d 6172 6b2d 7765  action=\"mark-we
-0000d4b0: 6c6c 5c22 3e50 6169 6b6b 613c 2f62 7574  ll\">Paikka</but
-0000d4c0: 746f 6e3e 5c72 5c6e 0a20 2020 2020 2020  ton>\r\n.       
-0000d4d0: 205c 2020 2020 2020 2020 2020 2020 2020   \              
-0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4f0: 203c 2f64 6976 3e5c 725c 6e20 2020 2020   </div>\r\n     
+0000d2a0: 2020 2020 2020 2020 2020 3c64 6976 0a20            <div. 
+0000d2b0: 2020 2020 2020 2063 6c61 7373 3d5c 2263         class=\"c
+0000d2c0: 6f6c 2d6d 642d 3420 636f 6c2d 6d64 2d70  ol-md-4 col-md-p
+0000d2d0: 7573 682d 385c 223e 5c72 5c6e 2020 2020  ush-8\">\r\n    
+0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2f0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0000d300: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+0000d310: 2273 686f 7070 696e 672d 6361 7274 5c22  "shopping-cart\"
+0000d320: 2064 6174 612d 726f 6c65 3d5c 2273 686f   data-role=\"sho
+0000d330: 7070 696e 672d 6361 7274 5c22 3e5c 725c  pping-cart\">\r\
+0000d340: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d360: 2020 2020 203c 6469 760a 2020 2020 2020       <div.      
+0000d370: 2020 636c 6173 733d 5c22 666f 726d 2d67    class=\"form-g
+0000d380: 726f 7570 5c22 3e5c 725c 6e20 2020 2020  roup\">\r\n     
+0000d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3b0: 2020 203c 6469 7620 6461 7461 2d72 6f6c     <div data-rol
+0000d3c0: 653d 5c22 6772 6964 5c22 3e3c 2f64 6976  e=\"grid\"></div
+0000d3d0: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
+0000d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d400: 2020 3c2f 6469 763e 5c72 5c6e 2020 2020    </div>\r\n    
+0000d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d430: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
+0000d440: 7373 3d5c 2266 6f72 6d2d 6772 6f75 705c  ss=\"form-group\
+0000d450: 223e 5c72 5c6e 2020 2020 2020 2020 2020  ">\r\n          
+0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d470: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
+0000d480: 7574 746f 6e20 7479 7065 3d5c 2262 7574  utton type=\"but
+0000d490: 746f 6e5c 220a 2020 2020 2020 2020 636c  ton\".        cl
+0000d4a0: 6173 733d 5c22 6274 6e20 6274 6e2d 7072  ass=\"btn btn-pr
+0000d4b0: 696d 6172 7920 6469 7361 626c 6564 5c22  imary disabled\"
+0000d4c0: 2064 6174 612d 6163 7469 6f6e 3d5c 226f   data-action=\"o
+0000d4d0: 7264 6572 5c22 3e54 696c 6161 3c2f 6275  rder\">Tilaa</bu
+0000d4e0: 7474 6f6e 3e5c 725c 6e0a 2020 2020 2020  tton>\r\n.      
+0000d4f0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
 0000d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d510: 2020 2020 2020 2020 2020 203c 6469 760a             <div.
-0000d520: 2020 2020 2020 2020 6461 7461 2d72 6f6c          data-rol
-0000d530: 653d 5c22 6b61 7274 7461 5c22 2063 6c61  e=\"kartta\" cla
-0000d540: 7373 3d5c 226d 6170 5c22 3e3c 2f64 6976  ss=\"map\"></div
-0000d550: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-0000d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d570: 203c 2f64 6976 3e5c 725c 6e0a 2020 2020   </div>\r\n.    
-0000d580: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-0000d590: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-0000d5a0: 763e 5c72 5c6e 5c72 5c6e 2020 2020 2020  v>\r\n\r\n      
-0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5c0: 2020 3c64 6976 2064 6174 612d 726f 6c65    <div data-role
-0000d5d0: 3d5c 2262 7574 746f 6e73 5c22 3e3c 2f64  =\"buttons\"></d
-0000d5e0: 6976 3e5c 725c 6e0a 2020 2020 2020 2020  iv>\r\n.        
-0000d5f0: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-0000d600: 2020 2020 3c2f 6469 763e 5c72 5c6e 2020      </div>\r\n  
-0000d610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d620: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
-0000d630: 2020 2020 2020 2020 2020 3c64 6976 0a20            <div. 
-0000d640: 2020 2020 2020 2063 6c61 7373 3d5c 2261         class=\"a
-0000d650: 325c 223e 3c2f 6469 763e 5c72 5c6e 2020  2\"></div>\r\n  
-0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d670: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
-0000d680: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0000d690: 6c61 7373 3d5c 2261 335c 223e 3c2f 6469  lass=\"a3\"></di
-0000d6a0: 763e 5c72 5c6e 0a20 2020 2020 2020 205c  v>\r\n.        \
-0000d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6c0: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
-0000d6d0: 6134 5c22 3e3c 2f64 6976 3e5c 725c 6e20  a4\"></div>\r\n 
-0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6f0: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
-0000d700: 6135 5c22 3e3c 2f64 6976 3e5c 725c 6e0a  a5\"></div>\r\n.
-0000d710: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-0000d720: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-0000d730: 5c6e 5c72 5c6e 2020 2020 2020 2020 2020  \n\r\n          
-0000d740: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0000d750: 3d5c 2267 6c6f 6261 6c2d 7661 6c69 6461  =\"global-valida
-0000d760: 7469 6f6e 2d65 7272 6f72 0a20 2020 2020  tion-error.     
-0000d770: 2020 2061 6c65 7274 2061 6c65 7274 2d64     alert alert-d
-0000d780: 616e 6765 725c 2220 7374 796c 653d 5c22  anger\" style=\"
-0000d790: 6469 7370 6c61 793a 6e6f 6e65 5c22 3e54  display:none\">T
-0000d7a0: 5c78 4534 7974 5c78 4534 2070 7575 7474  \xE4yt\xE4 puutt
-0000d7b0: 7576 6174 206b 656e 745c 7845 3474 3c2f  uvat kent\xE4t</
-0000d7c0: 6469 763e 5c72 5c6e 5c72 5c6e 0a20 2020  div>\r\n\r\n.   
-0000d7d0: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-0000d7e0: 203c 2f64 6976 3e5c 725c 6e20 2020 2020   </div>\r\n     
-0000d7f0: 2020 203c 2f64 6976 3e5c 725c 6e20 2020     </div>\r\n   
-0000d800: 203c 2f64 6976 3e5c 725c 6e3c 2f64 6976   </div>\r\n</div
-0000d810: 3e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  >\r\n\r\n\r\n\r\
-0000d820: 6e5c 725c 6e3c 6469 760a 2020 2020 2020  n\r\n<div.      
-0000d830: 2020 6964 3d5c 2263 6f6d 706f 7374 2d6d    id=\"compost-m
-0000d840: 6f64 616c 5c22 2063 6c61 7373 3d5c 226d  odal\" class=\"m
-0000d850: 6f64 616c 5c22 2073 7479 6c65 3d5c 2264  odal\" style=\"d
-0000d860: 6973 706c 6179 3a6e 6f6e 655c 223e 5c72  isplay:none\">\r
-0000d870: 5c6e 5c74 3c64 6976 2063 6c61 7373 3d5c  \n\t<div class=\
-0000d880: 226d 6f64 616c 2d64 6961 6c6f 670a 2020  "modal-dialog.  
-0000d890: 2020 2020 2020 6d6f 6461 6c2d 6c67 5c22        modal-lg\"
-0000d8a0: 3e5c 725c 6e5c 745c 743c 6469 7620 636c  >\r\n\t\t<div cl
-0000d8b0: 6173 733d 5c22 6d6f 6461 6c2d 636f 6e74  ass=\"modal-cont
-0000d8c0: 656e 745c 223e 5c72 5c6e 5c74 5c74 5c74  ent\">\r\n\t\t\t
-0000d8d0: 3c64 6976 2063 6c61 7373 3d5c 226d 6f64  <div class=\"mod
-0000d8e0: 616c 2d62 6f64 795c 223e 5c72 5c6e 5c72  al-body\">\r\n\r
-0000d8f0: 5c6e 5c74 5c74 5c74 5c74 3c64 6976 0a20  \n\t\t\t\t<div. 
-0000d900: 2020 2020 2020 2063 6c61 7373 3d5c 2270         class=\"p
-0000d910: 6167 652d 6865 6164 6572 5c22 3e5c 725c  age-header\">\r\
-0000d920: 6e5c 745c 745c 745c 745c 745c 725c 6e5c  n\t\t\t\t\t\r\n\
-0000d930: 745c 745c 745c 745c 743c 6275 7474 6f6e  t\t\t\t\t<button
-0000d940: 2063 6c61 7373 3d5c 2270 756c 6c2d 7269   class=\"pull-ri
-0000d950: 6768 740a 2020 2020 2020 2020 6274 6e2d  ght.        btn-
-0000d960: 6469 736d 6973 735c 2220 6172 6961 2d6c  dismiss\" aria-l
-0000d970: 6162 656c 3d5c 2253 756c 6a65 5c22 2064  abel=\"Sulje\" d
-0000d980: 6174 612d 6163 7469 6f6e 3d5c 2263 616e  ata-action=\"can
-0000d990: 6365 6c2d 616c 6c5c 223e 3c2f 6275 7474  cel-all\"></butt
-0000d9a0: 6f6e 3e5c 725c 6e0a 2020 2020 2020 2020  on>\r\n.        
-0000d9b0: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-0000d9c0: 2020 2020 3c68 313e 4b6f 6d70 6f73 746f      <h1>Komposto
-0000d9d0: 696e 6e69 7374 6120 696c 6d6f 6974 7461  innista ilmoitta
-0000d9e0: 6d69 6e65 6e3c 2f68 313e 5c72 5c6e 5c74  minen</h1>\r\n\t
-0000d9f0: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
-0000da00: 5c74 5c74 0a20 2020 2020 2020 205c 2020  \t\t.        \  
-0000da10: 205c 745c 725c 6e5c 745c 7420 2020 205c   \t\r\n\t\t    \
-0000da20: 743c 6469 7620 636c 6173 733d 5c22 666f  t<div class=\"fo
-0000da30: 726d 5c22 3e3c 2f64 6976 3e5c 725c 6e5c  rm\"></div>\r\n\
-0000da40: 725c 6e5c 745c 7420 2020 205c 743c 6469  r\n\t\t    \t<di
-0000da50: 7620 636c 6173 733d 5c22 676c 6f62 616c  v class=\"global
-0000da60: 2d76 616c 6964 6174 696f 6e2d 6572 726f  -validation-erro
-0000da70: 720a 2020 2020 2020 2020 616c 6572 7420  r.        alert 
-0000da80: 616c 6572 742d 6461 6e67 6572 5c22 2073  alert-danger\" s
-0000da90: 7479 6c65 3d5c 2264 6973 706c 6179 3a6e  tyle=\"display:n
-0000daa0: 6f6e 655c 223e 5c72 5c6e 5c74 5c74 2020  one\">\r\n\t\t  
-0000dab0: 2020 5c74 5c74 545c 7845 3479 745c 7845    \t\tT\xE4yt\xE
-0000dac0: 3420 7075 7574 7475 7661 740a 2020 2020  4 puuttuvat.    
-0000dad0: 2020 2020 6b65 6e74 5c78 4534 745c 725c      kent\xE4t\r\
-0000dae0: 6e5c 745c 7420 2020 205c 743c 2f64 6976  n\t\t    \t</div
-0000daf0: 3e5c 725c 6e5c 745c 745c 743c 2f64 6976  >\r\n\t\t\t</div
-0000db00: 3e5c 725c 6e5c 745c 743c 2f64 6976 3e5c  >\r\n\t\t</div>\
-0000db10: 725c 6e5c 743c 2f64 6976 3e5c 725c 6e3c  r\n\t</div>\r\n<
-0000db20: 2f64 6976 3e5c 725c 6e5c 725c 6e5c 725c  /div>\r\n\r\n\r\
-0000db30: 6e5c 725c 6e3c 6469 760a 2020 2020 2020  n\r\n<div.      
-0000db40: 2020 6964 3d5c 2272 6567 6973 7465 722d    id=\"register-
-0000db50: 6d6f 6461 6c5c 2220 636c 6173 733d 5c22  modal\" class=\"
-0000db60: 6d6f 6461 6c5c 2220 7374 796c 653d 5c22  modal\" style=\"
-0000db70: 6469 7370 6c61 793a 6e6f 6e65 5c22 3e5c  display:none\">\
-0000db80: 725c 6e5c 743c 6469 7620 636c 6173 733d  r\n\t<div class=
-0000db90: 5c22 6d6f 6461 6c2d 6469 616c 6f67 0a20  \"modal-dialog. 
-0000dba0: 2020 2020 2020 206d 6f64 616c 2d6c 675c         modal-lg\
-0000dbb0: 223e 5c72 5c6e 5c74 5c74 3c64 6976 2063  ">\r\n\t\t<div c
-0000dbc0: 6c61 7373 3d5c 226d 6f64 616c 2d63 6f6e  lass=\"modal-con
-0000dbd0: 7465 6e74 5c22 3e5c 725c 6e5c 745c 745c  tent\">\r\n\t\t\
-0000dbe0: 743c 6469 7620 636c 6173 733d 5c22 6d6f  t<div class=\"mo
-0000dbf0: 6461 6c2d 626f 6479 5c22 3e5c 725c 6e5c  dal-body\">\r\n\
-0000dc00: 745c 745c 745c 725c 6e5c 745c 745c 745c  t\t\t\r\n\t\t\t\
-0000dc10: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
-0000dc20: 6173 733d 5c22 7061 6765 2d68 6561 6465  ass=\"page-heade
-0000dc30: 725c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  r\">\r\n\t\t\t\t
-0000dc40: 5c74 3c68 313e 5469 6c61 6120 6b5c 7845  \t<h1>Tilaa k\xE
-0000dc50: 3479 7474 5c78 4534 6a5c 7845 3474 756e  4ytt\xE4j\xE4tun
-0000dc60: 6e75 733c 2f68 313e 5c72 5c6e 5c74 5c74  nus</h1>\r\n\t\t
-0000dc70: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c72  \t\t</div>\r\n\r
-0000dc80: 5c6e 5c74 5c74 5c74 5c74 3c64 6976 0a20  \n\t\t\t\t<div. 
-0000dc90: 2020 2020 2020 2063 6c61 7373 3d5c 2266         class=\"f
-0000dca0: 6f72 6d5c 223e 3c2f 6469 763e 5c72 5c6e  orm\"></div>\r\n
-0000dcb0: 5c72 5c6e 5c74 5c74 5c74 3c2f 6469 763e  \r\n\t\t\t</div>
-0000dcc0: 5c72 5c6e 5c74 5c74 3c2f 6469 763e 5c72  \r\n\t\t</div>\r
-0000dcd0: 5c6e 5c74 3c2f 6469 763e 5c72 5c6e 3c2f  \n\t</div>\r\n</
-0000dce0: 6469 763e 5c72 5c6e 5c72 5c6e 5c72 5c6e  div>\r\n\r\n\r\n
-0000dcf0: 5c72 5c6e 3c64 6976 0a20 2020 2020 2020  \r\n<div.       
-0000dd00: 2069 643d 5c22 626f 6f6b 7570 2d6d 6f64   id=\"bookup-mod
-0000dd10: 616c 5c22 2063 6c61 7373 3d5c 226d 6f64  al\" class=\"mod
-0000dd20: 616c 5c22 2073 7479 6c65 3d5c 2264 6973  al\" style=\"dis
-0000dd30: 706c 6179 3a6e 6f6e 655c 223e 5c72 5c6e  play:none\">\r\n
-0000dd40: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
-0000dd50: 226d 6f64 616c 2d64 6961 6c6f 670a 2020  "modal-dialog.  
-0000dd60: 2020 2020 2020 6d6f 6461 6c2d 6c67 5c22        modal-lg\"
-0000dd70: 3e5c 725c 6e20 2020 2020 2020 203c 6469  >\r\n        <di
-0000dd80: 7620 636c 6173 733d 5c22 6d6f 6461 6c2d  v class=\"modal-
-0000dd90: 636f 6e74 656e 745c 223e 5c72 5c6e 2020  content\">\r\n  
-0000dda0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0000ddb0: 6c61 7373 3d5c 226d 6f64 616c 2d62 6f64  lass=\"modal-bod
-0000ddc0: 795c 223e 5c72 5c6e 0a20 2020 2020 2020  y\">\r\n.       
-0000ddd0: 205c 2020 2020 2020 2020 2020 2020 2020   \              
-0000dde0: 203c 6469 7620 636c 6173 733d 5c22 7061   <div class=\"pa
-0000ddf0: 6765 2d68 6561 6465 725c 223e 5c72 5c6e  ge-header\">\r\n
-0000de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de10: 2020 2020 3c62 7574 746f 6e0a 2020 2020      <button.    
-0000de20: 2020 2020 636c 6173 733d 5c22 7075 6c6c      class=\"pull
-0000de30: 2d72 6967 6874 2062 746e 2d64 6973 6d69  -right btn-dismi
-0000de40: 7373 2063 616e 6365 6c5c 223e 3c2f 6275  ss cancel\"></bu
-0000de50: 7474 6f6e 3e5c 725c 6e20 2020 2020 2020  tton>\r\n       
-0000de60: 2020 2020 2020 2020 2020 2020 203c 6831               <h1
-0000de70: 3e54 696c 6161 0a20 2020 2020 2020 2070  >Tilaa.        p
-0000de80: 616c 7665 6c75 6974 613c 2f68 313e 5c72  alveluita</h1>\r
-0000de90: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0000dea0: 2020 3c2f 6469 763e 5c72 5c6e 5c72 5c6e    </div>\r\n\r\n
-0000deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dec0: 3c64 6976 2063 6c61 7373 3d5c 2263 6f6d  <div class=\"com
-0000ded0: 6d75 6e69 7479 2d66 6f72 6d5c 223e 5c72  munity-form\">\r
-0000dee0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-0000def0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000df00: 666f 726d 3e5c 725c 6e20 2020 2020 2020  form>\r\n       
-0000df10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df20: 203c 6469 7620 636c 6173 733d 5c22 666f   <div class=\"fo
-0000df30: 726d 2d67 726f 7570 5c22 3e5c 725c 6e0a  rm-group\">\r\n.
-0000df40: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df60: 2020 2020 3c6c 6162 656c 2066 6f72 3d5c      <label for=\
-0000df70: 2263 6f6d 6d75 6e69 7479 2d73 656c 6563  "community-selec
-0000df80: 745c 2220 636c 6173 733d 5c22 636f 6e74  t\" class=\"cont
-0000df90: 726f 6c2d 6c61 6265 6c5c 223e 5661 6c69  rol-label\">Vali
-0000dfa0: 7473 650a 2020 2020 2020 2020 6b75 6e74  tse.        kunt
-0000dfb0: 612c 206a 6f73 7361 2061 7375 743c 2f6c  a, jossa asut</l
-0000dfc0: 6162 656c 3e5c 725c 6e20 2020 2020 2020  abel>\r\n       
-0000dfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfe0: 2020 2020 203c 7365 6c65 6374 2069 643d       <select id=
-0000dff0: 5c22 636f 6d6d 756e 6974 792d 7365 6c65  \"community-sele
-0000e000: 6374 5c22 0a20 2020 2020 2020 206e 616d  ct\".        nam
-0000e010: 653d 5c22 636f 6d6d 756e 6974 792d 7365  e=\"community-se
-0000e020: 6c65 6374 5c22 2064 6174 612d 726f 6c65  lect\" data-role
-0000e030: 3d5c 2263 6f6d 6d75 6e69 7479 2d73 656c  =\"community-sel
-0000e040: 6563 745c 2220 636c 6173 733d 5c22 666f  ect\" class=\"fo
-0000e050: 726d 2d63 6f6e 7472 6f6c 5c22 3e3c 2f73  rm-control\"></s
-0000e060: 656c 6563 743e 5c72 5c6e 0a20 2020 2020  elect>\r\n.     
-0000e070: 2020 205c 2020 2020 2020 2020 2020 2020     \            
-0000e080: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-0000e090: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-0000e0a0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000e0b0: 7620 6964 3d5c 2265 7874 7261 2d6e 6f74  v id=\"extra-not
-0000e0c0: 655c 220a 2020 2020 2020 2020 636c 6173  e\".        clas
-0000e0d0: 733d 5c22 666f 726d 2d67 726f 7570 5c22  s=\"form-group\"
-0000e0e0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-0000e0f0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-0000e100: 6976 3e5c 725c 6e20 2020 2020 2020 2020  iv>\r\n         
-0000e110: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e120: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-0000e130: 733d 5c22 666f 726d 2d67 726f 7570 5c22  s=\"form-group\"
-0000e140: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-0000e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e160: 203c 6275 7474 6f6e 2074 7970 653d 5c22   <button type=\"
-0000e170: 6275 7474 6f6e 5c22 0a20 2020 2020 2020  button\".       
-0000e180: 2063 6c61 7373 3d5c 2262 746e 2062 746e   class=\"btn btn
-0000e190: 2d70 7269 6d61 7279 2064 6973 6162 6c65  -primary disable
-0000e1a0: 645c 2220 6461 7461 2d61 6374 696f 6e3d  d\" data-action=
-0000e1b0: 5c22 7365 6c65 6374 2d63 6f6d 6d75 6e69  \"select-communi
-0000e1c0: 7479 5c22 3e4f 6b3c 2f62 7574 746f 6e3e  ty\">Ok</button>
-0000e1d0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1f0: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
-0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e210: 2020 203c 2f66 6f72 6d3e 5c72 5c6e 2020     </form>\r\n  
-0000e220: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0000e230: 6469 763e 5c72 5c6e 5c72 5c6e 0a20 2020  div>\r\n\r\n.   
-0000e240: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-0000e250: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000e260: 5c22 7368 6f70 7069 6e67 2d70 6167 655c  \"shopping-page\
-0000e270: 2220 7374 796c 653d 5c22 6469 7370 6c61  " style=\"displa
-0000e280: 793a 6e6f 6e65 5c22 3e5c 725c 6e20 2020  y:none\">\r\n   
-0000e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2a0: 203c 6469 760a 2020 2020 2020 2020 636c   <div.        cl
-0000e2b0: 6173 733d 5c22 7368 6f70 7069 6e67 2d63  ass=\"shopping-c
-0000e2c0: 6172 742d 636f 6e74 656e 745c 2220 7374  art-content\" st
-0000e2d0: 796c 653d 5c22 6469 7370 6c61 793a 6e6f  yle=\"display:no
-0000e2e0: 6e65 5c22 3e5c 725c 6e20 2020 2020 2020  ne\">\r\n       
-0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e300: 203c 6469 760a 2020 2020 2020 2020 636c   <div.        cl
-0000e310: 6173 733d 5c22 666f 726d 5c22 3e3c 2f64  ass=\"form\"></d
-0000e320: 6976 3e5c 725c 6e20 2020 2020 2020 2020  iv>\r\n         
-0000e330: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e340: 6469 7620 636c 6173 733d 5c22 676c 6f62  div class=\"glob
-0000e350: 616c 2d76 616c 6964 6174 696f 6e2d 6572  al-validation-er
-0000e360: 726f 720a 2020 2020 2020 2020 616c 6572  ror.        aler
-0000e370: 7420 616c 6572 742d 6461 6e67 6572 5c22  t alert-danger\"
-0000e380: 2073 7479 6c65 3d5c 2264 6973 706c 6179   style=\"display
-0000e390: 3a6e 6f6e 655c 223e 5c72 5c6e 2020 2020  :none\">\r\n    
-0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3b0: 2020 2020 2020 2020 545c 7845 3479 745c          T\xE4yt\
-0000e3c0: 7845 340a 2020 2020 2020 2020 7075 7574  xE4.        puut
-0000e3d0: 7475 7661 7420 6b65 6e74 5c78 4534 745c  tuvat kent\xE4t\
-0000e3e0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-0000e3f0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-0000e400: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-0000e410: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-0000e420: 725c 6e5c 725c 6e0a 2020 2020 2020 2020  r\n\r\n.        
-0000e430: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-0000e440: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
-0000e450: 2272 6f77 5c22 3e5c 725c 6e20 2020 2020  "row\">\r\n     
-0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e470: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
-0000e480: 636f 6c2d 6d64 2d31 320a 2020 2020 2020  col-md-12.      
-0000e490: 2020 7465 7874 2d63 656e 7465 725c 223e    text-center\">
-0000e4a0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4c0: 3c64 6976 2064 6174 612d 726f 6c65 3d5c  <div data-role=\
-0000e4d0: 2274 6f6f 6c62 6172 5c22 3e3c 2f64 6976  "toolbar\"></div
-0000e4e0: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
-0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e500: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
-0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e520: 2020 2020 3c2f 6469 763e 5c72 5c6e 5c72      </div>\r\n\r
-0000e530: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0000e540: 2020 2020 2020 3c64 6976 0a20 2020 2020        <div.     
-0000e550: 2020 2063 6c61 7373 3d5c 2273 686f 7070     class=\"shopp
-0000e560: 696e 672d 7061 6765 2d63 6f6e 7465 6e74  ing-page-content
-0000e570: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
-0000e580: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e590: 6469 7620 636c 6173 733d 5c22 726f 775c  div class=\"row\
-0000e5a0: 223e 5c72 5c6e 0a20 2020 2020 2020 205c  ">\r\n.        \
-0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5c0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000e5d0: 636c 6173 733d 5c22 636f 6c2d 6d64 2d31  class=\"col-md-1
-0000e5e0: 325c 223e 5c72 5c6e 2020 2020 2020 2020  2\">\r\n        
-0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e600: 2020 2020 2020 2020 3c6c 6162 656c 0a20          <label. 
-0000e610: 2020 2020 2020 2064 6174 612d 726f 6c65         data-role
-0000e620: 3d5c 2273 7562 6361 7465 676f 7279 2d68  =\"subcategory-h
-0000e630: 6561 6465 725c 223e 416c 696b 6174 6567  eader\">Alikateg
-0000e640: 6f72 6961 3c2f 6c61 6265 6c3e 5c72 5c6e  oria</label>\r\n
-0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e670: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
-0000e680: 7373 3d5c 2273 7562 6361 7465 676f 7279  ss=\"subcategory
-0000e690: 2d74 6f6f 6c62 6172 5c22 2064 6174 612d  -toolbar\" data-
-0000e6a0: 726f 6c65 3d5c 2273 7562 6361 7465 676f  role=\"subcatego
-0000e6b0: 7279 2d74 6f6f 6c62 6172 5c22 3e3c 2f64  ry-toolbar\"></d
-0000e6c0: 6976 3e5c 725c 6e0a 2020 2020 2020 2020  iv>\r\n.        
-0000e6d0: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-0000e6e0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-0000e6f0: 763e 5c72 5c6e 2020 2020 2020 2020 2020  v>\r\n          
-0000e700: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0000e710: 6469 763e 5c72 5c6e 5c72 5c6e 0a20 2020  div>\r\n\r\n.   
-0000e720: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-0000e730: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000e740: 7620 636c 6173 733d 5c22 726f 775c 223e  v class=\"row\">
-0000e750: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e770: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
-0000e780: 7373 3d5c 2263 6f6c 2d6d 642d 3420 636f  ss=\"col-md-4 co
-0000e790: 6c2d 6d64 2d70 7573 682d 385c 223e 5c72  l-md-push-8\">\r
-0000e7a0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7c0: 2020 3c64 6976 0a20 2020 2020 2020 2063    <div.        c
-0000e7d0: 6c61 7373 3d5c 2273 686f 7070 696e 672d  lass=\"shopping-
-0000e7e0: 6361 7274 5c22 2064 6174 612d 726f 6c65  cart\" data-role
-0000e7f0: 3d5c 2273 686f 7070 696e 672d 6361 7274  =\"shopping-cart
-0000e800: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
-0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e820: 2020 2020 2020 2020 2020 203c 6469 760a             <div.
-0000e830: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-0000e840: 666f 726d 2d67 726f 7570 5c22 3e5c 725c  form-group\">\r\
-0000e850: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0000e860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e870: 2020 2020 2020 2020 203c 6469 7620 6461           <div da
-0000e880: 7461 2d72 6f6c 653d 5c22 6772 6964 5c22  ta-role=\"grid\"
-0000e890: 3e3c 2f64 6976 3e5c 725c 6e0a 2020 2020  ></div>\r\n.    
-0000e8a0: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8c0: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-0000e8d0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8f0: 2020 2020 2020 3c64 6976 0a20 2020 2020        <div.     
-0000e900: 2020 2063 6c61 7373 3d5c 2266 6f72 6d2d     class=\"form-
-0000e910: 6772 6f75 705c 223e 5c72 5c6e 2020 2020  group\">\r\n    
-0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e940: 2020 2020 3c62 7574 746f 6e20 7479 7065      <button type
-0000e950: 3d5c 2262 7574 746f 6e5c 220a 2020 2020  =\"button\".    
-0000e960: 2020 2020 636c 6173 733d 5c22 6274 6e20      class=\"btn 
-0000e970: 6274 6e2d 7072 696d 6172 7920 6469 7361  btn-primary disa
-0000e980: 626c 6564 5c22 2064 6174 612d 6163 7469  bled\" data-acti
-0000e990: 6f6e 3d5c 226f 7264 6572 5c22 3e54 696c  on=\"order\">Til
-0000e9a0: 6161 3c2f 6275 7474 6f6e 3e5c 725c 6e0a  aa</button>\r\n.
-0000e9b0: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9d0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-0000e9e0: 763e 5c72 5c6e 2020 2020 2020 2020 2020  v>\r\n          
-0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea00: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
-0000ea10: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
-0000ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea50: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000ea60: 636c 6173 733d 5c22 636f 6c2d 6d64 2d38  class=\"col-md-8
-0000ea70: 0a20 2020 2020 2020 2063 6f6c 2d6d 642d  .        col-md-
-0000ea80: 7075 6c6c 2d34 5c22 3e5c 725c 6e20 2020  pull-4\">\r\n   
-0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eaa0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0000eab0: 7620 636c 6173 733d 5c22 616c 6572 7420  v class=\"alert 
-0000eac0: 616c 6572 742d 696e 666f 5c22 0a20 2020  alert-info\".   
-0000ead0: 2020 2020 2064 6174 612d 726f 6c65 3d5c       data-role=\
-0000eae0: 226d 6573 7361 6765 5c22 3e3c 2f64 6976  "message\"></div
-0000eaf0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb10: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000eb20: 5c22 7072 6f64 7563 742d 6c69 7374 5c22  \"product-list\"
-0000eb30: 0a20 2020 2020 2020 2064 6174 612d 726f  .        data-ro
-0000eb40: 6c65 3d5c 2270 726f 6475 6374 2d6c 6973  le=\"product-lis
-0000eb50: 745c 223e 3c2f 6469 763e 5c72 5c6e 2020  t\"></div>\r\n  
-0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb70: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-0000eb80: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-0000eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eba0: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
-0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebc0: 2020 203c 2f64 6976 3e5c 725c 6e5c 725c     </div>\r\n\r\
-0000ebd0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0000ebe0: 2020 2020 205c 725c 6e0a 2020 2020 2020       \r\n.      
-0000ebf0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-0000ec00: 2020 2020 2020 2020 2020 5c72 5c6e 2020            \r\n  
-0000ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec20: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
-0000ec30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec40: 2020 5c72 5c6e 0a20 2020 2020 2020 205c    \r\n.        \
-0000ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec60: 2020 2020 2020 203c 6469 7620 6461 7461         <div data
-0000ec70: 2d72 6f6c 653d 5c22 7265 7073 696b 6b61  -role=\"repsikka
-0000ec80: 2d74 6162 5c22 3e5c 725c 6e20 2020 2020  -tab\">\r\n     
-0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eca0: 2020 2020 2020 203c 700a 2020 2020 2020         <p.      
-0000ecb0: 2020 636c 6173 733d 5c22 616c 6572 7420    class=\"alert 
-0000ecc0: 616c 6572 742d 696e 666f 5c22 3e3c 2f70  alert-info\"></p
-0000ecd0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-0000ece0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecf0: 203c 6469 7620 6461 7461 2d72 6f6c 653d   <div data-role=
-0000ed00: 5c22 666f 726d 5c22 3e3c 2f64 6976 3e5c  \"form\"></div>\
-0000ed10: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-0000ed20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed30: 2020 2020 2020 2020 3c70 3e54 6172 6b69          <p>Tarki
-0000ed40: 7374 6120 7968 7465 7973 7469 6574 6f73  sta yhteystietos
-0000ed50: 692e 2048 756f 6d69 6f69 7468 616e 2065  i. Huomioithan e
-0000ed60: 7269 7479 6973 6573 7469 2c0a 2020 2020  rityisesti,.    
-0000ed70: 2020 2020 6574 745c 7845 3420 7461 7276      ett\xE4 tarv
-0000ed80: 6974 7365 6d6d 6520 7075 6865 6c69 6e6e  itsemme puhelinn
-0000ed90: 756d 6572 6f6e 2c20 6a6f 7374 6120 7369  umeron, josta si
-0000eda0: 6e75 7420 7461 766f 6974 7461 6120 705c  nut tavoittaa p\
-0000edb0: 7845 3469 765c 7845 3473 6169 6b61 616e  xE4iv\xE4saikaan
-0000edc0: 2e3c 2f70 3e3c 703e 5661 6876 6973 7461  .</p><p>Vahvista
-0000edd0: 6d6d 650a 2020 2020 2020 2020 7469 6c61  mme.        tila
-0000ede0: 756b 7365 6e20 7669 656c 5c78 4534 2073  uksen viel\xE4 s
-0000edf0: 5c78 4534 686b 5c78 4636 706f 7374 6974  \xE4hk\xF6postit
-0000ee00: 7365 2074 6169 2070 7568 656c 696d 6974  se tai puhelimit
-0000ee10: 7365 2e3c 2f70 3e5c 725c 6e20 2020 2020  se.</p>\r\n     
-0000ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee30: 2020 2020 2020 203c 6469 760a 2020 2020         <div.    
-0000ee40: 2020 2020 636c 6173 733d 5c22 666f 726d      class=\"form
-0000ee50: 2d62 7574 746f 6e73 2074 6578 742d 6365  -buttons text-ce
-0000ee60: 6e74 6572 5c22 3e5c 725c 6e20 2020 2020  nter\">\r\n     
-0000ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee80: 2020 2020 2020 2020 2020 203c 6275 7474             <butt
-0000ee90: 6f6e 0a20 2020 2020 2020 2074 7970 653d  on.        type=
-0000eea0: 5c22 6275 7474 6f6e 5c22 2064 6174 612d  \"button\" data-
-0000eeb0: 6163 7469 6f6e 3d5c 2273 656e 645c 2220  action=\"send\" 
-0000eec0: 636c 6173 733d 5c22 6274 6e20 6274 6e2d  class=\"btn btn-
-0000eed0: 7072 696d 6172 795c 223e 4c5c 7845 3468  primary\">L\xE4h
-0000eee0: 6574 5c78 4534 3c2f 6275 7474 6f6e 3e5c  et\xE4</button>\
-0000eef0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-0000ef00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef10: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-0000ef20: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0000ef30: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0000ef40: 6976 2063 6c61 7373 3d5c 2267 6c6f 6261  iv class=\"globa
-0000ef50: 6c2d 7661 6c69 6461 7469 6f6e 2d65 7272  l-validation-err
-0000ef60: 6f72 0a20 2020 2020 2020 2061 6c65 7274  or.        alert
-0000ef70: 2061 6c65 7274 2d64 616e 6765 725c 2220   alert-danger\" 
-0000ef80: 7374 796c 653d 5c22 6469 7370 6c61 793a  style=\"display:
-0000ef90: 6e6f 6e65 5c22 3e5c 725c 6e20 2020 2020  none\">\r\n     
-0000efa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efb0: 2020 2020 2020 2020 2020 2054 5c78 4534             T\xE4
-0000efc0: 7974 5c78 4534 0a20 2020 2020 2020 2070  yt\xE4.        p
-0000efd0: 7575 7474 7576 6174 206b 656e 745c 7845  uuttuvat kent\xE
-0000efe0: 3474 5c72 5c6e 2020 2020 2020 2020 2020  4t\r\n          
-0000eff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f000: 2020 3c2f 6469 763e 5c72 5c6e 2020 2020    </div>\r\n    
-0000f010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f020: 2020 2020 3c2f 6469 763e 5c72 5c6e 0a20      </div>\r\n. 
-0000f030: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-0000f040: 2020 2020 2020 2020 2020 2020 2020 205c                 \
-0000f050: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-0000f060: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
-0000f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f080: 2020 205c 725c 6e0a 2020 2020 2020 2020     \r\n.        
-0000f090: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-0000f0a0: 3c2f 6469 763e 5c72 5c6e 2020 2020 2020  </div>\r\n      
-0000f0b0: 2020 2020 2020 2020 2020 3c62 7574 746f            <butto
-0000f0c0: 6e20 636c 6173 733d 5c22 6274 6e20 6274  n class=\"btn bt
-0000f0d0: 6e2d 6465 6661 756c 740a 2020 2020 2020  n-default.      
-0000f0e0: 2020 6361 6e63 656c 5c22 3e50 6572 7575    cancel\">Peruu
-0000f0f0: 7461 3c2f 6275 7474 6f6e 3e5c 725c 6e20  ta</button>\r\n 
-0000f100: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000f110: 6469 7620 636c 6173 733d 5c22 636c 6561  div class=\"clea
-0000f120: 7266 6978 5c22 3e3c 2f64 6976 3e5c 725c  rfix\"></div>\r\
-0000f130: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
-0000f140: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
-0000f150: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-0000f160: 5c6e 2020 2020 3c2f 6469 763e 5c72 5c6e  \n    </div>\r\n
-0000f170: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 5c72  </div>\r\n\r\n\r
-0000f180: 5c6e 5c72 5c6e 3c64 6976 0a20 2020 2020  \n\r\n<div.     
-0000f190: 2020 2069 643d 5c22 6665 6564 6261 636b     id=\"feedback
-0000f1a0: 2d6d 6f64 616c 5c22 2063 6c61 7373 3d5c  -modal\" class=\
-0000f1b0: 226d 6f64 616c 5c22 2073 7479 6c65 3d5c  "modal\" style=\
-0000f1c0: 2264 6973 706c 6179 3a6e 6f6e 655c 223e  "display:none\">
-0000f1d0: 5c72 5c6e 2020 2020 3c64 6976 0a20 2020  \r\n    <div.   
-0000f1e0: 2020 2020 2063 6c61 7373 3d5c 226d 6f64       class=\"mod
-0000f1f0: 616c 2d64 6961 6c6f 675c 223e 5c72 5c6e  al-dialog\">\r\n
-0000f200: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0000f210: 7373 3d5c 226d 6f64 616c 2d63 6f6e 7465  ss=\"modal-conte
-0000f220: 6e74 5c22 3e5c 725c 6e20 2020 2020 2020  nt\">\r\n       
-0000f230: 2020 2020 203c 6469 760a 2020 2020 2020       <div.      
-0000f240: 2020 636c 6173 733d 5c22 6d6f 6461 6c2d    class=\"modal-
-0000f250: 626f 6479 5c22 3e5c 725c 6e20 2020 2020  body\">\r\n     
-0000f260: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000f270: 636c 6173 733d 5c22 7061 6765 2d68 6561  class=\"page-hea
-0000f280: 6465 725c 223e 5c72 5c6e 2020 2020 2020  der\">\r\n      
-0000f290: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
-0000f2a0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-0000f2b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000f2c0: 6275 7474 6f6e 2063 6c61 7373 3d5c 2270  button class=\"p
-0000f2d0: 756c 6c2d 7269 6768 7420 6274 6e2d 6469  ull-right btn-di
-0000f2e0: 736d 6973 735c 2220 6172 6961 2d6c 6162  smiss\" aria-lab
-0000f2f0: 656c 3d5c 2253 756c 6a65 5c22 0a20 2020  el=\"Sulje\".   
-0000f300: 2020 2020 2064 6174 612d 6163 7469 6f6e       data-action
-0000f310: 3d5c 2263 616e 6365 6c2d 616c 6c5c 223e  =\"cancel-all\">
-0000f320: 3c2f 6275 7474 6f6e 3e5c 725c 6e20 2020  </button>\r\n   
-0000f330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f340: 203c 6831 3e41 6e6e 6120 7061 6c61 7574   <h1>Anna palaut
-0000f350: 6574 7461 3c2f 6831 3e5c 725c 6e0a 2020  etta</h1>\r\n.  
-0000f360: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-0000f370: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
-0000f380: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-0000f390: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
-0000f3a0: 2266 6f72 6d5c 223e 3c2f 6469 763e 5c72  "form\"></div>\r
-0000f3b0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-0000f3c0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0000f3d0: 636c 6173 733d 5c22 676c 6f62 616c 2d76  class=\"global-v
-0000f3e0: 616c 6964 6174 696f 6e2d 6572 726f 7220  alidation-error 
-0000f3f0: 616c 6572 7420 616c 6572 742d 6461 6e67  alert alert-dang
-0000f400: 6572 5c22 0a20 2020 2020 2020 2073 7479  er\".        sty
-0000f410: 6c65 3d5c 2264 6973 706c 6179 3a6e 6f6e  le=\"display:non
-0000f420: 655c 223e 5c72 5c6e 2020 2020 2020 2020  e\">\r\n        
-0000f430: 2020 2020 2020 2020 2020 2020 545c 7845              T\xE
-0000f440: 3479 745c 7845 3420 7075 7574 7475 7661  4yt\xE4 puuttuva
-0000f450: 7420 6b65 6e74 5c78 4534 745c 725c 6e0a  t kent\xE4t\r\n.
-0000f460: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-0000f470: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-0000f480: 5c6e 2020 2020 2020 2020 2020 2020 3c2f  \n            </
-0000f490: 6469 763e 5c72 5c6e 2020 2020 2020 2020  div>\r\n        
-0000f4a0: 3c2f 6469 763e 5c72 5c6e 2020 2020 3c2f  </div>\r\n    </
-0000f4b0: 6469 763e 5c72 5c6e 3c2f 6469 763e 5c72  div>\r\n</div>\r
-0000f4c0: 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72  \n\r\n\r\n\r\n\r
-0000f4d0: 5c6e 3c64 6976 0a20 2020 2020 2020 2069  \n<div.        i
-0000f4e0: 643d 5c22 666f 7267 6f74 7465 6e2d 7061  d=\"forgotten-pa
-0000f4f0: 7373 776f 7264 2d6d 6f64 616c 5c22 2063  ssword-modal\" c
-0000f500: 6c61 7373 3d5c 226d 6f64 616c 5c22 2073  lass=\"modal\" s
-0000f510: 7479 6c65 3d5c 2264 6973 706c 6179 3a6e  tyle=\"display:n
-0000f520: 6f6e 655c 223e 5c72 5c6e 0a20 2020 2020  one\">\r\n.     
-0000f530: 2020 205c 2020 203c 6469 7620 636c 6173     \   <div clas
-0000f540: 733d 5c22 6d6f 6461 6c2d 6469 616c 6f67  s=\"modal-dialog
-0000f550: 5c22 3e5c 725c 6e20 2020 2020 2020 203c  \">\r\n        <
-0000f560: 6469 7620 636c 6173 733d 5c22 6d6f 6461  div class=\"moda
-0000f570: 6c2d 636f 6e74 656e 745c 223e 5c72 5c6e  l-content\">\r\n
-0000f580: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-0000f590: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0000f5a0: 5c22 6d6f 6461 6c2d 626f 6479 5c22 3e5c  \"modal-body\">\
-0000f5b0: 725c 6e20 2020 2020 2020 2020 2020 205c  r\n            \
-0000f5c0: 743c 6469 7620 636c 6173 733d 5c22 7061  t<div class=\"pa
-0000f5d0: 6765 2d68 6561 6465 725c 223e 5c72 5c6e  ge-header\">\r\n
-0000f5e0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-0000f5f0: 2020 2020 205c 745c 743c 6832 3e54 696c       \t\t<h2>Til
-0000f600: 6161 2075 6e6f 6874 756e 7574 2073 616c  aa unohtunut sal
-0000f610: 6173 616e 613c 2f68 323e 5c72 5c6e 2020  asana</h2>\r\n  
-0000f620: 2020 2020 2020 2020 2020 5c74 3c2f 6469            \t</di
-0000f630: 763e 5c72 5c6e 5c72 5c6e 0a20 2020 2020  v>\r\n\r\n.     
-0000f640: 2020 205c 2020 2020 2020 2020 2020 2020     \            
-0000f650: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
-0000f660: 666f 726d 5c22 3e3c 2f64 6976 3e5c 725c  form\"></div>\r\
-0000f670: 6e20 2020 2020 2020 2020 2020 203c 2f64  n            </d
-0000f680: 6976 3e5c 725c 6e20 2020 2020 2020 203c  iv>\r\n        <
-0000f690: 2f64 6976 3e5c 725c 6e0a 2020 2020 2020  /div>\r\n.      
-0000f6a0: 2020 5c20 2020 3c2f 6469 763e 5c72 5c6e    \   </div>\r\n
-0000f6b0: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 5c72  </div>\r\n\r\n\r
-0000f6c0: 5c6e 5c72 5c6e 5c72 5c6e 3c64 6976 2069  \n\r\n\r\n<div i
-0000f6d0: 643d 5c22 7061 7373 776f 7264 2d6d 6f64  d=\"password-mod
-0000f6e0: 616c 5c22 2063 6c61 7373 3d5c 226d 6f64  al\" class=\"mod
-0000f6f0: 616c 5c22 0a20 2020 2020 2020 2073 7479  al\".        sty
-0000f700: 6c65 3d5c 2264 6973 706c 6179 3a6e 6f6e  le=\"display:non
-0000f710: 655c 223e 5c72 5c6e 5c74 3c64 6976 2063  e\">\r\n\t<div c
-0000f720: 6c61 7373 3d5c 226d 6f64 616c 2d64 6961  lass=\"modal-dia
-0000f730: 6c6f 675c 223e 5c72 5c6e 5c74 5c74 3c64  log\">\r\n\t\t<d
-0000f740: 6976 2063 6c61 7373 3d5c 226d 6f64 616c  iv class=\"modal
-0000f750: 2d63 6f6e 7465 6e74 5c22 3e5c 725c 6e5c  -content\">\r\n\
-0000f760: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
-0000f770: 2020 636c 6173 733d 5c22 6d6f 6461 6c2d    class=\"modal-
-0000f780: 626f 6479 5c22 3e5c 725c 6e5c 745c 745c  body\">\r\n\t\t\
-0000f790: 745c 743c 6469 7620 636c 6173 733d 5c22  t\t<div class=\"
-0000f7a0: 7061 6765 2d68 6561 6465 725c 223e 5c72  page-header\">\r
-0000f7b0: 5c6e 5c74 5c74 5c74 5c74 5c74 3c68 323e  \n\t\t\t\t\t<h2>
-0000f7c0: 5661 6968 6461 0a20 2020 2020 2020 2073  Vaihda.        s
-0000f7d0: 616c 6173 616e 613c 2f68 323e 5c72 5c6e  alasana</h2>\r\n
-0000f7e0: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
-0000f7f0: 5c6e 5c72 5c6e 5c74 5c74 5c74 5c74 3c64  \n\r\n\t\t\t\t<d
-0000f800: 6976 2063 6c61 7373 3d5c 2266 6f72 6d5c  iv class=\"form\
-0000f810: 2220 6461 7461 2d72 6f6c 653d 5c22 666f  " data-role=\"fo
-0000f820: 726d 5c22 3e3c 2f64 6976 3e5c 725c 6e5c  rm\"></div>\r\n\
-0000f830: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
-0000f840: 745c 743c 2f64 6976 3e5c 725c 6e5c 743c  t\t</div>\r\n\t<
-0000f850: 2f64 6976 3e5c 725c 6e3c 2f64 6976 3e5c  /div>\r\n</div>\
-0000f860: 725c 6e5c 725c 6e5c 725c 6e5c 725c 6e3c  r\n\r\n\r\n\r\n<
-0000f870: 7363 7269 7074 3e5c 725c 6e66 756e 6374  script>\r\nfunct
-0000f880: 696f 6e0a 2020 2020 2020 2020 7365 7276  ion.        serv
-0000f890: 6963 6553 656c 6563 746f 7243 6f6d 6269  iceSelectorCombi
-0000f8a0: 6e65 4e6f 6e42 6c61 6e6b 7328 7661 6c75  neNonBlanks(valu
-0000f8b0: 6573 2c20 7365 7061 7261 746f 7229 207b  es, separator) {
-0000f8c0: 5c72 5c6e 5c74 7661 7220 7265 7375 6c74  \r\n\tvar result
-0000f8d0: 203d 2027 273b 5c72 5c6e 5c74 666f 7228   = '';\r\n\tfor(
-0000f8e0: 7661 720a 2020 2020 2020 2020 6920 3d20  var.        i = 
-0000f8f0: 303b 2069 203c 2076 616c 7565 732e 6c65  0; i < values.le
-0000f900: 6e67 7468 3b20 2b2b 6929 207b 5c72 5c6e  ngth; ++i) {\r\n
-0000f910: 5c74 5c74 6966 2876 616c 7565 735b 695d  \t\tif(values[i]
-0000f920: 2021 3d3d 206e 756c 6c20 2626 2076 616c   !== null && val
-0000f930: 7565 735b 695d 0a20 2020 2020 2020 2021  ues[i].        !
-0000f940: 3d3d 2027 2729 207b 5c72 5c6e 5c74 5c74  == '') {\r\n\t\t
-0000f950: 5c74 6966 2872 6573 756c 7420 213d 3d20  \tif(result !== 
-0000f960: 2727 2920 7b5c 725c 6e5c 745c 745c 745c  '') {\r\n\t\t\t\
-0000f970: 7472 6573 756c 7420 2b3d 2073 6570 6172  tresult += separ
-0000f980: 6174 6f72 3b5c 725c 6e5c 745c 745c 747d  ator;\r\n\t\t\t}
-0000f990: 5c72 5c6e 5c74 5c74 5c74 7265 7375 6c74  \r\n\t\t\tresult
-0000f9a0: 0a20 2020 2020 2020 202b 3d20 7661 6c75  .        += valu
-0000f9b0: 6573 5b69 5d3b 5c72 5c6e 5c74 5c74 7d5c  es[i];\r\n\t\t}\
-0000f9c0: 725c 6e5c 747d 5c72 5c6e 5c74 7265 7475  r\n\t}\r\n\tretu
-0000f9d0: 726e 2072 6573 756c 743b 5c72 5c6e 7d5c  rn result;\r\n}\
-0000f9e0: 725c 6e5c 725c 6e66 756e 6374 696f 6e20  r\n\r\nfunction 
-0000f9f0: 7365 7276 6963 6553 656c 6563 746f 7249  serviceSelectorI
-0000fa00: 6e76 6f69 6369 6e67 2863 7573 746f 6d65  nvoicing(custome
-0000fa10: 7229 0a20 2020 2020 2020 207b 5c72 5c6e  r).        {\r\n
-0000fa20: 5c74 6966 2866 616c 7365 2026 2620 6375  \tif(false && cu
-0000fa30: 7374 6f6d 6572 2e69 7361 6e6e 6f69 7473  stomer.isannoits
-0000fa40: 696a 6129 207b 5c72 5c6e 5c74 5c74 7265  ija) {\r\n\t\tre
-0000fa50: 7475 726e 2073 6572 7669 6365 5365 6c65  turn serviceSele
-0000fa60: 6374 6f72 436f 6d62 696e 654e 6f6e 426c  ctorCombineNonBl
-0000fa70: 616e 6b73 285b 6375 7374 6f6d 6572 2e69  anks([customer.i
-0000fa80: 7361 6e6e 6f69 7473 696a 612e 6e61 6d65  sannoitsija.name
-0000fa90: 2c0a 2020 2020 2020 2020 6375 7374 6f6d  ,.        custom
-0000faa0: 6572 2e69 7361 6e6e 6f69 7473 696a 612e  er.isannoitsija.
-0000fab0: 7374 7265 6574 2c20 6375 7374 6f6d 6572  street, customer
-0000fac0: 2e69 7361 6e6e 6f69 7473 696a 612e 706f  .isannoitsija.po
-0000fad0: 7374 5d2c 2027 2c20 2729 5c72 5c6e 5c74  st], ', ')\r\n\t
-0000fae0: 7d20 656c 7365 0a20 2020 2020 2020 207b  } else.        {
-0000faf0: 5c72 5c6e 5c74 5c74 7265 7475 726e 2073  \r\n\t\treturn s
-0000fb00: 6572 7669 6365 5365 6c65 6374 6f72 436f  erviceSelectorCo
-0000fb10: 6d62 696e 654e 6f6e 426c 616e 6b73 285b  mbineNonBlanks([
-0000fb20: 6375 7374 6f6d 6572 2e6c 6173 6b75 7475  customer.laskutu
-0000fb30: 736e 696d 692c 2063 7573 746f 6d65 722e  snimi, customer.
-0000fb40: 6c61 736b 7574 7573 7968 7465 7973 6865  laskutusyhteyshe
-0000fb50: 6e6b 2c0a 2020 2020 2020 2020 6375 7374  nk,.        cust
-0000fb60: 6f6d 6572 2e6c 6173 6b75 7475 736b 6174  omer.laskutuskat
-0000fb70: 752c 2063 7573 746f 6d65 722e 6c61 736b  u, customer.lask
-0000fb80: 7574 7573 706f 7374 692c 2063 7573 746f  utusposti, custo
-0000fb90: 6d65 722e 6c61 736b 7574 7573 6d61 615d  mer.laskutusmaa]
-0000fba0: 2c20 272c 2027 290a 2020 2020 2020 2020  , ', ').        
-0000fbb0: 5c72 5c6e 5c74 7d5c 725c 6e7d 5c72 5c6e  \r\n\t}\r\n}\r\n
-0000fbc0: 5c72 5c6e 3c2f 7363 7269 7074 3e5c 725c  \r\n</script>\r\
-0000fbd0: 6e5c 725c 6e3c 7363 7269 7074 2069 643d  n\r\n<script id=
-0000fbe0: 5c22 7365 7276 6963 652d 7365 6c65 6374  \"service-select
-0000fbf0: 6f72 2d76 616c 7565 2d74 656d 706c 6174  or-value-templat
-0000fc00: 655c 220a 2020 2020 2020 2020 7479 7065  e\".        type
-0000fc10: 3d5c 2274 6578 742f 782d 6b65 6e64 6f2d  =\"text/x-kendo-
-0000fc20: 7465 6d70 6c61 7465 5c22 3e5c 725c 6e5c  template\">\r\n\
-0000fc30: 7423 2069 6628 7479 7065 6f66 2063 7573  t# if(typeof cus
-0000fc40: 746f 6d65 7273 2021 3d3d 2027 756e 6465  tomers !== 'unde
-0000fc50: 6669 6e65 6427 290a 2020 2020 2020 2020  fined').        
-0000fc60: 7b20 235c 725c 6e5c 745c 743c 6469 7620  { #\r\n\t\t<div 
-0000fc70: 636c 6173 733d 5c22 7365 7276 6963 652d  class=\"service-
-0000fc80: 6e61 6d65 5c22 3e23 3a20 436f 6d6d 6f6e  name\">#: Common
-0000fc90: 2e66 6f72 6d61 744e 756c 6c41 7345 6d70  .formatNullAsEmp
-0000fca0: 7479 2863 7573 746f 6d65 7273 5b30 5d2e  ty(customers[0].
-0000fcb0: 6e69 6d69 290a 2020 2020 2020 2020 2323  nimi).        ##
-0000fcc0: 3a20 6375 7374 6f6d 6572 735b 305d 2e79  : customers[0].y
-0000fcd0: 6874 6579 7368 656e 6b20 213d 3d20 6e75  hteyshenk !== nu
-0000fce0: 6c6c 2026 2620 6375 7374 6f6d 6572 735b  ll && customers[
-0000fcf0: 305d 2e79 6874 6579 7368 656e 6b20 213d  0].yhteyshenk !=
-0000fd00: 3d20 2727 2026 260a 2020 2020 2020 2020  = '' &&.        
-0000fd10: 6375 7374 6f6d 6572 735b 305d 2e79 6874  customers[0].yht
-0000fd20: 6579 7368 656e 6b20 213d 3d20 6375 7374  eyshenk !== cust
-0000fd30: 6f6d 6572 735b 305d 2e6e 696d 6920 3f20  omers[0].nimi ? 
-0000fd40: 272c 2027 202b 2063 7573 746f 6d65 7273  ', ' + customers
-0000fd50: 5b30 5d2e 7968 7465 7973 6865 6e6b 0a20  [0].yhteyshenk. 
-0000fd60: 2020 2020 2020 203a 2027 2720 233c 2f64         : '' #</d
-0000fd70: 6976 3e5c 725c 6e5c 745c 743c 6469 7620  iv>\r\n\t\t<div 
-0000fd80: 636c 6173 733d 5c22 7365 7276 6963 652d  class=\"service-
-0000fd90: 6164 6472 6573 735c 223e 233a 2073 6572  address\">#: ser
-0000fda0: 7669 6365 5365 6c65 6374 6f72 436f 6d62  viceSelectorComb
-0000fdb0: 696e 654e 6f6e 426c 616e 6b73 285b 6375  ineNonBlanks([cu
-0000fdc0: 7374 6f6d 6572 735b 305d 2e6b 6174 752c  stomers[0].katu,
-0000fdd0: 0a20 2020 2020 2020 2063 7573 746f 6d65  .        custome
-0000fde0: 7273 5b30 5d2e 706f 7374 695d 2c20 272c  rs[0].posti], ',
-0000fdf0: 2027 2920 233c 2f64 6976 3e5c 725c 6e5c   ') #</div>\r\n\
-0000fe00: 745c 745c 725c 6e5c 725c 6e5c 745c 745c  t\t\r\n\r\n\t\t\
-0000fe10: 725c 6e5c 7423 207d 2065 6c73 6520 7b20  r\n\t# } else { 
-0000fe20: 235c 725c 6e5c 745c 743c 6469 760a 2020  #\r\n\t\t<div.  
-0000fe30: 2020 2020 2020 636c 6173 733d 5c22 7365        class=\"se
-0000fe40: 7276 6963 652d 6e61 6d65 5c22 3e56 616c  rvice-name\">Val
-0000fe50: 6974 7365 206b 6f68 6465 3c2f 6469 763e  itse kohde</div>
-0000fe60: 5c72 5c6e 5c74 2320 7d20 235c 725c 6e3c  \r\n\t# } #\r\n<
-0000fe70: 2f73 6372 6970 743e 5c72 5c6e 5c72 5c6e  /script>\r\n\r\n
-0000fe80: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
-0000fe90: 6964 3d5c 2273 6572 7669 6365 2d73 656c  id=\"service-sel
-0000fea0: 6563 746f 722d 7465 6d70 6c61 7465 5c22  ector-template\"
-0000feb0: 2074 7970 653d 5c22 7465 7874 2f78 2d6b   type=\"text/x-k
-0000fec0: 656e 646f 2d74 656d 706c 6174 655c 223e  endo-template\">
-0000fed0: 2320 6966 2874 7970 656f 660a 2020 2020  # if(typeof.    
-0000fee0: 2020 2020 6375 7374 6f6d 6572 7320 213d      customers !=
-0000fef0: 3d20 2775 6e64 6566 696e 6564 2729 207b  = 'undefined') {
-0000ff00: 2023 5c72 5c6e 5c74 3c64 6976 2063 6c61   #\r\n\t<div cla
-0000ff10: 7373 3d5c 2273 6572 7669 6365 2d6e 616d  ss=\"service-nam
-0000ff20: 655c 223e 233a 2043 6f6d 6d6f 6e2e 666f  e\">#: Common.fo
-0000ff30: 726d 6174 4e75 6c6c 4173 456d 7074 7928  rmatNullAsEmpty(
-0000ff40: 6375 7374 6f6d 6572 735b 305d 2e6e 696d  customers[0].nim
-0000ff50: 6929 0a20 2020 2020 2020 2023 233a 2063  i).        ##: c
-0000ff60: 7573 746f 6d65 7273 5b30 5d2e 7968 7465  ustomers[0].yhte
-0000ff70: 7973 6865 6e6b 2021 3d3d 206e 756c 6c20  yshenk !== null 
-0000ff80: 2626 2063 7573 746f 6d65 7273 5b30 5d2e  && customers[0].
-0000ff90: 7968 7465 7973 6865 6e6b 2021 3d3d 2027  yhteyshenk !== '
-0000ffa0: 2720 2626 0a20 2020 2020 2020 2063 7573  ' &&.        cus
-0000ffb0: 746f 6d65 7273 5b30 5d2e 7968 7465 7973  tomers[0].yhteys
-0000ffc0: 6865 6e6b 2021 3d3d 2063 7573 746f 6d65  henk !== custome
-0000ffd0: 7273 5b30 5d2e 6e69 6d69 203f 2027 2c20  rs[0].nimi ? ', 
-0000ffe0: 2720 2b20 6375 7374 6f6d 6572 735b 305d  ' + customers[0]
-0000fff0: 2e79 6874 6579 7368 656e 6b0a 2020 2020  .yhteyshenk.    
-00010000: 2020 2020 3a20 2727 2023 3c2f 6469 763e      : '' #</div>
-00010010: 5c72 5c6e 5c74 3c64 6976 2063 6c61 7373  \r\n\t<div class
-00010020: 3d5c 2273 6572 7669 6365 2d61 6464 7265  =\"service-addre
-00010030: 7373 5c22 3e23 3a20 7365 7276 6963 6553  ss\">#: serviceS
-00010040: 656c 6563 746f 7243 6f6d 6269 6e65 4e6f  electorCombineNo
-00010050: 6e42 6c61 6e6b 7328 5b63 7573 746f 6d65  nBlanks([custome
-00010060: 7273 5b30 5d2e 6b61 7475 2c0a 2020 2020  rs[0].katu,.    
-00010070: 2020 2020 6375 7374 6f6d 6572 735b 305d      customers[0]
-00010080: 2e70 6f73 7469 5d2c 2027 2c20 2729 2023  .posti], ', ') #
-00010090: 3c2f 6469 763e 5c72 5c6e 5c74 5c72 5c6e  </div>\r\n\t\r\n
-000100a0: 5c72 5c6e 5c74 5c72 5c6e 2320 7d20 233c  \r\n\t\r\n# } #<
-000100b0: 2f73 6372 6970 743e 5c72 5c6e 5c72 5c6e  /script>\r\n\r\n
-000100c0: 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e  \r\n\r\n\r\n\r\n
-000100d0: 3c74 6578 7461 7265 610a 2020 2020 2020  <textarea.      
-000100e0: 2020 6964 3d5c 2274 7970 655f 6469 7368    id=\"type_dish
-000100f0: 315c 2220 7374 796c 653d 5c22 6469 7370  1\" style=\"disp
-00010100: 6c61 793a 6e6f 6e65 3b5c 223e 5c72 5c6e  lay:none;\">\r\n
-00010110: 5c74 3c64 6976 2063 6c61 7373 3d5c 2264  \t<div class=\"d
-00010120: 6973 6831 2070 726f 6475 6374 5c22 3e5c  ish1 product\">\
-00010130: 725c 6e5c 745c 743c 6469 760a 2020 2020  r\n\t\t<div.    
-00010140: 2020 2020 636c 6173 733d 5c22 636f 6e74      class=\"cont
-00010150: 6169 6e65 722d 666c 7569 645c 223e 5c72  ainer-fluid\">\r
-00010160: 5c6e 5c74 5c74 5c74 3c64 6976 2063 6c61  \n\t\t\t<div cla
-00010170: 7373 3d5c 2272 6f77 206e 6172 726f 772d  ss=\"row narrow-
-00010180: 6761 7073 5c22 3e5c 725c 6e5c 745c 745c  gaps\">\r\n\t\t\
-00010190: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
-000101a0: 636c 6173 733d 5c22 636f 6c2d 6d64 2d33  class=\"col-md-3
-000101b0: 2074 6578 742d 6365 6e74 6572 2d78 735c   text-center-xs\
-000101c0: 223e 7b63 6f6d 6d6f 6e2e 696d 6167 6545  ">{common.imageE
-000101d0: 6c65 6d65 6e74 2829 7d3c 2f64 6976 3e5c  lement()}</div>\
-000101e0: 725c 6e5c 745c 745c 745c 743c 6469 760a  r\n\t\t\t\t<div.
-000101f0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-00010200: 636f 6c2d 6d64 2d36 5c22 3e5c 725c 6e5c  col-md-6\">\r\n\
-00010210: 745c 745c 745c 745c 743c 6834 2063 6c61  t\t\t\t\t<h4 cla
-00010220: 7373 3d5c 2274 6578 742d 6365 6e74 6572  ss=\"text-center
-00010230: 2d78 7320 7072 6f64 7563 742d 6e61 6d65  -xs product-name
-00010240: 5c22 3e7b 6f62 6a2e 6e61 6d65 7d3c 2f68  \">{obj.name}</h
-00010250: 343e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  4>\r\n\t\t\t\t\t
-00010260: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
-00010270: 7373 3d5c 2264 6573 6372 6970 7469 6f6e  ss=\"description
-00010280: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
-00010290: 745c 747b 6f62 6a2e 6465 7363 7d5c 725c  t\t{obj.desc}\r\
-000102a0: 6e5c 745c 745c 745c 745c 745c 747b 6f62  n\t\t\t\t\t\t{ob
-000102b0: 6a2e 7765 6967 6874 4261 7365 640a 2020  j.weightBased.  
-000102c0: 2020 2020 2020 3d3d 2031 3f3c 6272 3e4b        == 1?<br>K
-000102d0: 5c78 4534 7369 7474 656c 796d 616b 7375  \xE4sittelymaksu
-000102e0: 2070 6169 6e6f 6e20 6d75 6b61 6973 6573   painon mukaises
-000102f0: 7469 3a7d 5c72 5c6e 5c74 5c74 5c74 5c74  ti:}\r\n\t\t\t\t
-00010300: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
-00010310: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-00010320: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
-00010330: 2020 2063 6c61 7373 3d5c 2263 6f6c 2d6d     class=\"col-m
-00010340: 642d 335c 223e 5c72 5c6e 5c74 5c74 5c74  d-3\">\r\n\t\t\t
-00010350: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 5c74  \t\t\r\n\t\t\t\t
-00010360: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
-00010370: 2272 6f77 5c22 207b 636f 6d6d 6f6e 2e64  "row\" {common.d
-00010380: 6973 706c 6179 5072 6963 6528 297d 3e5c  isplayPrice()}>\
-00010390: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
-000103a0: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
-000103b0: 6173 733d 5c22 636f 6c2d 6d64 2d34 2063  ass=\"col-md-4 c
-000103c0: 6f6c 2d78 732d 345c 223e 5c72 5c6e 5c74  ol-xs-4\">\r\n\t
-000103d0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c6c  \t\t\t\t\t\t\t<l
-000103e0: 6162 656c 2063 6c61 7373 3d5c 2263 6f6e  abel class=\"con
-000103f0: 7472 6f6c 2d6c 6162 656c 5c22 3e48 696e  trol-label\">Hin
-00010400: 7461 3c2f 6c61 6265 6c3e 5c72 5c6e 5c74  ta</label>\r\n\t
-00010410: 5c74 5c74 5c74 5c74 5c74 5c74 3c2f 6469  \t\t\t\t\t\t</di
-00010420: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  v>\r\n\t\t\t\t\t
-00010430: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-00010440: 2063 6c61 7373 3d5c 2263 6f6c 2d6d 642d   class=\"col-md-
-00010450: 3820 636f 6c2d 7873 2d38 5c22 3e5c 725c  8 col-xs-8\">\r\
-00010460: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
-00010470: 743c 6469 7620 636c 6173 733d 5c22 7072  t<div class=\"pr
-00010480: 6963 655c 223e 7b63 6f6d 6d6f 6e2e 636f  ice\">{common.co
-00010490: 6d62 696e 6564 5661 7450 7269 6365 2829  mbinedVatPrice()
-000104a0: 7d0a 2020 2020 2020 2020 2665 7572 6f3b  }.        &euro;
-000104b0: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
-000104c0: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
-000104d0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \n\t\t\t\t\t\t</
-000104e0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
-000104f0: 5c74 5c74 7b6f 626a 2e77 6569 6768 7442  \t\t{obj.weightB
-00010500: 6173 6564 0a20 2020 2020 2020 203d 3d20  ased.        == 
-00010510: 313f 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  1?\r\n\t\t\t\t\t
-00010520: 5c74 3c64 6976 2063 6c61 7373 3d5c 2272  \t<div class=\"r
-00010530: 6f77 5c22 207b 636f 6d6d 6f6e 2e64 6973  ow\" {common.dis
-00010540: 706c 6179 5072 6963 6528 297d 3e5c 725c  playPrice()}>\r\
-00010550: 6e5c 745c 745c 745c 745c 745c 745c 743c  n\t\t\t\t\t\t\t<
-00010560: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-00010570: 733d 5c22 636f 6c2d 6d64 2d34 2063 6f6c  s=\"col-md-4 col
-00010580: 2d78 732d 345c 223e 5c72 5c6e 5c74 5c74  -xs-4\">\r\n\t\t
-00010590: 5c74 5c74 5c74 5c74 5c74 5c74 3c6c 6162  \t\t\t\t\t\t<lab
-000105a0: 656c 2063 6c61 7373 3d5c 2263 6f6e 7472  el class=\"contr
-000105b0: 6f6c 2d6c 6162 656c 5c22 3e4b 5c78 4534  ol-label\">K\xE4
-000105c0: 7369 7474 656c 7926 7368 793b 6d61 6b73  sittely&shy;maks
-000105d0: 753c 2f6c 6162 656c 3e5c 725c 6e5c 745c  u</label>\r\n\t\
-000105e0: 745c 745c 745c 745c 745c 743c 2f64 6976  t\t\t\t\t\t</div
-000105f0: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-00010600: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
-00010610: 636c 6173 733d 5c22 636f 6c2d 6d64 2d38  class=\"col-md-8
-00010620: 2063 6f6c 2d78 732d 385c 223e 5c72 5c6e   col-xs-8\">\r\n
-00010630: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-00010640: 3c64 6976 2063 6c61 7373 3d5c 2270 7269  <div class=\"pri
-00010650: 6365 5c22 3e7b 6f62 6a2e 7770 7269 6365  ce\">{obj.wprice
-00010660: 7d0a 2020 2020 2020 2020 2665 7572 6f3b  }.        &euro;
-00010670: 2f74 6e3c 2f64 6976 3e5c 725c 6e5c 745c  /tn</div>\r\n\t\
-00010680: 745c 745c 745c 745c 745c 743c 2f64 6976  t\t\t\t\t\t</div
-00010690: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-000106a0: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
-000106b0: 745c 745c 745c 743a 7d5c 725c 6e5c 745c  t\t\t\t:}\r\n\t\
-000106c0: 745c 745c 745c 745c 725c 6e5c 745c 745c  t\t\t\t\r\n\t\t\
-000106d0: 745c 745c 745c 725c 6e5c 745c 745c 745c  t\t\t\r\n\t\t\t\
-000106e0: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
-000106f0: 636c 6173 733d 5c22 726f 775c 223e 5c72  class=\"row\">\r
-00010700: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c64  \n\t\t\t\t\t\t<d
-00010710: 6976 2063 6c61 7373 3d5c 2263 6f6c 2d6d  iv class=\"col-m
-00010720: 642d 3420 636f 6c2d 7873 2d34 5c22 3e5c  d-4 col-xs-4\">\
-00010730: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
-00010740: 743c 6c61 6265 6c0a 2020 2020 2020 2020  t<label.        
-00010750: 636c 6173 733d 5c22 636f 6e74 726f 6c2d  class=\"control-
-00010760: 6c61 6265 6c5c 223e 4d5c 7845 345c 7845  label\">M\xE4\xE
-00010770: 3472 5c78 4534 3c2f 6c61 6265 6c3e 5c72  4r\xE4</label>\r
-00010780: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \n\t\t\t\t\t\t</
-00010790: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
-000107a0: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-000107b0: 2063 6c61 7373 3d5c 2263 6f6c 2d6d 642d   class=\"col-md-
-000107c0: 3820 636f 6c2d 7873 2d38 5c22 3e5c 725c  8 col-xs-8\">\r\
-000107d0: 6e5c 745c 745c 745c 745c 745c 745c 743c  n\t\t\t\t\t\t\t<
-000107e0: 6469 7620 636c 6173 733d 5c22 616d 6f75  div class=\"amou
-000107f0: 6e74 5c22 3e5c 725c 6e5c 745c 745c 745c  nt\">\r\n\t\t\t\
-00010800: 745c 745c 745c 745c 745c 725c 6e5c 745c  t\t\t\t\t\r\n\t\
-00010810: 745c 745c 745c 745c 745c 745c 745c 725c  t\t\t\t\t\t\t\r\
-00010820: 6e5c 725c 6e5c 745c 745c 745c 745c 745c  n\r\n\t\t\t\t\t\
-00010830: 745c 745c 745c 725c 6e5c 745c 745c 745c  t\t\t\r\n\t\t\t\
-00010840: 745c 745c 745c 745c 745c 743c 7365 6c65  t\t\t\t\t\t<sele
-00010850: 6374 0a20 2020 2020 2020 2069 643d 5c22  ct.        id=\"
-00010860: 616d 6f75 6e74 5f7b 6f62 6a2e 7072 6963  amount_{obj.pric
-00010870: 6569 647d 5c22 2063 6c61 7373 3d5c 2266  eid}\" class=\"f
-00010880: 6f72 6d2d 636f 6e74 726f 6c5c 223e 5c72  orm-control\">\r
-00010890: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-000108a0: 5c74 5c74 5c74 3c6f 7074 696f 6e0a 2020  \t\t\t<option.  
-000108b0: 2020 2020 2020 7661 6c75 653d 5c22 315c        value=\"1\
-000108c0: 223e 313c 2f6f 7074 696f 6e3e 5c72 5c6e  ">1</option>\r\n
-000108d0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-000108e0: 5c74 5c74 3c6f 7074 696f 6e20 7661 6c75  \t\t<option valu
-000108f0: 653d 5c22 325c 223e 323c 2f6f 7074 696f  e=\"2\">2</optio
-00010900: 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  n>\r\n\t\t\t\t\t
-00010910: 5c74 5c74 5c74 5c74 5c74 3c6f 7074 696f  \t\t\t\t\t<optio
-00010920: 6e0a 2020 2020 2020 2020 7661 6c75 653d  n.        value=
-00010930: 5c22 335c 223e 333c 2f6f 7074 696f 6e3e  \"3\">3</option>
-00010940: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-00010950: 5c74 5c74 5c74 5c74 3c6f 7074 696f 6e20  \t\t\t\t<option 
-00010960: 7661 6c75 653d 5c22 345c 223e 343c 2f6f  value=\"4\">4</o
-00010970: 7074 696f 6e3e 5c72 5c6e 5c74 5c74 5c74  ption>\r\n\t\t\t
-00010980: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c6f  \t\t\t\t\t\t\t<o
-00010990: 7074 696f 6e0a 2020 2020 2020 2020 7661  ption.        va
-000109a0: 6c75 653d 5c22 355c 223e 353c 2f6f 7074  lue=\"5\">5</opt
-000109b0: 696f 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74  ion>\r\n\t\t\t\t
-000109c0: 5c74 5c74 5c74 5c74 5c74 5c74 3c6f 7074  \t\t\t\t\t\t<opt
-000109d0: 696f 6e20 7661 6c75 653d 5c22 365c 223e  ion value=\"6\">
-000109e0: 363c 2f6f 7074 696f 6e3e 5c72 5c6e 5c74  6</option>\r\n\t
-000109f0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-00010a00: 5c74 3c6f 7074 696f 6e0a 2020 2020 2020  \t<option.      
-00010a10: 2020 7661 6c75 653d 5c22 375c 223e 373c    value=\"7\">7<
-00010a20: 2f6f 7074 696f 6e3e 5c72 5c6e 5c74 5c74  /option>\r\n\t\t
-00010a30: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-00010a40: 3c6f 7074 696f 6e20 7661 6c75 653d 5c22  <option value=\"
-00010a50: 385c 223e 383c 2f6f 7074 696f 6e3e 5c72  8\">8</option>\r
-00010a60: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-00010a70: 5c74 5c74 5c74 3c6f 7074 696f 6e0a 2020  \t\t\t<option.  
-00010a80: 2020 2020 2020 7661 6c75 653d 5c22 395c        value=\"9\
-00010a90: 223e 393c 2f6f 7074 696f 6e3e 5c72 5c6e  ">9</option>\r\n
-00010aa0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-00010ab0: 5c74 5c74 3c6f 7074 696f 6e20 7661 6c75  \t\t<option valu
-00010ac0: 653d 5c22 3130 5c22 3e31 303c 2f6f 7074  e=\"10\">10</opt
-00010ad0: 696f 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74  ion>\r\n\t\t\t\t
-00010ae0: 5c74 5c74 5c74 5c74 5c74 3c2f 7365 6c65  \t\t\t\t\t</sele
-00010af0: 6374 3e5c 725c 6e5c 745c 745c 745c 745c  ct>\r\n\t\t\t\t\
-00010b00: 745c 745c 745c 745c 725c 6e5c 745c 745c  t\t\t\t\r\n\t\t\
-00010b10: 745c 745c 745c 745c 745c 745c 725c 6e5c  t\t\t\t\t\t\r\n\
-00010b20: 745c 745c 745c 745c 745c 745c 743c 2f64  t\t\t\t\t\t\t</d
-00010b30: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
-00010b40: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
-00010b50: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
-00010b60: 6e5c 745c 745c 745c 745c 743c 6469 760a  n\t\t\t\t\t<div.
-00010b70: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-00010b80: 726f 775c 223e 5c72 5c6e 5c74 5c74 5c74  row\">\r\n\t\t\t
-00010b90: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
-00010ba0: 3d5c 2263 6f6c 2d6d 642d 3820 636f 6c2d  =\"col-md-8 col-
-00010bb0: 6d64 2d6f 6666 7365 742d 3420 636f 6c2d  md-offset-4 col-
-00010bc0: 7873 2d38 0a20 2020 2020 2020 2063 6f6c  xs-8.        col
-00010bd0: 2d78 732d 6f66 6673 6574 2d34 5c22 3e5c  -xs-offset-4\">\
-00010be0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
-00010bf0: 745c 725c 6e5c 745c 745c 745c 745c 745c  t\r\n\t\t\t\t\t\
-00010c00: 745c 745c 743c 6275 7474 6f6e 2063 6c61  t\t\t<button cla
-00010c10: 7373 3d5c 2262 746e 0a20 2020 2020 2020  ss=\"btn.       
-00010c20: 2062 746e 2d64 6566 6175 6c74 2062 746e   btn-default btn
-00010c30: 2d62 6c6f 636b 206c 6f6e 672d 7465 7874  -block long-text
-00010c40: 2d62 7574 746f 6e5c 2220 6f6e 636c 6963  -button\" onclic
-00010c50: 6b3d 5c22 7368 6f70 7069 6e67 4361 7274  k=\"shoppingCart
-00010c60: 2e61 6464 5072 6f64 7563 7428 277b 6f62  .addProduct('{ob
-00010c70: 6a2e 7072 6963 6569 647d 272c 277b 6f62  j.priceid}','{ob
-00010c80: 6a2e 6e61 6d65 7d27 2c24 2827 2361 6d6f  j.name}',$('#amo
-00010c90: 756e 745f 7b6f 626a 2e70 7269 6365 6964  unt_{obj.priceid
-00010ca0: 7d27 292e 7661 6c28 292c 277b 636f 6d6d  }').val(),'{comm
-00010cb0: 6f6e 2e63 6174 6567 6f72 7928 297d 272c  on.category()}',
-00010cc0: 277b 636f 6d6d 6f6e 2e63 6f6d 6269 6e65  '{common.combine
-00010cd0: 6456 6174 5072 6963 6528 297d 2729 5c22  dVatPrice()}')\"
-00010ce0: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-00010cf0: 745c 745c 745c 744b 6f72 6969 6e5c 725c  t\t\t\tKoriin\r\
-00010d00: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
-00010d10: 743c 2f62 7574 746f 6e3e 5c72 5c6e 5c74  t</button>\r\n\t
-00010d20: 5c74 5c74 5c74 5c74 5c74 5c74 5c72 5c6e  \t\t\t\t\t\t\r\n
-00010d30: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c72  \t\t\t\t\t\t\t\r
-00010d40: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \n\t\t\t\t\t\t</
-00010d50: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
-00010d60: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
-00010d70: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-00010d80: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-00010d90: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 3c2f  \t</div>\r\n\t</
-00010da0: 6469 763e 5c72 5c6e 3c2f 7465 7874 6172  div>\r\n</textar
-00010db0: 6561 3e5c 745c 725c 6e5c 725c 6e5c 725c  ea>\t\r\n\r\n\r\
-00010dc0: 6e5c 725c 6e3c 6469 760a 2020 2020 2020  n\r\n<div.      
-00010dd0: 2020 6964 3d5c 2276 6964 656f 2d70 6f70    id=\"video-pop
-00010de0: 7570 2d6d 6f64 616c 5c22 2063 6c61 7373  up-modal\" class
-00010df0: 3d5c 226d 6f64 616c 5c22 2073 7479 6c65  =\"modal\" style
-00010e00: 3d5c 2264 6973 706c 6179 3a6e 6f6e 655c  =\"display:none\
-00010e10: 223e 5c72 5c6e 5c74 3c64 6976 0a20 2020  ">\r\n\t<div.   
-00010e20: 2020 2020 2063 6c61 7373 3d5c 226d 6f64       class=\"mod
-00010e30: 616c 2d64 6961 6c6f 6720 6d6f 6461 6c2d  al-dialog modal-
-00010e40: 6c67 5c22 3e5c 725c 6e5c 745c 743c 6469  lg\">\r\n\t\t<di
-00010e50: 7620 636c 6173 733d 5c22 6d6f 6461 6c2d  v class=\"modal-
-00010e60: 636f 6e74 656e 745c 223e 5c72 5c6e 5c74  content\">\r\n\t
-00010e70: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-00010e80: 2063 6c61 7373 3d5c 226d 6f64 616c 2d62   class=\"modal-b
-00010e90: 6f64 795c 223e 5c72 5c6e 5c74 5c74 5c74  ody\">\r\n\t\t\t
-00010ea0: 5c74 3c64 6976 2063 6c61 7373 3d5c 2265  \t<div class=\"e
-00010eb0: 6d62 6564 2d72 6573 706f 6e73 6976 6520  mbed-responsive 
-00010ec0: 656d 6265 642d 7265 7370 6f6e 7369 7665  embed-responsive
-00010ed0: 2d34 6279 335c 223e 5c72 5c6e 5c74 5c74  -4by3\">\r\n\t\t
-00010ee0: 5c74 5c74 5c74 3c76 6964 656f 0a20 2020  \t\t\t<video.   
-00010ef0: 2020 2020 2063 6f6e 7472 6f6c 733e 5c72       controls>\r
-00010f00: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5365  \n\t\t\t\t\t\tSe
-00010f10: 6c61 696d 6573 6920 6569 2074 7565 2048  laimesi ei tue H
-00010f20: 544d 4c35 2d76 6964 656f 612e 203c 6120  TML5-videoa. <a 
-00010f30: 6872 6566 3d5c 2223 5c22 2064 6174 612d  href=\"#\" data-
-00010f40: 726f 6c65 3d5c 2264 6f77 6e6c 6f61 645c  role=\"download\
-00010f50: 223e 4c61 7461 610a 2020 2020 2020 2020  ">Lataa.        
-00010f60: 7669 6465 6f2e 3c2f 613e 5c72 5c6e 5c74  video.</a>\r\n\t
-00010f70: 5c74 5c74 5c74 5c74 3c2f 7669 6465 6f3e  \t\t\t\t</video>
-00010f80: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c69  \r\n\t\t\t\t\t<i
-00010f90: 6672 616d 6520 6672 616d 6562 6f72 6465  frame frameborde
-00010fa0: 723d 5c22 305c 2220 7765 626b 6974 616c  r=\"0\" webkital
-00010fb0: 6c6f 7766 756c 6c73 6372 6565 6e0a 2020  lowfullscreen.  
-00010fc0: 2020 2020 2020 6d6f 7a61 6c6c 6f77 6675        mozallowfu
-00010fd0: 6c6c 7363 7265 656e 2061 6c6c 6f77 6675  llscreen allowfu
-00010fe0: 6c6c 7363 7265 656e 3e3c 2f69 6672 616d  llscreen></ifram
-00010ff0: 653e 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f  e>\r\n\t\t\t\t</
-00011000: 6469 763e 5c72 5c6e 5c72 5c6e 5c74 5c74  div>\r\n\r\n\t\t
-00011010: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-00011020: 2063 6c61 7373 3d5c 2266 6f72 6d2d 6275   class=\"form-bu
-00011030: 7474 6f6e 7320 7465 7874 2d63 656e 7465  ttons text-cente
-00011040: 725c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  r\">\r\n\t\t\t\t
-00011050: 5c74 3c62 7574 746f 6e20 636c 6173 733d  \t<button class=
-00011060: 5c22 6274 6e20 6274 6e2d 7072 696d 6172  \"btn btn-primar
-00011070: 795c 220a 2020 2020 2020 2020 6461 7461  y\".        data
-00011080: 2d64 6973 6d69 7373 3d5c 226d 6f64 616c  -dismiss=\"modal
-00011090: 5c22 3e53 756c 6a65 3c2f 6275 7474 6f6e  \">Sulje</button
-000110a0: 3e5c 725c 6e5c 745c 745c 745c 743c 2f64  >\r\n\t\t\t\t</d
-000110b0: 6976 3e5c 725c 6e5c 745c 745c 743c 2f64  iv>\r\n\t\t\t</d
-000110c0: 6976 3e5c 725c 6e5c 745c 743c 2f64 6976  iv>\r\n\t\t</div
-000110d0: 3e5c 725c 6e5c 743c 2f64 6976 3e5c 725c  >\r\n\t</div>\r\
-000110e0: 6e3c 2f64 6976 3e5c 725c 6e5c 725c 6e5c  n</div>\r\n\r\n\
-000110f0: 725c 6e3c 6469 760a 2020 2020 2020 2020  r\n<div.        
-00011100: 6964 3d5c 2261 6c65 7274 2d6d 6f64 616c  id=\"alert-modal
-00011110: 5c22 2063 6c61 7373 3d5c 226d 6f64 616c  \" class=\"modal
-00011120: 5c22 2073 7479 6c65 3d5c 2264 6973 706c  \" style=\"displ
-00011130: 6179 3a6e 6f6e 655c 223e 5c72 5c6e 5c74  ay:none\">\r\n\t
-00011140: 3c64 6976 2063 6c61 7373 3d5c 226d 6f64  <div class=\"mod
-00011150: 616c 2d64 6961 6c6f 670a 2020 2020 2020  al-dialog.      
-00011160: 2020 6d6f 6461 6c2d 736d 5c22 3e5c 725c    modal-sm\">\r\
-00011170: 6e5c 745c 743c 6469 7620 636c 6173 733d  n\t\t<div class=
-00011180: 5c22 6d6f 6461 6c2d 636f 6e74 656e 745c  \"modal-content\
-00011190: 223e 5c72 5c6e 5c74 5c74 5c74 3c64 6976  ">\r\n\t\t\t<div
-000111a0: 2063 6c61 7373 3d5c 226d 6f64 616c 2d62   class=\"modal-b
-000111b0: 6f64 795c 223e 5c72 5c6e 5c74 5c74 5c74  ody\">\r\n\t\t\t
-000111c0: 5c74 3c64 6976 0a20 2020 2020 2020 2064  \t<div.        d
-000111d0: 6174 612d 726f 6c65 3d5c 2274 6578 745c  ata-role=\"text\
-000111e0: 223e 3c2f 6469 763e 5c72 5c6e 5c74 5c74  "></div>\r\n\t\t
-000111f0: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
-00011200: 5c74 3c64 6976 2063 6c61 7373 3d5c 226d  \t<div class=\"m
-00011210: 6f64 616c 2d66 6f6f 7465 725c 223e 5c72  odal-footer\">\r
-00011220: 5c6e 5c74 5c74 5c74 5c74 3c64 6976 0a20  \n\t\t\t\t<div. 
-00011230: 2020 2020 2020 2063 6c61 7373 3d5c 2274         class=\"t
-00011240: 6578 742d 7269 6768 745c 223e 5c72 5c6e  ext-right\">\r\n
-00011250: 5c74 5c74 5c74 5c74 5c74 3c62 7574 746f  \t\t\t\t\t<butto
-00011260: 6e20 636c 6173 733d 5c22 6274 6e20 6274  n class=\"btn bt
-00011270: 6e2d 7072 696d 6172 795c 2220 6461 7461  n-primary\" data
-00011280: 2d61 6374 696f 6e3d 5c22 6f6b 5c22 0a20  -action=\"ok\". 
-00011290: 2020 2020 2020 2064 6174 612d 6469 736d         data-dism
-000112a0: 6973 733d 5c22 6d6f 6461 6c5c 223e 3c2f  iss=\"modal\"></
-000112b0: 6275 7474 6f6e 3e5c 725c 6e5c 745c 745c  button>\r\n\t\t\
-000112c0: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
-000112d0: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
-000112e0: 743c 2f64 6976 3e5c 725c 6e5c 743c 2f64  t</div>\r\n\t</d
-000112f0: 6976 3e5c 725c 6e3c 2f64 6976 3e5c 725c  iv>\r\n</div>\r\
-00011300: 6e5c 725c 6e3c 6469 760a 2020 2020 2020  n\r\n<div.      
-00011310: 2020 6964 3d5c 2263 6f6e 6669 726d 2d6d    id=\"confirm-m
-00011320: 6f64 616c 5c22 2063 6c61 7373 3d5c 226d  odal\" class=\"m
-00011330: 6f64 616c 5c22 2073 7479 6c65 3d5c 2264  odal\" style=\"d
-00011340: 6973 706c 6179 3a6e 6f6e 655c 223e 5c72  isplay:none\">\r
-00011350: 5c6e 5c74 3c64 6976 2063 6c61 7373 3d5c  \n\t<div class=\
-00011360: 226d 6f64 616c 2d64 6961 6c6f 670a 2020  "modal-dialog.  
-00011370: 2020 2020 2020 6d6f 6461 6c2d 736d 5c22        modal-sm\"
-00011380: 3e5c 725c 6e5c 745c 743c 6469 7620 636c  >\r\n\t\t<div cl
-00011390: 6173 733d 5c22 6d6f 6461 6c2d 636f 6e74  ass=\"modal-cont
-000113a0: 656e 745c 223e 5c72 5c6e 5c74 5c74 5c74  ent\">\r\n\t\t\t
-000113b0: 3c64 6976 2063 6c61 7373 3d5c 226d 6f64  <div class=\"mod
-000113c0: 616c 2d62 6f64 795c 223e 5c72 5c6e 5c74  al-body\">\r\n\t
-000113d0: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
-000113e0: 2020 2064 6174 612d 726f 6c65 3d5c 2274     data-role=\"t
-000113f0: 6578 745c 223e 3c2f 6469 763e 5c72 5c6e  ext\"></div>\r\n
-00011400: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
-00011410: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
-00011420: 3d5c 226d 6f64 616c 2d66 6f6f 7465 725c  =\"modal-footer\
-00011430: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 3c64  ">\r\n\t\t\t\t<d
-00011440: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
-00011450: 3d5c 2274 6578 742d 7269 6768 745c 223e  =\"text-right\">
-00011460: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c62  \r\n\t\t\t\t\t<b
-00011470: 7574 746f 6e20 636c 6173 733d 5c22 6274  utton class=\"bt
-00011480: 6e20 6274 6e2d 7072 696d 6172 795c 2220  n btn-primary\" 
-00011490: 6461 7461 2d61 6374 696f 6e3d 5c22 6f6b  data-action=\"ok
-000114a0: 5c22 3e3c 2f62 7574 746f 6e3e 5c72 5c6e  \"></button>\r\n
-000114b0: 5c74 5c74 5c74 5c74 5c74 3c62 7574 746f  \t\t\t\t\t<butto
-000114c0: 6e0a 2020 2020 2020 2020 636c 6173 733d  n.        class=
-000114d0: 5c22 6274 6e20 6274 6e2d 6465 6661 756c  \"btn btn-defaul
-000114e0: 745c 2220 6461 7461 2d61 6374 696f 6e3d  t\" data-action=
-000114f0: 5c22 6361 6e63 656c 5c22 3e3c 2f62 7574  \"cancel\"></but
-00011500: 746f 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74  ton>\r\n\t\t\t\t
-00011510: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
-00011520: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 3c2f  </div>\r\n\t\t</
-00011530: 6469 763e 5c72 5c6e 5c74 3c2f 6469 763e  div>\r\n\t</div>
-00011540: 5c72 5c6e 3c2f 6469 763e 5c72 5c6e 5c72  \r\n</div>\r\n\r
-00011550: 5c6e 3c73 6372 6970 743e 5c72 5c6e 5c72  \n<script>\r\n\r
-00011560: 5c6e 6675 6e63 7469 6f6e 0a20 2020 2020  \nfunction.     
-00011570: 2020 2073 686f 7741 6c65 7274 2874 7970     showAlert(typ
-00011580: 652c 2074 6578 742c 206f 6b54 6578 7429  e, text, okText)
-00011590: 207b 5c72 5c6e 2020 2020 7661 7220 246d   {\r\n    var $m
-000115a0: 6f64 616c 203d 2024 2827 2361 6c65 7274  odal = $('#alert
-000115b0: 2d6d 6f64 616c 2729 3b5c 725c 6e0a 2020  -modal');\r\n.  
-000115c0: 2020 2020 2020 5c20 2020 7661 7220 6465        \   var de
-000115d0: 6665 7272 6564 203d 206e 6577 2024 2e44  ferred = new $.D
-000115e0: 6566 6572 7265 6428 293b 5c72 5c6e 5c72  eferred();\r\n\r
-000115f0: 5c6e 2020 2020 246d 6f64 616c 2e66 696e  \n    $modal.fin
-00011600: 6428 275b 6461 7461 2d72 6f6c 653d 5c22  d('[data-role=\"
-00011610: 7465 7874 5c22 5d27 292e 6874 6d6c 2874  text\"]').html(t
-00011620: 6578 7429 3b5c 725c 6e0a 2020 2020 2020  ext);\r\n.      
-00011630: 2020 5c20 2020 6966 2874 7970 656f 6620    \   if(typeof 
-00011640: 6f6b 5465 7874 203d 3d3d 2027 756e 6465  okText === 'unde
-00011650: 6669 6e65 6427 2920 7b5c 725c 6e20 2020  fined') {\r\n   
-00011660: 2020 2020 206f 6b54 6578 7420 3d20 274f       okText = 'O
-00011670: 6b27 3b5c 725c 6e20 2020 207d 5c72 5c6e  k';\r\n    }\r\n
-00011680: 0a20 2020 2020 2020 205c 2020 2024 6d6f  .        \   $mo
-00011690: 6461 6c2e 6669 6e64 2827 5b64 6174 612d  dal.find('[data-
-000116a0: 6163 7469 6f6e 3d5c 226f 6b5c 225d 2729  action=\"ok\"]')
-000116b0: 2e68 746d 6c28 6f6b 5465 7874 293b 5c72  .html(okText);\r
-000116c0: 5c6e 5c72 5c6e 2020 2020 246d 6f64 616c  \n\r\n    $modal
-000116d0: 2e6d 6f64 616c 2827 7368 6f77 2729 3b5c  .modal('show');\
-000116e0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-000116f0: 246d 6f64 616c 2e6f 6e28 2768 6964 6465  $modal.on('hidde
-00011700: 6e2e 6273 2e6d 6f64 616c 272c 2066 756e  n.bs.modal', fun
-00011710: 6374 696f 6e28 6529 207b 5c72 5c6e 2020  ction(e) {\r\n  
-00011720: 2020 2020 2020 6465 6665 7272 6564 2e72        deferred.r
-00011730: 6573 6f6c 7665 2829 3b5c 725c 6e0a 2020  esolve();\r\n.  
-00011740: 2020 2020 2020 5c20 2020 7d29 3b5c 725c        \   });\r\
-00011750: 6e20 2020 2072 6574 7572 6e20 6465 6665  n    return defe
-00011760: 7272 6564 3b5c 725c 6e7d 5c72 5c6e 5c72  rred;\r\n}\r\n\r
-00011770: 5c6e 6675 6e63 7469 6f6e 2073 686f 7743  \nfunction showC
-00011780: 6f6e 6669 726d 2874 7970 652c 2074 6578  onfirm(type, tex
-00011790: 742c 0a20 2020 2020 2020 206f 6b54 6578  t,.        okTex
-000117a0: 742c 2063 616e 6365 6c54 6578 7429 207b  t, cancelText) {
-000117b0: 5c72 5c6e 2020 2020 7661 7220 246d 6f64  \r\n    var $mod
-000117c0: 616c 203d 2024 2827 2363 6f6e 6669 726d  al = $('#confirm
-000117d0: 2d6d 6f64 616c 2729 3b5c 725c 6e20 2020  -modal');\r\n   
-000117e0: 2076 6172 0a20 2020 2020 2020 2064 6566   var.        def
-000117f0: 6572 7265 6420 3d20 6e65 7720 242e 4465  erred = new $.De
-00011800: 6665 7272 6564 2829 3b5c 725c 6e5c 725c  ferred();\r\n\r\
-00011810: 6e20 2020 2024 6d6f 6461 6c2e 6669 6e64  n    $modal.find
-00011820: 2827 5b64 6174 612d 726f 6c65 3d5c 2274  ('[data-role=\"t
-00011830: 6578 745c 225d 2729 2e68 746d 6c28 7465  ext\"]').html(te
-00011840: 7874 293b 5c72 5c6e 0a20 2020 2020 2020  xt);\r\n.       
-00011850: 205c 2020 2069 6628 7479 7065 6f66 206f   \   if(typeof o
-00011860: 6b54 6578 7420 3d3d 3d20 2775 6e64 6566  kText === 'undef
-00011870: 696e 6564 2729 207b 5c72 5c6e 2020 2020  ined') {\r\n    
-00011880: 2020 2020 6f6b 5465 7874 203d 205c 224f      okText = \"O
-00011890: 6b5c 223b 5c72 5c6e 2020 2020 7d5c 725c  k\";\r\n    }\r\
-000118a0: 6e0a 2020 2020 2020 2020 5c20 2020 246d  n.        \   $m
-000118b0: 6f64 616c 2e66 696e 6428 275b 6461 7461  odal.find('[data
-000118c0: 2d61 6374 696f 6e3d 5c22 6f6b 5c22 5d27  -action=\"ok\"]'
-000118d0: 292e 6874 6d6c 286f 6b54 6578 7429 3b5c  ).html(okText);\
-000118e0: 725c 6e20 2020 2069 6628 7479 7065 6f66  r\n    if(typeof
-000118f0: 2063 616e 6365 6c54 6578 740a 2020 2020   cancelText.    
-00011900: 2020 2020 3d3d 3d20 2775 6e64 6566 696e      === 'undefin
-00011910: 6564 2729 207b 5c72 5c6e 2020 2020 2020  ed') {\r\n      
-00011920: 2020 6361 6e63 656c 5465 7874 203d 205c    cancelText = \
-00011930: 2250 6572 7575 7461 5c22 3b5c 725c 6e20  "Peruuta\";\r\n 
-00011940: 2020 207d 5c72 5c6e 2020 2020 246d 6f64     }\r\n    $mod
-00011950: 616c 2e66 696e 6428 275b 6461 7461 2d61  al.find('[data-a
-00011960: 6374 696f 6e3d 5c22 6361 6e63 656c 5c22  ction=\"cancel\"
-00011970: 5d27 292e 6874 6d6c 2863 616e 6365 6c54  ]').html(cancelT
-00011980: 6578 7429 3b5c 725c 6e5c 725c 6e0a 2020  ext);\r\n\r\n.  
-00011990: 2020 2020 2020 5c20 2020 246d 6f64 616c        \   $modal
-000119a0: 2e66 696e 6428 275b 6461 7461 2d61 6374  .find('[data-act
-000119b0: 696f 6e3d 5c22 6f6b 5c22 5d27 292e 6f66  ion=\"ok\"]').of
-000119c0: 6628 2763 6c69 636b 2729 2e6f 6e28 2763  f('click').on('c
-000119d0: 6c69 636b 272c 2066 756e 6374 696f 6e28  lick', function(
-000119e0: 6529 0a20 2020 2020 2020 207b 5c72 5c6e  e).        {\r\n
-000119f0: 2020 2020 2020 2020 246d 6f64 616c 2e6d          $modal.m
-00011a00: 6f64 616c 2827 6869 6465 2729 3b5c 725c  odal('hide');\r\
-00011a10: 6e20 2020 2020 2020 2064 6566 6572 7265  n        deferre
-00011a20: 642e 7265 736f 6c76 6528 7472 7565 293b  d.resolve(true);
-00011a30: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-00011a40: 207d 293b 5c72 5c6e 2020 2020 246d 6f64   });\r\n    $mod
-00011a50: 616c 2e66 696e 6428 275b 6461 7461 2d61  al.find('[data-a
-00011a60: 6374 696f 6e3d 5c22 6361 6e63 656c 5c22  ction=\"cancel\"
-00011a70: 5d27 292e 6f66 6628 2763 6c69 636b 2729  ]').off('click')
-00011a80: 2e6f 6e28 2763 6c69 636b 272c 0a20 2020  .on('click',.   
-00011a90: 2020 2020 2066 756e 6374 696f 6e28 6529       function(e)
-00011aa0: 207b 5c72 5c6e 2020 2020 2020 2020 246d   {\r\n        $m
-00011ab0: 6f64 616c 2e6d 6f64 616c 2827 6869 6465  odal.modal('hide
-00011ac0: 2729 3b5c 725c 6e20 2020 2020 2020 2064  ');\r\n        d
-00011ad0: 6566 6572 7265 642e 7265 6a65 6374 2866  eferred.reject(f
-00011ae0: 616c 7365 293b 5c72 5c6e 0a20 2020 2020  alse);\r\n.     
-00011af0: 2020 205c 2020 207d 293b 5c72 5c6e 5c72     \   });\r\n\r
-00011b00: 5c6e 2020 2020 246d 6f64 616c 2e6d 6f64  \n    $modal.mod
-00011b10: 616c 2827 7368 6f77 2729 3b5c 725c 6e20  al('show');\r\n 
-00011b20: 2020 2072 6574 7572 6e20 6465 6665 7272     return deferr
-00011b30: 6564 3b5c 725c 6e7d 5c72 5c6e 5c72 5c6e  ed;\r\n}\r\n\r\n
-00011b40: 3c2f 7363 7269 7074 3e5c 725c 6e5c 725c  </script>\r\n\r\
-00011b50: 6e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  n\r\n\r\n\r\n\r\
-00011b60: 6e5c 725c 6e3c 7363 7269 7074 0a20 2020  n\r\n<script.   
-00011b70: 2020 2020 2069 643d 5c22 7365 7276 6963       id=\"servic
-00011b80: 652d 6c69 7374 2d69 7465 6d2d 7465 6d70  e-list-item-temp
-00011b90: 6c61 7465 5c22 2074 7970 653d 5c22 7465  late\" type=\"te
-00011ba0: 7874 2f78 2d74 656d 706c 6174 655c 223e  xt/x-template\">
-00011bb0: 5c72 5c6e 5c72 5c6e 5c72 5c6e 3c66 6965  \r\n\r\n\r\n<fie
-00011bc0: 6c64 7365 740a 2020 2020 2020 2020 636c  ldset.        cl
-00011bd0: 6173 733d 5c22 7365 7276 6963 652d 6974  ass=\"service-it
-00011be0: 656d 5c22 3e5c 725c 6e5c 743c 6c65 6765  em\">\r\n\t<lege
-00011bf0: 6e64 2063 6c61 7373 3d5c 2273 6572 7669  nd class=\"servi
-00011c00: 6365 2d6e 616d 655c 223e 3c2f 6c65 6765  ce-name\"></lege
-00011c10: 6e64 3e5c 725c 6e5c 725c 6e5c 743c 6469  nd>\r\n\r\n\t<di
-00011c20: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
-00011c30: 5c22 6b69 6d70 7061 2d69 6e66 6f20 726f  \"kimppa-info ro
-00011c40: 775c 223e 5c72 5c6e 5c74 5c74 5c72 5c6e  w\">\r\n\t\t\r\n
-00011c50: 5c72 5c6e 5c74 5c74 5c72 5c6e 5c74 5c74  \r\n\t\t\r\n\t\t
-00011c60: 5c74 3c64 6976 2063 6c61 7373 3d5c 2263  \t<div class=\"c
-00011c70: 6f6c 2d6d 642d 3132 5c22 3e5c 725c 6e5c  ol-md-12\">\r\n\
-00011c80: 745c 745c 745c 743c 646c 3e5c 725c 6e5c  t\t\t\t<dl>\r\n\
-00011c90: 745c 745c 745c 745c 743c 6c61 6265 6c0a  t\t\t\t\t<label.
-00011ca0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-00011cb0: 6b69 6d70 616e 2d69 7361 6e74 615c 223e  kimpan-isanta\">
-00011cc0: 3c2f 6c61 6265 6c3e 5c72 5c6e 5c74 5c74  </label>\r\n\t\t
-00011cd0: 5c74 5c74 5c74 3c6c 6162 656c 2063 6c61  \t\t\t<label cla
-00011ce0: 7373 3d5c 2269 7361 6e6e 616e 2d6f 736f  ss=\"isannan-oso
-00011cf0: 6974 655c 223e 3c2f 6c61 6265 6c3e 5c72  ite\"></label>\r
-00011d00: 5c6e 5c74 5c74 5c74 5c74 5c74 3c6c 6162  \n\t\t\t\t\t<lab
-00011d10: 656c 3e3c 6c61 6265 6c0a 2020 2020 2020  el><label.      
-00011d20: 2020 636c 6173 733d 5c22 6b69 6d70 616e    class=\"kimpan
-00011d30: 2d6a 6173 656e 7465 6e2d 6d61 6172 615c  -jasenten-maara\
-00011d40: 223e 3c2f 6c61 6265 6c3e 206f 7361 6b61  "></label> osaka
-00011d50: 7374 613c 2f6c 6162 656c 3e5c 725c 6e5c  sta</label>\r\n\
-00011d60: 745c 745c 745c 745c 743c 6c61 6265 6c3e  t\t\t\t\t<label>
-00011d70: 6c61 736b 7574 7573 6f73 7575 730a 2020  laskutusosuus.  
-00011d80: 2020 2020 2020 3c6c 6162 656c 2063 6c61        <label cla
-00011d90: 7373 3d5c 224b 4952 5072 6f73 5c22 3e3c  ss=\"KIRPros\"><
-00011da0: 2f6c 6162 656c 3e3c 2f6c 6162 656c 3e5c  /label></label>\
-00011db0: 725c 6e5c 745c 745c 745c 743c 2f64 6c3e  r\n\t\t\t\t</dl>
-00011dc0: 5c72 5c6e 5c74 5c74 5c74 3c2f 6469 763e  \r\n\t\t\t</div>
-00011dd0: 5c72 5c6e 5c72 5c6e 5c74 5c74 5c74 5c72  \r\n\r\n\t\t\t\r
-00011de0: 5c6e 5c74 5c74 5c72 5c6e 5c72 5c6e 5c74  \n\t\t\r\n\r\n\t
-00011df0: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 5c74  </div>\r\n\r\n\t
-00011e00: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
-00011e10: 7373 3d5c 2272 6f77 5c22 2064 6174 612d  ss=\"row\" data-
-00011e20: 6865 6164 6572 3d5c 2241 5354 4b6f 6d6d  header=\"ASTKomm
-00011e30: 5c22 3e5c 725c 6e5c 745c 743c 6469 7620  \">\r\n\t\t<div 
-00011e40: 636c 6173 733d 5c22 636f 6c2d 6d64 2d6f  class=\"col-md-o
-00011e50: 6666 7365 742d 320a 2020 2020 2020 2020  ffset-2.        
-00011e60: 636f 6c2d 6d64 2d37 5c22 3e5c 725c 6e5c  col-md-7\">\r\n\
-00011e70: 745c 745c 743c 7020 6461 7461 2d76 616c  t\t\t<p data-val
-00011e80: 7565 3d5c 2241 5354 4b6f 6d6d 5c22 3e3c  ue=\"ASTKomm\"><
-00011e90: 2f70 3e5c 725c 6e5c 745c 743c 2f64 6976  /p>\r\n\t\t</div
-00011ea0: 3e5c 725c 6e5c 743c 2f64 6976 3e5c 725c  >\r\n\t</div>\r\
-00011eb0: 6e5c 725c 6e5c 743c 6469 760a 2020 2020  n\r\n\t<div.    
-00011ec0: 2020 2020 636c 6173 733d 5c22 726f 775c      class=\"row\
-00011ed0: 223e 5c72 5c6e 5c74 5c74 3c64 6976 2063  ">\r\n\t\t<div c
-00011ee0: 6c61 7373 3d5c 2263 6f6c 2d6d 642d 325c  lass=\"col-md-2\
-00011ef0: 223e 5c72 5c6e 5c74 5c74 5c74 3c69 6d67  ">\r\n\t\t\t<img
-00011f00: 2063 6c61 7373 3d5c 2273 6572 7669 6365   class=\"service
-00011f10: 2d69 6d61 6765 0a20 2020 2020 2020 2069  -image.        i
-00011f20: 6d67 2d72 6573 706f 6e73 6976 655c 2220  mg-responsive\" 
-00011f30: 616c 743d 5c22 5c22 206f 6e65 7272 6f72  alt=\"\" onerror
-00011f40: 3d5c 2274 6869 732e 7374 796c 652e 7669  =\"this.style.vi
-00011f50: 7369 6269 6c69 7479 3d27 6869 6464 656e  sibility='hidden
-00011f60: 273b 7265 7475 726e 0a20 2020 2020 2020  ';return.       
-00011f70: 2074 7275 655c 223e 5c72 5c6e 5c74 5c74   true\">\r\n\t\t
-00011f80: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 5c74  </div>\r\n\r\n\t
-00011f90: 5c74 3c64 6976 2063 6c61 7373 3d5c 2263  \t<div class=\"c
-00011fa0: 6f6c 2d6d 642d 375c 223e 5c72 5c6e 5c74  ol-md-7\">\r\n\t
-00011fb0: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
-00011fc0: 2273 6572 7669 6365 2d69 6e66 6f5c 223e  "service-info\">
-00011fd0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c72 5c6e  \r\n\t\t\t\t\r\n
-00011fe0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c72 5c6e  \r\n\t\t\t\t\r\n
-00011ff0: 5c74 5c74 5c74 5c74 3c64 6976 0a20 2020  \t\t\t\t<div.   
-00012000: 2020 2020 2064 6174 612d 6865 6164 6572       data-header
-00012010: 3d5c 2241 5354 4d61 6172 615c 223e 5c72  =\"ASTMaara\">\r
-00012020: 5c6e 5c74 5c74 5c74 5c74 5c74 3c73 7061  \n\t\t\t\t\t<spa
-00012030: 6e20 6461 7461 2d76 616c 7565 3d5c 2241  n data-value=\"A
-00012040: 5354 4d61 6172 615c 223e 3c2f 7370 616e  STMaara\"></span
-00012050: 3e3c 7370 616e 3e0a 2020 2020 2020 2020  ><span>.        
-00012060: 3c2f 7370 616e 3e3c 7370 616e 2064 6174  </span><span dat
-00012070: 612d 7661 6c75 653d 5c22 7461 7269 6666  a-value=\"tariff
-00012080: 2e75 6e69 745c 223e 6b70 6c2f 743c 2f73  .unit\">kpl/t</s
-00012090: 7061 6e3e 5c72 5c6e 5c72 5c6e 5c74 5c74  pan>\r\n\r\n\t\t
-000120a0: 5c74 5c74 5c74 5c72 5c6e 5c74 5c74 5c74  \t\t\t\r\n\t\t\t
-000120b0: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
-000120c0: 5c74 5c74 5c72 5c6e 5c72 5c6e 5c74 5c74  \t\t\r\n\r\n\t\t
-000120d0: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 5c74  \t\t\r\n\t\t\t\t
-000120e0: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
-000120f0: 6c61 7373 3d5c 2263 6f6c 6c65 6374 696f  lass=\"collectio
-00012100: 6e2d 7363 6865 6475 6c65 5c22 3e3c 6120  n-schedule\"><a 
-00012110: 6872 6566 3d5c 225c 2220 6461 7461 2d61  href=\"\" data-a
-00012120: 6374 696f 6e3d 5c22 636f 6c6c 6563 7469  ction=\"collecti
-00012130: 6f6e 2d73 6368 6564 756c 655c 223e 5c78  on-schedule\">\x
-00012140: 4242 0a20 2020 2020 2020 2054 7968 6a65  BB.        Tyhje
-00012150: 6e6e 7973 7279 746d 693c 2f61 3e3c 2f64  nnysrytmi</a></d
-00012160: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
-00012170: 725c 6e5c 725c 6e5c 745c 745c 745c 745c  r\n\r\n\t\t\t\t\
-00012180: 725c 6e5c 725c 6e5c 745c 745c 745c 745c  r\n\r\n\t\t\t\t\
-00012190: 725c 6e5c 725c 6e5c 745c 745c 745c 745c  r\n\r\n\t\t\t\t\
-000121a0: 725c 6e5c 725c 6e5c 745c 745c 745c 745c  r\n\r\n\t\t\t\t\
-000121b0: 725c 6e5c 725c 6e5c 745c 745c 745c 745c  r\n\r\n\t\t\t\t\
-000121c0: 725c 6e5c 725c 6e5c 745c 745c 745c 745c  r\n\r\n\t\t\t\t\
-000121d0: 725c 6e5c 745c 745c 745c 743c 6469 760a  r\n\t\t\t\t<div.
-000121e0: 2020 2020 2020 2020 6461 7461 2d68 6561          data-hea
-000121f0: 6465 723d 5c22 4153 544e 6578 7444 6174  der=\"ASTNextDat
-00012200: 655c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  e\">\r\n\t\t\t\t
-00012210: 5c74 3c64 6976 2064 6174 612d 6865 6164  \t<div data-head
-00012220: 6572 3d5c 2241 5354 4e65 7874 4461 7465  er=\"ASTNextDate
-00012230: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
-00012240: 745c 743c 7370 616e 3e53 6575 7261 6176  t\t<span>Seuraav
-00012250: 610a 2020 2020 2020 2020 7479 686a 656e  a.        tyhjen
-00012260: 6e79 7320 3c2f 7370 616e 3e5c 725c 6e5c  nys </span>\r\n\
-00012270: 745c 745c 745c 745c 745c 743c 7370 616e  t\t\t\t\t\t<span
-00012280: 2064 6174 612d 7661 6c75 653d 5c22 4153   data-value=\"AS
-00012290: 544e 6578 7444 6174 655c 223e 3c2f 7370  TNextDate\"></sp
-000122a0: 616e 3e5c 725c 6e5c 745c 745c 745c 745c  an>\r\n\t\t\t\t\
-000122b0: 745c 743c 7370 616e 0a20 2020 2020 2020  t\t<span.       
-000122c0: 2064 6174 612d 726f 6c65 3d5c 226e 6578   data-role=\"nex
-000122d0: 742d 656d 7074 7969 6e67 2d76 6172 6961  t-emptying-varia
-000122e0: 6e63 652d 7465 7874 5c22 3e5c 725c 6e5c  nce-text\">\r\n\
-000122f0: 745c 745c 745c 745c 745c 745c 7420 285c  t\t\t\t\t\t\t (\
-00012300: 7842 3120 312d 3220 705c 7845 3469 765c  xB1 1-2 p\xE4iv\
-00012310: 7845 345c 7845 3429 5c72 5c6e 5c74 5c74  xE4\xE4)\r\n\t\t
-00012320: 5c74 5c74 5c74 5c74 3c2f 7370 616e 3e5c  \t\t\t\t</span>\
-00012330: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012350: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
-00012360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012370: 2020 2020 3c69 2064 6174 612d 726f 6c65      <i data-role
-00012380: 3d5c 226e 6578 742d 656d 7074 7969 6e67  =\"next-emptying
-00012390: 2d76 6172 6961 6e63 652d 746f 6f6c 7469  -variance-toolti
-000123a0: 705c 220a 2020 2020 2020 2020 636c 6173  p\".        clas
-000123b0: 733d 5c22 676c 7970 6869 636f 6e20 676c  s=\"glyphicon gl
-000123c0: 7970 6869 636f 6e2d 7175 6573 7469 6f6e  yphicon-question
-000123d0: 2d73 6967 6e5c 225c 725c 6e20 2020 2020  -sign\"\r\n     
-000123e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123f0: 2020 2020 2020 2020 2020 2074 6162 696e             tabin
-00012400: 6465 783d 5c22 2d31 5c22 0a20 2020 2020  dex=\"-1\".     
-00012410: 2020 2064 6174 612d 6f72 6967 696e 616c     data-original
-00012420: 2d74 6974 6c65 3d5c 2241 6a6f 705c 7845  -title=\"Ajop\xE
-00012430: 3469 765c 7845 3420 766f 6920 6d75 7574  4iv\xE4 voi muut
-00012440: 7475 6120 285c 7842 3120 312d 3220 705c  tua (\xB1 1-2 p\
-00012450: 7845 3469 765c 7845 345c 7845 3429 0a20  xE4iv\xE4\xE4). 
-00012460: 2020 2020 2020 2065 7369 6d2e 2061 726b         esim. ark
-00012470: 6970 7968 5c78 4534 7669 696b 6f69 6c6c  ipyh\xE4viikoill
-00012480: 612e 5c22 5c72 5c6e 2020 2020 2020 2020  a.\"\r\n        
-00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124a0: 2020 2020 2020 2020 6461 7461 2d74 6f67          data-tog
-000124b0: 676c 653d 5c22 706f 706f 7665 725c 220a  gle=\"popover\".
-000124c0: 2020 2020 2020 2020 6461 7461 2d70 6c61          data-pla
-000124d0: 6365 6d65 6e74 3d5c 2261 7574 6f20 7269  cement=\"auto ri
-000124e0: 6768 745c 2220 6461 7461 2d74 7269 6767  ght\" data-trigg
-000124f0: 6572 3d5c 2266 6f63 7573 5c22 3e3c 2f69  er=\"focus\"></i
-00012500: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-00012510: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
-00012520: 6e5c 745c 745c 745c 745c 743c 2f64 6976  n\t\t\t\t\t</div
-00012530: 3e5c 725c 6e5c 745c 745c 745c 743c 2f64  >\r\n\t\t\t\t</d
-00012540: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
-00012550: 725c 6e5c 725c 6e5c 745c 745c 745c 745c  r\n\r\n\t\t\t\t\
-00012560: 725c 6e5c 725c 6e5c 745c 745c 745c 745c  r\n\r\n\t\t\t\t\
-00012570: 725c 6e5c 725c 6e5c 745c 745c 745c 745c  r\n\r\n\t\t\t\t\
-00012580: 725c 6e5c 745c 745c 745c 743c 6469 760a  r\n\t\t\t\t<div.
-00012590: 2020 2020 2020 2020 6461 7461 2d68 6561          data-hea
-000125a0: 6465 723d 5c22 4153 544d 6174 6b61 5c22  der=\"ASTMatka\"
-000125b0: 3e5c 725c 6e5c 745c 745c 745c 745c 743c  >\r\n\t\t\t\t\t<
-000125c0: 6469 7620 6461 7461 2d68 6561 6465 723d  div data-header=
-000125d0: 5c22 4153 544d 6174 6b61 5c22 3e4d 6174  \"ASTMatka\">Mat
-000125e0: 6b61 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ka\r\n\t\t\t\t\t
-000125f0: 3c73 7061 6e3e 0a20 2020 2020 2020 203c  <span>.        <
-00012600: 2f73 7061 6e3e 3c73 7061 6e20 6461 7461  /span><span data
-00012610: 2d76 616c 7565 3d5c 2241 5354 4d61 746b  -value=\"ASTMatk
-00012620: 615c 223e 3c2f 7370 616e 3e20 6d20 3c73  a\"></span> m <s
-00012630: 7061 6e20 6461 7461 2d76 616c 7565 3d5c  pan data-value=\
-00012640: 2241 5354 4d61 746b 6150 7269 6365 5c22  "ASTMatkaPrice\"
-00012650: 3e3c 2f73 7061 6e3e 5c72 5c6e 0a20 2020  ></span>\r\n.   
-00012660: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-00012670: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-00012680: 725c 6e5c 745c 745c 745c 743c 2f64 6976  r\n\t\t\t\t</div
-00012690: 3e5c 725c 6e5c 745c 745c 745c 745c 725c  >\r\n\t\t\t\t\r\
-000126a0: 6e5c 725c 6e5c 745c 745c 745c 745c 725c  n\r\n\t\t\t\t\r\
-000126b0: 6e5c 725c 6e5c 745c 745c 745c 745c 725c  n\r\n\t\t\t\t\r\
-000126c0: 6e5c 745c 745c 745c 743c 6469 760a 2020  n\t\t\t\t<div.  
-000126d0: 2020 2020 2020 6461 7461 2d68 6561 6465        data-heade
-000126e0: 723d 5c22 4153 544b 6573 6b41 6c6b 2d41  r=\"ASTKeskAlk-A
-000126f0: 7374 5c22 3e5c 725c 6e5c 745c 745c 745c  st\">\r\n\t\t\t\
-00012700: 745c 743c 6469 7620 6461 7461 2d68 6561  t\t<div data-hea
-00012710: 6465 723d 5c22 4153 544b 6573 6b41 6c6b  der=\"ASTKeskAlk
-00012720: 2d41 7374 5c22 3e4b 6573 6b65 7974 7973  -Ast\">Keskeytys
-00012730: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 3c73  \r\n\t\t\t\t\t<s
-00012740: 7061 6e3e 0a20 2020 2020 2020 203c 2f73  pan>.        </s
-00012750: 7061 6e3e 3c73 7061 6e20 6461 7461 2d76  pan><span data-v
-00012760: 616c 7565 3d5c 2241 5354 4b65 736b 416c  alue=\"ASTKeskAl
-00012770: 6b2d 4173 745c 223e 3c2f 7370 616e 3e5c  k-Ast\"></span>\
-00012780: 725c 6e5c 745c 745c 745c 745c 743c 2f64  r\n\t\t\t\t\t</d
-00012790: 6976 3e5c 725c 6e5c 745c 745c 745c 743c  iv>\r\n\t\t\t\t<
-000127a0: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
-000127b0: 745c 725c 6e5c 725c 6e5c 745c 745c 745c  t\r\n\r\n\t\t\t\
-000127c0: 743c 6469 760a 2020 2020 2020 2020 6461  t<div.        da
-000127d0: 7461 2d68 6561 6465 723d 5c22 4153 544c  ta-header=\"ASTL
-000127e0: 6f70 5076 6d5c 223e 5c72 5c6e 5c74 5c74  opPvm\">\r\n\t\t
-000127f0: 5c74 5c74 5c74 3c64 6976 2064 6174 612d  \t\t\t<div data-
-00012800: 6865 6164 6572 3d5c 2241 5354 4c6f 7050  header=\"ASTLopP
-00012810: 766d 5c22 3e4c 6f70 6574 7573 3c2f 6469  vm\">Lopetus</di
-00012820: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  v>\r\n\t\t\t\t\t
-00012830: 3c64 6976 0a20 2020 2020 2020 2064 6174  <div.        dat
-00012840: 612d 7661 6c75 653d 5c22 4153 544c 6f70  a-value=\"ASTLop
-00012850: 5076 6d5c 223e 3c2f 6469 763e 5c72 5c6e  Pvm\"></div>\r\n
-00012860: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
-00012870: 5c6e 5c72 5c6e 5c74 5c74 5c74 5c74 5c72  \n\r\n\t\t\t\t\r
-00012880: 5c6e 5c74 5c74 5c74 3c2f 6469 763e 5c72  \n\t\t\t</div>\r
-00012890: 5c6e 5c72 5c6e 5c74 5c74 5c74 5c72 5c6e  \n\r\n\t\t\t\r\n
-000128a0: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
-000128b0: 2020 2063 6c61 7373 3d5c 2265 7874 7261     class=\"extra
-000128c0: 2d74 6578 745c 223e 5c72 5c6e 5c74 5c74  -text\">\r\n\t\t
-000128d0: 5c74 5c74 3c61 2068 7265 663d 5c22 6874  \t\t<a href=\"ht
-000128e0: 7470 3a2f 2f77 7777 2e6a 6174 656b 756b  tp://www.jatekuk
-000128f0: 6b6f 2e66 692f 6c61 6a69 7474 656c 755c  ko.fi/lajittelu\
-00012900: 220a 2020 2020 2020 2020 7461 7267 6574  ".        target
-00012910: 3d5c 225f 626c 616e 6b5c 223e 3c73 6d61  =\"_blank\"><sma
-00012920: 6c6c 3e5c 7842 4220 4c61 6a69 7474 656c  ll>\xBB Lajittel
-00012930: 756f 686a 6565 743c 2f73 6d61 6c6c 3e20  uohjeet</small> 
-00012940: 3c2f 613e 3c61 2068 7265 663d 5c22 6874  </a><a href=\"ht
-00012950: 7470 3a2f 2f77 7777 2e6a 6174 656b 756b  tp://www.jatekuk
-00012960: 6b6f 2e66 692f 6869 6e6e 6174 5c22 0a20  ko.fi/hinnat\". 
-00012970: 2020 2020 2020 2074 6172 6765 743d 5c22         target=\"
-00012980: 5f62 6c61 6e6b 5c22 3e3c 736d 616c 6c3e  _blank\"><small>
-00012990: 5c78 4242 204c 6973 5c78 4534 7469 6574  \xBB Lis\xE4tiet
-000129a0: 6f6a 6120 6869 6e6e 6f69 7374 613c 2f73  oja hinnoista</s
-000129b0: 6d61 6c6c 3e3c 2f61 3e5c 725c 6e5c 745c  mall></a>\r\n\t\
-000129c0: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
-000129d0: 745c 745c 725c 6e5c 725c 6e0a 2020 2020  t\t\r\n\r\n.    
-000129e0: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-000129f0: 5c72 5c6e 5c74 5c74 5c74 2020 2020 3c64  \r\n\t\t\t    <d
-00012a00: 6976 2063 6c61 7373 3d5c 2273 6572 7669  iv class=\"servi
-00012a10: 6365 2d69 6e66 6f5c 223e 5c72 5c6e 5c74  ce-info\">\r\n\t
-00012a20: 5c74 5c74 5c74 2020 2020 3c64 6976 0a20  \t\t\t    <div. 
-00012a30: 2020 2020 2020 2064 6174 612d 6865 6164         data-head
-00012a40: 6572 3d5c 2241 5354 5065 724d 6174 6b61  er=\"ASTPerMatka
-00012a50: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
-00012a60: 7420 2020 203c 6469 7620 6461 7461 2d68  t    <div data-h
-00012a70: 6561 6465 723d 5c22 4153 5450 6572 4d61  eader=\"ASTPerMa
-00012a80: 746b 615c 223e 4d61 746b 615c 725c 6e5c  tka\">Matka\r\n\
-00012a90: 745c 745c 745c 745c 740a 2020 2020 2020  t\t\t\t\t.      
-00012aa0: 2020 5c20 2020 3c73 7061 6e3e 203c 2f73    \   <span> </s
-00012ab0: 7061 6e3e 3c73 7061 6e20 6461 7461 2d76  pan><span data-v
-00012ac0: 616c 7565 3d5c 2241 5354 5065 724d 6174  alue=\"ASTPerMat
-00012ad0: 6b61 5c22 3e3c 2f73 7061 6e3e 206d 3c2f  ka\"></span> m</
-00012ae0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
-00012af0: 0a20 2020 2020 2020 205c 2020 203c 2f64  .        \   </d
-00012b00: 6976 3e5c 725c 6e20 2020 2020 2020 2020  iv>\r\n         
-00012b10: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
-00012b20: 6e20 2020 2020 2020 2020 2020 205c 725c  n            \r\
-00012b30: 6e5c 725c 6e5c 745c 745c 745c 725c 6e5c  n\r\n\t\t\t\r\n\
-00012b40: 745c 745c 745c 725c 6e5c 745c 745c 745c  t\t\t\r\n\t\t\t\
-00012b50: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
-00012b60: 6173 733d 5c22 6465 7363 7269 7074 696f  ass=\"descriptio
-00012b70: 6e5c 223e 3c2f 6469 763e 5c72 5c6e 5c74  n\"></div>\r\n\t
-00012b80: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 5c72  \t\t\r\n\t\t\t\r
-00012b90: 5c6e 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \n\t\t\t\r\n\t\t
-00012ba0: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 5c74  </div>\r\n\r\n\t
-00012bb0: 5c74 5c72 5c6e 5c74 5c74 3c64 6976 0a20  \t\r\n\t\t<div. 
-00012bc0: 2020 2020 2020 2063 6c61 7373 3d5c 2264         class=\"d
-00012bd0: 726f 7064 6f77 6e2d 636f 6e74 656e 745c  ropdown-content\
-00012be0: 223e 5c72 5c6e 5c74 5c74 5c72 5c6e 5c74  ">\r\n\t\t\r\n\t
-00012bf0: 5c74 5c72 5c6e 5c74 5c74 3c64 6976 2063  \t\r\n\t\t<div c
-00012c00: 6c61 7373 3d5c 2263 6f6c 2d6d 642d 3320  lass=\"col-md-3 
-00012c10: 7365 7276 6963 652d 6275 7474 6f6e 735c  service-buttons\
-00012c20: 223e 5c72 5c6e 5c72 5c6e 5c74 5c74 5c74  ">\r\n\r\n\t\t\t
-00012c30: 5c72 5c6e 5c72 5c6e 0a20 2020 2020 2020  \r\n\r\n.       
-00012c40: 205c 2020 2020 2020 2020 2020 205c 725c   \           \r\
-00012c50: 6e20 2020 2020 2020 2020 2020 203c 6275  n            <bu
-00012c60: 7474 6f6e 2063 6c61 7373 3d5c 226f 7264  tton class=\"ord
-00012c70: 6572 2d62 7574 746f 6e20 6274 6e20 6274  er-button btn bt
-00012c80: 6e2d 7072 696d 6172 7920 6274 6e2d 626c  n-primary btn-bl
-00012c90: 6f63 6b0a 2020 2020 2020 2020 6274 6e2d  ock.        btn-
-00012ca0: 7772 6170 5c22 3e5c 725c 6e20 2020 2020  wrap\">\r\n     
-00012cb0: 2020 2020 2020 205c 7454 696c 6161 2079         \tTilaa y
-00012cc0: 6c69 6d5c 7845 345c 7845 3472 5c78 4534  lim\xE4\xE4r\xE4
-00012cd0: 696e 656e 2074 7968 6a65 6e6e 7973 5c72  inen tyhjennys\r
-00012ce0: 5c6e 2020 2020 2020 2020 5c74 3c2f 6275  \n        \t</bu
-00012cf0: 7474 6f6e 3e5c 725c 6e0a 2020 2020 2020  tton>\r\n.      
-00012d00: 2020 5c20 2020 2020 2020 2020 2020 5c72    \           \r
-00012d10: 5c6e 5c72 5c6e 2020 2020 2020 2020 2020  \n\r\n          
-00012d20: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
-00012d30: 2020 3c62 7574 746f 6e20 636c 6173 733d    <button class=
-00012d40: 5c22 7061 7573 652d 6275 7474 6f6e 0a20  \"pause-button. 
-00012d50: 2020 2020 2020 2062 746e 2062 746e 2d70         btn btn-p
-00012d60: 7269 6d61 7279 2062 746e 2d62 6c6f 636b  rimary btn-block
-00012d70: 2062 746e 2d77 7261 705c 223e 5c72 5c6e   btn-wrap\">\r\n
-00012d80: 2020 2020 2020 2020 2020 2020 5c74 4b65              \tKe
-00012d90: 736b 6579 745c 7845 345c 725c 6e20 2020  skeyt\xE4\r\n   
-00012da0: 2020 2020 205c 743c 2f62 7574 746f 6e3e       \t</button>
-00012db0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-00012dc0: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
-00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012de0: 205c 725c 6e20 2020 2020 2020 2020 2020   \r\n           
-00012df0: 205c 725c 6e5c 745c 745c 743c 6275 7474   \r\n\t\t\t<butt
-00012e00: 6f6e 2063 6c61 7373 3d5c 2263 6861 6e67  on class=\"chang
-00012e10: 652d 7265 7175 6573 742d 6275 7474 6f6e  e-request-button
-00012e20: 0a20 2020 2020 2020 2062 746e 2062 746e  .        btn btn
-00012e30: 2d70 7269 6d61 7279 2062 746e 2d62 6c6f  -primary btn-blo
-00012e40: 636b 2062 746e 2d77 7261 705c 223e 5c72  ck btn-wrap\">\r
-00012e50: 5c6e 5c74 5c74 5c74 5c74 4d75 7520 6d75  \n\t\t\t\tMuu mu
-00012e60: 7574 6f73 2070 616c 7665 6c75 756e 5c72  utos palveluun\r
-00012e70: 5c6e 5c74 5c74 5c74 3c2f 6275 7474 6f6e  \n\t\t\t</button
-00012e80: 3e5c 725c 6e5c 745c 745c 745c 725c 6e0a  >\r\n\t\t\t\r\n.
-00012e90: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-00012ea0: 2020 2020 2020 2020 5c72 5c6e 2020 2020          \r\n    
-00012eb0: 2020 2020 2020 2020 5c72 5c6e 5c74 5c74          \r\n\t\t
-00012ec0: 2020 2020 5c74 3c62 7574 746f 6e20 7479      \t<button ty
-00012ed0: 7065 3d5c 2262 7574 746f 6e5c 2220 636c  pe=\"button\" cl
-00012ee0: 6173 733d 5c22 6274 6e0a 2020 2020 2020  ass=\"btn.      
-00012ef0: 2020 6274 6e2d 7072 696d 6172 7920 6274    btn-primary bt
-00012f00: 6e2d 626c 6f63 6b20 6274 6e2d 7772 6170  n-block btn-wrap
-00012f10: 2066 756c 6c2d 7769 6474 685c 2220 6461   full-width\" da
-00012f20: 7461 2d61 6374 696f 6e3d 5c22 6564 6974  ta-action=\"edit
-00012f30: 2d6b 696d 7070 615c 223e 5c72 5c6e 5c74  -kimppa\">\r\n\t
-00012f40: 5c74 0a20 2020 2020 2020 205c 2020 205c  \t.        \   \
-00012f50: 745c 744d 756f 6b6b 6161 206b 696d 7070  t\tMuokkaa kimpp
-00012f60: 6161 5c72 5c6e 5c74 2020 2020 5c74 5c74  aa\r\n\t    \t\t
-00012f70: 3c2f 6275 7474 6f6e 3e5c 725c 6e5c 745c  </button>\r\n\t\
-00012f80: 7420 2020 205c 725c 6e5c 725c 6e5c 745c  t    \r\n\r\n\t\
-00012f90: 745c 745c 725c 6e5c 745c 745c 743c 6275  t\t\r\n\t\t\t<bu
-00012fa0: 7474 6f6e 0a20 2020 2020 2020 2063 6c61  tton.        cla
-00012fb0: 7373 3d5c 2272 6573 6967 6e2d 6b69 6d70  ss=\"resign-kimp
-00012fc0: 7061 2d62 7574 746f 6e20 6274 6e20 6274  pa-button btn bt
-00012fd0: 6e2d 7072 696d 6172 795c 223e 5c72 5c6e  n-primary\">\r\n
-00012fe0: 5c74 5c74 5c74 5c74 4572 6f61 206b 696d  \t\t\t\tEroa kim
-00012ff0: 7061 7374 615c 725c 6e5c 745c 745c 743c  pasta\r\n\t\t\t<
-00013000: 2f62 7574 746f 6e3e 5c72 5c6e 5c74 5c74  /button>\r\n\t\t
-00013010: 5c74 5c72 5c6e 5c72 5c6e 0a20 2020 2020  \t\r\n\r\n.     
-00013020: 2020 205c 2020 2020 2020 2020 2020 205c     \           \
-00013030: 725c 6e20 2020 2020 2020 2020 2020 205c  r\n            \
-00013040: 743c 6275 7474 6f6e 2063 6c61 7373 3d5c  t<button class=\
-00013050: 226b 696d 7061 6b73 692d 6275 7474 6f6e  "kimpaksi-button
-00013060: 2062 746e 2062 746e 2d70 7269 6d61 7279   btn btn-primary
-00013070: 0a20 2020 2020 2020 2062 746e 2d62 6c6f  .        btn-blo
-00013080: 636b 2062 746e 2d77 7261 705c 223e 5c72  ck btn-wrap\">\r
-00013090: 5c6e 2020 2020 2020 2020 2020 2020 5c74  \n            \t
-000130a0: 5c74 5065 7275 7374 6120 7575 7369 206b  \tPerusta uusi k
-000130b0: 696d 7070 615c 725c 6e20 2020 2020 2020  imppa\r\n       
-000130c0: 205c 745c 743c 2f62 7574 746f 6e3e 5c72   \t\t</button>\r
-000130d0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-000130e0: 2020 2020 2020 205c 725c 6e5c 725c 6e20         \r\n\r\n 
-000130f0: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
-00013100: 2020 2020 2020 2020 2020 205c 725c 6e5c             \r\n\
-00013110: 745c 745c 743c 6275 7474 6f6e 2063 6c61  t\t\t<button cla
-00013120: 7373 3d5c 2273 746f 702d 6275 7474 6f6e  ss=\"stop-button
-00013130: 0a20 2020 2020 2020 2062 746e 2062 746e  .        btn btn
-00013140: 2d70 7269 6d61 7279 2062 746e 2d62 6c6f  -primary btn-blo
-00013150: 636b 2062 746e 2d77 7261 705c 223e 5c72  ck btn-wrap\">\r
-00013160: 5c6e 5c74 5c74 5c74 5c74 4c6f 7065 7461  \n\t\t\t\tLopeta
-00013170: 5c72 5c6e 5c74 5c74 5c74 3c2f 6275 7474  \r\n\t\t\t</butt
-00013180: 6f6e 3e5c 725c 6e0a 2020 2020 2020 2020  on>\r\n.        
-00013190: 5c20 2020 2020 2020 2020 2020 5c72 5c6e  \           \r\n
-000131a0: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
-000131b0: 5c72 5c6e 5c74 5c74 3c2f 6469 763e 5c72  \r\n\t\t</div>\r
-000131c0: 5c6e 5c72 5c6e 5c74 5c74 3c64 6976 2063  \n\r\n\t\t<div c
-000131d0: 6c61 7373 3d5c 2263 6f6c 2d6d 642d 330a  lass=\"col-md-3.
-000131e0: 2020 2020 2020 2020 616b 702d 6275 7474          akp-butt
-000131f0: 6f6e 735c 223e 5c72 5c6e 5c74 5c74 5c74  ons\">\r\n\t\t\t
-00013200: 3c62 7574 746f 6e20 636c 6173 733d 5c22  <button class=\"
-00013210: 616b 702d 6c6f 6361 7469 6f6e 2d62 7574  akp-location-but
-00013220: 746f 6e20 6274 6e20 6274 6e2d 7072 696d  ton btn btn-prim
-00013230: 6172 790a 2020 2020 2020 2020 6274 6e2d  ary.        btn-
-00013240: 626c 6f63 6b5c 223e 5c72 5c6e 5c74 5c74  block\">\r\n\t\t
-00013250: 5c74 5c74 5069 7374 6565 6e20 7369 6a61  \t\tPisteen sija
-00013260: 696e 7469 202f 2056 6169 6864 6120 7069  inti / Vaihda pi
-00013270: 7374 6574 745c 7845 345c 725c 6e5c 745c  stett\xE4\r\n\t\
-00013280: 745c 743c 2f62 7574 746f 6e3e 5c72 5c6e  t\t</button>\r\n
-00013290: 5c72 5c6e 5c74 5c74 5c74 5c72 5c6e 5c74  \r\n\t\t\t\r\n\t
-000132a0: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-000132b0: 2063 6c61 7373 3d5c 2274 6578 742d 656c   class=\"text-el
-000132c0: 656d 656e 745c 223e 566f 6974 2070 5c78  ement\">Voit p\x
-000132d0: 4534 5c78 4534 7474 5c78 4534 5c78 4534  E4\xE4tt\xE4\xE4
-000132e0: 206b 6f68 7465 656e 206a 5c78 4534 7465   kohteen j\xE4te
-000132f0: 6875 6f6c 6c6f 6e20 7461 690a 2020 2020  huollon tai.    
-00013300: 2020 2020 6d75 7574 7461 6120 6a5c 7845      muuttaa j\xE
-00013310: 3474 6568 756f 6c6c 6f6e 206c 6969 7474  4tehuollon liitt
-00013320: 796d 6973 7461 7061 6120 3c61 2068 7265  ymistapaa <a hre
-00013330: 663d 5c22 235c 2220 6461 7461 2d61 6374  f=\"#\" data-act
-00013340: 696f 6e3d 5c22 676f 2d74 6f2d 6375 7374  ion=\"go-to-cust
-00013350: 6f6d 6572 2d64 6174 615c 223e 6b6f 6874  omer-data\">koht
-00013360: 6565 6e0a 2020 2020 2020 2020 7469 6564  een.        tied
-00013370: 6f74 202d 765c 7845 346c 696c 6568 6465  ot -v\xE4lilehde
-00013380: 6c6c 5c78 4534 3c2f 613e 2e3c 2f64 6976  ll\xE4</a>.</div
-00013390: 3e5c 725c 6e5c 745c 745c 745c 725c 6e5c  >\r\n\t\t\t\r\n\
-000133a0: 725c 6e5c 745c 745c 745c 725c 6e5c 745c  r\n\t\t\t\r\n\t\
-000133b0: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
-000133c0: 725c 6e5c 725c 6e5c 745c 745c 725c 6e5c  r\n\r\n\t\t\r\n\
-000133d0: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
-000133e0: 745c 725c 6e5c 745c 743c 610a 2020 2020  t\r\n\t\t<a.    
-000133f0: 2020 2020 636c 6173 733d 5c22 6d61 6b65      class=\"make
-00013400: 2d63 6861 6e67 6573 5c22 3e5c 725c 6e5c  -changes\">\r\n\
-00013410: 745c 745c 743c 7370 616e 3e5c 725c 6e5c  t\t\t<span>\r\n\
-00013420: 745c 745c 745c 7454 6565 206d 7575 746f  t\t\t\tTee muuto
-00013430: 6b73 6961 2070 616c 7665 6c75 756e 5c72  ksia palveluun\r
-00013440: 5c6e 5c74 5c74 5c74 3c2f 7370 616e 3e5c  \n\t\t\t</span>\
-00013450: 725c 6e5c 745c 743c 2f61 3e5c 725c 6e5c  r\n\t\t</a>\r\n\
-00013460: 745c 745c 725c 6e5c 745c 745c 725c 6e5c  t\t\r\n\t\t\r\n\
-00013470: 725c 6e5c 743c 2f64 6976 3e5c 725c 6e5c  r\n\t</div>\r\n\
-00013480: 725c 6e3c 2f66 6965 6c64 7365 743e 5c72  r\n</fieldset>\r
-00013490: 5c6e 3c2f 7363 7269 7074 3e5c 725c 6e5c  \n</script>\r\n\
-000134a0: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
-000134b0: 2020 2069 643d 5c22 6b69 6d70 7061 2d6f     id=\"kimppa-o
-000134c0: 7361 6b61 732d 6564 6974 6f72 2d74 656d  sakas-editor-tem
-000134d0: 706c 6174 655c 2220 7479 7065 3d5c 2274  plate\" type=\"t
-000134e0: 6578 742f 782d 7465 6d70 6c61 7465 5c22  ext/x-template\"
-000134f0: 3e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  >\r\n\r\n\r\n\r\
-00013500: 6e5c 725c 6e3c 6469 760a 2020 2020 2020  n\r\n<div.      
-00013510: 2020 636c 6173 733d 5c22 6f73 616b 6173    class=\"osakas
-00013520: 2d65 6469 746f 725c 223e 5c72 5c6e 5c74  -editor\">\r\n\t
-00013530: 3c64 6976 2063 6c61 7373 3d5c 2263 6f6e  <div class=\"con
-00013540: 7461 696e 6572 2d66 6c75 6964 5c22 3e5c  tainer-fluid\">\
-00013550: 725c 6e5c 745c 743c 666f 726d 3e5c 725c  r\n\t\t<form>\r\
-00013560: 6e5c 745c 745c 743c 6469 760a 2020 2020  n\t\t\t<div.    
-00013570: 2020 2020 636c 6173 733d 5c22 726f 7720      class=\"row 
-00013580: 626f 7264 6572 2d62 6f74 746f 6d5c 223e  border-bottom\">
-00013590: 5c72 5c6e 5c74 5c74 5c74 5c74 3c64 6976  \r\n\t\t\t\t<div
-000135a0: 2063 6c61 7373 3d5c 2263 6f6c 2d6d 642d   class=\"col-md-
-000135b0: 3132 5c22 3e5c 725c 6e5c 745c 745c 745c  12\">\r\n\t\t\t\
-000135c0: 745c 743c 6832 3e55 7573 690a 2020 2020  t\t<h2>Uusi.    
-000135d0: 2020 2020 6f73 616b 6173 3c2f 6832 3e5c      osakas</h2>\
-000135e0: 725c 6e5c 745c 745c 745c 743c 2f64 6976  r\n\t\t\t\t</div
-000135f0: 3e5c 725c 6e5c 745c 745c 743c 2f64 6976  >\r\n\t\t\t</div
-00013600: 3e5c 725c 6e5c 725c 6e5c 745c 745c 743c  >\r\n\r\n\t\t\t<
-00013610: 6469 7620 636c 6173 733d 5c22 726f 770a  div class=\"row.
-00013620: 2020 2020 2020 2020 626f 7264 6572 2d62          border-b
-00013630: 6f74 746f 6d5c 223e 5c72 5c6e 5c74 5c74  ottom\">\r\n\t\t
-00013640: 5c74 5c74 3c66 6965 6c64 7365 7420 636c  \t\t<fieldset cl
-00013650: 6173 733d 5c22 6669 656c 6473 6574 206d  ass=\"fieldset m
-00013660: 6172 6769 6e2d 626f 7474 6f6d 2d31 355c  argin-bottom-15\
-00013670: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
-00013680: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
-00013690: 7373 3d5c 2263 6f6c 2d6d 642d 3132 5c22  ss=\"col-md-12\"
-000136a0: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-000136b0: 743c 6c65 6765 6e64 3e4b 6969 6e74 6569  t<legend>Kiintei
-000136c0: 7374 5c78 4636 6e20 7469 6564 6f74 3c2f  st\xF6n tiedot</
-000136d0: 6c65 6765 6e64 3e5c 725c 6e5c 745c 745c  legend>\r\n\t\t\
-000136e0: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
-000136f0: 745c 745c 745c 745c 743c 6469 760a 2020  t\t\t\t\t<div.  
-00013700: 2020 2020 2020 636c 6173 733d 5c22 636f        class=\"co
-00013710: 6c2d 6d64 2d36 5c22 3e5c 725c 6e5c 745c  l-md-6\">\r\n\t\
-00013720: 745c 745c 745c 745c 743c 6469 7620 636c  t\t\t\t\t<div cl
-00013730: 6173 733d 5c22 666f 726d 2d67 726f 7570  ass=\"form-group
-00013740: 2072 6571 7569 7265 645c 223e 5c72 5c6e   required\">\r\n
-00013750: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c6c  \t\t\t\t\t\t\t<l
-00013760: 6162 656c 0a20 2020 2020 2020 2066 6f72  abel.        for
-00013770: 3d5c 226f 7361 6b61 732e 6b75 6e74 6174  =\"osakas.kuntat
-00013780: 756e 6e75 735c 223e 4b75 6e74 613c 2f6c  unnus\">Kunta</l
-00013790: 6162 656c 3e20 5c72 5c6e 5c74 5c74 5c74  abel> \r\n\t\t\t
-000137a0: 5c74 5c74 5c74 5c74 3c64 6976 2063 6c61  \t\t\t\t<div cla
-000137b0: 7373 3d5c 2273 656c 6563 745c 223e 5c72  ss=\"select\">\r
-000137c0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-000137d0: 5c74 3c73 656c 6563 740a 2020 2020 2020  \t<select.      
-000137e0: 2020 6964 3d5c 226f 7361 6b61 732e 6b75    id=\"osakas.ku
-000137f0: 6e74 6174 756e 6e75 735c 2220 6e61 6d65  ntatunnus\" name
-00013800: 3d5c 226f 7361 6b61 732e 6b75 6e74 6174  =\"osakas.kuntat
-00013810: 756e 6e75 735c 2220 636c 6173 733d 5c22  unnus\" class=\"
-00013820: 666f 726d 2d63 6f6e 7472 6f6c 5c22 0a20  form-control\". 
-00013830: 2020 2020 2020 2072 6571 7569 7265 643e         required>
-00013840: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-00013850: 5c74 5c74 5c74 3c6f 7074 696f 6e20 7661  \t\t\t<option va
-00013860: 6c75 653d 5c22 5c22 3e2d 2d20 5661 6c69  lue=\"\">-- Vali
-00013870: 7473 6520 2d2d 3c2f 6f70 7469 6f6e 3e5c  tse --</option>\
-00013880: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
-00013890: 745c 743c 2f73 656c 6563 743e 5c72 5c6e  t\t</select>\r\n
-000138a0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \t\t\t\t\t\t\t</
-000138b0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
-000138c0: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-000138d0: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
-000138e0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c72 5c6e  \n\t\t\t\t\t\r\n
-000138f0: 5c74 5c74 5c74 5c74 5c74 5c74 3c64 6976  \t\t\t\t\t\t<div
-00013900: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
-00013910: 2263 6f6c 2d6d 642d 365c 223e 5c72 5c6e  "col-md-6\">\r\n
-00013920: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c64  \t\t\t\t\t\t\t<d
-00013930: 6976 2063 6c61 7373 3d5c 2266 6f72 6d2d  iv class=\"form-
-00013940: 6772 6f75 705c 223e 5c72 5c6e 5c74 5c74  group\">\r\n\t\t
-00013950: 5c74 5c74 5c74 5c74 5c74 5c74 3c6c 6162  \t\t\t\t\t\t<lab
-00013960: 656c 0a20 2020 2020 2020 2066 6f72 3d5c  el.        for=\
-00013970: 226f 7361 6b61 732e 6b69 696e 7472 656b  "osakas.kiintrek
-00013980: 7475 6e6e 7573 5c22 3e4b 6969 6e74 6569  tunnus\">Kiintei
-00013990: 7374 5c78 4636 7265 6b69 7374 6572 6974  st\xF6rekisterit
-000139a0: 756e 6e75 733c 2f6c 6162 656c 3e20 5c72  unnus</label> \r
-000139b0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-000139c0: 5c74 3c69 6e70 7574 0a20 2020 2020 2020  \t<input.       
-000139d0: 2074 7970 653d 5c22 7465 7874 5c22 206e   type=\"text\" n
-000139e0: 616d 653d 5c22 6f73 616b 6173 2e6b 6969  ame=\"osakas.kii
-000139f0: 6e74 7265 6b74 756e 6e75 735c 2220 636c  ntrektunnus\" cl
-00013a00: 6173 733d 5c22 666f 726d 2d63 6f6e 7472  ass=\"form-contr
-00013a10: 6f6c 5c22 206d 6178 6c65 6e67 7468 3d5c  ol\" maxlength=\
-00013a20: 2232 335c 220a 2020 2020 2020 2020 3e5c  "23\".        >\
-00013a30: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
-00013a40: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
-00013a50: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
-00013a60: 6e5c 745c 745c 745c 745c 745c 725c 6e5c  n\t\t\t\t\t\r\n\
-00013a70: 745c 745c 745c 743c 2f66 6965 6c64 7365  t\t\t\t</fieldse
-00013a80: 743e 5c72 5c6e 5c74 5c74 5c74 3c2f 6469  t>\r\n\t\t\t</di
-00013a90: 763e 5c72 5c6e 5c72 5c6e 5c74 5c74 5c74  v>\r\n\r\n\t\t\t
-00013aa0: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
-00013ab0: 7373 3d5c 2272 6f77 2062 6f72 6465 722d  ss=\"row border-
-00013ac0: 626f 7474 6f6d 5c22 3e5c 725c 6e5c 745c  bottom\">\r\n\t\
-00013ad0: 745c 745c 743c 6669 656c 6473 6574 2063  t\t\t<fieldset c
-00013ae0: 6c61 7373 3d5c 2263 6f6c 2d6d 642d 3620  lass=\"col-md-6 
-00013af0: 7265 7175 6972 6564 5c22 3e5c 725c 6e5c  required\">\r\n\
-00013b00: 745c 745c 745c 745c 743c 6469 763e 5c72  t\t\t\t\t<div>\r
-00013b10: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c6c  \n\t\t\t\t\t\t<l
-00013b20: 6567 656e 643e 4b69 696e 7465 6973 745c  egend>Kiinteist\
-00013b30: 7846 366e 0a20 2020 2020 2020 206b 5c78  xF6n.        k\x
-00013b40: 4534 7974 745c 7846 3674 6172 6b6f 6974  E4ytt\xF6tarkoit
-00013b50: 7573 3c2f 6c65 6765 6e64 3e5c 725c 6e5c  us</legend>\r\n\
-00013b60: 745c 745c 745c 745c 743c 2f64 6976 3e5c  t\t\t\t\t</div>\
-00013b70: 725c 6e5c 745c 745c 745c 745c 743c 6469  r\n\t\t\t\t\t<di
-00013b80: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  v>\r\n\t\t\t\t\t
-00013b90: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
-00013ba0: 6c61 7373 3d5c 2266 6f72 6d2d 6772 6f75  lass=\"form-grou
-00013bb0: 705c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  p\">\r\n\t\t\t\t
-00013bc0: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
-00013bd0: 3d5c 2273 656c 6563 745c 223e 5c72 5c6e  =\"select\">\r\n
-00013be0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-00013bf0: 3c73 656c 6563 740a 2020 2020 2020 2020  <select.        
-00013c00: 6461 7461 2d72 6f6c 653d 5c22 6b61 7974  data-role=\"kayt
-00013c10: 746f 7461 726b 6f69 7475 732d 6b61 7465  totarkoitus-kate
-00013c20: 676f 7269 615c 2220 636c 6173 733d 5c22  goria\" class=\"
-00013c30: 666f 726d 2d63 6f6e 7472 6f6c 5c22 2072  form-control\" r
-00013c40: 6571 7569 7265 6420 3e5c 725c 6e5c 745c  equired >\r\n\t\
-00013c50: 745c 745c 745c 745c 745c 745c 745c 743c  t\t\t\t\t\t\t\t<
-00013c60: 6f70 7469 6f6e 0a20 2020 2020 2020 2076  option.        v
-00013c70: 616c 7565 3d5c 225c 223e 3c2f 6f70 7469  alue=\"\"></opti
-00013c80: 6f6e 3e5c 725c 6e5c 745c 745c 745c 745c  on>\r\n\t\t\t\t\
-00013c90: 745c 745c 745c 745c 743c 6f70 7469 6f6e  t\t\t\t\t<option
-00013ca0: 2076 616c 7565 3d5c 2230 5c22 3e56 616b   value=\"0\">Vak
-00013cb0: 6974 7569 6e65 6e20 6173 756e 746f 3c2f  ituinen asunto</
-00013cc0: 6f70 7469 6f6e 3e5c 725c 6e5c 745c 745c  option>\r\n\t\t\
-00013cd0: 745c 745c 745c 745c 745c 745c 743c 6f70  t\t\t\t\t\t\t<op
-00013ce0: 7469 6f6e 0a20 2020 2020 2020 2076 616c  tion.        val
-00013cf0: 7565 3d5c 2231 5c22 3e56 6170 6161 2d61  ue=\"1\">Vapaa-a
-00013d00: 6a61 6e20 6173 756e 746f 3c2f 6f70 7469  jan asunto</opti
-00013d10: 6f6e 3e5c 725c 6e5c 745c 745c 745c 745c  on>\r\n\t\t\t\t\
-00013d20: 745c 745c 745c 745c 743c 6f70 7469 6f6e  t\t\t\t\t<option
-00013d30: 2076 616c 7565 3d5c 2232 5c22 3e54 616c   value=\"2\">Tal
-00013d40: 6f79 6874 695c 7846 363c 2f6f 7074 696f  oyhti\xF6</optio
-00013d50: 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  n>\r\n\t\t\t\t\t
-00013d60: 5c74 5c74 5c74 5c74 3c6f 7074 696f 6e0a  \t\t\t\t<option.
-00013d70: 2020 2020 2020 2020 7661 6c75 653d 5c22          value=\"
-00013d80: 335c 223e 5972 6974 7973 3c2f 6f70 7469  3\">Yritys</opti
-00013d90: 6f6e 3e5c 725c 6e5c 745c 745c 745c 745c  on>\r\n\t\t\t\t\
-00013da0: 745c 745c 745c 745c 743c 6f70 7469 6f6e  t\t\t\t\t<option
-00013db0: 2076 616c 7565 3d5c 2234 5c22 3e59 6874   value=\"4\">Yht
-00013dc0: 6569 735c 7846 363c 2f6f 7074 696f 6e3e  eis\xF6</option>
-00013dd0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-00013de0: 5c74 5c74 3c2f 7365 6c65 6374 3e5c 725c  \t\t</select>\r\
-00013df0: 6e5c 745c 745c 745c 745c 745c 745c 743c  n\t\t\t\t\t\t\t<
-00013e00: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
-00013e10: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
-00013e20: 725c 6e5c 745c 745c 745c 745c 745c 743c  r\n\t\t\t\t\t\t<
-00013e30: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-00013e40: 733d 5c22 666f 726d 2d67 726f 7570 5c22  s=\"form-group\"
-00013e50: 203e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74   >\r\n\t\t\t\t\t
-00013e60: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
-00013e70: 2273 656c 6563 745c 223e 5c72 5c6e 5c74  "select\">\r\n\t
-00013e80: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c73  \t\t\t\t\t\t\t<s
-00013e90: 656c 6563 740a 2020 2020 2020 2020 6e61  elect.        na
-00013ea0: 6d65 3d5c 226f 7361 6b61 732e 6b61 7974  me=\"osakas.kayt
-00013eb0: 746f 7461 726b 6f69 7475 735c 2220 636c  totarkoitus\" cl
-00013ec0: 6173 733d 5c22 666f 726d 2d63 6f6e 7472  ass=\"form-contr
-00013ed0: 6f6c 5c22 2072 6571 7569 7265 6420 3e5c  ol\" required >\
-00013ee0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
-00013ef0: 745c 745c 743c 6f70 7469 6f6e 0a20 2020  t\t\t<option.   
-00013f00: 2020 2020 2076 616c 7565 3d5c 225c 223e       value=\"\">
-00013f10: 3c2f 6f70 7469 6f6e 3e5c 725c 6e5c 745c  </option>\r\n\t\
-00013f20: 745c 745c 745c 745c 745c 745c 745c 743c  t\t\t\t\t\t\t\t<
-00013f30: 6f70 7469 6f6e 2076 616c 7565 3d5c 2230  option value=\"0
-00013f40: 3131 5c22 2064 6174 612d 6b61 7465 676f  11\" data-katego
-00013f50: 7269 613d 5c22 305c 223e 5968 6465 6e0a  ria=\"0\">Yhden.
-00013f60: 2020 2020 2020 2020 6173 756e 6e6f 6e20          asunnon 
-00013f70: 7461 6c6f 3c2f 6f70 7469 6f6e 3e5c 725c  talo</option>\r\
-00013f80: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
-00013f90: 745c 743c 6f70 7469 6f6e 2076 616c 7565  t\t<option value
-00013fa0: 3d5c 2230 3132 5c22 2064 6174 612d 6b61  =\"012\" data-ka
-00013fb0: 7465 676f 7269 613d 5c22 305c 223e 4b61  tegoria=\"0\">Ka
-00013fc0: 6864 656e 0a20 2020 2020 2020 2061 7375  hden.        asu
-00013fd0: 6e6e 6f6e 2074 616c 6f3c 2f6f 7074 696f  nnon talo</optio
-00013fe0: 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  n>\r\n\t\t\t\t\t
-00013ff0: 5c74 5c74 5c74 5c74 3c6f 7074 696f 6e20  \t\t\t\t<option 
-00014000: 7661 6c75 653d 5c22 3031 335c 2220 6461  value=\"013\" da
-00014010: 7461 2d6b 6174 6567 6f72 6961 3d5c 2230  ta-kategoria=\"0
-00014020: 5c22 3e4d 7575 0a20 2020 2020 2020 2065  \">Muu.        e
-00014030: 7269 6c6c 696e 656e 2070 6965 6e74 616c  rillinen piental
-00014040: 6f3c 2f6f 7074 696f 6e3e 5c72 5c6e 5c74  o</option>\r\n\t
-00014050: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-00014060: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-00014070: 5c74 5c74 5c74 3c6f 7074 696f 6e0a 2020  \t\t\t<option.  
-00014080: 2020 2020 2020 7661 6c75 653d 5c22 3034        value=\"04
-00014090: 315c 2220 6461 7461 2d6b 6174 6567 6f72  1\" data-kategor
-000140a0: 6961 3d5c 2231 5c22 3e4b 6573 5c78 4534  ia=\"1\">Kes\xE4
-000140b0: 6d5c 7846 366b 6b69 2074 6169 2076 6170  m\xF6kki tai vap
-000140c0: 6161 2d61 6a61 6e20 6173 756e 746f 3c2f  aa-ajan asunto</
-000140d0: 6f70 7469 6f6e 3e5c 725c 6e5c 745c 745c  option>\r\n\t\t\
-000140e0: 745c 745c 745c 745c 745c 745c 743c 6f70  t\t\t\t\t\t\t<op
-000140f0: 7469 6f6e 0a20 2020 2020 2020 2076 616c  tion.        val
-00014100: 7565 3d5c 2239 3331 5c22 2064 6174 612d  ue=\"931\" data-
-00014110: 6b61 7465 676f 7269 613d 5c22 315c 223e  kategoria=\"1\">
-00014120: 5361 756e 6172 616b 656e 6e75 733c 2f6f  Saunarakennus</o
-00014130: 7074 696f 6e3e 5c72 5c6e 5c74 5c74 5c74  ption>\r\n\t\t\t
-00014140: 5c74 5c74 5c74 5c74 5c74 5c74 5c72 5c6e  \t\t\t\t\t\t\r\n
-00014150: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-00014160: 5c74 3c6f 7074 696f 6e0a 2020 2020 2020  \t<option.      
-00014170: 2020 7661 6c75 653d 5c22 3032 315c 2220    value=\"021\" 
-00014180: 6461 7461 2d6b 6174 6567 6f72 6961 3d5c  data-kategoria=\
-00014190: 2232 5c22 3e52 6976 6974 616c 6f3c 2f6f  "2\">Rivitalo</o
-000141a0: 7074 696f 6e3e 5c72 5c6e 5c74 5c74 5c74  ption>\r\n\t\t\t
-000141b0: 5c74 5c74 5c74 5c74 5c74 5c74 3c6f 7074  \t\t\t\t\t\t<opt
-000141c0: 696f 6e0a 2020 2020 2020 2020 7661 6c75  ion.        valu
-000141d0: 653d 5c22 3032 325c 2220 6461 7461 2d6b  e=\"022\" data-k
-000141e0: 6174 6567 6f72 6961 3d5c 2232 5c22 3e4b  ategoria=\"2\">K
-000141f0: 6574 6a75 7461 6c6f 3c2f 6f70 7469 6f6e  etjutalo</option
-00014200: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-00014210: 745c 745c 745c 743c 6f70 7469 6f6e 0a20  t\t\t\t<option. 
-00014220: 2020 2020 2020 2076 616c 7565 3d5c 2230         value=\"0
-00014230: 3332 5c22 2064 6174 612d 6b61 7465 676f  32\" data-katego
-00014240: 7269 613d 5c22 325c 223e 4c75 6874 6974  ria=\"2\">Luhtit
-00014250: 616c 6f3c 2f6f 7074 696f 6e3e 5c72 5c6e  alo</option>\r\n
-00014260: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-00014270: 5c74 3c6f 7074 696f 6e0a 2020 2020 2020  \t<option.      
-00014280: 2020 7661 6c75 653d 5c22 3033 395c 2220    value=\"039\" 
-00014290: 6461 7461 2d6b 6174 6567 6f72 6961 3d5c  data-kategoria=\
-000142a0: 2232 5c22 3e4b 6572 726f 7374 616c 6f3c  "2\">Kerrostalo<
-000142b0: 2f6f 7074 696f 6e3e 5c72 5c6e 5c74 5c74  /option>\r\n\t\t
-000142c0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c72  \t\t\t\t\t\t\t\r
-000142d0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-000142e0: 5c74 5c74 3c6f 7074 696f 6e0a 2020 2020  \t\t<option.    
-000142f0: 2020 2020 7661 6c75 653d 5c22 3131 315c      value=\"111\
-00014300: 2220 6461 7461 2d6b 6174 6567 6f72 6961  " data-kategoria
-00014310: 3d5c 2233 5c22 3e59 7269 7479 733c 2f6f  =\"3\">Yritys</o
-00014320: 7074 696f 6e3e 5c72 5c6e 5c74 5c74 5c74  ption>\r\n\t\t\t
-00014330: 5c74 5c74 5c74 5c74 5c74 5c74 5c72 5c6e  \t\t\t\t\t\t\r\n
-00014340: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
-00014350: 5c74 3c6f 7074 696f 6e0a 2020 2020 2020  \t<option.      
-00014360: 2020 7661 6c75 653d 5c22 3133 315c 2220    value=\"131\" 
-00014370: 6461 7461 2d6b 6174 6567 6f72 6961 3d5c  data-kategoria=\
-00014380: 2234 5c22 3e59 6874 6569 735c 7846 363c  "4\">Yhteis\xF6<
-00014390: 2f6f 7074 696f 6e3e 5c72 5c6e 5c74 5c74  /option>\r\n\t\t
-000143a0: 5c74 5c74 5c74 5c74 5c74 5c74 3c2f 7365  \t\t\t\t\t\t</se
-000143b0: 6c65 6374 3e5c 725c 6e5c 745c 745c 745c  lect>\r\n\t\t\t\
-000143c0: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
-000143d0: 6e5c 745c 745c 745c 745c 745c 743c 2f64  n\t\t\t\t\t\t</d
-000143e0: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
-000143f0: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
-00014400: 745c 743c 2f66 6965 6c64 7365 743e 5c72  t\t</fieldset>\r
-00014410: 5c6e 5c72 5c6e 5c74 5c74 5c74 5c74 5c72  \n\r\n\t\t\t\t\r
-00014420: 5c6e 5c74 5c74 5c74 3c2f 6469 763e 5c72  \n\t\t\t</div>\r
-00014430: 5c6e 5c74 5c74 5c74 5c74 5c72 5c6e 5c74  \n\t\t\t\t\r\n\t
-00014440: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-00014450: 2063 6c61 7373 3d5c 2272 6f77 5c22 3e5c   class=\"row\">\
-00014460: 725c 6e5c 745c 745c 745c 743c 6469 7620  r\n\t\t\t\t<div 
-00014470: 636c 6173 733d 5c22 636f 6c2d 6d64 2d36  class=\"col-md-6
-00014480: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
-00014490: 743c 6669 656c 6473 6574 0a20 2020 2020  t<fieldset.     
-000144a0: 2020 2063 6c61 7373 3d5c 2266 6965 6c64     class=\"field
-000144b0: 7365 7420 6d61 7267 696e 2d62 6f74 746f  set margin-botto
-000144c0: 6d2d 3135 5c22 3e5c 725c 6e5c 745c 745c  m-15\">\r\n\t\t\
-000144d0: 745c 745c 745c 743c 6c65 6765 6e64 3e4f  t\t\t\t<legend>O
-000144e0: 7361 6b6b 6161 6e20 7469 6564 6f74 3c2f  sakkaan tiedot</
-000144f0: 6c65 6765 6e64 3e5c 725c 6e5c 745c 745c  legend>\r\n\t\t\
-00014500: 745c 745c 745c 743c 6469 760a 2020 2020  t\t\t\t<div.    
-00014510: 2020 2020 636c 6173 733d 5c22 6368 6563      class=\"chec
-00014520: 6b62 6f78 2069 6e76 6973 6962 6c65 5c22  kbox invisible\"
-00014530: 3e3c 6c61 6265 6c3e 3c2f 6c61 6265 6c3e  ><label></label>
-00014540: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
-00014550: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
-00014560: 3d5c 2266 6f72 6d2d 6772 6f75 700a 2020  =\"form-group.  
-00014570: 2020 2020 2020 7265 7175 6972 6564 5c22        required\"
-00014580: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-00014590: 745c 743c 6c61 6265 6c20 666f 723d 5c22  t\t<label for=\"
-000145a0: 6f73 616b 6173 2e6e 696d 695c 223e 4f73  osakas.nimi\">Os
-000145b0: 616b 6b61 616e 206e 696d 693c 2f6c 6162  akkaan nimi</lab
-000145c0: 656c 3e0a 2020 2020 2020 2020 5c72 5c6e  el>.        \r\n
-000145d0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c69  \t\t\t\t\t\t\t<i
-000145e0: 6e70 7574 2072 6571 7569 7265 6420 7479  nput required ty
-000145f0: 7065 3d5c 2274 6578 745c 2220 6e61 6d65  pe=\"text\" name
-00014600: 3d5c 226f 7361 6b61 732e 6e69 6d69 5c22  =\"osakas.nimi\"
-00014610: 2063 6c61 7373 3d5c 2266 6f72 6d2d 636f   class=\"form-co
-00014620: 6e74 726f 6c5c 220a 2020 2020 2020 2020  ntrol\".        
-00014630: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-00014640: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
-00014650: 745c 745c 745c 743c 6469 7620 636c 6173  t\t\t\t<div clas
-00014660: 733d 5c22 666f 726d 2d67 726f 7570 2072  s=\"form-group r
-00014670: 6571 7569 7265 645c 223e 5c72 5c6e 5c74  equired\">\r\n\t
-00014680: 5c74 5c74 5c74 5c74 5c74 5c74 3c6c 6162  \t\t\t\t\t\t<lab
-00014690: 656c 0a20 2020 2020 2020 2066 6f72 3d5c  el.        for=\
-000146a0: 226f 7361 6b61 732e 6574 756e 696d 695c  "osakas.etunimi\
-000146b0: 223e 4f73 616b 6b61 616e 2065 7475 6e69  ">Osakkaan etuni
-000146c0: 6d69 3c2f 6c61 6265 6c3e 5c72 5c6e 5c74  mi</label>\r\n\t
-000146d0: 5c74 5c74 5c74 5c74 5c74 5c74 3c69 6e70  \t\t\t\t\t\t<inp
-000146e0: 7574 2072 6571 7569 7265 640a 2020 2020  ut required.    
-000146f0: 2020 2020 7479 7065 3d5c 2274 6578 745c      type=\"text\
-00014700: 2220 6e61 6d65 3d5c 226f 7361 6b61 732e  " name=\"osakas.
-00014710: 6574 756e 696d 695c 2220 636c 6173 733d  etunimi\" class=
-00014720: 5c22 666f 726d 2d63 6f6e 7472 6f6c 5c22  \"form-control\"
-00014730: 203e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74   >\r\n\t\t\t\t\t
-00014740: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
-00014750: 5c74 5c74 5c74 5c74 3c64 6976 0a20 2020  \t\t\t\t<div.   
-00014760: 2020 2020 2063 6c61 7373 3d5c 2266 6f72       class=\"for
-00014770: 6d2d 6772 6f75 7020 7265 7175 6972 6564  m-group required
-00014780: 5c22 2073 7479 6c65 3d5c 2264 6973 706c  \" style=\"displ
-00014790: 6179 3a6e 6f6e 655c 223e 5c72 5c6e 5c74  ay:none\">\r\n\t
-000147a0: 5c74 5c74 5c74 5c74 5c74 5c74 3c6c 6162  \t\t\t\t\t\t<lab
-000147b0: 656c 0a20 2020 2020 2020 2066 6f72 3d5c  el.        for=\
-000147c0: 226f 7361 6b61 732e 7375 6b75 6e69 6d69  "osakas.sukunimi
-000147d0: 5c22 3e4f 7361 6b6b 6161 6e20 7375 6b75  \">Osakkaan suku
-000147e0: 6e69 6d69 3c2f 6c61 6265 6c3e 5c72 5c6e  nimi</label>\r\n
-000147f0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c69  \t\t\t\t\t\t\t<i
-00014800: 6e70 7574 0a20 2020 2020 2020 2072 6571  nput.        req
-00014810: 7569 7265 6420 7479 7065 3d5c 2274 6578  uired type=\"tex
-00014820: 745c 2220 6e61 6d65 3d5c 226f 7361 6b61  t\" name=\"osaka
-00014830: 732e 7375 6b75 6e69 6d69 5c22 2063 6c61  s.sukunimi\" cla
-00014840: 7373 3d5c 2266 6f72 6d2d 636f 6e74 726f  ss=\"form-contro
-00014850: 6c5c 2220 3e5c 725c 6e5c 745c 745c 745c  l\" >\r\n\t\t\t\
-00014860: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
-00014870: 745c 745c 745c 745c 745c 743c 6469 760a  t\t\t\t\t\t<div.
-00014880: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-00014890: 666f 726d 2d67 726f 7570 5c22 3e5c 725c  form-group\">\r\
-000148a0: 6e5c 745c 745c 745c 745c 745c 745c 743c  n\t\t\t\t\t\t\t<
-000148b0: 6c61 6265 6c20 666f 723d 5c22 6f73 616b  label for=\"osak
-000148c0: 6173 2e79 6874 6579 7368 656e 6b5c 223e  as.yhteyshenk\">
-000148d0: 5968 7465 7973 6865 6e6b 696c 5c78 4636  Yhteyshenkil\xF6
-000148e0: 3c2f 6c61 6265 6c3e 5c72 5c6e 5c74 5c74  </label>\r\n\t\t
-000148f0: 5c74 5c74 5c74 5c74 5c74 3c69 6e70 7574  \t\t\t\t\t<input
-00014900: 0a20 2020 2020 2020 2074 7970 653d 5c22  .        type=\"
-00014910: 7465 7874 5c22 206e 616d 653d 5c22 6f73  text\" name=\"os
-00014920: 616b 6173 2e79 6874 6579 7368 656e 6b5c  akas.yhteyshenk\
-00014930: 2220 636c 6173 733d 5c22 666f 726d 2d63  " class=\"form-c
-00014940: 6f6e 7472 6f6c 5c22 203e 5c72 5c6e 5c74  ontrol\" >\r\n\t
-00014950: 5c74 5c74 5c74 5c74 5c74 3c2f 6469 763e  \t\t\t\t\t</div>
-00014960: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-00014970: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
-00014980: 7373 3d5c 2266 6f72 6d2d 6772 6f75 7020  ss=\"form-group 
-00014990: 7265 7175 6972 6564 5c22 3e5c 725c 6e5c  required\">\r\n\
-000149a0: 745c 745c 745c 745c 745c 745c 743c 6c61  t\t\t\t\t\t\t<la
-000149b0: 6265 6c20 666f 723d 5c22 6f73 616b 6173  bel for=\"osakas
-000149c0: 2e6b 6174 755c 223e 4b69 696e 7465 6973  .katu\">Kiinteis
-000149d0: 745c 7846 366e 0a20 2020 2020 2020 206f  t\xF6n.        o
-000149e0: 736f 6974 653c 2f6c 6162 656c 3e20 5c72  soite</label> \r
-000149f0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-00014a00: 3c69 6e70 7574 2072 6571 7569 7265 6420  <input required 
-00014a10: 7479 7065 3d5c 2274 6578 745c 2220 6e61  type=\"text\" na
-00014a20: 6d65 3d5c 226f 7361 6b61 732e 6b61 7475  me=\"osakas.katu
-00014a30: 5c22 0a20 2020 2020 2020 2063 6c61 7373  \".        class
-00014a40: 3d5c 2266 6f72 6d2d 636f 6e74 726f 6c5c  =\"form-control\
-00014a50: 2220 3e5c 725c 6e5c 745c 745c 745c 745c  " >\r\n\t\t\t\t\
-00014a60: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
-00014a70: 745c 745c 745c 745c 743c 6469 7620 636c  t\t\t\t\t<div cl
-00014a80: 6173 733d 5c22 666f 726d 2d67 726f 7570  ass=\"form-group
-00014a90: 0a20 2020 2020 2020 2072 6571 7569 7265  .        require
-00014aa0: 645c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  d\">\r\n\t\t\t\t
-00014ab0: 5c74 5c74 5c74 3c6c 6162 656c 2066 6f72  \t\t\t<label for
-00014ac0: 3d5c 226f 7361 6b61 732e 706f 7374 695c  =\"osakas.posti\
-00014ad0: 223e 506f 7374 696e 756d 6572 6f20 6a61  ">Postinumero ja
-00014ae0: 202d 746f 696d 6970 6169 6b6b 613c 2f6c   -toimipaikka</l
-00014af0: 6162 656c 3e0a 2020 2020 2020 2020 5c72  abel>.        \r
-00014b00: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-00014b10: 3c69 6e70 7574 2072 6571 7569 7265 6420  <input required 
-00014b20: 7479 7065 3d5c 2274 6578 745c 2220 6e61  type=\"text\" na
-00014b30: 6d65 3d5c 226f 7361 6b61 732e 706f 7374  me=\"osakas.post
-00014b40: 695c 2220 636c 6173 733d 5c22 666f 726d  i\" class=\"form
-00014b50: 2d63 6f6e 7472 6f6c 5c22 0a20 2020 2020  -control\".     
-00014b60: 2020 203e 5c72 5c6e 5c74 5c74 5c74 5c74     >\r\n\t\t\t\t
-00014b70: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-00014b80: 5c74 5c74 5c74 5c74 5c74 5c72 5c6e 5c74  \t\t\t\t\t\r\n\t
-00014b90: 5c74 5c74 5c74 5c74 5c74 5c72 5c6e 5c74  \t\t\t\t\t\r\n\t
-00014ba0: 5c74 5c74 5c74 5c74 5c74 5c74 3c64 6976  \t\t\t\t\t\t<div
-00014bb0: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
-00014bc0: 2266 6f72 6d2d 6772 6f75 705c 223e 5c72  "form-group\">\r
-00014bd0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-00014be0: 5c74 3c6c 6162 656c 2066 6f72 3d5c 226f  \t<label for=\"o
-00014bf0: 7361 6b61 732e 6865 6e6b 696c 6f74 756e  sakas.henkilotun
-00014c00: 6e75 7353 7472 696e 675c 223e 4865 6e6b  nusString\">Henk
-00014c10: 696c 5c78 4636 7475 6e6e 7573 2f59 2d74  il\xF6tunnus/Y-t
-00014c20: 756e 6e75 733c 2f6c 6162 656c 3e5c 725c  unnus</label>\r\
-00014c30: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
-00014c40: 743c 696e 7075 740a 2020 2020 2020 2020  t<input.        
-00014c50: 7479 7065 3d5c 2274 6578 745c 2220 6e61  type=\"text\" na
-00014c60: 6d65 3d5c 226f 7361 6b61 732e 6865 6e6b  me=\"osakas.henk
-00014c70: 696c 6f74 756e 6e75 7353 7472 696e 675c  ilotunnusString\
-00014c80: 2220 636c 6173 733d 5c22 666f 726d 2d63  " class=\"form-c
-00014c90: 6f6e 7472 6f6c 5c22 203e 5c72 5c6e 5c74  ontrol\" >\r\n\t
-00014ca0: 5c74 5c74 5c74 5c74 5c74 5c74 3c2f 6469  \t\t\t\t\t\t</di
-00014cb0: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  v>\r\n\t\t\t\t\t
-00014cc0: 5c74 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  \t\r\n\t\t\t\t\t
-00014cd0: 3c2f 6669 656c 6473 6574 3e5c 725c 6e5c  </fieldset>\r\n\
-00014ce0: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
-00014cf0: 6e5c 745c 745c 745c 743c 6469 760a 2020  n\t\t\t\t<div.  
-00014d00: 2020 2020 2020 636c 6173 733d 5c22 636f        class=\"co
-00014d10: 6c2d 6d64 2d36 5c22 3e5c 725c 6e5c 745c  l-md-6\">\r\n\t\
-00014d20: 745c 745c 745c 743c 6669 656c 6473 6574  t\t\t\t<fieldset
-00014d30: 2063 6c61 7373 3d5c 2266 6965 6c64 7365   class=\"fieldse
-00014d40: 7420 6d61 7267 696e 2d62 6f74 746f 6d2d  t margin-bottom-
-00014d50: 3135 5c22 3e5c 725c 6e5c 745c 745c 745c  15\">\r\n\t\t\t\
-00014d60: 745c 745c 743c 6c65 6765 6e64 3e4d 616b  t\t\t<legend>Mak
-00014d70: 7361 6a61 6e0a 2020 2020 2020 2020 7469  sajan.        ti
-00014d80: 6564 6f74 3c2f 6c65 6765 6e64 3e5c 725c  edot</legend>\r\
-00014d90: 6e5c 745c 745c 745c 745c 745c 743c 6469  n\t\t\t\t\t\t<di
-00014da0: 7620 636c 6173 733d 5c22 6368 6563 6b62  v class=\"checkb
-00014db0: 6f78 5c22 3e5c 725c 6e5c 745c 745c 745c  ox\">\r\n\t\t\t\
-00014dc0: 745c 745c 745c 743c 6c61 6265 6c0a 2020  t\t\t\t<label.  
-00014dd0: 2020 2020 2020 666f 723d 5c22 7361 6d65        for=\"same
-00014de0: 5f61 735f 6265 666f 7265 5c22 3e5c 725c  _as_before\">\r\
-00014df0: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
-00014e00: 743c 696e 7075 7420 7479 7065 3d5c 2263  t<input type=\"c
-00014e10: 6865 636b 626f 785c 2220 6964 3d5c 2273  heckbox\" id=\"s
-00014e20: 616d 655f 6173 5f62 6566 6f72 655c 220a  ame_as_before\".
-00014e30: 2020 2020 2020 2020 6e61 6d65 3d5c 2273          name=\"s
-00014e40: 616d 655f 6173 5f62 6566 6f72 655c 2220  ame_as_before\" 
-00014e50: 6461 7461 2d61 6374 696f 6e3d 5c22 7361  data-action=\"sa
-00014e60: 6d65 2d61 732d 6265 666f 7265 5c22 203e  me-as-before\" >
-00014e70: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-00014e80: 5c74 5c74 5361 6d61 740a 2020 2020 2020  \t\tSamat.      
-00014e90: 2020 6b75 696e 206f 7361 6b6b 6161 6e5c    kuin osakkaan\
-00014ea0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
-00014eb0: 743c 2f6c 6162 656c 3e5c 725c 6e5c 745c  t</label>\r\n\t\
-00014ec0: 745c 745c 745c 745c 743c 2f64 6976 3e5c  t\t\t\t\t</div>\
-00014ed0: 725c 6e5c 745c 745c 745c 745c 745c 743c  r\n\t\t\t\t\t\t<
-00014ee0: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-00014ef0: 733d 5c22 666f 726d 2d67 726f 7570 2072  s=\"form-group r
-00014f00: 6571 7569 7265 645c 223e 5c72 5c6e 5c74  equired\">\r\n\t
-00014f10: 5c74 5c74 5c74 5c74 5c74 5c74 3c6c 6162  \t\t\t\t\t\t<lab
-00014f20: 656c 2066 6f72 3d5c 226f 7361 6b61 732e  el for=\"osakas.
-00014f30: 6c61 736b 7574 7573 6e69 6d69 5c22 3e4d  laskutusnimi\">M
-00014f40: 616b 7361 6a61 6e0a 2020 2020 2020 2020  aksajan.        
-00014f50: 6e69 6d69 3c2f 6c61 6265 6c3e 205c 725c  nimi</label> \r\
-00014f60: 6e5c 745c 745c 745c 745c 745c 745c 743c  n\t\t\t\t\t\t\t<
-00014f70: 696e 7075 7420 7265 7175 6972 6564 2074  input required t
-00014f80: 7970 653d 5c22 7465 7874 5c22 206e 616d  ype=\"text\" nam
-00014f90: 653d 5c22 6f73 616b 6173 2e6c 6173 6b75  e=\"osakas.lasku
-00014fa0: 7475 736e 696d 695c 220a 2020 2020 2020  tusnimi\".      
-00014fb0: 2020 636c 6173 733d 5c22 666f 726d 2d63    class=\"form-c
-00014fc0: 6f6e 7472 6f6c 5c22 203e 5c72 5c6e 5c74  ontrol\" >\r\n\t
-00014fd0: 5c74 5c74 5c74 5c74 5c74 3c2f 6469 763e  \t\t\t\t\t</div>
-00014fe0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-00014ff0: 3c64 6976 2063 6c61 7373 3d5c 2266 6f72  <div class=\"for
-00015000: 6d2d 6772 6f75 700a 2020 2020 2020 2020  m-group.        
-00015010: 7265 7175 6972 6564 5c22 3e5c 725c 6e5c  required\">\r\n\
-00015020: 745c 745c 745c 745c 745c 745c 743c 6c61  t\t\t\t\t\t\t<la
-00015030: 6265 6c20 666f 723d 5c22 6f73 616b 6173  bel for=\"osakas
-00015040: 2e6c 6173 6b75 7475 7365 7475 6e69 6d69  .laskutusetunimi
-00015050: 5c22 3e4d 616b 7361 6a61 6e0a 2020 2020  \">Maksajan.    
-00015060: 2020 2020 6574 756e 696d 693c 2f6c 6162      etunimi</lab
-00015070: 656c 3e5c 725c 6e5c 745c 745c 745c 745c  el>\r\n\t\t\t\t\
-00015080: 745c 745c 743c 696e 7075 7420 7265 7175  t\t\t<input requ
-00015090: 6972 6564 2074 7970 653d 5c22 7465 7874  ired type=\"text
-000150a0: 5c22 206e 616d 653d 5c22 6f73 616b 6173  \" name=\"osakas
-000150b0: 2e6c 6173 6b75 7475 7365 7475 6e69 6d69  .laskutusetunimi
-000150c0: 5c22 0a20 2020 2020 2020 2063 6c61 7373  \".        class
-000150d0: 3d5c 2266 6f72 6d2d 636f 6e74 726f 6c5c  =\"form-control\
-000150e0: 2220 3e5c 725c 6e5c 745c 745c 745c 745c  " >\r\n\t\t\t\t\
-000150f0: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
-00015100: 745c 745c 745c 745c 743c 6469 7620 636c  t\t\t\t\t<div cl
-00015110: 6173 733d 5c22 666f 726d 2d67 726f 7570  ass=\"form-group
-00015120: 0a20 2020 2020 2020 2072 6571 7569 7265  .        require
-00015130: 645c 2220 7374 796c 653d 5c22 6469 7370  d\" style=\"disp
-00015140: 6c61 793a 6e6f 6e65 5c22 3e5c 725c 6e5c  lay:none\">\r\n\
-00015150: 745c 745c 745c 745c 745c 745c 743c 6c61  t\t\t\t\t\t\t<la
-00015160: 6265 6c20 666f 723d 5c22 6f73 616b 6173  bel for=\"osakas
-00015170: 2e6c 6173 6b75 7475 7373 756b 756e 696d  .laskutussukunim
-00015180: 695c 223e 4d61 6b73 616a 616e 0a20 2020  i\">Maksajan.   
-00015190: 2020 2020 2073 756b 756e 696d 693c 2f6c       sukunimi</l
-000151a0: 6162 656c 3e5c 725c 6e5c 745c 745c 745c  abel>\r\n\t\t\t\
-000151b0: 745c 745c 745c 743c 696e 7075 7420 7265  t\t\t\t<input re
-000151c0: 7175 6972 6564 2074 7970 653d 5c22 7465  quired type=\"te
-000151d0: 7874 5c22 206e 616d 653d 5c22 6f73 616b  xt\" name=\"osak
-000151e0: 6173 2e6c 6173 6b75 7475 7373 756b 756e  as.laskutussukun
-000151f0: 696d 695c 220a 2020 2020 2020 2020 636c  imi\".        cl
-00015200: 6173 733d 5c22 666f 726d 2d63 6f6e 7472  ass=\"form-contr
-00015210: 6f6c 5c22 203e 5c72 5c6e 5c74 5c74 5c74  ol\" >\r\n\t\t\t
-00015220: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
-00015230: 5c74 5c74 5c74 5c74 5c74 5c74 3c64 6976  \t\t\t\t\t\t<div
-00015240: 2063 6c61 7373 3d5c 2266 6f72 6d2d 6772   class=\"form-gr
-00015250: 6f75 705c 223e 5c72 5c6e 5c74 5c74 5c74  oup\">\r\n\t\t\t
-00015260: 5c74 5c74 5c74 5c74 3c6c 6162 656c 0a20  \t\t\t\t<label. 
-00015270: 2020 2020 2020 2066 6f72 3d5c 226f 7361         for=\"osa
-00015280: 6b61 732e 6c61 736b 7574 7573 7968 7465  kas.laskutusyhte
-00015290: 7973 6865 6e6b 5c22 3e4d 616b 7361 6a61  yshenk\">Maksaja
-000152a0: 6e20 7968 7465 7973 6865 6e6b 696c 5c78  n yhteyshenkil\x
-000152b0: 4636 3c2f 6c61 6265 6c3e 5c72 5c6e 5c74  F6</label>\r\n\t
-000152c0: 5c74 5c74 5c74 5c74 5c74 5c74 3c69 6e70  \t\t\t\t\t\t<inp
-000152d0: 7574 0a20 2020 2020 2020 2074 7970 653d  ut.        type=
-000152e0: 5c22 7465 7874 5c22 206e 616d 653d 5c22  \"text\" name=\"
-000152f0: 6f73 616b 6173 2e6c 6173 6b75 7475 7379  osakas.laskutusy
-00015300: 6874 6579 7368 656e 6b5c 2220 636c 6173  hteyshenk\" clas
-00015310: 733d 5c22 666f 726d 2d63 6f6e 7472 6f6c  s=\"form-control
-00015320: 5c22 203e 5c72 5c6e 5c74 5c74 5c74 5c74  \" >\r\n\t\t\t\t
-00015330: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-00015340: 5c74 5c74 5c74 5c74 5c74 3c64 6976 0a20  \t\t\t\t\t<div. 
-00015350: 2020 2020 2020 2063 6c61 7373 3d5c 2266         class=\"f
-00015360: 6f72 6d2d 6772 6f75 7020 7265 7175 6972  orm-group requir
-00015370: 6564 5c22 3e5c 725c 6e5c 745c 745c 745c  ed\">\r\n\t\t\t\
-00015380: 745c 745c 745c 743c 6c61 6265 6c20 666f  t\t\t\t<label fo
-00015390: 723d 5c22 6f73 616b 6173 2e6c 6173 6b75  r=\"osakas.lasku
-000153a0: 7475 736b 6174 755c 223e 4b69 696e 7465  tuskatu\">Kiinte
-000153b0: 6973 745c 7846 366e 0a20 2020 2020 2020  ist\xF6n.       
-000153c0: 206f 736f 6974 653c 2f6c 6162 656c 3e20   osoite</label> 
-000153d0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-000153e0: 5c74 3c69 6e70 7574 2072 6571 7569 7265  \t<input require
-000153f0: 6420 7479 7065 3d5c 2274 6578 745c 2220  d type=\"text\" 
-00015400: 6e61 6d65 3d5c 226f 7361 6b61 732e 6c61  name=\"osakas.la
-00015410: 736b 7574 7573 6b61 7475 5c22 0a20 2020  skutuskatu\".   
-00015420: 2020 2020 2063 6c61 7373 3d5c 2266 6f72       class=\"for
-00015430: 6d2d 636f 6e74 726f 6c5c 2220 3e5c 725c  m-control\" >\r\
-00015440: 6e5c 745c 745c 745c 745c 745c 743c 2f64  n\t\t\t\t\t\t</d
-00015450: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
-00015460: 745c 743c 6469 7620 636c 6173 733d 5c22  t\t<div class=\"
-00015470: 666f 726d 2d67 726f 7570 0a20 2020 2020  form-group.     
-00015480: 2020 2072 6571 7569 7265 645c 223e 5c72     required\">\r
-00015490: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-000154a0: 3c6c 6162 656c 2066 6f72 3d5c 226f 7361  <label for=\"osa
-000154b0: 6b61 732e 6c61 736b 7574 7573 706f 7374  kas.laskutuspost
-000154c0: 695c 223e 506f 7374 696e 756d 6572 6f0a  i\">Postinumero.
-000154d0: 2020 2020 2020 2020 6a61 202d 746f 696d          ja -toim
-000154e0: 6970 6169 6b6b 613c 2f6c 6162 656c 3e20  ipaikka</label> 
-000154f0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
-00015500: 5c74 3c69 6e70 7574 2074 7970 653d 5c22  \t<input type=\"
-00015510: 7465 7874 5c22 2072 6571 7569 7265 6420  text\" required 
-00015520: 6e61 6d65 3d5c 226f 7361 6b61 732e 6c61  name=\"osakas.la
-00015530: 736b 7574 7573 706f 7374 695c 220a 2020  skutusposti\".  
-00015540: 2020 2020 2020 636c 6173 733d 5c22 666f        class=\"fo
-00015550: 726d 2d63 6f6e 7472 6f6c 5c22 203e 5c72  rm-control\" >\r
-00015560: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \n\t\t\t\t\t\t</
-00015570: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
-00015580: 5c74 3c2f 6669 656c 6473 6574 3e5c 725c  \t</fieldset>\r\
-00015590: 6e5c 745c 745c 745c 743c 2f64 6976 3e5c  n\t\t\t\t</div>\
-000155a0: 725c 6e5c 745c 745c 743c 2f64 6976 3e5c  r\n\t\t\t</div>\
-000155b0: 725c 6e5c 725c 6e5c 745c 745c 743c 6469  r\n\r\n\t\t\t<di
-000155c0: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
-000155d0: 5c22 726f 7720 6274 6e2d 726f 775c 223e  \"row btn-row\">
-000155e0: 5c72 5c6e 5c74 5c74 5c74 5c74 3c64 6976  \r\n\t\t\t\t<div
-000155f0: 2063 6c61 7373 3d5c 2263 6f6c 2d6d 642d   class=\"col-md-
-00015600: 3132 2074 6578 742d 6365 6e74 6572 5c22  12 text-center\"
-00015610: 3e5c 725c 6e5c 745c 745c 745c 745c 743c  >\r\n\t\t\t\t\t<
-00015620: 756c 0a20 2020 2020 2020 2063 6c61 7373  ul.        class
-00015630: 3d5c 226c 6973 742d 696e 6c69 6e65 5c22  =\"list-inline\"
-00015640: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
-00015650: 745c 725c 6e5c 745c 745c 745c 745c 745c  t\r\n\t\t\t\t\t\
-00015660: 743c 6c69 3e5c 725c 6e5c 745c 745c 745c  t<li>\r\n\t\t\t\
-00015670: 745c 745c 745c 743c 6275 7474 6f6e 0a20  t\t\t\t<button. 
-00015680: 2020 2020 2020 2074 7970 653d 5c22 6275         type=\"bu
-00015690: 7474 6f6e 5c22 2063 6c61 7373 3d5c 2262  tton\" class=\"b
-000156a0: 746e 2062 746e 2d70 7269 6d61 7279 5c22  tn btn-primary\"
-000156b0: 2064 6174 612d 6163 7469 6f6e 3d5c 2273   data-action=\"s
-000156c0: 6176 652d 6164 645c 223e 5c72 5c6e 5c74  ave-add\">\r\n\t
-000156d0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 4a61  \t\t\t\t\t\t\tJa
-000156e0: 746b 615c 725c 6e5c 745c 745c 745c 745c  tka\r\n\t\t\t\t\
-000156f0: 745c 745c 743c 2f62 7574 746f 6e3e 5c72  t\t\t</button>\r
-00015700: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \n\t\t\t\t\t\t</
-00015710: 6c69 3e5c 725c 6e5c 745c 745c 745c 745c  li>\r\n\t\t\t\t\
-00015720: 745c 745c 725c 6e5c 745c 745c 745c 745c  t\t\r\n\t\t\t\t\
-00015730: 745c 743c 6c69 3e5c 725c 6e5c 745c 745c  t\t<li>\r\n\t\t\
-00015740: 745c 745c 745c 745c 743c 6275 7474 6f6e  t\t\t\t\t<button
-00015750: 0a20 2020 2020 2020 2074 7970 653d 5c22  .        type=\"
-00015760: 6275 7474 6f6e 5c22 2063 6c61 7373 3d5c  button\" class=\
-00015770: 2262 746e 2062 746e 2d70 7269 6d61 7279  "btn btn-primary
-00015780: 5c22 2064 6174 612d 6163 7469 6f6e 3d5c  \" data-action=\
-00015790: 2263 616e 6365 6c2d 6164 645c 223e 5c72  "cancel-add\">\r
-000157a0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
-000157b0: 5c74 5065 7275 7574 615c 725c 6e5c 745c  \tPeruuta\r\n\t\
-000157c0: 745c 745c 745c 745c 745c 743c 2f62 7574  t\t\t\t\t\t</but
-000157d0: 746f 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74  ton>\r\n\t\t\t\t
-000157e0: 5c74 5c74 3c2f 6c69 3e5c 725c 6e5c 745c  \t\t</li>\r\n\t\
-000157f0: 745c 745c 745c 743c 2f75 6c3e 5c72 5c6e  t\t\t\t</ul>\r\n
-00015800: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
-00015810: 5c6e 5c74 5c74 5c74 3c2f 6469 763e 5c72  \n\t\t\t</div>\r
-00015820: 5c6e 5c74 5c74 3c2f 666f 726d 3e5c 725c  \n\t\t</form>\r\
-00015830: 6e5c 743c 2f64 6976 3e5c 725c 6e3c 2f64  n\t</div>\r\n</d
-00015840: 6976 3e5c 725c 6e3c 2f73 6372 6970 743e  iv>\r\n</script>
-00015850: 5c72 5c6e 5c72 5c6e 3c73 6372 6970 740a  \r\n\r\n<script.
-00015860: 2020 2020 2020 2020 6964 3d5c 2261 6b70          id=\"akp
-00015870: 2d73 656c 6563 742d 7465 6d70 6c61 7465  -select-template
-00015880: 5c22 2074 7970 653d 5c22 7465 7874 2f78  \" type=\"text/x
-00015890: 2d74 656d 706c 6174 655c 223e 5c72 5c6e  -template\">\r\n
-000158a0: 5c72 5c6e 5c72 5c6e 3c64 6976 2063 6c61  \r\n\r\n<div cla
-000158b0: 7373 3d5c 2266 6f72 6d43 6f6c 5c22 3e5c  ss=\"formCol\">\
-000158c0: 725c 6e5c 743c 6469 760a 2020 2020 2020  r\n\t<div.      
-000158d0: 2020 636c 6173 733d 5c22 636f 6e74 6169    class=\"contai
-000158e0: 6e65 722d 666c 7569 645c 223e 5c72 5c6e  ner-fluid\">\r\n
-000158f0: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
-00015900: 2272 6f77 5c22 3e5c 725c 6e5c 745c 745c  "row\">\r\n\t\t\
-00015910: 743c 6469 7620 636c 6173 733d 5c22 636f  t<div class=\"co
-00015920: 6c2d 6d64 2d34 5c22 3e5c 725c 6e5c 745c  l-md-4\">\r\n\t\
-00015930: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
-00015940: 2020 636c 6173 733d 5c22 666f 726d 2d67    class=\"form-g
-00015950: 726f 7570 5c22 3e5c 725c 6e5c 745c 745c  roup\">\r\n\t\t\
-00015960: 745c 745c 743c 6c61 6265 6c20 666f 723d  t\t\t<label for=
-00015970: 5c22 636f 6d6d 756e 6974 792d 7365 6c65  \"community-sele
-00015980: 6374 6f72 5c22 3e56 616c 6974 7365 0a20  ctor\">Valitse. 
-00015990: 2020 2020 2020 206b 756e 7461 3c2f 6c61         kunta</la
-000159a0: 6265 6c3e 5c72 5c6e 5c74 5c74 5c74 5c74  bel>\r\n\t\t\t\t
-000159b0: 5c74 3c73 656c 6563 7420 6964 3d5c 2263  \t<select id=\"c
-000159c0: 6f6d 6d75 6e69 7479 2d73 656c 6563 746f  ommunity-selecto
-000159d0: 725c 2220 636c 6173 733d 5c22 666f 726d  r\" class=\"form
-000159e0: 2d63 6f6e 7472 6f6c 5c22 0a20 2020 2020  -control\".     
-000159f0: 2020 2064 6174 612d 726f 6c65 3d5c 2263     data-role=\"c
-00015a00: 6f6d 6d75 6e69 7479 2d73 656c 6563 746f  ommunity-selecto
-00015a10: 725c 223e 3c2f 7365 6c65 6374 3e5c 725c  r\"></select>\r\
-00015a20: 6e5c 745c 745c 745c 743c 2f64 6976 3e5c  n\t\t\t\t</div>\
-00015a30: 725c 6e5c 745c 745c 745c 743c 6469 760a  r\n\t\t\t\t<div.
-00015a40: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-00015a50: 666f 726d 2d67 726f 7570 5c22 3e5c 725c  form-group\">\r\
-00015a60: 6e5c 745c 745c 745c 745c 743c 6c61 6265  n\t\t\t\t\t<labe
-00015a70: 6c20 666f 723d 5c22 616b 702d 7365 6c65  l for=\"akp-sele
-00015a80: 6374 6f72 5c22 3e56 616c 6974 7365 2070  ctor\">Valitse p
-00015a90: 6973 7465 3c2f 6c61 6265 6c3e 5c72 5c6e  iste</label>\r\n
-00015aa0: 5c74 5c74 5c74 5c74 5c74 3c73 656c 6563  \t\t\t\t\t<selec
-00015ab0: 740a 2020 2020 2020 2020 6964 3d5c 2261  t.        id=\"a
-00015ac0: 6b70 2d73 656c 6563 746f 725c 2220 636c  kp-selector\" cl
-00015ad0: 6173 733d 5c22 666f 726d 2d63 6f6e 7472  ass=\"form-contr
-00015ae0: 6f6c 5c22 2064 6174 612d 726f 6c65 3d5c  ol\" data-role=\
-00015af0: 2261 6b70 2d73 656c 6563 746f 725c 223e  "akp-selector\">
-00015b00: 3c2f 7365 6c65 6374 3e5c 725c 6e5c 745c  </select>\r\n\t\
-00015b10: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
-00015b20: 725c 6e5c 745c 745c 745c 743c 6469 760a  r\n\t\t\t\t<div.
-00015b30: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-00015b40: 726f 775c 2220 6461 7461 2d72 6f6c 653d  row\" data-role=
-00015b50: 5c22 6275 7474 6f6e 2d63 6f6e 7461 696e  \"button-contain
-00015b60: 6572 5c22 2073 7479 6c65 3d5c 2264 6973  er\" style=\"dis
-00015b70: 706c 6179 3a20 6e6f 6e65 5c22 3e5c 725c  play: none\">\r\
-00015b80: 6e5c 745c 745c 745c 745c 743c 6469 760a  n\t\t\t\t\t<div.
-00015b90: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-00015ba0: 636f 6c2d 6d64 2d31 325c 223e 5c72 5c6e  col-md-12\">\r\n
-00015bb0: 5c74 5c74 5c74 5c74 5c74 5c74 3c62 7574  \t\t\t\t\t\t<but
-00015bc0: 746f 6e20 6461 7461 2d72 6f6c 653d 5c22  ton data-role=\"
-00015bd0: 6f6b 5c22 2063 6c61 7373 3d5c 2262 746e  ok\" class=\"btn
-00015be0: 2062 746e 2d70 7269 6d61 7279 0a20 2020   btn-primary.   
-00015bf0: 2020 2020 2062 746e 2d62 6c6f 636b 5c22       btn-block\"
-00015c00: 3e48 7976 5c78 4534 6b73 7920 7661 6c69  >Hyv\xE4ksy vali
-00015c10: 7474 7520 7069 7374 653c 2f62 7574 746f  ttu piste</butto
-00015c20: 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  n>\r\n\t\t\t\t\t
-00015c30: 5c74 3c62 7574 746f 6e20 6461 7461 2d72  \t<button data-r
-00015c40: 6f6c 653d 5c22 6361 6e63 656c 5c22 0a20  ole=\"cancel\". 
-00015c50: 2020 2020 2020 2063 6c61 7373 3d5c 2262         class=\"b
-00015c60: 746e 2062 746e 2d64 6566 6175 6c74 2062  tn btn-default b
-00015c70: 746e 2d62 6c6f 636b 5c22 3e50 6572 7575  tn-block\">Peruu
-00015c80: 7461 3c2f 6275 7474 6f6e 3e5c 725c 6e5c  ta</button>\r\n\
-00015c90: 745c 745c 745c 745c 743c 2f64 6976 3e5c  t\t\t\t\t</div>\
-00015ca0: 725c 6e5c 745c 745c 745c 743c 2f64 6976  r\n\t\t\t\t</div
-00015cb0: 3e5c 725c 6e5c 725c 6e5c 745c 745c 745c  >\r\n\r\n\t\t\t\
-00015cc0: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
-00015cd0: 6173 733d 5c22 726f 775c 223e 5c72 5c6e  ass=\"row\">\r\n
-00015ce0: 5c74 5c74 5c74 5c74 5c74 3c64 6976 2063  \t\t\t\t\t<div c
-00015cf0: 6c61 7373 3d5c 2263 6f6c 2d6d 642d 3132  lass=\"col-md-12
-00015d00: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
-00015d10: 745c 743c 7020 636c 6173 733d 5c22 6865  t\t<p class=\"he
-00015d20: 6c70 2d62 6c6f 636b 0a20 2020 2020 2020  lp-block.       
-00015d30: 2074 6578 742d 6365 6e74 6572 5c22 3e56   text-center\">V
-00015d40: 6f69 7420 7661 6c69 7461 2070 6973 7465  oit valita piste
-00015d50: 656e 206d 795c 7846 3673 206b 6172 7461  en my\xF6s karta
-00015d60: 6c74 613c 2f70 3e5c 725c 6e5c 745c 745c  lta</p>\r\n\t\t\
-00015d70: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
-00015d80: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
-00015d90: 6e5c 745c 745c 743c 2f64 6976 3e5c 725c  n\t\t\t</div>\r\
-00015da0: 6e5c 725c 6e5c 745c 745c 743c 6469 760a  n\r\n\t\t\t<div.
-00015db0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
-00015dc0: 636f 6c2d 6d64 2d38 5c22 3e5c 725c 6e5c  col-md-8\">\r\n\
-00015dd0: 745c 745c 745c 743c 6469 7620 6964 3d5c  t\t\t\t<div id=\
-00015de0: 2261 6b70 2d6d 6170 5c22 2064 6174 612d  "akp-map\" data-
-00015df0: 726f 6c65 3d5c 226d 6170 5c22 3e3c 2f64  role=\"map\"></d
-00015e00: 6976 3e5c 725c 6e5c 745c 745c 743c 2f64  iv>\r\n\t\t\t</d
-00015e10: 6976 3e5c 725c 6e5c 745c 743c 2f64 6976  iv>\r\n\t\t</div
-00015e20: 3e5c 725c 6e5c 743c 2f64 6976 3e5c 725c  >\r\n\t</div>\r\
-00015e30: 6e3c 2f64 6976 3e5c 725c 6e3c 2f73 6372  n</div>\r\n</scr
-00015e40: 6970 743e 5c72 5c6e 5c72 5c6e 5c72 5c6e  ipt>\r\n\r\n\r\n
-00015e50: 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e  \r\n\r\n\r\n\r\n
-00015e60: 5c72 5c6e 3c64 6976 0a20 2020 2020 2020  \r\n<div.       
-00015e70: 2069 643d 5c22 7761 7374 652d 7761 7465   id=\"waste-wate
-00015e80: 722d 6d6f 6461 6c5c 2220 636c 6173 733d  r-modal\" class=
-00015e90: 5c22 6d6f 6461 6c5c 2220 7374 796c 653d  \"modal\" style=
-00015ea0: 5c22 6469 7370 6c61 793a 6e6f 6e65 5c22  \"display:none\"
-00015eb0: 3e5c 725c 6e20 2020 203c 6469 760a 2020  >\r\n    <div.  
-00015ec0: 2020 2020 2020 636c 6173 733d 5c22 6d6f        class=\"mo
-00015ed0: 6461 6c2d 6469 616c 6f67 206d 6f64 616c  dal-dialog modal
-00015ee0: 2d6c 675c 223e 5c72 5c6e 2020 2020 2020  -lg\">\r\n      
-00015ef0: 2020 3c64 6976 2063 6c61 7373 3d5c 226d    <div class=\"m
-00015f00: 6f64 616c 2d63 6f6e 7465 6e74 5c22 3e5c  odal-content\">\
-00015f10: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-00015f20: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00015f30: 7373 3d5c 226d 6f64 616c 2d62 6f64 795c  ss=\"modal-body\
-00015f40: 223e 5c72 5c6e 5c72 5c6e 2020 2020 2020  ">\r\n\r\n      
-00015f50: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00015f60: 6c61 7373 3d5c 2270 6167 652d 6865 6164  lass=\"page-head
-00015f70: 6572 5c22 3e5c 725c 6e0a 2020 2020 2020  er\">\r\n.      
-00015f80: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-00015f90: 2020 2020 2020 3c68 313e 4c69 6974 7920        <h1>Liity 
-00015fa0: 6c69 6574 7465 6964 656e 206b 6572 5c78  lietteiden ker\x
-00015fb0: 4534 796b 7365 656e 3c2f 6831 3e5c 725c  E4ykseen</h1>\r\
-00015fc0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00015fd0: 203c 2f64 6976 3e5c 725c 6e5c 725c 6e0a   </div>\r\n\r\n.
-00015fe0: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-00015ff0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00016000: 7373 3d5c 226c 6f61 6469 6e67 2d69 636f  ss=\"loading-ico
-00016010: 6e5c 223e 3c2f 6469 763e 5c72 5c6e 5c72  n\"></div>\r\n\r
-00016020: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00016030: 2020 3c64 6976 0a20 2020 2020 2020 2064    <div.        d
-00016040: 6174 612d 726f 6c65 3d5c 2274 6162 6261  ata-role=\"tabba
-00016050: 725c 223e 5c72 5c6e 2020 2020 2020 2020  r\">\r\n        
-00016060: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
-00016070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016080: 2020 2020 3c75 6c20 636c 6173 733d 5c22      <ul class=\"
-00016090: 7461 622d 6c69 7374 0a20 2020 2020 2020  tab-list.       
-000160a0: 206c 6973 742d 696e 6c69 6e65 5c22 2064   list-inline\" d
-000160b0: 6174 612d 726f 6c65 3d5c 2274 6162 2d6c  ata-role=\"tab-l
-000160c0: 6973 745c 223e 5c72 5c6e 2020 2020 2020  ist\">\r\n      
-000160d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160e0: 2020 3c6c 6920 636c 6173 733d 5c22 6163    <li class=\"ac
-000160f0: 7469 7665 0a20 2020 2020 2020 2061 315c  tive.        a1\
-00016100: 223e 3c61 2068 7265 663d 5c22 2361 315c  "><a href=\"#a1\
-00016110: 223e 4131 3c2f 613e 3c2f 6c69 3e3c 6c69  ">A1</a></li><li
-00016120: 2063 6c61 7373 3d5c 2261 3220 6469 7361   class=\"a2 disa
-00016130: 626c 6564 5c22 3e3c 6120 6872 6566 3d5c  bled\"><a href=\
-00016140: 2223 6132 5c22 3e41 323c 2f61 3e3c 2f6c  "#a2\">A2</a></l
-00016150: 693e 3c6c 690a 2020 2020 2020 2020 636c  i><li.        cl
-00016160: 6173 733d 5c22 6133 2064 6973 6162 6c65  ass=\"a3 disable
-00016170: 645c 223e 3c61 2068 7265 663d 5c22 2361  d\"><a href=\"#a
-00016180: 335c 223e 4133 3c2f 613e 3c2f 6c69 3e3c  3\">A3</a></li><
-00016190: 6c69 2063 6c61 7373 3d5c 2261 3420 6469  li class=\"a4 di
-000161a0: 7361 626c 6564 5c22 3e3c 610a 2020 2020  sabled\"><a.    
-000161b0: 2020 2020 6872 6566 3d5c 2223 6134 5c22      href=\"#a4\"
-000161c0: 3e41 343c 2f61 3e3c 2f6c 693e 3c6c 6920  >A4</a></li><li 
-000161d0: 636c 6173 733d 5c22 6135 2064 6973 6162  class=\"a5 disab
-000161e0: 6c65 645c 223e 3c61 2068 7265 663d 5c22  led\"><a href=\"
-000161f0: 2361 355c 223e 4135 3c2f 613e 3c2f 6c69  #a5\">A5</a></li
-00016200: 3e3c 6c69 0a20 2020 2020 2020 2063 6c61  ><li.        cla
-00016210: 7373 3d5c 2261 3620 6469 7361 626c 6564  ss=\"a6 disabled
-00016220: 5c22 3e3c 6120 6872 6566 3d5c 2223 6136  \"><a href=\"#a6
-00016230: 5c22 3e41 363c 2f61 3e3c 2f6c 693e 5c72  \">A6</a></li>\r
-00016240: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00016250: 2020 2020 2020 3c2f 756c 3e5c 725c 6e0a        </ul>\r\n.
-00016260: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-00016270: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
+0000d510: 2020 2020 2020 3c2f 6469 763e 5c72 5c6e        </div>\r\n
+0000d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d540: 3c2f 6469 763e 5c72 5c6e 0a20 2020 2020  </div>\r\n.     
+0000d550: 2020 205c 2020 2020 2020 2020 2020 2020     \            
+0000d560: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000d570: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
+0000d580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d590: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000d5a0: 5c22 636f 6c2d 6d64 2d38 0a20 2020 2020  \"col-md-8.     
+0000d5b0: 2020 2063 6f6c 2d6d 642d 7075 6c6c 2d34     col-md-pull-4
+0000d5c0: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
+0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5e0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0000d5f0: 733d 5c22 616c 6572 7420 616c 6572 742d  s=\"alert alert-
+0000d600: 696e 666f 5c22 0a20 2020 2020 2020 2064  info\".        d
+0000d610: 6174 612d 726f 6c65 3d5c 226d 6573 7361  ata-role=\"messa
+0000d620: 6765 5c22 3e3c 2f64 6976 3e5c 725c 6e20  ge\"></div>\r\n 
+0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d640: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000d650: 6469 7620 636c 6173 733d 5c22 7072 6f64  div class=\"prod
+0000d660: 7563 742d 6c69 7374 5c22 0a20 2020 2020  uct-list\".     
+0000d670: 2020 2064 6174 612d 726f 6c65 3d5c 2270     data-role=\"p
+0000d680: 726f 6475 6374 2d6c 6973 745c 223e 3c2f  roduct-list\"></
+0000d690: 6469 763e 5c72 5c6e 2020 2020 2020 2020  div>\r\n        
+0000d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6b0: 2020 2020 3c2f 6469 763e 5c72 5c6e 0a20      </div>\r\n. 
+0000d6c0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+0000d6d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000d6e0: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
+0000d6f0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+0000d700: 6976 3e5c 725c 6e5c 725c 6e20 2020 2020  iv>\r\n\r\n     
+0000d710: 2020 2020 2020 2020 2020 2020 2020 205c                 \
+0000d720: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d740: 2020 2020 5c72 5c6e 2020 2020 2020 2020      \r\n        
+0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d760: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+0000d770: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
+0000d780: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7a0: 203c 6469 7620 6461 7461 2d72 6f6c 653d   <div data-role=
+0000d7b0: 5c22 7265 7073 696b 6b61 2d74 6162 5c22  \"repsikka-tab\"
+0000d7c0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7e0: 203c 700a 2020 2020 2020 2020 636c 6173   <p.        clas
+0000d7f0: 733d 5c22 616c 6572 7420 616c 6572 742d  s=\"alert alert-
+0000d800: 696e 666f 5c22 3e3c 2f70 3e5c 725c 6e20  info\"></p>\r\n 
+0000d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d820: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0000d830: 6461 7461 2d72 6f6c 653d 5c22 666f 726d  data-role=\"form
+0000d840: 5c22 3e3c 2f64 6976 3e5c 725c 6e0a 2020  \"></div>\r\n.  
+0000d850: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d870: 2020 3c70 3e54 6172 6b69 7374 6120 7968    <p>Tarkista yh
+0000d880: 7465 7973 7469 6574 6f73 692e 2048 756f  teystietosi. Huo
+0000d890: 6d69 6f69 7468 616e 2065 7269 7479 6973  mioithan erityis
+0000d8a0: 6573 7469 2c0a 2020 2020 2020 2020 6574  esti,.        et
+0000d8b0: 745c 7845 3420 7461 7276 6974 7365 6d6d  t\xE4 tarvitsemm
+0000d8c0: 6520 7075 6865 6c69 6e6e 756d 6572 6f6e  e puhelinnumeron
+0000d8d0: 2c20 6a6f 7374 6120 7369 6e75 7420 7461  , josta sinut ta
+0000d8e0: 766f 6974 7461 6120 705c 7845 3469 765c  voittaa p\xE4iv\
+0000d8f0: 7845 3473 6169 6b61 616e 2e3c 2f70 3e3c  xE4saikaan.</p><
+0000d900: 703e 5661 6876 6973 7461 6d6d 650a 2020  p>Vahvistamme.  
+0000d910: 2020 2020 2020 7469 6c61 756b 7365 6e20        tilauksen 
+0000d920: 7669 656c 5c78 4534 2073 5c78 4534 686b  viel\xE4 s\xE4hk
+0000d930: 5c78 4636 706f 7374 6974 7365 2074 6169  \xF6postitse tai
+0000d940: 2070 7568 656c 696d 6974 7365 2e3c 2f70   puhelimitse.</p
+0000d950: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d970: 203c 6469 760a 2020 2020 2020 2020 636c   <div.        cl
+0000d980: 6173 733d 5c22 666f 726d 2d62 7574 746f  ass=\"form-butto
+0000d990: 6e73 2074 6578 742d 6365 6e74 6572 5c22  ns text-center\"
+0000d9a0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9c0: 2020 2020 203c 6275 7474 6f6e 0a20 2020       <button.   
+0000d9d0: 2020 2020 2074 7970 653d 5c22 6275 7474       type=\"butt
+0000d9e0: 6f6e 5c22 2064 6174 612d 6163 7469 6f6e  on\" data-action
+0000d9f0: 3d5c 2273 656e 645c 2220 636c 6173 733d  =\"send\" class=
+0000da00: 5c22 6274 6e20 6274 6e2d 7072 696d 6172  \"btn btn-primar
+0000da10: 795c 223e 4c5c 7845 3468 6574 5c78 4534  y\">L\xE4het\xE4
+0000da20: 3c2f 6275 7474 6f6e 3e5c 725c 6e0a 2020  </button>\r\n.  
+0000da30: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da50: 2020 3c2f 6469 763e 5c72 5c6e 2020 2020    </div>\r\n    
+0000da60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da70: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0000da80: 7373 3d5c 2267 6c6f 6261 6c2d 7661 6c69  ss=\"global-vali
+0000da90: 6461 7469 6f6e 2d65 7272 6f72 0a20 2020  dation-error.   
+0000daa0: 2020 2020 2061 6c65 7274 2061 6c65 7274       alert alert
+0000dab0: 2d64 616e 6765 725c 2220 7374 796c 653d  -danger\" style=
+0000dac0: 5c22 6469 7370 6c61 793a 6e6f 6e65 5c22  \"display:none\"
+0000dad0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+0000dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000daf0: 2020 2020 2054 5c78 4534 7974 5c78 4534       T\xE4yt\xE4
+0000db00: 0a20 2020 2020 2020 2070 7575 7474 7576  .        puuttuv
+0000db10: 6174 206b 656e 745c 7845 3474 5c72 5c6e  at kent\xE4t\r\n
+0000db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db30: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+0000db40: 763e 5c72 5c6e 2020 2020 2020 2020 2020  v>\r\n          
+0000db50: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+0000db60: 6469 763e 5c72 5c6e 0a20 2020 2020 2020  div>\r\n.       
+0000db70: 205c 2020 2020 2020 2020 2020 2020 2020   \              
+0000db80: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
+0000db90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dba0: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
+0000dbb0: 2020 2020 2020 2020 2020 2020 205c 725c               \r\
+0000dbc0: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+0000dbd0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+0000dbe0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+0000dbf0: 2020 2020 3c62 7574 746f 6e20 636c 6173      <button clas
+0000dc00: 733d 5c22 6274 6e20 6274 6e2d 6465 6661  s=\"btn btn-defa
+0000dc10: 756c 740a 2020 2020 2020 2020 6361 6e63  ult.        canc
+0000dc20: 656c 5c22 3e50 6572 7575 7461 3c2f 6275  el\">Peruuta</bu
+0000dc30: 7474 6f6e 3e5c 725c 6e20 2020 2020 2020  tton>\r\n       
+0000dc40: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0000dc50: 6173 733d 5c22 636c 6561 7266 6978 5c22  ass=\"clearfix\"
+0000dc60: 3e3c 2f64 6976 3e5c 725c 6e0a 2020 2020  ></div>\r\n.    
+0000dc70: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
+0000dc80: 3c2f 6469 763e 5c72 5c6e 2020 2020 2020  </div>\r\n      
+0000dc90: 2020 3c2f 6469 763e 5c72 5c6e 2020 2020    </div>\r\n    
+0000dca0: 3c2f 6469 763e 5c72 5c6e 3c2f 6469 763e  </div>\r\n</div>
+0000dcb0: 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e  \r\n\r\n\r\n\r\n
+0000dcc0: 3c64 6976 0a20 2020 2020 2020 2069 643d  <div.        id=
+0000dcd0: 5c22 6665 6564 6261 636b 2d6d 6f64 616c  \"feedback-modal
+0000dce0: 5c22 2063 6c61 7373 3d5c 226d 6f64 616c  \" class=\"modal
+0000dcf0: 5c22 2073 7479 6c65 3d5c 2264 6973 706c  \" style=\"displ
+0000dd00: 6179 3a6e 6f6e 655c 223e 5c72 5c6e 2020  ay:none\">\r\n  
+0000dd10: 2020 3c64 6976 0a20 2020 2020 2020 2063    <div.        c
+0000dd20: 6c61 7373 3d5c 226d 6f64 616c 2d64 6961  lass=\"modal-dia
+0000dd30: 6c6f 675c 223e 5c72 5c6e 2020 2020 2020  log\">\r\n      
+0000dd40: 2020 3c64 6976 2063 6c61 7373 3d5c 226d    <div class=\"m
+0000dd50: 6f64 616c 2d63 6f6e 7465 6e74 5c22 3e5c  odal-content\">\
+0000dd60: 725c 6e20 2020 2020 2020 2020 2020 203c  r\n            <
+0000dd70: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
+0000dd80: 733d 5c22 6d6f 6461 6c2d 626f 6479 5c22  s=\"modal-body\"
+0000dd90: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+0000dda0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000ddb0: 5c22 7061 6765 2d68 6561 6465 725c 223e  \"page-header\">
+0000ddc0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+0000ddd0: 2020 2020 2020 2020 5c72 5c6e 0a20 2020          \r\n.   
+0000dde0: 2020 2020 205c 2020 2020 2020 2020 2020       \          
+0000ddf0: 2020 2020 2020 2020 203c 6275 7474 6f6e           <button
+0000de00: 2063 6c61 7373 3d5c 2270 756c 6c2d 7269   class=\"pull-ri
+0000de10: 6768 7420 6274 6e2d 6469 736d 6973 735c  ght btn-dismiss\
+0000de20: 2220 6172 6961 2d6c 6162 656c 3d5c 2253  " aria-label=\"S
+0000de30: 756c 6a65 5c22 0a20 2020 2020 2020 2064  ulje\".        d
+0000de40: 6174 612d 6163 7469 6f6e 3d5c 2263 616e  ata-action=\"can
+0000de50: 6365 6c2d 616c 6c5c 223e 3c2f 6275 7474  cel-all\"></butt
+0000de60: 6f6e 3e5c 725c 6e20 2020 2020 2020 2020  on>\r\n         
+0000de70: 2020 2020 2020 2020 2020 203c 6831 3e41             <h1>A
+0000de80: 6e6e 6120 7061 6c61 7574 6574 7461 3c2f  nna palautetta</
+0000de90: 6831 3e5c 725c 6e0a 2020 2020 2020 2020  h1>\r\n.        
+0000dea0: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+0000deb0: 3c2f 6469 763e 5c72 5c6e 5c72 5c6e 2020  </div>\r\n\r\n  
+0000dec0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+0000ded0: 6976 2063 6c61 7373 3d5c 2266 6f72 6d5c  iv class=\"form\
+0000dee0: 223e 3c2f 6469 763e 5c72 5c6e 0a20 2020  "></div>\r\n.   
+0000def0: 2020 2020 205c 2020 2020 2020 2020 2020       \          
+0000df00: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0000df10: 5c22 676c 6f62 616c 2d76 616c 6964 6174  \"global-validat
+0000df20: 696f 6e2d 6572 726f 7220 616c 6572 7420  ion-error alert 
+0000df30: 616c 6572 742d 6461 6e67 6572 5c22 0a20  alert-danger\". 
+0000df40: 2020 2020 2020 2073 7479 6c65 3d5c 2264         style=\"d
+0000df50: 6973 706c 6179 3a6e 6f6e 655c 223e 5c72  isplay:none\">\r
+0000df60: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0000df70: 2020 2020 2020 545c 7845 3479 745c 7845        T\xE4yt\xE
+0000df80: 3420 7075 7574 7475 7661 7420 6b65 6e74  4 puuttuvat kent
+0000df90: 5c78 4534 745c 725c 6e0a 2020 2020 2020  \xE4t\r\n.      
+0000dfa0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+0000dfb0: 2020 3c2f 6469 763e 5c72 5c6e 2020 2020    </div>\r\n    
+0000dfc0: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
+0000dfd0: 5c6e 2020 2020 2020 2020 3c2f 6469 763e  \n        </div>
+0000dfe0: 5c72 5c6e 2020 2020 3c2f 6469 763e 5c72  \r\n    </div>\r
+0000dff0: 5c6e 3c2f 6469 763e 5c72 5c6e 5c72 5c6e  \n</div>\r\n\r\n
+0000e000: 5c72 5c6e 5c72 5c6e 5c72 5c6e 3c64 6976  \r\n\r\n\r\n<div
+0000e010: 0a20 2020 2020 2020 2069 643d 5c22 666f  .        id=\"fo
+0000e020: 7267 6f74 7465 6e2d 7061 7373 776f 7264  rgotten-password
+0000e030: 2d6d 6f64 616c 5c22 2063 6c61 7373 3d5c  -modal\" class=\
+0000e040: 226d 6f64 616c 5c22 2073 7479 6c65 3d5c  "modal\" style=\
+0000e050: 2264 6973 706c 6179 3a6e 6f6e 655c 223e  "display:none\">
+0000e060: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+0000e070: 203c 6469 7620 636c 6173 733d 5c22 6d6f   <div class=\"mo
+0000e080: 6461 6c2d 6469 616c 6f67 5c22 3e5c 725c  dal-dialog\">\r\
+0000e090: 6e20 2020 2020 2020 203c 6469 7620 636c  n        <div cl
+0000e0a0: 6173 733d 5c22 6d6f 6461 6c2d 636f 6e74  ass=\"modal-cont
+0000e0b0: 656e 745c 223e 5c72 5c6e 0a20 2020 2020  ent\">\r\n.     
+0000e0c0: 2020 205c 2020 2020 2020 2020 2020 203c     \           <
+0000e0d0: 6469 7620 636c 6173 733d 5c22 6d6f 6461  div class=\"moda
+0000e0e0: 6c2d 626f 6479 5c22 3e5c 725c 6e20 2020  l-body\">\r\n   
+0000e0f0: 2020 2020 2020 2020 205c 743c 6469 7620           \t<div 
+0000e100: 636c 6173 733d 5c22 7061 6765 2d68 6561  class=\"page-hea
+0000e110: 6465 725c 223e 5c72 5c6e 0a20 2020 2020  der\">\r\n.     
+0000e120: 2020 205c 2020 2020 2020 2020 2020 205c     \           \
+0000e130: 745c 743c 6832 3e54 696c 6161 2075 6e6f  t\t<h2>Tilaa uno
+0000e140: 6874 756e 7574 2073 616c 6173 616e 613c  htunut salasana<
+0000e150: 2f68 323e 5c72 5c6e 2020 2020 2020 2020  /h2>\r\n        
+0000e160: 2020 2020 5c74 3c2f 6469 763e 5c72 5c6e      \t</div>\r\n
+0000e170: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+0000e180: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0000e190: 7620 636c 6173 733d 5c22 666f 726d 5c22  v class=\"form\"
+0000e1a0: 3e3c 2f64 6976 3e5c 725c 6e20 2020 2020  ></div>\r\n     
+0000e1b0: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
+0000e1c0: 6e20 2020 2020 2020 203c 2f64 6976 3e5c  n        </div>\
+0000e1d0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+0000e1e0: 3c2f 6469 763e 5c72 5c6e 3c2f 6469 763e  </div>\r\n</div>
+0000e1f0: 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e  \r\n\r\n\r\n\r\n
+0000e200: 5c72 5c6e 3c64 6976 2069 643d 5c22 7061  \r\n<div id=\"pa
+0000e210: 7373 776f 7264 2d6d 6f64 616c 5c22 2063  ssword-modal\" c
+0000e220: 6c61 7373 3d5c 226d 6f64 616c 5c22 0a20  lass=\"modal\". 
+0000e230: 2020 2020 2020 2073 7479 6c65 3d5c 2264         style=\"d
+0000e240: 6973 706c 6179 3a6e 6f6e 655c 223e 5c72  isplay:none\">\r
+0000e250: 5c6e 5c74 3c64 6976 2063 6c61 7373 3d5c  \n\t<div class=\
+0000e260: 226d 6f64 616c 2d64 6961 6c6f 675c 223e  "modal-dialog\">
+0000e270: 5c72 5c6e 5c74 5c74 3c64 6976 2063 6c61  \r\n\t\t<div cla
+0000e280: 7373 3d5c 226d 6f64 616c 2d63 6f6e 7465  ss=\"modal-conte
+0000e290: 6e74 5c22 3e5c 725c 6e5c 745c 745c 743c  nt\">\r\n\t\t\t<
+0000e2a0: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
+0000e2b0: 733d 5c22 6d6f 6461 6c2d 626f 6479 5c22  s=\"modal-body\"
+0000e2c0: 3e5c 725c 6e5c 745c 745c 745c 743c 6469  >\r\n\t\t\t\t<di
+0000e2d0: 7620 636c 6173 733d 5c22 7061 6765 2d68  v class=\"page-h
+0000e2e0: 6561 6465 725c 223e 5c72 5c6e 5c74 5c74  eader\">\r\n\t\t
+0000e2f0: 5c74 5c74 5c74 3c68 323e 5661 6968 6461  \t\t\t<h2>Vaihda
+0000e300: 0a20 2020 2020 2020 2073 616c 6173 616e  .        salasan
+0000e310: 613c 2f68 323e 5c72 5c6e 5c74 5c74 5c74  a</h2>\r\n\t\t\t
+0000e320: 5c74 3c2f 6469 763e 5c72 5c6e 5c72 5c6e  \t</div>\r\n\r\n
+0000e330: 5c74 5c74 5c74 5c74 3c64 6976 2063 6c61  \t\t\t\t<div cla
+0000e340: 7373 3d5c 2266 6f72 6d5c 2220 6461 7461  ss=\"form\" data
+0000e350: 2d72 6f6c 653d 5c22 666f 726d 5c22 3e3c  -role=\"form\"><
+0000e360: 2f64 6976 3e5c 725c 6e5c 745c 745c 743c  /div>\r\n\t\t\t<
+0000e370: 2f64 6976 3e5c 725c 6e5c 745c 743c 2f64  /div>\r\n\t\t</d
+0000e380: 6976 3e5c 725c 6e5c 743c 2f64 6976 3e5c  iv>\r\n\t</div>\
+0000e390: 725c 6e3c 2f64 6976 3e5c 725c 6e5c 725c  r\n</div>\r\n\r\
+0000e3a0: 6e5c 725c 6e5c 725c 6e3c 7363 7269 7074  n\r\n\r\n<script
+0000e3b0: 3e5c 725c 6e66 756e 6374 696f 6e0a 2020  >\r\nfunction.  
+0000e3c0: 2020 2020 2020 7365 7276 6963 6553 656c        serviceSel
+0000e3d0: 6563 746f 7243 6f6d 6269 6e65 4e6f 6e42  ectorCombineNonB
+0000e3e0: 6c61 6e6b 7328 7661 6c75 6573 2c20 7365  lanks(values, se
+0000e3f0: 7061 7261 746f 7229 207b 5c72 5c6e 5c74  parator) {\r\n\t
+0000e400: 7661 7220 7265 7375 6c74 203d 2027 273b  var result = '';
+0000e410: 5c72 5c6e 5c74 666f 7228 7661 720a 2020  \r\n\tfor(var.  
+0000e420: 2020 2020 2020 6920 3d20 303b 2069 203c        i = 0; i <
+0000e430: 2076 616c 7565 732e 6c65 6e67 7468 3b20   values.length; 
+0000e440: 2b2b 6929 207b 5c72 5c6e 5c74 5c74 6966  ++i) {\r\n\t\tif
+0000e450: 2876 616c 7565 735b 695d 2021 3d3d 206e  (values[i] !== n
+0000e460: 756c 6c20 2626 2076 616c 7565 735b 695d  ull && values[i]
+0000e470: 0a20 2020 2020 2020 2021 3d3d 2027 2729  .        !== '')
+0000e480: 207b 5c72 5c6e 5c74 5c74 5c74 6966 2872   {\r\n\t\t\tif(r
+0000e490: 6573 756c 7420 213d 3d20 2727 2920 7b5c  esult !== '') {\
+0000e4a0: 725c 6e5c 745c 745c 745c 7472 6573 756c  r\n\t\t\t\tresul
+0000e4b0: 7420 2b3d 2073 6570 6172 6174 6f72 3b5c  t += separator;\
+0000e4c0: 725c 6e5c 745c 745c 747d 5c72 5c6e 5c74  r\n\t\t\t}\r\n\t
+0000e4d0: 5c74 5c74 7265 7375 6c74 0a20 2020 2020  \t\tresult.     
+0000e4e0: 2020 202b 3d20 7661 6c75 6573 5b69 5d3b     += values[i];
+0000e4f0: 5c72 5c6e 5c74 5c74 7d5c 725c 6e5c 747d  \r\n\t\t}\r\n\t}
+0000e500: 5c72 5c6e 5c74 7265 7475 726e 2072 6573  \r\n\treturn res
+0000e510: 756c 743b 5c72 5c6e 7d5c 725c 6e5c 725c  ult;\r\n}\r\n\r\
+0000e520: 6e66 756e 6374 696f 6e20 7365 7276 6963  nfunction servic
+0000e530: 6553 656c 6563 746f 7249 6e76 6f69 6369  eSelectorInvoici
+0000e540: 6e67 2863 7573 746f 6d65 7229 0a20 2020  ng(customer).   
+0000e550: 2020 2020 207b 5c72 5c6e 5c74 6966 2866       {\r\n\tif(f
+0000e560: 616c 7365 2026 2620 6375 7374 6f6d 6572  alse && customer
+0000e570: 2e69 7361 6e6e 6f69 7473 696a 6129 207b  .isannoitsija) {
+0000e580: 5c72 5c6e 5c74 5c74 7265 7475 726e 2073  \r\n\t\treturn s
+0000e590: 6572 7669 6365 5365 6c65 6374 6f72 436f  erviceSelectorCo
+0000e5a0: 6d62 696e 654e 6f6e 426c 616e 6b73 285b  mbineNonBlanks([
+0000e5b0: 6375 7374 6f6d 6572 2e69 7361 6e6e 6f69  customer.isannoi
+0000e5c0: 7473 696a 612e 6e61 6d65 2c0a 2020 2020  tsija.name,.    
+0000e5d0: 2020 2020 6375 7374 6f6d 6572 2e69 7361      customer.isa
+0000e5e0: 6e6e 6f69 7473 696a 612e 7374 7265 6574  nnoitsija.street
+0000e5f0: 2c20 6375 7374 6f6d 6572 2e69 7361 6e6e  , customer.isann
+0000e600: 6f69 7473 696a 612e 706f 7374 5d2c 2027  oitsija.post], '
+0000e610: 2c20 2729 5c72 5c6e 5c74 7d20 656c 7365  , ')\r\n\t} else
+0000e620: 0a20 2020 2020 2020 207b 5c72 5c6e 5c74  .        {\r\n\t
+0000e630: 5c74 7265 7475 726e 2073 6572 7669 6365  \treturn service
+0000e640: 5365 6c65 6374 6f72 436f 6d62 696e 654e  SelectorCombineN
+0000e650: 6f6e 426c 616e 6b73 285b 6375 7374 6f6d  onBlanks([custom
+0000e660: 6572 2e6c 6173 6b75 7475 736e 696d 692c  er.laskutusnimi,
+0000e670: 2063 7573 746f 6d65 722e 6c61 736b 7574   customer.laskut
+0000e680: 7573 7968 7465 7973 6865 6e6b 2c0a 2020  usyhteyshenk,.  
+0000e690: 2020 2020 2020 6375 7374 6f6d 6572 2e6c        customer.l
+0000e6a0: 6173 6b75 7475 736b 6174 752c 2063 7573  askutuskatu, cus
+0000e6b0: 746f 6d65 722e 6c61 736b 7574 7573 706f  tomer.laskutuspo
+0000e6c0: 7374 692c 2063 7573 746f 6d65 722e 6c61  sti, customer.la
+0000e6d0: 736b 7574 7573 6d61 615d 2c20 272c 2027  skutusmaa], ', '
+0000e6e0: 290a 2020 2020 2020 2020 5c72 5c6e 5c74  ).        \r\n\t
+0000e6f0: 7d5c 725c 6e7d 5c72 5c6e 5c72 5c6e 3c2f  }\r\n}\r\n\r\n</
+0000e700: 7363 7269 7074 3e5c 725c 6e5c 725c 6e3c  script>\r\n\r\n<
+0000e710: 7363 7269 7074 2069 643d 5c22 7365 7276  script id=\"serv
+0000e720: 6963 652d 7365 6c65 6374 6f72 2d76 616c  ice-selector-val
+0000e730: 7565 2d74 656d 706c 6174 655c 220a 2020  ue-template\".  
+0000e740: 2020 2020 2020 7479 7065 3d5c 2274 6578        type=\"tex
+0000e750: 742f 782d 6b65 6e64 6f2d 7465 6d70 6c61  t/x-kendo-templa
+0000e760: 7465 5c22 3e5c 725c 6e5c 7423 2069 6628  te\">\r\n\t# if(
+0000e770: 7479 7065 6f66 2063 7573 746f 6d65 7273  typeof customers
+0000e780: 2021 3d3d 2027 756e 6465 6669 6e65 6427   !== 'undefined'
+0000e790: 290a 2020 2020 2020 2020 7b20 235c 725c  ).        { #\r\
+0000e7a0: 6e5c 745c 743c 6469 7620 636c 6173 733d  n\t\t<div class=
+0000e7b0: 5c22 7365 7276 6963 652d 6e61 6d65 5c22  \"service-name\"
+0000e7c0: 3e23 3a20 436f 6d6d 6f6e 2e66 6f72 6d61  >#: Common.forma
+0000e7d0: 744e 756c 6c41 7345 6d70 7479 2863 7573  tNullAsEmpty(cus
+0000e7e0: 746f 6d65 7273 5b30 5d2e 6e69 6d69 290a  tomers[0].nimi).
+0000e7f0: 2020 2020 2020 2020 2323 3a20 6375 7374          ##: cust
+0000e800: 6f6d 6572 735b 305d 2e79 6874 6579 7368  omers[0].yhteysh
+0000e810: 656e 6b20 213d 3d20 6e75 6c6c 2026 2620  enk !== null && 
+0000e820: 6375 7374 6f6d 6572 735b 305d 2e79 6874  customers[0].yht
+0000e830: 6579 7368 656e 6b20 213d 3d20 2727 2026  eyshenk !== '' &
+0000e840: 260a 2020 2020 2020 2020 6375 7374 6f6d  &.        custom
+0000e850: 6572 735b 305d 2e79 6874 6579 7368 656e  ers[0].yhteyshen
+0000e860: 6b20 213d 3d20 6375 7374 6f6d 6572 735b  k !== customers[
+0000e870: 305d 2e6e 696d 6920 3f20 272c 2027 202b  0].nimi ? ', ' +
+0000e880: 2063 7573 746f 6d65 7273 5b30 5d2e 7968   customers[0].yh
+0000e890: 7465 7973 6865 6e6b 0a20 2020 2020 2020  teyshenk.       
+0000e8a0: 203a 2027 2720 233c 2f64 6976 3e5c 725c   : '' #</div>\r\
+0000e8b0: 6e5c 745c 743c 6469 7620 636c 6173 733d  n\t\t<div class=
+0000e8c0: 5c22 7365 7276 6963 652d 6164 6472 6573  \"service-addres
+0000e8d0: 735c 223e 233a 2073 6572 7669 6365 5365  s\">#: serviceSe
+0000e8e0: 6c65 6374 6f72 436f 6d62 696e 654e 6f6e  lectorCombineNon
+0000e8f0: 426c 616e 6b73 285b 6375 7374 6f6d 6572  Blanks([customer
+0000e900: 735b 305d 2e6b 6174 752c 0a20 2020 2020  s[0].katu,.     
+0000e910: 2020 2063 7573 746f 6d65 7273 5b30 5d2e     customers[0].
+0000e920: 706f 7374 695d 2c20 272c 2027 2920 233c  posti], ', ') #<
+0000e930: 2f64 6976 3e5c 725c 6e5c 745c 745c 725c  /div>\r\n\t\t\r\
+0000e940: 6e5c 725c 6e5c 745c 745c 725c 6e5c 7423  n\r\n\t\t\r\n\t#
+0000e950: 207d 2065 6c73 6520 7b20 235c 725c 6e5c   } else { #\r\n\
+0000e960: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
+0000e970: 636c 6173 733d 5c22 7365 7276 6963 652d  class=\"service-
+0000e980: 6e61 6d65 5c22 3e56 616c 6974 7365 206b  name\">Valitse k
+0000e990: 6f68 6465 3c2f 6469 763e 5c72 5c6e 5c74  ohde</div>\r\n\t
+0000e9a0: 2320 7d20 235c 725c 6e3c 2f73 6372 6970  # } #\r\n</scrip
+0000e9b0: 743e 5c72 5c6e 5c72 5c6e 3c73 6372 6970  t>\r\n\r\n<scrip
+0000e9c0: 740a 2020 2020 2020 2020 6964 3d5c 2273  t.        id=\"s
+0000e9d0: 6572 7669 6365 2d73 656c 6563 746f 722d  ervice-selector-
+0000e9e0: 7465 6d70 6c61 7465 5c22 2074 7970 653d  template\" type=
+0000e9f0: 5c22 7465 7874 2f78 2d6b 656e 646f 2d74  \"text/x-kendo-t
+0000ea00: 656d 706c 6174 655c 223e 2320 6966 2874  emplate\"># if(t
+0000ea10: 7970 656f 660a 2020 2020 2020 2020 6375  ypeof.        cu
+0000ea20: 7374 6f6d 6572 7320 213d 3d20 2775 6e64  stomers !== 'und
+0000ea30: 6566 696e 6564 2729 207b 2023 5c72 5c6e  efined') { #\r\n
+0000ea40: 5c74 3c64 6976 2063 6c61 7373 3d5c 2273  \t<div class=\"s
+0000ea50: 6572 7669 6365 2d6e 616d 655c 223e 233a  ervice-name\">#:
+0000ea60: 2043 6f6d 6d6f 6e2e 666f 726d 6174 4e75   Common.formatNu
+0000ea70: 6c6c 4173 456d 7074 7928 6375 7374 6f6d  llAsEmpty(custom
+0000ea80: 6572 735b 305d 2e6e 696d 6929 0a20 2020  ers[0].nimi).   
+0000ea90: 2020 2020 2023 233a 2063 7573 746f 6d65       ##: custome
+0000eaa0: 7273 5b30 5d2e 7968 7465 7973 6865 6e6b  rs[0].yhteyshenk
+0000eab0: 2021 3d3d 206e 756c 6c20 2626 2063 7573   !== null && cus
+0000eac0: 746f 6d65 7273 5b30 5d2e 7968 7465 7973  tomers[0].yhteys
+0000ead0: 6865 6e6b 2021 3d3d 2027 2720 2626 0a20  henk !== '' &&. 
+0000eae0: 2020 2020 2020 2063 7573 746f 6d65 7273         customers
+0000eaf0: 5b30 5d2e 7968 7465 7973 6865 6e6b 2021  [0].yhteyshenk !
+0000eb00: 3d3d 2063 7573 746f 6d65 7273 5b30 5d2e  == customers[0].
+0000eb10: 6e69 6d69 203f 2027 2c20 2720 2b20 6375  nimi ? ', ' + cu
+0000eb20: 7374 6f6d 6572 735b 305d 2e79 6874 6579  stomers[0].yhtey
+0000eb30: 7368 656e 6b0a 2020 2020 2020 2020 3a20  shenk.        : 
+0000eb40: 2727 2023 3c2f 6469 763e 5c72 5c6e 5c74  '' #</div>\r\n\t
+0000eb50: 3c64 6976 2063 6c61 7373 3d5c 2273 6572  <div class=\"ser
+0000eb60: 7669 6365 2d61 6464 7265 7373 5c22 3e23  vice-address\">#
+0000eb70: 3a20 7365 7276 6963 6553 656c 6563 746f  : serviceSelecto
+0000eb80: 7243 6f6d 6269 6e65 4e6f 6e42 6c61 6e6b  rCombineNonBlank
+0000eb90: 7328 5b63 7573 746f 6d65 7273 5b30 5d2e  s([customers[0].
+0000eba0: 6b61 7475 2c0a 2020 2020 2020 2020 6375  katu,.        cu
+0000ebb0: 7374 6f6d 6572 735b 305d 2e70 6f73 7469  stomers[0].posti
+0000ebc0: 5d2c 2027 2c20 2729 2023 3c2f 6469 763e  ], ', ') #</div>
+0000ebd0: 5c72 5c6e 5c74 5c72 5c6e 5c72 5c6e 5c74  \r\n\t\r\n\r\n\t
+0000ebe0: 5c72 5c6e 2320 7d20 233c 2f73 6372 6970  \r\n# } #</scrip
+0000ebf0: 743e 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72  t>\r\n\r\n\r\n\r
+0000ec00: 5c6e 5c72 5c6e 5c72 5c6e 3c74 6578 7461  \n\r\n\r\n<texta
+0000ec10: 7265 610a 2020 2020 2020 2020 6964 3d5c  rea.        id=\
+0000ec20: 2274 7970 655f 6469 7368 315c 2220 7374  "type_dish1\" st
+0000ec30: 796c 653d 5c22 6469 7370 6c61 793a 6e6f  yle=\"display:no
+0000ec40: 6e65 3b5c 223e 5c72 5c6e 5c74 3c64 6976  ne;\">\r\n\t<div
+0000ec50: 2063 6c61 7373 3d5c 2264 6973 6831 2070   class=\"dish1 p
+0000ec60: 726f 6475 6374 5c22 3e5c 725c 6e5c 745c  roduct\">\r\n\t\
+0000ec70: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
+0000ec80: 6173 733d 5c22 636f 6e74 6169 6e65 722d  ass=\"container-
+0000ec90: 666c 7569 645c 223e 5c72 5c6e 5c74 5c74  fluid\">\r\n\t\t
+0000eca0: 5c74 3c64 6976 2063 6c61 7373 3d5c 2272  \t<div class=\"r
+0000ecb0: 6f77 206e 6172 726f 772d 6761 7073 5c22  ow narrow-gaps\"
+0000ecc0: 3e5c 725c 6e5c 745c 745c 745c 743c 6469  >\r\n\t\t\t\t<di
+0000ecd0: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
+0000ece0: 5c22 636f 6c2d 6d64 2d33 2074 6578 742d  \"col-md-3 text-
+0000ecf0: 6365 6e74 6572 2d78 735c 223e 7b63 6f6d  center-xs\">{com
+0000ed00: 6d6f 6e2e 696d 6167 6545 6c65 6d65 6e74  mon.imageElement
+0000ed10: 2829 7d3c 2f64 6976 3e5c 725c 6e5c 745c  ()}</div>\r\n\t\
+0000ed20: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+0000ed30: 2020 636c 6173 733d 5c22 636f 6c2d 6d64    class=\"col-md
+0000ed40: 2d36 5c22 3e5c 725c 6e5c 745c 745c 745c  -6\">\r\n\t\t\t\
+0000ed50: 745c 743c 6834 2063 6c61 7373 3d5c 2274  t\t<h4 class=\"t
+0000ed60: 6578 742d 6365 6e74 6572 2d78 7320 7072  ext-center-xs pr
+0000ed70: 6f64 7563 742d 6e61 6d65 5c22 3e7b 6f62  oduct-name\">{ob
+0000ed80: 6a2e 6e61 6d65 7d3c 2f68 343e 5c72 5c6e  j.name}</h4>\r\n
+0000ed90: 5c74 5c74 5c74 5c74 5c74 3c64 6976 0a20  \t\t\t\t\t<div. 
+0000eda0: 2020 2020 2020 2063 6c61 7373 3d5c 2264         class=\"d
+0000edb0: 6573 6372 6970 7469 6f6e 5c22 3e5c 725c  escription\">\r\
+0000edc0: 6e5c 745c 745c 745c 745c 745c 747b 6f62  n\t\t\t\t\t\t{ob
+0000edd0: 6a2e 6465 7363 7d5c 725c 6e5c 745c 745c  j.desc}\r\n\t\t\
+0000ede0: 745c 745c 745c 747b 6f62 6a2e 7765 6967  t\t\t\t{obj.weig
+0000edf0: 6874 4261 7365 640a 2020 2020 2020 2020  htBased.        
+0000ee00: 3d3d 2031 3f3c 6272 3e4b 5c78 4534 7369  == 1?<br>K\xE4si
+0000ee10: 7474 656c 796d 616b 7375 2070 6169 6e6f  ttelymaksu paino
+0000ee20: 6e20 6d75 6b61 6973 6573 7469 3a7d 5c72  n mukaisesti:}\r
+0000ee30: 5c6e 5c74 5c74 5c74 5c74 5c74 3c2f 6469  \n\t\t\t\t\t</di
+0000ee40: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f  v>\r\n\t\t\t\t</
+0000ee50: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
+0000ee60: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
+0000ee70: 7373 3d5c 2263 6f6c 2d6d 642d 335c 223e  ss=\"col-md-3\">
+0000ee80: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c72  \r\n\t\t\t\t\t\r
+0000ee90: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c64  \n\t\t\t\t\t\t<d
+0000eea0: 6976 2063 6c61 7373 3d5c 2272 6f77 5c22  iv class=\"row\"
+0000eeb0: 207b 636f 6d6d 6f6e 2e64 6973 706c 6179   {common.display
+0000eec0: 5072 6963 6528 297d 3e5c 725c 6e5c 745c  Price()}>\r\n\t\
+0000eed0: 745c 745c 745c 745c 745c 743c 6469 760a  t\t\t\t\t\t<div.
+0000eee0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+0000eef0: 636f 6c2d 6d64 2d34 2063 6f6c 2d78 732d  col-md-4 col-xs-
+0000ef00: 345c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  4\">\r\n\t\t\t\t
+0000ef10: 5c74 5c74 5c74 5c74 3c6c 6162 656c 2063  \t\t\t\t<label c
+0000ef20: 6c61 7373 3d5c 2263 6f6e 7472 6f6c 2d6c  lass=\"control-l
+0000ef30: 6162 656c 5c22 3e48 696e 7461 3c2f 6c61  abel\">Hinta</la
+0000ef40: 6265 6c3e 5c72 5c6e 5c74 5c74 5c74 5c74  bel>\r\n\t\t\t\t
+0000ef50: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
+0000ef60: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c64  \t\t\t\t\t\t\t<d
+0000ef70: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+0000ef80: 3d5c 2263 6f6c 2d6d 642d 3820 636f 6c2d  =\"col-md-8 col-
+0000ef90: 7873 2d38 5c22 3e5c 725c 6e5c 745c 745c  xs-8\">\r\n\t\t\
+0000efa0: 745c 745c 745c 745c 745c 743c 6469 7620  t\t\t\t\t\t<div 
+0000efb0: 636c 6173 733d 5c22 7072 6963 655c 223e  class=\"price\">
+0000efc0: 7b63 6f6d 6d6f 6e2e 636f 6d62 696e 6564  {common.combined
+0000efd0: 5661 7450 7269 6365 2829 7d0a 2020 2020  VatPrice()}.    
+0000efe0: 2020 2020 2665 7572 6f3b 3c2f 6469 763e      &euro;</div>
+0000eff0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+0000f000: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
+0000f010: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
+0000f020: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 7b6f  \n\t\t\t\t\t\t{o
+0000f030: 626a 2e77 6569 6768 7442 6173 6564 0a20  bj.weightBased. 
+0000f040: 2020 2020 2020 203d 3d20 313f 5c72 5c6e         == 1?\r\n
+0000f050: 5c74 5c74 5c74 5c74 5c74 5c74 3c64 6976  \t\t\t\t\t\t<div
+0000f060: 2063 6c61 7373 3d5c 2272 6f77 5c22 207b   class=\"row\" {
+0000f070: 636f 6d6d 6f6e 2e64 6973 706c 6179 5072  common.displayPr
+0000f080: 6963 6528 297d 3e5c 725c 6e5c 745c 745c  ice()}>\r\n\t\t\
+0000f090: 745c 745c 745c 745c 743c 6469 760a 2020  t\t\t\t\t<div.  
+0000f0a0: 2020 2020 2020 636c 6173 733d 5c22 636f        class=\"co
+0000f0b0: 6c2d 6d64 2d34 2063 6f6c 2d78 732d 345c  l-md-4 col-xs-4\
+0000f0c0: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
+0000f0d0: 5c74 5c74 5c74 3c6c 6162 656c 2063 6c61  \t\t\t<label cla
+0000f0e0: 7373 3d5c 2263 6f6e 7472 6f6c 2d6c 6162  ss=\"control-lab
+0000f0f0: 656c 5c22 3e4b 5c78 4534 7369 7474 656c  el\">K\xE4sittel
+0000f100: 7926 7368 793b 6d61 6b73 753c 2f6c 6162  y&shy;maksu</lab
+0000f110: 656c 3e5c 725c 6e5c 745c 745c 745c 745c  el>\r\n\t\t\t\t\
+0000f120: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
+0000f130: 745c 745c 745c 745c 745c 745c 743c 6469  t\t\t\t\t\t\t<di
+0000f140: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
+0000f150: 5c22 636f 6c2d 6d64 2d38 2063 6f6c 2d78  \"col-md-8 col-x
+0000f160: 732d 385c 223e 5c72 5c6e 5c74 5c74 5c74  s-8\">\r\n\t\t\t
+0000f170: 5c74 5c74 5c74 5c74 5c74 3c64 6976 2063  \t\t\t\t\t<div c
+0000f180: 6c61 7373 3d5c 2270 7269 6365 5c22 3e7b  lass=\"price\">{
+0000f190: 6f62 6a2e 7770 7269 6365 7d0a 2020 2020  obj.wprice}.    
+0000f1a0: 2020 2020 2665 7572 6f3b 2f74 6e3c 2f64      &euro;/tn</d
+0000f1b0: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
+0000f1c0: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
+0000f1d0: 745c 745c 745c 745c 745c 743c 2f64 6976  t\t\t\t\t\t</div
+0000f1e0: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+0000f1f0: 743a 7d5c 725c 6e5c 745c 745c 745c 745c  t:}\r\n\t\t\t\t\
+0000f200: 745c 725c 6e5c 745c 745c 745c 745c 745c  t\r\n\t\t\t\t\t\
+0000f210: 725c 6e5c 745c 745c 745c 745c 743c 6469  r\n\t\t\t\t\t<di
+0000f220: 760a 2020 2020 2020 2020 636c 6173 733d  v.        class=
+0000f230: 5c22 726f 775c 223e 5c72 5c6e 5c74 5c74  \"row\">\r\n\t\t
+0000f240: 5c74 5c74 5c74 5c74 3c64 6976 2063 6c61  \t\t\t\t<div cla
+0000f250: 7373 3d5c 2263 6f6c 2d6d 642d 3420 636f  ss=\"col-md-4 co
+0000f260: 6c2d 7873 2d34 5c22 3e5c 725c 6e5c 745c  l-xs-4\">\r\n\t\
+0000f270: 745c 745c 745c 745c 745c 743c 6c61 6265  t\t\t\t\t\t<labe
+0000f280: 6c0a 2020 2020 2020 2020 636c 6173 733d  l.        class=
+0000f290: 5c22 636f 6e74 726f 6c2d 6c61 6265 6c5c  \"control-label\
+0000f2a0: 223e 4d5c 7845 345c 7845 3472 5c78 4534  ">M\xE4\xE4r\xE4
+0000f2b0: 3c2f 6c61 6265 6c3e 5c72 5c6e 5c74 5c74  </label>\r\n\t\t
+0000f2c0: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
+0000f2d0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c64  \n\t\t\t\t\t\t<d
+0000f2e0: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+0000f2f0: 3d5c 2263 6f6c 2d6d 642d 3820 636f 6c2d  =\"col-md-8 col-
+0000f300: 7873 2d38 5c22 3e5c 725c 6e5c 745c 745c  xs-8\">\r\n\t\t\
+0000f310: 745c 745c 745c 745c 743c 6469 7620 636c  t\t\t\t\t<div cl
+0000f320: 6173 733d 5c22 616d 6f75 6e74 5c22 3e5c  ass=\"amount\">\
+0000f330: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+0000f340: 745c 745c 725c 6e5c 745c 745c 745c 745c  t\t\r\n\t\t\t\t\
+0000f350: 745c 745c 745c 745c 725c 6e5c 725c 6e5c  t\t\t\t\r\n\r\n\
+0000f360: 745c 745c 745c 745c 745c 745c 745c 745c  t\t\t\t\t\t\t\t\
+0000f370: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+0000f380: 745c 745c 743c 7365 6c65 6374 0a20 2020  t\t\t<select.   
+0000f390: 2020 2020 2069 643d 5c22 616d 6f75 6e74       id=\"amount
+0000f3a0: 5f7b 6f62 6a2e 7072 6963 6569 647d 5c22  _{obj.priceid}\"
+0000f3b0: 2063 6c61 7373 3d5c 2266 6f72 6d2d 636f   class=\"form-co
+0000f3c0: 6e74 726f 6c5c 223e 5c72 5c6e 5c74 5c74  ntrol\">\r\n\t\t
+0000f3d0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+0000f3e0: 3c6f 7074 696f 6e0a 2020 2020 2020 2020  <option.        
+0000f3f0: 7661 6c75 653d 5c22 315c 223e 313c 2f6f  value=\"1\">1</o
+0000f400: 7074 696f 6e3e 5c72 5c6e 5c74 5c74 5c74  ption>\r\n\t\t\t
+0000f410: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c6f  \t\t\t\t\t\t\t<o
+0000f420: 7074 696f 6e20 7661 6c75 653d 5c22 325c  ption value=\"2\
+0000f430: 223e 323c 2f6f 7074 696f 6e3e 5c72 5c6e  ">2</option>\r\n
+0000f440: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+0000f450: 5c74 5c74 3c6f 7074 696f 6e0a 2020 2020  \t\t<option.    
+0000f460: 2020 2020 7661 6c75 653d 5c22 335c 223e      value=\"3\">
+0000f470: 333c 2f6f 7074 696f 6e3e 5c72 5c6e 5c74  3</option>\r\n\t
+0000f480: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+0000f490: 5c74 3c6f 7074 696f 6e20 7661 6c75 653d  \t<option value=
+0000f4a0: 5c22 345c 223e 343c 2f6f 7074 696f 6e3e  \"4\">4</option>
+0000f4b0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+0000f4c0: 5c74 5c74 5c74 5c74 3c6f 7074 696f 6e0a  \t\t\t\t<option.
+0000f4d0: 2020 2020 2020 2020 7661 6c75 653d 5c22          value=\"
+0000f4e0: 355c 223e 353c 2f6f 7074 696f 6e3e 5c72  5\">5</option>\r
+0000f4f0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
+0000f500: 5c74 5c74 5c74 3c6f 7074 696f 6e20 7661  \t\t\t<option va
+0000f510: 6c75 653d 5c22 365c 223e 363c 2f6f 7074  lue=\"6\">6</opt
+0000f520: 696f 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74  ion>\r\n\t\t\t\t
+0000f530: 5c74 5c74 5c74 5c74 5c74 5c74 3c6f 7074  \t\t\t\t\t\t<opt
+0000f540: 696f 6e0a 2020 2020 2020 2020 7661 6c75  ion.        valu
+0000f550: 653d 5c22 375c 223e 373c 2f6f 7074 696f  e=\"7\">7</optio
+0000f560: 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  n>\r\n\t\t\t\t\t
+0000f570: 5c74 5c74 5c74 5c74 5c74 3c6f 7074 696f  \t\t\t\t\t<optio
+0000f580: 6e20 7661 6c75 653d 5c22 385c 223e 383c  n value=\"8\">8<
+0000f590: 2f6f 7074 696f 6e3e 5c72 5c6e 5c74 5c74  /option>\r\n\t\t
+0000f5a0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+0000f5b0: 3c6f 7074 696f 6e0a 2020 2020 2020 2020  <option.        
+0000f5c0: 7661 6c75 653d 5c22 395c 223e 393c 2f6f  value=\"9\">9</o
+0000f5d0: 7074 696f 6e3e 5c72 5c6e 5c74 5c74 5c74  ption>\r\n\t\t\t
+0000f5e0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c6f  \t\t\t\t\t\t\t<o
+0000f5f0: 7074 696f 6e20 7661 6c75 653d 5c22 3130  ption value=\"10
+0000f600: 5c22 3e31 303c 2f6f 7074 696f 6e3e 5c72  \">10</option>\r
+0000f610: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
+0000f620: 5c74 5c74 3c2f 7365 6c65 6374 3e5c 725c  \t\t</select>\r\
+0000f630: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
+0000f640: 745c 725c 6e5c 745c 745c 745c 745c 745c  t\r\n\t\t\t\t\t\
+0000f650: 745c 745c 745c 725c 6e5c 745c 745c 745c  t\t\t\r\n\t\t\t\
+0000f660: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
+0000f670: 6e5c 745c 745c 745c 745c 745c 743c 2f64  n\t\t\t\t\t\t</d
+0000f680: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
+0000f690: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
+0000f6a0: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+0000f6b0: 2020 636c 6173 733d 5c22 726f 775c 223e    class=\"row\">
+0000f6c0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+0000f6d0: 3c64 6976 2063 6c61 7373 3d5c 2263 6f6c  <div class=\"col
+0000f6e0: 2d6d 642d 3820 636f 6c2d 6d64 2d6f 6666  -md-8 col-md-off
+0000f6f0: 7365 742d 3420 636f 6c2d 7873 2d38 0a20  set-4 col-xs-8. 
+0000f700: 2020 2020 2020 2063 6f6c 2d78 732d 6f66         col-xs-of
+0000f710: 6673 6574 2d34 5c22 3e5c 725c 6e5c 745c  fset-4\">\r\n\t\
+0000f720: 745c 745c 745c 745c 745c 745c 725c 6e5c  t\t\t\t\t\t\r\n\
+0000f730: 745c 745c 745c 745c 745c 745c 745c 743c  t\t\t\t\t\t\t\t<
+0000f740: 6275 7474 6f6e 2063 6c61 7373 3d5c 2262  button class=\"b
+0000f750: 746e 0a20 2020 2020 2020 2062 746e 2d64  tn.        btn-d
+0000f760: 6566 6175 6c74 2062 746e 2d62 6c6f 636b  efault btn-block
+0000f770: 206c 6f6e 672d 7465 7874 2d62 7574 746f   long-text-butto
+0000f780: 6e5c 2220 6f6e 636c 6963 6b3d 5c22 7368  n\" onclick=\"sh
+0000f790: 6f70 7069 6e67 4361 7274 2e61 6464 5072  oppingCart.addPr
+0000f7a0: 6f64 7563 7428 277b 6f62 6a2e 7072 6963  oduct('{obj.pric
+0000f7b0: 6569 647d 272c 277b 6f62 6a2e 6e61 6d65  eid}','{obj.name
+0000f7c0: 7d27 2c24 2827 2361 6d6f 756e 745f 7b6f  }',$('#amount_{o
+0000f7d0: 626a 2e70 7269 6365 6964 7d27 292e 7661  bj.priceid}').va
+0000f7e0: 6c28 292c 277b 636f 6d6d 6f6e 2e63 6174  l(),'{common.cat
+0000f7f0: 6567 6f72 7928 297d 272c 277b 636f 6d6d  egory()}','{comm
+0000f800: 6f6e 2e63 6f6d 6269 6e65 6456 6174 5072  on.combinedVatPr
+0000f810: 6963 6528 297d 2729 5c22 3e5c 725c 6e5c  ice()}')\">\r\n\
+0000f820: 745c 745c 745c 745c 745c 745c 745c 745c  t\t\t\t\t\t\t\t\
+0000f830: 744b 6f72 6969 6e5c 725c 6e5c 745c 745c  tKoriin\r\n\t\t\
+0000f840: 745c 745c 745c 745c 745c 743c 2f62 7574  t\t\t\t\t\t</but
+0000f850: 746f 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74  ton>\r\n\t\t\t\t
+0000f860: 5c74 5c74 5c74 5c72 5c6e 5c74 5c74 5c74  \t\t\t\r\n\t\t\t
+0000f870: 5c74 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \t\t\t\t\r\n\t\t
+0000f880: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
+0000f890: 5c6e 5c74 5c74 5c74 5c74 5c74 3c2f 6469  \n\t\t\t\t\t</di
+0000f8a0: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f  v>\r\n\t\t\t\t</
+0000f8b0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 3c2f  div>\r\n\t\t\t</
+0000f8c0: 6469 763e 5c72 5c6e 5c74 5c74 3c2f 6469  div>\r\n\t\t</di
+0000f8d0: 763e 5c72 5c6e 5c74 3c2f 6469 763e 5c72  v>\r\n\t</div>\r
+0000f8e0: 5c6e 3c2f 7465 7874 6172 6561 3e5c 745c  \n</textarea>\t\
+0000f8f0: 725c 6e5c 725c 6e5c 725c 6e5c 725c 6e3c  r\n\r\n\r\n\r\n<
+0000f900: 6469 760a 2020 2020 2020 2020 6964 3d5c  div.        id=\
+0000f910: 2276 6964 656f 2d70 6f70 7570 2d6d 6f64  "video-popup-mod
+0000f920: 616c 5c22 2063 6c61 7373 3d5c 226d 6f64  al\" class=\"mod
+0000f930: 616c 5c22 2073 7479 6c65 3d5c 2264 6973  al\" style=\"dis
+0000f940: 706c 6179 3a6e 6f6e 655c 223e 5c72 5c6e  play:none\">\r\n
+0000f950: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
+0000f960: 6c61 7373 3d5c 226d 6f64 616c 2d64 6961  lass=\"modal-dia
+0000f970: 6c6f 6720 6d6f 6461 6c2d 6c67 5c22 3e5c  log modal-lg\">\
+0000f980: 725c 6e5c 745c 743c 6469 7620 636c 6173  r\n\t\t<div clas
+0000f990: 733d 5c22 6d6f 6461 6c2d 636f 6e74 656e  s=\"modal-conten
+0000f9a0: 745c 223e 5c72 5c6e 5c74 5c74 5c74 3c64  t\">\r\n\t\t\t<d
+0000f9b0: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+0000f9c0: 3d5c 226d 6f64 616c 2d62 6f64 795c 223e  =\"modal-body\">
+0000f9d0: 5c72 5c6e 5c74 5c74 5c74 5c74 3c64 6976  \r\n\t\t\t\t<div
+0000f9e0: 2063 6c61 7373 3d5c 2265 6d62 6564 2d72   class=\"embed-r
+0000f9f0: 6573 706f 6e73 6976 6520 656d 6265 642d  esponsive embed-
+0000fa00: 7265 7370 6f6e 7369 7665 2d34 6279 335c  responsive-4by3\
+0000fa10: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
+0000fa20: 3c76 6964 656f 0a20 2020 2020 2020 2063  <video.        c
+0000fa30: 6f6e 7472 6f6c 733e 5c72 5c6e 5c74 5c74  ontrols>\r\n\t\t
+0000fa40: 5c74 5c74 5c74 5c74 5365 6c61 696d 6573  \t\t\t\tSelaimes
+0000fa50: 6920 6569 2074 7565 2048 544d 4c35 2d76  i ei tue HTML5-v
+0000fa60: 6964 656f 612e 203c 6120 6872 6566 3d5c  ideoa. <a href=\
+0000fa70: 2223 5c22 2064 6174 612d 726f 6c65 3d5c  "#\" data-role=\
+0000fa80: 2264 6f77 6e6c 6f61 645c 223e 4c61 7461  "download\">Lata
+0000fa90: 610a 2020 2020 2020 2020 7669 6465 6f2e  a.        video.
+0000faa0: 3c2f 613e 5c72 5c6e 5c74 5c74 5c74 5c74  </a>\r\n\t\t\t\t
+0000fab0: 5c74 3c2f 7669 6465 6f3e 5c72 5c6e 5c74  \t</video>\r\n\t
+0000fac0: 5c74 5c74 5c74 5c74 3c69 6672 616d 6520  \t\t\t\t<iframe 
+0000fad0: 6672 616d 6562 6f72 6465 723d 5c22 305c  frameborder=\"0\
+0000fae0: 2220 7765 626b 6974 616c 6c6f 7766 756c  " webkitallowful
+0000faf0: 6c73 6372 6565 6e0a 2020 2020 2020 2020  lscreen.        
+0000fb00: 6d6f 7a61 6c6c 6f77 6675 6c6c 7363 7265  mozallowfullscre
+0000fb10: 656e 2061 6c6c 6f77 6675 6c6c 7363 7265  en allowfullscre
+0000fb20: 656e 3e3c 2f69 6672 616d 653e 5c72 5c6e  en></iframe>\r\n
+0000fb30: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
+0000fb40: 5c6e 5c72 5c6e 5c74 5c74 5c74 5c74 3c64  \n\r\n\t\t\t\t<d
+0000fb50: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+0000fb60: 3d5c 2266 6f72 6d2d 6275 7474 6f6e 7320  =\"form-buttons 
+0000fb70: 7465 7874 2d63 656e 7465 725c 223e 5c72  text-center\">\r
+0000fb80: 5c6e 5c74 5c74 5c74 5c74 5c74 3c62 7574  \n\t\t\t\t\t<but
+0000fb90: 746f 6e20 636c 6173 733d 5c22 6274 6e20  ton class=\"btn 
+0000fba0: 6274 6e2d 7072 696d 6172 795c 220a 2020  btn-primary\".  
+0000fbb0: 2020 2020 2020 6461 7461 2d64 6973 6d69        data-dismi
+0000fbc0: 7373 3d5c 226d 6f64 616c 5c22 3e53 756c  ss=\"modal\">Sul
+0000fbd0: 6a65 3c2f 6275 7474 6f6e 3e5c 725c 6e5c  je</button>\r\n\
+0000fbe0: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
+0000fbf0: 6e5c 745c 745c 743c 2f64 6976 3e5c 725c  n\t\t\t</div>\r\
+0000fc00: 6e5c 745c 743c 2f64 6976 3e5c 725c 6e5c  n\t\t</div>\r\n\
+0000fc10: 743c 2f64 6976 3e5c 725c 6e3c 2f64 6976  t</div>\r\n</div
+0000fc20: 3e5c 725c 6e5c 725c 6e5c 725c 6e3c 6469  >\r\n\r\n\r\n<di
+0000fc30: 760a 2020 2020 2020 2020 6964 3d5c 2261  v.        id=\"a
+0000fc40: 6c65 7274 2d6d 6f64 616c 5c22 2063 6c61  lert-modal\" cla
+0000fc50: 7373 3d5c 226d 6f64 616c 5c22 2073 7479  ss=\"modal\" sty
+0000fc60: 6c65 3d5c 2264 6973 706c 6179 3a6e 6f6e  le=\"display:non
+0000fc70: 655c 223e 5c72 5c6e 5c74 3c64 6976 2063  e\">\r\n\t<div c
+0000fc80: 6c61 7373 3d5c 226d 6f64 616c 2d64 6961  lass=\"modal-dia
+0000fc90: 6c6f 670a 2020 2020 2020 2020 6d6f 6461  log.        moda
+0000fca0: 6c2d 736d 5c22 3e5c 725c 6e5c 745c 743c  l-sm\">\r\n\t\t<
+0000fcb0: 6469 7620 636c 6173 733d 5c22 6d6f 6461  div class=\"moda
+0000fcc0: 6c2d 636f 6e74 656e 745c 223e 5c72 5c6e  l-content\">\r\n
+0000fcd0: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
+0000fce0: 3d5c 226d 6f64 616c 2d62 6f64 795c 223e  =\"modal-body\">
+0000fcf0: 5c72 5c6e 5c74 5c74 5c74 5c74 3c64 6976  \r\n\t\t\t\t<div
+0000fd00: 0a20 2020 2020 2020 2064 6174 612d 726f  .        data-ro
+0000fd10: 6c65 3d5c 2274 6578 745c 223e 3c2f 6469  le=\"text\"></di
+0000fd20: 763e 5c72 5c6e 5c74 5c74 5c74 3c2f 6469  v>\r\n\t\t\t</di
+0000fd30: 763e 5c72 5c6e 5c74 5c74 5c74 3c64 6976  v>\r\n\t\t\t<div
+0000fd40: 2063 6c61 7373 3d5c 226d 6f64 616c 2d66   class=\"modal-f
+0000fd50: 6f6f 7465 725c 223e 5c72 5c6e 5c74 5c74  ooter\">\r\n\t\t
+0000fd60: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
+0000fd70: 2063 6c61 7373 3d5c 2274 6578 742d 7269   class=\"text-ri
+0000fd80: 6768 745c 223e 5c72 5c6e 5c74 5c74 5c74  ght\">\r\n\t\t\t
+0000fd90: 5c74 5c74 3c62 7574 746f 6e20 636c 6173  \t\t<button clas
+0000fda0: 733d 5c22 6274 6e20 6274 6e2d 7072 696d  s=\"btn btn-prim
+0000fdb0: 6172 795c 2220 6461 7461 2d61 6374 696f  ary\" data-actio
+0000fdc0: 6e3d 5c22 6f6b 5c22 0a20 2020 2020 2020  n=\"ok\".       
+0000fdd0: 2064 6174 612d 6469 736d 6973 733d 5c22   data-dismiss=\"
+0000fde0: 6d6f 6461 6c5c 223e 3c2f 6275 7474 6f6e  modal\"></button
+0000fdf0: 3e5c 725c 6e5c 745c 745c 745c 743c 2f64  >\r\n\t\t\t\t</d
+0000fe00: 6976 3e5c 725c 6e5c 745c 745c 743c 2f64  iv>\r\n\t\t\t</d
+0000fe10: 6976 3e5c 725c 6e5c 745c 743c 2f64 6976  iv>\r\n\t\t</div
+0000fe20: 3e5c 725c 6e5c 743c 2f64 6976 3e5c 725c  >\r\n\t</div>\r\
+0000fe30: 6e3c 2f64 6976 3e5c 725c 6e5c 725c 6e3c  n</div>\r\n\r\n<
+0000fe40: 6469 760a 2020 2020 2020 2020 6964 3d5c  div.        id=\
+0000fe50: 2263 6f6e 6669 726d 2d6d 6f64 616c 5c22  "confirm-modal\"
+0000fe60: 2063 6c61 7373 3d5c 226d 6f64 616c 5c22   class=\"modal\"
+0000fe70: 2073 7479 6c65 3d5c 2264 6973 706c 6179   style=\"display
+0000fe80: 3a6e 6f6e 655c 223e 5c72 5c6e 5c74 3c64  :none\">\r\n\t<d
+0000fe90: 6976 2063 6c61 7373 3d5c 226d 6f64 616c  iv class=\"modal
+0000fea0: 2d64 6961 6c6f 670a 2020 2020 2020 2020  -dialog.        
+0000feb0: 6d6f 6461 6c2d 736d 5c22 3e5c 725c 6e5c  modal-sm\">\r\n\
+0000fec0: 745c 743c 6469 7620 636c 6173 733d 5c22  t\t<div class=\"
+0000fed0: 6d6f 6461 6c2d 636f 6e74 656e 745c 223e  modal-content\">
+0000fee0: 5c72 5c6e 5c74 5c74 5c74 3c64 6976 2063  \r\n\t\t\t<div c
+0000fef0: 6c61 7373 3d5c 226d 6f64 616c 2d62 6f64  lass=\"modal-bod
+0000ff00: 795c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  y\">\r\n\t\t\t\t
+0000ff10: 3c64 6976 0a20 2020 2020 2020 2064 6174  <div.        dat
+0000ff20: 612d 726f 6c65 3d5c 2274 6578 745c 223e  a-role=\"text\">
+0000ff30: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
+0000ff40: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
+0000ff50: 3c64 6976 2063 6c61 7373 3d5c 226d 6f64  <div class=\"mod
+0000ff60: 616c 2d66 6f6f 7465 725c 223e 5c72 5c6e  al-footer\">\r\n
+0000ff70: 5c74 5c74 5c74 5c74 3c64 6976 0a20 2020  \t\t\t\t<div.   
+0000ff80: 2020 2020 2063 6c61 7373 3d5c 2274 6578       class=\"tex
+0000ff90: 742d 7269 6768 745c 223e 5c72 5c6e 5c74  t-right\">\r\n\t
+0000ffa0: 5c74 5c74 5c74 5c74 3c62 7574 746f 6e20  \t\t\t\t<button 
+0000ffb0: 636c 6173 733d 5c22 6274 6e20 6274 6e2d  class=\"btn btn-
+0000ffc0: 7072 696d 6172 795c 2220 6461 7461 2d61  primary\" data-a
+0000ffd0: 6374 696f 6e3d 5c22 6f6b 5c22 3e3c 2f62  ction=\"ok\"></b
+0000ffe0: 7574 746f 6e3e 5c72 5c6e 5c74 5c74 5c74  utton>\r\n\t\t\t
+0000fff0: 5c74 5c74 3c62 7574 746f 6e0a 2020 2020  \t\t<button.    
+00010000: 2020 2020 636c 6173 733d 5c22 6274 6e20      class=\"btn 
+00010010: 6274 6e2d 6465 6661 756c 745c 2220 6461  btn-default\" da
+00010020: 7461 2d61 6374 696f 6e3d 5c22 6361 6e63  ta-action=\"canc
+00010030: 656c 5c22 3e3c 2f62 7574 746f 6e3e 5c72  el\"></button>\r
+00010040: 5c6e 5c74 5c74 5c74 5c74 3c2f 6469 763e  \n\t\t\t\t</div>
+00010050: 5c72 5c6e 5c74 5c74 5c74 3c2f 6469 763e  \r\n\t\t\t</div>
+00010060: 5c72 5c6e 5c74 5c74 3c2f 6469 763e 5c72  \r\n\t\t</div>\r
+00010070: 5c6e 5c74 3c2f 6469 763e 5c72 5c6e 3c2f  \n\t</div>\r\n</
+00010080: 6469 763e 5c72 5c6e 5c72 5c6e 3c73 6372  div>\r\n\r\n<scr
+00010090: 6970 743e 5c72 5c6e 5c72 5c6e 6675 6e63  ipt>\r\n\r\nfunc
+000100a0: 7469 6f6e 0a20 2020 2020 2020 2073 686f  tion.        sho
+000100b0: 7741 6c65 7274 2874 7970 652c 2074 6578  wAlert(type, tex
+000100c0: 742c 206f 6b54 6578 7429 207b 5c72 5c6e  t, okText) {\r\n
+000100d0: 2020 2020 7661 7220 246d 6f64 616c 203d      var $modal =
+000100e0: 2024 2827 2361 6c65 7274 2d6d 6f64 616c   $('#alert-modal
+000100f0: 2729 3b5c 725c 6e0a 2020 2020 2020 2020  ');\r\n.        
+00010100: 5c20 2020 7661 7220 6465 6665 7272 6564  \   var deferred
+00010110: 203d 206e 6577 2024 2e44 6566 6572 7265   = new $.Deferre
+00010120: 6428 293b 5c72 5c6e 5c72 5c6e 2020 2020  d();\r\n\r\n    
+00010130: 246d 6f64 616c 2e66 696e 6428 275b 6461  $modal.find('[da
+00010140: 7461 2d72 6f6c 653d 5c22 7465 7874 5c22  ta-role=\"text\"
+00010150: 5d27 292e 6874 6d6c 2874 6578 7429 3b5c  ]').html(text);\
+00010160: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00010170: 6966 2874 7970 656f 6620 6f6b 5465 7874  if(typeof okText
+00010180: 203d 3d3d 2027 756e 6465 6669 6e65 6427   === 'undefined'
+00010190: 2920 7b5c 725c 6e20 2020 2020 2020 206f  ) {\r\n        o
+000101a0: 6b54 6578 7420 3d20 274f 6b27 3b5c 725c  kText = 'Ok';\r\
+000101b0: 6e20 2020 207d 5c72 5c6e 0a20 2020 2020  n    }\r\n.     
+000101c0: 2020 205c 2020 2024 6d6f 6461 6c2e 6669     \   $modal.fi
+000101d0: 6e64 2827 5b64 6174 612d 6163 7469 6f6e  nd('[data-action
+000101e0: 3d5c 226f 6b5c 225d 2729 2e68 746d 6c28  =\"ok\"]').html(
+000101f0: 6f6b 5465 7874 293b 5c72 5c6e 5c72 5c6e  okText);\r\n\r\n
+00010200: 2020 2020 246d 6f64 616c 2e6d 6f64 616c      $modal.modal
+00010210: 2827 7368 6f77 2729 3b5c 725c 6e0a 2020  ('show');\r\n.  
+00010220: 2020 2020 2020 5c20 2020 246d 6f64 616c        \   $modal
+00010230: 2e6f 6e28 2768 6964 6465 6e2e 6273 2e6d  .on('hidden.bs.m
+00010240: 6f64 616c 272c 2066 756e 6374 696f 6e28  odal', function(
+00010250: 6529 207b 5c72 5c6e 2020 2020 2020 2020  e) {\r\n        
+00010260: 6465 6665 7272 6564 2e72 6573 6f6c 7665  deferred.resolve
+00010270: 2829 3b5c 725c 6e0a 2020 2020 2020 2020  ();\r\n.        
+00010280: 5c20 2020 7d29 3b5c 725c 6e20 2020 2072  \   });\r\n    r
+00010290: 6574 7572 6e20 6465 6665 7272 6564 3b5c  eturn deferred;\
+000102a0: 725c 6e7d 5c72 5c6e 5c72 5c6e 6675 6e63  r\n}\r\n\r\nfunc
+000102b0: 7469 6f6e 2073 686f 7743 6f6e 6669 726d  tion showConfirm
+000102c0: 2874 7970 652c 2074 6578 742c 0a20 2020  (type, text,.   
+000102d0: 2020 2020 206f 6b54 6578 742c 2063 616e       okText, can
+000102e0: 6365 6c54 6578 7429 207b 5c72 5c6e 2020  celText) {\r\n  
+000102f0: 2020 7661 7220 246d 6f64 616c 203d 2024    var $modal = $
+00010300: 2827 2363 6f6e 6669 726d 2d6d 6f64 616c  ('#confirm-modal
+00010310: 2729 3b5c 725c 6e20 2020 2076 6172 0a20  ');\r\n    var. 
+00010320: 2020 2020 2020 2064 6566 6572 7265 6420         deferred 
+00010330: 3d20 6e65 7720 242e 4465 6665 7272 6564  = new $.Deferred
+00010340: 2829 3b5c 725c 6e5c 725c 6e20 2020 2024  ();\r\n\r\n    $
+00010350: 6d6f 6461 6c2e 6669 6e64 2827 5b64 6174  modal.find('[dat
+00010360: 612d 726f 6c65 3d5c 2274 6578 745c 225d  a-role=\"text\"]
+00010370: 2729 2e68 746d 6c28 7465 7874 293b 5c72  ').html(text);\r
+00010380: 5c6e 0a20 2020 2020 2020 205c 2020 2069  \n.        \   i
+00010390: 6628 7479 7065 6f66 206f 6b54 6578 7420  f(typeof okText 
+000103a0: 3d3d 3d20 2775 6e64 6566 696e 6564 2729  === 'undefined')
+000103b0: 207b 5c72 5c6e 2020 2020 2020 2020 6f6b   {\r\n        ok
+000103c0: 5465 7874 203d 205c 224f 6b5c 223b 5c72  Text = \"Ok\";\r
+000103d0: 5c6e 2020 2020 7d5c 725c 6e0a 2020 2020  \n    }\r\n.    
+000103e0: 2020 2020 5c20 2020 246d 6f64 616c 2e66      \   $modal.f
+000103f0: 696e 6428 275b 6461 7461 2d61 6374 696f  ind('[data-actio
+00010400: 6e3d 5c22 6f6b 5c22 5d27 292e 6874 6d6c  n=\"ok\"]').html
+00010410: 286f 6b54 6578 7429 3b5c 725c 6e20 2020  (okText);\r\n   
+00010420: 2069 6628 7479 7065 6f66 2063 616e 6365   if(typeof cance
+00010430: 6c54 6578 740a 2020 2020 2020 2020 3d3d  lText.        ==
+00010440: 3d20 2775 6e64 6566 696e 6564 2729 207b  = 'undefined') {
+00010450: 5c72 5c6e 2020 2020 2020 2020 6361 6e63  \r\n        canc
+00010460: 656c 5465 7874 203d 205c 2250 6572 7575  elText = \"Peruu
+00010470: 7461 5c22 3b5c 725c 6e20 2020 207d 5c72  ta\";\r\n    }\r
+00010480: 5c6e 2020 2020 246d 6f64 616c 2e66 696e  \n    $modal.fin
+00010490: 6428 275b 6461 7461 2d61 6374 696f 6e3d  d('[data-action=
+000104a0: 5c22 6361 6e63 656c 5c22 5d27 292e 6874  \"cancel\"]').ht
+000104b0: 6d6c 2863 616e 6365 6c54 6578 7429 3b5c  ml(cancelText);\
+000104c0: 725c 6e5c 725c 6e0a 2020 2020 2020 2020  r\n\r\n.        
+000104d0: 5c20 2020 246d 6f64 616c 2e66 696e 6428  \   $modal.find(
+000104e0: 275b 6461 7461 2d61 6374 696f 6e3d 5c22  '[data-action=\"
+000104f0: 6f6b 5c22 5d27 292e 6f66 6628 2763 6c69  ok\"]').off('cli
+00010500: 636b 2729 2e6f 6e28 2763 6c69 636b 272c  ck').on('click',
+00010510: 2066 756e 6374 696f 6e28 6529 0a20 2020   function(e).   
+00010520: 2020 2020 207b 5c72 5c6e 2020 2020 2020       {\r\n      
+00010530: 2020 246d 6f64 616c 2e6d 6f64 616c 2827    $modal.modal('
+00010540: 6869 6465 2729 3b5c 725c 6e20 2020 2020  hide');\r\n     
+00010550: 2020 2064 6566 6572 7265 642e 7265 736f     deferred.reso
+00010560: 6c76 6528 7472 7565 293b 5c72 5c6e 0a20  lve(true);\r\n. 
+00010570: 2020 2020 2020 205c 2020 207d 293b 5c72         \   });\r
+00010580: 5c6e 2020 2020 246d 6f64 616c 2e66 696e  \n    $modal.fin
+00010590: 6428 275b 6461 7461 2d61 6374 696f 6e3d  d('[data-action=
+000105a0: 5c22 6361 6e63 656c 5c22 5d27 292e 6f66  \"cancel\"]').of
+000105b0: 6628 2763 6c69 636b 2729 2e6f 6e28 2763  f('click').on('c
+000105c0: 6c69 636b 272c 0a20 2020 2020 2020 2066  lick',.        f
+000105d0: 756e 6374 696f 6e28 6529 207b 5c72 5c6e  unction(e) {\r\n
+000105e0: 2020 2020 2020 2020 246d 6f64 616c 2e6d          $modal.m
+000105f0: 6f64 616c 2827 6869 6465 2729 3b5c 725c  odal('hide');\r\
+00010600: 6e20 2020 2020 2020 2064 6566 6572 7265  n        deferre
+00010610: 642e 7265 6a65 6374 2866 616c 7365 293b  d.reject(false);
+00010620: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+00010630: 207d 293b 5c72 5c6e 5c72 5c6e 2020 2020   });\r\n\r\n    
+00010640: 246d 6f64 616c 2e6d 6f64 616c 2827 7368  $modal.modal('sh
+00010650: 6f77 2729 3b5c 725c 6e20 2020 2072 6574  ow');\r\n    ret
+00010660: 7572 6e20 6465 6665 7272 6564 3b5c 725c  urn deferred;\r\
+00010670: 6e7d 5c72 5c6e 5c72 5c6e 3c2f 7363 7269  n}\r\n\r\n</scri
+00010680: 7074 3e5c 725c 6e5c 725c 6e5c 725c 6e5c  pt>\r\n\r\n\r\n\
+00010690: 725c 6e5c 725c 6e5c 725c 6e5c 725c 6e3c  r\n\r\n\r\n\r\n<
+000106a0: 7363 7269 7074 0a20 2020 2020 2020 2069  script.        i
+000106b0: 643d 5c22 7365 7276 6963 652d 6c69 7374  d=\"service-list
+000106c0: 2d69 7465 6d2d 7465 6d70 6c61 7465 5c22  -item-template\"
+000106d0: 2074 7970 653d 5c22 7465 7874 2f78 2d74   type=\"text/x-t
+000106e0: 656d 706c 6174 655c 223e 5c72 5c6e 5c72  emplate\">\r\n\r
+000106f0: 5c6e 5c72 5c6e 3c66 6965 6c64 7365 740a  \n\r\n<fieldset.
+00010700: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+00010710: 7365 7276 6963 652d 6974 656d 5c22 3e5c  service-item\">\
+00010720: 725c 6e5c 743c 6c65 6765 6e64 2063 6c61  r\n\t<legend cla
+00010730: 7373 3d5c 2273 6572 7669 6365 2d6e 616d  ss=\"service-nam
+00010740: 655c 223e 3c2f 6c65 6765 6e64 3e5c 725c  e\"></legend>\r\
+00010750: 6e5c 725c 6e5c 743c 6469 760a 2020 2020  n\r\n\t<div.    
+00010760: 2020 2020 636c 6173 733d 5c22 6b69 6d70      class=\"kimp
+00010770: 7061 2d69 6e66 6f20 726f 775c 223e 5c72  pa-info row\">\r
+00010780: 5c6e 5c74 5c74 5c72 5c6e 5c72 5c6e 5c74  \n\t\t\r\n\r\n\t
+00010790: 5c74 5c72 5c6e 5c74 5c74 5c74 3c64 6976  \t\r\n\t\t\t<div
+000107a0: 2063 6c61 7373 3d5c 2263 6f6c 2d6d 642d   class=\"col-md-
+000107b0: 3132 5c22 3e5c 725c 6e5c 745c 745c 745c  12\">\r\n\t\t\t\
+000107c0: 743c 646c 3e5c 725c 6e5c 745c 745c 745c  t<dl>\r\n\t\t\t\
+000107d0: 745c 743c 6c61 6265 6c0a 2020 2020 2020  t\t<label.      
+000107e0: 2020 636c 6173 733d 5c22 6b69 6d70 616e    class=\"kimpan
+000107f0: 2d69 7361 6e74 615c 223e 3c2f 6c61 6265  -isanta\"></labe
+00010800: 6c3e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  l>\r\n\t\t\t\t\t
+00010810: 3c6c 6162 656c 2063 6c61 7373 3d5c 2269  <label class=\"i
+00010820: 7361 6e6e 616e 2d6f 736f 6974 655c 223e  sannan-osoite\">
+00010830: 3c2f 6c61 6265 6c3e 5c72 5c6e 5c74 5c74  </label>\r\n\t\t
+00010840: 5c74 5c74 5c74 3c6c 6162 656c 3e3c 6c61  \t\t\t<label><la
+00010850: 6265 6c0a 2020 2020 2020 2020 636c 6173  bel.        clas
+00010860: 733d 5c22 6b69 6d70 616e 2d6a 6173 656e  s=\"kimpan-jasen
+00010870: 7465 6e2d 6d61 6172 615c 223e 3c2f 6c61  ten-maara\"></la
+00010880: 6265 6c3e 206f 7361 6b61 7374 613c 2f6c  bel> osakasta</l
+00010890: 6162 656c 3e5c 725c 6e5c 745c 745c 745c  abel>\r\n\t\t\t\
+000108a0: 745c 743c 6c61 6265 6c3e 6c61 736b 7574  t\t<label>laskut
+000108b0: 7573 6f73 7575 730a 2020 2020 2020 2020  usosuus.        
+000108c0: 3c6c 6162 656c 2063 6c61 7373 3d5c 224b  <label class=\"K
+000108d0: 4952 5072 6f73 5c22 3e3c 2f6c 6162 656c  IRPros\"></label
+000108e0: 3e3c 2f6c 6162 656c 3e5c 725c 6e5c 745c  ></label>\r\n\t\
+000108f0: 745c 745c 743c 2f64 6c3e 5c72 5c6e 5c74  t\t\t</dl>\r\n\t
+00010900: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c72  \t\t</div>\r\n\r
+00010910: 5c6e 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \n\t\t\t\r\n\t\t
+00010920: 5c72 5c6e 5c72 5c6e 5c74 3c2f 6469 763e  \r\n\r\n\t</div>
+00010930: 5c72 5c6e 5c72 5c6e 5c74 3c64 6976 0a20  \r\n\r\n\t<div. 
+00010940: 2020 2020 2020 2063 6c61 7373 3d5c 2272         class=\"r
+00010950: 6f77 5c22 2064 6174 612d 6865 6164 6572  ow\" data-header
+00010960: 3d5c 2241 5354 4b6f 6d6d 5c22 3e5c 725c  =\"ASTKomm\">\r\
+00010970: 6e5c 745c 743c 6469 7620 636c 6173 733d  n\t\t<div class=
+00010980: 5c22 636f 6c2d 6d64 2d6f 6666 7365 742d  \"col-md-offset-
+00010990: 320a 2020 2020 2020 2020 636f 6c2d 6d64  2.        col-md
+000109a0: 2d37 5c22 3e5c 725c 6e5c 745c 745c 743c  -7\">\r\n\t\t\t<
+000109b0: 7020 6461 7461 2d76 616c 7565 3d5c 2241  p data-value=\"A
+000109c0: 5354 4b6f 6d6d 5c22 3e3c 2f70 3e5c 725c  STKomm\"></p>\r\
+000109d0: 6e5c 745c 743c 2f64 6976 3e5c 725c 6e5c  n\t\t</div>\r\n\
+000109e0: 743c 2f64 6976 3e5c 725c 6e5c 725c 6e5c  t</div>\r\n\r\n\
+000109f0: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
+00010a00: 6173 733d 5c22 726f 775c 223e 5c72 5c6e  ass=\"row\">\r\n
+00010a10: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
+00010a20: 2263 6f6c 2d6d 642d 325c 223e 5c72 5c6e  "col-md-2\">\r\n
+00010a30: 5c74 5c74 5c74 3c69 6d67 2063 6c61 7373  \t\t\t<img class
+00010a40: 3d5c 2273 6572 7669 6365 2d69 6d61 6765  =\"service-image
+00010a50: 0a20 2020 2020 2020 2069 6d67 2d72 6573  .        img-res
+00010a60: 706f 6e73 6976 655c 2220 616c 743d 5c22  ponsive\" alt=\"
+00010a70: 5c22 206f 6e65 7272 6f72 3d5c 2274 6869  \" onerror=\"thi
+00010a80: 732e 7374 796c 652e 7669 7369 6269 6c69  s.style.visibili
+00010a90: 7479 3d27 6869 6464 656e 273b 7265 7475  ty='hidden';retu
+00010aa0: 726e 0a20 2020 2020 2020 2074 7275 655c  rn.        true\
+00010ab0: 223e 5c72 5c6e 5c74 5c74 3c2f 6469 763e  ">\r\n\t\t</div>
+00010ac0: 5c72 5c6e 5c72 5c6e 5c74 5c74 3c64 6976  \r\n\r\n\t\t<div
+00010ad0: 2063 6c61 7373 3d5c 2263 6f6c 2d6d 642d   class=\"col-md-
+00010ae0: 375c 223e 5c72 5c6e 5c74 5c74 5c74 3c64  7\">\r\n\t\t\t<d
+00010af0: 6976 2063 6c61 7373 3d5c 2273 6572 7669  iv class=\"servi
+00010b00: 6365 2d69 6e66 6f5c 223e 5c72 5c6e 5c74  ce-info\">\r\n\t
+00010b10: 5c74 5c74 5c74 5c72 5c6e 5c72 5c6e 5c74  \t\t\t\r\n\r\n\t
+00010b20: 5c74 5c74 5c74 5c72 5c6e 5c74 5c74 5c74  \t\t\t\r\n\t\t\t
+00010b30: 5c74 3c64 6976 0a20 2020 2020 2020 2064  \t<div.        d
+00010b40: 6174 612d 6865 6164 6572 3d5c 2241 5354  ata-header=\"AST
+00010b50: 4d61 6172 615c 223e 5c72 5c6e 5c74 5c74  Maara\">\r\n\t\t
+00010b60: 5c74 5c74 5c74 3c73 7061 6e20 6461 7461  \t\t\t<span data
+00010b70: 2d76 616c 7565 3d5c 2241 5354 4d61 6172  -value=\"ASTMaar
+00010b80: 615c 223e 3c2f 7370 616e 3e3c 7370 616e  a\"></span><span
+00010b90: 3e0a 2020 2020 2020 2020 3c2f 7370 616e  >.        </span
+00010ba0: 3e3c 7370 616e 2064 6174 612d 7661 6c75  ><span data-valu
+00010bb0: 653d 5c22 7461 7269 6666 2e75 6e69 745c  e=\"tariff.unit\
+00010bc0: 223e 6b70 6c2f 743c 2f73 7061 6e3e 5c72  ">kpl/t</span>\r
+00010bd0: 5c6e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  \n\r\n\t\t\t\t\t
+00010be0: 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f 6469  \r\n\t\t\t\t</di
+00010bf0: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 5c72  v>\r\n\t\t\t\t\r
+00010c00: 5c6e 5c72 5c6e 5c74 5c74 5c74 5c74 5c72  \n\r\n\t\t\t\t\r
+00010c10: 5c6e 5c74 5c74 5c74 5c74 5c74 3c64 6976  \n\t\t\t\t\t<div
+00010c20: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+00010c30: 2263 6f6c 6c65 6374 696f 6e2d 7363 6865  "collection-sche
+00010c40: 6475 6c65 5c22 3e3c 6120 6872 6566 3d5c  dule\"><a href=\
+00010c50: 225c 2220 6461 7461 2d61 6374 696f 6e3d  "\" data-action=
+00010c60: 5c22 636f 6c6c 6563 7469 6f6e 2d73 6368  \"collection-sch
+00010c70: 6564 756c 655c 223e 5c78 4242 0a20 2020  edule\">\xBB.   
+00010c80: 2020 2020 2054 7968 6a65 6e6e 7973 7279       Tyhjennysry
+00010c90: 746d 693c 2f61 3e3c 2f64 6976 3e5c 725c  tmi</a></div>\r\
+00010ca0: 6e5c 745c 745c 745c 745c 725c 6e5c 725c  n\t\t\t\t\r\n\r\
+00010cb0: 6e5c 745c 745c 745c 745c 725c 6e5c 725c  n\t\t\t\t\r\n\r\
+00010cc0: 6e5c 745c 745c 745c 745c 725c 6e5c 725c  n\t\t\t\t\r\n\r\
+00010cd0: 6e5c 745c 745c 745c 745c 725c 6e5c 725c  n\t\t\t\t\r\n\r\
+00010ce0: 6e5c 745c 745c 745c 745c 725c 6e5c 725c  n\t\t\t\t\r\n\r\
+00010cf0: 6e5c 745c 745c 745c 745c 725c 6e5c 725c  n\t\t\t\t\r\n\r\
+00010d00: 6e5c 745c 745c 745c 745c 725c 6e5c 745c  n\t\t\t\t\r\n\t\
+00010d10: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+00010d20: 2020 6461 7461 2d68 6561 6465 723d 5c22    data-header=\"
+00010d30: 4153 544e 6578 7444 6174 655c 223e 5c72  ASTNextDate\">\r
+00010d40: 5c6e 5c74 5c74 5c74 5c74 5c74 3c64 6976  \n\t\t\t\t\t<div
+00010d50: 2064 6174 612d 6865 6164 6572 3d5c 2241   data-header=\"A
+00010d60: 5354 4e65 7874 4461 7465 5c22 3e5c 725c  STNextDate\">\r\
+00010d70: 6e5c 745c 745c 745c 745c 745c 743c 7370  n\t\t\t\t\t\t<sp
+00010d80: 616e 3e53 6575 7261 6176 610a 2020 2020  an>Seuraava.    
+00010d90: 2020 2020 7479 686a 656e 6e79 7320 3c2f      tyhjennys </
+00010da0: 7370 616e 3e5c 725c 6e5c 745c 745c 745c  span>\r\n\t\t\t\
+00010db0: 745c 745c 743c 7370 616e 2064 6174 612d  t\t\t<span data-
+00010dc0: 7661 6c75 653d 5c22 4153 544e 6578 7444  value=\"ASTNextD
+00010dd0: 6174 655c 223e 3c2f 7370 616e 3e5c 725c  ate\"></span>\r\
+00010de0: 6e5c 745c 745c 745c 745c 745c 743c 7370  n\t\t\t\t\t\t<sp
+00010df0: 616e 0a20 2020 2020 2020 2064 6174 612d  an.        data-
+00010e00: 726f 6c65 3d5c 226e 6578 742d 656d 7074  role=\"next-empt
+00010e10: 7969 6e67 2d76 6172 6961 6e63 652d 7465  ying-variance-te
+00010e20: 7874 5c22 3e5c 725c 6e5c 745c 745c 745c  xt\">\r\n\t\t\t\
+00010e30: 745c 745c 745c 7420 285c 7842 3120 312d  t\t\t\t (\xB1 1-
+00010e40: 3220 705c 7845 3469 765c 7845 345c 7845  2 p\xE4iv\xE4\xE
+00010e50: 3429 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  4)\r\n\t\t\t\t\t
+00010e60: 5c74 3c2f 7370 616e 3e5c 725c 6e0a 2020  \t</span>\r\n.  
+00010e70: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+00010e80: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+00010e90: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00010ea0: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
+00010eb0: 2064 6174 612d 726f 6c65 3d5c 226e 6578   data-role=\"nex
+00010ec0: 742d 656d 7074 7969 6e67 2d76 6172 6961  t-emptying-varia
+00010ed0: 6e63 652d 746f 6f6c 7469 705c 220a 2020  nce-tooltip\".  
+00010ee0: 2020 2020 2020 636c 6173 733d 5c22 676c        class=\"gl
+00010ef0: 7970 6869 636f 6e20 676c 7970 6869 636f  yphicon glyphico
+00010f00: 6e2d 7175 6573 7469 6f6e 2d73 6967 6e5c  n-question-sign\
+00010f10: 225c 725c 6e20 2020 2020 2020 2020 2020  "\r\n           
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f30: 2020 2020 2074 6162 696e 6465 783d 5c22       tabindex=\"
+00010f40: 2d31 5c22 0a20 2020 2020 2020 2064 6174  -1\".        dat
+00010f50: 612d 6f72 6967 696e 616c 2d74 6974 6c65  a-original-title
+00010f60: 3d5c 2241 6a6f 705c 7845 3469 765c 7845  =\"Ajop\xE4iv\xE
+00010f70: 3420 766f 6920 6d75 7574 7475 6120 285c  4 voi muuttua (\
+00010f80: 7842 3120 312d 3220 705c 7845 3469 765c  xB1 1-2 p\xE4iv\
+00010f90: 7845 345c 7845 3429 0a20 2020 2020 2020  xE4\xE4).       
+00010fa0: 2065 7369 6d2e 2061 726b 6970 7968 5c78   esim. arkipyh\x
+00010fb0: 4534 7669 696b 6f69 6c6c 612e 5c22 5c72  E4viikoilla.\"\r
+00010fc0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fe0: 2020 6461 7461 2d74 6f67 676c 653d 5c22    data-toggle=\"
+00010ff0: 706f 706f 7665 725c 220a 2020 2020 2020  popover\".      
+00011000: 2020 6461 7461 2d70 6c61 6365 6d65 6e74    data-placement
+00011010: 3d5c 2261 7574 6f20 7269 6768 745c 2220  =\"auto right\" 
+00011020: 6461 7461 2d74 7269 6767 6572 3d5c 2266  data-trigger=\"f
+00011030: 6f63 7573 5c22 3e3c 2f69 3e5c 725c 6e20  ocus\"></i>\r\n 
+00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011050: 2020 2020 2020 205c 725c 6e5c 745c 745c         \r\n\t\t\
+00011060: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
+00011070: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
+00011080: 6e5c 745c 745c 745c 745c 725c 6e5c 725c  n\t\t\t\t\r\n\r\
+00011090: 6e5c 745c 745c 745c 745c 725c 6e5c 725c  n\t\t\t\t\r\n\r\
+000110a0: 6e5c 745c 745c 745c 745c 725c 6e5c 725c  n\t\t\t\t\r\n\r\
+000110b0: 6e5c 745c 745c 745c 745c 725c 6e5c 745c  n\t\t\t\t\r\n\t\
+000110c0: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+000110d0: 2020 6461 7461 2d68 6561 6465 723d 5c22    data-header=\"
+000110e0: 4153 544d 6174 6b61 5c22 3e5c 725c 6e5c  ASTMatka\">\r\n\
+000110f0: 745c 745c 745c 745c 743c 6469 7620 6461  t\t\t\t\t<div da
+00011100: 7461 2d68 6561 6465 723d 5c22 4153 544d  ta-header=\"ASTM
+00011110: 6174 6b61 5c22 3e4d 6174 6b61 5c72 5c6e  atka\">Matka\r\n
+00011120: 5c74 5c74 5c74 5c74 5c74 3c73 7061 6e3e  \t\t\t\t\t<span>
+00011130: 0a20 2020 2020 2020 203c 2f73 7061 6e3e  .        </span>
+00011140: 3c73 7061 6e20 6461 7461 2d76 616c 7565  <span data-value
+00011150: 3d5c 2241 5354 4d61 746b 615c 223e 3c2f  =\"ASTMatka\"></
+00011160: 7370 616e 3e20 6d20 3c73 7061 6e20 6461  span> m <span da
+00011170: 7461 2d76 616c 7565 3d5c 2241 5354 4d61  ta-value=\"ASTMa
+00011180: 746b 6150 7269 6365 5c22 3e3c 2f73 7061  tkaPrice\"></spa
+00011190: 6e3e 5c72 5c6e 0a20 2020 2020 2020 205c  n>\r\n.        \
+000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111b0: 2020 203c 2f64 6976 3e5c 725c 6e5c 745c     </div>\r\n\t\
+000111c0: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
+000111d0: 745c 745c 745c 745c 725c 6e5c 725c 6e5c  t\t\t\t\r\n\r\n\
+000111e0: 745c 745c 745c 745c 725c 6e5c 725c 6e5c  t\t\t\t\r\n\r\n\
+000111f0: 745c 745c 745c 745c 725c 6e5c 745c 745c  t\t\t\t\r\n\t\t\
+00011200: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
+00011210: 6461 7461 2d68 6561 6465 723d 5c22 4153  data-header=\"AS
+00011220: 544b 6573 6b41 6c6b 2d41 7374 5c22 3e5c  TKeskAlk-Ast\">\
+00011230: 725c 6e5c 745c 745c 745c 745c 743c 6469  r\n\t\t\t\t\t<di
+00011240: 7620 6461 7461 2d68 6561 6465 723d 5c22  v data-header=\"
+00011250: 4153 544b 6573 6b41 6c6b 2d41 7374 5c22  ASTKeskAlk-Ast\"
+00011260: 3e4b 6573 6b65 7974 7973 5c72 5c6e 5c74  >Keskeytys\r\n\t
+00011270: 5c74 5c74 5c74 5c74 3c73 7061 6e3e 0a20  \t\t\t\t<span>. 
+00011280: 2020 2020 2020 203c 2f73 7061 6e3e 3c73         </span><s
+00011290: 7061 6e20 6461 7461 2d76 616c 7565 3d5c  pan data-value=\
+000112a0: 2241 5354 4b65 736b 416c 6b2d 4173 745c  "ASTKeskAlk-Ast\
+000112b0: 223e 3c2f 7370 616e 3e5c 725c 6e5c 745c  "></span>\r\n\t\
+000112c0: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
+000112d0: 6e5c 745c 745c 745c 743c 2f64 6976 3e5c  n\t\t\t\t</div>\
+000112e0: 725c 6e5c 745c 745c 745c 745c 725c 6e5c  r\n\t\t\t\t\r\n\
+000112f0: 725c 6e5c 745c 745c 745c 743c 6469 760a  r\n\t\t\t\t<div.
+00011300: 2020 2020 2020 2020 6461 7461 2d68 6561          data-hea
+00011310: 6465 723d 5c22 4153 544c 6f70 5076 6d5c  der=\"ASTLopPvm\
+00011320: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
+00011330: 3c64 6976 2064 6174 612d 6865 6164 6572  <div data-header
+00011340: 3d5c 2241 5354 4c6f 7050 766d 5c22 3e4c  =\"ASTLopPvm\">L
+00011350: 6f70 6574 7573 3c2f 6469 763e 5c72 5c6e  opetus</div>\r\n
+00011360: 5c74 5c74 5c74 5c74 5c74 3c64 6976 0a20  \t\t\t\t\t<div. 
+00011370: 2020 2020 2020 2064 6174 612d 7661 6c75         data-valu
+00011380: 653d 5c22 4153 544c 6f70 5076 6d5c 223e  e=\"ASTLopPvm\">
+00011390: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
+000113a0: 5c74 3c2f 6469 763e 5c72 5c6e 5c72 5c6e  \t</div>\r\n\r\n
+000113b0: 5c74 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \t\t\t\t\r\n\t\t
+000113c0: 5c74 3c2f 6469 763e 5c72 5c6e 5c72 5c6e  \t</div>\r\n\r\n
+000113d0: 5c74 5c74 5c74 5c72 5c6e 5c74 5c74 5c74  \t\t\t\r\n\t\t\t
+000113e0: 3c64 6976 0a20 2020 2020 2020 2063 6c61  <div.        cla
+000113f0: 7373 3d5c 2265 7874 7261 2d74 6578 745c  ss=\"extra-text\
+00011400: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 3c61  ">\r\n\t\t\t\t<a
+00011410: 2068 7265 663d 5c22 6874 7470 3a2f 2f77   href=\"http://w
+00011420: 7777 2e6a 6174 656b 756b 6b6f 2e66 692f  ww.jatekukko.fi/
+00011430: 6c61 6a69 7474 656c 755c 220a 2020 2020  lajittelu\".    
+00011440: 2020 2020 7461 7267 6574 3d5c 225f 626c      target=\"_bl
+00011450: 616e 6b5c 223e 3c73 6d61 6c6c 3e5c 7842  ank\"><small>\xB
+00011460: 4220 4c61 6a69 7474 656c 756f 686a 6565  B Lajitteluohjee
+00011470: 743c 2f73 6d61 6c6c 3e20 3c2f 613e 3c61  t</small> </a><a
+00011480: 2068 7265 663d 5c22 6874 7470 3a2f 2f77   href=\"http://w
+00011490: 7777 2e6a 6174 656b 756b 6b6f 2e66 692f  ww.jatekukko.fi/
+000114a0: 6869 6e6e 6174 5c22 0a20 2020 2020 2020  hinnat\".       
+000114b0: 2074 6172 6765 743d 5c22 5f62 6c61 6e6b   target=\"_blank
+000114c0: 5c22 3e3c 736d 616c 6c3e 5c78 4242 204c  \"><small>\xBB L
+000114d0: 6973 5c78 4534 7469 6574 6f6a 6120 6869  is\xE4tietoja hi
+000114e0: 6e6e 6f69 7374 613c 2f73 6d61 6c6c 3e3c  nnoista</small><
+000114f0: 2f61 3e5c 725c 6e5c 745c 745c 743c 2f64  /a>\r\n\t\t\t</d
+00011500: 6976 3e5c 725c 6e5c 745c 745c 745c 725c  iv>\r\n\t\t\t\r\
+00011510: 6e5c 725c 6e0a 2020 2020 2020 2020 5c20  n\r\n.        \ 
+00011520: 2020 2020 2020 2020 2020 5c72 5c6e 5c74            \r\n\t
+00011530: 5c74 5c74 2020 2020 3c64 6976 2063 6c61  \t\t    <div cla
+00011540: 7373 3d5c 2273 6572 7669 6365 2d69 6e66  ss=\"service-inf
+00011550: 6f5c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  o\">\r\n\t\t\t\t
+00011560: 2020 2020 3c64 6976 0a20 2020 2020 2020      <div.       
+00011570: 2064 6174 612d 6865 6164 6572 3d5c 2241   data-header=\"A
+00011580: 5354 5065 724d 6174 6b61 5c22 3e5c 725c  STPerMatka\">\r\
+00011590: 6e5c 745c 745c 745c 745c 7420 2020 203c  n\t\t\t\t\t    <
+000115a0: 6469 7620 6461 7461 2d68 6561 6465 723d  div data-header=
+000115b0: 5c22 4153 5450 6572 4d61 746b 615c 223e  \"ASTPerMatka\">
+000115c0: 4d61 746b 615c 725c 6e5c 745c 745c 745c  Matka\r\n\t\t\t\
+000115d0: 745c 740a 2020 2020 2020 2020 5c20 2020  t\t.        \   
+000115e0: 3c73 7061 6e3e 203c 2f73 7061 6e3e 3c73  <span> </span><s
+000115f0: 7061 6e20 6461 7461 2d76 616c 7565 3d5c  pan data-value=\
+00011600: 2241 5354 5065 724d 6174 6b61 5c22 3e3c  "ASTPerMatka\"><
+00011610: 2f73 7061 6e3e 206d 3c2f 6469 763e 5c72  /span> m</div>\r
+00011620: 5c6e 5c74 5c74 5c74 5c74 0a20 2020 2020  \n\t\t\t\t.     
+00011630: 2020 205c 2020 203c 2f64 6976 3e5c 725c     \   </div>\r\
+00011640: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00011650: 203c 2f64 6976 3e5c 725c 6e20 2020 2020   </div>\r\n     
+00011660: 2020 2020 2020 205c 725c 6e5c 725c 6e5c         \r\n\r\n\
+00011670: 745c 745c 745c 725c 6e5c 745c 745c 745c  t\t\t\r\n\t\t\t\
+00011680: 725c 6e5c 745c 745c 745c 743c 6469 760a  r\n\t\t\t\t<div.
+00011690: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+000116a0: 6465 7363 7269 7074 696f 6e5c 223e 3c2f  description\"></
+000116b0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c72  div>\r\n\t\t\t\r
+000116c0: 5c6e 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \n\t\t\t\r\n\t\t
+000116d0: 5c74 5c72 5c6e 5c74 5c74 3c2f 6469 763e  \t\r\n\t\t</div>
+000116e0: 5c72 5c6e 5c72 5c6e 5c74 5c74 5c72 5c6e  \r\n\r\n\t\t\r\n
+000116f0: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
+00011700: 2063 6c61 7373 3d5c 2264 726f 7064 6f77   class=\"dropdow
+00011710: 6e2d 636f 6e74 656e 745c 223e 5c72 5c6e  n-content\">\r\n
+00011720: 5c74 5c74 5c72 5c6e 5c74 5c74 5c72 5c6e  \t\t\r\n\t\t\r\n
+00011730: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
+00011740: 2263 6f6c 2d6d 642d 3320 7365 7276 6963  "col-md-3 servic
+00011750: 652d 6275 7474 6f6e 735c 223e 5c72 5c6e  e-buttons\">\r\n
+00011760: 5c72 5c6e 5c74 5c74 5c74 5c72 5c6e 5c72  \r\n\t\t\t\r\n\r
+00011770: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00011780: 2020 2020 2020 205c 725c 6e20 2020 2020         \r\n     
+00011790: 2020 2020 2020 203c 6275 7474 6f6e 2063         <button c
+000117a0: 6c61 7373 3d5c 226f 7264 6572 2d62 7574  lass=\"order-but
+000117b0: 746f 6e20 6274 6e20 6274 6e2d 7072 696d  ton btn btn-prim
+000117c0: 6172 7920 6274 6e2d 626c 6f63 6b0a 2020  ary btn-block.  
+000117d0: 2020 2020 2020 6274 6e2d 7772 6170 5c22        btn-wrap\"
+000117e0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+000117f0: 205c 7454 696c 6161 2079 6c69 6d5c 7845   \tTilaa ylim\xE
+00011800: 345c 7845 3472 5c78 4534 696e 656e 2074  4\xE4r\xE4inen t
+00011810: 7968 6a65 6e6e 7973 5c72 5c6e 2020 2020  yhjennys\r\n    
+00011820: 2020 2020 5c74 3c2f 6275 7474 6f6e 3e5c      \t</button>\
+00011830: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00011840: 2020 2020 2020 2020 5c72 5c6e 5c72 5c6e          \r\n\r\n
+00011850: 2020 2020 2020 2020 2020 2020 5c72 5c6e              \r\n
+00011860: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
+00011870: 746f 6e20 636c 6173 733d 5c22 7061 7573  ton class=\"paus
+00011880: 652d 6275 7474 6f6e 0a20 2020 2020 2020  e-button.       
+00011890: 2062 746e 2062 746e 2d70 7269 6d61 7279   btn btn-primary
+000118a0: 2062 746e 2d62 6c6f 636b 2062 746e 2d77   btn-block btn-w
+000118b0: 7261 705c 223e 5c72 5c6e 2020 2020 2020  rap\">\r\n      
+000118c0: 2020 2020 2020 5c74 4b65 736b 6579 745c        \tKeskeyt\
+000118d0: 7845 345c 725c 6e20 2020 2020 2020 205c  xE4\r\n        \
+000118e0: 743c 2f62 7574 746f 6e3e 5c72 5c6e 0a20  t</button>\r\n. 
+000118f0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+00011900: 2020 205c 725c 6e20 2020 2020 2020 2020     \r\n         
+00011910: 2020 2020 2020 2020 2020 205c 725c 6e20             \r\n 
+00011920: 2020 2020 2020 2020 2020 205c 725c 6e5c             \r\n\
+00011930: 745c 745c 743c 6275 7474 6f6e 2063 6c61  t\t\t<button cla
+00011940: 7373 3d5c 2263 6861 6e67 652d 7265 7175  ss=\"change-requ
+00011950: 6573 742d 6275 7474 6f6e 0a20 2020 2020  est-button.     
+00011960: 2020 2062 746e 2062 746e 2d70 7269 6d61     btn btn-prima
+00011970: 7279 2062 746e 2d62 6c6f 636b 2062 746e  ry btn-block btn
+00011980: 2d77 7261 705c 223e 5c72 5c6e 5c74 5c74  -wrap\">\r\n\t\t
+00011990: 5c74 5c74 4d75 7520 6d75 7574 6f73 2070  \t\tMuu muutos p
+000119a0: 616c 7665 6c75 756e 5c72 5c6e 5c74 5c74  alveluun\r\n\t\t
+000119b0: 5c74 3c2f 6275 7474 6f6e 3e5c 725c 6e5c  \t</button>\r\n\
+000119c0: 745c 745c 745c 725c 6e0a 2020 2020 2020  t\t\t\r\n.      
+000119d0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+000119e0: 2020 5c72 5c6e 2020 2020 2020 2020 2020    \r\n          
+000119f0: 2020 5c72 5c6e 5c74 5c74 2020 2020 5c74    \r\n\t\t    \t
+00011a00: 3c62 7574 746f 6e20 7479 7065 3d5c 2262  <button type=\"b
+00011a10: 7574 746f 6e5c 2220 636c 6173 733d 5c22  utton\" class=\"
+00011a20: 6274 6e0a 2020 2020 2020 2020 6274 6e2d  btn.        btn-
+00011a30: 7072 696d 6172 7920 6274 6e2d 626c 6f63  primary btn-bloc
+00011a40: 6b20 6274 6e2d 7772 6170 2066 756c 6c2d  k btn-wrap full-
+00011a50: 7769 6474 685c 2220 6461 7461 2d61 6374  width\" data-act
+00011a60: 696f 6e3d 5c22 6564 6974 2d6b 696d 7070  ion=\"edit-kimpp
+00011a70: 615c 223e 5c72 5c6e 5c74 5c74 0a20 2020  a\">\r\n\t\t.   
+00011a80: 2020 2020 205c 2020 205c 745c 744d 756f       \   \t\tMuo
+00011a90: 6b6b 6161 206b 696d 7070 6161 5c72 5c6e  kkaa kimppaa\r\n
+00011aa0: 5c74 2020 2020 5c74 5c74 3c2f 6275 7474  \t    \t\t</butt
+00011ab0: 6f6e 3e5c 725c 6e5c 745c 7420 2020 205c  on>\r\n\t\t    \
+00011ac0: 725c 6e5c 725c 6e5c 745c 745c 745c 725c  r\n\r\n\t\t\t\r\
+00011ad0: 6e5c 745c 745c 743c 6275 7474 6f6e 0a20  n\t\t\t<button. 
+00011ae0: 2020 2020 2020 2063 6c61 7373 3d5c 2272         class=\"r
+00011af0: 6573 6967 6e2d 6b69 6d70 7061 2d62 7574  esign-kimppa-but
+00011b00: 746f 6e20 6274 6e20 6274 6e2d 7072 696d  ton btn btn-prim
+00011b10: 6172 795c 223e 5c72 5c6e 5c74 5c74 5c74  ary\">\r\n\t\t\t
+00011b20: 5c74 4572 6f61 206b 696d 7061 7374 615c  \tEroa kimpasta\
+00011b30: 725c 6e5c 745c 745c 743c 2f62 7574 746f  r\n\t\t\t</butto
+00011b40: 6e3e 5c72 5c6e 5c74 5c74 5c74 5c72 5c6e  n>\r\n\t\t\t\r\n
+00011b50: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+00011b60: 2020 2020 2020 2020 205c 725c 6e20 2020           \r\n   
+00011b70: 2020 2020 2020 2020 205c 743c 6275 7474           \t<butt
+00011b80: 6f6e 2063 6c61 7373 3d5c 226b 696d 7061  on class=\"kimpa
+00011b90: 6b73 692d 6275 7474 6f6e 2062 746e 2062  ksi-button btn b
+00011ba0: 746e 2d70 7269 6d61 7279 0a20 2020 2020  tn-primary.     
+00011bb0: 2020 2062 746e 2d62 6c6f 636b 2062 746e     btn-block btn
+00011bc0: 2d77 7261 705c 223e 5c72 5c6e 2020 2020  -wrap\">\r\n    
+00011bd0: 2020 2020 2020 2020 5c74 5c74 5065 7275          \t\tPeru
+00011be0: 7374 6120 7575 7369 206b 696d 7070 615c  sta uusi kimppa\
+00011bf0: 725c 6e20 2020 2020 2020 205c 745c 743c  r\n        \t\t<
+00011c00: 2f62 7574 746f 6e3e 5c72 5c6e 0a20 2020  /button>\r\n.   
+00011c10: 2020 2020 205c 2020 2020 2020 2020 2020       \          
+00011c20: 205c 725c 6e5c 725c 6e20 2020 2020 2020   \r\n\r\n       
+00011c30: 2020 2020 205c 725c 6e20 2020 2020 2020       \r\n       
+00011c40: 2020 2020 205c 725c 6e5c 745c 745c 743c       \r\n\t\t\t<
+00011c50: 6275 7474 6f6e 2063 6c61 7373 3d5c 2273  button class=\"s
+00011c60: 746f 702d 6275 7474 6f6e 0a20 2020 2020  top-button.     
+00011c70: 2020 2062 746e 2062 746e 2d70 7269 6d61     btn btn-prima
+00011c80: 7279 2062 746e 2d62 6c6f 636b 2062 746e  ry btn-block btn
+00011c90: 2d77 7261 705c 223e 5c72 5c6e 5c74 5c74  -wrap\">\r\n\t\t
+00011ca0: 5c74 5c74 4c6f 7065 7461 5c72 5c6e 5c74  \t\tLopeta\r\n\t
+00011cb0: 5c74 5c74 3c2f 6275 7474 6f6e 3e5c 725c  \t\t</button>\r\
+00011cc0: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+00011cd0: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
+00011ce0: 2020 2020 2020 5c72 5c6e 5c72 5c6e 5c74        \r\n\r\n\t
+00011cf0: 5c74 3c2f 6469 763e 5c72 5c6e 5c72 5c6e  \t</div>\r\n\r\n
+00011d00: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
+00011d10: 2263 6f6c 2d6d 642d 330a 2020 2020 2020  "col-md-3.      
+00011d20: 2020 616b 702d 6275 7474 6f6e 735c 223e    akp-buttons\">
+00011d30: 5c72 5c6e 5c74 5c74 5c74 3c62 7574 746f  \r\n\t\t\t<butto
+00011d40: 6e20 636c 6173 733d 5c22 616b 702d 6c6f  n class=\"akp-lo
+00011d50: 6361 7469 6f6e 2d62 7574 746f 6e20 6274  cation-button bt
+00011d60: 6e20 6274 6e2d 7072 696d 6172 790a 2020  n btn-primary.  
+00011d70: 2020 2020 2020 6274 6e2d 626c 6f63 6b5c        btn-block\
+00011d80: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5069  ">\r\n\t\t\t\tPi
+00011d90: 7374 6565 6e20 7369 6a61 696e 7469 202f  steen sijainti /
+00011da0: 2056 6169 6864 6120 7069 7374 6574 745c   Vaihda pistett\
+00011db0: 7845 345c 725c 6e5c 745c 745c 743c 2f62  xE4\r\n\t\t\t</b
+00011dc0: 7574 746f 6e3e 5c72 5c6e 5c72 5c6e 5c74  utton>\r\n\r\n\t
+00011dd0: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 3c64  \t\t\r\n\t\t\t<d
+00011de0: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+00011df0: 3d5c 2274 6578 742d 656c 656d 656e 745c  =\"text-element\
+00011e00: 223e 566f 6974 2070 5c78 4534 5c78 4534  ">Voit p\xE4\xE4
+00011e10: 7474 5c78 4534 5c78 4534 206b 6f68 7465  tt\xE4\xE4 kohte
+00011e20: 656e 206a 5c78 4534 7465 6875 6f6c 6c6f  en j\xE4tehuollo
+00011e30: 6e20 7461 690a 2020 2020 2020 2020 6d75  n tai.        mu
+00011e40: 7574 7461 6120 6a5c 7845 3474 6568 756f  uttaa j\xE4tehuo
+00011e50: 6c6c 6f6e 206c 6969 7474 796d 6973 7461  llon liittymista
+00011e60: 7061 6120 3c61 2068 7265 663d 5c22 235c  paa <a href=\"#\
+00011e70: 2220 6461 7461 2d61 6374 696f 6e3d 5c22  " data-action=\"
+00011e80: 676f 2d74 6f2d 6375 7374 6f6d 6572 2d64  go-to-customer-d
+00011e90: 6174 615c 223e 6b6f 6874 6565 6e0a 2020  ata\">kohteen.  
+00011ea0: 2020 2020 2020 7469 6564 6f74 202d 765c        tiedot -v\
+00011eb0: 7845 346c 696c 6568 6465 6c6c 5c78 4534  xE4lilehdell\xE4
+00011ec0: 3c2f 613e 2e3c 2f64 6976 3e5c 725c 6e5c  </a>.</div>\r\n\
+00011ed0: 745c 745c 745c 725c 6e5c 725c 6e5c 745c  t\t\t\r\n\r\n\t\
+00011ee0: 745c 745c 725c 6e5c 745c 743c 2f64 6976  t\t\r\n\t\t</div
+00011ef0: 3e5c 725c 6e5c 745c 745c 725c 6e5c 725c  >\r\n\t\t\r\n\r\
+00011f00: 6e5c 745c 745c 725c 6e5c 745c 743c 2f64  n\t\t\r\n\t\t</d
+00011f10: 6976 3e5c 725c 6e5c 745c 745c 725c 6e5c  iv>\r\n\t\t\r\n\
+00011f20: 745c 743c 610a 2020 2020 2020 2020 636c  t\t<a.        cl
+00011f30: 6173 733d 5c22 6d61 6b65 2d63 6861 6e67  ass=\"make-chang
+00011f40: 6573 5c22 3e5c 725c 6e5c 745c 745c 743c  es\">\r\n\t\t\t<
+00011f50: 7370 616e 3e5c 725c 6e5c 745c 745c 745c  span>\r\n\t\t\t\
+00011f60: 7454 6565 206d 7575 746f 6b73 6961 2070  tTee muutoksia p
+00011f70: 616c 7665 6c75 756e 5c72 5c6e 5c74 5c74  alveluun\r\n\t\t
+00011f80: 5c74 3c2f 7370 616e 3e5c 725c 6e5c 745c  \t</span>\r\n\t\
+00011f90: 743c 2f61 3e5c 725c 6e5c 745c 745c 725c  t</a>\r\n\t\t\r\
+00011fa0: 6e5c 745c 745c 725c 6e5c 725c 6e5c 743c  n\t\t\r\n\r\n\t<
+00011fb0: 2f64 6976 3e5c 725c 6e5c 725c 6e3c 2f66  /div>\r\n\r\n</f
+00011fc0: 6965 6c64 7365 743e 5c72 5c6e 3c2f 7363  ieldset>\r\n</sc
+00011fd0: 7269 7074 3e5c 725c 6e5c 725c 6e3c 7363  ript>\r\n\r\n<sc
+00011fe0: 7269 7074 0a20 2020 2020 2020 2069 643d  ript.        id=
+00011ff0: 5c22 6b69 6d70 7061 2d6f 7361 6b61 732d  \"kimppa-osakas-
+00012000: 6564 6974 6f72 2d74 656d 706c 6174 655c  editor-template\
+00012010: 2220 7479 7065 3d5c 2274 6578 742f 782d  " type=\"text/x-
+00012020: 7465 6d70 6c61 7465 5c22 3e5c 725c 6e5c  template\">\r\n\
+00012030: 725c 6e5c 725c 6e5c 725c 6e5c 725c 6e3c  r\n\r\n\r\n\r\n<
+00012040: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
+00012050: 733d 5c22 6f73 616b 6173 2d65 6469 746f  s=\"osakas-edito
+00012060: 725c 223e 5c72 5c6e 5c74 3c64 6976 2063  r\">\r\n\t<div c
+00012070: 6c61 7373 3d5c 2263 6f6e 7461 696e 6572  lass=\"container
+00012080: 2d66 6c75 6964 5c22 3e5c 725c 6e5c 745c  -fluid\">\r\n\t\
+00012090: 743c 666f 726d 3e5c 725c 6e5c 745c 745c  t<form>\r\n\t\t\
+000120a0: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
+000120b0: 6173 733d 5c22 726f 7720 626f 7264 6572  ass=\"row border
+000120c0: 2d62 6f74 746f 6d5c 223e 5c72 5c6e 5c74  -bottom\">\r\n\t
+000120d0: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
+000120e0: 3d5c 2263 6f6c 2d6d 642d 3132 5c22 3e5c  =\"col-md-12\">\
+000120f0: 725c 6e5c 745c 745c 745c 745c 743c 6832  r\n\t\t\t\t\t<h2
+00012100: 3e55 7573 690a 2020 2020 2020 2020 6f73  >Uusi.        os
+00012110: 616b 6173 3c2f 6832 3e5c 725c 6e5c 745c  akas</h2>\r\n\t\
+00012120: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
+00012130: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
+00012140: 725c 6e5c 745c 745c 743c 6469 7620 636c  r\n\t\t\t<div cl
+00012150: 6173 733d 5c22 726f 770a 2020 2020 2020  ass=\"row.      
+00012160: 2020 626f 7264 6572 2d62 6f74 746f 6d5c    border-bottom\
+00012170: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 3c66  ">\r\n\t\t\t\t<f
+00012180: 6965 6c64 7365 7420 636c 6173 733d 5c22  ieldset class=\"
+00012190: 6669 656c 6473 6574 206d 6172 6769 6e2d  fieldset margin-
+000121a0: 626f 7474 6f6d 2d31 355c 223e 5c72 5c6e  bottom-15\">\r\n
+000121b0: 5c74 5c74 5c74 5c74 5c74 3c64 6976 0a20  \t\t\t\t\t<div. 
+000121c0: 2020 2020 2020 2063 6c61 7373 3d5c 2263         class=\"c
+000121d0: 6f6c 2d6d 642d 3132 5c22 3e5c 725c 6e5c  ol-md-12\">\r\n\
+000121e0: 745c 745c 745c 745c 745c 743c 6c65 6765  t\t\t\t\t\t<lege
+000121f0: 6e64 3e4b 6969 6e74 6569 7374 5c78 4636  nd>Kiinteist\xF6
+00012200: 6e20 7469 6564 6f74 3c2f 6c65 6765 6e64  n tiedot</legend
+00012210: 3e5c 725c 6e5c 745c 745c 745c 745c 743c  >\r\n\t\t\t\t\t<
+00012220: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
+00012230: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
+00012240: 636c 6173 733d 5c22 636f 6c2d 6d64 2d36  class=\"col-md-6
+00012250: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
+00012260: 745c 743c 6469 7620 636c 6173 733d 5c22  t\t<div class=\"
+00012270: 666f 726d 2d67 726f 7570 2072 6571 7569  form-group requi
+00012280: 7265 645c 223e 5c72 5c6e 5c74 5c74 5c74  red\">\r\n\t\t\t
+00012290: 5c74 5c74 5c74 5c74 3c6c 6162 656c 0a20  \t\t\t\t<label. 
+000122a0: 2020 2020 2020 2066 6f72 3d5c 226f 7361         for=\"osa
+000122b0: 6b61 732e 6b75 6e74 6174 756e 6e75 735c  kas.kuntatunnus\
+000122c0: 223e 4b75 6e74 613c 2f6c 6162 656c 3e20  ">Kunta</label> 
+000122d0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+000122e0: 5c74 3c64 6976 2063 6c61 7373 3d5c 2273  \t<div class=\"s
+000122f0: 656c 6563 745c 223e 5c72 5c6e 5c74 5c74  elect\">\r\n\t\t
+00012300: 5c74 5c74 5c74 5c74 5c74 5c74 3c73 656c  \t\t\t\t\t\t<sel
+00012310: 6563 740a 2020 2020 2020 2020 6964 3d5c  ect.        id=\
+00012320: 226f 7361 6b61 732e 6b75 6e74 6174 756e  "osakas.kuntatun
+00012330: 6e75 735c 2220 6e61 6d65 3d5c 226f 7361  nus\" name=\"osa
+00012340: 6b61 732e 6b75 6e74 6174 756e 6e75 735c  kas.kuntatunnus\
+00012350: 2220 636c 6173 733d 5c22 666f 726d 2d63  " class=\"form-c
+00012360: 6f6e 7472 6f6c 5c22 0a20 2020 2020 2020  ontrol\".       
+00012370: 2072 6571 7569 7265 643e 5c72 5c6e 5c74   required>\r\n\t
+00012380: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+00012390: 3c6f 7074 696f 6e20 7661 6c75 653d 5c22  <option value=\"
+000123a0: 5c22 3e2d 2d20 5661 6c69 7473 6520 2d2d  \">-- Valitse --
+000123b0: 3c2f 6f70 7469 6f6e 3e5c 725c 6e5c 745c  </option>\r\n\t\
+000123c0: 745c 745c 745c 745c 745c 745c 743c 2f73  t\t\t\t\t\t\t</s
+000123d0: 656c 6563 743e 5c72 5c6e 5c74 5c74 5c74  elect>\r\n\t\t\t
+000123e0: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
+000123f0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \n\t\t\t\t\t\t</
+00012400: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
+00012410: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
+00012420: 5c74 5c74 5c74 5c72 5c6e 5c74 5c74 5c74  \t\t\t\r\n\t\t\t
+00012430: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
+00012440: 2020 2063 6c61 7373 3d5c 2263 6f6c 2d6d     class=\"col-m
+00012450: 642d 365c 223e 5c72 5c6e 5c74 5c74 5c74  d-6\">\r\n\t\t\t
+00012460: 5c74 5c74 5c74 5c74 3c64 6976 2063 6c61  \t\t\t\t<div cla
+00012470: 7373 3d5c 2266 6f72 6d2d 6772 6f75 705c  ss=\"form-group\
+00012480: 223e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  ">\r\n\t\t\t\t\t
+00012490: 5c74 5c74 5c74 3c6c 6162 656c 0a20 2020  \t\t\t<label.   
+000124a0: 2020 2020 2066 6f72 3d5c 226f 7361 6b61       for=\"osaka
+000124b0: 732e 6b69 696e 7472 656b 7475 6e6e 7573  s.kiintrektunnus
+000124c0: 5c22 3e4b 6969 6e74 6569 7374 5c78 4636  \">Kiinteist\xF6
+000124d0: 7265 6b69 7374 6572 6974 756e 6e75 733c  rekisteritunnus<
+000124e0: 2f6c 6162 656c 3e20 5c72 5c6e 5c74 5c74  /label> \r\n\t\t
+000124f0: 5c74 5c74 5c74 5c74 5c74 5c74 3c69 6e70  \t\t\t\t\t\t<inp
+00012500: 7574 0a20 2020 2020 2020 2074 7970 653d  ut.        type=
+00012510: 5c22 7465 7874 5c22 206e 616d 653d 5c22  \"text\" name=\"
+00012520: 6f73 616b 6173 2e6b 6969 6e74 7265 6b74  osakas.kiintrekt
+00012530: 756e 6e75 735c 2220 636c 6173 733d 5c22  unnus\" class=\"
+00012540: 666f 726d 2d63 6f6e 7472 6f6c 5c22 206d  form-control\" m
+00012550: 6178 6c65 6e67 7468 3d5c 2232 335c 220a  axlength=\"23\".
+00012560: 2020 2020 2020 2020 3e5c 725c 6e5c 745c          >\r\n\t\
+00012570: 745c 745c 745c 745c 745c 743c 2f64 6976  t\t\t\t\t\t</div
+00012580: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00012590: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
+000125a0: 745c 745c 745c 725c 6e5c 745c 745c 745c  t\t\t\r\n\t\t\t\
+000125b0: 743c 2f66 6965 6c64 7365 743e 5c72 5c6e  t</fieldset>\r\n
+000125c0: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
+000125d0: 5c72 5c6e 5c74 5c74 5c74 3c64 6976 0a20  \r\n\t\t\t<div. 
+000125e0: 2020 2020 2020 2063 6c61 7373 3d5c 2272         class=\"r
+000125f0: 6f77 2062 6f72 6465 722d 626f 7474 6f6d  ow border-bottom
+00012600: 5c22 3e5c 725c 6e5c 745c 745c 745c 743c  \">\r\n\t\t\t\t<
+00012610: 6669 656c 6473 6574 2063 6c61 7373 3d5c  fieldset class=\
+00012620: 2263 6f6c 2d6d 642d 3620 7265 7175 6972  "col-md-6 requir
+00012630: 6564 5c22 3e5c 725c 6e5c 745c 745c 745c  ed\">\r\n\t\t\t\
+00012640: 745c 743c 6469 763e 5c72 5c6e 5c74 5c74  t\t<div>\r\n\t\t
+00012650: 5c74 5c74 5c74 5c74 3c6c 6567 656e 643e  \t\t\t\t<legend>
+00012660: 4b69 696e 7465 6973 745c 7846 366e 0a20  Kiinteist\xF6n. 
+00012670: 2020 2020 2020 206b 5c78 4534 7974 745c         k\xE4ytt\
+00012680: 7846 3674 6172 6b6f 6974 7573 3c2f 6c65  xF6tarkoitus</le
+00012690: 6765 6e64 3e5c 725c 6e5c 745c 745c 745c  gend>\r\n\t\t\t\
+000126a0: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
+000126b0: 745c 745c 745c 743c 6469 763e 5c72 5c6e  t\t\t\t<div>\r\n
+000126c0: 5c74 5c74 5c74 5c74 5c74 5c74 3c64 6976  \t\t\t\t\t\t<div
+000126d0: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+000126e0: 2266 6f72 6d2d 6772 6f75 705c 223e 5c72  "form-group\">\r
+000126f0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
+00012700: 3c64 6976 2063 6c61 7373 3d5c 2273 656c  <div class=\"sel
+00012710: 6563 745c 223e 5c72 5c6e 5c74 5c74 5c74  ect\">\r\n\t\t\t
+00012720: 5c74 5c74 5c74 5c74 5c74 3c73 656c 6563  \t\t\t\t\t<selec
+00012730: 740a 2020 2020 2020 2020 6461 7461 2d72  t.        data-r
+00012740: 6f6c 653d 5c22 6b61 7974 746f 7461 726b  ole=\"kayttotark
+00012750: 6f69 7475 732d 6b61 7465 676f 7269 615c  oitus-kategoria\
+00012760: 2220 636c 6173 733d 5c22 666f 726d 2d63  " class=\"form-c
+00012770: 6f6e 7472 6f6c 5c22 2072 6571 7569 7265  ontrol\" require
+00012780: 6420 3e5c 725c 6e5c 745c 745c 745c 745c  d >\r\n\t\t\t\t\
+00012790: 745c 745c 745c 745c 743c 6f70 7469 6f6e  t\t\t\t\t<option
+000127a0: 0a20 2020 2020 2020 2076 616c 7565 3d5c  .        value=\
+000127b0: 225c 223e 3c2f 6f70 7469 6f6e 3e5c 725c  "\"></option>\r\
+000127c0: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
+000127d0: 745c 743c 6f70 7469 6f6e 2076 616c 7565  t\t<option value
+000127e0: 3d5c 2230 5c22 3e56 616b 6974 7569 6e65  =\"0\">Vakituine
+000127f0: 6e20 6173 756e 746f 3c2f 6f70 7469 6f6e  n asunto</option
+00012800: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00012810: 745c 745c 745c 743c 6f70 7469 6f6e 0a20  t\t\t\t<option. 
+00012820: 2020 2020 2020 2076 616c 7565 3d5c 2231         value=\"1
+00012830: 5c22 3e56 6170 6161 2d61 6a61 6e20 6173  \">Vapaa-ajan as
+00012840: 756e 746f 3c2f 6f70 7469 6f6e 3e5c 725c  unto</option>\r\
+00012850: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
+00012860: 745c 743c 6f70 7469 6f6e 2076 616c 7565  t\t<option value
+00012870: 3d5c 2232 5c22 3e54 616c 6f79 6874 695c  =\"2\">Taloyhti\
+00012880: 7846 363c 2f6f 7074 696f 6e3e 5c72 5c6e  xF6</option>\r\n
+00012890: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+000128a0: 5c74 3c6f 7074 696f 6e0a 2020 2020 2020  \t<option.      
+000128b0: 2020 7661 6c75 653d 5c22 335c 223e 5972    value=\"3\">Yr
+000128c0: 6974 7973 3c2f 6f70 7469 6f6e 3e5c 725c  itys</option>\r\
+000128d0: 6e5c 745c 745c 745c 745c 745c 745c 745c  n\t\t\t\t\t\t\t\
+000128e0: 745c 743c 6f70 7469 6f6e 2076 616c 7565  t\t<option value
+000128f0: 3d5c 2234 5c22 3e59 6874 6569 735c 7846  =\"4\">Yhteis\xF
+00012900: 363c 2f6f 7074 696f 6e3e 5c72 5c6e 5c74  6</option>\r\n\t
+00012910: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \t\t\t\t\t\t\t</
+00012920: 7365 6c65 6374 3e5c 725c 6e5c 745c 745c  select>\r\n\t\t\
+00012930: 745c 745c 745c 745c 743c 2f64 6976 3e5c  t\t\t\t\t</div>\
+00012940: 725c 6e5c 745c 745c 745c 745c 745c 743c  r\n\t\t\t\t\t\t<
+00012950: 2f64 6976 3e5c 725c 6e5c 725c 6e5c 745c  /div>\r\n\r\n\t\
+00012960: 745c 745c 745c 745c 743c 6469 760a 2020  t\t\t\t\t<div.  
+00012970: 2020 2020 2020 636c 6173 733d 5c22 666f        class=\"fo
+00012980: 726d 2d67 726f 7570 5c22 203e 5c72 5c6e  rm-group\" >\r\n
+00012990: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c64  \t\t\t\t\t\t\t<d
+000129a0: 6976 2063 6c61 7373 3d5c 2273 656c 6563  iv class=\"selec
+000129b0: 745c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  t\">\r\n\t\t\t\t
+000129c0: 5c74 5c74 5c74 5c74 3c73 656c 6563 740a  \t\t\t\t<select.
+000129d0: 2020 2020 2020 2020 6e61 6d65 3d5c 226f          name=\"o
+000129e0: 7361 6b61 732e 6b61 7974 746f 7461 726b  sakas.kayttotark
+000129f0: 6f69 7475 735c 2220 636c 6173 733d 5c22  oitus\" class=\"
+00012a00: 666f 726d 2d63 6f6e 7472 6f6c 5c22 2072  form-control\" r
+00012a10: 6571 7569 7265 6420 3e5c 725c 6e5c 745c  equired >\r\n\t\
+00012a20: 745c 745c 745c 745c 745c 745c 745c 743c  t\t\t\t\t\t\t\t<
+00012a30: 6f70 7469 6f6e 0a20 2020 2020 2020 2076  option.        v
+00012a40: 616c 7565 3d5c 225c 223e 3c2f 6f70 7469  alue=\"\"></opti
+00012a50: 6f6e 3e5c 725c 6e5c 745c 745c 745c 745c  on>\r\n\t\t\t\t\
+00012a60: 745c 745c 745c 745c 743c 6f70 7469 6f6e  t\t\t\t\t<option
+00012a70: 2076 616c 7565 3d5c 2230 3131 5c22 2064   value=\"011\" d
+00012a80: 6174 612d 6b61 7465 676f 7269 613d 5c22  ata-kategoria=\"
+00012a90: 305c 223e 5968 6465 6e0a 2020 2020 2020  0\">Yhden.      
+00012aa0: 2020 6173 756e 6e6f 6e20 7461 6c6f 3c2f    asunnon talo</
+00012ab0: 6f70 7469 6f6e 3e5c 725c 6e5c 745c 745c  option>\r\n\t\t\
+00012ac0: 745c 745c 745c 745c 745c 745c 743c 6f70  t\t\t\t\t\t\t<op
+00012ad0: 7469 6f6e 2076 616c 7565 3d5c 2230 3132  tion value=\"012
+00012ae0: 5c22 2064 6174 612d 6b61 7465 676f 7269  \" data-kategori
+00012af0: 613d 5c22 305c 223e 4b61 6864 656e 0a20  a=\"0\">Kahden. 
+00012b00: 2020 2020 2020 2061 7375 6e6e 6f6e 2074         asunnon t
+00012b10: 616c 6f3c 2f6f 7074 696f 6e3e 5c72 5c6e  alo</option>\r\n
+00012b20: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+00012b30: 5c74 3c6f 7074 696f 6e20 7661 6c75 653d  \t<option value=
+00012b40: 5c22 3031 335c 2220 6461 7461 2d6b 6174  \"013\" data-kat
+00012b50: 6567 6f72 6961 3d5c 2230 5c22 3e4d 7575  egoria=\"0\">Muu
+00012b60: 0a20 2020 2020 2020 2065 7269 6c6c 696e  .        erillin
+00012b70: 656e 2070 6965 6e74 616c 6f3c 2f6f 7074  en pientalo</opt
+00012b80: 696f 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74  ion>\r\n\t\t\t\t
+00012b90: 5c74 5c74 5c74 5c74 5c74 5c72 5c6e 5c74  \t\t\t\t\t\r\n\t
+00012ba0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \t\t\t\t\t\t\t\t
+00012bb0: 3c6f 7074 696f 6e0a 2020 2020 2020 2020  <option.        
+00012bc0: 7661 6c75 653d 5c22 3034 315c 2220 6461  value=\"041\" da
+00012bd0: 7461 2d6b 6174 6567 6f72 6961 3d5c 2231  ta-kategoria=\"1
+00012be0: 5c22 3e4b 6573 5c78 4534 6d5c 7846 366b  \">Kes\xE4m\xF6k
+00012bf0: 6b69 2074 6169 2076 6170 6161 2d61 6a61  ki tai vapaa-aja
+00012c00: 6e20 6173 756e 746f 3c2f 6f70 7469 6f6e  n asunto</option
+00012c10: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00012c20: 745c 745c 745c 743c 6f70 7469 6f6e 0a20  t\t\t\t<option. 
+00012c30: 2020 2020 2020 2076 616c 7565 3d5c 2239         value=\"9
+00012c40: 3331 5c22 2064 6174 612d 6b61 7465 676f  31\" data-katego
+00012c50: 7269 613d 5c22 315c 223e 5361 756e 6172  ria=\"1\">Saunar
+00012c60: 616b 656e 6e75 733c 2f6f 7074 696f 6e3e  akennus</option>
+00012c70: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+00012c80: 5c74 5c74 5c74 5c72 5c6e 5c74 5c74 5c74  \t\t\t\r\n\t\t\t
+00012c90: 5c74 5c74 5c74 5c74 5c74 5c74 3c6f 7074  \t\t\t\t\t\t<opt
+00012ca0: 696f 6e0a 2020 2020 2020 2020 7661 6c75  ion.        valu
+00012cb0: 653d 5c22 3032 315c 2220 6461 7461 2d6b  e=\"021\" data-k
+00012cc0: 6174 6567 6f72 6961 3d5c 2232 5c22 3e52  ategoria=\"2\">R
+00012cd0: 6976 6974 616c 6f3c 2f6f 7074 696f 6e3e  ivitalo</option>
+00012ce0: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+00012cf0: 5c74 5c74 5c74 3c6f 7074 696f 6e0a 2020  \t\t\t<option.  
+00012d00: 2020 2020 2020 7661 6c75 653d 5c22 3032        value=\"02
+00012d10: 325c 2220 6461 7461 2d6b 6174 6567 6f72  2\" data-kategor
+00012d20: 6961 3d5c 2232 5c22 3e4b 6574 6a75 7461  ia=\"2\">Ketjuta
+00012d30: 6c6f 3c2f 6f70 7469 6f6e 3e5c 725c 6e5c  lo</option>\r\n\
+00012d40: 745c 745c 745c 745c 745c 745c 745c 745c  t\t\t\t\t\t\t\t\
+00012d50: 743c 6f70 7469 6f6e 0a20 2020 2020 2020  t<option.       
+00012d60: 2076 616c 7565 3d5c 2230 3332 5c22 2064   value=\"032\" d
+00012d70: 6174 612d 6b61 7465 676f 7269 613d 5c22  ata-kategoria=\"
+00012d80: 325c 223e 4c75 6874 6974 616c 6f3c 2f6f  2\">Luhtitalo</o
+00012d90: 7074 696f 6e3e 5c72 5c6e 5c74 5c74 5c74  ption>\r\n\t\t\t
+00012da0: 5c74 5c74 5c74 5c74 5c74 5c74 3c6f 7074  \t\t\t\t\t\t<opt
+00012db0: 696f 6e0a 2020 2020 2020 2020 7661 6c75  ion.        valu
+00012dc0: 653d 5c22 3033 395c 2220 6461 7461 2d6b  e=\"039\" data-k
+00012dd0: 6174 6567 6f72 6961 3d5c 2232 5c22 3e4b  ategoria=\"2\">K
+00012de0: 6572 726f 7374 616c 6f3c 2f6f 7074 696f  errostalo</optio
+00012df0: 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  n>\r\n\t\t\t\t\t
+00012e00: 5c74 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \t\t\t\t\r\n\t\t
+00012e10: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 3c6f  \t\t\t\t\t\t\t<o
+00012e20: 7074 696f 6e0a 2020 2020 2020 2020 7661  ption.        va
+00012e30: 6c75 653d 5c22 3131 315c 2220 6461 7461  lue=\"111\" data
+00012e40: 2d6b 6174 6567 6f72 6961 3d5c 2233 5c22  -kategoria=\"3\"
+00012e50: 3e59 7269 7479 733c 2f6f 7074 696f 6e3e  >Yritys</option>
+00012e60: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+00012e70: 5c74 5c74 5c74 5c72 5c6e 5c74 5c74 5c74  \t\t\t\r\n\t\t\t
+00012e80: 5c74 5c74 5c74 5c74 5c74 5c74 3c6f 7074  \t\t\t\t\t\t<opt
+00012e90: 696f 6e0a 2020 2020 2020 2020 7661 6c75  ion.        valu
+00012ea0: 653d 5c22 3133 315c 2220 6461 7461 2d6b  e=\"131\" data-k
+00012eb0: 6174 6567 6f72 6961 3d5c 2234 5c22 3e59  ategoria=\"4\">Y
+00012ec0: 6874 6569 735c 7846 363c 2f6f 7074 696f  hteis\xF6</optio
+00012ed0: 6e3e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  n>\r\n\t\t\t\t\t
+00012ee0: 5c74 5c74 5c74 3c2f 7365 6c65 6374 3e5c  \t\t\t</select>\
+00012ef0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+00012f00: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
+00012f10: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
+00012f20: 6e5c 745c 745c 745c 745c 743c 2f64 6976  n\t\t\t\t\t</div
+00012f30: 3e5c 725c 6e5c 745c 745c 745c 743c 2f66  >\r\n\t\t\t\t</f
+00012f40: 6965 6c64 7365 743e 5c72 5c6e 5c72 5c6e  ieldset>\r\n\r\n
+00012f50: 5c74 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \t\t\t\t\r\n\t\t
+00012f60: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
+00012f70: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 3c64  \t\t\r\n\t\t\t<d
+00012f80: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+00012f90: 3d5c 2272 6f77 5c22 3e5c 725c 6e5c 745c  =\"row\">\r\n\t\
+00012fa0: 745c 745c 743c 6469 7620 636c 6173 733d  t\t\t<div class=
+00012fb0: 5c22 636f 6c2d 6d64 2d36 5c22 3e5c 725c  \"col-md-6\">\r\
+00012fc0: 6e5c 745c 745c 745c 745c 743c 6669 656c  n\t\t\t\t\t<fiel
+00012fd0: 6473 6574 0a20 2020 2020 2020 2063 6c61  dset.        cla
+00012fe0: 7373 3d5c 2266 6965 6c64 7365 7420 6d61  ss=\"fieldset ma
+00012ff0: 7267 696e 2d62 6f74 746f 6d2d 3135 5c22  rgin-bottom-15\"
+00013000: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00013010: 743c 6c65 6765 6e64 3e4f 7361 6b6b 6161  t<legend>Osakkaa
+00013020: 6e20 7469 6564 6f74 3c2f 6c65 6765 6e64  n tiedot</legend
+00013030: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00013040: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
+00013050: 6173 733d 5c22 6368 6563 6b62 6f78 2069  ass=\"checkbox i
+00013060: 6e76 6973 6962 6c65 5c22 3e3c 6c61 6265  nvisible\"><labe
+00013070: 6c3e 3c2f 6c61 6265 6c3e 3c2f 6469 763e  l></label></div>
+00013080: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+00013090: 3c64 6976 2063 6c61 7373 3d5c 2266 6f72  <div class=\"for
+000130a0: 6d2d 6772 6f75 700a 2020 2020 2020 2020  m-group.        
+000130b0: 7265 7175 6972 6564 5c22 3e5c 725c 6e5c  required\">\r\n\
+000130c0: 745c 745c 745c 745c 745c 745c 743c 6c61  t\t\t\t\t\t\t<la
+000130d0: 6265 6c20 666f 723d 5c22 6f73 616b 6173  bel for=\"osakas
+000130e0: 2e6e 696d 695c 223e 4f73 616b 6b61 616e  .nimi\">Osakkaan
+000130f0: 206e 696d 693c 2f6c 6162 656c 3e0a 2020   nimi</label>.  
+00013100: 2020 2020 2020 5c72 5c6e 5c74 5c74 5c74        \r\n\t\t\t
+00013110: 5c74 5c74 5c74 5c74 3c69 6e70 7574 2072  \t\t\t\t<input r
+00013120: 6571 7569 7265 6420 7479 7065 3d5c 2274  equired type=\"t
+00013130: 6578 745c 2220 6e61 6d65 3d5c 226f 7361  ext\" name=\"osa
+00013140: 6b61 732e 6e69 6d69 5c22 2063 6c61 7373  kas.nimi\" class
+00013150: 3d5c 2266 6f72 6d2d 636f 6e74 726f 6c5c  =\"form-control\
+00013160: 220a 2020 2020 2020 2020 3e5c 725c 6e5c  ".        >\r\n\
+00013170: 745c 745c 745c 745c 745c 743c 2f64 6976  t\t\t\t\t\t</div
+00013180: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00013190: 743c 6469 7620 636c 6173 733d 5c22 666f  t<div class=\"fo
+000131a0: 726d 2d67 726f 7570 2072 6571 7569 7265  rm-group require
+000131b0: 645c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  d\">\r\n\t\t\t\t
+000131c0: 5c74 5c74 5c74 3c6c 6162 656c 0a20 2020  \t\t\t<label.   
+000131d0: 2020 2020 2066 6f72 3d5c 226f 7361 6b61       for=\"osaka
+000131e0: 732e 6574 756e 696d 695c 223e 4f73 616b  s.etunimi\">Osak
+000131f0: 6b61 616e 2065 7475 6e69 6d69 3c2f 6c61  kaan etunimi</la
+00013200: 6265 6c3e 5c72 5c6e 5c74 5c74 5c74 5c74  bel>\r\n\t\t\t\t
+00013210: 5c74 5c74 5c74 3c69 6e70 7574 2072 6571  \t\t\t<input req
+00013220: 7569 7265 640a 2020 2020 2020 2020 7479  uired.        ty
+00013230: 7065 3d5c 2274 6578 745c 2220 6e61 6d65  pe=\"text\" name
+00013240: 3d5c 226f 7361 6b61 732e 6574 756e 696d  =\"osakas.etunim
+00013250: 695c 2220 636c 6173 733d 5c22 666f 726d  i\" class=\"form
+00013260: 2d63 6f6e 7472 6f6c 5c22 203e 5c72 5c6e  -control\" >\r\n
+00013270: 5c74 5c74 5c74 5c74 5c74 5c74 3c2f 6469  \t\t\t\t\t\t</di
+00013280: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  v>\r\n\t\t\t\t\t
+00013290: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
+000132a0: 6c61 7373 3d5c 2266 6f72 6d2d 6772 6f75  lass=\"form-grou
+000132b0: 7020 7265 7175 6972 6564 5c22 2073 7479  p required\" sty
+000132c0: 6c65 3d5c 2264 6973 706c 6179 3a6e 6f6e  le=\"display:non
+000132d0: 655c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  e\">\r\n\t\t\t\t
+000132e0: 5c74 5c74 5c74 3c6c 6162 656c 0a20 2020  \t\t\t<label.   
+000132f0: 2020 2020 2066 6f72 3d5c 226f 7361 6b61       for=\"osaka
+00013300: 732e 7375 6b75 6e69 6d69 5c22 3e4f 7361  s.sukunimi\">Osa
+00013310: 6b6b 6161 6e20 7375 6b75 6e69 6d69 3c2f  kkaan sukunimi</
+00013320: 6c61 6265 6c3e 5c72 5c6e 5c74 5c74 5c74  label>\r\n\t\t\t
+00013330: 5c74 5c74 5c74 5c74 3c69 6e70 7574 0a20  \t\t\t\t<input. 
+00013340: 2020 2020 2020 2072 6571 7569 7265 6420         required 
+00013350: 7479 7065 3d5c 2274 6578 745c 2220 6e61  type=\"text\" na
+00013360: 6d65 3d5c 226f 7361 6b61 732e 7375 6b75  me=\"osakas.suku
+00013370: 6e69 6d69 5c22 2063 6c61 7373 3d5c 2266  nimi\" class=\"f
+00013380: 6f72 6d2d 636f 6e74 726f 6c5c 2220 3e5c  orm-control\" >\
+00013390: 725c 6e5c 745c 745c 745c 745c 745c 743c  r\n\t\t\t\t\t\t<
+000133a0: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
+000133b0: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+000133c0: 2020 636c 6173 733d 5c22 666f 726d 2d67    class=\"form-g
+000133d0: 726f 7570 5c22 3e5c 725c 6e5c 745c 745c  roup\">\r\n\t\t\
+000133e0: 745c 745c 745c 745c 743c 6c61 6265 6c20  t\t\t\t\t<label 
+000133f0: 666f 723d 5c22 6f73 616b 6173 2e79 6874  for=\"osakas.yht
+00013400: 6579 7368 656e 6b5c 223e 5968 7465 7973  eyshenk\">Yhteys
+00013410: 6865 6e6b 696c 5c78 4636 3c2f 6c61 6265  henkil\xF6</labe
+00013420: 6c3e 5c72 5c6e 5c74 5c74 5c74 5c74 5c74  l>\r\n\t\t\t\t\t
+00013430: 5c74 5c74 3c69 6e70 7574 0a20 2020 2020  \t\t<input.     
+00013440: 2020 2074 7970 653d 5c22 7465 7874 5c22     type=\"text\"
+00013450: 206e 616d 653d 5c22 6f73 616b 6173 2e79   name=\"osakas.y
+00013460: 6874 6579 7368 656e 6b5c 2220 636c 6173  hteyshenk\" clas
+00013470: 733d 5c22 666f 726d 2d63 6f6e 7472 6f6c  s=\"form-control
+00013480: 5c22 203e 5c72 5c6e 5c74 5c74 5c74 5c74  \" >\r\n\t\t\t\t
+00013490: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
+000134a0: 5c74 5c74 5c74 5c74 5c74 3c64 6976 0a20  \t\t\t\t\t<div. 
+000134b0: 2020 2020 2020 2063 6c61 7373 3d5c 2266         class=\"f
+000134c0: 6f72 6d2d 6772 6f75 7020 7265 7175 6972  orm-group requir
+000134d0: 6564 5c22 3e5c 725c 6e5c 745c 745c 745c  ed\">\r\n\t\t\t\
+000134e0: 745c 745c 745c 743c 6c61 6265 6c20 666f  t\t\t\t<label fo
+000134f0: 723d 5c22 6f73 616b 6173 2e6b 6174 755c  r=\"osakas.katu\
+00013500: 223e 4b69 696e 7465 6973 745c 7846 366e  ">Kiinteist\xF6n
+00013510: 0a20 2020 2020 2020 206f 736f 6974 653c  .        osoite<
+00013520: 2f6c 6162 656c 3e20 5c72 5c6e 5c74 5c74  /label> \r\n\t\t
+00013530: 5c74 5c74 5c74 5c74 5c74 3c69 6e70 7574  \t\t\t\t\t<input
+00013540: 2072 6571 7569 7265 6420 7479 7065 3d5c   required type=\
+00013550: 2274 6578 745c 2220 6e61 6d65 3d5c 226f  "text\" name=\"o
+00013560: 7361 6b61 732e 6b61 7475 5c22 0a20 2020  sakas.katu\".   
+00013570: 2020 2020 2063 6c61 7373 3d5c 2266 6f72       class=\"for
+00013580: 6d2d 636f 6e74 726f 6c5c 2220 3e5c 725c  m-control\" >\r\
+00013590: 6e5c 745c 745c 745c 745c 745c 743c 2f64  n\t\t\t\t\t\t</d
+000135a0: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
+000135b0: 745c 743c 6469 7620 636c 6173 733d 5c22  t\t<div class=\"
+000135c0: 666f 726d 2d67 726f 7570 0a20 2020 2020  form-group.     
+000135d0: 2020 2072 6571 7569 7265 645c 223e 5c72     required\">\r
+000135e0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c74  \n\t\t\t\t\t\t\t
+000135f0: 3c6c 6162 656c 2066 6f72 3d5c 226f 7361  <label for=\"osa
+00013600: 6b61 732e 706f 7374 695c 223e 506f 7374  kas.posti\">Post
+00013610: 696e 756d 6572 6f20 6a61 202d 746f 696d  inumero ja -toim
+00013620: 6970 6169 6b6b 613c 2f6c 6162 656c 3e0a  ipaikka</label>.
+00013630: 2020 2020 2020 2020 5c72 5c6e 5c74 5c74          \r\n\t\t
+00013640: 5c74 5c74 5c74 5c74 5c74 3c69 6e70 7574  \t\t\t\t\t<input
+00013650: 2072 6571 7569 7265 6420 7479 7065 3d5c   required type=\
+00013660: 2274 6578 745c 2220 6e61 6d65 3d5c 226f  "text\" name=\"o
+00013670: 7361 6b61 732e 706f 7374 695c 2220 636c  sakas.posti\" cl
+00013680: 6173 733d 5c22 666f 726d 2d63 6f6e 7472  ass=\"form-contr
+00013690: 6f6c 5c22 0a20 2020 2020 2020 203e 5c72  ol\".        >\r
+000136a0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \n\t\t\t\t\t\t</
+000136b0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
+000136c0: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 5c74  \t\t\r\n\t\t\t\t
+000136d0: 5c74 5c74 5c72 5c6e 5c74 5c74 5c74 5c74  \t\t\r\n\t\t\t\t
+000136e0: 5c74 5c74 5c74 3c64 6976 0a20 2020 2020  \t\t\t<div.     
+000136f0: 2020 2063 6c61 7373 3d5c 2266 6f72 6d2d     class=\"form-
+00013700: 6772 6f75 705c 223e 5c72 5c6e 5c74 5c74  group\">\r\n\t\t
+00013710: 5c74 5c74 5c74 5c74 5c74 5c74 3c6c 6162  \t\t\t\t\t\t<lab
+00013720: 656c 2066 6f72 3d5c 226f 7361 6b61 732e  el for=\"osakas.
+00013730: 6865 6e6b 696c 6f74 756e 6e75 7353 7472  henkilotunnusStr
+00013740: 696e 675c 223e 4865 6e6b 696c 5c78 4636  ing\">Henkil\xF6
+00013750: 7475 6e6e 7573 2f59 2d74 756e 6e75 733c  tunnus/Y-tunnus<
+00013760: 2f6c 6162 656c 3e5c 725c 6e5c 745c 745c  /label>\r\n\t\t\
+00013770: 745c 745c 745c 745c 745c 743c 696e 7075  t\t\t\t\t\t<inpu
+00013780: 740a 2020 2020 2020 2020 7479 7065 3d5c  t.        type=\
+00013790: 2274 6578 745c 2220 6e61 6d65 3d5c 226f  "text\" name=\"o
+000137a0: 7361 6b61 732e 6865 6e6b 696c 6f74 756e  sakas.henkilotun
+000137b0: 6e75 7353 7472 696e 675c 2220 636c 6173  nusString\" clas
+000137c0: 733d 5c22 666f 726d 2d63 6f6e 7472 6f6c  s=\"form-control
+000137d0: 5c22 203e 5c72 5c6e 5c74 5c74 5c74 5c74  \" >\r\n\t\t\t\t
+000137e0: 5c74 5c74 5c74 3c2f 6469 763e 5c72 5c6e  \t\t\t</div>\r\n
+000137f0: 5c74 5c74 5c74 5c74 5c74 5c74 5c72 5c6e  \t\t\t\t\t\t\r\n
+00013800: 5c74 5c74 5c74 5c74 5c74 3c2f 6669 656c  \t\t\t\t\t</fiel
+00013810: 6473 6574 3e5c 725c 6e5c 745c 745c 745c  dset>\r\n\t\t\t\
+00013820: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
+00013830: 745c 743c 6469 760a 2020 2020 2020 2020  t\t<div.        
+00013840: 636c 6173 733d 5c22 636f 6c2d 6d64 2d36  class=\"col-md-6
+00013850: 5c22 3e5c 725c 6e5c 745c 745c 745c 745c  \">\r\n\t\t\t\t\
+00013860: 743c 6669 656c 6473 6574 2063 6c61 7373  t<fieldset class
+00013870: 3d5c 2266 6965 6c64 7365 7420 6d61 7267  =\"fieldset marg
+00013880: 696e 2d62 6f74 746f 6d2d 3135 5c22 3e5c  in-bottom-15\">\
+00013890: 725c 6e5c 745c 745c 745c 745c 745c 743c  r\n\t\t\t\t\t\t<
+000138a0: 6c65 6765 6e64 3e4d 616b 7361 6a61 6e0a  legend>Maksajan.
+000138b0: 2020 2020 2020 2020 7469 6564 6f74 3c2f          tiedot</
+000138c0: 6c65 6765 6e64 3e5c 725c 6e5c 745c 745c  legend>\r\n\t\t\
+000138d0: 745c 745c 745c 743c 6469 7620 636c 6173  t\t\t\t<div clas
+000138e0: 733d 5c22 6368 6563 6b62 6f78 5c22 3e5c  s=\"checkbox\">\
+000138f0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+00013900: 743c 6c61 6265 6c0a 2020 2020 2020 2020  t<label.        
+00013910: 666f 723d 5c22 7361 6d65 5f61 735f 6265  for=\"same_as_be
+00013920: 666f 7265 5c22 3e5c 725c 6e5c 745c 745c  fore\">\r\n\t\t\
+00013930: 745c 745c 745c 745c 745c 743c 696e 7075  t\t\t\t\t\t<inpu
+00013940: 7420 7479 7065 3d5c 2263 6865 636b 626f  t type=\"checkbo
+00013950: 785c 2220 6964 3d5c 2273 616d 655f 6173  x\" id=\"same_as
+00013960: 5f62 6566 6f72 655c 220a 2020 2020 2020  _before\".      
+00013970: 2020 6e61 6d65 3d5c 2273 616d 655f 6173    name=\"same_as
+00013980: 5f62 6566 6f72 655c 2220 6461 7461 2d61  _before\" data-a
+00013990: 6374 696f 6e3d 5c22 7361 6d65 2d61 732d  ction=\"same-as-
+000139a0: 6265 666f 7265 5c22 203e 5c72 5c6e 5c74  before\" >\r\n\t
+000139b0: 5c74 5c74 5c74 5c74 5c74 5c74 5c74 5361  \t\t\t\t\t\t\tSa
+000139c0: 6d61 740a 2020 2020 2020 2020 6b75 696e  mat.        kuin
+000139d0: 206f 7361 6b6b 6161 6e5c 725c 6e5c 745c   osakkaan\r\n\t\
+000139e0: 745c 745c 745c 745c 745c 743c 2f6c 6162  t\t\t\t\t\t</lab
+000139f0: 656c 3e5c 725c 6e5c 745c 745c 745c 745c  el>\r\n\t\t\t\t\
+00013a00: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
+00013a10: 745c 745c 745c 745c 743c 6469 760a 2020  t\t\t\t\t<div.  
+00013a20: 2020 2020 2020 636c 6173 733d 5c22 666f        class=\"fo
+00013a30: 726d 2d67 726f 7570 2072 6571 7569 7265  rm-group require
+00013a40: 645c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  d\">\r\n\t\t\t\t
+00013a50: 5c74 5c74 5c74 3c6c 6162 656c 2066 6f72  \t\t\t<label for
+00013a60: 3d5c 226f 7361 6b61 732e 6c61 736b 7574  =\"osakas.laskut
+00013a70: 7573 6e69 6d69 5c22 3e4d 616b 7361 6a61  usnimi\">Maksaja
+00013a80: 6e0a 2020 2020 2020 2020 6e69 6d69 3c2f  n.        nimi</
+00013a90: 6c61 6265 6c3e 205c 725c 6e5c 745c 745c  label> \r\n\t\t\
+00013aa0: 745c 745c 745c 745c 743c 696e 7075 7420  t\t\t\t\t<input 
+00013ab0: 7265 7175 6972 6564 2074 7970 653d 5c22  required type=\"
+00013ac0: 7465 7874 5c22 206e 616d 653d 5c22 6f73  text\" name=\"os
+00013ad0: 616b 6173 2e6c 6173 6b75 7475 736e 696d  akas.laskutusnim
+00013ae0: 695c 220a 2020 2020 2020 2020 636c 6173  i\".        clas
+00013af0: 733d 5c22 666f 726d 2d63 6f6e 7472 6f6c  s=\"form-control
+00013b00: 5c22 203e 5c72 5c6e 5c74 5c74 5c74 5c74  \" >\r\n\t\t\t\t
+00013b10: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
+00013b20: 5c74 5c74 5c74 5c74 5c74 3c64 6976 2063  \t\t\t\t\t<div c
+00013b30: 6c61 7373 3d5c 2266 6f72 6d2d 6772 6f75  lass=\"form-grou
+00013b40: 700a 2020 2020 2020 2020 7265 7175 6972  p.        requir
+00013b50: 6564 5c22 3e5c 725c 6e5c 745c 745c 745c  ed\">\r\n\t\t\t\
+00013b60: 745c 745c 745c 743c 6c61 6265 6c20 666f  t\t\t\t<label fo
+00013b70: 723d 5c22 6f73 616b 6173 2e6c 6173 6b75  r=\"osakas.lasku
+00013b80: 7475 7365 7475 6e69 6d69 5c22 3e4d 616b  tusetunimi\">Mak
+00013b90: 7361 6a61 6e0a 2020 2020 2020 2020 6574  sajan.        et
+00013ba0: 756e 696d 693c 2f6c 6162 656c 3e5c 725c  unimi</label>\r\
+00013bb0: 6e5c 745c 745c 745c 745c 745c 745c 743c  n\t\t\t\t\t\t\t<
+00013bc0: 696e 7075 7420 7265 7175 6972 6564 2074  input required t
+00013bd0: 7970 653d 5c22 7465 7874 5c22 206e 616d  ype=\"text\" nam
+00013be0: 653d 5c22 6f73 616b 6173 2e6c 6173 6b75  e=\"osakas.lasku
+00013bf0: 7475 7365 7475 6e69 6d69 5c22 0a20 2020  tusetunimi\".   
+00013c00: 2020 2020 2063 6c61 7373 3d5c 2266 6f72       class=\"for
+00013c10: 6d2d 636f 6e74 726f 6c5c 2220 3e5c 725c  m-control\" >\r\
+00013c20: 6e5c 745c 745c 745c 745c 745c 743c 2f64  n\t\t\t\t\t\t</d
+00013c30: 6976 3e5c 725c 6e5c 745c 745c 745c 745c  iv>\r\n\t\t\t\t\
+00013c40: 745c 743c 6469 7620 636c 6173 733d 5c22  t\t<div class=\"
+00013c50: 666f 726d 2d67 726f 7570 0a20 2020 2020  form-group.     
+00013c60: 2020 2072 6571 7569 7265 645c 2220 7374     required\" st
+00013c70: 796c 653d 5c22 6469 7370 6c61 793a 6e6f  yle=\"display:no
+00013c80: 6e65 5c22 3e5c 725c 6e5c 745c 745c 745c  ne\">\r\n\t\t\t\
+00013c90: 745c 745c 745c 743c 6c61 6265 6c20 666f  t\t\t\t<label fo
+00013ca0: 723d 5c22 6f73 616b 6173 2e6c 6173 6b75  r=\"osakas.lasku
+00013cb0: 7475 7373 756b 756e 696d 695c 223e 4d61  tussukunimi\">Ma
+00013cc0: 6b73 616a 616e 0a20 2020 2020 2020 2073  ksajan.        s
+00013cd0: 756b 756e 696d 693c 2f6c 6162 656c 3e5c  ukunimi</label>\
+00013ce0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+00013cf0: 743c 696e 7075 7420 7265 7175 6972 6564  t<input required
+00013d00: 2074 7970 653d 5c22 7465 7874 5c22 206e   type=\"text\" n
+00013d10: 616d 653d 5c22 6f73 616b 6173 2e6c 6173  ame=\"osakas.las
+00013d20: 6b75 7475 7373 756b 756e 696d 695c 220a  kutussukunimi\".
+00013d30: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+00013d40: 666f 726d 2d63 6f6e 7472 6f6c 5c22 203e  form-control\" >
+00013d50: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+00013d60: 3c2f 6469 763e 5c72 5c6e 5c74 5c74 5c74  </div>\r\n\t\t\t
+00013d70: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
+00013d80: 3d5c 2266 6f72 6d2d 6772 6f75 705c 223e  =\"form-group\">
+00013d90: 5c72 5c6e 5c74 5c74 5c74 5c74 5c74 5c74  \r\n\t\t\t\t\t\t
+00013da0: 5c74 3c6c 6162 656c 0a20 2020 2020 2020  \t<label.       
+00013db0: 2066 6f72 3d5c 226f 7361 6b61 732e 6c61   for=\"osakas.la
+00013dc0: 736b 7574 7573 7968 7465 7973 6865 6e6b  skutusyhteyshenk
+00013dd0: 5c22 3e4d 616b 7361 6a61 6e20 7968 7465  \">Maksajan yhte
+00013de0: 7973 6865 6e6b 696c 5c78 4636 3c2f 6c61  yshenkil\xF6</la
+00013df0: 6265 6c3e 5c72 5c6e 5c74 5c74 5c74 5c74  bel>\r\n\t\t\t\t
+00013e00: 5c74 5c74 5c74 3c69 6e70 7574 0a20 2020  \t\t\t<input.   
+00013e10: 2020 2020 2074 7970 653d 5c22 7465 7874       type=\"text
+00013e20: 5c22 206e 616d 653d 5c22 6f73 616b 6173  \" name=\"osakas
+00013e30: 2e6c 6173 6b75 7475 7379 6874 6579 7368  .laskutusyhteysh
+00013e40: 656e 6b5c 2220 636c 6173 733d 5c22 666f  enk\" class=\"fo
+00013e50: 726d 2d63 6f6e 7472 6f6c 5c22 203e 5c72  rm-control\" >\r
+00013e60: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \n\t\t\t\t\t\t</
+00013e70: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
+00013e80: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
+00013e90: 2063 6c61 7373 3d5c 2266 6f72 6d2d 6772   class=\"form-gr
+00013ea0: 6f75 7020 7265 7175 6972 6564 5c22 3e5c  oup required\">\
+00013eb0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+00013ec0: 743c 6c61 6265 6c20 666f 723d 5c22 6f73  t<label for=\"os
+00013ed0: 616b 6173 2e6c 6173 6b75 7475 736b 6174  akas.laskutuskat
+00013ee0: 755c 223e 4b69 696e 7465 6973 745c 7846  u\">Kiinteist\xF
+00013ef0: 366e 0a20 2020 2020 2020 206f 736f 6974  6n.        osoit
+00013f00: 653c 2f6c 6162 656c 3e20 5c72 5c6e 5c74  e</label> \r\n\t
+00013f10: 5c74 5c74 5c74 5c74 5c74 5c74 3c69 6e70  \t\t\t\t\t\t<inp
+00013f20: 7574 2072 6571 7569 7265 6420 7479 7065  ut required type
+00013f30: 3d5c 2274 6578 745c 2220 6e61 6d65 3d5c  =\"text\" name=\
+00013f40: 226f 7361 6b61 732e 6c61 736b 7574 7573  "osakas.laskutus
+00013f50: 6b61 7475 5c22 0a20 2020 2020 2020 2063  katu\".        c
+00013f60: 6c61 7373 3d5c 2266 6f72 6d2d 636f 6e74  lass=\"form-cont
+00013f70: 726f 6c5c 2220 3e5c 725c 6e5c 745c 745c  rol\" >\r\n\t\t\
+00013f80: 745c 745c 745c 743c 2f64 6976 3e5c 725c  t\t\t\t</div>\r\
+00013f90: 6e5c 745c 745c 745c 745c 745c 743c 6469  n\t\t\t\t\t\t<di
+00013fa0: 7620 636c 6173 733d 5c22 666f 726d 2d67  v class=\"form-g
+00013fb0: 726f 7570 0a20 2020 2020 2020 2072 6571  roup.        req
+00013fc0: 7569 7265 645c 223e 5c72 5c6e 5c74 5c74  uired\">\r\n\t\t
+00013fd0: 5c74 5c74 5c74 5c74 5c74 3c6c 6162 656c  \t\t\t\t\t<label
+00013fe0: 2066 6f72 3d5c 226f 7361 6b61 732e 6c61   for=\"osakas.la
+00013ff0: 736b 7574 7573 706f 7374 695c 223e 506f  skutusposti\">Po
+00014000: 7374 696e 756d 6572 6f0a 2020 2020 2020  stinumero.      
+00014010: 2020 6a61 202d 746f 696d 6970 6169 6b6b    ja -toimipaikk
+00014020: 613c 2f6c 6162 656c 3e20 5c72 5c6e 5c74  a</label> \r\n\t
+00014030: 5c74 5c74 5c74 5c74 5c74 5c74 3c69 6e70  \t\t\t\t\t\t<inp
+00014040: 7574 2074 7970 653d 5c22 7465 7874 5c22  ut type=\"text\"
+00014050: 2072 6571 7569 7265 6420 6e61 6d65 3d5c   required name=\
+00014060: 226f 7361 6b61 732e 6c61 736b 7574 7573  "osakas.laskutus
+00014070: 706f 7374 695c 220a 2020 2020 2020 2020  posti\".        
+00014080: 636c 6173 733d 5c22 666f 726d 2d63 6f6e  class=\"form-con
+00014090: 7472 6f6c 5c22 203e 5c72 5c6e 5c74 5c74  trol\" >\r\n\t\t
+000140a0: 5c74 5c74 5c74 5c74 3c2f 6469 763e 5c72  \t\t\t\t</div>\r
+000140b0: 5c6e 5c74 5c74 5c74 5c74 5c74 3c2f 6669  \n\t\t\t\t\t</fi
+000140c0: 656c 6473 6574 3e5c 725c 6e5c 745c 745c  eldset>\r\n\t\t\
+000140d0: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
+000140e0: 745c 743c 2f64 6976 3e5c 725c 6e5c 725c  t\t</div>\r\n\r\
+000140f0: 6e5c 745c 745c 743c 6469 760a 2020 2020  n\t\t\t<div.    
+00014100: 2020 2020 636c 6173 733d 5c22 726f 7720      class=\"row 
+00014110: 6274 6e2d 726f 775c 223e 5c72 5c6e 5c74  btn-row\">\r\n\t
+00014120: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
+00014130: 3d5c 2263 6f6c 2d6d 642d 3132 2074 6578  =\"col-md-12 tex
+00014140: 742d 6365 6e74 6572 5c22 3e5c 725c 6e5c  t-center\">\r\n\
+00014150: 745c 745c 745c 745c 743c 756c 0a20 2020  t\t\t\t\t<ul.   
+00014160: 2020 2020 2063 6c61 7373 3d5c 226c 6973       class=\"lis
+00014170: 742d 696e 6c69 6e65 5c22 3e5c 725c 6e5c  t-inline\">\r\n\
+00014180: 745c 745c 745c 745c 745c 745c 725c 6e5c  t\t\t\t\t\t\r\n\
+00014190: 745c 745c 745c 745c 745c 743c 6c69 3e5c  t\t\t\t\t\t<li>\
+000141a0: 725c 6e5c 745c 745c 745c 745c 745c 745c  r\n\t\t\t\t\t\t\
+000141b0: 743c 6275 7474 6f6e 0a20 2020 2020 2020  t<button.       
+000141c0: 2074 7970 653d 5c22 6275 7474 6f6e 5c22   type=\"button\"
+000141d0: 2063 6c61 7373 3d5c 2262 746e 2062 746e   class=\"btn btn
+000141e0: 2d70 7269 6d61 7279 5c22 2064 6174 612d  -primary\" data-
+000141f0: 6163 7469 6f6e 3d5c 2273 6176 652d 6164  action=\"save-ad
+00014200: 645c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  d\">\r\n\t\t\t\t
+00014210: 5c74 5c74 5c74 5c74 4a61 746b 615c 725c  \t\t\t\tJatka\r\
+00014220: 6e5c 745c 745c 745c 745c 745c 745c 743c  n\t\t\t\t\t\t\t<
+00014230: 2f62 7574 746f 6e3e 5c72 5c6e 5c74 5c74  /button>\r\n\t\t
+00014240: 5c74 5c74 5c74 5c74 3c2f 6c69 3e5c 725c  \t\t\t\t</li>\r\
+00014250: 6e5c 745c 745c 745c 745c 745c 745c 725c  n\t\t\t\t\t\t\r\
+00014260: 6e5c 745c 745c 745c 745c 745c 743c 6c69  n\t\t\t\t\t\t<li
+00014270: 3e5c 725c 6e5c 745c 745c 745c 745c 745c  >\r\n\t\t\t\t\t\
+00014280: 745c 743c 6275 7474 6f6e 0a20 2020 2020  t\t<button.     
+00014290: 2020 2074 7970 653d 5c22 6275 7474 6f6e     type=\"button
+000142a0: 5c22 2063 6c61 7373 3d5c 2262 746e 2062  \" class=\"btn b
+000142b0: 746e 2d70 7269 6d61 7279 5c22 2064 6174  tn-primary\" dat
+000142c0: 612d 6163 7469 6f6e 3d5c 2263 616e 6365  a-action=\"cance
+000142d0: 6c2d 6164 645c 223e 5c72 5c6e 5c74 5c74  l-add\">\r\n\t\t
+000142e0: 5c74 5c74 5c74 5c74 5c74 5c74 5065 7275  \t\t\t\t\t\tPeru
+000142f0: 7574 615c 725c 6e5c 745c 745c 745c 745c  uta\r\n\t\t\t\t\
+00014300: 745c 745c 743c 2f62 7574 746f 6e3e 5c72  t\t\t</button>\r
+00014310: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 3c2f  \n\t\t\t\t\t\t</
+00014320: 6c69 3e5c 725c 6e5c 745c 745c 745c 745c  li>\r\n\t\t\t\t\
+00014330: 743c 2f75 6c3e 5c72 5c6e 5c74 5c74 5c74  t</ul>\r\n\t\t\t
+00014340: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
+00014350: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
+00014360: 3c2f 666f 726d 3e5c 725c 6e5c 743c 2f64  </form>\r\n\t</d
+00014370: 6976 3e5c 725c 6e3c 2f64 6976 3e5c 725c  iv>\r\n</div>\r\
+00014380: 6e3c 2f73 6372 6970 743e 5c72 5c6e 5c72  n</script>\r\n\r
+00014390: 5c6e 3c73 6372 6970 740a 2020 2020 2020  \n<script.      
+000143a0: 2020 6964 3d5c 2261 6b70 2d73 656c 6563    id=\"akp-selec
+000143b0: 742d 7465 6d70 6c61 7465 5c22 2074 7970  t-template\" typ
+000143c0: 653d 5c22 7465 7874 2f78 2d74 656d 706c  e=\"text/x-templ
+000143d0: 6174 655c 223e 5c72 5c6e 5c72 5c6e 5c72  ate\">\r\n\r\n\r
+000143e0: 5c6e 3c64 6976 2063 6c61 7373 3d5c 2266  \n<div class=\"f
+000143f0: 6f72 6d43 6f6c 5c22 3e5c 725c 6e5c 743c  ormCol\">\r\n\t<
+00014400: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
+00014410: 733d 5c22 636f 6e74 6169 6e65 722d 666c  s=\"container-fl
+00014420: 7569 645c 223e 5c72 5c6e 5c74 5c74 3c64  uid\">\r\n\t\t<d
+00014430: 6976 2063 6c61 7373 3d5c 2272 6f77 5c22  iv class=\"row\"
+00014440: 3e5c 725c 6e5c 745c 745c 743c 6469 7620  >\r\n\t\t\t<div 
+00014450: 636c 6173 733d 5c22 636f 6c2d 6d64 2d34  class=\"col-md-4
+00014460: 5c22 3e5c 725c 6e5c 745c 745c 745c 743c  \">\r\n\t\t\t\t<
+00014470: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
+00014480: 733d 5c22 666f 726d 2d67 726f 7570 5c22  s=\"form-group\"
+00014490: 3e5c 725c 6e5c 745c 745c 745c 745c 743c  >\r\n\t\t\t\t\t<
+000144a0: 6c61 6265 6c20 666f 723d 5c22 636f 6d6d  label for=\"comm
+000144b0: 756e 6974 792d 7365 6c65 6374 6f72 5c22  unity-selector\"
+000144c0: 3e56 616c 6974 7365 0a20 2020 2020 2020  >Valitse.       
+000144d0: 206b 756e 7461 3c2f 6c61 6265 6c3e 5c72   kunta</label>\r
+000144e0: 5c6e 5c74 5c74 5c74 5c74 5c74 3c73 656c  \n\t\t\t\t\t<sel
+000144f0: 6563 7420 6964 3d5c 2263 6f6d 6d75 6e69  ect id=\"communi
+00014500: 7479 2d73 656c 6563 746f 725c 2220 636c  ty-selector\" cl
+00014510: 6173 733d 5c22 666f 726d 2d63 6f6e 7472  ass=\"form-contr
+00014520: 6f6c 5c22 0a20 2020 2020 2020 2064 6174  ol\".        dat
+00014530: 612d 726f 6c65 3d5c 2263 6f6d 6d75 6e69  a-role=\"communi
+00014540: 7479 2d73 656c 6563 746f 725c 223e 3c2f  ty-selector\"></
+00014550: 7365 6c65 6374 3e5c 725c 6e5c 745c 745c  select>\r\n\t\t\
+00014560: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
+00014570: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+00014580: 2020 636c 6173 733d 5c22 666f 726d 2d67    class=\"form-g
+00014590: 726f 7570 5c22 3e5c 725c 6e5c 745c 745c  roup\">\r\n\t\t\
+000145a0: 745c 745c 743c 6c61 6265 6c20 666f 723d  t\t\t<label for=
+000145b0: 5c22 616b 702d 7365 6c65 6374 6f72 5c22  \"akp-selector\"
+000145c0: 3e56 616c 6974 7365 2070 6973 7465 3c2f  >Valitse piste</
+000145d0: 6c61 6265 6c3e 5c72 5c6e 5c74 5c74 5c74  label>\r\n\t\t\t
+000145e0: 5c74 5c74 3c73 656c 6563 740a 2020 2020  \t\t<select.    
+000145f0: 2020 2020 6964 3d5c 2261 6b70 2d73 656c      id=\"akp-sel
+00014600: 6563 746f 725c 2220 636c 6173 733d 5c22  ector\" class=\"
+00014610: 666f 726d 2d63 6f6e 7472 6f6c 5c22 2064  form-control\" d
+00014620: 6174 612d 726f 6c65 3d5c 2261 6b70 2d73  ata-role=\"akp-s
+00014630: 656c 6563 746f 725c 223e 3c2f 7365 6c65  elector\"></sele
+00014640: 6374 3e5c 725c 6e5c 745c 745c 745c 743c  ct>\r\n\t\t\t\t<
+00014650: 2f64 6976 3e5c 725c 6e5c 725c 6e5c 745c  /div>\r\n\r\n\t\
+00014660: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+00014670: 2020 636c 6173 733d 5c22 726f 775c 2220    class=\"row\" 
+00014680: 6461 7461 2d72 6f6c 653d 5c22 6275 7474  data-role=\"butt
+00014690: 6f6e 2d63 6f6e 7461 696e 6572 5c22 2073  on-container\" s
+000146a0: 7479 6c65 3d5c 2264 6973 706c 6179 3a20  tyle=\"display: 
+000146b0: 6e6f 6e65 5c22 3e5c 725c 6e5c 745c 745c  none\">\r\n\t\t\
+000146c0: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+000146d0: 2020 636c 6173 733d 5c22 636f 6c2d 6d64    class=\"col-md
+000146e0: 2d31 325c 223e 5c72 5c6e 5c74 5c74 5c74  -12\">\r\n\t\t\t
+000146f0: 5c74 5c74 5c74 3c62 7574 746f 6e20 6461  \t\t\t<button da
+00014700: 7461 2d72 6f6c 653d 5c22 6f6b 5c22 2063  ta-role=\"ok\" c
+00014710: 6c61 7373 3d5c 2262 746e 2062 746e 2d70  lass=\"btn btn-p
+00014720: 7269 6d61 7279 0a20 2020 2020 2020 2062  rimary.        b
+00014730: 746e 2d62 6c6f 636b 5c22 3e48 7976 5c78  tn-block\">Hyv\x
+00014740: 4534 6b73 7920 7661 6c69 7474 7520 7069  E4ksy valittu pi
+00014750: 7374 653c 2f62 7574 746f 6e3e 5c72 5c6e  ste</button>\r\n
+00014760: 5c74 5c74 5c74 5c74 5c74 5c74 3c62 7574  \t\t\t\t\t\t<but
+00014770: 746f 6e20 6461 7461 2d72 6f6c 653d 5c22  ton data-role=\"
+00014780: 6361 6e63 656c 5c22 0a20 2020 2020 2020  cancel\".       
+00014790: 2063 6c61 7373 3d5c 2262 746e 2062 746e   class=\"btn btn
+000147a0: 2d64 6566 6175 6c74 2062 746e 2d62 6c6f  -default btn-blo
+000147b0: 636b 5c22 3e50 6572 7575 7461 3c2f 6275  ck\">Peruuta</bu
+000147c0: 7474 6f6e 3e5c 725c 6e5c 745c 745c 745c  tton>\r\n\t\t\t\
+000147d0: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
+000147e0: 745c 745c 743c 2f64 6976 3e5c 725c 6e5c  t\t\t</div>\r\n\
+000147f0: 725c 6e5c 745c 745c 745c 743c 6469 760a  r\n\t\t\t\t<div.
+00014800: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+00014810: 726f 775c 223e 5c72 5c6e 5c74 5c74 5c74  row\">\r\n\t\t\t
+00014820: 5c74 5c74 3c64 6976 2063 6c61 7373 3d5c  \t\t<div class=\
+00014830: 2263 6f6c 2d6d 642d 3132 5c22 3e5c 725c  "col-md-12\">\r\
+00014840: 6e5c 745c 745c 745c 745c 745c 743c 7020  n\t\t\t\t\t\t<p 
+00014850: 636c 6173 733d 5c22 6865 6c70 2d62 6c6f  class=\"help-blo
+00014860: 636b 0a20 2020 2020 2020 2074 6578 742d  ck.        text-
+00014870: 6365 6e74 6572 5c22 3e56 6f69 7420 7661  center\">Voit va
+00014880: 6c69 7461 2070 6973 7465 656e 206d 795c  lita pisteen my\
+00014890: 7846 3673 206b 6172 7461 6c74 613c 2f70  xF6s kartalta</p
+000148a0: 3e5c 725c 6e5c 745c 745c 745c 745c 743c  >\r\n\t\t\t\t\t<
+000148b0: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
+000148c0: 743c 2f64 6976 3e5c 725c 6e5c 745c 745c  t</div>\r\n\t\t\
+000148d0: 743c 2f64 6976 3e5c 725c 6e5c 725c 6e5c  t</div>\r\n\r\n\
+000148e0: 745c 745c 743c 6469 760a 2020 2020 2020  t\t\t<div.      
+000148f0: 2020 636c 6173 733d 5c22 636f 6c2d 6d64    class=\"col-md
+00014900: 2d38 5c22 3e5c 725c 6e5c 745c 745c 745c  -8\">\r\n\t\t\t\
+00014910: 743c 6469 7620 6964 3d5c 2261 6b70 2d6d  t<div id=\"akp-m
+00014920: 6170 5c22 2064 6174 612d 726f 6c65 3d5c  ap\" data-role=\
+00014930: 226d 6170 5c22 3e3c 2f64 6976 3e5c 725c  "map\"></div>\r\
+00014940: 6e5c 745c 745c 743c 2f64 6976 3e5c 725c  n\t\t\t</div>\r\
+00014950: 6e5c 745c 743c 2f64 6976 3e5c 725c 6e5c  n\t\t</div>\r\n\
+00014960: 743c 2f64 6976 3e5c 725c 6e3c 2f64 6976  t</div>\r\n</div
+00014970: 3e5c 725c 6e3c 2f73 6372 6970 743e 5c72  >\r\n</script>\r
+00014980: 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e 5c72  \n\r\n\r\n\r\n\r
+00014990: 5c6e 5c72 5c6e 5c72 5c6e 5c72 5c6e 3c64  \n\r\n\r\n\r\n<d
+000149a0: 6976 0a20 2020 2020 2020 2069 643d 5c22  iv.        id=\"
+000149b0: 7761 7374 652d 7761 7465 722d 6d6f 6461  waste-water-moda
+000149c0: 6c5c 2220 636c 6173 733d 5c22 6d6f 6461  l\" class=\"moda
+000149d0: 6c5c 2220 7374 796c 653d 5c22 6469 7370  l\" style=\"disp
+000149e0: 6c61 793a 6e6f 6e65 5c22 3e5c 725c 6e20  lay:none\">\r\n 
+000149f0: 2020 203c 6469 760a 2020 2020 2020 2020     <div.        
+00014a00: 636c 6173 733d 5c22 6d6f 6461 6c2d 6469  class=\"modal-di
+00014a10: 616c 6f67 206d 6f64 616c 2d6c 675c 223e  alog modal-lg\">
+00014a20: 5c72 5c6e 2020 2020 2020 2020 3c64 6976  \r\n        <div
+00014a30: 2063 6c61 7373 3d5c 226d 6f64 616c 2d63   class=\"modal-c
+00014a40: 6f6e 7465 6e74 5c22 3e5c 725c 6e0a 2020  ontent\">\r\n.  
+00014a50: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+00014a60: 2020 3c64 6976 2063 6c61 7373 3d5c 226d    <div class=\"m
+00014a70: 6f64 616c 2d62 6f64 795c 223e 5c72 5c6e  odal-body\">\r\n
+00014a80: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00014a90: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
+00014aa0: 2270 6167 652d 6865 6164 6572 5c22 3e5c  "page-header\">\
+00014ab0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00014ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ad0: 3c68 313e 4c69 6974 7920 6c69 6574 7465  <h1>Liity liette
+00014ae0: 6964 656e 206b 6572 5c78 4534 796b 7365  iden ker\xE4ykse
+00014af0: 656e 3c2f 6831 3e5c 725c 6e20 2020 2020  en</h1>\r\n     
+00014b00: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00014b10: 3e5c 725c 6e5c 725c 6e0a 2020 2020 2020  >\r\n\r\n.      
+00014b20: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+00014b30: 2020 3c64 6976 2063 6c61 7373 3d5c 226c    <div class=\"l
+00014b40: 6f61 6469 6e67 2d69 636f 6e5c 223e 3c2f  oading-icon\"></
+00014b50: 6469 763e 5c72 5c6e 5c72 5c6e 2020 2020  div>\r\n\r\n    
+00014b60: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00014b70: 0a20 2020 2020 2020 2064 6174 612d 726f  .        data-ro
+00014b80: 6c65 3d5c 2274 6162 6261 725c 223e 5c72  le=\"tabbar\">\r
+00014b90: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00014ba0: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
+00014bb0: 2020 2020 2020 2020 2020 2020 2020 3c75                <u
+00014bc0: 6c20 636c 6173 733d 5c22 7461 622d 6c69  l class=\"tab-li
+00014bd0: 7374 0a20 2020 2020 2020 206c 6973 742d  st.        list-
+00014be0: 696e 6c69 6e65 5c22 2064 6174 612d 726f  inline\" data-ro
+00014bf0: 6c65 3d5c 2274 6162 2d6c 6973 745c 223e  le=\"tab-list\">
+00014c00: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00014c10: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
+00014c20: 636c 6173 733d 5c22 6163 7469 7665 0a20  class=\"active. 
+00014c30: 2020 2020 2020 2061 315c 223e 3c61 2068         a1\"><a h
+00014c40: 7265 663d 5c22 2361 315c 223e 4131 3c2f  ref=\"#a1\">A1</
+00014c50: 613e 3c2f 6c69 3e3c 6c69 2063 6c61 7373  a></li><li class
+00014c60: 3d5c 2261 3220 6469 7361 626c 6564 5c22  =\"a2 disabled\"
+00014c70: 3e3c 6120 6872 6566 3d5c 2223 6132 5c22  ><a href=\"#a2\"
+00014c80: 3e41 323c 2f61 3e3c 2f6c 693e 3c6c 690a  >A2</a></li><li.
+00014c90: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+00014ca0: 6133 2064 6973 6162 6c65 645c 223e 3c61  a3 disabled\"><a
+00014cb0: 2068 7265 663d 5c22 2361 335c 223e 4133   href=\"#a3\">A3
+00014cc0: 3c2f 613e 3c2f 6c69 3e3c 6c69 2063 6c61  </a></li><li cla
+00014cd0: 7373 3d5c 2261 3420 6469 7361 626c 6564  ss=\"a4 disabled
+00014ce0: 5c22 3e3c 610a 2020 2020 2020 2020 6872  \"><a.        hr
+00014cf0: 6566 3d5c 2223 6134 5c22 3e41 343c 2f61  ef=\"#a4\">A4</a
+00014d00: 3e3c 2f6c 693e 3c6c 6920 636c 6173 733d  ></li><li class=
+00014d10: 5c22 6135 2064 6973 6162 6c65 645c 223e  \"a5 disabled\">
+00014d20: 3c61 2068 7265 663d 5c22 2361 355c 223e  <a href=\"#a5\">
+00014d30: 4135 3c2f 613e 3c2f 6c69 3e3c 6c69 0a20  A5</a></li><li. 
+00014d40: 2020 2020 2020 2063 6c61 7373 3d5c 2261         class=\"a
+00014d50: 3620 6469 7361 626c 6564 5c22 3e3c 6120  6 disabled\"><a 
+00014d60: 6872 6566 3d5c 2223 6136 5c22 3e41 363c  href=\"#a6\">A6<
+00014d70: 2f61 3e3c 2f6c 693e 5c72 5c6e 2020 2020  /a></li>\r\n    
+00014d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d90: 3c2f 756c 3e5c 725c 6e0a 2020 2020 2020  </ul>\r\n.      
+00014da0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+00014db0: 2020 2020 2020 5c72 5c6e 2020 2020 2020        \r\n      
+00014dc0: 2020 2020 2020 2020 2020 2020 2020 5c72                \r
+00014dd0: 5c6e 5c72 5c6e 2020 2020 2020 2020 2020  \n\r\n          
+00014de0: 2020 2020 2020 2020 2020 5c72 5c6e 0a20            \r\n. 
+00014df0: 2020 2020 2020 205c 2020 2020 2020 2020         \        
+00014e00: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00014e10: 636c 6173 733d 5c22 6131 5c22 3e3c 2f64  class=\"a1\"></d
+00014e20: 6976 3e5c 725c 6e20 2020 2020 2020 2020  iv>\r\n         
+00014e30: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00014e40: 636c 6173 733d 5c22 6132 5c22 3e3c 2f64  class=\"a2\"></d
+00014e50: 6976 3e5c 725c 6e0a 2020 2020 2020 2020  iv>\r\n.        
+00014e60: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+00014e70: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
+00014e80: 2261 335c 223e 3c2f 6469 763e 5c72 5c6e  "a3\"></div>\r\n
+00014e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ea0: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
+00014eb0: 2261 345c 223e 3c2f 6469 763e 5c72 5c6e  "a4\"></div>\r\n
+00014ec0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+00014ed0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00014ee0: 7620 636c 6173 733d 5c22 6135 5c22 3e3c  v class=\"a5\"><
+00014ef0: 2f64 6976 3e5c 725c 6e5c 725c 6e20 2020  /div>\r\n\r\n   
+00014f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f10: 203c 6469 760a 2020 2020 2020 2020 636c   <div.        cl
+00014f20: 6173 733d 5c22 6136 5c22 3e5c 725c 6e20  ass=\"a6\">\r\n 
+00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f40: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00014f50: 733d 5c22 6d61 702d 696e 666f 5c22 3e5c  s=\"map-info\">\
+00014f60: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00014f70: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00014f80: 6469 763e 4b61 7274 7461 610a 2020 2020  div>Karttaa.    
+00014f90: 2020 2020 766f 6920 7369 6972 745c 7845      voi siirt\xE
+00014fa0: 345c 7845 3420 6869 6972 656c 6c5c 7845  4\xE4 hiirell\xE
+00014fb0: 3420 7261 6168 6161 6d61 6c6c 612e 204b  4 raahaamalla. K
+00014fc0: 6c69 6b6b 6161 2050 6169 6b6b 6120 2d70  likkaa Paikka -p
+00014fd0: 6169 6e69 6b65 7474 6120 6a61 2076 6965  ainiketta ja vie
+00014fe0: 0a20 2020 2020 2020 2068 6969 7269 206b  .        hiiri k
+00014ff0: 6172 7461 6c6c 6120 6b6f 6874 6161 6e2c  artalla kohtaan,
+00015000: 206a 6f73 7361 206b 6169 766f 206f 6e2e   jossa kaivo on.
+00015010: 204f 686a 656c 6d61 2076 6172 6d69 7374   Ohjelma varmist
+00015020: 6161 2076 6965 6c5c 7845 3420 7661 6c69  aa viel\xE4 vali
+00015030: 6e6e 616e 0a20 2020 2020 2020 206f 696b  nnan.        oik
+00015040: 6561 6b73 6920 3c2f 6469 763e 5c72 5c6e  eaksi </div>\r\n
+00015050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015060: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
+00015070: 746f 6e20 6461 7461 2d61 6374 696f 6e3d  ton data-action=
+00015080: 5c22 6d61 726b 2d77 656c 6c5c 223e 5061  \"mark-well\">Pa
+00015090: 696b 6b61 3c2f 6275 7474 6f6e 3e5c 725c  ikka</button>\r\
+000150a0: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+000150b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150c0: 2020 3c2f 6469 763e 5c72 5c6e 2020 2020    </div>\r\n    
+000150d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150e0: 2020 2020 3c64 6976 2064 6174 612d 726f      <div data-ro
+000150f0: 6c65 3d5c 226b 6172 7474 615c 220a 2020  le=\"kartta\".  
+00015100: 2020 2020 2020 636c 6173 733d 5c22 6d61        class=\"ma
+00015110: 705c 223e 3c2f 6469 763e 5c72 5c6e 2020  p\"></div>\r\n  
+00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015130: 2020 3c2f 6469 763e 5c72 5c6e 5c72 5c6e    </div>\r\n\r\n
+00015140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015150: 2020 2020 3c64 6976 0a20 2020 2020 2020      <div.       
+00015160: 2063 6c61 7373 3d5c 2267 6c6f 6261 6c2d   class=\"global-
+00015170: 7661 6c69 6461 7469 6f6e 2d65 7272 6f72  validation-error
+00015180: 2061 6c65 7274 2061 6c65 7274 2d64 616e   alert alert-dan
+00015190: 6765 725c 2220 7374 796c 653d 5c22 6469  ger\" style=\"di
+000151a0: 7370 6c61 793a 6e6f 6e65 5c22 3e54 5c78  splay:none\">T\x
+000151b0: 4534 7974 5c78 4534 0a20 2020 2020 2020  E4yt\xE4.       
+000151c0: 2070 7575 7474 7576 6174 206b 656e 745c   puuttuvat kent\
+000151d0: 7845 3474 3c2f 6469 763e 5c72 5c6e 2020  xE4t</div>\r\n  
+000151e0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000151f0: 6469 763e 5c72 5c6e 2020 2020 2020 2020  div>\r\n        
+00015200: 2020 2020 3c2f 6469 763e 5c72 5c6e 0a20      </div>\r\n. 
+00015210: 2020 2020 2020 205c 2020 2020 2020 203c         \       <
+00015220: 2f64 6976 3e5c 725c 6e20 2020 203c 2f64  /div>\r\n    </d
+00015230: 6976 3e5c 725c 6e3c 2f64 6976 3e5c 725c  iv>\r\n</div>\r\
+00015240: 6e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  n\r\n\r\n\r\n\r\
+00015250: 6e5c 725c 6e5c 725c 6e5c 725c 6e3c 6469  n\r\n\r\n\r\n<di
+00015260: 760a 2020 2020 2020 2020 6964 3d5c 2263  v.        id=\"c
+00015270: 6f6c 6c65 6374 696f 6e2d 7363 6865 6475  ollection-schedu
+00015280: 6c65 2d6d 6f64 616c 5c22 2063 6c61 7373  le-modal\" class
+00015290: 3d5c 226d 6f64 616c 5c22 2073 7479 6c65  =\"modal\" style
+000152a0: 3d5c 2264 6973 706c 6179 3a6e 6f6e 655c  =\"display:none\
+000152b0: 223e 5c72 5c6e 0a20 2020 2020 2020 205c  ">\r\n.        \
+000152c0: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
+000152d0: 6d6f 6461 6c2d 6469 616c 6f67 5c22 3e5c  modal-dialog\">\
+000152e0: 725c 6e20 2020 2020 2020 203c 6469 7620  r\n        <div 
+000152f0: 636c 6173 733d 5c22 6d6f 6461 6c2d 636f  class=\"modal-co
+00015300: 6e74 656e 745c 223e 5c72 5c6e 0a20 2020  ntent\">\r\n.   
+00015310: 2020 2020 205c 2020 2020 2020 2020 2020       \          
+00015320: 203c 6469 7620 636c 6173 733d 5c22 6d6f   <div class=\"mo
+00015330: 6461 6c2d 626f 6479 5c22 3e5c 725c 6e20  dal-body\">\r\n 
+00015340: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00015350: 6469 7620 636c 6173 733d 5c22 726f 775c  div class=\"row\
+00015360: 223e 5c72 5c6e 0a20 2020 2020 2020 205c  ">\r\n.        \
+00015370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015380: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
+00015390: 7061 6765 2d68 6561 6465 725c 223e 5c72  page-header\">\r
+000153a0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+000153b0: 2020 2020 2020 2020 2020 3c68 313e 4a5c            <h1>J\
+000153c0: 7845 3474 6561 7374 6961 6e0a 2020 2020  xE4teastian.    
+000153d0: 2020 2020 7479 686a 656e 6e79 7372 7974      tyhjennysryt
+000153e0: 6d69 3c2f 6831 3e5c 725c 6e20 2020 2020  mi</h1>\r\n     
+000153f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00015400: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
+00015410: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
+00015420: 725c 6e5c 725c 6e0a 2020 2020 2020 2020  r\n\r\n.        
+00015430: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+00015440: 3c64 6976 2063 6c61 7373 3d5c 2272 6f77  <div class=\"row
+00015450: 2063 7573 746f 6d65 722d 6461 7461 2d69   customer-data-i
+00015460: 6e66 6f5c 223e 5c72 5c6e 2020 2020 2020  nfo\">\r\n      
+00015470: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00015480: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+00015490: 3d5c 2270 6167 652d 6865 6164 6572 5c22  =\"page-header\"
+000154a0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+000154b0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+000154c0: 7620 636c 6173 733d 5c22 636f 6c2d 736d  v class=\"col-sm
+000154d0: 2d36 5c22 3e5c 725c 6e0a 2020 2020 2020  -6\">\r\n.      
+000154e0: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+000154f0: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
+00015500: 343e 5479 686a 656e 6e79 736f 736f 6974  4>Tyhjennysosoit
+00015510: 653c 2f68 343e 5c72 5c6e 2020 2020 2020  e</h4>\r\n      
+00015520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015530: 2020 2020 2020 3c61 6464 7265 7373 3e5c        <address>\
+00015540: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00015550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015560: 2020 2020 2020 2020 3c73 7061 6e20 6461          <span da
+00015570: 7461 2d72 6f6c 653d 5c22 6c6f 6361 7469  ta-role=\"locati
+00015580: 6f6e 2d6e 616d 655c 223e 3c2f 7370 616e  on-name\"></span
+00015590: 3e3c 6272 3e3c 6272 3e5c 725c 6e0a 2020  ><br><br>\r\n.  
+000155a0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
+000155b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155c0: 2020 3c73 7061 6e20 6461 7461 2d72 6f6c    <span data-rol
+000155d0: 653d 5c22 6c6f 6361 7469 6f6e 2d61 6464  e=\"location-add
+000155e0: 7265 7373 5c22 3e3c 2f73 7061 6e3e 3c62  ress\"></span><b
+000155f0: 723e 5c72 5c6e 0a20 2020 2020 2020 205c  r>\r\n.        \
+00015600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015610: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+00015620: 2064 6174 612d 726f 6c65 3d5c 226c 6f63   data-role=\"loc
+00015630: 6174 696f 6e2d 706f 7374 5c22 3e3c 2f73  ation-post\"></s
+00015640: 7061 6e3e 5c72 5c6e 0a20 2020 2020 2020  pan>\r\n.       
+00015650: 205c 2020 2020 2020 2020 2020 2020 2020   \              
+00015660: 2020 2020 2020 2020 2020 2020 203c 2f61               </a
+00015670: 6464 7265 7373 3e5c 725c 6e20 2020 2020  ddress>\r\n     
+00015680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015690: 2020 203c 2f64 6976 3e5c 725c 6e5c 725c     </div>\r\n\r\
+000156a0: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+000156b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156c0: 2020 3c64 6976 2063 6c61 7373 3d5c 2263    <div class=\"c
+000156d0: 6f6c 2d73 6d2d 365c 223e 5c72 5c6e 2020  ol-sm-6\">\r\n  
+000156e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156f0: 2020 2020 2020 2020 2020 3c68 343e 4c61            <h4>La
+00015700: 736b 7574 7573 6f73 6f69 7465 3c2f 6834  skutusosoite</h4
+00015710: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
+00015720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015730: 2020 2020 2020 2020 2020 3c61 6464 7265            <addre
+00015740: 7373 3e5c 725c 6e20 2020 2020 2020 2020  ss>\r\n         
+00015750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015760: 2020 2020 2020 203c 7370 616e 0a20 2020         <span.   
+00015770: 2020 2020 2064 6174 612d 726f 6c65 3d5c       data-role=\
+00015780: 2269 6e76 6f69 6369 6e67 2d6e 616d 655c  "invoicing-name\
+00015790: 223e 3c2f 7370 616e 3e3c 6272 3e3c 6272  "></span><br><br
+000157a0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+000157b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157c0: 2020 2020 203c 7370 616e 0a20 2020 2020       <span.     
+000157d0: 2020 2064 6174 612d 726f 6c65 3d5c 2269     data-role=\"i
+000157e0: 6e76 6f69 6369 6e67 2d61 6464 7265 7373  nvoicing-address
+000157f0: 5c22 3e3c 2f73 7061 6e3e 3c62 723e 5c72  \"></span><br>\r
+00015800: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00015810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015820: 2020 3c73 7061 6e0a 2020 2020 2020 2020    <span.        
+00015830: 6461 7461 2d72 6f6c 653d 5c22 696e 766f  data-role=\"invo
+00015840: 6963 696e 672d 706f 7374 5c22 3e3c 2f73  icing-post\"></s
+00015850: 7061 6e3e 5c72 5c6e 2020 2020 2020 2020  pan>\r\n        
+00015860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015870: 2020 2020 3c2f 6164 6472 6573 733e 5c72      </address>\r
+00015880: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
+00015890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000158a0: 2020 203c 2f64 6976 3e5c 725c 6e5c 725c     </div>\r\n\r\
+000158b0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+000158c0: 2020 2020 2020 2020 205c 725c 6e5c 725c           \r\n\r\
+000158d0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+000158e0: 2020 2020 2020 2020 203c 6469 760a 2020           <div.  
+000158f0: 2020 2020 2020 7374 796c 653d 5c22 636c        style=\"cl
+00015900: 6561 723a 626f 7468 5c22 3e3c 2f64 6976  ear:both\"></div
+00015910: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+00015920: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
+00015930: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00015940: 2020 203c 2f64 6976 3e5c 725c 6e5c 725c     </div>\r\n\r\
+00015950: 6e0a 2020 2020 2020 2020 5c20 2020 2020  n.        \     
+00015960: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00015970: 6c61 7373 3d5c 2273 6d61 6c6c 5c22 3e41  lass=\"small\">A
+00015980: 6a6f 705c 7845 3469 765c 7845 3420 766f  jop\xE4iv\xE4 vo
+00015990: 6920 6d75 7574 7475 6120 285c 7842 3120  i muuttua (\xB1 
+000159a0: 312d 320a 2020 2020 2020 2020 705c 7845  1-2.        p\xE
+000159b0: 3469 765c 7845 345c 7845 3429 2065 7369  4iv\xE4\xE4) esi
+000159c0: 6d2e 2061 726b 6970 7968 5c78 4534 7669  m. arkipyh\xE4vi
+000159d0: 696b 6f69 6c6c 612e 3c2f 6469 763e 5c72  ikoilla.</div>\r
+000159e0: 5c6e 5c72 5c6e 2020 2020 2020 2020 2020  \n\r\n          
+000159f0: 2020 2020 2020 3c64 6976 0a20 2020 2020        <div.     
+00015a00: 2020 2063 6c61 7373 3d5c 2273 6368 6564     class=\"sched
+00015a10: 756c 652d 6865 6164 6572 5c22 3e5c 725c  ule-header\">\r\
+00015a20: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00015a30: 2020 2020 203c 7370 616e 3e50 616c 7665       <span>Palve
+00015a40: 6c75 3c2f 7370 616e 3e3c 7370 616e 3e56  lu</span><span>V
+00015a50: 6969 6b6b 6f3c 2f73 7061 6e3e 5c72 5c6e  iikko</span>\r\n
+00015a60: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
+00015a70: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
+00015a80: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00015a90: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
+00015aa0: 7363 726f 6c6c 2d66 7261 6d65 5c22 3e5c  scroll-frame\">\
+00015ab0: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00015ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ad0: 3c74 6162 6c65 2064 6174 612d 726f 6c65  <table data-role
+00015ae0: 3d5c 2273 6368 6564 756c 655c 223e 5c72  =\"schedule\">\r
+00015af0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00015b00: 2020 2020 2020 2020 2020 3c74 626f 6479            <tbody
+00015b10: 3e5c 725c 6e0a 2020 2020 2020 2020 5c20  >\r\n.        \ 
+00015b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b30: 2020 2020 2020 3c2f 7462 6f64 793e 5c72        </tbody>\r
+00015b40: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00015b50: 2020 2020 2020 2020 2020 3c74 666f 6f74            <tfoot
+00015b60: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+00015b70: 2020 2020 2020 2020 2020 2020 203c 2f74               </t
+00015b80: 666f 6f74 3e5c 725c 6e0a 2020 2020 2020  foot>\r\n.      
+00015b90: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+00015ba0: 2020 2020 2020 3c2f 7461 626c 653e 5c72        </table>\r
+00015bb0: 5c6e 5c72 5c6e 2020 2020 2020 2020 2020  \n\r\n          
+00015bc0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00015bd0: 6c61 7373 3d5c 2273 6372 6f6c 6c62 6172  lass=\"scrollbar
+00015be0: 0a20 2020 2020 2020 2073 7469 636b 795c  .        sticky\
+00015bf0: 2220 6461 7461 2d72 6f6c 653d 5c22 7363  " data-role=\"sc
+00015c00: 726f 6c6c 6261 725c 223e 5c72 5c6e 2020  rollbar\">\r\n  
+00015c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c20: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00015c30: 3d5c 2268 616e 646c 655c 220a 2020 2020  =\"handle\".    
+00015c40: 2020 2020 6461 7461 2d72 6f6c 653d 5c22      data-role=\"
+00015c50: 7363 726f 6c6c 6261 722d 6861 6e64 6c65  scrollbar-handle
+00015c60: 5c22 3e3c 2f64 6976 3e5c 725c 6e20 2020  \"></div>\r\n   
+00015c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c80: 203c 2f64 6976 3e5c 725c 6e5c 725c 6e0a   </div>\r\n\r\n.
+00015c90: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
+00015ca0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00015cb0: 2063 6c61 7373 3d5c 2273 7469 636b 7920   class=\"sticky 
+00015cc0: 7368 6164 6f77 2d6c 6566 745c 223e 3c2f  shadow-left\"></
+00015cd0: 6469 763e 5c72 5c6e 2020 2020 2020 2020  div>\r\n        
+00015ce0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00015cf0: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+00015d00: 2273 7469 636b 7920 7368 6164 6f77 2d72  "sticky shadow-r
+00015d10: 6967 6874 5c22 3e3c 2f64 6976 3e5c 725c  ight\"></div>\r\
+00015d20: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00015d30: 203c 2f64 6976 3e5c 725c 6e5c 725c 6e20   </div>\r\n\r\n 
+00015d40: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00015d50: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
+00015d60: 733d 5c22 6564 6974 2d6d 656e 755c 2220  s=\"edit-menu\" 
+00015d70: 6461 7461 2d72 6f6c 653d 5c22 6564 6974  data-role=\"edit
+00015d80: 2d6d 656e 755c 2220 7374 796c 653d 5c22  -menu\" style=\"
+00015d90: 6469 7370 6c61 793a 6e6f 6e65 5c22 3e5c  display:none\">\
+00015da0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
+00015db0: 2020 2020 2020 203c 6275 7474 6f6e 0a20         <button. 
+00015dc0: 2020 2020 2020 2063 6c61 7373 3d5c 2262         class=\"b
+00015dd0: 746e 2d64 6973 6d69 7373 5c22 2064 6174  tn-dismiss\" dat
+00015de0: 612d 6163 7469 6f6e 3d5c 2263 6c6f 7365  a-action=\"close
+00015df0: 2d6d 656e 755c 223e 3c2f 6275 7474 6f6e  -menu\"></button
+00015e00: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+00015e10: 2020 2020 2020 2020 203c 6469 760a 2020           <div.  
+00015e20: 2020 2020 2020 636c 6173 733d 5c22 726f        class=\"ro
+00015e30: 775c 223e 5c72 5c6e 2020 2020 2020 2020  w\">\r\n        
+00015e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e50: 3c64 6976 2063 6c61 7373 3d5c 2263 6f6c  <div class=\"col
+00015e60: 2d73 6d2d 335c 223e 5c72 5c6e 2020 2020  -sm-3\">\r\n    
+00015e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e80: 2020 2020 2020 2020 3c62 7574 746f 6e0a          <button.
+00015e90: 2020 2020 2020 2020 6461 7461 2d61 6374          data-act
+00015ea0: 696f 6e3d 5c22 7061 7573 655c 2220 636c  ion=\"pause\" cl
+00015eb0: 6173 733d 5c22 6274 6e20 6274 6e2d 7072  ass=\"btn btn-pr
+00015ec0: 696d 6172 7920 6274 6e2d 626c 6f63 6b5c  imary btn-block\
+00015ed0: 223e 4b65 736b 6579 745c 7845 343c 2f62  ">Keskeyt\xE4</b
+00015ee0: 7574 746f 6e3e 5c72 5c6e 0a20 2020 2020  utton>\r\n.     
+00015ef0: 2020 205c 2020 2020 2020 2020 2020 2020     \            
+00015f00: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00015f10: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+00015f20: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00015f30: 7620 636c 6173 733d 5c22 636f 6c2d 736d  v class=\"col-sm
+00015f40: 2d33 5c22 3e5c 725c 6e0a 2020 2020 2020  -3\">\r\n.      
+00015f50: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
+00015f60: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
+00015f70: 7574 746f 6e20 6461 7461 2d61 6374 696f  utton data-actio
+00015f80: 6e3d 5c22 7374 6f70 5c22 2063 6c61 7373  n=\"stop\" class
+00015f90: 3d5c 2262 746e 2062 746e 2d70 7269 6d61  =\"btn btn-prima
+00015fa0: 7279 0a20 2020 2020 2020 2062 746e 2d62  ry.        btn-b
+00015fb0: 6c6f 636b 5c22 3e4c 6f70 6574 613c 2f62  lock\">Lopeta</b
+00015fc0: 7574 746f 6e3e 5c72 5c6e 2020 2020 2020  utton>\r\n      
+00015fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015fe0: 2020 3c2f 6469 763e 5c72 5c6e 2020 2020    </div>\r\n    
+00015ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016000: 2020 2020 3c64 6976 0a20 2020 2020 2020      <div.       
+00016010: 2063 6c61 7373 3d5c 2263 6f6c 2d73 6d2d   class=\"col-sm-
+00016020: 335c 223e 5c72 5c6e 2020 2020 2020 2020  3\">\r\n        
+00016030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016040: 2020 2020 3c62 7574 746f 6e20 6461 7461      <button data
+00016050: 2d61 6374 696f 6e3d 5c22 6f74 6865 725c  -action=\"other\
+00016060: 220a 2020 2020 2020 2020 636c 6173 733d  ".        class=
+00016070: 5c22 6274 6e20 6274 6e2d 7072 696d 6172  \"btn btn-primar
+00016080: 7920 6274 6e2d 626c 6f63 6b5c 223e 4d75  y btn-block\">Mu
+00016090: 7520 6d75 7574 6f73 3c2f 6275 7474 6f6e  u muutos</button
+000160a0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
+000160b0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+000160c0: 6976 3e5c 725c 6e0a 2020 2020 2020 2020  iv>\r\n.        
+000160d0: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
+000160e0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000160f0: 7373 3d5c 2263 6f6c 2d73 6d2d 335c 223e  ss=\"col-sm-3\">
+00016100: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00016110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016120: 3c62 7574 746f 6e0a 2020 2020 2020 2020  <button.        
+00016130: 6461 7461 2d61 6374 696f 6e3d 5c22 6b69  data-action=\"ki
+00016140: 6d70 7061 5c22 2063 6c61 7373 3d5c 2262  mppa\" class=\"b
+00016150: 746e 2062 746e 2d70 7269 6d61 7279 2062  tn btn-primary b
+00016160: 746e 2d62 6c6f 636b 5c22 3e50 6572 7573  tn-block\">Perus
+00016170: 7461 206b 696d 7070 613c 2f62 7574 746f  ta kimppa</butto
+00016180: 6e3e 5c72 5c6e 0a20 2020 2020 2020 205c  n>\r\n.        \
+00016190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161a0: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
+000161b0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+000161c0: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
+000161d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000161e0: 2f64 6976 3e5c 725c 6e0a 2020 2020 2020  /div>\r\n.      
+000161f0: 2020 5c20 2020 2020 2020 2020 2020 3c2f    \           </
+00016200: 6469 763e 5c72 5c6e 5c72 5c6e 2020 2020  div>\r\n\r\n    
+00016210: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00016220: 7373 3d5c 226d 6f64 616c 2d66 6f6f 7465  ss=\"modal-foote
+00016230: 725c 223e 5c72 5c6e 2020 2020 2020 2020  r\">\r\n        
+00016240: 2020 2020 2020 2020 3c64 6976 0a20 2020          <div.   
+00016250: 2020 2020 2063 6c61 7373 3d5c 2266 6f72       class=\"for
+00016260: 6d2d 6275 7474 6f6e 7320 7465 7874 2d63  m-buttons text-c
+00016270: 656e 7465 725c 223e 5c72 5c6e 2020 2020  enter\">\r\n    
 00016280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016290: 2020 2020 5c72 5c6e 5c72 5c6e 2020 2020      \r\n\r\n    
-000162a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162b0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-000162c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162d0: 203c 6469 7620 636c 6173 733d 5c22 6131   <div class=\"a1
-000162e0: 5c22 3e3c 2f64 6976 3e5c 725c 6e20 2020  \"></div>\r\n   
-000162f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016300: 203c 6469 7620 636c 6173 733d 5c22 6132   <div class=\"a2
-00016310: 5c22 3e3c 2f64 6976 3e5c 725c 6e0a 2020  \"></div>\r\n.  
-00016320: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-00016330: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00016340: 6c61 7373 3d5c 2261 335c 223e 3c2f 6469  lass=\"a3\"></di
-00016350: 763e 5c72 5c6e 2020 2020 2020 2020 2020  v>\r\n          
-00016360: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00016370: 6c61 7373 3d5c 2261 345c 223e 3c2f 6469  lass=\"a4\"></di
-00016380: 763e 5c72 5c6e 0a20 2020 2020 2020 205c  v>\r\n.        \
-00016390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163a0: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
-000163b0: 6135 5c22 3e3c 2f64 6976 3e5c 725c 6e5c  a5\"></div>\r\n\
-000163c0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-000163d0: 2020 2020 2020 203c 6469 760a 2020 2020         <div.    
-000163e0: 2020 2020 636c 6173 733d 5c22 6136 5c22      class=\"a6\"
-000163f0: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-00016400: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00016410: 7620 636c 6173 733d 5c22 6d61 702d 696e  v class=\"map-in
-00016420: 666f 5c22 3e5c 725c 6e20 2020 2020 2020  fo\">\r\n       
-00016430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016440: 2020 2020 203c 6469 763e 4b61 7274 7461       <div>Kartta
-00016450: 610a 2020 2020 2020 2020 766f 6920 7369  a.        voi si
-00016460: 6972 745c 7845 345c 7845 3420 6869 6972  irt\xE4\xE4 hiir
-00016470: 656c 6c5c 7845 3420 7261 6168 6161 6d61  ell\xE4 raahaama
-00016480: 6c6c 612e 204b 6c69 6b6b 6161 2050 6169  lla. Klikkaa Pai
-00016490: 6b6b 6120 2d70 6169 6e69 6b65 7474 6120  kka -painiketta 
-000164a0: 6a61 2076 6965 0a20 2020 2020 2020 2068  ja vie.        h
-000164b0: 6969 7269 206b 6172 7461 6c6c 6120 6b6f  iiri kartalla ko
-000164c0: 6874 6161 6e2c 206a 6f73 7361 206b 6169  htaan, jossa kai
-000164d0: 766f 206f 6e2e 204f 686a 656c 6d61 2076  vo on. Ohjelma v
-000164e0: 6172 6d69 7374 6161 2076 6965 6c5c 7845  armistaa viel\xE
-000164f0: 3420 7661 6c69 6e6e 616e 0a20 2020 2020  4 valinnan.     
-00016500: 2020 206f 696b 6561 6b73 6920 3c2f 6469     oikeaksi </di
-00016510: 763e 5c72 5c6e 2020 2020 2020 2020 2020  v>\r\n          
-00016520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016530: 2020 3c62 7574 746f 6e20 6461 7461 2d61    <button data-a
-00016540: 6374 696f 6e3d 5c22 6d61 726b 2d77 656c  ction=\"mark-wel
-00016550: 6c5c 223e 5061 696b 6b61 3c2f 6275 7474  l\">Paikka</butt
-00016560: 6f6e 3e5c 725c 6e0a 2020 2020 2020 2020  on>\r\n.        
-00016570: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-00016580: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-00016590: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-000165a0: 2020 2020 2020 2020 2020 3c64 6976 2064            <div d
-000165b0: 6174 612d 726f 6c65 3d5c 226b 6172 7474  ata-role=\"kartt
-000165c0: 615c 220a 2020 2020 2020 2020 636c 6173  a\".        clas
-000165d0: 733d 5c22 6d61 705c 223e 3c2f 6469 763e  s=\"map\"></div>
-000165e0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-000165f0: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-00016600: 5c6e 5c72 5c6e 2020 2020 2020 2020 2020  \n\r\n          
-00016610: 2020 2020 2020 2020 2020 3c64 6976 0a20            <div. 
-00016620: 2020 2020 2020 2063 6c61 7373 3d5c 2267         class=\"g
-00016630: 6c6f 6261 6c2d 7661 6c69 6461 7469 6f6e  lobal-validation
-00016640: 2d65 7272 6f72 2061 6c65 7274 2061 6c65  -error alert ale
-00016650: 7274 2d64 616e 6765 725c 2220 7374 796c  rt-danger\" styl
-00016660: 653d 5c22 6469 7370 6c61 793a 6e6f 6e65  e=\"display:none
-00016670: 5c22 3e54 5c78 4534 7974 5c78 4534 0a20  \">T\xE4yt\xE4. 
-00016680: 2020 2020 2020 2070 7575 7474 7576 6174         puuttuvat
-00016690: 206b 656e 745c 7845 3474 3c2f 6469 763e   kent\xE4t</div>
-000166a0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-000166b0: 2020 2020 3c2f 6469 763e 5c72 5c6e 2020      </div>\r\n  
-000166c0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-000166d0: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-000166e0: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
-000166f0: 2020 203c 2f64 6976 3e5c 725c 6e3c 2f64     </div>\r\n</d
-00016700: 6976 3e5c 725c 6e5c 725c 6e5c 725c 6e5c  iv>\r\n\r\n\r\n\
-00016710: 725c 6e5c 725c 6e5c 725c 6e5c 725c 6e5c  r\n\r\n\r\n\r\n\
-00016720: 725c 6e3c 6469 760a 2020 2020 2020 2020  r\n<div.        
-00016730: 6964 3d5c 2263 6f6c 6c65 6374 696f 6e2d  id=\"collection-
-00016740: 7363 6865 6475 6c65 2d6d 6f64 616c 5c22  schedule-modal\"
-00016750: 2063 6c61 7373 3d5c 226d 6f64 616c 5c22   class=\"modal\"
-00016760: 2073 7479 6c65 3d5c 2264 6973 706c 6179   style=\"display
-00016770: 3a6e 6f6e 655c 223e 5c72 5c6e 0a20 2020  :none\">\r\n.   
-00016780: 2020 2020 205c 2020 203c 6469 7620 636c       \   <div cl
-00016790: 6173 733d 5c22 6d6f 6461 6c2d 6469 616c  ass=\"modal-dial
-000167a0: 6f67 5c22 3e5c 725c 6e20 2020 2020 2020  og\">\r\n       
-000167b0: 203c 6469 7620 636c 6173 733d 5c22 6d6f   <div class=\"mo
-000167c0: 6461 6c2d 636f 6e74 656e 745c 223e 5c72  dal-content\">\r
-000167d0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-000167e0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000167f0: 733d 5c22 6d6f 6461 6c2d 626f 6479 5c22  s=\"modal-body\"
-00016800: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-00016810: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00016820: 5c22 726f 775c 223e 5c72 5c6e 0a20 2020  \"row\">\r\n.   
-00016830: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-00016840: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00016850: 6173 733d 5c22 7061 6765 2d68 6561 6465  ass=\"page-heade
-00016860: 725c 223e 5c72 5c6e 2020 2020 2020 2020  r\">\r\n        
-00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016880: 3c68 313e 4a5c 7845 3474 6561 7374 6961  <h1>J\xE4teastia
-00016890: 6e0a 2020 2020 2020 2020 7479 686a 656e  n.        tyhjen
-000168a0: 6e79 7372 7974 6d69 3c2f 6831 3e5c 725c  nysrytmi</h1>\r\
-000168b0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-000168c0: 2020 2020 203c 2f64 6976 3e5c 725c 6e20       </div>\r\n 
-000168d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000168e0: 2f64 6976 3e5c 725c 6e5c 725c 6e0a 2020  /div>\r\n\r\n.  
-000168f0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-00016900: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00016910: 3d5c 2272 6f77 2063 7573 746f 6d65 722d  =\"row customer-
-00016920: 6461 7461 2d69 6e66 6f5c 223e 5c72 5c6e  data-info\">\r\n
-00016930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016940: 2020 2020 3c64 6976 0a20 2020 2020 2020      <div.       
-00016950: 2063 6c61 7373 3d5c 2270 6167 652d 6865   class=\"page-he
-00016960: 6164 6572 5c22 3e5c 725c 6e20 2020 2020  ader\">\r\n     
-00016970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016980: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
-00016990: 636f 6c2d 736d 2d36 5c22 3e5c 725c 6e0a  col-sm-6\">\r\n.
-000169a0: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-000169b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169c0: 2020 2020 3c68 343e 5479 686a 656e 6e79      <h4>Tyhjenny
-000169d0: 736f 736f 6974 653c 2f68 343e 5c72 5c6e  sosoite</h4>\r\n
-000169e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169f0: 2020 2020 2020 2020 2020 2020 3c61 6464              <add
-00016a00: 7265 7373 3e5c 725c 6e0a 2020 2020 2020  ress>\r\n.      
-00016a10: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-00016a20: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00016a30: 7061 6e20 6461 7461 2d72 6f6c 653d 5c22  pan data-role=\"
-00016a40: 6c6f 6361 7469 6f6e 2d6e 616d 655c 223e  location-name\">
-00016a50: 3c2f 7370 616e 3e3c 6272 3e3c 6272 3e5c  </span><br><br>\
-00016a60: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
-00016a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a80: 2020 2020 2020 2020 3c73 7061 6e20 6461          <span da
-00016a90: 7461 2d72 6f6c 653d 5c22 6c6f 6361 7469  ta-role=\"locati
-00016aa0: 6f6e 2d61 6464 7265 7373 5c22 3e3c 2f73  on-address\"></s
-00016ab0: 7061 6e3e 3c62 723e 5c72 5c6e 0a20 2020  pan><br>\r\n.   
-00016ac0: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-00016ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ae0: 203c 7370 616e 2064 6174 612d 726f 6c65   <span data-role
-00016af0: 3d5c 226c 6f63 6174 696f 6e2d 706f 7374  =\"location-post
-00016b00: 5c22 3e3c 2f73 7061 6e3e 5c72 5c6e 0a20  \"></span>\r\n. 
-00016b10: 2020 2020 2020 205c 2020 2020 2020 2020         \        
-00016b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b30: 2020 203c 2f61 6464 7265 7373 3e5c 725c     </address>\r\
-00016b40: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00016b50: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-00016b60: 725c 6e5c 725c 6e0a 2020 2020 2020 2020  r\n\r\n.        
-00016b70: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-00016b80: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00016b90: 7373 3d5c 2263 6f6c 2d73 6d2d 365c 223e  ss=\"col-sm-6\">
-00016ba0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-00016bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bc0: 3c68 343e 4c61 736b 7574 7573 6f73 6f69  <h4>Laskutusosoi
-00016bd0: 7465 3c2f 6834 3e5c 725c 6e0a 2020 2020  te</h4>\r\n.    
-00016be0: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-00016bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c00: 3c61 6464 7265 7373 3e5c 725c 6e20 2020  <address>\r\n   
-00016c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c20: 2020 2020 2020 2020 2020 2020 203c 7370               <sp
-00016c30: 616e 0a20 2020 2020 2020 2064 6174 612d  an.        data-
-00016c40: 726f 6c65 3d5c 2269 6e76 6f69 6369 6e67  role=\"invoicing
-00016c50: 2d6e 616d 655c 223e 3c2f 7370 616e 3e3c  -name\"></span><
-00016c60: 6272 3e3c 6272 3e5c 725c 6e20 2020 2020  br><br>\r\n     
-00016c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c80: 2020 2020 2020 2020 2020 203c 7370 616e             <span
-00016c90: 0a20 2020 2020 2020 2064 6174 612d 726f  .        data-ro
-00016ca0: 6c65 3d5c 2269 6e76 6f69 6369 6e67 2d61  le=\"invoicing-a
-00016cb0: 6464 7265 7373 5c22 3e3c 2f73 7061 6e3e  ddress\"></span>
-00016cc0: 3c62 723e 5c72 5c6e 2020 2020 2020 2020  <br>\r\n        
-00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ce0: 2020 2020 2020 2020 3c73 7061 6e0a 2020          <span.  
-00016cf0: 2020 2020 2020 6461 7461 2d72 6f6c 653d        data-role=
-00016d00: 5c22 696e 766f 6963 696e 672d 706f 7374  \"invoicing-post
-00016d10: 5c22 3e3c 2f73 7061 6e3e 5c72 5c6e 2020  \"></span>\r\n  
-00016d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d30: 2020 2020 2020 2020 2020 3c2f 6164 6472            </addr
-00016d40: 6573 733e 5c72 5c6e 0a20 2020 2020 2020  ess>\r\n.       
-00016d50: 205c 2020 2020 2020 2020 2020 2020 2020   \              
-00016d60: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-00016d70: 725c 6e5c 725c 6e20 2020 2020 2020 2020  r\n\r\n         
-00016d80: 2020 2020 2020 2020 2020 2020 2020 205c                 \
-00016d90: 725c 6e5c 725c 6e20 2020 2020 2020 2020  r\n\r\n         
-00016da0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00016db0: 6469 760a 2020 2020 2020 2020 7374 796c  div.        styl
-00016dc0: 653d 5c22 636c 6561 723a 626f 7468 5c22  e=\"clear:both\"
-00016dd0: 3e3c 2f64 6976 3e5c 725c 6e20 2020 2020  ></div>\r\n     
-00016de0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00016df0: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
-00016e00: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-00016e10: 725c 6e5c 725c 6e0a 2020 2020 2020 2020  r\n\r\n.        
-00016e20: 5c20 2020 2020 2020 2020 2020 2020 2020  \               
-00016e30: 3c64 6976 2063 6c61 7373 3d5c 2273 6d61  <div class=\"sma
-00016e40: 6c6c 5c22 3e41 6a6f 705c 7845 3469 765c  ll\">Ajop\xE4iv\
-00016e50: 7845 3420 766f 6920 6d75 7574 7475 6120  xE4 voi muuttua 
-00016e60: 285c 7842 3120 312d 320a 2020 2020 2020  (\xB1 1-2.      
-00016e70: 2020 705c 7845 3469 765c 7845 345c 7845    p\xE4iv\xE4\xE
-00016e80: 3429 2065 7369 6d2e 2061 726b 6970 7968  4) esim. arkipyh
-00016e90: 5c78 4534 7669 696b 6f69 6c6c 612e 3c2f  \xE4viikoilla.</
-00016ea0: 6469 763e 5c72 5c6e 5c72 5c6e 2020 2020  div>\r\n\r\n    
-00016eb0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00016ec0: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
-00016ed0: 2273 6368 6564 756c 652d 6865 6164 6572  "schedule-header
-00016ee0: 5c22 3e5c 725c 6e20 2020 2020 2020 2020  \">\r\n         
-00016ef0: 2020 2020 2020 2020 2020 203c 7370 616e             <span
-00016f00: 3e50 616c 7665 6c75 3c2f 7370 616e 3e3c  >Palvelu</span><
-00016f10: 7370 616e 3e56 6969 6b6b 6f3c 2f73 7061  span>Viikko</spa
-00016f20: 6e3e 5c72 5c6e 0a20 2020 2020 2020 205c  n>\r\n.        \
-00016f30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00016f40: 2f64 6976 3e5c 725c 6e20 2020 2020 2020  /div>\r\n       
-00016f50: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00016f60: 6173 733d 5c22 7363 726f 6c6c 2d66 7261  ass=\"scroll-fra
-00016f70: 6d65 5c22 3e5c 725c 6e0a 2020 2020 2020  me\">\r\n.      
-00016f80: 2020 5c20 2020 2020 2020 2020 2020 2020    \             
-00016f90: 2020 2020 2020 3c74 6162 6c65 2064 6174        <table dat
-00016fa0: 612d 726f 6c65 3d5c 2273 6368 6564 756c  a-role=\"schedul
-00016fb0: 655c 223e 5c72 5c6e 2020 2020 2020 2020  e\">\r\n        
-00016fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fd0: 3c74 626f 6479 3e5c 725c 6e0a 2020 2020  <tbody>\r\n.    
-00016fe0: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-00016ff0: 2020 2020 2020 2020 2020 2020 3c2f 7462              </tb
-00017000: 6f64 793e 5c72 5c6e 2020 2020 2020 2020  ody>\r\n        
-00017010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017020: 3c74 666f 6f74 3e5c 725c 6e20 2020 2020  <tfoot>\r\n     
-00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017040: 2020 203c 2f74 666f 6f74 3e5c 725c 6e0a     </tfoot>\r\n.
-00017050: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-00017060: 2020 2020 2020 2020 2020 2020 3c2f 7461              </ta
-00017070: 626c 653e 5c72 5c6e 5c72 5c6e 2020 2020  ble>\r\n\r\n    
-00017080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017090: 3c64 6976 2063 6c61 7373 3d5c 2273 6372  <div class=\"scr
-000170a0: 6f6c 6c62 6172 0a20 2020 2020 2020 2073  ollbar.        s
-000170b0: 7469 636b 795c 2220 6461 7461 2d72 6f6c  ticky\" data-rol
-000170c0: 653d 5c22 7363 726f 6c6c 6261 725c 223e  e=\"scrollbar\">
-000170d0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-000170e0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-000170f0: 2063 6c61 7373 3d5c 2268 616e 646c 655c   class=\"handle\
-00017100: 220a 2020 2020 2020 2020 6461 7461 2d72  ".        data-r
-00017110: 6f6c 653d 5c22 7363 726f 6c6c 6261 722d  ole=\"scrollbar-
-00017120: 6861 6e64 6c65 5c22 3e3c 2f64 6976 3e5c  handle\"></div>\
-00017130: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-00017140: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
-00017150: 6e5c 725c 6e0a 2020 2020 2020 2020 5c20  n\r\n.        \ 
-00017160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017170: 2020 3c64 6976 2063 6c61 7373 3d5c 2273    <div class=\"s
-00017180: 7469 636b 7920 7368 6164 6f77 2d6c 6566  ticky shadow-lef
-00017190: 745c 223e 3c2f 6469 763e 5c72 5c6e 2020  t\"></div>\r\n  
-000171a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171b0: 2020 3c64 6976 0a20 2020 2020 2020 2063    <div.        c
-000171c0: 6c61 7373 3d5c 2273 7469 636b 7920 7368  lass=\"sticky sh
-000171d0: 6164 6f77 2d72 6967 6874 5c22 3e3c 2f64  adow-right\"></d
-000171e0: 6976 3e5c 725c 6e20 2020 2020 2020 2020  iv>\r\n         
-000171f0: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
-00017200: 6e5c 725c 6e20 2020 2020 2020 2020 2020  n\r\n           
-00017210: 2020 2020 203c 6469 760a 2020 2020 2020       <div.      
-00017220: 2020 636c 6173 733d 5c22 6564 6974 2d6d    class=\"edit-m
-00017230: 656e 755c 2220 6461 7461 2d72 6f6c 653d  enu\" data-role=
-00017240: 5c22 6564 6974 2d6d 656e 755c 2220 7374  \"edit-menu\" st
-00017250: 796c 653d 5c22 6469 7370 6c61 793a 6e6f  yle=\"display:no
-00017260: 6e65 5c22 3e5c 725c 6e20 2020 2020 2020  ne\">\r\n       
-00017270: 2020 2020 2020 2020 2020 2020 203c 6275               <bu
-00017280: 7474 6f6e 0a20 2020 2020 2020 2063 6c61  tton.        cla
-00017290: 7373 3d5c 2262 746e 2d64 6973 6d69 7373  ss=\"btn-dismiss
-000172a0: 5c22 2064 6174 612d 6163 7469 6f6e 3d5c  \" data-action=\
-000172b0: 2263 6c6f 7365 2d6d 656e 755c 223e 3c2f  "close-menu\"></
-000172c0: 6275 7474 6f6e 3e5c 725c 6e20 2020 2020  button>\r\n     
-000172d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000172e0: 6469 760a 2020 2020 2020 2020 636c 6173  div.        clas
-000172f0: 733d 5c22 726f 775c 223e 5c72 5c6e 2020  s=\"row\">\r\n  
-00017300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017310: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00017320: 3d5c 2263 6f6c 2d73 6d2d 335c 223e 5c72  =\"col-sm-3\">\r
-00017330: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00017340: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
-00017350: 7574 746f 6e0a 2020 2020 2020 2020 6461  utton.        da
-00017360: 7461 2d61 6374 696f 6e3d 5c22 7061 7573  ta-action=\"paus
-00017370: 655c 2220 636c 6173 733d 5c22 6274 6e20  e\" class=\"btn 
-00017380: 6274 6e2d 7072 696d 6172 7920 6274 6e2d  btn-primary btn-
-00017390: 626c 6f63 6b5c 223e 4b65 736b 6579 745c  block\">Keskeyt\
-000173a0: 7845 343c 2f62 7574 746f 6e3e 5c72 5c6e  xE4</button>\r\n
-000173b0: 0a20 2020 2020 2020 205c 2020 2020 2020  .        \      
-000173c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173d0: 203c 2f64 6976 3e5c 725c 6e20 2020 2020   </div>\r\n     
-000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173f0: 2020 203c 6469 7620 636c 6173 733d 5c22     <div class=\"
-00017400: 636f 6c2d 736d 2d33 5c22 3e5c 725c 6e0a  col-sm-3\">\r\n.
-00017410: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-00017420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017430: 2020 2020 3c62 7574 746f 6e20 6461 7461      <button data
-00017440: 2d61 6374 696f 6e3d 5c22 7374 6f70 5c22  -action=\"stop\"
-00017450: 2063 6c61 7373 3d5c 2262 746e 2062 746e   class=\"btn btn
-00017460: 2d70 7269 6d61 7279 0a20 2020 2020 2020  -primary.       
-00017470: 2062 746e 2d62 6c6f 636b 5c22 3e4c 6f70   btn-block\">Lop
-00017480: 6574 613c 2f62 7574 746f 6e3e 5c72 5c6e  eta</button>\r\n
-00017490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174a0: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-000174b0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-000174c0: 2020 2020 2020 2020 2020 3c64 6976 0a20            <div. 
-000174d0: 2020 2020 2020 2063 6c61 7373 3d5c 2263         class=\"c
-000174e0: 6f6c 2d73 6d2d 335c 223e 5c72 5c6e 2020  ol-sm-3\">\r\n  
-000174f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017500: 2020 2020 2020 2020 2020 3c62 7574 746f            <butto
-00017510: 6e20 6461 7461 2d61 6374 696f 6e3d 5c22  n data-action=\"
-00017520: 6f74 6865 725c 220a 2020 2020 2020 2020  other\".        
-00017530: 636c 6173 733d 5c22 6274 6e20 6274 6e2d  class=\"btn btn-
-00017540: 7072 696d 6172 7920 6274 6e2d 626c 6f63  primary btn-bloc
-00017550: 6b5c 223e 4d75 7520 6d75 7574 6f73 3c2f  k\">Muu muutos</
-00017560: 6275 7474 6f6e 3e5c 725c 6e20 2020 2020  button>\r\n     
-00017570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017580: 2020 203c 2f64 6976 3e5c 725c 6e0a 2020     </div>\r\n.  
-00017590: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-000175a0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000175b0: 6976 2063 6c61 7373 3d5c 2263 6f6c 2d73  iv class=\"col-s
-000175c0: 6d2d 335c 223e 5c72 5c6e 2020 2020 2020  m-3\">\r\n      
-000175d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175e0: 2020 2020 2020 3c62 7574 746f 6e0a 2020        <button.  
-000175f0: 2020 2020 2020 6461 7461 2d61 6374 696f        data-actio
-00017600: 6e3d 5c22 6b69 6d70 7061 5c22 2063 6c61  n=\"kimppa\" cla
-00017610: 7373 3d5c 2262 746e 2062 746e 2d70 7269  ss=\"btn btn-pri
-00017620: 6d61 7279 2062 746e 2d62 6c6f 636b 5c22  mary btn-block\"
-00017630: 3e50 6572 7573 7461 206b 696d 7070 613c  >Perusta kimppa<
-00017640: 2f62 7574 746f 6e3e 5c72 5c6e 0a20 2020  /button>\r\n.   
-00017650: 2020 2020 205c 2020 2020 2020 2020 2020       \          
-00017660: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00017670: 6976 3e5c 725c 6e20 2020 2020 2020 2020  iv>\r\n         
-00017680: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00017690: 3e5c 725c 6e20 2020 2020 2020 2020 2020  >\r\n           
-000176a0: 2020 2020 203c 2f64 6976 3e5c 725c 6e0a       </div>\r\n.
-000176b0: 2020 2020 2020 2020 5c20 2020 2020 2020          \       
-000176c0: 2020 2020 3c2f 6469 763e 5c72 5c6e 5c72      </div>\r\n\r
-000176d0: 5c6e 2020 2020 2020 2020 2020 2020 3c64  \n            <d
-000176e0: 6976 2063 6c61 7373 3d5c 226d 6f64 616c  iv class=\"modal
-000176f0: 2d66 6f6f 7465 725c 223e 5c72 5c6e 2020  -footer\">\r\n  
-00017700: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00017710: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
-00017720: 3d5c 2266 6f72 6d2d 6275 7474 6f6e 7320  =\"form-buttons 
-00017730: 7465 7874 2d63 656e 7465 725c 223e 5c72  text-center\">\r
-00017740: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00017750: 2020 2020 2020 3c62 7574 746f 6e20 636c        <button cl
-00017760: 6173 733d 5c22 6274 6e0a 2020 2020 2020  ass=\"btn.      
-00017770: 2020 6274 6e2d 7072 696d 6172 795c 2220    btn-primary\" 
-00017780: 6461 7461 2d61 6374 696f 6e3d 5c22 6578  data-action=\"ex
-00017790: 6974 5c22 3e50 6f69 7374 753c 2f62 7574  it\">Poistu</but
-000177a0: 746f 6e3e 5c72 5c6e 2020 2020 2020 2020  ton>\r\n        
-000177b0: 2020 2020 2020 2020 3c2f 6469 763e 5c72          </div>\r
-000177c0: 5c6e 0a20 2020 2020 2020 205c 2020 2020  \n.        \    
-000177d0: 2020 2020 2020 203c 2f64 6976 3e5c 725c         </div>\r\
-000177e0: 6e20 2020 2020 2020 203c 2f64 6976 3e5c  n        </div>\
-000177f0: 725c 6e20 2020 203c 2f64 6976 3e5c 725c  r\n    </div>\r\
-00017800: 6e3c 2f64 6976 3e5c 725c 6e5c 725c 6e5c  n</div>\r\n\r\n\
-00017810: 725c 6e5c 725c 6e3c 7363 7269 7074 0a20  r\n\r\n<script. 
-00017820: 2020 2020 2020 2069 643d 5c22 696e 766f         id=\"invo
-00017830: 6963 652d 6465 7461 696c 732d 7465 6d70  ice-details-temp
-00017840: 6c61 7465 5c22 2074 7970 653d 5c22 7465  late\" type=\"te
-00017850: 7874 2f78 2d6b 656e 646f 2d74 656d 706c  xt/x-kendo-templ
-00017860: 6174 655c 223e 5c72 5c6e 5c72 5c6e 5c72  ate\">\r\n\r\n\r
-00017870: 5c6e 3c74 643e 3c2f 7464 3e5c 725c 6e3c  \n<td></td>\r\n<
-00017880: 7464 0a20 2020 2020 2020 2063 6f6c 7370  td.        colsp
-00017890: 616e 3d5c 2238 5c22 3e5c 725c 6e5c 743c  an=\"8\">\r\n\t<
-000178a0: 6172 7469 636c 6520 636c 6173 733d 5c22  article class=\"
-000178b0: 696e 766f 6963 652d 6465 7461 696c 735c  invoice-details\
-000178c0: 223e 5c72 5c6e 5c74 5c74 3c74 6162 6c65  ">\r\n\t\t<table
-000178d0: 2063 6c61 7373 3d5c 2274 6162 6c65 5c22   class=\"table\"
-000178e0: 3e5c 725c 6e5c 745c 745c 743c 7472 3e5c  >\r\n\t\t\t<tr>\
-000178f0: 725c 6e5c 745c 745c 745c 743c 7468 3e53  r\n\t\t\t\t<th>S
-00017900: 5c78 4534 696c 695c 7846 363c 2f74 683e  \xE4ili\xF6</th>
-00017910: 5c72 5c6e 5c74 5c74 5c74 5c74 3c74 683e  \r\n\t\t\t\t<th>
-00017920: 4e6f 7574 6f61 696b 613c 2f74 683e 5c72  Noutoaika</th>\r
-00017930: 5c6e 5c74 5c74 5c74 5c74 3c74 683e 5061  \n\t\t\t\t<th>Pa
-00017940: 6c76 656c 756e 0a20 2020 2020 2020 2073  lvelun.        s
-00017950: 756f 7269 7474 616a 613c 2f74 683e 5c72  uorittaja</th>\r
-00017960: 5c6e 5c74 5c74 5c74 5c74 3c74 683e 5661  \n\t\t\t\t<th>Va
-00017970: 7374 6561 696b 613c 2f74 683e 5c72 5c6e  steaika</th>\r\n
-00017980: 5c74 5c74 5c74 3c2f 7472 3e5c 725c 6e5c  \t\t\t</tr>\r\n\
-00017990: 745c 745c 743c 7472 3e5c 725c 6e5c 745c  t\t\t<tr>\r\n\t\
-000179a0: 745c 745c 743c 7464 3e23 3a0a 2020 2020  t\t\t<td>#:.    
-000179b0: 2020 2020 7369 676e 6174 7572 652e 6269      signature.bi
-000179c0: 6e20 233c 2f74 643e 5c72 5c6e 5c74 5c74  n #</td>\r\n\t\t
-000179d0: 5c74 5c74 3c74 643e 233a 206b 656e 646f  \t\t<td>#: kendo
-000179e0: 2e74 6f53 7472 696e 6728 6b65 6e64 6f2e  .toString(kendo.
-000179f0: 7061 7273 6544 6174 6528 7369 676e 6174  parseDate(signat
-00017a00: 7572 652e 7069 636b 7570 4461 7465 292c  ure.pickupDate),
-00017a10: 0a20 2020 2020 2020 2027 6727 2920 233c  .        'g') #<
-00017a20: 2f74 643e 5c72 5c6e 5c74 5c74 5c74 5c74  /td>\r\n\t\t\t\t
-00017a30: 3c74 643e 233a 2073 6967 6e61 7475 7265  <td>#: signature
-00017a40: 2e65 7865 6375 7465 7220 3f20 7369 676e  .executer ? sign
-00017a50: 6174 7572 652e 6578 6563 7574 6572 203a  ature.executer :
-00017a60: 2027 270a 2020 2020 2020 2020 233c 2f74   ''.        #</t
-00017a70: 643e 5c72 5c6e 5c74 5c74 5c74 5c74 3c74  d>\r\n\t\t\t\t<t
-00017a80: 643e 3c2f 7464 3e5c 725c 6e5c 745c 745c  d></td>\r\n\t\t\
-00017a90: 743c 2f74 723e 5c72 5c6e 5c72 5c6e 5c74  t</tr>\r\n\r\n\t
-00017aa0: 5c74 5c74 3c74 723e 5c72 5c6e 5c74 5c74  \t\t<tr>\r\n\t\t
-00017ab0: 5c74 5c74 3c74 683e 5246 4944 3c2f 7468  \t\t<th>RFID</th
-00017ac0: 3e5c 725c 6e5c 745c 745c 745c 743c 7468  >\r\n\t\t\t\t<th
-00017ad0: 3e56 6173 7461 616e 6f74 746f 6169 6b61  >Vastaanottoaika
-00017ae0: 3c2f 7468 3e5c 725c 6e5c 745c 745c 745c  </th>\r\n\t\t\t\
-00017af0: 743c 7468 3e50 7572 6b61 6a61 3c2f 7468  t<th>Purkaja</th
-00017b00: 3e5c 725c 6e5c 745c 745c 745c 743c 7468  >\r\n\t\t\t\t<th
-00017b10: 3e3c 2f74 683e 5c72 5c6e 5c74 5c74 5c74  ></th>\r\n\t\t\t
-00017b20: 3c2f 7472 3e5c 725c 6e5c 745c 745c 743c  </tr>\r\n\t\t\t<
-00017b30: 7472 3e5c 725c 6e5c 745c 745c 745c 743c  tr>\r\n\t\t\t\t<
-00017b40: 7464 3e23 3a0a 2020 2020 2020 2020 7369  td>#:.        si
-00017b50: 676e 6174 7572 652e 7266 6964 203f 2073  gnature.rfid ? s
-00017b60: 6967 6e61 7475 7265 2e72 6669 6420 3a20  ignature.rfid : 
-00017b70: 2727 2023 3c2f 7464 3e5c 725c 6e5c 745c  '' #</td>\r\n\t\
-00017b80: 745c 745c 743c 7464 3e23 3a20 7369 676e  t\t\t<td>#: sign
-00017b90: 6174 7572 652e 7265 6365 6976 6544 6174  ature.receiveDat
-00017ba0: 650a 2020 2020 2020 2020 3f20 6b65 6e64  e.        ? kend
-00017bb0: 6f2e 746f 5374 7269 6e67 286b 656e 646f  o.toString(kendo
-00017bc0: 2e70 6172 7365 4461 7465 2873 6967 6e61  .parseDate(signa
-00017bd0: 7475 7265 2e72 6563 6569 7665 4461 7465  ture.receiveDate
-00017be0: 292c 2027 6727 2920 3a20 2727 2023 3c2f  ), 'g') : '' #</
-00017bf0: 7464 3e5c 725c 6e5c 745c 745c 745c 743c  td>\r\n\t\t\t\t<
-00017c00: 7464 3e23 3a0a 2020 2020 2020 2020 7369  td>#:.        si
-00017c10: 676e 6174 7572 652e 756e 6c6f 6164 6572  gnature.unloader
-00017c20: 203f 2073 6967 6e61 7475 7265 2e75 6e6c   ? signature.unl
-00017c30: 6f61 6465 7220 3a20 2727 2023 3c2f 7464  oader : '' #</td
-00017c40: 3e5c 725c 6e5c 745c 745c 745c 743c 7464  >\r\n\t\t\t\t<td
-00017c50: 3e23 3a20 666f 726d 6174 496e 7465 7276  >#: formatInterv
-00017c60: 616c 2873 6967 6e61 7475 7265 2e74 696d  al(signature.tim
-00017c70: 6554 6f55 6e6c 6f61 6429 0a20 2020 2020  eToUnload).     
-00017c80: 2020 2023 3c2f 7464 3e5c 725c 6e5c 745c     #</td>\r\n\t\
-00017c90: 745c 743c 2f74 723e 5c72 5c6e 5c72 5c6e  t\t</tr>\r\n\r\n
-00017ca0: 5c74 5c74 5c74 3c74 723e 5c72 5c6e 5c74  \t\t\t<tr>\r\n\t
-00017cb0: 5c74 5c74 5c74 3c74 683e 5475 686f 7573  \t\t\t<th>Tuhous
-00017cc0: 746f 6469 7374 7573 3c2f 7468 3e5c 725c  todistus</th>\r\
-00017cd0: 6e5c 745c 745c 745c 743c 7468 3e54 7568  n\t\t\t\t<th>Tuh
-00017ce0: 6f75 7361 696b 613c 2f74 683e 5c72 5c6e  ousaika</th>\r\n
-00017cf0: 5c74 5c74 5c74 5c74 3c74 683e 5661 7374  \t\t\t\t<th>Vast
-00017d00: 7575 6c6c 696e 656e 0a20 2020 2020 2020  uullinen.       
-00017d10: 2074 7568 6f61 6a61 3c2f 7468 3e5c 725c   tuhoaja</th>\r\
-00017d20: 6e5c 745c 745c 745c 743c 7468 3e3c 2f74  n\t\t\t\t<th></t
-00017d30: 683e 5c72 5c6e 5c74 5c74 5c74 3c2f 7472  h>\r\n\t\t\t</tr
-00017d40: 3e5c 725c 6e5c 745c 745c 743c 7472 3e5c  >\r\n\t\t\t<tr>\
-00017d50: 725c 6e5c 745c 745c 745c 743c 7464 3e23  r\n\t\t\t\t<td>#
-00017d60: 3a0a 2020 2020 2020 2020 7369 676e 6174  :.        signat
-00017d70: 7572 652e 7461 736b 4964 2023 3c2f 7464  ure.taskId #</td
-00017d80: 3e5c 725c 6e5c 745c 745c 745c 743c 7464  >\r\n\t\t\t\t<td
-00017d90: 3e23 3a20 7369 676e 6174 7572 652e 6465  >#: signature.de
-00017da0: 7374 726f 7944 6174 6520 3f20 6b65 6e64  stroyDate ? kend
-00017db0: 6f2e 746f 5374 7269 6e67 286b 656e 646f  o.toString(kendo
-00017dc0: 2e70 6172 7365 4461 7465 2873 6967 6e61  .parseDate(signa
-00017dd0: 7475 7265 2e64 6573 7472 6f79 4461 7465  ture.destroyDate
-00017de0: 292c 0a20 2020 2020 2020 2027 6727 2920  ),.        'g') 
-00017df0: 3a20 2727 2023 3c2f 7464 3e5c 725c 6e5c  : '' #</td>\r\n\
-00017e00: 745c 745c 745c 743c 7464 3e23 3a20 7369  t\t\t\t<td>#: si
-00017e10: 676e 6174 7572 652e 6465 7374 726f 7965  gnature.destroye
-00017e20: 7220 3f20 7369 676e 6174 7572 652e 6465  r ? signature.de
-00017e30: 7374 726f 7965 720a 2020 2020 2020 2020  stroyer.        
-00017e40: 3a20 2727 2023 3c2f 7464 3e5c 725c 6e5c  : '' #</td>\r\n\
-00017e50: 745c 745c 745c 743c 7464 3e23 3a20 666f  t\t\t\t<td>#: fo
-00017e60: 726d 6174 496e 7465 7276 616c 2873 6967  rmatInterval(sig
-00017e70: 6e61 7475 7265 2e74 696d 6554 6f44 6573  nature.timeToDes
-00017e80: 7472 6f79 2920 233c 2f74 643e 5c72 5c6e  troy) #</td>\r\n
-00017e90: 5c74 5c74 5c74 3c2f 7472 3e5c 725c 6e5c  \t\t\t</tr>\r\n\
-00017ea0: 725c 6e5c 745c 745c 743c 7472 3e5c 725c  r\n\t\t\t<tr>\r\
-00017eb0: 6e5c 745c 745c 745c 743c 7468 3e4d 6174  n\t\t\t\t<th>Mat
-00017ec0: 6572 6961 616c 693c 2f74 683e 5c72 5c6e  eriaali</th>\r\n
-00017ed0: 5c74 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \t\t\t\t\r\n\t\t
-00017ee0: 5c74 5c74 3c74 680a 2020 2020 2020 2020  \t\t<th.        
-00017ef0: 636f 6c73 7061 6e3d 5c22 335c 223e 4875  colspan=\"3\">Hu
-00017f00: 6f6d 3c2f 7468 3e5c 725c 6e5c 745c 745c  om</th>\r\n\t\t\
-00017f10: 745c 745c 725c 6e5c 745c 745c 743c 2f74  t\t\r\n\t\t\t</t
-00017f20: 723e 5c72 5c6e 5c74 5c74 5c74 3c74 723e  r>\r\n\t\t\t<tr>
-00017f30: 5c72 5c6e 5c74 5c74 5c74 5c74 3c74 643e  \r\n\t\t\t\t<td>
-00017f40: 233a 0a20 2020 2020 2020 2073 6967 6e61  #:.        signa
-00017f50: 7475 7265 2e6d 6174 6572 6961 6c20 233c  ture.material #<
-00017f60: 2f74 643e 5c72 5c6e 5c74 5c74 5c74 5c74  /td>\r\n\t\t\t\t
-00017f70: 5c72 5c6e 5c74 5c74 5c74 5c74 3c74 6420  \r\n\t\t\t\t<td 
-00017f80: 636f 6c73 7061 6e3d 5c22 335c 2220 726f  colspan=\"3\" ro
-00017f90: 7773 7061 6e3d 5c22 335c 223e 233a 0a20  wspan=\"3\">#:. 
-00017fa0: 2020 2020 2020 2073 6967 6e61 7475 7265         signature
-00017fb0: 2e63 6f6d 6d65 6e74 2023 3c2f 7464 3e5c  .comment #</td>\
-00017fc0: 725c 6e5c 745c 745c 745c 745c 725c 6e5c  r\n\t\t\t\t\r\n\
-00017fd0: 745c 745c 743c 2f74 723e 5c72 5c6e 5c72  t\t\t</tr>\r\n\r
-00017fe0: 5c6e 5c74 5c74 5c74 3c74 723e 5c72 5c6e  \n\t\t\t<tr>\r\n
-00017ff0: 5c74 5c74 5c74 5c74 3c74 683e 6b67 2f6b  \t\t\t\t<th>kg/k
-00018000: 706c 3c2f 7468 3e5c 725c 6e5c 745c 745c  pl</th>\r\n\t\t\
-00018010: 743c 2f74 723e 5c72 5c6e 5c74 5c74 5c74  t</tr>\r\n\t\t\t
-00018020: 3c74 723e 5c72 5c6e 5c74 5c74 5c74 5c74  <tr>\r\n\t\t\t\t
-00018030: 3c74 643e 233a 0a20 2020 2020 2020 2073  <td>#:.        s
-00018040: 6967 6e61 7475 7265 2e61 6d6f 756e 7420  ignature.amount 
-00018050: 3f20 7369 676e 6174 7572 652e 616d 6f75  ? signature.amou
-00018060: 6e74 203a 2027 2720 233c 2f74 643e 5c72  nt : '' #</td>\r
-00018070: 5c6e 5c74 5c74 5c74 3c2f 7472 3e5c 725c  \n\t\t\t</tr>\r\
-00018080: 6e5c 745c 743c 2f74 6162 6c65 3e5c 725c  n\t\t</table>\r\
-00018090: 6e5c 743c 2f61 7274 6963 6c65 3e5c 725c  n\t</article>\r\
-000180a0: 6e3c 2f74 643e 5c72 5c6e 3c2f 7363 7269  n</td>\r\n</scri
-000180b0: 7074 3e5c 725c 6e0a 2020 2020 2020 2020  pt>\r\n.        
-000180c0: 5c20 2020 3c2f 6469 763e 5c72 5c6e 5c72  \   </div>\r\n\r
-000180d0: 5c6e 2020 2020 3c66 6f6f 7465 723e 5c72  \n    <footer>\r
-000180e0: 5c6e 5c74 3c64 6976 3e5c 725c 6e5c 745c  \n\t<div>\r\n\t\
-000180f0: 743c 6469 7620 636c 6173 733d 5c22 636f  t<div class=\"co
-00018100: 6e74 6169 6e65 725c 223e 5c72 5c6e 5c74  ntainer\">\r\n\t
-00018110: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-00018120: 2063 6c61 7373 3d5c 2272 6f77 5c22 3e5c   class=\"row\">\
-00018130: 725c 6e5c 745c 745c 745c 743c 6469 7620  r\n\t\t\t\t<div 
-00018140: 636c 6173 733d 5c22 636f 6c2d 736d 2d34  class=\"col-sm-4
-00018150: 2063 6f6c 2d6d 642d 345c 223e 5c72 5c6e   col-md-4\">\r\n
-00018160: 5c74 5c74 5c74 5c74 5c74 3c61 6464 7265  \t\t\t\t\t<addre
-00018170: 7373 3e5c 725c 6e5c 745c 745c 745c 745c  ss>\r\n\t\t\t\t\
-00018180: 745c 744a 5c78 4534 7465 6b75 6b6b 6f0a  t\tJ\xE4tekukko.
-00018190: 2020 2020 2020 2020 4f79 3c62 723e 5c72          Oy<br>\r
-000181a0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 5c72  \n\t\t\t\t\t\t\r
-000181b0: 5c6e 5c74 5c74 5c74 5c74 5c74 3c2f 6164  \n\t\t\t\t\t</ad
-000181c0: 6472 6573 733e 5c72 5c6e 5c74 5c74 5c74  dress>\r\n\t\t\t
-000181d0: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 5c74  \t</div>\r\n\t\t
-000181e0: 5c74 5c74 3c64 6976 0a20 2020 2020 2020  \t\t<div.       
-000181f0: 2063 6c61 7373 3d5c 2263 6f6c 2d73 6d2d   class=\"col-sm-
-00018200: 3420 636f 6c2d 6d64 2d34 5c22 3e5c 725c  4 col-md-4\">\r\
-00018210: 6e5c 745c 745c 745c 745c 7441 7369 616b  n\t\t\t\t\tAsiak
-00018220: 6173 7061 6c76 656c 7520 5c75 3230 3232  aspalvelu \u2022
-00018230: 2030 3137 2033 3638 3020 3135 320a 2020   017 3680 152.  
-00018240: 2020 2020 2020 5c75 3230 3232 2061 7369        \u2022 asi
-00018250: 616b 6173 7061 6c76 656c 7540 6a61 7465  akaspalvelu@jate
-00018260: 6b75 6b6b 6f2e 6669 5c72 5c6e 5c74 5c74  kukko.fi\r\n\t\t
-00018270: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-00018280: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
-00018290: 3d5c 2263 6f6c 2d73 6d2d 330a 2020 2020  =\"col-sm-3.    
-000182a0: 2020 2020 636f 6c2d 6d64 2d33 5c22 3e5c      col-md-3\">\
-000182b0: 725c 6e5c 745c 745c 745c 745c 745c 725c  r\n\t\t\t\t\t\r\
-000182c0: 6e5c 745c 745c 745c 745c 745c 745c 725c  n\t\t\t\t\t\t\r\
-000182d0: 6e5c 745c 745c 745c 745c 745c 745c 725c  n\t\t\t\t\t\t\r\
-000182e0: 6e5c 745c 745c 745c 745c 745c 745c 725c  n\t\t\t\t\t\t\r\
-000182f0: 6e5c 745c 745c 745c 745c 745c 725c 6e5c  n\t\t\t\t\t\r\n\
-00018300: 745c 745c 745c 745c 745c 725c 6e5c 745c  t\t\t\t\t\r\n\t\
-00018310: 745c 745c 745c 745c 745c 725c 6e5c 745c  t\t\t\t\t\r\n\t\
-00018320: 745c 745c 745c 745c 745c 725c 6e5c 745c  t\t\t\t\t\r\n\t\
-00018330: 745c 745c 745c 745c 745c 725c 6e5c 745c  t\t\t\t\t\r\n\t\
-00018340: 745c 745c 745c 745c 725c 6e5c 745c 745c  t\t\t\t\r\n\t\t\
-00018350: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
-00018360: 745c 743c 2f64 6976 3e5c 725c 6e5c 745c  t\t</div>\r\n\t\
-00018370: 745c 745c 725c 6e5c 745c 745c 745c 725c  t\t\r\n\t\t\t\r\
-00018380: 6e5c 745c 745c 745c 725c 6e5c 745c 745c  n\t\t\t\r\n\t\t\
-00018390: 745c 725c 6e5c 745c 743c 2f64 6976 3e5c  t\r\n\t\t</div>\
-000183a0: 725c 6e5c 743c 2f64 6976 3e5c 725c 6e5c  r\n\t</div>\r\n\
-000183b0: 725c 6e5c 743c 6469 763e 5c72 5c6e 5c74  r\n\t<div>\r\n\t
-000183c0: 5c74 3c64 6976 0a20 2020 2020 2020 2063  \t<div.        c
-000183d0: 6c61 7373 3d5c 2263 6f6e 7461 696e 6572  lass=\"container
-000183e0: 5c22 3e5c 725c 6e5c 745c 745c 743c 6469  \">\r\n\t\t\t<di
-000183f0: 7620 636c 6173 733d 5c22 726f 775c 223e  v class=\"row\">
-00018400: 5c72 5c6e 5c74 5c74 5c74 5c74 3c64 6976  \r\n\t\t\t\t<div
-00018410: 2063 6c61 7373 3d5c 2263 6f6c 2d73 6d2d   class=\"col-sm-
-00018420: 360a 2020 2020 2020 2020 636f 6c2d 6d64  6.        col-md
-00018430: 2d36 5c22 3e5c 725c 6e5c 745c 745c 745c  -6\">\r\n\t\t\t\
-00018440: 745c 7420 4a5c 7845 3474 656b 756b 6b6f  t\t J\xE4tekukko
-00018450: 204f 795c 725c 6e5c 745c 745c 745c 743c   Oy\r\n\t\t\t\t<
-00018460: 2f64 6976 3e5c 725c 6e5c 745c 745c 745c  /div>\r\n\t\t\t\
-00018470: 743c 6469 760a 2020 2020 2020 2020 636c  t<div.        cl
-00018480: 6173 733d 5c22 636f 6c2d 736d 2d36 2063  ass=\"col-sm-6 c
-00018490: 6f6c 2d6d 642d 365c 223e 5c72 5c6e 5c74  ol-md-6\">\r\n\t
-000184a0: 5c74 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \t\t\t\t\r\n\t\t
-000184b0: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-000184c0: 5c74 5c74 3c2f 6469 763e 5c72 5c6e 5c74  \t\t</div>\r\n\t
-000184d0: 5c74 3c2f 6469 763e 5c72 5c6e 5c74 3c2f  \t</div>\r\n\t</
-000184e0: 6469 763e 5c72 5c6e 3c2f 666f 6f74 6572  div>\r\n</footer
-000184f0: 3e5c 725c 6e5c 725c 6e0a 2020 2020 2020  >\r\n\r\n.      
-00018500: 2020 5c20 2020 3c21 2d2d 204a 5175 6572    \   <!-- JQuer
-00018510: 7920 2d2d 3e5c 725c 6e3c 7363 7269 7074  y -->\r\n<script
-00018520: 2073 7263 3d5c 222f 2f61 6a61 782e 676f   src=\"//ajax.go
-00018530: 6f67 6c65 6170 6973 2e63 6f6d 2f61 6a61  ogleapis.com/aja
-00018540: 782f 6c69 6273 2f6a 7175 6572 792f 312e  x/libs/jquery/1.
-00018550: 3132 2e34 2f6a 7175 6572 792e 6d69 6e2e  12.4/jquery.min.
-00018560: 6a73 5c22 3e3c 2f73 6372 6970 743e 5c72  js\"></script>\r
-00018570: 5c6e 3c73 6372 6970 743e 7769 6e64 6f77  \n<script>window
-00018580: 2e6a 5175 6572 790a 2020 2020 2020 2020  .jQuery.        
-00018590: 7c7c 2064 6f63 756d 656e 742e 7772 6974  || document.writ
-000185a0: 6528 273c 7363 7269 7074 2073 7263 3d5c  e('<script src=\
-000185b0: 226a 732f 7665 6e64 6f72 2f6a 7175 6572  "js/vendor/jquer
-000185c0: 792d 312e 3130 2e32 2e6d 696e 2e6a 735c  y-1.10.2.min.js\
-000185d0: 223e 3c5c 5c2f 7363 7269 7074 3e27 293c  "><\\/script>')<
-000185e0: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
-000185f0: 6970 740a 2020 2020 2020 2020 7372 633d  ipt.        src=
-00018600: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
-00018610: 6a71 7565 7279 2e76 616c 6964 6174 652e  jquery.validate.
-00018620: 6d69 6e2e 6a73 5c22 3e3c 2f73 6372 6970  min.js\"></scrip
-00018630: 743e 5c72 5c6e 3c73 6372 6970 7420 7372  t>\r\n<script sr
-00018640: 633d 5c22 2f6a 6174 656b 756b 6b6f 2f6a  c=\"/jatekukko/j
-00018650: 732f 6a71 7565 7279 2e6e 756d 6265 722e  s/jquery.number.
-00018660: 6d69 6e2e 6a73 5c22 3e3c 2f73 6372 6970  min.js\"></scrip
-00018670: 743e 5c72 5c6e 5c72 5c6e 3c21 2d2d 0a20  t>\r\n\r\n<!--. 
-00018680: 2020 2020 2020 204a 5175 6572 7920 476c         JQuery Gl
-00018690: 6f62 616c 697a 6520 2d2d 3e5c 725c 6e3c  obalize -->\r\n<
-000186a0: 7363 7269 7074 2073 7263 3d5c 222f 6a61  script src=\"/ja
-000186b0: 7465 6b75 6b6b 6f2f 6a73 2f67 6c6f 6261  tekukko/js/globa
-000186c0: 6c69 7a65 2f63 6c64 722e 6a73 5c22 3e3c  lize/cldr.js\"><
-000186d0: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
-000186e0: 6970 740a 2020 2020 2020 2020 7372 633d  ipt.        src=
-000186f0: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
-00018700: 676c 6f62 616c 697a 652f 636c 6472 2f65  globalize/cldr/e
-00018710: 7665 6e74 2e6a 735c 223e 3c2f 7363 7269  vent.js\"></scri
-00018720: 7074 3e5c 725c 6e3c 7363 7269 7074 2073  pt>\r\n<script s
-00018730: 7263 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  rc=\"/jatekukko/
-00018740: 6a73 2f67 6c6f 6261 6c69 7a65 2f63 6c64  js/globalize/cld
-00018750: 722f 7375 7070 6c65 6d65 6e74 616c 2e6a  r/supplemental.j
-00018760: 735c 223e 3c2f 7363 7269 7074 3e5c 725c  s\"></script>\r\
-00018770: 6e3c 7363 7269 7074 0a20 2020 2020 2020  n<script.       
-00018780: 2073 7263 3d5c 222f 6a61 7465 6b75 6b6b   src=\"/jatekukk
-00018790: 6f2f 6a73 2f67 6c6f 6261 6c69 7a65 2f67  o/js/globalize/g
-000187a0: 6c6f 6261 6c69 7a65 2e6a 735c 223e 3c2f  lobalize.js\"></
-000187b0: 7363 7269 7074 3e5c 725c 6e3c 7363 7269  script>\r\n<scri
-000187c0: 7074 2073 7263 3d5c 222f 6a61 7465 6b75  pt src=\"/jateku
-000187d0: 6b6b 6f2f 6a73 2f67 6c6f 6261 6c69 7a65  kko/js/globalize
-000187e0: 2f67 6c6f 6261 6c69 7a65 2f6d 6573 7361  /globalize/messa
-000187f0: 6765 2e6a 735c 223e 3c2f 7363 7269 7074  ge.js\"></script
-00018800: 3e5c 725c 6e5c 725c 6e3c 212d 2d0a 2020  >\r\n\r\n<!--.  
-00018810: 2020 2020 2020 4a53 2043 6f6f 6b69 6520        JS Cookie 
-00018820: 2d2d 3e5c 725c 6e3c 7363 7269 7074 2073  -->\r\n<script s
-00018830: 7263 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  rc=\"/jatekukko/
-00018840: 6a73 2f6a 732d 636f 6f6b 6965 2f6a 732e  js/js-cookie/js.
-00018850: 636f 6f6b 6965 2e6a 735c 223e 3c2f 7363  cookie.js\"></sc
-00018860: 7269 7074 3e5c 725c 6e5c 725c 6e3c 7363  ript>\r\n\r\n<sc
-00018870: 7269 7074 0a20 2020 2020 2020 2073 7263  ript.        src
-00018880: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6a73  =\"/jatekukko/js
-00018890: 2f6d 6f6d 656e 742f 6d6f 6d65 6e74 2d77  /moment/moment-w
-000188a0: 6974 682d 6c6f 6361 6c65 732e 6d69 6e2e  ith-locales.min.
-000188b0: 6a73 5c22 3e3c 2f73 6372 6970 743e 5c72  js\"></script>\r
-000188c0: 5c6e 3c73 6372 6970 743e 6d6f 6d65 6e74  \n<script>moment
-000188d0: 2e6c 6f63 616c 6528 2766 695f 4649 272e  .locale('fi_FI'.
-000188e0: 7265 706c 6163 6528 275f 272c 0a20 2020  replace('_',.   
-000188f0: 2020 2020 2027 2d27 2929 3b3c 2f73 6372       '-'));</scr
-00018900: 6970 743e 5c72 5c6e 5c72 5c6e 3c21 2d2d  ipt>\r\n\r\n<!--
-00018910: 2057 6562 7368 696d 202d 2d3e 5c72 5c6e   Webshim -->\r\n
-00018920: 3c21 2d2d 5b69 6620 6c74 2049 4520 3130  <!--[if lt IE 10
-00018930: 5d3e 5c72 5c6e 5c74 3c73 6372 6970 740a  ]>\r\n\t<script.
-00018940: 2020 2020 2020 2020 7372 633d 5c22 2f6a          src=\"/j
-00018950: 6174 656b 756b 6b6f 2f6a 732f 6a73 2d77  atekukko/js/js-w
-00018960: 6562 7368 696d 2f6d 696e 6966 6965 642f  ebshim/minified/
-00018970: 706f 6c79 6669 6c6c 6572 2e6a 735c 223e  polyfiller.js\">
-00018980: 3c2f 7363 7269 7074 3e5c 725c 6e5c 743c  </script>\r\n\t<
-00018990: 7363 7269 7074 3e5c 725c 6e5c 7477 6562  script>\r\n\tweb
-000189a0: 7368 696d 2e73 6574 4f70 7469 6f6e 7328  shim.setOptions(
-000189b0: 2765 7874 656e 644e 6174 6976 6527 2c0a  'extendNative',.
-000189c0: 2020 2020 2020 2020 7472 7565 293b 5c72          true);\r
-000189d0: 5c6e 5c74 7765 6273 6869 6d2e 706f 6c79  \n\twebshim.poly
-000189e0: 6669 6c6c 2827 666f 726d 7327 293b 5c72  fill('forms');\r
-000189f0: 5c6e 5c74 3c2f 7363 7269 7074 3e5c 725c  \n\t</script>\r\
-00018a00: 6e3c 215b 656e 6469 665d 2d2d 3e5c 725c  n<![endif]-->\r\
-00018a10: 6e5c 725c 6e3c 212d 2d0a 2020 2020 2020  n\r\n<!--.      
-00018a20: 2020 6874 6d6c 3573 6869 7620 2d2d 3e5c    html5shiv -->\
-00018a30: 725c 6e3c 212d 2d5b 6966 206c 7420 4945  r\n<!--[if lt IE
-00018a40: 2039 5d3e 5c72 5c6e 2020 2020 3c73 6372   9]>\r\n    <scr
-00018a50: 6970 7420 7372 633d 5c22 2f6a 6174 656b  ipt src=\"/jatek
-00018a60: 756b 6b6f 2f6a 732f 6874 6d6c 3573 6869  ukko/js/html5shi
-00018a70: 762e 6d69 6e2e 6a73 5c22 3e3c 2f73 6372  v.min.js\"></scr
-00018a80: 6970 743e 5c72 5c6e 3c21 5b65 6e64 6966  ipt>\r\n<![endif
-00018a90: 5d2d 2d3e 5c72 5c6e 5c72 5c6e 3c21 2d2d  ]-->\r\n\r\n<!--
-00018aa0: 0a20 2020 2020 2020 2044 4854 4d4c 5820  .        DHTMLX 
-00018ab0: 2d2d 3e5c 725c 6e3c 7363 7269 7074 2073  -->\r\n<script s
-00018ac0: 7263 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  rc=\"/jatekukko/
-00018ad0: 6a73 2f64 6874 6d6c 7853 7569 7465 2f73  js/dhtmlxSuite/s
-00018ae0: 6f75 7263 6573 2f64 6874 6d6c 7843 6f6d  ources/dhtmlxCom
-00018af0: 6d6f 6e2f 636f 6465 6261 7365 2f64 6874  mon/codebase/dht
-00018b00: 6d6c 7863 6f6d 6d6f 6e2e 6a73 5c22 3e3c  mlxcommon.js\"><
-00018b10: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
-00018b20: 6970 740a 2020 2020 2020 2020 7372 633d  ipt.        src=
-00018b30: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
-00018b40: 6468 746d 6c78 5375 6974 652f 736f 7572  dhtmlxSuite/sour
-00018b50: 6365 732f 6468 746d 6c78 436f 6d6d 6f6e  ces/dhtmlxCommon
-00018b60: 2f63 6f64 6562 6173 652f 6468 746d 6c78  /codebase/dhtmlx
-00018b70: 636f 7265 2e6a 735c 223e 3c2f 7363 7269  core.js\"></scri
-00018b80: 7074 3e5c 725c 6e3c 7363 7269 7074 0a20  pt>\r\n<script. 
-00018b90: 2020 2020 2020 2073 7263 3d5c 222f 6a61         src=\"/ja
-00018ba0: 7465 6b75 6b6b 6f2f 6a73 2f64 6874 6d6c  tekukko/js/dhtml
-00018bb0: 7853 7569 7465 2f73 6f75 7263 6573 2f64  xSuite/sources/d
-00018bc0: 6874 6d6c 7846 6f72 6d2f 636f 6465 6261  htmlxForm/codeba
-00018bd0: 7365 2f64 6874 6d6c 7866 6f72 6d2e 6a73  se/dhtmlxform.js
-00018be0: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
-00018bf0: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
-00018c00: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
-00018c10: 2f6a 732f 6468 746d 6c78 5375 6974 652f  /js/dhtmlxSuite/
-00018c20: 736f 7572 6365 732f 6468 746d 6c78 466f  sources/dhtmlxFo
-00018c30: 726d 2f63 6f64 6562 6173 652f 6578 742f  rm/codebase/ext/
-00018c40: 6468 746d 6c78 666f 726d 5f69 7465 6d5f  dhtmlxform_item_
-00018c50: 6361 6c65 6e64 6172 2e6a 735c 223e 3c2f  calendar.js\"></
-00018c60: 7363 7269 7074 3e5c 725c 6e3c 7363 7269  script>\r\n<scri
-00018c70: 7074 0a20 2020 2020 2020 2073 7263 3d5c  pt.        src=\
-00018c80: 222f 6a61 7465 6b75 6b6b 6f2f 6a73 2f64  "/jatekukko/js/d
-00018c90: 6874 6d6c 7853 7569 7465 2f73 6f75 7263  htmlxSuite/sourc
-00018ca0: 6573 2f64 6874 6d6c 7846 6f72 6d2f 636f  es/dhtmlxForm/co
-00018cb0: 6465 6261 7365 2f65 7874 2f64 6874 6d6c  debase/ext/dhtml
-00018cc0: 7866 6f72 6d5f 6479 6e2e 6a73 5c22 3e3c  xform_dyn.js\"><
-00018cd0: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
-00018ce0: 6970 740a 2020 2020 2020 2020 7372 633d  ipt.        src=
-00018cf0: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
-00018d00: 6468 746d 6c78 5375 6974 652f 736f 7572  dhtmlxSuite/sour
-00018d10: 6365 732f 6468 746d 6c78 4361 6c65 6e64  ces/dhtmlxCalend
-00018d20: 6172 2f63 6f64 6562 6173 652f 6468 746d  ar/codebase/dhtm
-00018d30: 6c78 6361 6c65 6e64 6172 2e6a 735c 223e  lxcalendar.js\">
-00018d40: 3c2f 7363 7269 7074 3e5c 725c 6e3c 7363  </script>\r\n<sc
-00018d50: 7269 7074 0a20 2020 2020 2020 2073 7263  ript.        src
-00018d60: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6a73  =\"/jatekukko/js
-00018d70: 2f64 6874 6d6c 7853 7569 7465 2f73 6f75  /dhtmlxSuite/sou
-00018d80: 7263 6573 2f64 6874 6d6c 7854 6f6f 6c62  rces/dhtmlxToolb
-00018d90: 6172 2f63 6f64 6562 6173 652f 6468 746d  ar/codebase/dhtm
-00018da0: 6c78 746f 6f6c 6261 722e 6a73 5c22 3e3c  lxtoolbar.js\"><
-00018db0: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
-00018dc0: 6970 740a 2020 2020 2020 2020 7372 633d  ipt.        src=
-00018dd0: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
-00018de0: 6468 746d 6c78 5375 6974 652f 736f 7572  dhtmlxSuite/sour
-00018df0: 6365 732f 6468 746d 6c78 4461 7461 5669  ces/dhtmlxDataVi
-00018e00: 6577 2f63 6f64 6562 6173 652f 6468 746d  ew/codebase/dhtm
-00018e10: 6c78 6461 7461 7669 6577 2e6a 735c 223e  lxdataview.js\">
-00018e20: 3c2f 7363 7269 7074 3e5c 725c 6e3c 7363  </script>\r\n<sc
-00018e30: 7269 7074 0a20 2020 2020 2020 2073 7263  ript.        src
-00018e40: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6a73  =\"/jatekukko/js
-00018e50: 2f64 6874 6d6c 7853 7569 7465 2f73 6f75  /dhtmlxSuite/sou
-00018e60: 7263 6573 2f64 6874 6d6c 7847 7269 642f  rces/dhtmlxGrid/
-00018e70: 636f 6465 6261 7365 2f64 6874 6d6c 7867  codebase/dhtmlxg
-00018e80: 7269 642e 6a73 5c22 3e3c 2f73 6372 6970  rid.js\"></scrip
-00018e90: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
-00018ea0: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
-00018eb0: 656b 756b 6b6f 2f6a 732f 6468 746d 6c78  ekukko/js/dhtmlx
-00018ec0: 5375 6974 652f 736f 7572 6365 732f 6468  Suite/sources/dh
-00018ed0: 746d 6c78 4d65 7373 6167 652f 636f 6465  tmlxMessage/code
-00018ee0: 6261 7365 2f64 6874 6d6c 786d 6573 7361  base/dhtmlxmessa
-00018ef0: 6765 2e6a 735c 223e 3c2f 7363 7269 7074  ge.js\"></script
-00018f00: 3e5c 725c 6e5c 725c 6e3c 212d 2d0a 2020  >\r\n\r\n<!--.  
-00018f10: 2020 2020 2020 4f76 6572 7772 6974 6520        Overwrite 
-00018f20: 4448 544d 4c58 2064 6878 666f 726d 5f62  DHTMLX dhxform_b
-00018f30: 746e 2072 6f6c 652e 2054 6869 7320 6d75  tn role. This mu
-00018f40: 7374 2062 6520 6c6f 6164 6564 2061 6674  st be loaded aft
-00018f50: 6572 2044 4854 4d4c 5821 202d 2d3e 5c72  er DHTMLX! -->\r
-00018f60: 5c6e 3c73 6372 6970 740a 2020 2020 2020  \n<script.      
-00018f70: 2020 7372 633d 5c22 2f6a 6174 656b 756b    src=\"/jatekuk
-00018f80: 6b6f 2f6a 732f 6468 746d 6c78 5f66 6f72  ko/js/dhtmlx_for
-00018f90: 6d5f 706f 7374 6c6f 6164 2e6a 733f 7469  m_postload.js?ti
-00018fa0: 6d65 7374 616d 703d 3230 3233 3035 3035  mestamp=20230505
-00018fb0: 2d30 3732 395c 223e 3c2f 7363 7269 7074  -0729\"></script
-00018fc0: 3e5c 725c 6e5c 725c 6e3c 212d 2d0a 2020  >\r\n\r\n<!--.  
-00018fd0: 2020 2020 2020 5c20 4b65 6e64 6f20 5549        \ Kendo UI
-00018fe0: 202d 2d3e 5c72 5c6e 3c73 6372 6970 7420   -->\r\n<script 
-00018ff0: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
-00019000: 2f6a 732f 6b65 6e64 6f75 692f 6b65 6e64  /js/kendoui/kend
-00019010: 6f2e 636f 7265 2e6d 696e 2e6a 735c 223e  o.core.min.js\">
-00019020: 3c2f 7363 7269 7074 3e5c 745c 725c 6e3c  </script>\t\r\n<
-00019030: 7363 7269 7074 0a20 2020 2020 2020 2073  script.        s
-00019040: 7263 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  rc=\"/jatekukko/
-00019050: 6a73 2f6b 656e 646f 7569 2f6b 656e 646f  js/kendoui/kendo
-00019060: 2e64 6174 612e 6d69 6e2e 6a73 5c22 3e3c  .data.min.js\"><
-00019070: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
-00019080: 6970 7420 7372 633d 5c22 2f6a 6174 656b  ipt src=\"/jatek
-00019090: 756b 6b6f 2f6a 732f 6b65 6e64 6f75 692f  ukko/js/kendoui/
-000190a0: 6b65 6e64 6f2e 646f 6d2e 6d69 6e2e 6a73  kendo.dom.min.js
-000190b0: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
-000190c0: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
-000190d0: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
-000190e0: 2f6a 732f 6b65 6e64 6f75 692f 6b65 6e64  /js/kendoui/kend
-000190f0: 6f2e 706f 7075 702e 6d69 6e2e 6a73 5c22  o.popup.min.js\"
-00019100: 3e3c 2f73 6372 6970 743e 5c72 5c6e 3c73  ></script>\r\n<s
-00019110: 6372 6970 7420 7372 633d 5c22 2f6a 6174  cript src=\"/jat
-00019120: 656b 756b 6b6f 2f6a 732f 6b65 6e64 6f75  ekukko/js/kendou
-00019130: 692f 6b65 6e64 6f2e 6c69 7374 2e6d 696e  i/kendo.list.min
-00019140: 2e6a 735c 223e 3c2f 7363 7269 7074 3e5c  .js\"></script>\
-00019150: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
-00019160: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
-00019170: 6b6b 6f2f 6a73 2f6b 656e 646f 7569 2f6b  kko/js/kendoui/k
-00019180: 656e 646f 2e66 782e 6d69 6e2e 6a73 5c22  endo.fx.min.js\"
-00019190: 3e3c 2f73 6372 6970 743e 5c72 5c6e 3c73  ></script>\r\n<s
-000191a0: 6372 6970 7420 7372 633d 5c22 2f6a 6174  cript src=\"/jat
-000191b0: 656b 756b 6b6f 2f6a 732f 6b65 6e64 6f75  ekukko/js/kendou
-000191c0: 692f 6b65 6e64 6f2e 7573 6572 6576 656e  i/kendo.usereven
-000191d0: 7473 2e6d 696e 2e6a 735c 223e 3c2f 7363  ts.min.js\"></sc
-000191e0: 7269 7074 3e5c 725c 6e3c 7363 7269 7074  ript>\r\n<script
-000191f0: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
-00019200: 6a61 7465 6b75 6b6b 6f2f 6a73 2f6b 656e  jatekukko/js/ken
-00019210: 646f 7569 2f6b 656e 646f 2e64 7261 6761  doui/kendo.draga
-00019220: 6e64 6472 6f70 2e6d 696e 2e6a 735c 223e  nddrop.min.js\">
-00019230: 3c2f 7363 7269 7074 3e5c 725c 6e3c 7363  </script>\r\n<sc
-00019240: 7269 7074 0a20 2020 2020 2020 2073 7263  ript.        src
-00019250: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6a73  =\"/jatekukko/js
-00019260: 2f6b 656e 646f 7569 2f6b 656e 646f 2e72  /kendoui/kendo.r
-00019270: 6573 697a 6162 6c65 2e6d 696e 2e6a 735c  esizable.min.js\
-00019280: 223e 3c2f 7363 7269 7074 3e5c 725c 6e3c  "></script>\r\n<
-00019290: 7363 7269 7074 0a20 2020 2020 2020 2073  script.        s
-000192a0: 7263 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  rc=\"/jatekukko/
-000192b0: 6a73 2f6b 656e 646f 7569 2f6b 656e 646f  js/kendoui/kendo
-000192c0: 2e65 6469 7461 626c 652e 6d69 6e2e 6a73  .editable.min.js
-000192d0: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
-000192e0: 3c73 6372 6970 7420 7372 633d 5c22 2f6a  <script src=\"/j
-000192f0: 6174 656b 756b 6b6f 2f6a 732f 6b65 6e64  atekukko/js/kend
-00019300: 6f75 692f 6b65 6e64 6f2e 6269 6e64 6572  oui/kendo.binder
-00019310: 2e6d 696e 2e6a 735c 223e 3c2f 7363 7269  .min.js\"></scri
-00019320: 7074 3e5c 725c 6e3c 7363 7269 7074 0a20  pt>\r\n<script. 
-00019330: 2020 2020 2020 2073 7263 3d5c 222f 6a61         src=\"/ja
-00019340: 7465 6b75 6b6b 6f2f 6a73 2f6b 656e 646f  tekukko/js/kendo
-00019350: 7569 2f6b 656e 646f 2e76 616c 6964 6174  ui/kendo.validat
-00019360: 6f72 2e6d 696e 2e6a 735c 223e 3c2f 7363  or.min.js\"></sc
-00019370: 7269 7074 3e5c 725c 6e3c 7363 7269 7074  ript>\r\n<script
-00019380: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
-00019390: 6a61 7465 6b75 6b6b 6f2f 6a73 2f6b 656e  jatekukko/js/ken
-000193a0: 646f 7569 2f6b 656e 646f 2e6d 6f62 696c  doui/kendo.mobil
-000193b0: 652e 7363 726f 6c6c 6572 2e6d 696e 2e6a  e.scroller.min.j
-000193c0: 735c 223e 3c2f 7363 7269 7074 3e5c 725c  s\"></script>\r\
-000193d0: 6e3c 7363 7269 7074 0a20 2020 2020 2020  n<script.       
-000193e0: 2073 7263 3d5c 222f 6a61 7465 6b75 6b6b   src=\"/jatekukk
-000193f0: 6f2f 6a73 2f6b 656e 646f 7569 2f6b 656e  o/js/kendoui/ken
-00019400: 646f 2e76 6972 7475 616c 6c69 7374 2e6d  do.virtuallist.m
-00019410: 696e 2e6a 735c 223e 3c2f 7363 7269 7074  in.js\"></script
-00019420: 3e5c 725c 6e3c 7363 7269 7074 0a20 2020  >\r\n<script.   
-00019430: 2020 2020 2073 7263 3d5c 222f 6a61 7465       src=\"/jate
-00019440: 6b75 6b6b 6f2f 6a73 2f6b 656e 646f 7569  kukko/js/kendoui
-00019450: 2f6b 656e 646f 2e63 6f6c 756d 6e73 6f72  /kendo.columnsor
-00019460: 7465 722e 6d69 6e2e 6a73 5c22 3e3c 2f73  ter.min.js\"></s
-00019470: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
-00019480: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
-00019490: 2f6a 6174 656b 756b 6b6f 2f6a 732f 6b65  /jatekukko/js/ke
-000194a0: 6e64 6f75 692f 6375 6c74 7572 6573 2f6b  ndoui/cultures/k
-000194b0: 656e 646f 2e63 756c 7475 7265 2e66 692d  endo.culture.fi-
-000194c0: 4649 2e6d 696e 2e6a 735c 223e 3c2f 7363  FI.min.js\"></sc
-000194d0: 7269 7074 3e5c 725c 6e3c 7363 7269 7074  ript>\r\n<script
-000194e0: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
-000194f0: 6a61 7465 6b75 6b6b 6f2f 6a73 2f6b 656e  jatekukko/js/ken
-00019500: 646f 7569 2f63 756c 7475 7265 732f 6b65  doui/cultures/ke
-00019510: 6e64 6f2e 6375 6c74 7572 652e 7376 2d46  ndo.culture.sv-F
-00019520: 492e 6d69 6e2e 6a73 5c22 3e3c 2f73 6372  I.min.js\"></scr
-00019530: 6970 743e 5c72 5c6e 5c72 5c6e 3c21 2d2d  ipt>\r\n\r\n<!--
-00019540: 0a20 2020 2020 2020 204b 656e 646f 2055  .        Kendo U
-00019550: 492c 2061 6374 7561 6c20 636f 6d70 6f6e  I, actual compon
-00019560: 656e 7473 202d 2d3e 5c72 5c6e 3c73 6372  ents -->\r\n<scr
-00019570: 6970 7420 7372 633d 5c22 2f6a 6174 656b  ipt src=\"/jatek
-00019580: 756b 6b6f 2f6a 732f 6b65 6e64 6f75 692f  ukko/js/kendoui/
-00019590: 6b65 6e64 6f2e 6472 6f70 646f 776e 6c69  kendo.dropdownli
-000195a0: 7374 2e6d 696e 2e6a 735c 223e 3c2f 7363  st.min.js\"></sc
-000195b0: 7269 7074 3e5c 725c 6e3c 7363 7269 7074  ript>\r\n<script
-000195c0: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
-000195d0: 6a61 7465 6b75 6b6b 6f2f 6a73 2f6b 656e  jatekukko/js/ken
-000195e0: 646f 7569 2f6b 656e 646f 2e6e 756d 6572  doui/kendo.numer
-000195f0: 6963 7465 7874 626f 782e 6d69 6e2e 6a73  ictextbox.min.js
-00019600: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
-00019610: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
-00019620: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
-00019630: 2f6a 732f 6b65 6e64 6f75 692f 6b65 6e64  /js/kendoui/kend
-00019640: 6f2e 6772 6964 2e6d 696e 2e6a 735c 223e  o.grid.min.js\">
-00019650: 3c2f 7363 7269 7074 3e5c 725c 6e3c 7363  </script>\r\n<sc
-00019660: 7269 7074 2073 7263 3d5c 222f 6a61 7465  ript src=\"/jate
-00019670: 6b75 6b6b 6f2f 6a73 2f6b 656e 646f 7569  kukko/js/kendoui
-00019680: 2f6b 656e 646f 2e6d 756c 7469 7365 6c65  /kendo.multisele
-00019690: 6374 2e6d 696e 2e6a 735c 223e 3c2f 7363  ct.min.js\"></sc
-000196a0: 7269 7074 3e5c 725c 6e3c 7363 7269 7074  ript>\r\n<script
-000196b0: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
-000196c0: 6a61 7465 6b75 6b6b 6f2f 6a73 2f6b 656e  jatekukko/js/ken
-000196d0: 646f 7569 2f6b 656e 646f 2e74 7265 656c  doui/kendo.treel
-000196e0: 6973 742e 6d69 6e2e 6a73 5c22 3e3c 2f73  ist.min.js\"></s
-000196f0: 6372 6970 743e 5c72 5c6e 5c72 5c6e 3c73  cript>\r\n\r\n<s
-00019700: 6372 6970 740a 2020 2020 2020 2020 7372  cript.        sr
-00019710: 633d 5c22 2f6a 6174 656b 756b 6b6f 2f6a  c=\"/jatekukko/j
-00019720: 732f 6b65 6e64 6f75 692f 6d65 7373 6167  s/kendoui/messag
-00019730: 6573 2f6b 656e 646f 2e6d 6573 7361 6765  es/kendo.message
-00019740: 732e 6669 2d46 492e 6d69 6e2e 6a73 5c22  s.fi-FI.min.js\"
-00019750: 3e3c 2f73 6372 6970 743e 5c72 5c6e 3c21  ></script>\r\n<!
-00019760: 2d2d 0a20 2020 2020 2020 2053 6574 206b  --.        Set k
-00019770: 656e 646f 2074 6f20 7269 6768 7420 6375  endo to right cu
-00019780: 6c74 7572 6520 2d2d 3e5c 725c 6e3c 7363  lture -->\r\n<sc
-00019790: 7269 7074 3e5c 725c 6e5c 746b 656e 646f  ript>\r\n\tkendo
-000197a0: 2e63 756c 7475 7265 285c 2266 695f 4649  .culture(\"fi_FI
-000197b0: 5c22 2e72 6570 6c61 6365 2827 5f27 2c0a  \".replace('_',.
-000197c0: 2020 2020 2020 2020 272d 2729 293b 5c72          '-'));\r
-000197d0: 5c6e 3c2f 7363 7269 7074 3e5c 725c 6e5c  \n</script>\r\n\
-000197e0: 725c 6e5c 725c 6e3c 212d 2d20 4172 6347  r\n\r\n<!-- ArcG
-000197f0: 4953 202d 2d3e 5c72 5c6e 3c73 6372 6970  IS -->\r\n<scrip
-00019800: 743e 5c72 5c6e 2020 2020 7661 7220 646f  t>\r\n    var do
-00019810: 6a6f 436f 6e66 6967 0a20 2020 2020 2020  joConfig.       
-00019820: 203d 207b 5c72 5c6e 2020 2020 2020 2020   = {\r\n        
-00019830: 6c6f 6361 6c65 3a20 2766 695f 4649 272e  locale: 'fi_FI'.
-00019840: 746f 4c6f 7765 7243 6173 6528 292e 7265  toLowerCase().re
-00019850: 706c 6163 6528 275f 272c 2027 2d27 295c  place('_', '-')\
-00019860: 725c 6e20 2020 207d 3b5c 725c 6e3c 2f73  r\n    };\r\n</s
-00019870: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
-00019880: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
-00019890: 6874 7470 733a 2f2f 6a73 2e61 7263 6769  https://js.arcgi
-000198a0: 732e 636f 6d2f 332e 3339 2f5c 223e 3c2f  s.com/3.39/\"></
-000198b0: 7363 7269 7074 3e5c 725c 6e5c 725c 6e3c  script>\r\n\r\n<
-000198c0: 212d 2d20 426f 6f74 7374 7261 7020 2d2d  !-- Bootstrap --
-000198d0: 3e5c 725c 6e3c 7363 7269 7074 0a20 2020  >\r\n<script.   
-000198e0: 2020 2020 2073 7263 3d5c 222f 6a61 7465       src=\"/jate
-000198f0: 6b75 6b6b 6f2f 6a73 2f62 6f6f 7473 7472  kukko/js/bootstr
-00019900: 6170 2f62 6f6f 7473 7472 6170 2e6d 696e  ap/bootstrap.min
-00019910: 2e6a 735c 223e 3c2f 7363 7269 7074 3e5c  .js\"></script>\
-00019920: 725c 6e5c 725c 6e3c 212d 2d20 4375 7374  r\n\r\n<!-- Cust
-00019930: 6f6d 0a20 2020 2020 2020 202d 2d3e 5c72  om.        -->\r
-00019940: 5c6e 3c73 6372 6970 7420 7372 633d 5c22  \n<script src=\"
-00019950: 2f6a 6174 656b 756b 6b6f 2f6a 732f 6468  /jatekukko/js/dh
-00019960: 746d 6c78 5f65 7874 2e6a 733f 7469 6d65  tmlx_ext.js?time
-00019970: 7374 616d 703d 3230 3233 3035 3035 2d30  stamp=20230505-0
-00019980: 3732 395c 223e 3c2f 7363 7269 7074 3e5c  729\"></script>\
-00019990: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
-000199a0: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
-000199b0: 6b6b 6f2f 6a73 2f64 6874 6d6c 785f 6578  kko/js/dhtmlx_ex
-000199c0: 745f 7765 656b 5f63 616c 656e 6461 722e  t_week_calendar.
-000199d0: 6a73 3f74 696d 6573 7461 6d70 3d32 3032  js?timestamp=202
-000199e0: 3330 3530 352d 3037 3239 5c22 3e3c 2f73  30505-0729\"></s
-000199f0: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
-00019a00: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
-00019a10: 2f6a 6174 656b 756b 6b6f 2f6a 732f 636f  /jatekukko/js/co
-00019a20: 6d6d 6f6e 2e6a 733f 7469 6d65 7374 616d  mmon.js?timestam
-00019a30: 703d 3230 3233 3035 3035 2d30 3732 395c  p=20230505-0729\
-00019a40: 223e 3c2f 7363 7269 7074 3e5c 725c 6e3c  "></script>\r\n<
-00019a50: 7363 7269 7074 0a20 2020 2020 2020 2073  script.        s
-00019a60: 7263 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  rc=\"/jatekukko/
-00019a70: 6a73 2f76 616c 6964 6174 6f72 732e 6a73  js/validators.js
-00019a80: 3f74 696d 6573 7461 6d70 3d32 3032 3330  ?timestamp=20230
-00019a90: 3530 352d 3037 3239 5c22 3e3c 2f73 6372  505-0729\"></scr
-00019aa0: 6970 743e 5c72 5c6e 3c73 6372 6970 740a  ipt>\r\n<script.
-00019ab0: 2020 2020 2020 2020 7372 633d 5c22 2f6a          src=\"/j
-00019ac0: 6174 656b 756b 6b6f 2f6a 732f 676f 6f67  atekukko/js/goog
-00019ad0: 6c65 2e6a 733f 7469 6d65 7374 616d 703d  le.js?timestamp=
-00019ae0: 3230 3233 3035 3035 2d30 3732 395c 223e  20230505-0729\">
-00019af0: 3c2f 7363 7269 7074 3e5c 725c 6e3c 7363  </script>\r\n<sc
-00019b00: 7269 7074 0a20 2020 2020 2020 2073 7263  ript.        src
-00019b10: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6a73  =\"/jatekukko/js
-00019b20: 2f73 6861 7265 642f 7469 6d65 6f75 742e  /shared/timeout.
-00019b30: 6a73 3f74 696d 6573 7461 6d70 3d32 3032  js?timestamp=202
-00019b40: 3330 3530 352d 3037 3239 5c22 3e3c 2f73  30505-0729\"></s
-00019b50: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
-00019b60: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
-00019b70: 2f6a 6174 656b 756b 6b6f 2f6a 732f 7368  /jatekukko/js/sh
-00019b80: 6172 6564 2f76 696d 656f 2e6a 733f 7469  ared/vimeo.js?ti
-00019b90: 6d65 7374 616d 703d 3230 3233 3035 3035  mestamp=20230505
-00019ba0: 2d30 3732 395c 223e 3c2f 7363 7269 7074  -0729\"></script
-00019bb0: 3e5c 725c 6e5c 725c 6e3c 7363 7269 7074  >\r\n\r\n<script
-00019bc0: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
-00019bd0: 6a61 7465 6b75 6b6b 6f2f 6a73 2f73 6168  jatekukko/js/sah
-00019be0: 6173 2f61 7070 6c69 6361 7469 6f6e 2e6a  as/application.j
-00019bf0: 733f 7469 6d65 7374 616d 703d 3230 3233  s?timestamp=2023
-00019c00: 3035 3035 2d30 3732 395c 223e 3c2f 7363  0505-0729\"></sc
-00019c10: 7269 7074 3e5c 725c 6e3c 7363 7269 7074  ript>\r\n<script
-00019c20: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
-00019c30: 6a61 7465 6b75 6b6b 6f2f 6a73 2f73 6168  jatekukko/js/sah
-00019c40: 6173 2f6c 6f67 696e 2e6a 733f 7469 6d65  as/login.js?time
-00019c50: 7374 616d 703d 3230 3233 3035 3035 2d30  stamp=20230505-0
-00019c60: 3732 395c 223e 3c2f 7363 7269 7074 3e5c  729\"></script>\
-00019c70: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
-00019c80: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
-00019c90: 6b6b 6f2f 6a73 2f73 6168 6173 2f73 6572  kko/js/sahas/ser
-00019ca0: 7669 6365 5f77 696e 646f 7773 2e6a 733f  vice_windows.js?
-00019cb0: 7469 6d65 7374 616d 703d 3230 3233 3035  timestamp=202305
-00019cc0: 3035 2d30 3732 395c 223e 3c2f 7363 7269  05-0729\"></scri
-00019cd0: 7074 3e5c 725c 6e3c 7363 7269 7074 0a20  pt>\r\n<script. 
-00019ce0: 2020 2020 2020 2073 7263 3d5c 222f 6a61         src=\"/ja
-00019cf0: 7465 6b75 6b6b 6f2f 6a73 2f73 6168 6173  tekukko/js/sahas
-00019d00: 2f73 686f 7070 696e 6763 6172 742e 6a73  /shoppingcart.js
-00019d10: 3f74 696d 6573 7461 6d70 3d32 3032 3330  ?timestamp=20230
-00019d20: 3530 352d 3037 3239 5c22 3e3c 2f73 6372  505-0729\"></scr
-00019d30: 6970 743e 5c72 5c6e 3c73 6372 6970 740a  ipt>\r\n<script.
-00019d40: 2020 2020 2020 2020 7372 633d 5c22 2f6a          src=\"/j
-00019d50: 6174 656b 756b 6b6f 2f6a 732f 7361 6861  atekukko/js/saha
-00019d60: 732f 7365 7276 6963 655f 616b 702e 6a73  s/service_akp.js
-00019d70: 3f74 696d 6573 7461 6d70 3d32 3032 3330  ?timestamp=20230
-00019d80: 3530 352d 3037 3239 5c22 3e3c 2f73 6372  505-0729\"></scr
-00019d90: 6970 743e 5c72 5c6e 5c72 5c6e 3c73 6372  ipt>\r\n\r\n<scr
-00019da0: 6970 740a 2020 2020 2020 2020 7372 633d  ipt.        src=
-00019db0: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
-00019dc0: 7361 6861 732f 7461 6273 2f73 6572 7669  sahas/tabs/servi
-00019dd0: 6365 2d6c 6973 742e 6a73 3f74 696d 6573  ce-list.js?times
-00019de0: 7461 6d70 3d32 3032 3330 3530 352d 3037  tamp=20230505-07
-00019df0: 3239 5c22 3e3c 2f73 6372 6970 743e 5c72  29\"></script>\r
-00019e00: 5c6e 5c72 5c6e 3c73 6372 6970 740a 2020  \n\r\n<script.  
-00019e10: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
-00019e20: 656b 756b 6b6f 2f6a 732f 7361 6861 732f  ekukko/js/sahas/
-00019e30: 7461 6273 2f63 7573 746f 6d65 722d 6461  tabs/customer-da
-00019e40: 7461 2e6a 733f 7469 6d65 7374 616d 703d  ta.js?timestamp=
-00019e50: 3230 3233 3035 3035 2d30 3732 395c 223e  20230505-0729\">
-00019e60: 3c2f 7363 7269 7074 3e5c 725c 6e5c 725c  </script>\r\n\r\
-00019e70: 6e5c 725c 6e3c 7363 7269 7074 0a20 2020  n\r\n<script.   
-00019e80: 2020 2020 2073 7263 3d5c 222f 6a61 7465       src=\"/jate
-00019e90: 6b75 6b6b 6f2f 6a73 2f73 6168 6173 2f74  kukko/js/sahas/t
-00019ea0: 6162 732f 6665 6564 6261 636b 2e6a 733f  abs/feedback.js?
-00019eb0: 7469 6d65 7374 616d 703d 3230 3233 3035  timestamp=202305
-00019ec0: 3035 2d30 3732 395c 223e 3c2f 7363 7269  05-0729\"></scri
-00019ed0: 7074 3e5c 725c 6e5c 725c 6e3c 7363 7269  pt>\r\n\r\n<scri
-00019ee0: 7074 0a20 2020 2020 2020 2073 7263 3d5c  pt.        src=\
-00019ef0: 222f 6a61 7465 6b75 6b6b 6f2f 6a73 2f73  "/jatekukko/js/s
-00019f00: 6168 6173 2f74 6162 732f 7573 6572 2d64  ahas/tabs/user-d
-00019f10: 6574 6169 6c73 2e6a 733f 7469 6d65 7374  etails.js?timest
-00019f20: 616d 703d 3230 3233 3035 3035 2d30 3732  amp=20230505-072
-00019f30: 395c 223e 3c2f 7363 7269 7074 3e5c 725c  9\"></script>\r\
-00019f40: 6e3c 7363 7269 7074 0a20 2020 2020 2020  n<script.       
-00019f50: 2073 7263 3d5c 222f 6a61 7465 6b75 6b6b   src=\"/jatekukk
-00019f60: 6f2f 6a73 2f73 6168 6173 2f74 6162 732f  o/js/sahas/tabs/
-00019f70: 6c6f 6769 6e2d 7061 6765 2e6a 733f 7469  login-page.js?ti
-00019f80: 6d65 7374 616d 703d 3230 3233 3035 3035  mestamp=20230505
-00019f90: 2d30 3732 395c 223e 3c2f 7363 7269 7074  -0729\"></script
-00019fa0: 3e5c 725c 6e5c 725c 6e5c 725c 6e3c 7363  >\r\n\r\n\r\n<sc
-00019fb0: 7269 7074 0a20 2020 2020 2020 2073 7263  ript.        src
-00019fc0: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6a73  =\"/jatekukko/js
-00019fd0: 2f73 6168 6173 2f74 6162 732f 696e 766f  /sahas/tabs/invo
-00019fe0: 6963 652d 6c69 7374 2e6a 733f 7469 6d65  ice-list.js?time
-00019ff0: 7374 616d 703d 3230 3233 3035 3035 2d30  stamp=20230505-0
-0001a000: 3732 395c 223e 3c2f 7363 7269 7074 3e5c  729\"></script>\
-0001a010: 725c 6e5c 725c 6e5c 725c 6e3c 7363 7269  r\n\r\n\r\n<scri
-0001a020: 7074 0a20 2020 2020 2020 2073 7263 3d5c  pt.        src=\
-0001a030: 222f 6a61 7465 6b75 6b6b 6f2f 6a73 2f73  "/jatekukko/js/s
-0001a040: 6168 6173 2f77 696e 646f 7773 2f6c 6f73  ahas/windows/los
-0001a050: 742d 7061 7373 776f 7264 2d77 696e 646f  t-password-windo
-0001a060: 772e 6a73 3f74 696d 6573 7461 6d70 3d32  w.js?timestamp=2
-0001a070: 3032 3330 3530 352d 3037 3239 5c22 3e3c  0230505-0729\"><
-0001a080: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
-0001a090: 6970 740a 2020 2020 2020 2020 7372 633d  ipt.        src=
-0001a0a0: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
-0001a0b0: 7361 6861 732f 7769 6e64 6f77 732f 6368  sahas/windows/ch
-0001a0c0: 616e 6765 2d6a 6f69 6e2d 7479 7065 2d77  ange-join-type-w
-0001a0d0: 696e 646f 772e 6a73 3f74 696d 6573 7461  indow.js?timesta
-0001a0e0: 6d70 3d32 3032 3330 3530 352d 3037 3239  mp=20230505-0729
-0001a0f0: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
-0001a100: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
-0001a110: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
-0001a120: 2f6a 732f 7361 6861 732f 7769 6e64 6f77  /js/sahas/window
-0001a130: 732f 616b 702d 6c6f 6361 7469 6f6e 2d77  s/akp-location-w
-0001a140: 696e 646f 772e 6a73 3f74 696d 6573 7461  indow.js?timesta
-0001a150: 6d70 3d32 3032 3330 3530 352d 3037 3239  mp=20230505-0729
-0001a160: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
-0001a170: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
-0001a180: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
-0001a190: 2f6a 732f 7361 6861 732f 7769 6e64 6f77  /js/sahas/window
-0001a1a0: 732f 626f 6f6b 7570 2d77 696e 646f 772e  s/bookup-window.
-0001a1b0: 6a73 3f74 696d 6573 7461 6d70 3d32 3032  js?timestamp=202
-0001a1c0: 3330 3530 352d 3037 3239 5c22 3e3c 2f73  30505-0729\"></s
-0001a1d0: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
-0001a1e0: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
-0001a1f0: 2f6a 6174 656b 756b 6b6f 2f6a 732f 7361  /jatekukko/js/sa
-0001a200: 6861 732f 7769 6e64 6f77 732f 6665 6564  has/windows/feed
-0001a210: 6261 636b 2d77 696e 646f 772e 6a73 3f74  back-window.js?t
-0001a220: 696d 6573 7461 6d70 3d32 3032 3330 3530  imestamp=2023050
-0001a230: 352d 3037 3239 5c22 3e3c 2f73 6372 6970  5-0729\"></scrip
-0001a240: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
-0001a250: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
-0001a260: 656b 756b 6b6f 2f6a 732f 7361 6861 732f  ekukko/js/sahas/
-0001a270: 7769 6e64 6f77 732f 7061 7373 776f 7264  windows/password
-0001a280: 2d77 696e 646f 772e 6a73 3f74 696d 6573  -window.js?times
-0001a290: 7461 6d70 3d32 3032 3330 3530 352d 3037  tamp=20230505-07
-0001a2a0: 3239 5c22 3e3c 2f73 6372 6970 743e 5c72  29\"></script>\r
-0001a2b0: 5c6e 3c73 6372 6970 740a 2020 2020 2020  \n<script.      
-0001a2c0: 2020 7372 633d 5c22 2f6a 6174 656b 756b    src=\"/jatekuk
-0001a2d0: 6b6f 2f6a 732f 7361 6861 732f 7769 6e64  ko/js/sahas/wind
-0001a2e0: 6f77 732f 6368 616e 6765 2d77 696e 646f  ows/change-windo
-0001a2f0: 772e 6a73 3f74 696d 6573 7461 6d70 3d32  w.js?timestamp=2
-0001a300: 3032 3330 3530 352d 3037 3239 5c22 3e3c  0230505-0729\"><
-0001a310: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
-0001a320: 6970 740a 2020 2020 2020 2020 7372 633d  ipt.        src=
-0001a330: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
-0001a340: 7361 6861 732f 7769 6e64 6f77 732f 7465  sahas/windows/te
-0001a350: 726d 696e 6174 652d 7769 6e64 6f77 2e6a  rminate-window.j
-0001a360: 733f 7469 6d65 7374 616d 703d 3230 3233  s?timestamp=2023
-0001a370: 3035 3035 2d30 3732 395c 223e 3c2f 7363  0505-0729\"></sc
-0001a380: 7269 7074 3e5c 725c 6e3c 7363 7269 7074  ript>\r\n<script
-0001a390: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
-0001a3a0: 6a61 7465 6b75 6b6b 6f2f 6a73 2f73 6168  jatekukko/js/sah
-0001a3b0: 6173 2f77 696e 646f 7773 2f63 7265 6174  as/windows/creat
-0001a3c0: 652d 6f72 6465 722d 7769 6e64 6f77 2e6a  e-order-window.j
-0001a3d0: 733f 7469 6d65 7374 616d 703d 3230 3233  s?timestamp=2023
-0001a3e0: 3035 3035 2d30 3732 395c 223e 3c2f 7363  0505-0729\"></sc
-0001a3f0: 7269 7074 3e5c 725c 6e3c 7363 7269 7074  ript>\r\n<script
-0001a400: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
-0001a410: 6a61 7465 6b75 6b6b 6f2f 6a73 2f73 6168  jatekukko/js/sah
-0001a420: 6173 2f77 696e 646f 7773 2f66 6f72 6d2d  as/windows/form-
-0001a430: 7769 6e64 6f77 2e6a 733f 7469 6d65 7374  window.js?timest
-0001a440: 616d 703d 3230 3233 3035 3035 2d30 3732  amp=20230505-072
-0001a450: 395c 223e 3c2f 7363 7269 7074 3e5c 725c  9\"></script>\r\
-0001a460: 6e3c 7363 7269 7074 0a20 2020 2020 2020  n<script.       
-0001a470: 2073 7263 3d5c 222f 6a61 7465 6b75 6b6b   src=\"/jatekukk
-0001a480: 6f2f 6a73 2f73 6168 6173 2f77 696e 646f  o/js/sahas/windo
-0001a490: 7773 2f63 6f6d 706f 7374 2d77 696e 646f  ws/compost-windo
-0001a4a0: 772e 6a73 3f74 696d 6573 7461 6d70 3d32  w.js?timestamp=2
-0001a4b0: 3032 3330 3530 352d 3037 3239 5c22 3e3c  0230505-0729\"><
-0001a4c0: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
-0001a4d0: 6970 740a 2020 2020 2020 2020 7372 633d  ipt.        src=
-0001a4e0: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
-0001a4f0: 7361 6861 732f 7769 6e64 6f77 732f 7265  sahas/windows/re
-0001a500: 6769 7374 6572 2d77 696e 646f 772e 6a73  gister-window.js
-0001a510: 3f74 696d 6573 7461 6d70 3d32 3032 3330  ?timestamp=20230
-0001a520: 3530 352d 3037 3239 5c22 3e3c 2f73 6372  505-0729\"></scr
-0001a530: 6970 743e 5c72 5c6e 3c73 6372 6970 740a  ipt>\r\n<script.
-0001a540: 2020 2020 2020 2020 7372 633d 5c22 2f6a          src=\"/j
-0001a550: 6174 656b 756b 6b6f 2f6a 732f 7361 6861  atekukko/js/saha
-0001a560: 732f 7769 6e64 6f77 732f 6372 6561 7465  s/windows/create
-0001a570: 2d6e 6577 2d75 7365 722d 7769 6e64 6f77  -new-user-window
-0001a580: 2e6a 733f 7469 6d65 7374 616d 703d 3230  .js?timestamp=20
-0001a590: 3233 3035 3035 2d30 3732 395c 223e 3c2f  230505-0729\"></
-0001a5a0: 7363 7269 7074 3e5c 725c 6e3c 7363 7269  script>\r\n<scri
-0001a5b0: 7074 0a20 2020 2020 2020 2073 7263 3d5c  pt.        src=\
-0001a5c0: 222f 6a61 7465 6b75 6b6b 6f2f 6a73 2f73  "/jatekukko/js/s
-0001a5d0: 6168 6173 2f77 696e 646f 7773 2f65 6d61  ahas/windows/ema
-0001a5e0: 696c 2d70 686f 6e65 2d77 696e 646f 772e  il-phone-window.
-0001a5f0: 6a73 3f74 696d 6573 7461 6d70 3d32 3032  js?timestamp=202
-0001a600: 3330 3530 352d 3037 3239 5c22 3e3c 2f73  30505-0729\"></s
-0001a610: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
-0001a620: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
-0001a630: 2f6a 6174 656b 756b 6b6f 2f6a 732f 7361  /jatekukko/js/sa
-0001a640: 6861 732f 7769 6e64 6f77 732f 6b69 6d70  has/windows/kimp
-0001a650: 616b 7369 2d77 696e 646f 772e 6a73 3f74  aksi-window.js?t
-0001a660: 696d 6573 7461 6d70 3d32 3032 3330 3530  imestamp=2023050
-0001a670: 352d 3037 3239 5c22 3e3c 2f73 6372 6970  5-0729\"></scrip
-0001a680: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
-0001a690: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
-0001a6a0: 656b 756b 6b6f 2f6a 732f 7361 6861 732f  ekukko/js/sahas/
-0001a6b0: 7769 6e64 6f77 732f 6f72 6465 722d 7769  windows/order-wi
-0001a6c0: 6e64 6f77 2e6a 733f 7469 6d65 7374 616d  ndow.js?timestam
-0001a6d0: 703d 3230 3233 3035 3035 2d30 3732 395c  p=20230505-0729\
-0001a6e0: 223e 3c2f 7363 7269 7074 3e5c 725c 6e3c  "></script>\r\n<
-0001a6f0: 7363 7269 7074 0a20 2020 2020 2020 2073  script.        s
-0001a700: 7263 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  rc=\"/jatekukko/
-0001a710: 6a73 2f73 6168 6173 2f77 696e 646f 7773  js/sahas/windows
-0001a720: 2f72 6573 6967 6e2d 6b69 6d70 7061 2d77  /resign-kimppa-w
-0001a730: 696e 646f 772e 6a73 3f74 696d 6573 7461  indow.js?timesta
-0001a740: 6d70 3d32 3032 3330 3530 352d 3037 3239  mp=20230505-0729
-0001a750: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
-0001a760: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
-0001a770: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
-0001a780: 2f6a 732f 7361 6861 732f 7769 6e64 6f77  /js/sahas/window
-0001a790: 732f 636f 6c6c 6563 7469 6f6e 2d73 6368  s/collection-sch
-0001a7a0: 6564 756c 652d 7769 6e64 6f77 2e6a 733f  edule-window.js?
-0001a7b0: 7469 6d65 7374 616d 703d 3230 3233 3035  timestamp=202305
-0001a7c0: 3035 2d30 3732 395c 223e 3c2f 7363 7269  05-0729\"></scri
-0001a7d0: 7074 3e5c 725c 6e5c 725c 6e5c 725c 6e5c  pt>\r\n\r\n\r\n\
-0001a7e0: 743c 7363 7269 7074 0a20 2020 2020 2020  t<script.       
-0001a7f0: 2073 7263 3d5c 222f 6a61 7465 6b75 6b6b   src=\"/jatekukk
-0001a800: 6f2f 6a73 2f73 6168 6173 2f77 696e 646f  o/js/sahas/windo
-0001a810: 7773 2f72 6570 7369 6b6b 612d 7769 6e64  ws/repsikka-wind
-0001a820: 6f77 2e6a 733f 7469 6d65 7374 616d 703d  ow.js?timestamp=
-0001a830: 3230 3233 3035 3035 2d30 3732 395c 223e  20230505-0729\">
-0001a840: 3c2f 7363 7269 7074 3e5c 725c 6e5c 725c  </script>\r\n\r\
-0001a850: 6e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  n\r\n\r\n\r\n\r\
-0001a860: 6e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  n\r\n\r\n\r\n\r\
-0001a870: 6e5c 743c 7363 7269 7074 0a20 2020 2020  n\t<script.     
-0001a880: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
-0001a890: 6b6b 6f2f 6a73 2f73 6168 6173 2f77 696e  kko/js/sahas/win
-0001a8a0: 646f 7773 2f77 6173 7465 2d77 6174 6572  dows/waste-water
-0001a8b0: 2d77 696e 646f 772e 6a73 3f74 696d 6573  -window.js?times
-0001a8c0: 7461 6d70 3d32 3032 3330 3530 352d 3037  tamp=20230505-07
-0001a8d0: 3239 5c22 3e3c 2f73 6372 6970 743e 5c72  29\"></script>\r
-0001a8e0: 5c6e 5c72 5c6e 5c72 5c6e 3c73 6372 6970  \n\r\n\r\n<scrip
-0001a8f0: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
-0001a900: 2f6a 6174 656b 756b 6b6f 2f6a 732f 636f  /jatekukko/js/co
-0001a910: 6d70 6f6e 656e 7473 2f74 6162 6261 722e  mponents/tabbar.
-0001a920: 6a73 3f74 696d 6573 7461 6d70 3d32 3032  js?timestamp=202
-0001a930: 3330 3530 352d 3037 3239 5c22 3e3c 2f73  30505-0729\"></s
-0001a940: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
-0001a950: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
-0001a960: 2f6a 6174 656b 756b 6b6f 2f6a 732f 636f  /jatekukko/js/co
-0001a970: 6d70 6f6e 656e 7473 2f74 6572 6d73 2d77  mponents/terms-w
-0001a980: 696e 646f 772e 6a73 3f74 696d 6573 7461  indow.js?timesta
-0001a990: 6d70 3d32 3032 3330 3530 352d 3037 3239  mp=20230505-0729
-0001a9a0: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
-0001a9b0: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
-0001a9c0: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
-0001a9d0: 2f6a 732f 636f 6d70 6f6e 656e 7473 2f74  /js/components/t
-0001a9e0: 6572 6d73 2d62 616e 6e65 722e 6a73 3f74  erms-banner.js?t
-0001a9f0: 696d 6573 7461 6d70 3d32 3032 3330 3530  imestamp=2023050
-0001aa00: 352d 3037 3239 5c22 3e3c 2f73 6372 6970  5-0729\"></scrip
-0001aa10: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
-0001aa20: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
-0001aa30: 656b 756b 6b6f 2f6a 732f 636f 6d70 6f6e  ekukko/js/compon
-0001aa40: 656e 7473 2f76 6964 656f 2d70 6f70 7570  ents/video-popup
-0001aa50: 2e6a 733f 7469 6d65 7374 616d 703d 3230  .js?timestamp=20
-0001aa60: 3233 3035 3035 2d30 3732 395c 223e 3c2f  230505-0729\"></
-0001aa70: 7363 7269 7074 3e5c 725c 6e5c 725c 6e5c  script>\r\n\r\n\
-0001aa80: 725c 6e5c 725c 6e3c 7363 7269 7074 0a20  r\n\r\n<script. 
-0001aa90: 2020 2020 2020 2074 7970 653d 5c22 7465         type=\"te
-0001aaa0: 7874 2f6a 6176 6173 6372 6970 745c 223e  xt/javascript\">
-0001aab0: 5c72 5c6e 5c74 7661 7220 6261 7365 7572  \r\n\tvar baseur
-0001aac0: 6c20 3d20 5c22 2f6a 6174 656b 756b 6b6f  l = \"/jatekukko
-0001aad0: 5c22 3b5c 725c 6e5c 725c 6e5c 7477 696e  \";\r\n\r\n\twin
-0001aae0: 646f 772e 6468 785f 676c 6f62 616c 496d  dow.dhx_globalIm
-0001aaf0: 6750 6174 680a 2020 2020 2020 2020 3d20  gPath.        = 
-0001ab00: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
-0001ab10: 6468 746d 6c78 5375 6974 652f 6468 746d  dhtmlxSuite/dhtm
-0001ab20: 6c78 436f 6d62 6f2f 636f 6465 6261 7365  lxCombo/codebase
-0001ab30: 2f69 6d67 732f 5c22 3b5c 725c 6e5c 725c  /imgs/\";\r\n\r\
-0001ab40: 6e5c 7473 6974 654c 616e 6775 6167 653d  n\tsiteLanguage=
-0001ab50: 0a20 2020 2020 2020 205c 2266 695f 4649  .        \"fi_FI
-0001ab60: 5c22 3b5c 725c 6e5c 745c 725c 6e5c 745c  \";\r\n\t\r\n\t\
-0001ab70: 725c 6e3c 2f73 6372 6970 743e 5c72 5c6e  r\n</script>\r\n
-0001ab80: 5c72 5c6e 3c73 6372 6970 7420 7372 633d  \r\n<script src=
-0001ab90: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
-0001aba0: 7361 6861 732f 6d61 696e 2e6a 733f 7469  sahas/main.js?ti
-0001abb0: 6d65 7374 616d 703d 3230 3233 3035 3035  mestamp=20230505
-0001abc0: 2d30 3732 395c 223e 3c2f 7363 7269 7074  -0729\"></script
-0001abd0: 3e5c 725c 6e5c 725c 6e5c 725c 6e3c 7363  >\r\n\r\n\r\n<sc
-0001abe0: 7269 7074 3e5c 725c 6e0a 2020 2020 2020  ript>\r\n.      
-0001abf0: 2020 5c20 2866 756e 6374 696f 6e28 692c    \ (function(i,
-0001ac00: 732c 6f2c 672c 722c 612c 6d29 7b69 5b27  s,o,g,r,a,m){i['
-0001ac10: 476f 6f67 6c65 416e 616c 7974 6963 734f  GoogleAnalyticsO
-0001ac20: 626a 6563 7427 5d3d 723b 695b 725d 3d69  bject']=r;i[r]=i
-0001ac30: 5b72 5d7c 7c66 756e 6374 696f 6e28 297b  [r]||function(){
-0001ac40: 5c72 5c6e 0a20 2020 2020 2020 205c 2028  \r\n.        \ (
-0001ac50: 695b 725d 2e71 3d69 5b72 5d2e 717c 7c5b  i[r].q=i[r].q||[
-0001ac60: 5d29 2e70 7573 6828 6172 6775 6d65 6e74  ]).push(argument
-0001ac70: 7329 7d2c 695b 725d 2e6c 3d31 2a6e 6577  s)},i[r].l=1*new
-0001ac80: 2044 6174 6528 293b 613d 732e 6372 6561   Date();a=s.crea
-0001ac90: 7465 456c 656d 656e 7428 6f29 2c5c 725c  teElement(o),\r\
-0001aca0: 6e0a 2020 2020 2020 2020 5c20 6d3d 732e  n.        \ m=s.
-0001acb0: 6765 7445 6c65 6d65 6e74 7342 7954 6167  getElementsByTag
-0001acc0: 4e61 6d65 286f 295b 305d 3b61 2e61 7379  Name(o)[0];a.asy
-0001acd0: 6e63 3d31 3b61 2e73 7263 3d67 3b6d 2e70  nc=1;a.src=g;m.p
-0001ace0: 6172 656e 744e 6f64 652e 696e 7365 7274  arentNode.insert
-0001acf0: 4265 666f 7265 2861 2c6d 295c 725c 6e0a  Before(a,m)\r\n.
-0001ad00: 2020 2020 2020 2020 5c20 7d29 2877 696e          \ })(win
-0001ad10: 646f 772c 646f 6375 6d65 6e74 2c27 7363  dow,document,'sc
-0001ad20: 7269 7074 272c 272f 2f77 7777 2e67 6f6f  ript','//www.goo
-0001ad30: 676c 652d 616e 616c 7974 6963 732e 636f  gle-analytics.co
-0001ad40: 6d2f 616e 616c 7974 6963 732e 6a73 272c  m/analytics.js',
-0001ad50: 2767 6127 293b 5c72 5c6e 5c72 5c6e 0a20  'ga');\r\n\r\n. 
-0001ad60: 2020 2020 2020 205c 2067 6128 2763 7265         \ ga('cre
-0001ad70: 6174 6527 2c20 2755 412d 3335 3935 3638  ate', 'UA-359568
-0001ad80: 3232 2d31 3127 2c20 2761 7574 6f27 293b  22-11', 'auto');
-0001ad90: 5c72 5c6e 2020 6761 2827 7365 6e64 272c  \r\n  ga('send',
-0001ada0: 2027 7061 6765 7669 6577 2729 3b5c 725c   'pageview');\r\
-0001adb0: 6e3c 2f73 6372 6970 743e 5c72 5c6e 5c72  n</script>\r\n\r
-0001adc0: 5c6e 5c72 5c6e 5c72 5c6e 0a20 2020 2020  \n\r\n\r\n.     
-0001add0: 2020 205c 2020 2020 2020 203c 7363 7269     \       <scri
-0001ade0: 7074 3e5c 725c 6e5c 745c 7424 2827 7365  pt>\r\n\t\t$('se
-0001adf0: 6374 696f 6e23 6c6f 6769 6e20 2e6e 6176  ction#login .nav
-0001ae00: 2d74 6162 7320 6127 292e 636c 6963 6b28  -tabs a').click(
-0001ae10: 6675 6e63 7469 6f6e 2028 6529 0a20 2020  function (e).   
-0001ae20: 2020 2020 207b 5c72 5c6e 5c74 5c74 2020       {\r\n\t\t  
-0001ae30: 652e 7072 6576 656e 7444 6566 6175 6c74  e.preventDefault
-0001ae40: 2829 5c72 5c6e 5c74 5c74 2020 2428 7468  ()\r\n\t\t  $(th
-0001ae50: 6973 292e 7461 6228 2773 686f 7727 295c  is).tab('show')\
-0001ae60: 725c 6e5c 745c 747d 293b 5c72 5c6e 5c74  r\n\t\t});\r\n\t
-0001ae70: 3c2f 7363 7269 7074 3e5c 725c 6e5c 725c  </script>\r\n\r\
-0001ae80: 6e0a 2020 2020 2020 2020 5c20 2020 3c73  n.        \   <s
-0001ae90: 6372 6970 743e 5c72 5c6e 2020 2020 2020  cript>\r\n      
-0001aea0: 2020 6966 2028 2161 7070 6c69 6361 7469    if (!applicati
-0001aeb0: 6f6e 2e69 7342 726f 7773 6572 436f 6d70  on.isBrowserComp
-0001aec0: 6174 6962 6c65 2829 2920 7b5c 725c 6e20  atible()) {\r\n 
-0001aed0: 2020 2020 2020 2020 2020 2024 2827 2362             $('#b
-0001aee0: 726f 7773 6572 2d69 6e63 6f6d 7061 7469  rowser-incompati
-0001aef0: 626c 652d 6d65 7373 6167 6527 292e 7368  ble-message').sh
-0001af00: 6f77 2829 3b5c 725c 6e0a 2020 2020 2020  ow();\r\n.      
-0001af10: 2020 5c20 2020 2020 2020 7d5c 725c 6e5c    \       }\r\n\
-0001af20: 725c 6e20 2020 2020 2020 2066 756e 6374  r\n        funct
-0001af30: 696f 6e20 7365 7442 6f64 7950 6164 6469  ion setBodyPaddi
-0001af40: 6e67 466f 7246 6f6f 7465 7228 2920 7b5c  ngForFooter() {\
-0001af50: 725c 6e20 2020 2020 2020 2020 2020 2076  r\n            v
-0001af60: 6172 0a20 2020 2020 2020 2066 6f6f 7465  ar.        foote
-0001af70: 7248 6569 6768 7420 3d20 2428 2762 6f64  rHeight = $('bod
-0001af80: 7920 3e20 666f 6f74 6572 2729 2e68 6569  y > footer').hei
-0001af90: 6768 7428 293b 5c72 5c6e 2020 2020 2020  ght();\r\n      
-0001afa0: 2020 2020 2020 2428 2762 6f64 7927 292e        $('body').
-0001afb0: 6373 7328 2770 6164 6469 6e67 2d62 6f74  css('padding-bot
-0001afc0: 746f 6d27 2c0a 2020 2020 2020 2020 666f  tom',.        fo
-0001afd0: 6f74 6572 4865 6967 6874 202b 2027 7078  oterHeight + 'px
-0001afe0: 2729 3b5c 725c 6e20 2020 2020 2020 207d  ');\r\n        }
-0001aff0: 5c72 5c6e 5c72 5c6e 2020 2020 2020 2020  \r\n\r\n        
-0001b000: 2428 7769 6e64 6f77 292e 6f6e 2827 7265  $(window).on('re
-0001b010: 7369 7a65 272c 2073 6574 426f 6479 5061  size', setBodyPa
-0001b020: 6464 696e 6746 6f72 466f 6f74 6572 293b  ddingForFooter);
-0001b030: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
-0001b040: 2020 2020 2073 6574 426f 6479 5061 6464       setBodyPadd
-0001b050: 696e 6746 6f72 466f 6f74 6572 2829 3b5c  ingForFooter();\
-0001b060: 725c 6e20 2020 203c 2f73 6372 6970 743e  r\n    </script>
-0001b070: 5c72 5c6e 5c72 5c6e 2020 2020 5c72 5c6e  \r\n\r\n    \r\n
-0001b080: 2020 2020 3c21 2d2d 0a20 2020 2020 2020      <!--.       
-0001b090: 2062 6567 696e 2053 6e61 7045 6e67 6167   begin SnapEngag
-0001b0a0: 6520 636f 6465 202d 2d3e 5c72 5c6e 2020  e code -->\r\n  
-0001b0b0: 2020 3c73 6372 6970 7420 7479 7065 3d5c    <script type=\
-0001b0c0: 2274 6578 742f 6a61 7661 7363 7269 7074  "text/javascript
-0001b0d0: 5c22 3e5c 725c 6e20 2020 2020 2020 2028  \">\r\n        (
-0001b0e0: 6675 6e63 7469 6f6e 2829 0a20 2020 2020  function().     
-0001b0f0: 2020 207b 5c72 5c6e 2020 2020 2020 2020     {\r\n        
-0001b100: 2020 2020 7661 7220 7365 203d 2064 6f63      var se = doc
-0001b110: 756d 656e 742e 6372 6561 7465 456c 656d  ument.createElem
-0001b120: 656e 7428 2773 6372 6970 7427 293b 2073  ent('script'); s
-0001b130: 652e 7479 7065 203d 2027 7465 7874 2f6a  e.type = 'text/j
-0001b140: 6176 6173 6372 6970 7427 3b0a 2020 2020  avascript';.    
-0001b150: 2020 2020 7365 2e61 7379 6e63 203d 2074      se.async = t
-0001b160: 7275 653b 5c72 5c6e 2020 2020 2020 2020  rue;\r\n        
-0001b170: 2020 2020 7365 2e73 7263 203d 2027 6874      se.src = 'ht
-0001b180: 7470 733a 2f2f 7374 6f72 6167 652e 676f  tps://storage.go
-0001b190: 6f67 6c65 6170 6973 2e63 6f6d 2f73 6e61  ogleapis.com/sna
-0001b1a0: 7065 6e67 6167 652d 6575 2f6a 732f 6339  pengage-eu/js/c9
-0001b1b0: 3065 3239 3661 2d39 6661 332d 3438 3739  0e296a-9fa3-4879
-0001b1c0: 2d61 3535 392d 6637 3461 6165 3665 3765  -a559-f74aae6e7e
-0001b1d0: 6334 2e6a 7327 3b5c 725c 6e0a 2020 2020  c4.js';\r\n.    
-0001b1e0: 2020 2020 5c20 2020 2020 2020 2020 2020      \           
-0001b1f0: 7661 7220 646f 6e65 203d 2066 616c 7365  var done = false
-0001b200: 3b5c 725c 6e20 2020 2020 2020 2020 2020  ;\r\n           
-0001b210: 2073 652e 6f6e 6c6f 6164 203d 2073 652e   se.onload = se.
-0001b220: 6f6e 7265 6164 7973 7461 7465 6368 616e  onreadystatechan
-0001b230: 6765 0a20 2020 2020 2020 203d 2066 756e  ge.        = fun
-0001b240: 6374 696f 6e28 2920 7b5c 725c 6e20 2020  ction() {\r\n   
-0001b250: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001b260: 2821 646f 6e65 2626 2821 7468 6973 2e72  (!done&&(!this.r
-0001b270: 6561 6479 5374 6174 657c 7c74 6869 732e  eadyState||this.
-0001b280: 7265 6164 7953 7461 7465 3d3d 3d27 6c6f  readyState==='lo
-0001b290: 6164 6564 277c 7c74 6869 732e 7265 6164  aded'||this.read
-0001b2a0: 7953 7461 7465 3d3d 3d27 636f 6d70 6c65  yState==='comple
-0001b2b0: 7465 2729 290a 2020 2020 2020 2020 7b5c  te')).        {\
-0001b2c0: 725c 6e20 2020 2020 2020 2020 2020 2020  r\n             
-0001b2d0: 2020 2020 2020 2064 6f6e 6520 3d20 7472         done = tr
-0001b2e0: 7565 3b5c 725c 6e20 2020 2020 2020 2020  ue;\r\n         
-0001b2f0: 2020 2020 2020 2020 2020 202f 2a20 506c             /* Pl
-0001b300: 6163 6520 796f 7572 0a20 2020 2020 2020  ace your.       
-0001b310: 2053 6e61 7045 6e67 6167 6520 4a53 2041   SnapEngage JS A
-0001b320: 5049 2063 6f64 6520 6265 6c6f 7720 2a2f  PI code below */
-0001b330: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
-0001b340: 2020 2020 2020 2020 2f2a 2053 6e61 7045          /* SnapE
-0001b350: 6e67 6167 652e 616c 6c6f 7743 6861 7453  ngage.allowChatS
-0001b360: 6f75 6e64 2874 7275 6529 3b0a 2020 2020  ound(true);.    
-0001b370: 2020 2020 4578 616d 706c 6520 4a53 2041      Example JS A
-0001b380: 5049 3a20 456e 6162 6c65 2073 6f75 6e64  PI: Enable sound
-0001b390: 7320 666f 7220 5669 7369 746f 7273 2e20  s for Visitors. 
-0001b3a0: 2a2f 5c72 5c6e 2020 2020 2020 2020 2020  */\r\n          
-0001b3b0: 2020 2020 2020 7d5c 725c 6e20 2020 2020        }\r\n     
-0001b3c0: 2020 2020 2020 207d 3b5c 725c 6e0a 2020         };\r\n.  
-0001b3d0: 2020 2020 2020 5c20 2020 2020 2020 2020        \         
-0001b3e0: 2020 7661 7220 7320 3d20 646f 6375 6d65    var s = docume
-0001b3f0: 6e74 2e67 6574 456c 656d 656e 7473 4279  nt.getElementsBy
-0001b400: 5461 674e 616d 6528 2773 6372 6970 7427  TagName('script'
-0001b410: 295b 305d 3b20 732e 7061 7265 6e74 4e6f  )[0]; s.parentNo
-0001b420: 6465 2e69 6e73 6572 7442 6566 6f72 6528  de.insertBefore(
-0001b430: 7365 2c0a 2020 2020 2020 2020 7329 3b5c  se,.        s);\
-0001b440: 725c 6e20 2020 2020 2020 207d 2928 293b  r\n        })();
-0001b450: 5c72 5c6e 2020 2020 3c2f 7363 7269 7074  \r\n    </script
-0001b460: 3e5c 725c 6e20 2020 203c 212d 2d20 656e  >\r\n    <!-- en
-0001b470: 6420 536e 6170 456e 6761 6765 2063 6f64  d SnapEngage cod
-0001b480: 6520 2d2d 3e5c 725c 6e0a 2020 2020 2020  e -->\r\n.      
-0001b490: 2020 5c20 2020 5c72 5c6e 2020 2020 5c72    \   \r\n    \r
-0001b4a0: 5c6e 2020 2020 3c2f 626f 6479 3e5c 725c  \n    </body>\r\
-0001b4b0: 6e20 2020 203c 2f68 746d 6c3e 5c72 5c6e  n    </html>\r\n
-0001b4c0: 5c72 5c6e 220a 2020 2020 6865 6164 6572  \r\n".    header
-0001b4d0: 733a 0a20 2020 2020 2043 6f6e 6e65 6374  s:.      Connect
-0001b4e0: 696f 6e3a 0a20 2020 2020 202d 206b 6565  ion:.      - kee
-0001b4f0: 702d 616c 6976 650a 2020 2020 2020 436f  p-alive.      Co
-0001b500: 6e74 656e 742d 456e 636f 6469 6e67 3a0a  ntent-Encoding:.
-0001b510: 2020 2020 2020 2d20 677a 6970 0a20 2020        - gzip.   
-0001b520: 2020 2043 6f6e 7465 6e74 2d4c 616e 6775     Content-Langu
-0001b530: 6167 653a 0a20 2020 2020 202d 2066 692d  age:.      - fi-
-0001b540: 4649 0a20 2020 2020 2043 6f6e 7465 6e74  FI.      Content
-0001b550: 2d53 6563 7572 6974 792d 506f 6c69 6379  -Security-Policy
-0001b560: 3a0a 2020 2020 2020 2d20 6672 616d 652d  :.      - frame-
-0001b570: 616e 6365 7374 6f72 7320 276e 6f6e 6527  ancestors 'none'
-0001b580: 0a20 2020 2020 2043 6f6e 7465 6e74 2d54  .      Content-T
-0001b590: 7970 653a 0a20 2020 2020 202d 2074 6578  ype:.      - tex
-0001b5a0: 742f 6874 6d6c 3b63 6861 7273 6574 3d75  t/html;charset=u
-0001b5b0: 7466 2d38 0a20 2020 2020 2044 6174 653a  tf-8.      Date:
-0001b5c0: 0a20 2020 2020 202d 2046 7269 2c20 3236  .      - Fri, 26
-0001b5d0: 204d 6179 2032 3032 3320 3037 3a35 383a   May 2023 07:58:
-0001b5e0: 3037 2047 4d54 0a20 2020 2020 2053 6572  07 GMT.      Ser
-0001b5f0: 7665 723a 0a20 2020 2020 202d 206e 6769  ver:.      - ngi
-0001b600: 6e78 0a20 2020 2020 2053 7472 6963 742d  nx.      Strict-
-0001b610: 5472 616e 7370 6f72 742d 5365 6375 7269  Transport-Securi
-0001b620: 7479 3a0a 2020 2020 2020 2d20 6d61 782d  ty:.      - max-
-0001b630: 6167 653d 3633 3037 3230 3030 0a20 2020  age=63072000.   
-0001b640: 2020 2054 7261 6e73 6665 722d 456e 636f     Transfer-Enco
-0001b650: 6469 6e67 3a0a 2020 2020 2020 2d20 6368  ding:.      - ch
-0001b660: 756e 6b65 640a 2020 2020 2020 582d 4672  unked.      X-Fr
-0001b670: 616d 652d 4f70 7469 6f6e 733a 0a20 2020  ame-Options:.   
-0001b680: 2020 202d 2044 454e 590a 2020 2020 2020     - DENY.      
-0001b690: 582d 506f 7765 7265 642d 4279 3a0a 2020  X-Powered-By:.  
-0001b6a0: 2020 2020 2d20 2753 6572 766c 6574 2f34      - 'Servlet/4
-0001b6b0: 2e30 204a 5350 2f32 2e33 2028 5061 7961  .0 JSP/2.3 (Paya
-0001b6c0: 7261 2053 6572 7665 7220 2035 2e32 3032  ra Server  5.202
-0001b6d0: 322e 3520 2362 6164 6173 7366 6973 6820  2.5 #badassfish 
-0001b6e0: 4a61 7661 2f45 636c 6970 7365 204f 7065  Java/Eclipse Ope
-0001b6f0: 6e4a 392f 312e 3829 270a 2020 2020 7374  nJ9/1.8)'.    st
-0001b700: 6174 7573 3a0a 2020 2020 2020 636f 6465  atus:.      code
-0001b710: 3a20 3230 300a 2020 2020 2020 6d65 7373  : 200.      mess
-0001b720: 6167 653a 204f 4b0a 2020 2020 7572 6c3a  age: OK.    url:
-0001b730: 2068 7474 7073 3a2f 2f74 696c 6173 746f   https://tilasto
-0001b740: 2e6a 6174 656b 756b 6b6f 2e66 692f 6a61  .jatekukko.fi/ja
-0001b750: 7465 6b75 6b6b 6f2f 7361 6861 732e 6a73  tekukko/sahas.js
-0001b760: 700a 7665 7273 696f 6e3a 2031 0a         p.version: 1.
+00016290: 3c62 7574 746f 6e20 636c 6173 733d 5c22  <button class=\"
+000162a0: 6274 6e0a 2020 2020 2020 2020 6274 6e2d  btn.        btn-
+000162b0: 7072 696d 6172 795c 2220 6461 7461 2d61  primary\" data-a
+000162c0: 6374 696f 6e3d 5c22 6578 6974 5c22 3e50  ction=\"exit\">P
+000162d0: 6f69 7374 753c 2f62 7574 746f 6e3e 5c72  oistu</button>\r
+000162e0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+000162f0: 2020 3c2f 6469 763e 5c72 5c6e 0a20 2020    </div>\r\n.   
+00016300: 2020 2020 205c 2020 2020 2020 2020 2020       \          
+00016310: 203c 2f64 6976 3e5c 725c 6e20 2020 2020   </div>\r\n     
+00016320: 2020 203c 2f64 6976 3e5c 725c 6e20 2020     </div>\r\n   
+00016330: 203c 2f64 6976 3e5c 725c 6e3c 2f64 6976   </div>\r\n</div
+00016340: 3e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  >\r\n\r\n\r\n\r\
+00016350: 6e3c 7363 7269 7074 0a20 2020 2020 2020  n<script.       
+00016360: 2069 643d 5c22 696e 766f 6963 652d 6465   id=\"invoice-de
+00016370: 7461 696c 732d 7465 6d70 6c61 7465 5c22  tails-template\"
+00016380: 2074 7970 653d 5c22 7465 7874 2f78 2d6b   type=\"text/x-k
+00016390: 656e 646f 2d74 656d 706c 6174 655c 223e  endo-template\">
+000163a0: 5c72 5c6e 5c72 5c6e 5c72 5c6e 3c74 643e  \r\n\r\n\r\n<td>
+000163b0: 3c2f 7464 3e5c 725c 6e3c 7464 0a20 2020  </td>\r\n<td.   
+000163c0: 2020 2020 2063 6f6c 7370 616e 3d5c 2238       colspan=\"8
+000163d0: 5c22 3e5c 725c 6e5c 743c 6172 7469 636c  \">\r\n\t<articl
+000163e0: 6520 636c 6173 733d 5c22 696e 766f 6963  e class=\"invoic
+000163f0: 652d 6465 7461 696c 735c 223e 5c72 5c6e  e-details\">\r\n
+00016400: 5c74 5c74 3c74 6162 6c65 2063 6c61 7373  \t\t<table class
+00016410: 3d5c 2274 6162 6c65 5c22 3e5c 725c 6e5c  =\"table\">\r\n\
+00016420: 745c 745c 743c 7472 3e5c 725c 6e5c 745c  t\t\t<tr>\r\n\t\
+00016430: 745c 745c 743c 7468 3e53 5c78 4534 696c  t\t\t<th>S\xE4il
+00016440: 695c 7846 363c 2f74 683e 5c72 5c6e 5c74  i\xF6</th>\r\n\t
+00016450: 5c74 5c74 5c74 3c74 683e 4e6f 7574 6f61  \t\t\t<th>Noutoa
+00016460: 696b 613c 2f74 683e 5c72 5c6e 5c74 5c74  ika</th>\r\n\t\t
+00016470: 5c74 5c74 3c74 683e 5061 6c76 656c 756e  \t\t<th>Palvelun
+00016480: 0a20 2020 2020 2020 2073 756f 7269 7474  .        suoritt
+00016490: 616a 613c 2f74 683e 5c72 5c6e 5c74 5c74  aja</th>\r\n\t\t
+000164a0: 5c74 5c74 3c74 683e 5661 7374 6561 696b  \t\t<th>Vasteaik
+000164b0: 613c 2f74 683e 5c72 5c6e 5c74 5c74 5c74  a</th>\r\n\t\t\t
+000164c0: 3c2f 7472 3e5c 725c 6e5c 745c 745c 743c  </tr>\r\n\t\t\t<
+000164d0: 7472 3e5c 725c 6e5c 745c 745c 745c 743c  tr>\r\n\t\t\t\t<
+000164e0: 7464 3e23 3a0a 2020 2020 2020 2020 7369  td>#:.        si
+000164f0: 676e 6174 7572 652e 6269 6e20 233c 2f74  gnature.bin #</t
+00016500: 643e 5c72 5c6e 5c74 5c74 5c74 5c74 3c74  d>\r\n\t\t\t\t<t
+00016510: 643e 233a 206b 656e 646f 2e74 6f53 7472  d>#: kendo.toStr
+00016520: 696e 6728 6b65 6e64 6f2e 7061 7273 6544  ing(kendo.parseD
+00016530: 6174 6528 7369 676e 6174 7572 652e 7069  ate(signature.pi
+00016540: 636b 7570 4461 7465 292c 0a20 2020 2020  ckupDate),.     
+00016550: 2020 2027 6727 2920 233c 2f74 643e 5c72     'g') #</td>\r
+00016560: 5c6e 5c74 5c74 5c74 5c74 3c74 643e 233a  \n\t\t\t\t<td>#:
+00016570: 2073 6967 6e61 7475 7265 2e65 7865 6375   signature.execu
+00016580: 7465 7220 3f20 7369 676e 6174 7572 652e  ter ? signature.
+00016590: 6578 6563 7574 6572 203a 2027 270a 2020  executer : ''.  
+000165a0: 2020 2020 2020 233c 2f74 643e 5c72 5c6e        #</td>\r\n
+000165b0: 5c74 5c74 5c74 5c74 3c74 643e 3c2f 7464  \t\t\t\t<td></td
+000165c0: 3e5c 725c 6e5c 745c 745c 743c 2f74 723e  >\r\n\t\t\t</tr>
+000165d0: 5c72 5c6e 5c72 5c6e 5c74 5c74 5c74 3c74  \r\n\r\n\t\t\t<t
+000165e0: 723e 5c72 5c6e 5c74 5c74 5c74 5c74 3c74  r>\r\n\t\t\t\t<t
+000165f0: 683e 5246 4944 3c2f 7468 3e5c 725c 6e5c  h>RFID</th>\r\n\
+00016600: 745c 745c 745c 743c 7468 3e56 6173 7461  t\t\t\t<th>Vasta
+00016610: 616e 6f74 746f 6169 6b61 3c2f 7468 3e5c  anottoaika</th>\
+00016620: 725c 6e5c 745c 745c 745c 743c 7468 3e50  r\n\t\t\t\t<th>P
+00016630: 7572 6b61 6a61 3c2f 7468 3e5c 725c 6e5c  urkaja</th>\r\n\
+00016640: 745c 745c 745c 743c 7468 3e3c 2f74 683e  t\t\t\t<th></th>
+00016650: 5c72 5c6e 5c74 5c74 5c74 3c2f 7472 3e5c  \r\n\t\t\t</tr>\
+00016660: 725c 6e5c 745c 745c 743c 7472 3e5c 725c  r\n\t\t\t<tr>\r\
+00016670: 6e5c 745c 745c 745c 743c 7464 3e23 3a0a  n\t\t\t\t<td>#:.
+00016680: 2020 2020 2020 2020 7369 676e 6174 7572          signatur
+00016690: 652e 7266 6964 203f 2073 6967 6e61 7475  e.rfid ? signatu
+000166a0: 7265 2e72 6669 6420 3a20 2727 2023 3c2f  re.rfid : '' #</
+000166b0: 7464 3e5c 725c 6e5c 745c 745c 745c 743c  td>\r\n\t\t\t\t<
+000166c0: 7464 3e23 3a20 7369 676e 6174 7572 652e  td>#: signature.
+000166d0: 7265 6365 6976 6544 6174 650a 2020 2020  receiveDate.    
+000166e0: 2020 2020 3f20 6b65 6e64 6f2e 746f 5374      ? kendo.toSt
+000166f0: 7269 6e67 286b 656e 646f 2e70 6172 7365  ring(kendo.parse
+00016700: 4461 7465 2873 6967 6e61 7475 7265 2e72  Date(signature.r
+00016710: 6563 6569 7665 4461 7465 292c 2027 6727  eceiveDate), 'g'
+00016720: 2920 3a20 2727 2023 3c2f 7464 3e5c 725c  ) : '' #</td>\r\
+00016730: 6e5c 745c 745c 745c 743c 7464 3e23 3a0a  n\t\t\t\t<td>#:.
+00016740: 2020 2020 2020 2020 7369 676e 6174 7572          signatur
+00016750: 652e 756e 6c6f 6164 6572 203f 2073 6967  e.unloader ? sig
+00016760: 6e61 7475 7265 2e75 6e6c 6f61 6465 7220  nature.unloader 
+00016770: 3a20 2727 2023 3c2f 7464 3e5c 725c 6e5c  : '' #</td>\r\n\
+00016780: 745c 745c 745c 743c 7464 3e23 3a20 666f  t\t\t\t<td>#: fo
+00016790: 726d 6174 496e 7465 7276 616c 2873 6967  rmatInterval(sig
+000167a0: 6e61 7475 7265 2e74 696d 6554 6f55 6e6c  nature.timeToUnl
+000167b0: 6f61 6429 0a20 2020 2020 2020 2023 3c2f  oad).        #</
+000167c0: 7464 3e5c 725c 6e5c 745c 745c 743c 2f74  td>\r\n\t\t\t</t
+000167d0: 723e 5c72 5c6e 5c72 5c6e 5c74 5c74 5c74  r>\r\n\r\n\t\t\t
+000167e0: 3c74 723e 5c72 5c6e 5c74 5c74 5c74 5c74  <tr>\r\n\t\t\t\t
+000167f0: 3c74 683e 5475 686f 7573 746f 6469 7374  <th>Tuhoustodist
+00016800: 7573 3c2f 7468 3e5c 725c 6e5c 745c 745c  us</th>\r\n\t\t\
+00016810: 745c 743c 7468 3e54 7568 6f75 7361 696b  t\t<th>Tuhousaik
+00016820: 613c 2f74 683e 5c72 5c6e 5c74 5c74 5c74  a</th>\r\n\t\t\t
+00016830: 5c74 3c74 683e 5661 7374 7575 6c6c 696e  \t<th>Vastuullin
+00016840: 656e 0a20 2020 2020 2020 2074 7568 6f61  en.        tuhoa
+00016850: 6a61 3c2f 7468 3e5c 725c 6e5c 745c 745c  ja</th>\r\n\t\t\
+00016860: 745c 743c 7468 3e3c 2f74 683e 5c72 5c6e  t\t<th></th>\r\n
+00016870: 5c74 5c74 5c74 3c2f 7472 3e5c 725c 6e5c  \t\t\t</tr>\r\n\
+00016880: 745c 745c 743c 7472 3e5c 725c 6e5c 745c  t\t\t<tr>\r\n\t\
+00016890: 745c 745c 743c 7464 3e23 3a0a 2020 2020  t\t\t<td>#:.    
+000168a0: 2020 2020 7369 676e 6174 7572 652e 7461      signature.ta
+000168b0: 736b 4964 2023 3c2f 7464 3e5c 725c 6e5c  skId #</td>\r\n\
+000168c0: 745c 745c 745c 743c 7464 3e23 3a20 7369  t\t\t\t<td>#: si
+000168d0: 676e 6174 7572 652e 6465 7374 726f 7944  gnature.destroyD
+000168e0: 6174 6520 3f20 6b65 6e64 6f2e 746f 5374  ate ? kendo.toSt
+000168f0: 7269 6e67 286b 656e 646f 2e70 6172 7365  ring(kendo.parse
+00016900: 4461 7465 2873 6967 6e61 7475 7265 2e64  Date(signature.d
+00016910: 6573 7472 6f79 4461 7465 292c 0a20 2020  estroyDate),.   
+00016920: 2020 2020 2027 6727 2920 3a20 2727 2023       'g') : '' #
+00016930: 3c2f 7464 3e5c 725c 6e5c 745c 745c 745c  </td>\r\n\t\t\t\
+00016940: 743c 7464 3e23 3a20 7369 676e 6174 7572  t<td>#: signatur
+00016950: 652e 6465 7374 726f 7965 7220 3f20 7369  e.destroyer ? si
+00016960: 676e 6174 7572 652e 6465 7374 726f 7965  gnature.destroye
+00016970: 720a 2020 2020 2020 2020 3a20 2727 2023  r.        : '' #
+00016980: 3c2f 7464 3e5c 725c 6e5c 745c 745c 745c  </td>\r\n\t\t\t\
+00016990: 743c 7464 3e23 3a20 666f 726d 6174 496e  t<td>#: formatIn
+000169a0: 7465 7276 616c 2873 6967 6e61 7475 7265  terval(signature
+000169b0: 2e74 696d 6554 6f44 6573 7472 6f79 2920  .timeToDestroy) 
+000169c0: 233c 2f74 643e 5c72 5c6e 5c74 5c74 5c74  #</td>\r\n\t\t\t
+000169d0: 3c2f 7472 3e5c 725c 6e5c 725c 6e5c 745c  </tr>\r\n\r\n\t\
+000169e0: 745c 743c 7472 3e5c 725c 6e5c 745c 745c  t\t<tr>\r\n\t\t\
+000169f0: 745c 743c 7468 3e4d 6174 6572 6961 616c  t\t<th>Materiaal
+00016a00: 693c 2f74 683e 5c72 5c6e 5c74 5c74 5c74  i</th>\r\n\t\t\t
+00016a10: 5c74 5c72 5c6e 5c74 5c74 5c74 5c74 3c74  \t\r\n\t\t\t\t<t
+00016a20: 680a 2020 2020 2020 2020 636f 6c73 7061  h.        colspa
+00016a30: 6e3d 5c22 335c 223e 4875 6f6d 3c2f 7468  n=\"3\">Huom</th
+00016a40: 3e5c 725c 6e5c 745c 745c 745c 745c 725c  >\r\n\t\t\t\t\r\
+00016a50: 6e5c 745c 745c 743c 2f74 723e 5c72 5c6e  n\t\t\t</tr>\r\n
+00016a60: 5c74 5c74 5c74 3c74 723e 5c72 5c6e 5c74  \t\t\t<tr>\r\n\t
+00016a70: 5c74 5c74 5c74 3c74 643e 233a 0a20 2020  \t\t\t<td>#:.   
+00016a80: 2020 2020 2073 6967 6e61 7475 7265 2e6d       signature.m
+00016a90: 6174 6572 6961 6c20 233c 2f74 643e 5c72  aterial #</td>\r
+00016aa0: 5c6e 5c74 5c74 5c74 5c74 5c72 5c6e 5c74  \n\t\t\t\t\r\n\t
+00016ab0: 5c74 5c74 5c74 3c74 6420 636f 6c73 7061  \t\t\t<td colspa
+00016ac0: 6e3d 5c22 335c 2220 726f 7773 7061 6e3d  n=\"3\" rowspan=
+00016ad0: 5c22 335c 223e 233a 0a20 2020 2020 2020  \"3\">#:.       
+00016ae0: 2073 6967 6e61 7475 7265 2e63 6f6d 6d65   signature.comme
+00016af0: 6e74 2023 3c2f 7464 3e5c 725c 6e5c 745c  nt #</td>\r\n\t\
+00016b00: 745c 745c 745c 725c 6e5c 745c 745c 743c  t\t\t\r\n\t\t\t<
+00016b10: 2f74 723e 5c72 5c6e 5c72 5c6e 5c74 5c74  /tr>\r\n\r\n\t\t
+00016b20: 5c74 3c74 723e 5c72 5c6e 5c74 5c74 5c74  \t<tr>\r\n\t\t\t
+00016b30: 5c74 3c74 683e 6b67 2f6b 706c 3c2f 7468  \t<th>kg/kpl</th
+00016b40: 3e5c 725c 6e5c 745c 745c 743c 2f74 723e  >\r\n\t\t\t</tr>
+00016b50: 5c72 5c6e 5c74 5c74 5c74 3c74 723e 5c72  \r\n\t\t\t<tr>\r
+00016b60: 5c6e 5c74 5c74 5c74 5c74 3c74 643e 233a  \n\t\t\t\t<td>#:
+00016b70: 0a20 2020 2020 2020 2073 6967 6e61 7475  .        signatu
+00016b80: 7265 2e61 6d6f 756e 7420 3f20 7369 676e  re.amount ? sign
+00016b90: 6174 7572 652e 616d 6f75 6e74 203a 2027  ature.amount : '
+00016ba0: 2720 233c 2f74 643e 5c72 5c6e 5c74 5c74  ' #</td>\r\n\t\t
+00016bb0: 5c74 3c2f 7472 3e5c 725c 6e5c 745c 743c  \t</tr>\r\n\t\t<
+00016bc0: 2f74 6162 6c65 3e5c 725c 6e5c 743c 2f61  /table>\r\n\t</a
+00016bd0: 7274 6963 6c65 3e5c 725c 6e3c 2f74 643e  rticle>\r\n</td>
+00016be0: 5c72 5c6e 3c2f 7363 7269 7074 3e5c 725c  \r\n</script>\r\
+00016bf0: 6e0a 2020 2020 2020 2020 5c20 2020 3c2f  n.        \   </
+00016c00: 6469 763e 5c72 5c6e 5c72 5c6e 2020 2020  div>\r\n\r\n    
+00016c10: 3c66 6f6f 7465 723e 5c72 5c6e 5c74 3c64  <footer>\r\n\t<d
+00016c20: 6976 3e5c 725c 6e5c 745c 743c 6469 7620  iv>\r\n\t\t<div 
+00016c30: 636c 6173 733d 5c22 636f 6e74 6169 6e65  class=\"containe
+00016c40: 725c 223e 5c72 5c6e 5c74 5c74 5c74 3c64  r\">\r\n\t\t\t<d
+00016c50: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+00016c60: 3d5c 2272 6f77 5c22 3e5c 725c 6e5c 745c  =\"row\">\r\n\t\
+00016c70: 745c 745c 743c 6469 7620 636c 6173 733d  t\t\t<div class=
+00016c80: 5c22 636f 6c2d 736d 2d34 2063 6f6c 2d6d  \"col-sm-4 col-m
+00016c90: 642d 345c 223e 5c72 5c6e 5c74 5c74 5c74  d-4\">\r\n\t\t\t
+00016ca0: 5c74 5c74 3c61 6464 7265 7373 3e5c 725c  \t\t<address>\r\
+00016cb0: 6e5c 745c 745c 745c 745c 745c 744a 5c78  n\t\t\t\t\t\tJ\x
+00016cc0: 4534 7465 6b75 6b6b 6f0a 2020 2020 2020  E4tekukko.      
+00016cd0: 2020 4f79 3c62 723e 5c72 5c6e 5c74 5c74    Oy<br>\r\n\t\t
+00016ce0: 5c74 5c74 5c74 5c74 5c72 5c6e 5c74 5c74  \t\t\t\t\r\n\t\t
+00016cf0: 5c74 5c74 5c74 3c2f 6164 6472 6573 733e  \t\t\t</address>
+00016d00: 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f 6469  \r\n\t\t\t\t</di
+00016d10: 763e 5c72 5c6e 5c74 5c74 5c74 5c74 3c64  v>\r\n\t\t\t\t<d
+00016d20: 6976 0a20 2020 2020 2020 2063 6c61 7373  iv.        class
+00016d30: 3d5c 2263 6f6c 2d73 6d2d 3420 636f 6c2d  =\"col-sm-4 col-
+00016d40: 6d64 2d34 5c22 3e5c 725c 6e5c 745c 745c  md-4\">\r\n\t\t\
+00016d50: 745c 745c 7441 7369 616b 6173 7061 6c76  t\t\tAsiakaspalv
+00016d60: 656c 7520 5c75 3230 3232 2030 3137 2033  elu \u2022 017 3
+00016d70: 3638 3020 3135 320a 2020 2020 2020 2020  680 152.        
+00016d80: 5c75 3230 3232 2061 7369 616b 6173 7061  \u2022 asiakaspa
+00016d90: 6c76 656c 7540 6a61 7465 6b75 6b6b 6f2e  lvelu@jatekukko.
+00016da0: 6669 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f  fi\r\n\t\t\t\t</
+00016db0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 5c74  div>\r\n\t\t\t\t
+00016dc0: 3c64 6976 2063 6c61 7373 3d5c 2263 6f6c  <div class=\"col
+00016dd0: 2d73 6d2d 330a 2020 2020 2020 2020 636f  -sm-3.        co
+00016de0: 6c2d 6d64 2d33 5c22 3e5c 725c 6e5c 745c  l-md-3\">\r\n\t\
+00016df0: 745c 745c 745c 745c 725c 6e5c 745c 745c  t\t\t\t\r\n\t\t\
+00016e00: 745c 745c 745c 745c 725c 6e5c 745c 745c  t\t\t\t\r\n\t\t\
+00016e10: 745c 745c 745c 745c 725c 6e5c 745c 745c  t\t\t\t\r\n\t\t\
+00016e20: 745c 745c 745c 745c 725c 6e5c 745c 745c  t\t\t\t\r\n\t\t\
+00016e30: 745c 745c 745c 725c 6e5c 745c 745c 745c  t\t\t\r\n\t\t\t\
+00016e40: 745c 745c 725c 6e5c 745c 745c 745c 745c  t\t\r\n\t\t\t\t\
+00016e50: 745c 745c 725c 6e5c 745c 745c 745c 745c  t\t\r\n\t\t\t\t\
+00016e60: 745c 745c 725c 6e5c 745c 745c 745c 745c  t\t\r\n\t\t\t\t\
+00016e70: 745c 745c 725c 6e5c 745c 745c 745c 745c  t\t\r\n\t\t\t\t\
+00016e80: 745c 725c 6e5c 745c 745c 745c 743c 2f64  t\r\n\t\t\t\t</d
+00016e90: 6976 3e5c 725c 6e5c 745c 745c 743c 2f64  iv>\r\n\t\t\t</d
+00016ea0: 6976 3e5c 725c 6e5c 745c 745c 745c 725c  iv>\r\n\t\t\t\r\
+00016eb0: 6e5c 745c 745c 745c 725c 6e5c 745c 745c  n\t\t\t\r\n\t\t\
+00016ec0: 745c 725c 6e5c 745c 745c 745c 725c 6e5c  t\r\n\t\t\t\r\n\
+00016ed0: 745c 743c 2f64 6976 3e5c 725c 6e5c 743c  t\t</div>\r\n\t<
+00016ee0: 2f64 6976 3e5c 725c 6e5c 725c 6e5c 743c  /div>\r\n\r\n\t<
+00016ef0: 6469 763e 5c72 5c6e 5c74 5c74 3c64 6976  div>\r\n\t\t<div
+00016f00: 0a20 2020 2020 2020 2063 6c61 7373 3d5c  .        class=\
+00016f10: 2263 6f6e 7461 696e 6572 5c22 3e5c 725c  "container\">\r\
+00016f20: 6e5c 745c 745c 743c 6469 7620 636c 6173  n\t\t\t<div clas
+00016f30: 733d 5c22 726f 775c 223e 5c72 5c6e 5c74  s=\"row\">\r\n\t
+00016f40: 5c74 5c74 5c74 3c64 6976 2063 6c61 7373  \t\t\t<div class
+00016f50: 3d5c 2263 6f6c 2d73 6d2d 360a 2020 2020  =\"col-sm-6.    
+00016f60: 2020 2020 636f 6c2d 6d64 2d36 5c22 3e5c      col-md-6\">\
+00016f70: 725c 6e5c 745c 745c 745c 745c 7420 4a5c  r\n\t\t\t\t\t J\
+00016f80: 7845 3474 656b 756b 6b6f 204f 795c 725c  xE4tekukko Oy\r\
+00016f90: 6e5c 745c 745c 745c 743c 2f64 6976 3e5c  n\t\t\t\t</div>\
+00016fa0: 725c 6e5c 745c 745c 745c 743c 6469 760a  r\n\t\t\t\t<div.
+00016fb0: 2020 2020 2020 2020 636c 6173 733d 5c22          class=\"
+00016fc0: 636f 6c2d 736d 2d36 2063 6f6c 2d6d 642d  col-sm-6 col-md-
+00016fd0: 365c 223e 5c72 5c6e 5c74 5c74 5c74 5c74  6\">\r\n\t\t\t\t
+00016fe0: 5c74 5c72 5c6e 5c74 5c74 5c74 5c74 3c2f  \t\r\n\t\t\t\t</
+00016ff0: 6469 763e 5c72 5c6e 5c74 5c74 5c74 3c2f  div>\r\n\t\t\t</
+00017000: 6469 763e 5c72 5c6e 5c74 5c74 3c2f 6469  div>\r\n\t\t</di
+00017010: 763e 5c72 5c6e 5c74 3c2f 6469 763e 5c72  v>\r\n\t</div>\r
+00017020: 5c6e 3c2f 666f 6f74 6572 3e5c 725c 6e5c  \n</footer>\r\n\
+00017030: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00017040: 3c21 2d2d 204a 5175 6572 7920 2d2d 3e5c  <!-- JQuery -->\
+00017050: 725c 6e3c 7363 7269 7074 2073 7263 3d5c  r\n<script src=\
+00017060: 222f 2f61 6a61 782e 676f 6f67 6c65 6170  "//ajax.googleap
+00017070: 6973 2e63 6f6d 2f61 6a61 782f 6c69 6273  is.com/ajax/libs
+00017080: 2f6a 7175 6572 792f 312e 3132 2e34 2f6a  /jquery/1.12.4/j
+00017090: 7175 6572 792e 6d69 6e2e 6a73 5c22 3e3c  query.min.js\"><
+000170a0: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
+000170b0: 6970 743e 7769 6e64 6f77 2e6a 5175 6572  ipt>window.jQuer
+000170c0: 790a 2020 2020 2020 2020 7c7c 2064 6f63  y.        || doc
+000170d0: 756d 656e 742e 7772 6974 6528 273c 7363  ument.write('<sc
+000170e0: 7269 7074 2073 7263 3d5c 226a 732f 7665  ript src=\"js/ve
+000170f0: 6e64 6f72 2f6a 7175 6572 792d 312e 3130  ndor/jquery-1.10
+00017100: 2e32 2e6d 696e 2e6a 735c 223e 3c5c 5c2f  .2.min.js\"><\\/
+00017110: 7363 7269 7074 3e27 293c 2f73 6372 6970  script>')</scrip
+00017120: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
+00017130: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
+00017140: 656b 756b 6b6f 2f6a 732f 6a71 7565 7279  ekukko/js/jquery
+00017150: 2e76 616c 6964 6174 652e 6d69 6e2e 6a73  .validate.min.js
+00017160: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
+00017170: 3c73 6372 6970 7420 7372 633d 5c22 2f6a  <script src=\"/j
+00017180: 6174 656b 756b 6b6f 2f6a 732f 6a71 7565  atekukko/js/jque
+00017190: 7279 2e6e 756d 6265 722e 6d69 6e2e 6a73  ry.number.min.js
+000171a0: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
+000171b0: 5c72 5c6e 3c21 2d2d 0a20 2020 2020 2020  \r\n<!--.       
+000171c0: 204a 5175 6572 7920 476c 6f62 616c 697a   JQuery Globaliz
+000171d0: 6520 2d2d 3e5c 725c 6e3c 7363 7269 7074  e -->\r\n<script
+000171e0: 2073 7263 3d5c 222f 6a61 7465 6b75 6b6b   src=\"/jatekukk
+000171f0: 6f2f 6a73 2f67 6c6f 6261 6c69 7a65 2f63  o/js/globalize/c
+00017200: 6c64 722e 6a73 5c22 3e3c 2f73 6372 6970  ldr.js\"></scrip
+00017210: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
+00017220: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
+00017230: 656b 756b 6b6f 2f6a 732f 676c 6f62 616c  ekukko/js/global
+00017240: 697a 652f 636c 6472 2f65 7665 6e74 2e6a  ize/cldr/event.j
+00017250: 735c 223e 3c2f 7363 7269 7074 3e5c 725c  s\"></script>\r\
+00017260: 6e3c 7363 7269 7074 2073 7263 3d5c 222f  n<script src=\"/
+00017270: 6a61 7465 6b75 6b6b 6f2f 6a73 2f67 6c6f  jatekukko/js/glo
+00017280: 6261 6c69 7a65 2f63 6c64 722f 7375 7070  balize/cldr/supp
+00017290: 6c65 6d65 6e74 616c 2e6a 735c 223e 3c2f  lemental.js\"></
+000172a0: 7363 7269 7074 3e5c 725c 6e3c 7363 7269  script>\r\n<scri
+000172b0: 7074 0a20 2020 2020 2020 2073 7263 3d5c  pt.        src=\
+000172c0: 222f 6a61 7465 6b75 6b6b 6f2f 6a73 2f67  "/jatekukko/js/g
+000172d0: 6c6f 6261 6c69 7a65 2f67 6c6f 6261 6c69  lobalize/globali
+000172e0: 7a65 2e6a 735c 223e 3c2f 7363 7269 7074  ze.js\"></script
+000172f0: 3e5c 725c 6e3c 7363 7269 7074 2073 7263  >\r\n<script src
+00017300: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6a73  =\"/jatekukko/js
+00017310: 2f67 6c6f 6261 6c69 7a65 2f67 6c6f 6261  /globalize/globa
+00017320: 6c69 7a65 2f6d 6573 7361 6765 2e6a 735c  lize/message.js\
+00017330: 223e 3c2f 7363 7269 7074 3e5c 725c 6e5c  "></script>\r\n\
+00017340: 725c 6e3c 212d 2d0a 2020 2020 2020 2020  r\n<!--.        
+00017350: 4a53 2043 6f6f 6b69 6520 2d2d 3e5c 725c  JS Cookie -->\r\
+00017360: 6e3c 7363 7269 7074 2073 7263 3d5c 222f  n<script src=\"/
+00017370: 6a61 7465 6b75 6b6b 6f2f 6a73 2f6a 732d  jatekukko/js/js-
+00017380: 636f 6f6b 6965 2f6a 732e 636f 6f6b 6965  cookie/js.cookie
+00017390: 2e6a 735c 223e 3c2f 7363 7269 7074 3e5c  .js\"></script>\
+000173a0: 725c 6e5c 725c 6e3c 7363 7269 7074 0a20  r\n\r\n<script. 
+000173b0: 2020 2020 2020 2073 7263 3d5c 222f 6a61         src=\"/ja
+000173c0: 7465 6b75 6b6b 6f2f 6a73 2f6d 6f6d 656e  tekukko/js/momen
+000173d0: 742f 6d6f 6d65 6e74 2d77 6974 682d 6c6f  t/moment-with-lo
+000173e0: 6361 6c65 732e 6d69 6e2e 6a73 5c22 3e3c  cales.min.js\"><
+000173f0: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
+00017400: 6970 743e 6d6f 6d65 6e74 2e6c 6f63 616c  ipt>moment.local
+00017410: 6528 2766 695f 4649 272e 7265 706c 6163  e('fi_FI'.replac
+00017420: 6528 275f 272c 0a20 2020 2020 2020 2027  e('_',.        '
+00017430: 2d27 2929 3b3c 2f73 6372 6970 743e 5c72  -'));</script>\r
+00017440: 5c6e 5c72 5c6e 3c21 2d2d 2057 6562 7368  \n\r\n<!-- Websh
+00017450: 696d 202d 2d3e 5c72 5c6e 3c21 2d2d 5b69  im -->\r\n<!--[i
+00017460: 6620 6c74 2049 4520 3130 5d3e 5c72 5c6e  f lt IE 10]>\r\n
+00017470: 5c74 3c73 6372 6970 740a 2020 2020 2020  \t<script.      
+00017480: 2020 7372 633d 5c22 2f6a 6174 656b 756b    src=\"/jatekuk
+00017490: 6b6f 2f6a 732f 6a73 2d77 6562 7368 696d  ko/js/js-webshim
+000174a0: 2f6d 696e 6966 6965 642f 706f 6c79 6669  /minified/polyfi
+000174b0: 6c6c 6572 2e6a 735c 223e 3c2f 7363 7269  ller.js\"></scri
+000174c0: 7074 3e5c 725c 6e5c 743c 7363 7269 7074  pt>\r\n\t<script
+000174d0: 3e5c 725c 6e5c 7477 6562 7368 696d 2e73  >\r\n\twebshim.s
+000174e0: 6574 4f70 7469 6f6e 7328 2765 7874 656e  etOptions('exten
+000174f0: 644e 6174 6976 6527 2c0a 2020 2020 2020  dNative',.      
+00017500: 2020 7472 7565 293b 5c72 5c6e 5c74 7765    true);\r\n\twe
+00017510: 6273 6869 6d2e 706f 6c79 6669 6c6c 2827  bshim.polyfill('
+00017520: 666f 726d 7327 293b 5c72 5c6e 5c74 3c2f  forms');\r\n\t</
+00017530: 7363 7269 7074 3e5c 725c 6e3c 215b 656e  script>\r\n<![en
+00017540: 6469 665d 2d2d 3e5c 725c 6e5c 725c 6e3c  dif]-->\r\n\r\n<
+00017550: 212d 2d0a 2020 2020 2020 2020 6874 6d6c  !--.        html
+00017560: 3573 6869 7620 2d2d 3e5c 725c 6e3c 212d  5shiv -->\r\n<!-
+00017570: 2d5b 6966 206c 7420 4945 2039 5d3e 5c72  -[if lt IE 9]>\r
+00017580: 5c6e 2020 2020 3c73 6372 6970 7420 7372  \n    <script sr
+00017590: 633d 5c22 2f6a 6174 656b 756b 6b6f 2f6a  c=\"/jatekukko/j
+000175a0: 732f 6874 6d6c 3573 6869 762e 6d69 6e2e  s/html5shiv.min.
+000175b0: 6a73 5c22 3e3c 2f73 6372 6970 743e 5c72  js\"></script>\r
+000175c0: 5c6e 3c21 5b65 6e64 6966 5d2d 2d3e 5c72  \n<![endif]-->\r
+000175d0: 5c6e 5c72 5c6e 3c21 2d2d 0a20 2020 2020  \n\r\n<!--.     
+000175e0: 2020 2044 4854 4d4c 5820 2d2d 3e5c 725c     DHTMLX -->\r\
+000175f0: 6e3c 7363 7269 7074 2073 7263 3d5c 222f  n<script src=\"/
+00017600: 6a61 7465 6b75 6b6b 6f2f 6a73 2f64 6874  jatekukko/js/dht
+00017610: 6d6c 7853 7569 7465 2f73 6f75 7263 6573  mlxSuite/sources
+00017620: 2f64 6874 6d6c 7843 6f6d 6d6f 6e2f 636f  /dhtmlxCommon/co
+00017630: 6465 6261 7365 2f64 6874 6d6c 7863 6f6d  debase/dhtmlxcom
+00017640: 6d6f 6e2e 6a73 5c22 3e3c 2f73 6372 6970  mon.js\"></scrip
+00017650: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
+00017660: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
+00017670: 656b 756b 6b6f 2f6a 732f 6468 746d 6c78  ekukko/js/dhtmlx
+00017680: 5375 6974 652f 736f 7572 6365 732f 6468  Suite/sources/dh
+00017690: 746d 6c78 436f 6d6d 6f6e 2f63 6f64 6562  tmlxCommon/codeb
+000176a0: 6173 652f 6468 746d 6c78 636f 7265 2e6a  ase/dhtmlxcore.j
+000176b0: 735c 223e 3c2f 7363 7269 7074 3e5c 725c  s\"></script>\r\
+000176c0: 6e3c 7363 7269 7074 0a20 2020 2020 2020  n<script.       
+000176d0: 2073 7263 3d5c 222f 6a61 7465 6b75 6b6b   src=\"/jatekukk
+000176e0: 6f2f 6a73 2f64 6874 6d6c 7853 7569 7465  o/js/dhtmlxSuite
+000176f0: 2f73 6f75 7263 6573 2f64 6874 6d6c 7846  /sources/dhtmlxF
+00017700: 6f72 6d2f 636f 6465 6261 7365 2f64 6874  orm/codebase/dht
+00017710: 6d6c 7866 6f72 6d2e 6a73 5c22 3e3c 2f73  mlxform.js\"></s
+00017720: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
+00017730: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
+00017740: 2f6a 6174 656b 756b 6b6f 2f6a 732f 6468  /jatekukko/js/dh
+00017750: 746d 6c78 5375 6974 652f 736f 7572 6365  tmlxSuite/source
+00017760: 732f 6468 746d 6c78 466f 726d 2f63 6f64  s/dhtmlxForm/cod
+00017770: 6562 6173 652f 6578 742f 6468 746d 6c78  ebase/ext/dhtmlx
+00017780: 666f 726d 5f69 7465 6d5f 6361 6c65 6e64  form_item_calend
+00017790: 6172 2e6a 735c 223e 3c2f 7363 7269 7074  ar.js\"></script
+000177a0: 3e5c 725c 6e3c 7363 7269 7074 0a20 2020  >\r\n<script.   
+000177b0: 2020 2020 2073 7263 3d5c 222f 6a61 7465       src=\"/jate
+000177c0: 6b75 6b6b 6f2f 6a73 2f64 6874 6d6c 7853  kukko/js/dhtmlxS
+000177d0: 7569 7465 2f73 6f75 7263 6573 2f64 6874  uite/sources/dht
+000177e0: 6d6c 7846 6f72 6d2f 636f 6465 6261 7365  mlxForm/codebase
+000177f0: 2f65 7874 2f64 6874 6d6c 7866 6f72 6d5f  /ext/dhtmlxform_
+00017800: 6479 6e2e 6a73 5c22 3e3c 2f73 6372 6970  dyn.js\"></scrip
+00017810: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
+00017820: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
+00017830: 656b 756b 6b6f 2f6a 732f 6468 746d 6c78  ekukko/js/dhtmlx
+00017840: 5375 6974 652f 736f 7572 6365 732f 6468  Suite/sources/dh
+00017850: 746d 6c78 4361 6c65 6e64 6172 2f63 6f64  tmlxCalendar/cod
+00017860: 6562 6173 652f 6468 746d 6c78 6361 6c65  ebase/dhtmlxcale
+00017870: 6e64 6172 2e6a 735c 223e 3c2f 7363 7269  ndar.js\"></scri
+00017880: 7074 3e5c 725c 6e3c 7363 7269 7074 0a20  pt>\r\n<script. 
+00017890: 2020 2020 2020 2073 7263 3d5c 222f 6a61         src=\"/ja
+000178a0: 7465 6b75 6b6b 6f2f 6a73 2f64 6874 6d6c  tekukko/js/dhtml
+000178b0: 7853 7569 7465 2f73 6f75 7263 6573 2f64  xSuite/sources/d
+000178c0: 6874 6d6c 7854 6f6f 6c62 6172 2f63 6f64  htmlxToolbar/cod
+000178d0: 6562 6173 652f 6468 746d 6c78 746f 6f6c  ebase/dhtmlxtool
+000178e0: 6261 722e 6a73 5c22 3e3c 2f73 6372 6970  bar.js\"></scrip
+000178f0: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
+00017900: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
+00017910: 656b 756b 6b6f 2f6a 732f 6468 746d 6c78  ekukko/js/dhtmlx
+00017920: 5375 6974 652f 736f 7572 6365 732f 6468  Suite/sources/dh
+00017930: 746d 6c78 4461 7461 5669 6577 2f63 6f64  tmlxDataView/cod
+00017940: 6562 6173 652f 6468 746d 6c78 6461 7461  ebase/dhtmlxdata
+00017950: 7669 6577 2e6a 735c 223e 3c2f 7363 7269  view.js\"></scri
+00017960: 7074 3e5c 725c 6e3c 7363 7269 7074 0a20  pt>\r\n<script. 
+00017970: 2020 2020 2020 2073 7263 3d5c 222f 6a61         src=\"/ja
+00017980: 7465 6b75 6b6b 6f2f 6a73 2f64 6874 6d6c  tekukko/js/dhtml
+00017990: 7853 7569 7465 2f73 6f75 7263 6573 2f64  xSuite/sources/d
+000179a0: 6874 6d6c 7847 7269 642f 636f 6465 6261  htmlxGrid/codeba
+000179b0: 7365 2f64 6874 6d6c 7867 7269 642e 6a73  se/dhtmlxgrid.js
+000179c0: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
+000179d0: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
+000179e0: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
+000179f0: 2f6a 732f 6468 746d 6c78 5375 6974 652f  /js/dhtmlxSuite/
+00017a00: 736f 7572 6365 732f 6468 746d 6c78 4d65  sources/dhtmlxMe
+00017a10: 7373 6167 652f 636f 6465 6261 7365 2f64  ssage/codebase/d
+00017a20: 6874 6d6c 786d 6573 7361 6765 2e6a 735c  htmlxmessage.js\
+00017a30: 223e 3c2f 7363 7269 7074 3e5c 725c 6e5c  "></script>\r\n\
+00017a40: 725c 6e3c 212d 2d0a 2020 2020 2020 2020  r\n<!--.        
+00017a50: 4f76 6572 7772 6974 6520 4448 544d 4c58  Overwrite DHTMLX
+00017a60: 2064 6878 666f 726d 5f62 746e 2072 6f6c   dhxform_btn rol
+00017a70: 652e 2054 6869 7320 6d75 7374 2062 6520  e. This must be 
+00017a80: 6c6f 6164 6564 2061 6674 6572 2044 4854  loaded after DHT
+00017a90: 4d4c 5821 202d 2d3e 5c72 5c6e 3c73 6372  MLX! -->\r\n<scr
+00017aa0: 6970 740a 2020 2020 2020 2020 7372 633d  ipt.        src=
+00017ab0: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
+00017ac0: 6468 746d 6c78 5f66 6f72 6d5f 706f 7374  dhtmlx_form_post
+00017ad0: 6c6f 6164 2e6a 733f 7469 6d65 7374 616d  load.js?timestam
+00017ae0: 703d 3230 3231 3037 3139 2d31 3433 365c  p=20210719-1436\
+00017af0: 223e 3c2f 7363 7269 7074 3e5c 725c 6e5c  "></script>\r\n\
+00017b00: 725c 6e3c 212d 2d0a 2020 2020 2020 2020  r\n<!--.        
+00017b10: 5c20 4b65 6e64 6f20 5549 202d 2d3e 5c72  \ Kendo UI -->\r
+00017b20: 5c6e 3c73 6372 6970 7420 7372 633d 5c22  \n<script src=\"
+00017b30: 2f6a 6174 656b 756b 6b6f 2f6a 732f 6b65  /jatekukko/js/ke
+00017b40: 6e64 6f75 692f 6b65 6e64 6f2e 636f 7265  ndoui/kendo.core
+00017b50: 2e6d 696e 2e6a 735c 223e 3c2f 7363 7269  .min.js\"></scri
+00017b60: 7074 3e5c 745c 725c 6e3c 7363 7269 7074  pt>\t\r\n<script
+00017b70: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
+00017b80: 6a61 7465 6b75 6b6b 6f2f 6a73 2f6b 656e  jatekukko/js/ken
+00017b90: 646f 7569 2f6b 656e 646f 2e64 6174 612e  doui/kendo.data.
+00017ba0: 6d69 6e2e 6a73 5c22 3e3c 2f73 6372 6970  min.js\"></scrip
+00017bb0: 743e 5c72 5c6e 3c73 6372 6970 7420 7372  t>\r\n<script sr
+00017bc0: 633d 5c22 2f6a 6174 656b 756b 6b6f 2f6a  c=\"/jatekukko/j
+00017bd0: 732f 6b65 6e64 6f75 692f 6b65 6e64 6f2e  s/kendoui/kendo.
+00017be0: 646f 6d2e 6d69 6e2e 6a73 5c22 3e3c 2f73  dom.min.js\"></s
+00017bf0: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
+00017c00: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
+00017c10: 2f6a 6174 656b 756b 6b6f 2f6a 732f 6b65  /jatekukko/js/ke
+00017c20: 6e64 6f75 692f 6b65 6e64 6f2e 706f 7075  ndoui/kendo.popu
+00017c30: 702e 6d69 6e2e 6a73 5c22 3e3c 2f73 6372  p.min.js\"></scr
+00017c40: 6970 743e 5c72 5c6e 3c73 6372 6970 7420  ipt>\r\n<script 
+00017c50: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
+00017c60: 2f6a 732f 6b65 6e64 6f75 692f 6b65 6e64  /js/kendoui/kend
+00017c70: 6f2e 6c69 7374 2e6d 696e 2e6a 735c 223e  o.list.min.js\">
+00017c80: 3c2f 7363 7269 7074 3e5c 725c 6e3c 7363  </script>\r\n<sc
+00017c90: 7269 7074 0a20 2020 2020 2020 2073 7263  ript.        src
+00017ca0: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6a73  =\"/jatekukko/js
+00017cb0: 2f6b 656e 646f 7569 2f6b 656e 646f 2e66  /kendoui/kendo.f
+00017cc0: 782e 6d69 6e2e 6a73 5c22 3e3c 2f73 6372  x.min.js\"></scr
+00017cd0: 6970 743e 5c72 5c6e 3c73 6372 6970 7420  ipt>\r\n<script 
+00017ce0: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
+00017cf0: 2f6a 732f 6b65 6e64 6f75 692f 6b65 6e64  /js/kendoui/kend
+00017d00: 6f2e 7573 6572 6576 656e 7473 2e6d 696e  o.userevents.min
+00017d10: 2e6a 735c 223e 3c2f 7363 7269 7074 3e5c  .js\"></script>\
+00017d20: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
+00017d30: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
+00017d40: 6b6b 6f2f 6a73 2f6b 656e 646f 7569 2f6b  kko/js/kendoui/k
+00017d50: 656e 646f 2e64 7261 6761 6e64 6472 6f70  endo.draganddrop
+00017d60: 2e6d 696e 2e6a 735c 223e 3c2f 7363 7269  .min.js\"></scri
+00017d70: 7074 3e5c 725c 6e3c 7363 7269 7074 0a20  pt>\r\n<script. 
+00017d80: 2020 2020 2020 2073 7263 3d5c 222f 6a61         src=\"/ja
+00017d90: 7465 6b75 6b6b 6f2f 6a73 2f6b 656e 646f  tekukko/js/kendo
+00017da0: 7569 2f6b 656e 646f 2e72 6573 697a 6162  ui/kendo.resizab
+00017db0: 6c65 2e6d 696e 2e6a 735c 223e 3c2f 7363  le.min.js\"></sc
+00017dc0: 7269 7074 3e5c 725c 6e3c 7363 7269 7074  ript>\r\n<script
+00017dd0: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
+00017de0: 6a61 7465 6b75 6b6b 6f2f 6a73 2f6b 656e  jatekukko/js/ken
+00017df0: 646f 7569 2f6b 656e 646f 2e65 6469 7461  doui/kendo.edita
+00017e00: 626c 652e 6d69 6e2e 6a73 5c22 3e3c 2f73  ble.min.js\"></s
+00017e10: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
+00017e20: 7420 7372 633d 5c22 2f6a 6174 656b 756b  t src=\"/jatekuk
+00017e30: 6b6f 2f6a 732f 6b65 6e64 6f75 692f 6b65  ko/js/kendoui/ke
+00017e40: 6e64 6f2e 6269 6e64 6572 2e6d 696e 2e6a  ndo.binder.min.j
+00017e50: 735c 223e 3c2f 7363 7269 7074 3e5c 725c  s\"></script>\r\
+00017e60: 6e3c 7363 7269 7074 0a20 2020 2020 2020  n<script.       
+00017e70: 2073 7263 3d5c 222f 6a61 7465 6b75 6b6b   src=\"/jatekukk
+00017e80: 6f2f 6a73 2f6b 656e 646f 7569 2f6b 656e  o/js/kendoui/ken
+00017e90: 646f 2e76 616c 6964 6174 6f72 2e6d 696e  do.validator.min
+00017ea0: 2e6a 735c 223e 3c2f 7363 7269 7074 3e5c  .js\"></script>\
+00017eb0: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
+00017ec0: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
+00017ed0: 6b6b 6f2f 6a73 2f6b 656e 646f 7569 2f6b  kko/js/kendoui/k
+00017ee0: 656e 646f 2e6d 6f62 696c 652e 7363 726f  endo.mobile.scro
+00017ef0: 6c6c 6572 2e6d 696e 2e6a 735c 223e 3c2f  ller.min.js\"></
+00017f00: 7363 7269 7074 3e5c 725c 6e3c 7363 7269  script>\r\n<scri
+00017f10: 7074 0a20 2020 2020 2020 2073 7263 3d5c  pt.        src=\
+00017f20: 222f 6a61 7465 6b75 6b6b 6f2f 6a73 2f6b  "/jatekukko/js/k
+00017f30: 656e 646f 7569 2f6b 656e 646f 2e76 6972  endoui/kendo.vir
+00017f40: 7475 616c 6c69 7374 2e6d 696e 2e6a 735c  tuallist.min.js\
+00017f50: 223e 3c2f 7363 7269 7074 3e5c 725c 6e3c  "></script>\r\n<
+00017f60: 7363 7269 7074 0a20 2020 2020 2020 2073  script.        s
+00017f70: 7263 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  rc=\"/jatekukko/
+00017f80: 6a73 2f6b 656e 646f 7569 2f6b 656e 646f  js/kendoui/kendo
+00017f90: 2e63 6f6c 756d 6e73 6f72 7465 722e 6d69  .columnsorter.mi
+00017fa0: 6e2e 6a73 5c22 3e3c 2f73 6372 6970 743e  n.js\"></script>
+00017fb0: 5c72 5c6e 3c73 6372 6970 740a 2020 2020  \r\n<script.    
+00017fc0: 2020 2020 7372 633d 5c22 2f6a 6174 656b      src=\"/jatek
+00017fd0: 756b 6b6f 2f6a 732f 6b65 6e64 6f75 692f  ukko/js/kendoui/
+00017fe0: 6375 6c74 7572 6573 2f6b 656e 646f 2e63  cultures/kendo.c
+00017ff0: 756c 7475 7265 2e66 692d 4649 2e6d 696e  ulture.fi-FI.min
+00018000: 2e6a 735c 223e 3c2f 7363 7269 7074 3e5c  .js\"></script>\
+00018010: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
+00018020: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
+00018030: 6b6b 6f2f 6a73 2f6b 656e 646f 7569 2f63  kko/js/kendoui/c
+00018040: 756c 7475 7265 732f 6b65 6e64 6f2e 6375  ultures/kendo.cu
+00018050: 6c74 7572 652e 7376 2d46 492e 6d69 6e2e  lture.sv-FI.min.
+00018060: 6a73 5c22 3e3c 2f73 6372 6970 743e 5c72  js\"></script>\r
+00018070: 5c6e 5c72 5c6e 3c21 2d2d 0a20 2020 2020  \n\r\n<!--.     
+00018080: 2020 204b 656e 646f 2055 492c 2061 6374     Kendo UI, act
+00018090: 7561 6c20 636f 6d70 6f6e 656e 7473 202d  ual components -
+000180a0: 2d3e 5c72 5c6e 3c73 6372 6970 7420 7372  ->\r\n<script sr
+000180b0: 633d 5c22 2f6a 6174 656b 756b 6b6f 2f6a  c=\"/jatekukko/j
+000180c0: 732f 6b65 6e64 6f75 692f 6b65 6e64 6f2e  s/kendoui/kendo.
+000180d0: 6472 6f70 646f 776e 6c69 7374 2e6d 696e  dropdownlist.min
+000180e0: 2e6a 735c 223e 3c2f 7363 7269 7074 3e5c  .js\"></script>\
+000180f0: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
+00018100: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
+00018110: 6b6b 6f2f 6a73 2f6b 656e 646f 7569 2f6b  kko/js/kendoui/k
+00018120: 656e 646f 2e6e 756d 6572 6963 7465 7874  endo.numerictext
+00018130: 626f 782e 6d69 6e2e 6a73 5c22 3e3c 2f73  box.min.js\"></s
+00018140: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
+00018150: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
+00018160: 2f6a 6174 656b 756b 6b6f 2f6a 732f 6b65  /jatekukko/js/ke
+00018170: 6e64 6f75 692f 6b65 6e64 6f2e 6772 6964  ndoui/kendo.grid
+00018180: 2e6d 696e 2e6a 735c 223e 3c2f 7363 7269  .min.js\"></scri
+00018190: 7074 3e5c 725c 6e3c 7363 7269 7074 2073  pt>\r\n<script s
+000181a0: 7263 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  rc=\"/jatekukko/
+000181b0: 6a73 2f6b 656e 646f 7569 2f6b 656e 646f  js/kendoui/kendo
+000181c0: 2e6d 756c 7469 7365 6c65 6374 2e6d 696e  .multiselect.min
+000181d0: 2e6a 735c 223e 3c2f 7363 7269 7074 3e5c  .js\"></script>\
+000181e0: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
+000181f0: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
+00018200: 6b6b 6f2f 6a73 2f6b 656e 646f 7569 2f6b  kko/js/kendoui/k
+00018210: 656e 646f 2e74 7265 656c 6973 742e 6d69  endo.treelist.mi
+00018220: 6e2e 6a73 5c22 3e3c 2f73 6372 6970 743e  n.js\"></script>
+00018230: 5c72 5c6e 5c72 5c6e 3c73 6372 6970 740a  \r\n\r\n<script.
+00018240: 2020 2020 2020 2020 7372 633d 5c22 2f6a          src=\"/j
+00018250: 6174 656b 756b 6b6f 2f6a 732f 6b65 6e64  atekukko/js/kend
+00018260: 6f75 692f 6d65 7373 6167 6573 2f6b 656e  oui/messages/ken
+00018270: 646f 2e6d 6573 7361 6765 732e 6669 2d46  do.messages.fi-F
+00018280: 492e 6d69 6e2e 6a73 5c22 3e3c 2f73 6372  I.min.js\"></scr
+00018290: 6970 743e 5c72 5c6e 3c21 2d2d 0a20 2020  ipt>\r\n<!--.   
+000182a0: 2020 2020 2053 6574 206b 656e 646f 2074       Set kendo t
+000182b0: 6f20 7269 6768 7420 6375 6c74 7572 6520  o right culture 
+000182c0: 2d2d 3e5c 725c 6e3c 7363 7269 7074 3e5c  -->\r\n<script>\
+000182d0: 725c 6e5c 746b 656e 646f 2e63 756c 7475  r\n\tkendo.cultu
+000182e0: 7265 285c 2266 695f 4649 5c22 2e72 6570  re(\"fi_FI\".rep
+000182f0: 6c61 6365 2827 5f27 2c0a 2020 2020 2020  lace('_',.      
+00018300: 2020 272d 2729 293b 5c72 5c6e 3c2f 7363    '-'));\r\n</sc
+00018310: 7269 7074 3e5c 725c 6e5c 725c 6e5c 725c  ript>\r\n\r\n\r\
+00018320: 6e3c 212d 2d20 4172 6347 4953 202d 2d3e  n<!-- ArcGIS -->
+00018330: 5c72 5c6e 3c73 6372 6970 743e 5c72 5c6e  \r\n<script>\r\n
+00018340: 2020 2020 7661 7220 646f 6a6f 436f 6e66      var dojoConf
+00018350: 6967 0a20 2020 2020 2020 203d 207b 5c72  ig.        = {\r
+00018360: 5c6e 2020 2020 2020 2020 6c6f 6361 6c65  \n        locale
+00018370: 3a20 2766 695f 4649 272e 746f 4c6f 7765  : 'fi_FI'.toLowe
+00018380: 7243 6173 6528 292e 7265 706c 6163 6528  rCase().replace(
+00018390: 275f 272c 2027 2d27 295c 725c 6e20 2020  '_', '-')\r\n   
+000183a0: 207d 3b5c 725c 6e3c 2f73 6372 6970 743e   };\r\n</script>
+000183b0: 5c72 5c6e 3c73 6372 6970 740a 2020 2020  \r\n<script.    
+000183c0: 2020 2020 7372 633d 5c22 6874 7470 733a      src=\"https:
+000183d0: 2f2f 6a73 2e61 7263 6769 732e 636f 6d2f  //js.arcgis.com/
+000183e0: 332e 3333 2f5c 223e 3c2f 7363 7269 7074  3.33/\"></script
+000183f0: 3e5c 725c 6e5c 725c 6e3c 212d 2d20 426f  >\r\n\r\n<!-- Bo
+00018400: 6f74 7374 7261 7020 2d2d 3e5c 725c 6e3c  otstrap -->\r\n<
+00018410: 7363 7269 7074 0a20 2020 2020 2020 2073  script.        s
+00018420: 7263 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  rc=\"/jatekukko/
+00018430: 6a73 2f62 6f6f 7473 7472 6170 2f62 6f6f  js/bootstrap/boo
+00018440: 7473 7472 6170 2e6d 696e 2e6a 735c 223e  tstrap.min.js\">
+00018450: 3c2f 7363 7269 7074 3e5c 725c 6e5c 725c  </script>\r\n\r\
+00018460: 6e3c 212d 2d20 4375 7374 6f6d 0a20 2020  n<!-- Custom.   
+00018470: 2020 2020 202d 2d3e 5c72 5c6e 3c73 6372       -->\r\n<scr
+00018480: 6970 7420 7372 633d 5c22 2f6a 6174 656b  ipt src=\"/jatek
+00018490: 756b 6b6f 2f6a 732f 6468 746d 6c78 5f65  ukko/js/dhtmlx_e
+000184a0: 7874 2e6a 733f 7469 6d65 7374 616d 703d  xt.js?timestamp=
+000184b0: 3230 3231 3037 3139 2d31 3433 365c 223e  20210719-1436\">
+000184c0: 3c2f 7363 7269 7074 3e5c 725c 6e3c 7363  </script>\r\n<sc
+000184d0: 7269 7074 0a20 2020 2020 2020 2073 7263  ript.        src
+000184e0: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6a73  =\"/jatekukko/js
+000184f0: 2f64 6874 6d6c 785f 6578 745f 7765 656b  /dhtmlx_ext_week
+00018500: 5f63 616c 656e 6461 722e 6a73 3f74 696d  _calendar.js?tim
+00018510: 6573 7461 6d70 3d32 3032 3130 3731 392d  estamp=20210719-
+00018520: 3134 3336 5c22 3e3c 2f73 6372 6970 743e  1436\"></script>
+00018530: 5c72 5c6e 3c73 6372 6970 740a 2020 2020  \r\n<script.    
+00018540: 2020 2020 7372 633d 5c22 2f6a 6174 656b      src=\"/jatek
+00018550: 756b 6b6f 2f6a 732f 636f 6d6d 6f6e 2e6a  ukko/js/common.j
+00018560: 733f 7469 6d65 7374 616d 703d 3230 3231  s?timestamp=2021
+00018570: 3037 3139 2d31 3433 365c 223e 3c2f 7363  0719-1436\"></sc
+00018580: 7269 7074 3e5c 725c 6e3c 7363 7269 7074  ript>\r\n<script
+00018590: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
+000185a0: 6a61 7465 6b75 6b6b 6f2f 6a73 2f76 616c  jatekukko/js/val
+000185b0: 6964 6174 6f72 732e 6a73 3f74 696d 6573  idators.js?times
+000185c0: 7461 6d70 3d32 3032 3130 3731 392d 3134  tamp=20210719-14
+000185d0: 3336 5c22 3e3c 2f73 6372 6970 743e 5c72  36\"></script>\r
+000185e0: 5c6e 3c73 6372 6970 740a 2020 2020 2020  \n<script.      
+000185f0: 2020 7372 633d 5c22 2f6a 6174 656b 756b    src=\"/jatekuk
+00018600: 6b6f 2f6a 732f 676f 6f67 6c65 2e6a 733f  ko/js/google.js?
+00018610: 7469 6d65 7374 616d 703d 3230 3231 3037  timestamp=202107
+00018620: 3139 2d31 3433 365c 223e 3c2f 7363 7269  19-1436\"></scri
+00018630: 7074 3e5c 725c 6e3c 7363 7269 7074 0a20  pt>\r\n<script. 
+00018640: 2020 2020 2020 2073 7263 3d5c 222f 6a61         src=\"/ja
+00018650: 7465 6b75 6b6b 6f2f 6a73 2f73 6861 7265  tekukko/js/share
+00018660: 642f 7469 6d65 6f75 742e 6a73 3f74 696d  d/timeout.js?tim
+00018670: 6573 7461 6d70 3d32 3032 3130 3731 392d  estamp=20210719-
+00018680: 3134 3336 5c22 3e3c 2f73 6372 6970 743e  1436\"></script>
+00018690: 5c72 5c6e 3c73 6372 6970 740a 2020 2020  \r\n<script.    
+000186a0: 2020 2020 7372 633d 5c22 2f6a 6174 656b      src=\"/jatek
+000186b0: 756b 6b6f 2f6a 732f 7368 6172 6564 2f76  ukko/js/shared/v
+000186c0: 696d 656f 2e6a 733f 7469 6d65 7374 616d  imeo.js?timestam
+000186d0: 703d 3230 3231 3037 3139 2d31 3433 365c  p=20210719-1436\
+000186e0: 223e 3c2f 7363 7269 7074 3e5c 725c 6e5c  "></script>\r\n\
+000186f0: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
+00018700: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
+00018710: 6b6b 6f2f 6a73 2f73 6168 6173 2f61 7070  kko/js/sahas/app
+00018720: 6c69 6361 7469 6f6e 2e6a 733f 7469 6d65  lication.js?time
+00018730: 7374 616d 703d 3230 3231 3037 3139 2d31  stamp=20210719-1
+00018740: 3433 365c 223e 3c2f 7363 7269 7074 3e5c  436\"></script>\
+00018750: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
+00018760: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
+00018770: 6b6b 6f2f 6a73 2f73 6168 6173 2f6c 6f67  kko/js/sahas/log
+00018780: 696e 2e6a 733f 7469 6d65 7374 616d 703d  in.js?timestamp=
+00018790: 3230 3231 3037 3139 2d31 3433 365c 223e  20210719-1436\">
+000187a0: 3c2f 7363 7269 7074 3e5c 725c 6e3c 7363  </script>\r\n<sc
+000187b0: 7269 7074 0a20 2020 2020 2020 2073 7263  ript.        src
+000187c0: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6a73  =\"/jatekukko/js
+000187d0: 2f73 6168 6173 2f73 6572 7669 6365 5f77  /sahas/service_w
+000187e0: 696e 646f 7773 2e6a 733f 7469 6d65 7374  indows.js?timest
+000187f0: 616d 703d 3230 3231 3037 3139 2d31 3433  amp=20210719-143
+00018800: 365c 223e 3c2f 7363 7269 7074 3e5c 725c  6\"></script>\r\
+00018810: 6e3c 7363 7269 7074 0a20 2020 2020 2020  n<script.       
+00018820: 2073 7263 3d5c 222f 6a61 7465 6b75 6b6b   src=\"/jatekukk
+00018830: 6f2f 6a73 2f73 6168 6173 2f73 686f 7070  o/js/sahas/shopp
+00018840: 696e 6763 6172 742e 6a73 3f74 696d 6573  ingcart.js?times
+00018850: 7461 6d70 3d32 3032 3130 3731 392d 3134  tamp=20210719-14
+00018860: 3336 5c22 3e3c 2f73 6372 6970 743e 5c72  36\"></script>\r
+00018870: 5c6e 3c73 6372 6970 740a 2020 2020 2020  \n<script.      
+00018880: 2020 7372 633d 5c22 2f6a 6174 656b 756b    src=\"/jatekuk
+00018890: 6b6f 2f6a 732f 7361 6861 732f 7365 7276  ko/js/sahas/serv
+000188a0: 6963 655f 616b 702e 6a73 3f74 696d 6573  ice_akp.js?times
+000188b0: 7461 6d70 3d32 3032 3130 3731 392d 3134  tamp=20210719-14
+000188c0: 3336 5c22 3e3c 2f73 6372 6970 743e 5c72  36\"></script>\r
+000188d0: 5c6e 5c72 5c6e 3c73 6372 6970 740a 2020  \n\r\n<script.  
+000188e0: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
+000188f0: 656b 756b 6b6f 2f6a 732f 7361 6861 732f  ekukko/js/sahas/
+00018900: 7461 6273 2f73 6572 7669 6365 2d6c 6973  tabs/service-lis
+00018910: 742e 6a73 3f74 696d 6573 7461 6d70 3d32  t.js?timestamp=2
+00018920: 3032 3130 3731 392d 3134 3336 5c22 3e3c  0210719-1436\"><
+00018930: 2f73 6372 6970 743e 5c72 5c6e 5c72 5c6e  /script>\r\n\r\n
+00018940: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
+00018950: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
+00018960: 2f6a 732f 7361 6861 732f 7461 6273 2f63  /js/sahas/tabs/c
+00018970: 7573 746f 6d65 722d 6461 7461 2e6a 733f  ustomer-data.js?
+00018980: 7469 6d65 7374 616d 703d 3230 3231 3037  timestamp=202107
+00018990: 3139 2d31 3433 365c 223e 3c2f 7363 7269  19-1436\"></scri
+000189a0: 7074 3e5c 725c 6e5c 725c 6e5c 725c 6e3c  pt>\r\n\r\n\r\n<
+000189b0: 7363 7269 7074 0a20 2020 2020 2020 2073  script.        s
+000189c0: 7263 3d5c 222f 6a61 7465 6b75 6b6b 6f2f  rc=\"/jatekukko/
+000189d0: 6a73 2f73 6168 6173 2f74 6162 732f 6665  js/sahas/tabs/fe
+000189e0: 6564 6261 636b 2e6a 733f 7469 6d65 7374  edback.js?timest
+000189f0: 616d 703d 3230 3231 3037 3139 2d31 3433  amp=20210719-143
+00018a00: 365c 223e 3c2f 7363 7269 7074 3e5c 725c  6\"></script>\r\
+00018a10: 6e5c 725c 6e3c 7363 7269 7074 0a20 2020  n\r\n<script.   
+00018a20: 2020 2020 2073 7263 3d5c 222f 6a61 7465       src=\"/jate
+00018a30: 6b75 6b6b 6f2f 6a73 2f73 6168 6173 2f74  kukko/js/sahas/t
+00018a40: 6162 732f 7573 6572 2d64 6574 6169 6c73  abs/user-details
+00018a50: 2e6a 733f 7469 6d65 7374 616d 703d 3230  .js?timestamp=20
+00018a60: 3231 3037 3139 2d31 3433 365c 223e 3c2f  210719-1436\"></
+00018a70: 7363 7269 7074 3e5c 725c 6e3c 7363 7269  script>\r\n<scri
+00018a80: 7074 0a20 2020 2020 2020 2073 7263 3d5c  pt.        src=\
+00018a90: 222f 6a61 7465 6b75 6b6b 6f2f 6a73 2f73  "/jatekukko/js/s
+00018aa0: 6168 6173 2f74 6162 732f 6c6f 6769 6e2d  ahas/tabs/login-
+00018ab0: 7061 6765 2e6a 733f 7469 6d65 7374 616d  page.js?timestam
+00018ac0: 703d 3230 3231 3037 3139 2d31 3433 365c  p=20210719-1436\
+00018ad0: 223e 3c2f 7363 7269 7074 3e5c 725c 6e5c  "></script>\r\n\
+00018ae0: 725c 6e5c 725c 6e3c 7363 7269 7074 0a20  r\n\r\n<script. 
+00018af0: 2020 2020 2020 2073 7263 3d5c 222f 6a61         src=\"/ja
+00018b00: 7465 6b75 6b6b 6f2f 6a73 2f73 6168 6173  tekukko/js/sahas
+00018b10: 2f74 6162 732f 696e 766f 6963 652d 6c69  /tabs/invoice-li
+00018b20: 7374 2e6a 733f 7469 6d65 7374 616d 703d  st.js?timestamp=
+00018b30: 3230 3231 3037 3139 2d31 3433 365c 223e  20210719-1436\">
+00018b40: 3c2f 7363 7269 7074 3e5c 725c 6e5c 725c  </script>\r\n\r\
+00018b50: 6e5c 725c 6e3c 7363 7269 7074 0a20 2020  n\r\n<script.   
+00018b60: 2020 2020 2073 7263 3d5c 222f 6a61 7465       src=\"/jate
+00018b70: 6b75 6b6b 6f2f 6a73 2f73 6168 6173 2f77  kukko/js/sahas/w
+00018b80: 696e 646f 7773 2f6c 6f73 742d 7061 7373  indows/lost-pass
+00018b90: 776f 7264 2d77 696e 646f 772e 6a73 3f74  word-window.js?t
+00018ba0: 696d 6573 7461 6d70 3d32 3032 3130 3731  imestamp=2021071
+00018bb0: 392d 3134 3336 5c22 3e3c 2f73 6372 6970  9-1436\"></scrip
+00018bc0: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
+00018bd0: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
+00018be0: 656b 756b 6b6f 2f6a 732f 7361 6861 732f  ekukko/js/sahas/
+00018bf0: 7769 6e64 6f77 732f 6368 616e 6765 2d6a  windows/change-j
+00018c00: 6f69 6e2d 7479 7065 2d77 696e 646f 772e  oin-type-window.
+00018c10: 6a73 3f74 696d 6573 7461 6d70 3d32 3032  js?timestamp=202
+00018c20: 3130 3731 392d 3134 3336 5c22 3e3c 2f73  10719-1436\"></s
+00018c30: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
+00018c40: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
+00018c50: 2f6a 6174 656b 756b 6b6f 2f6a 732f 7361  /jatekukko/js/sa
+00018c60: 6861 732f 7769 6e64 6f77 732f 616b 702d  has/windows/akp-
+00018c70: 6c6f 6361 7469 6f6e 2d77 696e 646f 772e  location-window.
+00018c80: 6a73 3f74 696d 6573 7461 6d70 3d32 3032  js?timestamp=202
+00018c90: 3130 3731 392d 3134 3336 5c22 3e3c 2f73  10719-1436\"></s
+00018ca0: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
+00018cb0: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
+00018cc0: 2f6a 6174 656b 756b 6b6f 2f6a 732f 7361  /jatekukko/js/sa
+00018cd0: 6861 732f 7769 6e64 6f77 732f 626f 6f6b  has/windows/book
+00018ce0: 7570 2d77 696e 646f 772e 6a73 3f74 696d  up-window.js?tim
+00018cf0: 6573 7461 6d70 3d32 3032 3130 3731 392d  estamp=20210719-
+00018d00: 3134 3336 5c22 3e3c 2f73 6372 6970 743e  1436\"></script>
+00018d10: 5c72 5c6e 3c73 6372 6970 740a 2020 2020  \r\n<script.    
+00018d20: 2020 2020 7372 633d 5c22 2f6a 6174 656b      src=\"/jatek
+00018d30: 756b 6b6f 2f6a 732f 7361 6861 732f 7769  ukko/js/sahas/wi
+00018d40: 6e64 6f77 732f 6665 6564 6261 636b 2d77  ndows/feedback-w
+00018d50: 696e 646f 772e 6a73 3f74 696d 6573 7461  indow.js?timesta
+00018d60: 6d70 3d32 3032 3130 3731 392d 3134 3336  mp=20210719-1436
+00018d70: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
+00018d80: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
+00018d90: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
+00018da0: 2f6a 732f 7361 6861 732f 7769 6e64 6f77  /js/sahas/window
+00018db0: 732f 7061 7373 776f 7264 2d77 696e 646f  s/password-windo
+00018dc0: 772e 6a73 3f74 696d 6573 7461 6d70 3d32  w.js?timestamp=2
+00018dd0: 3032 3130 3731 392d 3134 3336 5c22 3e3c  0210719-1436\"><
+00018de0: 2f73 6372 6970 743e 5c72 5c6e 3c73 6372  /script>\r\n<scr
+00018df0: 6970 740a 2020 2020 2020 2020 7372 633d  ipt.        src=
+00018e00: 5c22 2f6a 6174 656b 756b 6b6f 2f6a 732f  \"/jatekukko/js/
+00018e10: 7361 6861 732f 7769 6e64 6f77 732f 6368  sahas/windows/ch
+00018e20: 616e 6765 2d77 696e 646f 772e 6a73 3f74  ange-window.js?t
+00018e30: 696d 6573 7461 6d70 3d32 3032 3130 3731  imestamp=2021071
+00018e40: 392d 3134 3336 5c22 3e3c 2f73 6372 6970  9-1436\"></scrip
+00018e50: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
+00018e60: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
+00018e70: 656b 756b 6b6f 2f6a 732f 7361 6861 732f  ekukko/js/sahas/
+00018e80: 7769 6e64 6f77 732f 7465 726d 696e 6174  windows/terminat
+00018e90: 652d 7769 6e64 6f77 2e6a 733f 7469 6d65  e-window.js?time
+00018ea0: 7374 616d 703d 3230 3231 3037 3139 2d31  stamp=20210719-1
+00018eb0: 3433 365c 223e 3c2f 7363 7269 7074 3e5c  436\"></script>\
+00018ec0: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
+00018ed0: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
+00018ee0: 6b6b 6f2f 6a73 2f73 6168 6173 2f77 696e  kko/js/sahas/win
+00018ef0: 646f 7773 2f63 7265 6174 652d 6f72 6465  dows/create-orde
+00018f00: 722d 7769 6e64 6f77 2e6a 733f 7469 6d65  r-window.js?time
+00018f10: 7374 616d 703d 3230 3231 3037 3139 2d31  stamp=20210719-1
+00018f20: 3433 365c 223e 3c2f 7363 7269 7074 3e5c  436\"></script>\
+00018f30: 725c 6e3c 7363 7269 7074 0a20 2020 2020  r\n<script.     
+00018f40: 2020 2073 7263 3d5c 222f 6a61 7465 6b75     src=\"/jateku
+00018f50: 6b6b 6f2f 6a73 2f73 6168 6173 2f77 696e  kko/js/sahas/win
+00018f60: 646f 7773 2f66 6f72 6d2d 7769 6e64 6f77  dows/form-window
+00018f70: 2e6a 733f 7469 6d65 7374 616d 703d 3230  .js?timestamp=20
+00018f80: 3231 3037 3139 2d31 3433 365c 223e 3c2f  210719-1436\"></
+00018f90: 7363 7269 7074 3e5c 725c 6e3c 7363 7269  script>\r\n<scri
+00018fa0: 7074 0a20 2020 2020 2020 2073 7263 3d5c  pt.        src=\
+00018fb0: 222f 6a61 7465 6b75 6b6b 6f2f 6a73 2f73  "/jatekukko/js/s
+00018fc0: 6168 6173 2f77 696e 646f 7773 2f63 6f6d  ahas/windows/com
+00018fd0: 706f 7374 2d77 696e 646f 772e 6a73 3f74  post-window.js?t
+00018fe0: 696d 6573 7461 6d70 3d32 3032 3130 3731  imestamp=2021071
+00018ff0: 392d 3134 3336 5c22 3e3c 2f73 6372 6970  9-1436\"></scrip
+00019000: 743e 5c72 5c6e 3c73 6372 6970 740a 2020  t>\r\n<script.  
+00019010: 2020 2020 2020 7372 633d 5c22 2f6a 6174        src=\"/jat
+00019020: 656b 756b 6b6f 2f6a 732f 7361 6861 732f  ekukko/js/sahas/
+00019030: 7769 6e64 6f77 732f 7265 6769 7374 6572  windows/register
+00019040: 2d77 696e 646f 772e 6a73 3f74 696d 6573  -window.js?times
+00019050: 7461 6d70 3d32 3032 3130 3731 392d 3134  tamp=20210719-14
+00019060: 3336 5c22 3e3c 2f73 6372 6970 743e 5c72  36\"></script>\r
+00019070: 5c6e 3c73 6372 6970 740a 2020 2020 2020  \n<script.      
+00019080: 2020 7372 633d 5c22 2f6a 6174 656b 756b    src=\"/jatekuk
+00019090: 6b6f 2f6a 732f 7361 6861 732f 7769 6e64  ko/js/sahas/wind
+000190a0: 6f77 732f 6372 6561 7465 2d6e 6577 2d75  ows/create-new-u
+000190b0: 7365 722d 7769 6e64 6f77 2e6a 733f 7469  ser-window.js?ti
+000190c0: 6d65 7374 616d 703d 3230 3231 3037 3139  mestamp=20210719
+000190d0: 2d31 3433 365c 223e 3c2f 7363 7269 7074  -1436\"></script
+000190e0: 3e5c 725c 6e3c 7363 7269 7074 0a20 2020  >\r\n<script.   
+000190f0: 2020 2020 2073 7263 3d5c 222f 6a61 7465       src=\"/jate
+00019100: 6b75 6b6b 6f2f 6a73 2f73 6168 6173 2f77  kukko/js/sahas/w
+00019110: 696e 646f 7773 2f65 6d61 696c 2d70 686f  indows/email-pho
+00019120: 6e65 2d77 696e 646f 772e 6a73 3f74 696d  ne-window.js?tim
+00019130: 6573 7461 6d70 3d32 3032 3130 3731 392d  estamp=20210719-
+00019140: 3134 3336 5c22 3e3c 2f73 6372 6970 743e  1436\"></script>
+00019150: 5c72 5c6e 3c73 6372 6970 740a 2020 2020  \r\n<script.    
+00019160: 2020 2020 7372 633d 5c22 2f6a 6174 656b      src=\"/jatek
+00019170: 756b 6b6f 2f6a 732f 7361 6861 732f 7769  ukko/js/sahas/wi
+00019180: 6e64 6f77 732f 6b69 6d70 616b 7369 2d77  ndows/kimpaksi-w
+00019190: 696e 646f 772e 6a73 3f74 696d 6573 7461  indow.js?timesta
+000191a0: 6d70 3d32 3032 3130 3731 392d 3134 3336  mp=20210719-1436
+000191b0: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
+000191c0: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
+000191d0: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
+000191e0: 2f6a 732f 7361 6861 732f 7769 6e64 6f77  /js/sahas/window
+000191f0: 732f 6f72 6465 722d 7769 6e64 6f77 2e6a  s/order-window.j
+00019200: 733f 7469 6d65 7374 616d 703d 3230 3231  s?timestamp=2021
+00019210: 3037 3139 2d31 3433 365c 223e 3c2f 7363  0719-1436\"></sc
+00019220: 7269 7074 3e5c 725c 6e3c 7363 7269 7074  ript>\r\n<script
+00019230: 0a20 2020 2020 2020 2073 7263 3d5c 222f  .        src=\"/
+00019240: 6a61 7465 6b75 6b6b 6f2f 6a73 2f73 6168  jatekukko/js/sah
+00019250: 6173 2f77 696e 646f 7773 2f72 6573 6967  as/windows/resig
+00019260: 6e2d 6b69 6d70 7061 2d77 696e 646f 772e  n-kimppa-window.
+00019270: 6a73 3f74 696d 6573 7461 6d70 3d32 3032  js?timestamp=202
+00019280: 3130 3731 392d 3134 3336 5c22 3e3c 2f73  10719-1436\"></s
+00019290: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
+000192a0: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
+000192b0: 2f6a 6174 656b 756b 6b6f 2f6a 732f 7361  /jatekukko/js/sa
+000192c0: 6861 732f 7769 6e64 6f77 732f 636f 6c6c  has/windows/coll
+000192d0: 6563 7469 6f6e 2d73 6368 6564 756c 652d  ection-schedule-
+000192e0: 7769 6e64 6f77 2e6a 733f 7469 6d65 7374  window.js?timest
+000192f0: 616d 703d 3230 3231 3037 3139 2d31 3433  amp=20210719-143
+00019300: 365c 223e 3c2f 7363 7269 7074 3e5c 725c  6\"></script>\r\
+00019310: 6e5c 725c 6e5c 725c 6e5c 743c 7363 7269  n\r\n\r\n\t<scri
+00019320: 7074 0a20 2020 2020 2020 2073 7263 3d5c  pt.        src=\
+00019330: 222f 6a61 7465 6b75 6b6b 6f2f 6a73 2f73  "/jatekukko/js/s
+00019340: 6168 6173 2f77 696e 646f 7773 2f72 6570  ahas/windows/rep
+00019350: 7369 6b6b 612d 7769 6e64 6f77 2e6a 733f  sikka-window.js?
+00019360: 7469 6d65 7374 616d 703d 3230 3231 3037  timestamp=202107
+00019370: 3139 2d31 3433 365c 223e 3c2f 7363 7269  19-1436\"></scri
+00019380: 7074 3e5c 725c 6e5c 725c 6e5c 725c 6e5c  pt>\r\n\r\n\r\n\
+00019390: 725c 6e5c 725c 6e5c 725c 6e5c 725c 6e5c  r\n\r\n\r\n\r\n\
+000193a0: 725c 6e5c 725c 6e5c 725c 6e5c 743c 7363  r\n\r\n\r\n\t<sc
+000193b0: 7269 7074 0a20 2020 2020 2020 2073 7263  ript.        src
+000193c0: 3d5c 222f 6a61 7465 6b75 6b6b 6f2f 6a73  =\"/jatekukko/js
+000193d0: 2f73 6168 6173 2f77 696e 646f 7773 2f77  /sahas/windows/w
+000193e0: 6173 7465 2d77 6174 6572 2d77 696e 646f  aste-water-windo
+000193f0: 772e 6a73 3f74 696d 6573 7461 6d70 3d32  w.js?timestamp=2
+00019400: 3032 3130 3731 392d 3134 3336 5c22 3e3c  0210719-1436\"><
+00019410: 2f73 6372 6970 743e 5c72 5c6e 5c72 5c6e  /script>\r\n\r\n
+00019420: 5c72 5c6e 3c73 6372 6970 740a 2020 2020  \r\n<script.    
+00019430: 2020 2020 7372 633d 5c22 2f6a 6174 656b      src=\"/jatek
+00019440: 756b 6b6f 2f6a 732f 636f 6d70 6f6e 656e  ukko/js/componen
+00019450: 7473 2f74 6162 6261 722e 6a73 3f74 696d  ts/tabbar.js?tim
+00019460: 6573 7461 6d70 3d32 3032 3130 3731 392d  estamp=20210719-
+00019470: 3134 3336 5c22 3e3c 2f73 6372 6970 743e  1436\"></script>
+00019480: 5c72 5c6e 3c73 6372 6970 740a 2020 2020  \r\n<script.    
+00019490: 2020 2020 7372 633d 5c22 2f6a 6174 656b      src=\"/jatek
+000194a0: 756b 6b6f 2f6a 732f 636f 6d70 6f6e 656e  ukko/js/componen
+000194b0: 7473 2f74 6572 6d73 2d77 696e 646f 772e  ts/terms-window.
+000194c0: 6a73 3f74 696d 6573 7461 6d70 3d32 3032  js?timestamp=202
+000194d0: 3130 3731 392d 3134 3336 5c22 3e3c 2f73  10719-1436\"></s
+000194e0: 6372 6970 743e 5c72 5c6e 3c73 6372 6970  cript>\r\n<scrip
+000194f0: 740a 2020 2020 2020 2020 7372 633d 5c22  t.        src=\"
+00019500: 2f6a 6174 656b 756b 6b6f 2f6a 732f 636f  /jatekukko/js/co
+00019510: 6d70 6f6e 656e 7473 2f74 6572 6d73 2d62  mponents/terms-b
+00019520: 616e 6e65 722e 6a73 3f74 696d 6573 7461  anner.js?timesta
+00019530: 6d70 3d32 3032 3130 3731 392d 3134 3336  mp=20210719-1436
+00019540: 5c22 3e3c 2f73 6372 6970 743e 5c72 5c6e  \"></script>\r\n
+00019550: 3c73 6372 6970 740a 2020 2020 2020 2020  <script.        
+00019560: 7372 633d 5c22 2f6a 6174 656b 756b 6b6f  src=\"/jatekukko
+00019570: 2f6a 732f 636f 6d70 6f6e 656e 7473 2f76  /js/components/v
+00019580: 6964 656f 2d70 6f70 7570 2e6a 733f 7469  ideo-popup.js?ti
+00019590: 6d65 7374 616d 703d 3230 3231 3037 3139  mestamp=20210719
+000195a0: 2d31 3433 365c 223e 3c2f 7363 7269 7074  -1436\"></script
+000195b0: 3e5c 725c 6e5c 725c 6e5c 725c 6e5c 725c  >\r\n\r\n\r\n\r\
+000195c0: 6e3c 7363 7269 7074 0a20 2020 2020 2020  n<script.       
+000195d0: 2074 7970 653d 5c22 7465 7874 2f6a 6176   type=\"text/jav
+000195e0: 6173 6372 6970 745c 223e 5c72 5c6e 5c74  ascript\">\r\n\t
+000195f0: 7661 7220 6261 7365 7572 6c20 3d20 5c22  var baseurl = \"
+00019600: 2f6a 6174 656b 756b 6b6f 5c22 3b5c 725c  /jatekukko\";\r\
+00019610: 6e5c 725c 6e5c 7477 696e 646f 772e 6468  n\r\n\twindow.dh
+00019620: 785f 676c 6f62 616c 496d 6750 6174 680a  x_globalImgPath.
+00019630: 2020 2020 2020 2020 3d20 5c22 2f6a 6174          = \"/jat
+00019640: 656b 756b 6b6f 2f6a 732f 6468 746d 6c78  ekukko/js/dhtmlx
+00019650: 5375 6974 652f 6468 746d 6c78 436f 6d62  Suite/dhtmlxComb
+00019660: 6f2f 636f 6465 6261 7365 2f69 6d67 732f  o/codebase/imgs/
+00019670: 5c22 3b5c 725c 6e5c 725c 6e5c 7473 6974  \";\r\n\r\n\tsit
+00019680: 654c 616e 6775 6167 653d 0a20 2020 2020  eLanguage=.     
+00019690: 2020 205c 2266 695f 4649 5c22 3b5c 725c     \"fi_FI\";\r\
+000196a0: 6e5c 745c 725c 6e5c 745c 725c 6e3c 2f73  n\t\r\n\t\r\n</s
+000196b0: 6372 6970 743e 5c72 5c6e 5c72 5c6e 3c73  cript>\r\n\r\n<s
+000196c0: 6372 6970 7420 7372 633d 5c22 2f6a 6174  cript src=\"/jat
+000196d0: 656b 756b 6b6f 2f6a 732f 7361 6861 732f  ekukko/js/sahas/
+000196e0: 6d61 696e 2e6a 733f 7469 6d65 7374 616d  main.js?timestam
+000196f0: 703d 3230 3231 3037 3139 2d31 3433 365c  p=20210719-1436\
+00019700: 223e 3c2f 7363 7269 7074 3e5c 725c 6e5c  "></script>\r\n\
+00019710: 725c 6e5c 725c 6e3c 7363 7269 7074 3e5c  r\n\r\n<script>\
+00019720: 725c 6e0a 2020 2020 2020 2020 5c20 2866  r\n.        \ (f
+00019730: 756e 6374 696f 6e28 692c 732c 6f2c 672c  unction(i,s,o,g,
+00019740: 722c 612c 6d29 7b69 5b27 476f 6f67 6c65  r,a,m){i['Google
+00019750: 416e 616c 7974 6963 734f 626a 6563 7427  AnalyticsObject'
+00019760: 5d3d 723b 695b 725d 3d69 5b72 5d7c 7c66  ]=r;i[r]=i[r]||f
+00019770: 756e 6374 696f 6e28 297b 5c72 5c6e 0a20  unction(){\r\n. 
+00019780: 2020 2020 2020 205c 2028 695b 725d 2e71         \ (i[r].q
+00019790: 3d69 5b72 5d2e 717c 7c5b 5d29 2e70 7573  =i[r].q||[]).pus
+000197a0: 6828 6172 6775 6d65 6e74 7329 7d2c 695b  h(arguments)},i[
+000197b0: 725d 2e6c 3d31 2a6e 6577 2044 6174 6528  r].l=1*new Date(
+000197c0: 293b 613d 732e 6372 6561 7465 456c 656d  );a=s.createElem
+000197d0: 656e 7428 6f29 2c5c 725c 6e0a 2020 2020  ent(o),\r\n.    
+000197e0: 2020 2020 5c20 6d3d 732e 6765 7445 6c65      \ m=s.getEle
+000197f0: 6d65 6e74 7342 7954 6167 4e61 6d65 286f  mentsByTagName(o
+00019800: 295b 305d 3b61 2e61 7379 6e63 3d31 3b61  )[0];a.async=1;a
+00019810: 2e73 7263 3d67 3b6d 2e70 6172 656e 744e  .src=g;m.parentN
+00019820: 6f64 652e 696e 7365 7274 4265 666f 7265  ode.insertBefore
+00019830: 2861 2c6d 295c 725c 6e0a 2020 2020 2020  (a,m)\r\n.      
+00019840: 2020 5c20 7d29 2877 696e 646f 772c 646f    \ })(window,do
+00019850: 6375 6d65 6e74 2c27 7363 7269 7074 272c  cument,'script',
+00019860: 272f 2f77 7777 2e67 6f6f 676c 652d 616e  '//www.google-an
+00019870: 616c 7974 6963 732e 636f 6d2f 616e 616c  alytics.com/anal
+00019880: 7974 6963 732e 6a73 272c 2767 6127 293b  ytics.js','ga');
+00019890: 5c72 5c6e 5c72 5c6e 0a20 2020 2020 2020  \r\n\r\n.       
+000198a0: 205c 2067 6128 2763 7265 6174 6527 2c20   \ ga('create', 
+000198b0: 2755 412d 3335 3935 3638 3232 2d31 3127  'UA-35956822-11'
+000198c0: 2c20 2761 7574 6f27 293b 5c72 5c6e 2020  , 'auto');\r\n  
+000198d0: 6761 2827 7365 6e64 272c 2027 7061 6765  ga('send', 'page
+000198e0: 7669 6577 2729 3b5c 725c 6e3c 2f73 6372  view');\r\n</scr
+000198f0: 6970 743e 5c72 5c6e 5c72 5c6e 5c72 5c6e  ipt>\r\n\r\n\r\n
+00019900: 5c72 5c6e 0a20 2020 2020 2020 205c 2020  \r\n.        \  
+00019910: 2020 2020 203c 7363 7269 7074 3e5c 725c       <script>\r\
+00019920: 6e5c 745c 7424 2827 7365 6374 696f 6e23  n\t\t$('section#
+00019930: 6c6f 6769 6e20 2e6e 6176 2d74 6162 7320  login .nav-tabs 
+00019940: 6127 292e 636c 6963 6b28 6675 6e63 7469  a').click(functi
+00019950: 6f6e 2028 6529 0a20 2020 2020 2020 207b  on (e).        {
+00019960: 5c72 5c6e 5c74 5c74 2020 652e 7072 6576  \r\n\t\t  e.prev
+00019970: 656e 7444 6566 6175 6c74 2829 5c72 5c6e  entDefault()\r\n
+00019980: 5c74 5c74 2020 2428 7468 6973 292e 7461  \t\t  $(this).ta
+00019990: 6228 2773 686f 7727 295c 725c 6e5c 745c  b('show')\r\n\t\
+000199a0: 747d 293b 5c72 5c6e 5c74 3c2f 7363 7269  t});\r\n\t</scri
+000199b0: 7074 3e5c 725c 6e5c 725c 6e0a 2020 2020  pt>\r\n\r\n.    
+000199c0: 2020 2020 5c20 2020 3c73 6372 6970 743e      \   <script>
+000199d0: 5c72 5c6e 2020 2020 2020 2020 6966 2028  \r\n        if (
+000199e0: 2161 7070 6c69 6361 7469 6f6e 2e69 7342  !application.isB
+000199f0: 726f 7773 6572 436f 6d70 6174 6962 6c65  rowserCompatible
+00019a00: 2829 2920 7b5c 725c 6e20 2020 2020 2020  ()) {\r\n       
+00019a10: 2020 2020 2024 2827 2362 726f 7773 6572       $('#browser
+00019a20: 2d69 6e63 6f6d 7061 7469 626c 652d 6d65  -incompatible-me
+00019a30: 7373 6167 6527 292e 7368 6f77 2829 3b5c  ssage').show();\
+00019a40: 725c 6e0a 2020 2020 2020 2020 5c20 2020  r\n.        \   
+00019a50: 2020 2020 7d5c 725c 6e5c 725c 6e20 2020      }\r\n\r\n   
+00019a60: 2020 2020 2066 756e 6374 696f 6e20 7365       function se
+00019a70: 7442 6f64 7950 6164 6469 6e67 466f 7246  tBodyPaddingForF
+00019a80: 6f6f 7465 7228 2920 7b5c 725c 6e20 2020  ooter() {\r\n   
+00019a90: 2020 2020 2020 2020 2076 6172 0a20 2020           var.   
+00019aa0: 2020 2020 2066 6f6f 7465 7248 6569 6768       footerHeigh
+00019ab0: 7420 3d20 2428 2762 6f64 7920 3e20 666f  t = $('body > fo
+00019ac0: 6f74 6572 2729 2e68 6569 6768 7428 293b  oter').height();
+00019ad0: 5c72 5c6e 2020 2020 2020 2020 2020 2020  \r\n            
+00019ae0: 2428 2762 6f64 7927 292e 6373 7328 2770  $('body').css('p
+00019af0: 6164 6469 6e67 2d62 6f74 746f 6d27 2c0a  adding-bottom',.
+00019b00: 2020 2020 2020 2020 666f 6f74 6572 4865          footerHe
+00019b10: 6967 6874 202b 2027 7078 2729 3b5c 725c  ight + 'px');\r\
+00019b20: 6e20 2020 2020 2020 207d 5c72 5c6e 5c72  n        }\r\n\r
+00019b30: 5c6e 2020 2020 2020 2020 2428 7769 6e64  \n        $(wind
+00019b40: 6f77 292e 6f6e 2827 7265 7369 7a65 272c  ow).on('resize',
+00019b50: 2073 6574 426f 6479 5061 6464 696e 6746   setBodyPaddingF
+00019b60: 6f72 466f 6f74 6572 293b 5c72 5c6e 0a20  orFooter);\r\n. 
+00019b70: 2020 2020 2020 205c 2020 2020 2020 2073         \       s
+00019b80: 6574 426f 6479 5061 6464 696e 6746 6f72  etBodyPaddingFor
+00019b90: 466f 6f74 6572 2829 3b5c 725c 6e20 2020  Footer();\r\n   
+00019ba0: 203c 2f73 6372 6970 743e 5c72 5c6e 2020   </script>\r\n  
+00019bb0: 2020 3c2f 626f 6479 3e5c 725c 6e20 2020    </body>\r\n   
+00019bc0: 203c 2f68 746d 6c3e 5c72 5c6e 5c72 5c6e   </html>\r\n\r\n
+00019bd0: 220a 2020 2020 6865 6164 6572 733a 0a20  ".    headers:. 
+00019be0: 2020 2020 2043 6f6e 6e65 6374 696f 6e3a       Connection:
+00019bf0: 0a20 2020 2020 202d 206b 6565 702d 616c  .      - keep-al
+00019c00: 6976 650a 2020 2020 2020 436f 6e74 656e  ive.      Conten
+00019c10: 742d 456e 636f 6469 6e67 3a0a 2020 2020  t-Encoding:.    
+00019c20: 2020 2d20 677a 6970 0a20 2020 2020 2043    - gzip.      C
+00019c30: 6f6e 7465 6e74 2d4c 616e 6775 6167 653a  ontent-Language:
+00019c40: 0a20 2020 2020 202d 2066 692d 4649 0a20  .      - fi-FI. 
+00019c50: 2020 2020 2043 6f6e 7465 6e74 2d53 6563       Content-Sec
+00019c60: 7572 6974 792d 506f 6c69 6379 3a0a 2020  urity-Policy:.  
+00019c70: 2020 2020 2d20 6672 616d 652d 616e 6365      - frame-ance
+00019c80: 7374 6f72 7320 276e 6f6e 6527 0a20 2020  stors 'none'.   
+00019c90: 2020 2043 6f6e 7465 6e74 2d54 7970 653a     Content-Type:
+00019ca0: 0a20 2020 2020 202d 2074 6578 742f 6874  .      - text/ht
+00019cb0: 6d6c 3b63 6861 7273 6574 3d75 7466 2d38  ml;charset=utf-8
+00019cc0: 0a20 2020 2020 2044 6174 653a 0a20 2020  .      Date:.   
+00019cd0: 2020 202d 2053 6174 2c20 3034 2053 6570     - Sat, 04 Sep
+00019ce0: 2032 3032 3120 3038 3a35 383a 3331 2047   2021 08:58:31 G
+00019cf0: 4d54 0a20 2020 2020 2053 6572 7665 723a  MT.      Server:
+00019d00: 0a20 2020 2020 202d 206e 6769 6e78 0a20  .      - nginx. 
+00019d10: 2020 2020 2053 7472 6963 742d 5472 616e       Strict-Tran
+00019d20: 7370 6f72 742d 5365 6375 7269 7479 3a0a  sport-Security:.
+00019d30: 2020 2020 2020 2d20 6d61 782d 6167 653d        - max-age=
+00019d40: 3633 3037 3230 3030 0a20 2020 2020 2054  63072000.      T
+00019d50: 7261 6e73 6665 722d 456e 636f 6469 6e67  ransfer-Encoding
+00019d60: 3a0a 2020 2020 2020 2d20 6368 756e 6b65  :.      - chunke
+00019d70: 640a 2020 2020 2020 582d 4672 616d 652d  d.      X-Frame-
+00019d80: 4f70 7469 6f6e 733a 0a20 2020 2020 202d  Options:.      -
+00019d90: 2044 454e 590a 2020 2020 2020 582d 506f   DENY.      X-Po
+00019da0: 7765 7265 642d 4279 3a0a 2020 2020 2020  wered-By:.      
+00019db0: 2d20 2753 6572 766c 6574 2f34 2e30 204a  - 'Servlet/4.0 J
+00019dc0: 5350 2f32 2e33 2028 5061 7961 7261 2053  SP/2.3 (Payara S
+00019dd0: 6572 7665 7220 2035 2e32 3032 312e 3520  erver  5.2021.5 
+00019de0: 2362 6164 6173 7366 6973 6820 4a61 7661  #badassfish Java
+00019df0: 2f45 636c 6970 7365 204f 7065 6e4a 392f  /Eclipse OpenJ9/
+00019e00: 312e 3829 270a 2020 2020 7374 6174 7573  1.8)'.    status
+00019e10: 3a0a 2020 2020 2020 636f 6465 3a20 3230  :.      code: 20
+00019e20: 300a 2020 2020 2020 6d65 7373 6167 653a  0.      message:
+00019e30: 204f 4b0a 2020 2020 7572 6c3a 2068 7474   OK.    url: htt
+00019e40: 7073 3a2f 2f74 696c 6173 746f 2e6a 6174  ps://tilasto.jat
+00019e50: 656b 756b 6b6f 2e66 692f 6a61 7465 6b75  ekukko.fi/jateku
+00019e60: 6b6b 6f2f 7361 6861 732e 6a73 700a 7665  kko/sahas.jsp.ve
+00019e70: 7273 696f 6e3a 2031 0a                   rsion: 1.
```

### Comparing `pytekukko-0.14.0/tests/test_pytekukko.py` & `pytekukko-0.9.0/tests/test_pytekukko.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,121 +1,125 @@
 """Pytekukko tests."""
 
 import datetime
 import os
-from typing import Any, TypeVar
+from typing import Any, Dict, TypeVar
 from urllib.parse import parse_qs, quote_plus, urlparse, urlunparse
 
+import dotenv
 import pytest
 from aiohttp import ClientSession
 
 from pytekukko import Pytekukko
-from pytekukko.examples import load_pytekukko_dotenv
 
-T = TypeVar("T", bound=dict[str, Any])
+T = TypeVar("T", bound=Dict[str, Any])  # pylint: disable=invalid-name
 
 FAKE_CUSTOMER_NUMBER = "00-0000000-00"
 FAKE_PASSWORD = "secret"  # noqa: S105
 FAKE_POS = "1234"
 
 QUERY_PARAMETER_FILTERS = [
     ("customerId", FAKE_CUSTOMER_NUMBER),
     ("customerNumber", FAKE_CUSTOMER_NUMBER),
     ("pos", FAKE_POS),
 ]
-POST_DATA_FILTERS = [
-    ("j_username", FAKE_CUSTOMER_NUMBER),
-    ("j_password", FAKE_PASSWORD),
-]
 
 
 def before_record_response(response: T) -> T:
     """Scrub unwanted data before recording response."""
+
     response["headers"].pop("Set-Cookie", None)
 
-    # As of vcrpy 5.0.0, filter_query_parameters does not affect
-    # parameters in response["url"], so address them here.
-    # Refs https://github.com/kevin1024/vcrpy/issues/517
+    # As of vcrpy 4.1.1, query parameters filtered with filter_query_parameters
+    # do not end up filtered in response["url"], so address them here.
     url_parts = urlparse(response["url"])
-    new_query_parts: list[str] = []
+    new_query_parts = []
     query_params = parse_qs(url_parts.query)
     for key, values in query_params.items():
         for filter_key, filter_value in QUERY_PARAMETER_FILTERS:
             if key == filter_key:
-                values = [filter_value]  # noqa: PLW2901
-        new_query_parts.extend(
-            f"{quote_plus(key)}={quote_plus(value)}" for value in values
-        )
+                values = [filter_value]
+        for value in values:
+            new_query_parts.append(f"{quote_plus(key)}={quote_plus(value)}")
     new_url_parts = list(url_parts)
     new_url_parts[4] = "&".join(new_query_parts)
     response["url"] = urlunparse(new_url_parts)
 
     if response["url"].endswith("/login.do"):
         response["body"]["string"] = b"redacted"  # unused, bloats cassettes
 
     return response
 
 
 @pytest.fixture(scope="module", autouse=True)
-def _load_dotenv() -> None:
-    """Load our environment."""
-    _ = load_pytekukko_dotenv()
+def load_dotenv() -> None:
+    """Load environment."""
+    dotenv.load_dotenv()
 
 
 @pytest.fixture(scope="module")
-def vcr_config() -> dict[str, Any]:
+def vcr_config() -> Dict[str, Any]:
     """Get vcrpy configuration."""
     return {
         "before_record_response": before_record_response,
         "filter_headers": ["Cookie"],
         "filter_query_parameters": QUERY_PARAMETER_FILTERS,
-        "filter_post_data_parameters": POST_DATA_FILTERS,
+        # NOTE: this should be uncommented when upgrading vcrpy to a fixed > 4.1.1:
+        #   https://github.com/kevin1024/vcrpy/issues/398
+        #   https://github.com/kevin1024/vcrpy/pull/582
+        #   https://github.com/kevin1024/vcrpy/pull/581
+        # "filter_post_data_parameters": ["j_username", "j_password"],
     }
 
 
-@pytest.fixture(name="client")
+@pytest.fixture(name="client", scope="function")
 async def fixture_client() -> Pytekukko:
     """Get a client."""
     return Pytekukko(
         session=ClientSession(),
         customer_number=os.environ.get(
-            "PYTEKUKKO_CUSTOMER_NUMBER",
-            FAKE_CUSTOMER_NUMBER,
+            "PYTEKUKKO_CUSTOMER_NUMBER", FAKE_CUSTOMER_NUMBER
         ),
         password=os.environ.get("PYTEKUKKO_PASSWORD", FAKE_PASSWORD),
     )
 
 
-@pytest.mark.vcr()
-async def test_login_logout(client: Pytekukko) -> None:
-    """Test login followed by logout."""
+@pytest.mark.asyncio
+@pytest.mark.vcr
+async def test_login(client: Pytekukko) -> None:
+    """Test login."""
     async with client.session:
-        assert await client.login()
-        await client.logout()  # No exception counts as success here
+        result = await client.login()
+    assert result
 
 
-@pytest.mark.vcr()
+@pytest.mark.asyncio
+@pytest.mark.vcr
 async def test_logout(client: Pytekukko) -> None:
-    """Test bare logout."""
+    """Test logout."""
+    # TODO(scop): would be better to test from a logged in session
     async with client.session:
-        await client.logout()  # No exception counts as success here
+        await client.logout()
+    # No exception counts as success here
 
 
-@pytest.mark.vcr()
+@pytest.mark.asyncio
+@pytest.mark.vcr
 async def test_get_collection_schedule(client: Pytekukko) -> None:
     """Test getting collection schedule."""
     async with client.session:
         dates = await client.get_collection_schedule(
-            what=int(os.environ.get("PYTEKUKKO_TEST_POS", FAKE_POS)),
+            what=int(os.environ.get("PYTEKUKKO_TEST_POS", FAKE_POS))
         )
     assert dates
     assert all(isinstance(date, datetime.date) for date in dates)
 
 
-@pytest.mark.vcr()
+@pytest.mark.asyncio
+@pytest.mark.vcr
 async def test_get_invoice_headers(client: Pytekukko) -> None:
     """Test getting invoice headers."""
     async with client.session:
         invoice_headers = await client.get_invoice_headers()
     assert invoice_headers
     assert all(invoice_header.raw_data for invoice_header in invoice_headers)
     assert all(invoice_header.name for invoice_header in invoice_headers)
```

