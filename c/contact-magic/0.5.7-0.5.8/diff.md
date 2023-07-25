# Comparing `tmp/contact_magic-0.5.7.tar.gz` & `tmp/contact_magic-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.5.7.tar", max compression
+gzip compressed data, was "contact_magic-0.5.8.tar", max compression
```

## Comparing `contact_magic-0.5.7.tar` & `contact_magic-0.5.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.7/README.md
--rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.7/contact_magic/__init__.py
--rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.7/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.7/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5418 2023-07-20 15:24:39.359080 contact_magic-0.5.7/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     2663 2023-07-20 16:08:38.910133 contact_magic-0.5.7/contact_magic/dict_utils.py
--rw-r--r--   0        0        0     3716 2023-07-20 14:30:01.195479 contact_magic-0.5.7/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.7/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2579 2023-07-24 08:11:52.431177 contact_magic-0.5.7/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1786 2023-07-24 08:11:09.776013 contact_magic-0.5.7/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1698 2023-07-09 10:24:31.018382 contact_magic-0.5.7/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.7/contact_magic/logger.py
--rw-r--r--   0        0        0    16920 2023-07-20 15:55:40.352110 contact_magic-0.5.7/contact_magic/models.py
--rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.7/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.7/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.5.7/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0     4512 2023-07-09 10:38:25.519902 contact_magic-0.5.7/contact_magic/scripts/default_scraper_options.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.7/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.5.7/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2517 2023-07-09 10:38:25.532220 contact_magic-0.5.7/contact_magic/scripts/sync_scraper_options_to_workersheets.py
--rw-r--r--   0        0        0     2166 2023-07-08 12:50:09.842574 contact_magic-0.5.7/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.7/contact_magic/utils.py
--rw-r--r--   0        0        0     1925 2023-07-24 08:11:37.573552 contact_magic-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.5.8/README.md
+-rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.5.8/contact_magic/__init__.py
+-rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.5.8/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.5.8/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5729 2023-07-25 11:21:41.873646 contact_magic-0.5.8/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     2663 2023-07-20 16:08:38.910133 contact_magic-0.5.8/contact_magic/dict_utils.py
+-rw-r--r--   0        0        0     3716 2023-07-20 14:30:01.195479 contact_magic-0.5.8/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.5.8/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2579 2023-07-24 08:11:52.431177 contact_magic-0.5.8/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1786 2023-07-24 08:11:09.776013 contact_magic-0.5.8/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1841 2023-07-25 12:42:54.024616 contact_magic-0.5.8/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.5.8/contact_magic/logger.py
+-rw-r--r--   0        0        0    16920 2023-07-20 15:55:40.352110 contact_magic-0.5.8/contact_magic/models.py
+-rw-r--r--   0        0        0     3079 2023-06-14 20:15:12.624966 contact_magic-0.5.8/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.5.8/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.5.8/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0     4512 2023-07-09 10:38:25.519902 contact_magic-0.5.8/contact_magic/scripts/default_scraper_options.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.5.8/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     5838 2023-07-25 12:44:12.632190 contact_magic-0.5.8/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2517 2023-07-09 10:38:25.532220 contact_magic-0.5.8/contact_magic/scripts/sync_scraper_options_to_workersheets.py
+-rw-r--r--   0        0        0     2166 2023-07-08 12:50:09.842574 contact_magic-0.5.8/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     1517 2023-06-14 19:19:52.625076 contact_magic-0.5.8/contact_magic/utils.py
+-rw-r--r--   0        0        0     1925 2023-07-25 12:46:00.148073 contact_magic-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.5.8/PKG-INFO
```

### Comparing `contact_magic-0.5.7/README.md` & `contact_magic-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/asyncio.py` & `contact_magic-0.5.8/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/conf/settings.py` & `contact_magic-0.5.8/contact_magic/conf/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Config file that reads from .env file and parses based on type set.
 
 https://docs.pydantic.dev/usage/settings/
 """
 from urllib.parse import urlparse
 
 import pytz
+import requests
 from pydantic import AnyUrl, BaseSettings, Field, validate_model, validator
 
 
 class BaseConfig(BaseSettings):
     """
     Settings for project.
     """
@@ -66,14 +67,17 @@
         default={},
     )
     ENABLE_SCRAPER_REUSE: bool = Field(
         description="This setting determines whether a contact can "
         "have multiple personalized sentences from the same scraper.",
         default=False,
     )
+    WEBHOOK_URL: AnyUrl = Field(
+        description="A webhook endpoint to be notified of events.", default=None
+    )
 
     @validator("TIMEZONE")
     def validate_timezone(cls, value):
         timezones = pytz.all_timezones_set
         if value not in timezones:
             value = "America/New_York"
         return value
@@ -138,14 +142,18 @@
         }.items():
             self.__setattr__(k, v)
         *_, validation_error = validate_model(self.__class__, self.__dict__)
         if validation_error:
             raise validation_error
         return self
 
+    def notify_webhook(self, event_name: str, data: dict):
+        if self.WEBHOOK_URL:
+            requests.post(self.WEBHOOK_URL, json={"event": event_name, "data": data})
+
     class Config:
         validate_assignment = True
         env_file = ".env"
         env_file_encoding = "utf-8"
 
 
 SETTINGS = BaseConfig()
```

### Comparing `contact_magic-0.5.7/contact_magic/dict_utils.py` & `contact_magic-0.5.8/contact_magic/dict_utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/helpers.py` & `contact_magic-0.5.8/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/integrations/copyfactory.py` & `contact_magic-0.5.8/contact_magic/integrations/copyfactory.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.5.8/contact_magic/integrations/sales_scrapers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/integrations/sheets.py` & `contact_magic-0.5.8/contact_magic/integrations/sheets.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     for _ in range(20):
         sleepy_time *= 2
         try:
             return func(*args)
         except APIError as e:
             res = e.response.json()["error"]
             if "status" in res and res.get("code", None) == 429:
-                sleep(15)
+                sleep(min([sleepy_time, 60]))
                 continue
             raise
         except Exception as e:
             print(f"Error in Gsheet with error '{e}'")
 
 
 def get_spreadsheet_by_url(url) -> gspread.models.Spreadsheet:
@@ -54,7 +54,11 @@
 
 def update_cell(sheet, row, col, value):
     return retry_req(sheet.update_cell, row, col, value)
 
 
 def clear_sheet(sheet):
     return retry_req(sheet.clear)
+
+
+def format_range(sheet, cell_range: str, format_data: dict):
+    return retry_req(sheet.format, cell_range, format_data)
```

### Comparing `contact_magic-0.5.7/contact_magic/models.py` & `contact_magic-0.5.8/contact_magic/models.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/preprocessors.py` & `contact_magic-0.5.8/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/scripts/agency.py` & `contact_magic-0.5.8/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/scripts/default_scraper_options.py` & `contact_magic-0.5.8/contact_magic/scripts/default_scraper_options.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/scripts/run_workflows.py` & `contact_magic-0.5.8/contact_magic/scripts/run_workflows.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from contact_magic.helpers import (
     get_personalization_settings_from_sheet,
     prepare_data_for_gsheet,
     worksheet_to_dataframe,
 )
 from contact_magic.integrations.sheets import (
     bulk_update,
+    format_range,
     get_spreadsheet_by_url,
     get_worksheet_from_spreadsheet,
     update_cell,
 )
 from contact_magic.scripts.logger import logger
 from contact_magic.utils import is_google_workflow_url_valid
 
@@ -56,71 +57,126 @@
     if row["is_approved"] == "TRUE":
         return True
     if pd.isnull(row["Website"]):
         return True
     return False
 
 
-def run_sheets():
+def uncheck_rows_and_format(sheet, df: pd.DataFrame, col_number=4):
+    for i, row in df.iterrows():
+        row_num = i + 2
+        update_cell(sheet, row_num, col_number, False)
+        format_range(
+            sheet,
+            f"{row_num}:{row_num}",
+            {
+                "backgroundColor": {"red": 1.0, "green": 1.0, "blue": 0.3},
+            },
+        )
+
+
+def mark_row_as_completed(sheet, row_number):
+    row_num = row_number + 2
+    format_range(
+        sheet,
+        f"{row_num}:{row_num}",
+        {
+            "backgroundColor": {"red": 0.0, "green": 1.0, "blue": 0.0},
+        },
+    )
+
+
+def run_sheets(return_as_arguments=False):
     workflows_sheet = get_worksheet_from_spreadsheet(
         get_spreadsheet_by_url(SETTINGS.MASTERSHEET_URL), "Workflows"
     )
-    for i, row in get_workflows_to_run(workflows_sheet).iterrows():
+    workflows_to_run = get_workflows_to_run(workflows_sheet)
+    uncheck_rows_and_format(workflows_sheet, workflows_to_run)
+
+    tasks = []
+    for i, row in workflows_to_run.iterrows():
         if not is_google_workflow_url_valid(row["WorkflowUrl"]):
             continue
         workflow_sheet = get_spreadsheet_by_url(row["WorkflowUrl"])
         filtered_working_data = worksheet_to_dataframe(workflow_sheet)
         # Don't filter working data since need to maintain
         # index so do spoof check to know if any rows to process.
         if (
             filtered_working_data.loc[filtered_working_data["is_approved"] == "FALSE"]
             .dropna(subset=["Website"])
             .empty
         ):
             continue
-        logger.info(
-            "running_workflow",
-            row_number=i + 2,
-            dataset_size=len(filtered_working_data),
-            sequence_name=row["WorkflowName"],
-            client_name=row["ClientName"],
-            status="STARTING",
-        )
-        if all(
-            col in filtered_working_data.columns for col in ["Company Name", "City"]
-        ):
-            filtered_working_data["search_query"] = filtered_working_data[
-                "Company Name"
-            ].str.cat(filtered_working_data["City"], sep=" ")
-        if all(
-            col in filtered_working_data.columns for col in ["City", "State", "Country"]
-        ):
-            filtered_working_data["location_search_from"] = filtered_working_data[
-                "City"
-            ].str.cat(
-                [filtered_working_data["State"], filtered_working_data["Country"]],
-                sep=", ",
+        if return_as_arguments:
+            tasks.append(
+                (
+                    process_worksheet,
+                    {
+                        "filtered_working_data": filtered_working_data,
+                        "i": i,
+                        "row": row,
+                        "workflow_sheet": workflow_sheet,
+                        "workflows_sheet": workflows_sheet,
+                    },
+                )
             )
-        settings = get_personalization_settings_from_sheet(workflow_sheet)
-        updated_df = settings.process_from_dataframe(
-            filtered_working_data, filter_out_row
-        )
-        data = prepare_data_for_gsheet(
-            updated_df,
-            {"is_approved": {"TRUE": True, "FALSE": False}},
-            enforced_columns=["Website"],
-        )
-        working_sheet = get_worksheet_from_spreadsheet(workflow_sheet, "WorkingSheet")
-        bulk_update(working_sheet, data)
-        update_date_last_ran(workflows_sheet, i + 2)
-        logger.info(
-            "running_workflow",
-            row_number=i + 2,
-            dataset_size=len(updated_df),
-            sequence_name=row["WorkflowName"],
-            client_name=row["ClientName"],
-            status="COMPLETE",
+        else:
+            process_worksheet(
+                filtered_working_data, i, row, workflow_sheet, workflows_sheet
+            )
+    return tasks
+
+
+def process_worksheet(filtered_working_data, i, row, workflow_sheet, workflows_sheet):
+    logger.info(
+        "running_workflow",
+        row_number=i + 2,
+        dataset_size=len(filtered_working_data),
+        sequence_name=row["WorkflowName"],
+        client_name=row["ClientName"],
+        status="STARTING",
+    )
+    if all(col in filtered_working_data.columns for col in ["Company Name", "City"]):
+        filtered_working_data["search_query"] = filtered_working_data[
+            "Company Name"
+        ].str.cat(filtered_working_data["City"], sep=" ")
+    if all(
+        col in filtered_working_data.columns for col in ["City", "State", "Country"]
+    ):
+        filtered_working_data["location_search_from"] = filtered_working_data[
+            "City"
+        ].str.cat(
+            [filtered_working_data["State"], filtered_working_data["Country"]],
+            sep=", ",
         )
+    settings = get_personalization_settings_from_sheet(workflow_sheet)
+    updated_df = settings.process_from_dataframe(filtered_working_data, filter_out_row)
+    data = prepare_data_for_gsheet(
+        updated_df,
+        {"is_approved": {"TRUE": True, "FALSE": False}},
+        enforced_columns=["Website"],
+    )
+    working_sheet = get_worksheet_from_spreadsheet(workflow_sheet, "WorkingSheet")
+    bulk_update(working_sheet, data)
+    update_date_last_ran(workflows_sheet, i + 2)
+    logger.info(
+        "running_workflow",
+        row_number=i + 2,
+        dataset_size=len(updated_df),
+        sequence_name=row["WorkflowName"],
+        client_name=row["ClientName"],
+        status="COMPLETE",
+    )
+    row = row.fillna("")
+    SETTINGS.notify_webhook(
+        "worksheet_complete",
+        {
+            "client_name": row["ClientName"],
+            "sequence_name": row["WorkflowName"],
+            "workflow_url": row["WorkflowUrl"],
+        },
+    )
+    mark_row_as_completed(workflows_sheet, i)
 
 
 if __name__ == "__main__":
     run_sheets()
```

### Comparing `contact_magic-0.5.7/contact_magic/scripts/sync_scraper_options_to_workersheets.py` & `contact_magic-0.5.8/contact_magic/scripts/sync_scraper_options_to_workersheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.5.8/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/contact_magic/utils.py` & `contact_magic-0.5.8/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.5.7/pyproject.toml` & `contact_magic-0.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.5.7"
+version = "0.5.8"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.5.7/PKG-INFO` & `contact_magic-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.5.7
+Version: 0.5.8
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

