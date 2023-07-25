# Comparing `tmp/medit-0.0.8.tar.gz` & `tmp/medit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medit-0.0.8.tar", max compression
+gzip compressed data, was "medit-0.0.9.tar", max compression
```

## Comparing `medit-0.0.8.tar` & `medit-0.0.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     3399 2023-07-25 17:45:28.116423 medit-0.0.8/Readme.md
--rw-r--r--   0        0        0        0 2023-07-01 03:43:26.302528 medit-0.0.8/medit/__init__.py
--rwxr-xr-x   0        0        0     2192 2023-07-25 16:55:11.883381 medit-0.0.8/medit/cli.py
--rw-r--r--   0        0        0     2340 2023-07-25 17:49:29.441015 medit-0.0.8/medit/medit.ui
--rw-r--r--   0        0        0     5067 2023-07-25 16:55:11.883381 medit-0.0.8/medit/meditor.py
--rw-r--r--   0        0        0     7873 2023-07-25 16:55:11.884381 medit-0.0.8/medit/mview.py
--rw-r--r--   0        0        0        0 2023-07-02 16:04:58.958106 medit-0.0.8/medit/styles/__init__.py
--rw-r--r--   0        0        0    18966 2023-07-02 11:28:30.508468 medit-0.0.8/medit/styles/external/github-markdown-dark.css
--rw-r--r--   0        0        0    18979 2023-07-02 11:28:30.508468 medit-0.0.8/medit/styles/external/github-markdown-light.css
--rw-r--r--   0        0        0    23562 2022-09-24 11:57:23.000000 medit-0.0.8/medit/styles/external/github-markdown.css
--rw-r--r--   0        0        0     5061 2023-07-02 11:28:30.508468 medit-0.0.8/medit/styles/external/pygments-solarized-style/solarized-dark.css
--rw-r--r--   0        0        0     5061 2023-07-02 11:28:30.508468 medit-0.0.8/medit/styles/external/pygments-solarized-style/solarized-light.css
--rw-r--r--   0        0        0     2247 2023-07-02 08:09:35.126975 medit-0.0.8/medit/styles/external/retro.css
--rw-r--r--   0        0        0    36899 2023-07-02 11:28:30.509468 medit-0.0.8/medit/styles/external/solarized-dark-all-sites.css
--rw-r--r--   0        0        0    36890 2023-07-02 11:28:30.509468 medit-0.0.8/medit/styles/external/solarized-light-all-sites.css
--rw-r--r--   0        0        0     4282 2023-07-02 11:28:30.509468 medit-0.0.8/medit/styles/external/thomasf-solarized-css/solarized-dark.css
--rw-r--r--   0        0        0     4282 2023-07-02 11:28:30.509468 medit-0.0.8/medit/styles/external/thomasf-solarized-css/solarized-light.css
--rw-r--r--   0        0        0     2831 2023-07-02 10:24:56.448801 medit-0.0.8/medit/styles/markdown.min.css
--rw-r--r--   0        0        0     4046 2023-07-02 08:45:15.342414 medit-0.0.8/medit/styles/pygments/abap.css
--rw-r--r--   0        0        0     4106 2023-07-02 08:45:15.978432 medit-0.0.8/medit/styles/pygments/algol.css
--rw-r--r--   0        0        0     3910 2023-07-02 08:45:15.664423 medit-0.0.8/medit/styles/pygments/algol_nu.css
--rw-r--r--   0        0        0     3955 2023-07-02 08:45:16.299441 medit-0.0.8/medit/styles/pygments/arduino.css
--rw-r--r--   0        0        0     4556 2023-07-02 08:45:16.618450 medit-0.0.8/medit/styles/pygments/autumn.css
--rw-r--r--   0        0        0     3826 2023-07-02 08:45:16.940460 medit-0.0.8/medit/styles/pygments/borland.css
--rw-r--r--   0        0        0     2865 2023-07-02 08:45:17.260469 medit-0.0.8/medit/styles/pygments/bw.css
--rw-r--r--   0        0        0     5200 2023-07-02 08:45:17.583478 medit-0.0.8/medit/styles/pygments/colorful.css
--rw-r--r--   0        0        0     4889 2023-07-02 08:45:17.900487 medit-0.0.8/medit/styles/pygments/default.css
--rw-r--r--   0        0        0     5159 2023-07-02 08:45:18.220497 medit-0.0.8/medit/styles/pygments/dracula.css
--rw-r--r--   0        0        0     4888 2023-07-02 08:45:18.538506 medit-0.0.8/medit/styles/pygments/emacs.css
--rw-r--r--   0        0        0     4916 2023-07-02 08:45:19.181524 medit-0.0.8/medit/styles/pygments/friendly.css
--rw-r--r--   0        0        0     4916 2023-07-02 08:45:18.860515 medit-0.0.8/medit/styles/pygments/friendly_grayscale.css
--rw-r--r--   0        0        0     5687 2023-07-02 08:45:19.500533 medit-0.0.8/medit/styles/pygments/fruity.css
--rw-r--r--   0        0        0     2565 2023-07-02 08:45:20.520563 medit-0.0.8/medit/styles/pygments/igor.css
--rw-r--r--   0        0        0     5248 2023-07-02 08:45:21.192582 medit-0.0.8/medit/styles/pygments/inkpot.css
--rw-r--r--   0        0        0     4458 2023-07-02 08:45:21.513591 medit-0.0.8/medit/styles/pygments/lilypond.css
--rw-r--r--   0        0        0     4805 2023-07-02 08:45:21.835600 medit-0.0.8/medit/styles/pygments/lovelace.css
--rw-r--r--   0        0        0     5000 2023-07-02 08:45:22.153610 medit-0.0.8/medit/styles/pygments/manni.css
--rw-r--r--   0        0        0     5097 2023-07-02 08:45:22.474619 medit-0.0.8/medit/styles/pygments/material.css
--rw-r--r--   0        0        0     5036 2023-07-02 08:45:22.790628 medit-0.0.8/medit/styles/pygments/monokai.css
--rw-r--r--   0        0        0     5282 2023-07-02 08:45:23.113637 medit-0.0.8/medit/styles/pygments/murphy.css
--rw-r--r--   0        0        0     5437 2023-07-02 08:45:23.440647 medit-0.0.8/medit/styles/pygments/native.css
--rw-r--r--   0        0        0     5312 2023-07-02 08:45:23.766656 medit-0.0.8/medit/styles/pygments/nord.css
--rw-r--r--   0        0        0     5330 2023-07-02 08:45:25.136695 medit-0.0.8/medit/styles/pygments/pastie.css
--rw-r--r--   0        0        0     4602 2023-07-02 08:45:25.457705 medit-0.0.8/medit/styles/pygments/perldoc.css
--rw-r--r--   0        0        0     4845 2023-07-02 08:45:25.778714 medit-0.0.8/medit/styles/pygments/rainbow_dash.css
--rw-r--r--   0        0        0     4951 2023-07-02 08:45:26.102723 medit-0.0.8/medit/styles/pygments/rrt.css
--rw-r--r--   0        0        0     4421 2023-07-02 08:45:26.421733 medit-0.0.8/medit/styles/pygments/sas.css
--rw-r--r--   0        0        0     4951 2023-07-02 08:45:27.095752 medit-0.0.8/medit/styles/pygments/staroffice.css
--rw-r--r--   0        0        0     5589 2023-07-02 08:45:28.112781 medit-0.0.8/medit/styles/pygments/tango.css
--rw-r--r--   0        0        0     4684 2023-07-02 08:45:28.434790 medit-0.0.8/medit/styles/pygments/trac.css
--rw-r--r--   0        0        0     5112 2023-07-02 08:45:28.758800 medit-0.0.8/medit/styles/pygments/vim.css
--rw-r--r--   0        0        0     2666 2023-07-02 08:45:29.079809 medit-0.0.8/medit/styles/pygments/vs.css
--rw-r--r--   0        0        0     4057 2023-07-02 08:45:29.402818 medit-0.0.8/medit/styles/pygments/xcode.css
--rw-r--r--   0        0        0     5506 2023-07-02 08:45:29.728828 medit-0.0.8/medit/styles/pygments/zenburn.css
--rwxr-xr-x   0        0        0     9923 2023-07-25 19:18:23.170479 medit-0.0.8/medit/ui.py
--rw-r--r--   0        0        0     5361 2023-07-25 16:55:11.884381 medit-0.0.8/medit/utils.py
--rw-r--r--   0        0        0     2393 2023-07-25 17:15:38.969466 medit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 medit-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3399 2023-07-25 17:45:28.116423 medit-0.0.9/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-01 03:43:26.302528 medit-0.0.9/medit/__init__.py
+-rwxr-xr-x   0        0        0     2192 2023-07-25 16:55:11.883381 medit-0.0.9/medit/cli.py
+-rw-r--r--   0        0        0     2340 2023-07-25 17:49:29.441015 medit-0.0.9/medit/medit.ui
+-rw-r--r--   0        0        0     5067 2023-07-25 16:55:11.883381 medit-0.0.9/medit/meditor.py
+-rw-r--r--   0        0        0     7895 2023-07-25 19:39:22.893076 medit-0.0.9/medit/mview.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:04:58.958106 medit-0.0.9/medit/styles/__init__.py
+-rw-r--r--   0        0        0    18966 2023-07-02 11:28:30.508468 medit-0.0.9/medit/styles/external/github-markdown-dark.css
+-rw-r--r--   0        0        0    18979 2023-07-02 11:28:30.508468 medit-0.0.9/medit/styles/external/github-markdown-light.css
+-rw-r--r--   0        0        0    23562 2022-09-24 11:57:23.000000 medit-0.0.9/medit/styles/external/github-markdown.css
+-rw-r--r--   0        0        0     5061 2023-07-02 11:28:30.508468 medit-0.0.9/medit/styles/external/pygments-solarized-style/solarized-dark.css
+-rw-r--r--   0        0        0     5061 2023-07-02 11:28:30.508468 medit-0.0.9/medit/styles/external/pygments-solarized-style/solarized-light.css
+-rw-r--r--   0        0        0     2247 2023-07-02 08:09:35.126975 medit-0.0.9/medit/styles/external/retro.css
+-rw-r--r--   0        0        0    36899 2023-07-02 11:28:30.509468 medit-0.0.9/medit/styles/external/solarized-dark-all-sites.css
+-rw-r--r--   0        0        0    36890 2023-07-02 11:28:30.509468 medit-0.0.9/medit/styles/external/solarized-light-all-sites.css
+-rw-r--r--   0        0        0     4282 2023-07-02 11:28:30.509468 medit-0.0.9/medit/styles/external/thomasf-solarized-css/solarized-dark.css
+-rw-r--r--   0        0        0     4282 2023-07-02 11:28:30.509468 medit-0.0.9/medit/styles/external/thomasf-solarized-css/solarized-light.css
+-rw-r--r--   0        0        0     2831 2023-07-02 10:24:56.448801 medit-0.0.9/medit/styles/markdown.min.css
+-rw-r--r--   0        0        0     4046 2023-07-02 08:45:15.342414 medit-0.0.9/medit/styles/pygments/abap.css
+-rw-r--r--   0        0        0     4106 2023-07-02 08:45:15.978432 medit-0.0.9/medit/styles/pygments/algol.css
+-rw-r--r--   0        0        0     3910 2023-07-02 08:45:15.664423 medit-0.0.9/medit/styles/pygments/algol_nu.css
+-rw-r--r--   0        0        0     3955 2023-07-02 08:45:16.299441 medit-0.0.9/medit/styles/pygments/arduino.css
+-rw-r--r--   0        0        0     4556 2023-07-02 08:45:16.618450 medit-0.0.9/medit/styles/pygments/autumn.css
+-rw-r--r--   0        0        0     3826 2023-07-02 08:45:16.940460 medit-0.0.9/medit/styles/pygments/borland.css
+-rw-r--r--   0        0        0     2865 2023-07-02 08:45:17.260469 medit-0.0.9/medit/styles/pygments/bw.css
+-rw-r--r--   0        0        0     5200 2023-07-02 08:45:17.583478 medit-0.0.9/medit/styles/pygments/colorful.css
+-rw-r--r--   0        0        0     4889 2023-07-02 08:45:17.900487 medit-0.0.9/medit/styles/pygments/default.css
+-rw-r--r--   0        0        0     5159 2023-07-02 08:45:18.220497 medit-0.0.9/medit/styles/pygments/dracula.css
+-rw-r--r--   0        0        0     4888 2023-07-02 08:45:18.538506 medit-0.0.9/medit/styles/pygments/emacs.css
+-rw-r--r--   0        0        0     4916 2023-07-02 08:45:19.181524 medit-0.0.9/medit/styles/pygments/friendly.css
+-rw-r--r--   0        0        0     4916 2023-07-02 08:45:18.860515 medit-0.0.9/medit/styles/pygments/friendly_grayscale.css
+-rw-r--r--   0        0        0     5687 2023-07-02 08:45:19.500533 medit-0.0.9/medit/styles/pygments/fruity.css
+-rw-r--r--   0        0        0     2565 2023-07-02 08:45:20.520563 medit-0.0.9/medit/styles/pygments/igor.css
+-rw-r--r--   0        0        0     5248 2023-07-02 08:45:21.192582 medit-0.0.9/medit/styles/pygments/inkpot.css
+-rw-r--r--   0        0        0     4458 2023-07-02 08:45:21.513591 medit-0.0.9/medit/styles/pygments/lilypond.css
+-rw-r--r--   0        0        0     4805 2023-07-02 08:45:21.835600 medit-0.0.9/medit/styles/pygments/lovelace.css
+-rw-r--r--   0        0        0     5000 2023-07-02 08:45:22.153610 medit-0.0.9/medit/styles/pygments/manni.css
+-rw-r--r--   0        0        0     5097 2023-07-02 08:45:22.474619 medit-0.0.9/medit/styles/pygments/material.css
+-rw-r--r--   0        0        0     5036 2023-07-02 08:45:22.790628 medit-0.0.9/medit/styles/pygments/monokai.css
+-rw-r--r--   0        0        0     5282 2023-07-02 08:45:23.113637 medit-0.0.9/medit/styles/pygments/murphy.css
+-rw-r--r--   0        0        0     5437 2023-07-02 08:45:23.440647 medit-0.0.9/medit/styles/pygments/native.css
+-rw-r--r--   0        0        0     5312 2023-07-02 08:45:23.766656 medit-0.0.9/medit/styles/pygments/nord.css
+-rw-r--r--   0        0        0     5330 2023-07-02 08:45:25.136695 medit-0.0.9/medit/styles/pygments/pastie.css
+-rw-r--r--   0        0        0     4602 2023-07-02 08:45:25.457705 medit-0.0.9/medit/styles/pygments/perldoc.css
+-rw-r--r--   0        0        0     4845 2023-07-02 08:45:25.778714 medit-0.0.9/medit/styles/pygments/rainbow_dash.css
+-rw-r--r--   0        0        0     4951 2023-07-02 08:45:26.102723 medit-0.0.9/medit/styles/pygments/rrt.css
+-rw-r--r--   0        0        0     4421 2023-07-02 08:45:26.421733 medit-0.0.9/medit/styles/pygments/sas.css
+-rw-r--r--   0        0        0     4951 2023-07-02 08:45:27.095752 medit-0.0.9/medit/styles/pygments/staroffice.css
+-rw-r--r--   0        0        0     5589 2023-07-02 08:45:28.112781 medit-0.0.9/medit/styles/pygments/tango.css
+-rw-r--r--   0        0        0     4684 2023-07-02 08:45:28.434790 medit-0.0.9/medit/styles/pygments/trac.css
+-rw-r--r--   0        0        0     5112 2023-07-02 08:45:28.758800 medit-0.0.9/medit/styles/pygments/vim.css
+-rw-r--r--   0        0        0     2666 2023-07-02 08:45:29.079809 medit-0.0.9/medit/styles/pygments/vs.css
+-rw-r--r--   0        0        0     4057 2023-07-02 08:45:29.402818 medit-0.0.9/medit/styles/pygments/xcode.css
+-rw-r--r--   0        0        0     5506 2023-07-02 08:45:29.728828 medit-0.0.9/medit/styles/pygments/zenburn.css
+-rwxr-xr-x   0        0        0     9923 2023-07-25 19:18:23.170479 medit-0.0.9/medit/ui.py
+-rw-r--r--   0        0        0     5361 2023-07-25 16:55:11.884381 medit-0.0.9/medit/utils.py
+-rw-r--r--   0        0        0     2393 2023-07-25 19:39:42.484677 medit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 medit-0.0.9/PKG-INFO
```

### Comparing `medit-0.0.8/Readme.md` & `medit-0.0.9/Readme.md`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/cli.py` & `medit-0.0.9/medit/cli.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/medit.ui` & `medit-0.0.9/medit/medit.ui`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/meditor.py` & `medit-0.0.9/medit/meditor.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/mview.py` & `medit-0.0.9/medit/mview.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,28 +96,28 @@
                 # "styles/pygments/vs.css",  #                 | light, transparent, decent
                 # "styles/pygments/xcode.css",  #              | light, transparent, decent
                 # "styles/pygments/zenburn.css",  #            | dark
             )
         )
 
     def show(self, content, highlight_mode, base_dir: Path):
