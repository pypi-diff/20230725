# Comparing `tmp/imap-tools-1.0.0.tar.gz` & `tmp/imap-tools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imap-tools-1.0.0.tar", last modified: Mon Nov 21 11:58:04 2022, max compression
+gzip compressed data, was "dist\imap-tools-1.1.0.tar", last modified: Tue Jul 25 09:15:33 2023, max compression
```

## Comparing `imap-tools-1.0.0.tar` & `imap-tools-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-11-21 11:58:04.000000 imap-tools-1.0.0/
-drwxrwxrwx   0        0        0        0 2022-11-21 11:58:04.000000 imap-tools-1.0.0/imap_tools/
--rw-rw-rw-   0        0        0     1209 2022-03-06 11:54:23.000000 imap-tools-1.0.0/imap_tools/consts.py
--rw-rw-rw-   0        0        0     2109 2022-02-15 11:27:46.000000 imap-tools-1.0.0/imap_tools/errors.py
--rw-rw-rw-   0        0        0     7084 2022-03-14 10:53:53.000000 imap-tools-1.0.0/imap_tools/folder.py
--rw-rw-rw-   0        0        0     4465 2022-11-21 11:14:06.000000 imap-tools-1.0.0/imap_tools/idle.py
--rw-rw-rw-   0        0        0     2059 2021-09-20 07:00:52.000000 imap-tools-1.0.0/imap_tools/imap_utf7.py
--rw-rw-rw-   0        0        0    16193 2022-08-31 05:00:37.000000 imap-tools-1.0.0/imap_tools/mailbox.py
--rw-rw-rw-   0        0        0     9662 2021-11-25 11:36:59.000000 imap-tools-1.0.0/imap_tools/message.py
--rw-rw-rw-   0        0        0    16320 2022-08-31 05:00:37.000000 imap-tools-1.0.0/imap_tools/query.py
--rw-rw-rw-   0        0        0     7386 2022-08-31 05:00:37.000000 imap-tools-1.0.0/imap_tools/utils.py
--rw-rw-rw-   0        0        0      522 2022-11-21 11:08:33.000000 imap-tools-1.0.0/imap_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-21 11:58:04.000000 imap-tools-1.0.0/imap_tools.egg-info/
--rw-rw-rw-   0        0        0        1 2022-11-21 11:58:03.000000 imap-tools-1.0.0/imap_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    20543 2022-11-21 11:58:03.000000 imap-tools-1.0.0/imap_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2022-11-21 11:58:03.000000 imap-tools-1.0.0/imap_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2022-11-21 11:58:03.000000 imap-tools-1.0.0/imap_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11548 2019-10-23 05:52:39.000000 imap-tools-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       56 2021-01-28 06:25:19.000000 imap-tools-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    20543 2022-11-21 11:58:04.000000 imap-tools-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    20033 2022-08-31 04:52:48.000000 imap-tools-1.0.0/README.rst
--rw-rw-rw-   0        0        0       42 2022-11-21 11:58:04.000000 imap-tools-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1125 2021-08-06 04:21:06.000000 imap-tools-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:15:33.000000 imap-tools-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools/
+-rw-rw-rw-   0        0        0     1209 2022-03-06 11:54:23.000000 imap-tools-1.1.0/imap_tools/consts.py
+-rw-rw-rw-   0        0        0     2109 2022-02-15 11:27:46.000000 imap-tools-1.1.0/imap_tools/errors.py
+-rw-rw-rw-   0        0        0     7084 2022-03-14 10:53:53.000000 imap-tools-1.1.0/imap_tools/folder.py
+-rw-rw-rw-   0        0        0     4465 2022-11-21 11:14:06.000000 imap-tools-1.1.0/imap_tools/idle.py
+-rw-rw-rw-   0        0        0     2059 2021-09-20 07:00:52.000000 imap-tools-1.1.0/imap_tools/imap_utf7.py
+-rw-rw-rw-   0        0        0    15852 2023-07-25 09:13:31.000000 imap-tools-1.1.0/imap_tools/mailbox.py
+-rw-rw-rw-   0        0        0     9662 2021-11-25 11:36:59.000000 imap-tools-1.1.0/imap_tools/message.py
+-rw-rw-rw-   0        0        0    16320 2022-08-31 05:00:37.000000 imap-tools-1.1.0/imap_tools/query.py
+-rw-rw-rw-   0        0        0     7386 2022-08-31 05:00:37.000000 imap-tools-1.1.0/imap_tools/utils.py
+-rw-rw-rw-   0        0        0      522 2023-07-25 09:13:31.000000 imap-tools-1.1.0/imap_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    20633 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 09:15:33.000000 imap-tools-1.1.0/imap_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11548 2019-10-23 05:52:39.000000 imap-tools-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       56 2021-01-28 06:25:19.000000 imap-tools-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    20633 2023-07-25 09:15:33.000000 imap-tools-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    20123 2023-07-25 09:13:31.000000 imap-tools-1.1.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-25 09:15:33.000000 imap-tools-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2021-08-06 04:21:06.000000 imap-tools-1.1.0/setup.py
```

### Comparing `imap-tools-1.0.0/imap_tools/consts.py` & `imap-tools-1.1.0/imap_tools/consts.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.0.0/imap_tools/errors.py` & `imap-tools-1.1.0/imap_tools/errors.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.0.0/imap_tools/folder.py` & `imap-tools-1.1.0/imap_tools/folder.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.0.0/imap_tools/idle.py` & `imap-tools-1.1.0/imap_tools/idle.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.0.0/imap_tools/imap_utf7.py` & `imap-tools-1.1.0/imap_tools/imap_utf7.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.0.0/imap_tools/mailbox.py` & `imap-tools-1.1.0/imap_tools/mailbox.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import re
 import sys
 import imaplib
 import datetime
 from collections import UserString
 from typing import AnyStr, Optional, List, Iterable, Sequence, Union, Tuple, Iterator
 
