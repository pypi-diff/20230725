# Comparing `tmp/nsdotpy-2.0.0.tar.gz` & `tmp/nsdotpy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-2.0.0.tar", max compression
+gzip compressed data, was "nsdotpy-2.1.0.tar", max compression
```

## Comparing `nsdotpy-2.0.0.tar` & `nsdotpy-2.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-06-20 03:08:11.893972 nsdotpy-2.0.0/LICENSE.md
--rw-r--r--   0        0        0     2847 2023-06-20 03:08:11.893972 nsdotpy-2.0.0/README.md
--rw-r--r--   0        0        0      787 2023-06-20 03:08:11.909972 nsdotpy-2.0.0/nsdotpy/__init__.py
--rw-r--r--   0        0        0    49237 2023-06-20 03:08:11.909972 nsdotpy-2.0.0/nsdotpy/session.py
--rw-r--r--   0        0        0     5033 2023-06-20 03:08:11.909972 nsdotpy-2.0.0/nsdotpy/valid.py
--rw-r--r--   0        0        0      786 2023-06-20 03:08:11.909972 nsdotpy-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3822 1970-01-01 00:00:00.000000 nsdotpy-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-07-25 02:56:57.548869 nsdotpy-2.1.0/LICENSE.md
+-rw-r--r--   0        0        0     2847 2023-07-25 02:56:57.548869 nsdotpy-2.1.0/README.md
+-rw-r--r--   0        0        0      787 2023-07-25 02:56:57.568869 nsdotpy-2.1.0/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    59057 2023-07-25 02:56:57.568869 nsdotpy-2.1.0/nsdotpy/session.py
+-rw-r--r--   0        0        0     5033 2023-07-25 02:56:57.568869 nsdotpy-2.1.0/nsdotpy/valid.py
+-rw-r--r--   0        0        0      786 2023-07-25 02:56:57.568869 nsdotpy-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3822 1970-01-01 00:00:00.000000 nsdotpy-2.1.0/PKG-INFO
```

### Comparing `nsdotpy-2.0.0/LICENSE.md` & `nsdotpy-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-2.0.0/README.md` & `nsdotpy-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-2.0.0/nsdotpy/__init__.py` & `nsdotpy-2.1.0/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-2.0.0/nsdotpy/session.py` & `nsdotpy-2.1.0/nsdotpy/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "2.0.0"
+        self.VERSION = "2.1.0"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -251,14 +251,26 @@
                 raise ValueError(f"{key} should have a minimum length of 2 characters.")
             # check if pretitle contains any non-alphanumeric characters (except spaces)
             if key == "pretitle" and not value.replace(" ", "").isalnum():
                 raise ValueError(
                     "Pretitle should only contain alphanumeric characters or spaces."
                 )
 
