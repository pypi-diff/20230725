# Comparing `tmp/quota_notifier-0.5.8.tar.gz` & `tmp/quota_notifier-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quota_notifier-0.5.8.tar", max compression
+gzip compressed data, was "quota_notifier-0.5.9.tar", max compression
```

## Comparing `quota_notifier-0.5.8.tar` & `quota_notifier-0.5.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34906 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/LICENSE.md
--rw-r--r--   0        0        0      653 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/README.md
--rw-r--r--   0        0        0     1415 2023-06-13 13:11:12.004049 quota_notifier-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     1506 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/__init__.py
--rw-r--r--   0        0        0      202 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/__main__.py
--rw-r--r--   0        0        0     6662 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/cli.py
--rw-r--r--   0        0        0      298 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/data/template.html
--rw-r--r--   0        0        0    10990 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/disk_utils.py
--rw-r--r--   0        0        0    11137 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/notify.py
--rw-r--r--   0        0        0     3220 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/orm.py
--rw-r--r--   0        0        0     9157 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/settings.py
--rw-r--r--   0        0        0     2874 2023-06-13 13:10:52.748133 quota_notifier-0.5.8/quota_notifier/shell.py
--rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 quota_notifier-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    34906 2023-06-14 16:04:50.602401 quota_notifier-0.5.9/LICENSE.md
+-rw-r--r--   0        0        0      695 2023-06-14 16:04:50.602401 quota_notifier-0.5.9/README.md
+-rw-r--r--   0        0        0     1386 2023-06-14 16:05:18.354752 quota_notifier-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     1506 2023-06-14 16:04:50.602401 quota_notifier-0.5.9/quota_notifier/__init__.py
+-rw-r--r--   0        0        0      202 2023-06-14 16:04:50.602401 quota_notifier-0.5.9/quota_notifier/__main__.py
+-rw-r--r--   0        0        0     8210 2023-06-14 16:04:50.602401 quota_notifier-0.5.9/quota_notifier/cli.py
+-rw-r--r--   0        0        0      298 2023-06-14 16:04:50.602401 quota_notifier-0.5.9/quota_notifier/data/template.html
+-rw-r--r--   0        0        0    10990 2023-06-14 16:04:50.602401 quota_notifier-0.5.9/quota_notifier/disk_utils.py
+-rw-r--r--   0        0        0    10716 2023-06-14 16:04:50.602401 quota_notifier-0.5.9/quota_notifier/notify.py
+-rw-r--r--   0        0        0     3220 2023-06-14 16:04:50.602401 quota_notifier-0.5.9/quota_notifier/orm.py
+-rw-r--r--   0        0        0     8824 2023-06-14 16:04:50.602401 quota_notifier-0.5.9/quota_notifier/settings.py
+-rw-r--r--   0        0        0     2874 2023-06-14 16:04:50.602401 quota_notifier-0.5.9/quota_notifier/shell.py
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 quota_notifier-0.5.9/PKG-INFO
```

### Comparing `quota_notifier-0.5.8/LICENSE.md` & `quota_notifier-0.5.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.8/README.md` & `quota_notifier-0.5.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Storage Quota Notifier
 
 [![](https://app.codacy.com/project/badge/Grade/583c607400c2429ebbc1554d777d26b4)](https://app.codacy.com/gh/pitt-crc/quota_notifier/dashboard)
 [![](https://app.codacy.com/project/badge/Coverage/583c607400c2429ebbc1554d777d26b4)](https://app.codacy.com/gh/pitt-crc/quota_notifier/dashboard)
 [![](https://github.com/pitt-crc/quota_notifier/actions/workflows/PackageTest.yml/badge.svg)](https://github.com/pitt-crc/quota_notifier/actions/workflows/PackageTest.yml)
 
-A command line utility for emailing users when they exceed storage quota thresholds
+A command line utility for emailing users when they exceed storage quota thresholds on mounted file systems.
 
-See the [official documentation](https://crc-pages.pitt.edu/quota_notifier/).
+See the [official documentation](https://crc-pages.pitt.edu/quota_notifier/) for more details.
```

### Comparing `quota_notifier-0.5.8/pyproject.toml` & `quota_notifier-0.5.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "quota-notifier"
-version = "0.5.8"  # Version is set dynamically by the CI tool on publication
+version = "0.5.9"  # Version is set dynamically by the CI tool on publication
 authors = ["Pitt Center for Research Computing", ]
 readme = "README.md"
 description = "Automatic email notification tool for disk quota usage."
 homepage = "https://github.com/pitt-crc/quota_notifier"
 repository = "https://github.com/pitt-crc/quota_notifier"
 documentation = "https://crc-pages.pitt.edu/quota_notifier/"
 keywords = ["disk", "usage", "quota", "notify", "email", ]
@@ -26,15 +26,14 @@
 [tool.poetry.scripts]
 notifier = "quota_notifier.cli:Application.execute"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 pydantic = "1.10.9"
 sqlalchemy = "2.0.15"
-prometheus_client = "0.17.0"
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
 coverage = "*"
```

### Comparing `quota_notifier-0.5.8/quota_notifier/__init__.py` & `quota_notifier-0.5.9/quota_notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.8/quota_notifier/cli.py` & `quota_notifier-0.5.9/quota_notifier/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ---------------
 """
 
 import logging
 import logging.config
 from argparse import ArgumentParser
 from pathlib import Path
+from smtplib import SMTP
 from typing import List
 
 from . import __version__
 from .notify import UserNotifier
 from .orm import DBConnection
 from .settings import ApplicationSettings
 
@@ -104,82 +105,116 @@
                     'level': console_log_level
                 },
                 'log_file_handler': {
                     'class': 'logging.FileHandler',
                     'formatter': 'log_file_formatter',
                     'level': ApplicationSettings.get('log_level'),
                     'filename': ApplicationSettings.get('log_path')
+                },
+                'smtp_handler': {
+                    'class': 'logging.handlers.SMTPHandler',
+                    'formatter': 'log_file_formatter',
+                    'level': 'CRITICAL',
+                    'mailhost': ApplicationSettings.get('smtp_host'),
+                    'fromaddr': ApplicationSettings.get('email_from'),
+                    'toaddrs': ApplicationSettings.get('email_admins'),
+                    'subject': 'Quota Notifier - Admin Notification'
                 }
             },
             'loggers': {
                 'console_logger': {'handlers': ['console_handler'], 'level': 0, 'propagate': False},
                 'file_logger': {'handlers': ['log_file_handler'], 'level': 0, 'propagate': False},
+                'smtp_logger': {'handlers': ['smtp_handler'], 'level': 0, 'propagate': False},
                 '': {'handlers': ['console_handler', 'log_file_handler'], 'level': 0, 'propagate': False},
             }
         })
 
     @classmethod
     def _configure_database(cls) -> None:
         """Configure the application database connection"""
 
+        logging.debug('Configuring database connection...')
         if ApplicationSettings.get('debug'):
             DBConnection.configure('sqlite:///:memory:')
 
         else:
             DBConnection.configure(ApplicationSettings.get('db_url'))
 
     @classmethod
+    def _test_smtp_server(cls) -> None:
+        """Ensure the SMTP server can be reached"""
+
+        logging.debug('Testing SMTP server...')
+        host = ApplicationSettings.get('smtp_host')
+        port = ApplicationSettings.get('smtp_port')
+        server = SMTP(host=host, port=port)
+
+        try:
+            server.connect()
+
+        except Exception as caught:
+            raise ConnectionError(
+                f'Could not connect to SMTP server at {host}:{port}. Please check your application settings file.'
+            ) from caught
+
+    @classmethod
     def run(cls, validate: bool = False, verbosity: int = 0, debug: bool = False) -> None:
         """Run the application using parsed commandline arguments
 
         Args:
             validate: Validate application settings without issuing user notifications
             verbosity: Console output verbosity
             debug: Run the application in debug mode
         """
 
         # Configure application settings
         cls._load_settings(force_debug=debug)
         if validate:
             return
 
-        # Map number of verbosity flags to logging levels
-        log_levels = {
-            0: logging.ERROR,
-            1: logging.WARNING,
-            2: logging.INFO,
-            3: logging.DEBUG}
-
         # Configure application logging (to console and file)
-        cls._configure_logging(console_log_level=log_levels.get(verbosity, logging.DEBUG))
+        verbosity_to_log_level = {0: logging.ERROR, 1: logging.WARNING, 2: logging.INFO, 3: logging.DEBUG}
+        cls._configure_logging(console_log_level=verbosity_to_log_level.get(verbosity, logging.DEBUG))
+
+        # Test the SMTP server can be reached
         if ApplicationSettings.get('debug'):
             logging.warning('Running application in debug mode')
 
-        # Connect to the database and run the core application logic
+        else:
+            cls._test_smtp_server()
+
+        # Connect to the application database
         cls._configure_database()
+
+        # Run the core application logic
         UserNotifier().send_notifications()
 
     @classmethod
     def execute(cls, arg_list: List[str] = None) -> None:
         """Parse arguments and execute the application
 
-        Raised exceptions are passed to STDERR via the argument parser.
+        This method is equivalent to parsing arguments and passing them to the `run` method.
 
         Args:
-            arg_list: Run the application with the given arguments instead of parsing the command line
+            arg_list: Parse the given argument list instead of parsing the command line
         """
 
         parser = Parser()
         args = parser.parse_args(arg_list)
 
         try:
             cls.run(
                 validate=args.validate,
                 verbosity=args.verbose,
                 debug=args.debug)
 
+        except ConnectionError as caught:
+            logging.getLogger('console_logger').critical(f'Error connecting to SMTP server - {caught}')
+
         except Exception as caught:
             logging.getLogger('file_logger').critical('Application crash', exc_info=caught)
             logging.getLogger('console_logger').critical(str(caught))
+            if ApplicationSettings.get('admin_emails'):
+                logging.getLogger('smtp_logger').critical(str(caught))
 
         else:
             logging.info('Exiting application gracefully')
```

### Comparing `quota_notifier-0.5.8/quota_notifier/disk_utils.py` & `quota_notifier-0.5.9/quota_notifier/disk_utils.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.8/quota_notifier/notify.py` & `quota_notifier-0.5.9/quota_notifier/notify.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 import logging
 from bisect import bisect_right
 from email.message import EmailMessage
 from pathlib import Path
 from smtplib import SMTP
 from typing import Collection, Optional, Set, Union, Tuple, List
+from typing import Iterable
 
-from prometheus_client import Summary, CollectorRegistry, push_to_gateway
 from sqlalchemy import delete, insert, select
 from sqlalchemy.orm import Session
 
 from .disk_utils import AbstractQuota, BeeGFSQuota, QuotaFactory
 from .orm import DBConnection, Notification
 from .settings import ApplicationSettings
 from .shell import User
@@ -77,27 +77,27 @@
         email["To"] = address
 
         logging.debug(f'Sending email notification to {address}')
         if ApplicationSettings.get('debug'):
             return email
 
         with smtp or SMTP(
-            host=ApplicationSettings.get('smtp_host'),
-            port=ApplicationSettings.get('smtp_port')
+                host=ApplicationSettings.get('smtp_host'),
+                port=ApplicationSettings.get('smtp_port')
         ) as smtp_server:
             smtp_server.send_message(email)
 
         return email
 
 
 class UserNotifier:
     """Issue and manage user quota notifications"""
 
     @classmethod
-    def get_users(cls) -> List[User]:
+    def get_users(cls) -> Iterable[User]:
         """Return a collection of users to check quotas for
 
         Returns:
             An iterable collection of ``User`` objects
         """
 
         logging.info('Fetching user list...')
@@ -280,32 +280,22 @@
                 cachable_systems_found = True
                 BeeGFSQuota.cache_quotas(name=file_system.name, path=file_system.path, users=users)
 
         if not cachable_systems_found:
             logging.debug('No cachable system queries found')
 
         logging.info('Scanning user quotas...')
-        failures = 0
+        failure = False
         for user in users:
             try:
                 self.notify_user(user)
 
             except Exception as caught:
-                failures += 1
+                # Only include exception information in the logfile, not the console
                 logging.getLogger('file_logger').error(f'Error notifying {user}', exc_info=caught)
                 logging.getLogger('console_logger').error(f'Error notifying {user} - {caught}')
+                failure = True
 
-        # Check if prometheus reporting is enabled
-        prom_host = ApplicationSettings.get('prometheus_host')
-        if not prom_host:
-            return
-
-        registry = CollectorRegistry()
-        failed_summary = Summary('failed_users', 'Number of users with failed notifications', registry=registry)
-        failed_summary.observe(failures)
-
-        processed_summary = Summary('processed_users', 'Number of users scanned for notification', registry=registry)
-        processed_summary.observe(len(users))
-
-        prom_port = ApplicationSettings.get('prometheus_port')
-        prom_job = ApplicationSettings.get('prometheus_job')
-        push_to_gateway(f'{prom_host}:{prom_port}', job=prom_job, registry=registry)
+        if failure and ApplicationSettings.get('admin_emails'):
+            logging.getLogger('smtp_logger').critical(
+                'Email notifications failed for one or more user accounts. See the application logs for more details.'
+            )
```

### Comparing `quota_notifier-0.5.8/quota_notifier/orm.py` & `quota_notifier-0.5.9/quota_notifier/orm.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.8/quota_notifier/settings.py` & `quota_notifier-0.5.9/quota_notifier/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,33 +135,14 @@
         description='Application logging level.')
 
     log_path: Optional[Path] = Field(
         title='Log Path',
         default_factory=lambda: Path(NamedTemporaryFile().name),
         description='Optionally log application events to a file.')
 
-    # Prometheus settings
-    prometheus_host: str = Field(
-        title='Prometheus Server Host Name',
-        default='',
-        description='Optional report metrics to a Prometheus server.'
-    )
-
-    prometheus_port: int = Field(
-        title='Prometheus Server Port Number',
-        default=9091,
-        description='Port for the Prometheus server'
-    )
-
-    prometheus_job: str = Field(
-        title='Prometheus Job Name',
-        default='notifier',
-        description='Job label attached to pushed metrics '
-    )
-
     # Settings for the smtp host/port
     smtp_host: str = Field(
         title='SMTP Server Host Name',
         default='',
         description='Name of the SMTP host server'
     )
 
@@ -191,14 +172,20 @@
 
     email_domain: str = Field(
         title='User Email Address Domain',
         default='@domain.com',
         description=('String to append to usernames when generating user email addresses. '
                      'The leading `@` is optional.'))
 
+    email_admins: List[str] = Field(
+        title='Administrator Emails',
+        default=[],
+        description='Admin users to contact when the application encounters a critical issue.'
+    )
+
     # Settings for debug / dry-runs
     debug: bool = Field(
         title='Debug Mode',
         default=False,
         description='Disable database commits and email notifications. Useful for development and testing.')
 
     @validator('file_systems')
```

### Comparing `quota_notifier-0.5.8/quota_notifier/shell.py` & `quota_notifier-0.5.9/quota_notifier/shell.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.8/PKG-INFO` & `quota_notifier-0.5.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quota-notifier
-Version: 0.5.8
+Version: 0.5.9
 Summary: Automatic email notification tool for disk quota usage.
 Home-page: https://github.com/pitt-crc/quota_notifier
 Keywords: disk,usage,quota,notify,email
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -14,24 +14,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: System :: Monitoring
 Classifier: Typing :: Typed
-Requires-Dist: prometheus_client (==0.17.0)
 Requires-Dist: pydantic (==1.10.9)
 Requires-Dist: sqlalchemy (==2.0.15)
 Project-URL: Documentation, https://crc-pages.pitt.edu/quota_notifier/
 Project-URL: Repository, https://github.com/pitt-crc/quota_notifier
 Description-Content-Type: text/markdown
 
 # Storage Quota Notifier
 
 [![](https://app.codacy.com/project/badge/Grade/583c607400c2429ebbc1554d777d26b4)](https://app.codacy.com/gh/pitt-crc/quota_notifier/dashboard)
 [![](https://app.codacy.com/project/badge/Coverage/583c607400c2429ebbc1554d777d26b4)](https://app.codacy.com/gh/pitt-crc/quota_notifier/dashboard)
 [![](https://github.com/pitt-crc/quota_notifier/actions/workflows/PackageTest.yml/badge.svg)](https://github.com/pitt-crc/quota_notifier/actions/workflows/PackageTest.yml)
 
-A command line utility for emailing users when they exceed storage quota thresholds
+A command line utility for emailing users when they exceed storage quota thresholds on mounted file systems.
 
-See the [official documentation](https://crc-pages.pitt.edu/quota_notifier/).
+See the [official documentation](https://crc-pages.pitt.edu/quota_notifier/) for more details.
```