-from .consts import UID_PATTERN
 from .message import MailMessage
 from .folder import MailBoxFolderManager
 from .idle import IdleManager
-from .utils import clean_uids, check_command_status, chunks, encode_folder, clean_flags, decode_value, \
-    check_timeout_arg_support
+from .utils import clean_uids, check_command_status, chunks, encode_folder, clean_flags, check_timeout_arg_support
 from .errors import MailboxStarttlsError, MailboxLoginError, MailboxLogoutError, MailboxNumbersError, \
     MailboxFetchError, MailboxExpungeError, MailboxDeleteError, MailboxCopyError, MailboxFlagError, \
     MailboxAppendError, MailboxUidsError, MailboxTaggedResponseError
 
 # Maximal line length when calling readline(). This is to prevent reading arbitrary length lines.
 # 20Mb is enough for search response with about 2 000 000 message numbers
 imaplib._MAXLINE = 20 * 1024 * 1024  # 20Mb
@@ -96,87 +93,77 @@
         result = self.client.logout()
         check_command_status(result, MailboxLogoutError, expected='BYE')
         return result
 
     def numbers(self, criteria: Criteria = 'ALL', charset: str = 'US-ASCII') -> List[str]:
         """
         Search mailbox for matching message numbers in current folder (this is not uids)
+        Message Sequence Number Message Attribute - to accessing messages by relative position in the mailbox,
+        it also can be used in mathematical calculations, see rfc3501.
         :param criteria: message search criteria (see examples at ./doc/imap_search_criteria.txt)
         :param charset: IANA charset, indicates charset of the strings that appear in the search criteria. See rfc2978
         :return email message numbers
         """
         encoded_criteria = criteria if type(criteria) is bytes else str(criteria).encode(charset)
         search_result = self.client.search(charset, encoded_criteria)
         check_command_status(search_result, MailboxNumbersError)
         return search_result[1][0].decode().split() if search_result[1][0] else []
 
-    def uids(self, criteria: Criteria = 'ALL', charset: str = 'US-ASCII', miss_no_uid=True) -> List[str]:
+    def uids(self, criteria: Criteria = 'ALL', charset: str = 'US-ASCII') -> List[str]:
         """
         Search mailbox for matching message uids in current folder
         :param criteria: message search criteria (see examples at ./doc/imap_search_criteria.txt)
         :param charset: IANA charset, indicates charset of the strings that appear in the search criteria. See rfc2978
-        :param miss_no_uid: not add None values to result when uid item not matched to pattern
         :return: email message uids
         """