+    def _wait_for_ratelimit(self, head: dict, constant_rate_limit: bool):
+        if "X-Pin" in head:
+            self.pin = head["X-Pin"]
+        if waiting_time := head.get("Retry-After"):
+            self.logger.warning(f"Rate limited. Waiting {waiting_time} seconds.")
+            time.sleep(int(waiting_time))
+        # slow down requests so we dont hit the rate limit in the first place
+        requests_left = int(head["RateLimit-Remaining"])
+        if requests_left < 10 or constant_rate_limit:
+            seconds_until_reset = int(head["RateLimit-Reset"])
+            time.sleep(seconds_until_reset / requests_left)
+
     def _html_request(
         self, url, data={}, files=None, follow_redirects=False
     ) -> httpx.Response:
         data |= {"chk": self.chk, "localid": self.localid}
         userclick = self._wait_for_input(self.keybind)
         # userclick is the number of milliseconds since the epoch, admin uses this for help enforcing the simultaneity rule
         response = self._session.post(
@@ -384,32 +396,221 @@
         if password:
             self._session.headers["X-Password"] = password
         if self.pin:
             self._session.headers["X-Pin"] = self.pin
         # rate limiting section
         response = self._session.post(url, data=data)
         # if the server tells us to wait, wait
-        head = response.headers
-        if "X-Pin" in head:
-            self.pin = head["X-Pin"]
-        if waiting_time := head.get("Retry-After"):
-            self.logger.warning(f"Rate limited. Waiting {waiting_time} seconds.")
-            time.sleep(int(waiting_time))
-        # slow down requests so we dont hit the rate limit in the first place
-        requests_left = int(head["RateLimit-Remaining"])
-        if requests_left < 10 or constant_rate_limit:
-            seconds_until_reset = int(head["RateLimit-Reset"])
-            time.sleep(seconds_until_reset / requests_left)
-        # end rate limiting section
+        self._wait_for_ratelimit(response.headers, constant_rate_limit)
         response.raise_for_status()
         parsed_response = benedict.from_xml(response.text, keyattr_dynamic=True)
         parsed_response.standardize()
         parsed_response: benedict = parsed_response[api]  # type: ignore
         return parsed_response
 
+    def api_issue(
+        self,
+        nation: str,
+        issue: int,
+        option: int,
+        password: str = "",
+        constant_rate_limit: bool = False,
+    ) -> benedict:
+        """Answers an issue via the API.
+
+        Args:
+            nation (str): The nation to perform the command with.
+            issue (int): the ID of the issue.
+            option (int): the issue option to choose.
+            password (str, optional): The password to use for authenticating private api requests. Defaults to "". Not required if already signed in, whether through the api or through the HTML site.
+            constant_rate_limit (bool, optional): If True, will always rate limit. If False, will only rate limit when there's less than 10 requests left in the current bucket. Defaults to False.
+
+        Returns:
+            benedict: A benedict object containing the response from the server. Acts like a dictionary, with keypath and keylist support.
+        """
+        if not (password or self.pin):
+            raise ValueError("must specify authentication")
+        data = {
+            "v": "12",
+            "c": "issue",
+            "nation": canonicalize(nation),
+            "issue": issue,
+            "option": option,
+        }
+        url = "https://www.nationstates.net/cgi-bin/api.cgi"
+        if password:
+            self._session.headers["X-Password"] = password
+        if self.pin:
+            self._session.headers["X-Pin"] = self.pin
+        # rate limiting section
+        response = self._session.get(url, params=data)
+        # if the server tells us to wait, wait
+        self._wait_for_ratelimit(response.headers, constant_rate_limit)
+        response.raise_for_status()
+        parsed_response = benedict.from_xml(response.text, keyattr_dynamic=True)
+        parsed_response.standardize()
+        parsed_response: benedict = parsed_response["nation"]  # type: ignore
+        return parsed_response
+
+    def api_command(
+        self,
+        nation: str,
+        command: str,
+        data: dict,
+        password: str = "",
+        mode: str = "",
+        constant_rate_limit: bool = False,
+    ) -> benedict:
+        """Sends a non-issue command to the nationstates api with the given data and password.
+
+        Args:
+            nation (str): The nation to perform the command with.
+            command (str): The command to perform. Must be "giftcard", "dispatch", "rmbpost"
+            data (str, optional): The unique data to send with the parameters of the command; consult the API docs for more information.
+            password (str, optional): The password to use for authenticating private api requests. Defaults to "". Not required if already signed in, whether through the api or through the HTML site.
+            mode (str, optional): Whether to prepare or to execute the command. If value is given, does one of the two and returns result, if no value is given, does both and returns result of execute.
+            constant_rate_limit (bool, optional): If True, will always rate limit. If False, will only rate limit when there's less than 10 requests left in the current bucket. Defaults to False.
+
+        Returns:
+            benedict: A benedict object containing the response from the server. Acts like a dictionary, with keypath and keylist support.
+        """
+        if command not in {"giftcard", "dispatch", "rmbpost"}:
+            raise ValueError("command must be 'giftcard', 'dispatch', or 'rmbpost'")
+        if not (password or self.pin):
+            raise ValueError("must specify authentication")
+        if mode not in {"", "prepare", "execute"}:
+            raise ValueError("mode must be prepare or execute")
+        data["v"] = "12"
+        data["nation"] = canonicalize(nation)
+        data["c"] = command
+        data["mode"] = mode if mode else "prepare"  # if no mode than first prepare
+        url = "https://www.nationstates.net/cgi-bin/api.cgi"
+        if password:
+            self._session.headers["X-Password"] = password
+        if self.pin:
+            self._session.headers["X-Pin"] = self.pin
+        # rate limiting section
+        response = self._session.get(url, params=data)
+        # if the server tells us to wait, wait
+        self._wait_for_ratelimit(response.headers, constant_rate_limit)
+        response.raise_for_status()
+        parsed_response = benedict.from_xml(response.text, keyattr_dynamic=True)
+        parsed_response.standardize()
+        parsed_response: benedict = parsed_response["nation"]  # type: ignore
+        if mode == "":
+            # if no mode was specified earlier, repeat command with execute and token
+            data["token"] = parsed_response["success"]
+            return self.api_command(nation, command, data, mode="execute")
+        else:
+            return parsed_response
+
+    def api_giftcard(
+        self,
+        nation: str,
+        card_id: int,
+        season: int,
+        recipient: str,
+        password: str = "",
+        constant_rate_limit: bool = False,
+    ) -> benedict:
+        """Gifts a card using the API.
+
+        Args:
+            nation (str): The nation to perform the command with.
+            card_id (int): The ID of the card to gift.
+            season (int): The season of the card to gift.
+            recipient (str): The nation to gift the card to.
+            password (str, optional): The password to use for authenticating private api requests. Defaults to "". Not required if already signed in, whether through the api or through the HTML site.
+            constant_rate_limit (bool, optional): If True, will always rate limit. If False, will only rate limit when there's less than 10 requests left in the current bucket. Defaults to False.
+
+        Returns:
+            benedict: A benedict object containing the response from the server. Acts like a dictionary, with keypath and keylist support.
+        """
+        data = {"cardid": card_id, "season": season, "to": canonicalize(recipient)}
+        return self.api_command(
+            nation, "giftcard", data, password, constant_rate_limit=constant_rate_limit
+        )
+
+    def api_dispatch(
+        self,
+        nation: str,
+        action: str,
+        title: str = "",
+        text: str = "",
+        category: int = 0,
+        subcategory: int = 0,
+        dispatchid: int = 0,
+        password: str = "",
+        constant_rate_limit: bool = False,
+    ) -> benedict:
+        """Add, edit, or remove a dispatch.
+
+        Args:
+            nation (str): The nation to perform the command with.
+            action (str): The action to take. Must be "add", "edit", "remove"
+            title (str, optional): The dispatch title when adding or editing.
+            text (str, optional): The dispatch text when adding or editing.
+            category: (int, optional), The category ID when adding or editing.
+            subcategory (int, optional): The subcategory ID when adding or editing.
+            dispatchid (int, optional): The dispatch ID when editing or removing.
+            password (str, optional): The password to use for authenticating private api requests. Defaults to "". Not required if already signed in, whether through the api or through the HTML site.
+            constant_rate_limit (bool, optional): If True, will always rate limit. If False, will only rate limit when there's less than 10 requests left in the current bucket. Defaults to False.
+
+        Returns:
+            benedict: A benedict object containing the response from the server. Acts like a dictionary, with keypath and keylist support.
+        """
+        # TODO: maybe consider splitting these three functions?
+        # TODO: maybe create enums for category and subcategory
+        if action not in {"add", "edit", "remove"}:
+            raise ValueError("action must be 'add', 'edit', or 'remove'")
+        if action != "remove" and not all({title, text, category, subcategory}):
+            raise ValueError("must specify title, text, category, and subcategory")
+        if action != "add" and not dispatchid:
+            raise ValueError("must specify a dispatch id")
+
+        data = {"dispatch": action}
+        if title:
+            data["title"] = title
+        if text:
+            data["text"] = text
+        if category:
+            data["category"] = category
+        if subcategory:
+            data["subcategory"] = subcategory
+        if dispatchid:
+            data["dispatchid"] = dispatchid
+        return self.api_command(
+            nation, "dispatch", data, password, constant_rate_limit=constant_rate_limit
+        )
+
+    def api_rmb(
+        self,
+        nation: str,
+        region: str,
+        text: str,
+        password: str = "",
+        constant_rate_limit: bool = False,
+    ) -> benedict:
+        """Post a message on the regional message board via the API.
+
+        Args:
+            nation (str): The nation to perform the command with.
+            region (str): the region to post the message in.
+            text (str): the text to post.
+            password (str, optional): The password to use for authenticating private api requests. Defaults to "". Not required if already signed in, whether through the api or through the HTML site.
+            constant_rate_limit (bool, optional): If True, will always rate limit. If False, will only rate limit when there's less than 10 requests left in the current bucket. Defaults to False.
+
+        Returns:
+            benedict: A benedict object containing the response from the server. Acts like a dictionary, with keypath and keylist support.
+        """
+        data = {"region": region, "text": text}
+        return self.api_command(
+            nation, "rmbpost", data, password, constant_rate_limit=constant_rate_limit
+        )
+
     def login(self, nation: str, password: str) -> bool:
         """Logs in to the nationstates site.
 
         Args:
             nation (str): Nation name
             password (str): Nation password
```

### Comparing `nsdotpy-2.0.0/nsdotpy/valid.py` & `nsdotpy-2.1.0/nsdotpy/valid.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-2.0.0/pyproject.toml` & `nsdotpy-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "2.0.0"
+version = "2.1.0"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-2.0.0/PKG-INFO` & `nsdotpy-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 2.0.0
+Version: 2.1.0
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