-
+        content = "AÄOÖ"
         if highlight_mode == ".md":
             html, style = (
                 markdown(
                     content,
                     extensions=[
                         "extra",
                         "codehilite",
                         "markdown_checklist.extension",
-                        "md_mermaid",
+                        #"md_mermaid",
                         MarkdownInclude(
                             configs={
                                 "base_path": base_dir,
-                                "encoding": "iso-8859-1",
+                                "encoding": "utf-8",
                             }
                         ),
                     ],
                 ),
                 self.css_content_markdown,
             )
         else:
@@ -137,15 +137,15 @@
             html, style = highlight(content, lexer, formatter), self.css_content
 
         #        print(html)
         self.setHtml(
             f"""
 <!doctype html>
 <html lang="en">
-  <meta charset="utf-8"><head>{style}</head></meta>
+  <meta charset="UTF-8"><head>{style}</head></meta>
   <body class="markdown-body markdown">{html}</body>
 </html>
         """
         )
 
         return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `medit-0.0.8/medit/styles/external/github-markdown-dark.css` & `medit-0.0.9/medit/styles/external/github-markdown-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/external/github-markdown-light.css` & `medit-0.0.9/medit/styles/external/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/external/github-markdown.css` & `medit-0.0.9/medit/styles/external/github-markdown.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/external/pygments-solarized-style/solarized-dark.css` & `medit-0.0.9/medit/styles/external/pygments-solarized-style/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/external/pygments-solarized-style/solarized-light.css` & `medit-0.0.9/medit/styles/external/pygments-solarized-style/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/external/retro.css` & `medit-0.0.9/medit/styles/external/retro.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/external/solarized-dark-all-sites.css` & `medit-0.0.9/medit/styles/external/solarized-dark-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/external/solarized-light-all-sites.css` & `medit-0.0.9/medit/styles/external/solarized-light-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/external/thomasf-solarized-css/solarized-dark.css` & `medit-0.0.9/medit/styles/external/thomasf-solarized-css/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/external/thomasf-solarized-css/solarized-light.css` & `medit-0.0.9/medit/styles/external/thomasf-solarized-css/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/markdown.min.css` & `medit-0.0.9/medit/styles/markdown.min.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/abap.css` & `medit-0.0.9/medit/styles/pygments/abap.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/algol.css` & `medit-0.0.9/medit/styles/pygments/algol.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/algol_nu.css` & `medit-0.0.9/medit/styles/pygments/algol_nu.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/arduino.css` & `medit-0.0.9/medit/styles/pygments/arduino.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/autumn.css` & `medit-0.0.9/medit/styles/pygments/autumn.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/borland.css` & `medit-0.0.9/medit/styles/pygments/borland.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/bw.css` & `medit-0.0.9/medit/styles/pygments/bw.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/colorful.css` & `medit-0.0.9/medit/styles/pygments/colorful.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/default.css` & `medit-0.0.9/medit/styles/pygments/default.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/dracula.css` & `medit-0.0.9/medit/styles/pygments/dracula.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/emacs.css` & `medit-0.0.9/medit/styles/pygments/emacs.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/friendly.css` & `medit-0.0.9/medit/styles/pygments/friendly.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/friendly_grayscale.css` & `medit-0.0.9/medit/styles/pygments/friendly_grayscale.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/fruity.css` & `medit-0.0.9/medit/styles/pygments/fruity.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/igor.css` & `medit-0.0.9/medit/styles/pygments/igor.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/inkpot.css` & `medit-0.0.9/medit/styles/pygments/inkpot.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/lilypond.css` & `medit-0.0.9/medit/styles/pygments/lilypond.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/lovelace.css` & `medit-0.0.9/medit/styles/pygments/lovelace.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/manni.css` & `medit-0.0.9/medit/styles/pygments/manni.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/material.css` & `medit-0.0.9/medit/styles/pygments/material.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/monokai.css` & `medit-0.0.9/medit/styles/pygments/monokai.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/murphy.css` & `medit-0.0.9/medit/styles/pygments/murphy.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/native.css` & `medit-0.0.9/medit/styles/pygments/native.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/nord.css` & `medit-0.0.9/medit/styles/pygments/nord.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/pastie.css` & `medit-0.0.9/medit/styles/pygments/pastie.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/perldoc.css` & `medit-0.0.9/medit/styles/pygments/perldoc.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/rainbow_dash.css` & `medit-0.0.9/medit/styles/pygments/rainbow_dash.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/rrt.css` & `medit-0.0.9/medit/styles/pygments/rrt.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/sas.css` & `medit-0.0.9/medit/styles/pygments/sas.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/staroffice.css` & `medit-0.0.9/medit/styles/pygments/staroffice.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/tango.css` & `medit-0.0.9/medit/styles/pygments/tango.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/trac.css` & `medit-0.0.9/medit/styles/pygments/trac.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/vim.css` & `medit-0.0.9/medit/styles/pygments/vim.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/vs.css` & `medit-0.0.9/medit/styles/pygments/vs.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/xcode.css` & `medit-0.0.9/medit/styles/pygments/xcode.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/styles/pygments/zenburn.css` & `medit-0.0.9/medit/styles/pygments/zenburn.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/ui.py` & `medit-0.0.9/medit/ui.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/medit/utils.py` & `medit-0.0.9/medit/utils.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.8/pyproject.toml` & `medit-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medit"
-version = "0.0.8"
+version = "0.0.9"
 description = "Markup Editor"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/medit.git"
 readme = "Readme.md"
 packages = [
   {include = "medit/**/*.py"},
   {include = "medit/**/*.ui"},
```

### Comparing `medit-0.0.8/PKG-INFO` & `medit-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Markup Editor
 Home-page: https://projects.om-office.de/frans/medit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