-        nums = self.numbers(criteria, charset)
-        if not nums:
-            return []
-        fetch_result = self.client.fetch(','.join(nums), "(UID)")
-        check_command_status(fetch_result, MailboxUidsError)
-        result = []
-        for fetch_item in fetch_result[1]:
-            # fetch_item: AnyStr  # todo uncomment after drop 3.5
-            uid_match = re.search(UID_PATTERN, decode_value(fetch_item))  # noqa
-            if uid_match:
-                result.append(uid_match.group('uid'))
-            elif not miss_no_uid:
-                result.append(None)
-        return result
-
-    def _fetch_by_one(self, message_nums: Sequence[str], message_parts: str, reverse: bool) -> Iterator[list]:  # noqa
-        for message_num in message_nums:
-            fetch_result = self.client.fetch(message_num, message_parts)
+        encoded_criteria = criteria if type(criteria) is bytes else str(criteria).encode(charset)
+        uid_result = self.client.uid('SEARCH', 'CHARSET', charset, encoded_criteria)
+        check_command_status(uid_result, MailboxUidsError)
+        return uid_result[1][0].decode().split() if uid_result[1][0] else []
+
+    def _fetch_by_one(self, uid_list: Sequence[str], message_parts: str, reverse: bool) -> Iterator[list]:  # noqa
+        for uid in uid_list:
+            fetch_result = self.client.uid('fetch', uid, message_parts)
             check_command_status(fetch_result, MailboxFetchError)
+            if not fetch_result[1] or fetch_result[1][0] is None:
+                continue
             yield fetch_result[1]
 
-    def _fetch_in_bulk(self, message_nums: Sequence[str], message_parts: str, reverse: bool) -> Iterator[list]:
-        if not message_nums:
+    def _fetch_in_bulk(self, uid_list: Sequence[str], message_parts: str, reverse: bool) -> Iterator[list]:
+        if not uid_list:
             return
-        fetch_result = self.client.fetch(','.join(message_nums), message_parts)
+        fetch_result = self.client.uid('fetch', ','.join(uid_list), message_parts)
         check_command_status(fetch_result, MailboxFetchError)
+        if not fetch_result[1] or fetch_result[1][0] is None:
+            return
         for built_fetch_item in chunks((reversed if reverse else iter)(fetch_result[1]), 2):
             yield built_fetch_item
 
     def fetch(self, criteria: Criteria = 'ALL', charset: str = 'US-ASCII', limit: Optional[Union[int, slice]] = None,
-              miss_no_uid=True, mark_seen=True, reverse=False, headers_only=False,
-              bulk=False) -> Iterator[MailMessage]:
+              mark_seen=True, reverse=False, headers_only=False, bulk=False) -> Iterator[MailMessage]:
         """
         Mail message generator in current folder by search criteria
         :param criteria: message search criteria (see examples at ./doc/imap_search_criteria.txt)
         :param charset: IANA charset, indicates charset of the strings that appear in the search criteria. See rfc2978
         :param limit: int | slice - limit number of read emails | slice emails range for read
                       useful for actions with a large number of messages, like "move" | paging
-        :param miss_no_uid: miss emails without uid
         :param mark_seen: mark emails as seen on fetch
         :param reverse: in order from the larger date to the smaller
         :param headers_only: get only email headers (without text, html, attachments)
         :param bulk: False - fetch each message separately per N commands - low memory consumption, slow
                      True  - fetch all messages per 1 command - high memory consumption, fast
         :return generator: MailMessage
         """
         message_parts = "(BODY{}[{}] UID FLAGS RFC822.SIZE)".format(
             '' if mark_seen else '.PEEK', 'HEADER' if headers_only else '')
         limit_range = slice(0, limit) if type(limit) is int else limit or slice(None)
         assert type(limit_range) is slice
-        nums = tuple((reversed if reverse else iter)(self.numbers(criteria, charset)))[limit_range]
-        for fetch_item in (self._fetch_in_bulk if bulk else self._fetch_by_one)(nums, message_parts, reverse):  # noqa
-            mail_message = self.email_message_class(fetch_item)
-            if miss_no_uid and not mail_message.uid:
-                continue
-            yield mail_message
+        uids = tuple((reversed if reverse else iter)(self.uids(criteria, charset)))[limit_range]
+        for fetch_item in (self._fetch_in_bulk if bulk else self._fetch_by_one)(uids, message_parts, reverse):  # noqa
+            yield self.email_message_class(fetch_item)
 
     def expunge(self) -> tuple:
         result = self.client.expunge()
         check_command_status(result, MailboxExpungeError)
         return result
 
     def delete(self, uid_list: Union[str, Iterable[str]]) -> Optional[Tuple[tuple, tuple]]:
```

### Comparing `imap-tools-1.0.0/imap_tools/message.py` & `imap-tools-1.1.0/imap_tools/message.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.0.0/imap_tools/query.py` & `imap-tools-1.1.0/imap_tools/query.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.0.0/imap_tools/utils.py` & `imap-tools-1.1.0/imap_tools/utils.py`

 * *Files identical despite different names*

### Comparing `imap-tools-1.0.0/imap_tools/__init__.py` & `imap-tools-1.1.0/imap_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 from .mailbox import BaseMailBox, MailBox, MailBoxUnencrypted, MailBoxTls
 from .message import MailMessage, MailAttachment
 from .folder import MailBoxFolderManager, FolderInfo
 from .consts import MailMessageFlags, MailBoxFolderStatusOptions
 from .utils import EmailAddress
 from .errors import *
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
```

### Comparing `imap-tools-1.0.0/imap_tools.egg-info/PKG-INFO` & `imap-tools-1.1.0/imap_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap-tools
-Version: 1.0.0
+Version: 1.1.0
 Summary: Work with email by IMAP
 Home-page: https://github.com/ikvk/imap_tools
 Author: Vladimir Kaukin
 Author-email: KaukinVK@ya.ru
 License: Apache-2.0
 Keywords: imap,imap-client,python3,python,email
 Platform: UNKNOWN
@@ -36,15 +36,15 @@
 .. image:: https://img.shields.io/pypi/dm/imap_tools.svg?style=social
 
 ===============  ================================================================================================
 Python version   3.5+
 License          Apache-2.0
 PyPI             https://pypi.python.org/pypi/imap_tools/
 RFC              `IMAP4.1 <https://tools.ietf.org/html/rfc3501>`_,
-                 `EMAIL <https://tools.ietf.org/html/rfc3501>`_,
+                 `EMAIL <https://tools.ietf.org/html/rfc2822>`_,
                  `IMAP related RFCs <https://github.com/ikvk/imap_tools/blob/master/docs/IMAP_related_RFCs.txt>`_
 ===============  ================================================================================================
 
 .. contents::
 
 Installation
 ------------
@@ -69,32 +69,30 @@
         for msg in mailbox.fetch():
             print(msg.date, msg.subject, len(msg.text or msg.html))
 
 `Description of this^ example <https://github.com/ikvk/imap_tools/blob/master/examples/basic.py>`_.
 
 MailBox, MailBoxTls, MailBoxUnencrypted - for create mailbox client. `TLS example <https://github.com/ikvk/imap_tools/blob/master/examples/tls.py>`_.
 
-BaseMailBox.login, BaseMailBox.login_utf8, MailBox.xoauth2, BaseMailBox.logout - authentication functions, they support context manager.
+BaseMailBox.<auth> - login, login_utf8, xoauth2, logout - authentication functions, they support context manager.
 
 BaseMailBox.fetch - first searches email nums by criteria in current folder, then fetch and yields `MailMessage <#email-attributes>`_:
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
 * *limit* = None, limit on the number of read emails, useful for actions with a large number of messages, like "move"
-* *miss_no_uid* = True, miss emails without uid
 * *mark_seen* = True, mark emails as seen on fetch
 * *reverse* = False, in order from the larger date to the smaller
 * *headers_only* = False, get only email headers (without text, html, attachments)
 * *bulk* = False, False - fetch each message separately per N commands - low memory consumption, slow; True - fetch all messages per 1 command - high memory consumption, fast
 
 BaseMailBox.uids - search mailbox for matching message uids in current folder, returns [str | None]
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
-* *miss_no_uid* = True, not add None values to result when uid item not matched to pattern
 
 BaseMailBox.<action> - `copy, move, delete, flag, append <#actions-with-emails>`_
 
 BaseMailBox.folder - `folder manager <#actions-with-folders>`_
 
 BaseMailBox.idle - `idle manager <#idle-workflow>`_
 
@@ -150,15 +148,15 @@
 
 .. code-block:: python
 
     from imap_tools import AND
 
     mailbox.fetch(AND(subject='weather'))  # query, the str-like object
     mailbox.fetch('TEXT "hello"')          # str
-    mailbox.fetch(b'TEXT "\xd1\x8f"')      # bytes, *charset arg is ignored
+    mailbox.fetch(b'TEXT "\xd1\x8f"')      # bytes
 
 Use "charset" argument for encode criteria to the desired encoding. If "criteria" is bytes - encoding will be ignored.
 
 .. code-block:: python
 
     mailbox.uids(A(subject='жёлтый'), charset='utf8')
 
@@ -220,26 +218,26 @@
 size_lt        int >= 0         SMALLER 512             rfc2822 size smaller than specified number of octets
 new            True             NEW                     have the Recent flag set but not the Seen flag
 old            True             OLD                     do not have the Recent flag set
 recent         True             RECENT                  have the Recent flag set
 all            True             ALL                     all, criteria by default
 uid            iter(str)/str/U  UID 1,2,17              corresponding to the specified unique identifier set
 header         H(str, str)*     HEADER "A-Spam" "5.8"   have a header that contains the specified str in the text
-gmail_label    str*             X-GM-LABELS "label1"    have this gmail label.
+gmail_label    str*             X-GM-LABELS "label1"    have this gmail label
 =============  ===============  ======================  ================================================================
 
 Server side search notes:
 
 * For string search keys a message matches if the string is a substring of the field. The matching is case-insensitive.
 * When searching by dates - email's time and timezone are disregarding.
 
 Actions with emails
 ^^^^^^^^^^^^^^^^^^^
 
-First of all read about uid `at rfc3501 <https://tools.ietf.org/html/rfc3501#section-2.3.1.1>`_.
+First of all read about UID `at rfc3501 <https://tools.ietf.org/html/rfc3501#section-2.3.1.1>`_.
 
 Action's uid_list arg may takes:
 
 * str, that is comma separated uids
 * Sequence, that contains str uids
 
 To get uids, use the maibox methods: uids, fetch.
@@ -419,14 +417,18 @@
 `UlisseMini <https://github.com/UlisseMini>`_,
 `Nicarex <https://github.com/Nicarex>`_,
 `RanjithNair1980 <https://github.com/RanjithNair1980>`_,
 `NickC-NZ <https://github.com/NickC-NZ>`_,
 `mweinelt <https://github.com/mweinelt>`_,
 `lucbouge <https://github.com/lucbouge>`_,
 `JacquelinCharbonnel <https://github.com/JacquelinCharbonnel>`_,
-`stumpylog <https://github.com/stumpylog>`_
+`stumpylog <https://github.com/stumpylog>`_,
+`dimitrisstr <https://github.com/dimitrisstr>`_
 
-Donate
-------
-`✋ I want to help this library <https://github.com/ikvk/imap_tools/blob/master/docs/donate.rst>`_
+Help the project
+----------------
+1. Found a bug or figure out how to improve the library - open issue or merge request 🎯
+2. Do not know how to improve library - try to help other open projects that you use ✋
+3. Nowhere to put your money - spend it on your family, friends, loved ones, or people around you 💰
+4. Star the project ⭐
```

### Comparing `imap-tools-1.0.0/LICENSE` & `imap-tools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imap-tools-1.0.0/PKG-INFO` & `imap-tools-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap-tools
-Version: 1.0.0
+Version: 1.1.0
 Summary: Work with email by IMAP
 Home-page: https://github.com/ikvk/imap_tools
 Author: Vladimir Kaukin
 Author-email: KaukinVK@ya.ru
 License: Apache-2.0
 Keywords: imap,imap-client,python3,python,email
 Platform: UNKNOWN
@@ -36,15 +36,15 @@
 .. image:: https://img.shields.io/pypi/dm/imap_tools.svg?style=social
 
 ===============  ================================================================================================
 Python version   3.5+
 License          Apache-2.0
 PyPI             https://pypi.python.org/pypi/imap_tools/
 RFC              `IMAP4.1 <https://tools.ietf.org/html/rfc3501>`_,
-                 `EMAIL <https://tools.ietf.org/html/rfc3501>`_,
+                 `EMAIL <https://tools.ietf.org/html/rfc2822>`_,
                  `IMAP related RFCs <https://github.com/ikvk/imap_tools/blob/master/docs/IMAP_related_RFCs.txt>`_
 ===============  ================================================================================================
 
 .. contents::
 
 Installation
 ------------
@@ -69,32 +69,30 @@
         for msg in mailbox.fetch():
             print(msg.date, msg.subject, len(msg.text or msg.html))
 
 `Description of this^ example <https://github.com/ikvk/imap_tools/blob/master/examples/basic.py>`_.
 
 MailBox, MailBoxTls, MailBoxUnencrypted - for create mailbox client. `TLS example <https://github.com/ikvk/imap_tools/blob/master/examples/tls.py>`_.
 
-BaseMailBox.login, BaseMailBox.login_utf8, MailBox.xoauth2, BaseMailBox.logout - authentication functions, they support context manager.
+BaseMailBox.<auth> - login, login_utf8, xoauth2, logout - authentication functions, they support context manager.
 
 BaseMailBox.fetch - first searches email nums by criteria in current folder, then fetch and yields `MailMessage <#email-attributes>`_:
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
 * *limit* = None, limit on the number of read emails, useful for actions with a large number of messages, like "move"
-* *miss_no_uid* = True, miss emails without uid
 * *mark_seen* = True, mark emails as seen on fetch
 * *reverse* = False, in order from the larger date to the smaller
 * *headers_only* = False, get only email headers (without text, html, attachments)
 * *bulk* = False, False - fetch each message separately per N commands - low memory consumption, slow; True - fetch all messages per 1 command - high memory consumption, fast
 
 BaseMailBox.uids - search mailbox for matching message uids in current folder, returns [str | None]
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
-* *miss_no_uid* = True, not add None values to result when uid item not matched to pattern
 
 BaseMailBox.<action> - `copy, move, delete, flag, append <#actions-with-emails>`_
 
 BaseMailBox.folder - `folder manager <#actions-with-folders>`_
 
 BaseMailBox.idle - `idle manager <#idle-workflow>`_
 
@@ -150,15 +148,15 @@
 
 .. code-block:: python
 
     from imap_tools import AND
 
     mailbox.fetch(AND(subject='weather'))  # query, the str-like object
     mailbox.fetch('TEXT "hello"')          # str
-    mailbox.fetch(b'TEXT "\xd1\x8f"')      # bytes, *charset arg is ignored
+    mailbox.fetch(b'TEXT "\xd1\x8f"')      # bytes
 
 Use "charset" argument for encode criteria to the desired encoding. If "criteria" is bytes - encoding will be ignored.
 
 .. code-block:: python
 
     mailbox.uids(A(subject='жёлтый'), charset='utf8')
 
@@ -220,26 +218,26 @@
 size_lt        int >= 0         SMALLER 512             rfc2822 size smaller than specified number of octets
 new            True             NEW                     have the Recent flag set but not the Seen flag
 old            True             OLD                     do not have the Recent flag set
 recent         True             RECENT                  have the Recent flag set
 all            True             ALL                     all, criteria by default
 uid            iter(str)/str/U  UID 1,2,17              corresponding to the specified unique identifier set
 header         H(str, str)*     HEADER "A-Spam" "5.8"   have a header that contains the specified str in the text
-gmail_label    str*             X-GM-LABELS "label1"    have this gmail label.
+gmail_label    str*             X-GM-LABELS "label1"    have this gmail label
 =============  ===============  ======================  ================================================================
 
 Server side search notes:
 
 * For string search keys a message matches if the string is a substring of the field. The matching is case-insensitive.
 * When searching by dates - email's time and timezone are disregarding.
 
 Actions with emails
 ^^^^^^^^^^^^^^^^^^^
 
-First of all read about uid `at rfc3501 <https://tools.ietf.org/html/rfc3501#section-2.3.1.1>`_.
+First of all read about UID `at rfc3501 <https://tools.ietf.org/html/rfc3501#section-2.3.1.1>`_.
 
 Action's uid_list arg may takes:
 
 * str, that is comma separated uids
 * Sequence, that contains str uids
 
 To get uids, use the maibox methods: uids, fetch.
@@ -419,14 +417,18 @@
 `UlisseMini <https://github.com/UlisseMini>`_,
 `Nicarex <https://github.com/Nicarex>`_,
 `RanjithNair1980 <https://github.com/RanjithNair1980>`_,
 `NickC-NZ <https://github.com/NickC-NZ>`_,
 `mweinelt <https://github.com/mweinelt>`_,
 `lucbouge <https://github.com/lucbouge>`_,
 `JacquelinCharbonnel <https://github.com/JacquelinCharbonnel>`_,
-`stumpylog <https://github.com/stumpylog>`_
+`stumpylog <https://github.com/stumpylog>`_,
+`dimitrisstr <https://github.com/dimitrisstr>`_
 
-Donate
-------
-`✋ I want to help this library <https://github.com/ikvk/imap_tools/blob/master/docs/donate.rst>`_
+Help the project
+----------------
+1. Found a bug or figure out how to improve the library - open issue or merge request 🎯
+2. Do not know how to improve library - try to help other open projects that you use ✋
+3. Nowhere to put your money - spend it on your family, friends, loved ones, or people around you 💰
+4. Star the project ⭐
```

### Comparing `imap-tools-1.0.0/README.rst` & `imap-tools-1.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 .. image:: https://img.shields.io/pypi/dm/imap_tools.svg?style=social
 
 ===============  ================================================================================================
 Python version   3.5+
 License          Apache-2.0
 PyPI             https://pypi.python.org/pypi/imap_tools/
 RFC              `IMAP4.1 <https://tools.ietf.org/html/rfc3501>`_,
-                 `EMAIL <https://tools.ietf.org/html/rfc3501>`_,
+                 `EMAIL <https://tools.ietf.org/html/rfc2822>`_,
                  `IMAP related RFCs <https://github.com/ikvk/imap_tools/blob/master/docs/IMAP_related_RFCs.txt>`_
 ===============  ================================================================================================
 
 .. contents::
 
 Installation
 ------------
@@ -53,32 +53,30 @@
         for msg in mailbox.fetch():
             print(msg.date, msg.subject, len(msg.text or msg.html))
 
 `Description of this^ example <https://github.com/ikvk/imap_tools/blob/master/examples/basic.py>`_.
 
 MailBox, MailBoxTls, MailBoxUnencrypted - for create mailbox client. `TLS example <https://github.com/ikvk/imap_tools/blob/master/examples/tls.py>`_.
 
-BaseMailBox.login, BaseMailBox.login_utf8, MailBox.xoauth2, BaseMailBox.logout - authentication functions, they support context manager.
+BaseMailBox.<auth> - login, login_utf8, xoauth2, logout - authentication functions, they support context manager.
 
 BaseMailBox.fetch - first searches email nums by criteria in current folder, then fetch and yields `MailMessage <#email-attributes>`_:
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
 * *limit* = None, limit on the number of read emails, useful for actions with a large number of messages, like "move"
-* *miss_no_uid* = True, miss emails without uid
 * *mark_seen* = True, mark emails as seen on fetch
 * *reverse* = False, in order from the larger date to the smaller
 * *headers_only* = False, get only email headers (without text, html, attachments)
 * *bulk* = False, False - fetch each message separately per N commands - low memory consumption, slow; True - fetch all messages per 1 command - high memory consumption, fast
 
 BaseMailBox.uids - search mailbox for matching message uids in current folder, returns [str | None]
 
 * *criteria* = 'ALL', message search criteria, `query builder <#search-criteria>`_
 * *charset* = 'US-ASCII', indicates charset of the strings that appear in the search criteria. See rfc2978
-* *miss_no_uid* = True, not add None values to result when uid item not matched to pattern
 
 BaseMailBox.<action> - `copy, move, delete, flag, append <#actions-with-emails>`_
 
 BaseMailBox.folder - `folder manager <#actions-with-folders>`_
 
 BaseMailBox.idle - `idle manager <#idle-workflow>`_
 
@@ -134,15 +132,15 @@
 
 .. code-block:: python
 
     from imap_tools import AND
 
     mailbox.fetch(AND(subject='weather'))  # query, the str-like object
     mailbox.fetch('TEXT "hello"')          # str
-    mailbox.fetch(b'TEXT "\xd1\x8f"')      # bytes, *charset arg is ignored
+    mailbox.fetch(b'TEXT "\xd1\x8f"')      # bytes
 
 Use "charset" argument for encode criteria to the desired encoding. If "criteria" is bytes - encoding will be ignored.
 
 .. code-block:: python
 
     mailbox.uids(A(subject='жёлтый'), charset='utf8')
 
@@ -204,26 +202,26 @@
 size_lt        int >= 0         SMALLER 512             rfc2822 size smaller than specified number of octets
 new            True             NEW                     have the Recent flag set but not the Seen flag
 old            True             OLD                     do not have the Recent flag set
 recent         True             RECENT                  have the Recent flag set
 all            True             ALL                     all, criteria by default
 uid            iter(str)/str/U  UID 1,2,17              corresponding to the specified unique identifier set
 header         H(str, str)*     HEADER "A-Spam" "5.8"   have a header that contains the specified str in the text
-gmail_label    str*             X-GM-LABELS "label1"    have this gmail label.
+gmail_label    str*             X-GM-LABELS "label1"    have this gmail label
 =============  ===============  ======================  ================================================================
 
 Server side search notes:
 
 * For string search keys a message matches if the string is a substring of the field. The matching is case-insensitive.
 * When searching by dates - email's time and timezone are disregarding.
 
 Actions with emails
 ^^^^^^^^^^^^^^^^^^^
 
-First of all read about uid `at rfc3501 <https://tools.ietf.org/html/rfc3501#section-2.3.1.1>`_.
+First of all read about UID `at rfc3501 <https://tools.ietf.org/html/rfc3501#section-2.3.1.1>`_.
 
 Action's uid_list arg may takes:
 
 * str, that is comma separated uids
 * Sequence, that contains str uids
 
 To get uids, use the maibox methods: uids, fetch.
@@ -403,12 +401,16 @@
 `UlisseMini <https://github.com/UlisseMini>`_,
 `Nicarex <https://github.com/Nicarex>`_,
 `RanjithNair1980 <https://github.com/RanjithNair1980>`_,
 `NickC-NZ <https://github.com/NickC-NZ>`_,
 `mweinelt <https://github.com/mweinelt>`_,
 `lucbouge <https://github.com/lucbouge>`_,
 `JacquelinCharbonnel <https://github.com/JacquelinCharbonnel>`_,
-`stumpylog <https://github.com/stumpylog>`_
+`stumpylog <https://github.com/stumpylog>`_,
+`dimitrisstr <https://github.com/dimitrisstr>`_
 
-Donate
-------
-`✋ I want to help this library <https://github.com/ikvk/imap_tools/blob/master/docs/donate.rst>`_
+Help the project
+----------------
+1. Found a bug or figure out how to improve the library - open issue or merge request 🎯
+2. Do not know how to improve library - try to help other open projects that you use ✋
+3. Nowhere to put your money - spend it on your family, friends, loved ones, or people around you 💰
+4. Star the project ⭐
```

### Comparing `imap-tools-1.0.0/setup.py` & `imap-tools-1.1.0/setup.py`

 * *Files identical despite different names*

