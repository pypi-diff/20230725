# Comparing `tmp/pygments_better_html-0.1.4.tar.gz` & `tmp/pygments_better_html-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygments_better_html-0.1.4.tar", last modified: Thu Mar 26 18:06:12 2020, max compression
+gzip compressed data, was "pygments_better_html-0.1.5.tar", last modified: Tue Jul 25 21:22:58 2023, max compression
```

## Comparing `pygments_better_html-0.1.4.tar` & `pygments_better_html-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kwpolska   (501) staff       (20)        0 2020-03-26 18:06:12.000000 pygments_better_html-0.1.4/
--rw-r--r--   0 kwpolska   (501) staff       (20)       79 2020-03-18 19:12:34.000000 pygments_better_html-0.1.4/AUTHORS
--rw-r--r--   0 kwpolska   (501) staff       (20)      567 2020-03-26 18:05:50.000000 pygments_better_html-0.1.4/CHANGELOG.md
--rw-r--r--   0 kwpolska   (501) staff       (20)     1521 2020-03-18 18:39:42.000000 pygments_better_html-0.1.4/LICENSE
--rw-r--r--   0 kwpolska   (501) staff       (20)     1331 2020-03-18 18:49:54.000000 pygments_better_html-0.1.4/LICENSE.pygments
--rw-r--r--   0 kwpolska   (501) staff       (20)      182 2020-03-18 19:12:14.000000 pygments_better_html-0.1.4/MANIFEST.in
--rw-r--r--   0 kwpolska   (501) staff       (20)      197 2020-03-19 13:20:10.000000 pygments_better_html-0.1.4/Makefile
--rw-r--r--   0 kwpolska   (501) staff       (20)     8024 2020-03-26 18:06:12.000000 pygments_better_html-0.1.4/PKG-INFO
--rw-r--r--   0 kwpolska   (501) staff       (20)     6657 2020-03-26 18:05:14.000000 pygments_better_html-0.1.4/README.md
--rwxr-xr-x   0 kwpolska   (501) staff       (20)     1836 2020-03-19 13:42:13.000000 pygments_better_html-0.1.4/demo.py
-drwxr-xr-x   0 kwpolska   (501) staff       (20)        0 2020-03-26 18:06:12.000000 pygments_better_html-0.1.4/pygments_better_html/
--rw-r--r--   0 kwpolska   (501) staff       (20)     9602 2020-03-26 18:06:06.000000 pygments_better_html-0.1.4/pygments_better_html/__init__.py
-drwxr-xr-x   0 kwpolska   (501) staff       (20)        0 2020-03-26 18:06:12.000000 pygments_better_html-0.1.4/pygments_better_html.egg-info/
--rw-r--r--   0 kwpolska   (501) staff       (20)     8024 2020-03-26 18:06:11.000000 pygments_better_html-0.1.4/pygments_better_html.egg-info/PKG-INFO
--rw-r--r--   0 kwpolska   (501) staff       (20)      420 2020-03-26 18:06:11.000000 pygments_better_html-0.1.4/pygments_better_html.egg-info/SOURCES.txt
--rw-r--r--   0 kwpolska   (501) staff       (20)        1 2020-03-26 18:06:11.000000 pygments_better_html-0.1.4/pygments_better_html.egg-info/dependency_links.txt
--rw-r--r--   0 kwpolska   (501) staff       (20)        1 2020-03-18 19:02:22.000000 pygments_better_html-0.1.4/pygments_better_html.egg-info/not-zip-safe
--rw-r--r--   0 kwpolska   (501) staff       (20)       16 2020-03-26 18:06:11.000000 pygments_better_html-0.1.4/pygments_better_html.egg-info/requires.txt
--rw-r--r--   0 kwpolska   (501) staff       (20)       21 2020-03-26 18:06:11.000000 pygments_better_html-0.1.4/pygments_better_html.egg-info/top_level.txt
--rw-r--r--   0 kwpolska   (501) staff       (20)       57 2020-03-18 18:44:15.000000 pygments_better_html-0.1.4/pyproject.toml
--rw-r--r--   0 kwpolska   (501) staff       (20)      419 2020-03-18 19:02:04.000000 pygments_better_html-0.1.4/requirements.txt
--rw-r--r--   0 kwpolska   (501) staff       (20)       38 2020-03-26 18:06:12.000000 pygments_better_html-0.1.4/setup.cfg
--rwxr-xr-x   0 kwpolska   (501) staff       (20)     1152 2020-03-26 18:06:06.000000 pygments_better_html-0.1.4/setup.py
+drwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)        0 2023-07-25 21:22:58.095391 pygments_better_html-0.1.5/
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)       79 2023-07-25 21:01:17.000000 pygments_better_html-0.1.5/AUTHORS
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)      614 2023-07-25 21:21:18.000000 pygments_better_html-0.1.5/CHANGELOG.md
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)     1526 2023-07-25 21:21:18.000000 pygments_better_html-0.1.5/LICENSE
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)     1331 2023-07-25 21:21:18.000000 pygments_better_html-0.1.5/LICENSE.pygments
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)      182 2023-07-25 21:01:17.000000 pygments_better_html-0.1.5/MANIFEST.in
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)      197 2023-07-25 21:01:17.000000 pygments_better_html-0.1.5/Makefile
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)     7259 2023-07-25 21:22:58.090380 pygments_better_html-0.1.5/PKG-INFO
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)     6662 2023-07-25 21:21:18.000000 pygments_better_html-0.1.5/README.md
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)     1858 2023-07-25 21:05:41.000000 pygments_better_html-0.1.5/demo.py
+drwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)        0 2023-07-25 21:22:57.848397 pygments_better_html-0.1.5/pygments_better_html/
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)     9705 2023-07-25 21:21:18.000000 pygments_better_html-0.1.5/pygments_better_html/__init__.py
+drwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)        0 2023-07-25 21:22:58.047575 pygments_better_html-0.1.5/pygments_better_html.egg-info/
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)     7259 2023-07-25 21:22:54.000000 pygments_better_html-0.1.5/pygments_better_html.egg-info/PKG-INFO
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)      420 2023-07-25 21:22:55.000000 pygments_better_html-0.1.5/pygments_better_html.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)        1 2023-07-25 21:22:54.000000 pygments_better_html-0.1.5/pygments_better_html.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)        1 2023-07-25 21:22:54.000000 pygments_better_html-0.1.5/pygments_better_html.egg-info/not-zip-safe
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)       17 2023-07-25 21:22:54.000000 pygments_better_html-0.1.5/pygments_better_html.egg-info/requires.txt
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)       21 2023-07-25 21:22:54.000000 pygments_better_html-0.1.5/pygments_better_html.egg-info/top_level.txt
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)       57 2023-07-25 21:01:17.000000 pygments_better_html-0.1.5/pyproject.toml
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)      594 2023-07-25 21:22:11.000000 pygments_better_html-0.1.5/requirements.txt
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)       38 2023-07-25 21:22:58.096391 pygments_better_html-0.1.5/setup.cfg
+-rwxrwxrwx   0 kwpolska  (1000) kwpolska  (1000)      957 2023-07-25 21:21:18.000000 pygments_better_html-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pygments_better_html-0.1.4/CHANGELOG.md` & `pygments_better_html-0.1.5/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog for pygments_better_html
 ==================================
 
+v0.1.5
+------
+
+* Support for Pygments 2.15.1.
+
 v0.1.4
 ------
 
 * Preserve blank lines when copying (#1).
 * Minor CSS fix.
 
 v0.1.3
```

### Comparing `pygments_better_html-0.1.4/LICENSE` & `pygments_better_html-0.1.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright © 2020, Chris Warrick.
+Copyright © 2020-2023, Chris Warrick.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
 1. Redistributions of source code must retain the above copyright
```

### Comparing `pygments_better_html-0.1.4/LICENSE.pygments` & `pygments_better_html-0.1.5/LICENSE.pygments`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2006-2019 by the respective authors (see AUTHORS file).
+Copyright (c) 2006-2022 by the respective authors (see AUTHORS file).
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
 * Redistributions of source code must retain the above copyright
```

### Comparing `pygments_better_html-0.1.4/PKG-INFO` & `pygments_better_html-0.1.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,79 @@
-Metadata-Version: 2.1
-Name: pygments_better_html
-Version: 0.1.4
-Summary: Better HTML formatter for Pygments
-Home-page: https://github.com/Kwpolska/pygments_better_html
-Author: Chris Warrick
-Author-email: chris@chriswarrick.com
-License: 3-clause BSD
-Description: Better line numbers for Pygments HTML
-        =====================================
-        
-        This library provides improved line numbers for the Pygments HTML formatter. The `BetterHtmlFormatter` supports two styles:
-        
-        * `linenos="table"` (the default) — every line of the code is a separate table row (a 2xN table, as opposed to Pygments’ standard 2x1 table) This improves the appearance if the code contains characters with unusual line-height, and allows for the code to be word-wrapped with the numbers kept in the right places.
-        * `linenos="ol"` — lines are `<li>` elements in an `<ol>` list.
-        
-        Both styles allow for copy-pasting into a code editor. Directly copy-pasting into Microsoft Word (or similar) might produce something ugly. The first style is inspired by GitHub, and the second can be seen at pastebin.com.
-        
-        The `table` style is more flexible and looks better. The `ol` style is slightly more compatible with broken browsers and minifiers. Pick whichever one works best for you.
-        
-        Usage
-        =====
-        
-        In most cases, it’s a drop-in replacement for `HtmlFormatter`. Just add the import:
-        
-            from pygments_better_html import BetterHtmlFormatter
-        
-        and when calling `highlight()`, instead of `HtmlFormatter`, pass the `BetterHtmlFormatter` class:
-        
-            BetterHtmlFormatter(linenos="table", …other options…)
-            BetterHtmlFormatter(linenos="ol", …other options…)
-        
-        You can see a simple demo in `demo.py`.
-        
-        Required CSS
-        ------------
-        
-        To make this work, you will need to add the following CSS:
-        
-        ```css
-        .highlight table, .highlight tr, .highlight td { border-spacing: 0; border-collapse: separate; padding: 0 }
-        .highlight pre { white-space: pre-wrap; line-height: normal }
-        .highlighttable td.linenos { vertical-align: top; padding-left: 10px; padding-right: 10px; user-select: none; -webkit-user-select: none }
-        .highlighttable td.linenos code:before { content: attr(data-line-number) }
-        .highlighttable td.code { overflow-wrap: normal; border-collapse: collapse }
-        .highlighttable td.code code { overflow: unset; border: none; padding: 0; margin: 0; white-space: pre-wrap; line-height: unset; background: none }
-        .highlight .lineno.nonumber { list-style: none }
-        ```
-        
-        If you’re using ``get_style_defs``, those will be included for you.
-        
-        Browser support
-        ===============
-        
-        All reasonably modern versions of reasonable browsers are supported. Internet Explorer is neither, so it isn’t supported. Firefox, Chrome and Safari are supported. Either mode works with these browsers, although I’ve seen Firefox add extra spaces to the front of lines randomly, and Safari requires an ugly hack for the table mode.
-        
-        Known limitations
-        =================
-        
-        1. The `anchorlinenos` option is not supported for `linenos="ol"`.
-        2. Third-party minifier tools may destroy your indentation if you use tabs. Spaces use a work-around, described in the following point.
-        3. Because of overly clever HTML minifiers, `&nbsp;` tags are used for indentation and sequences of whitespace longer than one character. This might break in the event web browsers decide to copy non-breaking spaces as non-breaking instead of regular spaces. Currently, browsers do the right thing on all platforms. It might also lead to degraded apperance in some edge cases (indentation longer than the code box width, or long runs of spaces inside the code).
-        4. Some completely broken HTML minifiers will remove line numbers, because they are empty tags (that’s the only way to make Safari ignore them on copy-paste). Removing empty tags is just wrong, considering how many browser hacks were built on top of these throughout the years. I saw this issue with HTML Tidy, which is an antique tool detached from reality (even in the HTML5 fork).
-        
-        If you care about compatiblity with bad tools or unusual scenarios, and don’t mind losing `anchorlinenos`, consider using the `lineos="ol"` mode instead of `lineos="table"`.
-        
-        Browsers vs code vs minifiers
-        -----------------------------
-        
-        Limitations (3) and (4) might be considered bugs in my code and not the minifiers. But note that browsers don’t ignore whitespace when parsing, and although the default `white-space: normal` setting for most tags collapses them, you can use `white-space: pre` or `white-space: pre-wrap` to display them. Those minifiers don’t take the CSS into account, and assume the default behavior, collapsing spaces outside of `<pre>` tags. Which is wrong if you override `white-space` on other elements, and “wasteful” if you do `pre { white-space: normal }` for some unusual reason (yeah, don’t do that.)
-        
-        Collapsing whitespace could be worked around with a `<pre>` tag around each line of code, but Firefox will add extra newlines when copying (so the actual code is on every other line of the copied text). This is not avoidable and hard-coded (the plaintext conversion does not look at CSS either, and has a special case for `<pre>` since it makes sense for normal use of that tag. And you can’t wrap the entire table in a `<pre>` tag. If I added one, browsers would move it outside of the table to make the HTML valid. But if browsers do that, some of those clever minifiers might fix HTML syntax as well.
-        
-        I decided to use a different solution, and work around these tools, by using non-breaking spaces for longer runs of spaces. This depends on web browsers replacing those with regular spaces when copying. Luckily, all browsers do this, and considering a 2008 4chan meme (“can’t triforce”, search results might be NSFW), that’s been a thing since forever and is not likely to change.
-        
-        The selected solution of replacing runs of spaces with non-breaking spaces can lead to the code overflowing the box/adding a horizontal scrollbar. Those will happen only in very specific edge cases, i.e. very narrow windows + very large fonts + large indents + no regular (single) spaces close to the indent.
-        
-        I also decided not to apply it to tabs (\t, ^I, U+0009 HORIZONTAL TAB), because tab width can be random, and tabs move the caret to a place, not by a set amount (so in `"a\tb"` and `"aa\tb"`, the `"b"` appears in the same place on the line). Which is generally difficult to handle properly, and you should be using spaces to indent your code anyway.
-        
-        You should also note that GitHub uses both of these techniques, and BitBucket uses the first one. And that it’s easier for everyone to find a better tool if their current tool does stupid stuff.
-        
-        License
-        =======
-        
-        Copyright © 2020, Chris Warrick. Licensed under the 3-clause BSD license.
-        
-        Many parts of the code are taken from Pygments’ original HTMLFormatter, which is copyright © 2006-2019 by the Pygments team, and is licensed under the 2-clause BSD license.
-        
-Keywords: pygments,html,code,highlighting
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Software Development
-Description-Content-Type: text/markdown
+Better line numbers for Pygments HTML
+=====================================
+
+This library provides improved line numbers for the Pygments HTML formatter. The `BetterHtmlFormatter` supports two styles:
+
+* `linenos="table"` (the default) — every line of the code is a separate table row (a 2xN table, as opposed to Pygments’ standard 2x1 table) This improves the appearance if the code contains characters with unusual line-height, and allows for the code to be word-wrapped with the numbers kept in the right places.
+* `linenos="ol"` — lines are `<li>` elements in an `<ol>` list.
+
+Both styles allow for copy-pasting into a code editor. Directly copy-pasting into Microsoft Word (or similar) might produce something ugly. The first style is inspired by GitHub, and the second can be seen at pastebin.com.
+
+The `table` style is more flexible and looks better. The `ol` style is slightly more compatible with broken browsers and minifiers. Pick whichever one works best for you.
+
+Usage
+=====
+
+In most cases, it’s a drop-in replacement for `HtmlFormatter`. Just add the import:
+
+    from pygments_better_html import BetterHtmlFormatter
+
+and when calling `highlight()`, instead of `HtmlFormatter`, pass the `BetterHtmlFormatter` class:
+
+    BetterHtmlFormatter(linenos="table", …other options…)
+    BetterHtmlFormatter(linenos="ol", …other options…)
+
+You can see a simple demo in `demo.py`.
+
+Required CSS
+------------
+
+To make this work, you will need to add the following CSS:
+
+```css
+.highlight table, .highlight tr, .highlight td { border-spacing: 0; border-collapse: separate; padding: 0 }
+.highlight pre { white-space: pre-wrap; line-height: normal }
+.highlighttable td.linenos { vertical-align: top; padding-left: 10px; padding-right: 10px; user-select: none; -webkit-user-select: none }
+.highlighttable td.linenos code:before { content: attr(data-line-number) }
+.highlighttable td.code { overflow-wrap: normal; border-collapse: collapse }
+.highlighttable td.code code { overflow: unset; border: none; padding: 0; margin: 0; white-space: pre-wrap; line-height: unset; background: none }
+.highlight .lineno.nonumber { list-style: none }
+```
+
+If you’re using ``get_style_defs``, those will be included for you.
+
+Browser support
+===============
+
+All reasonably modern versions of reasonable browsers are supported. Internet Explorer is neither, so it isn’t supported. Firefox, Chrome and Safari are supported. Either mode works with these browsers, although I’ve seen Firefox add extra spaces to the front of lines randomly, and Safari requires an ugly hack for the table mode.
+
+Known limitations
+=================
+
+1. The `anchorlinenos` option is not supported for `linenos="ol"`.
+2. Third-party minifier tools may destroy your indentation if you use tabs. Spaces use a work-around, described in the following point.
+3. Because of overly clever HTML minifiers, `&nbsp;` tags are used for indentation and sequences of whitespace longer than one character. This might break in the event web browsers decide to copy non-breaking spaces as non-breaking instead of regular spaces. Currently, browsers do the right thing on all platforms. It might also lead to degraded apperance in some edge cases (indentation longer than the code box width, or long runs of spaces inside the code).
+4. Some completely broken HTML minifiers will remove line numbers, because they are empty tags (that’s the only way to make Safari ignore them on copy-paste). Removing empty tags is just wrong, considering how many browser hacks were built on top of these throughout the years. I saw this issue with HTML Tidy, which is an antique tool detached from reality (even in the HTML5 fork).
+
+If you care about compatiblity with bad tools or unusual scenarios, and don’t mind losing `anchorlinenos`, consider using the `lineos="ol"` mode instead of `lineos="table"`.
+
+Browsers vs code vs minifiers
+-----------------------------
+
+Limitations (3) and (4) might be considered bugs in my code and not the minifiers. But note that browsers don’t ignore whitespace when parsing, and although the default `white-space: normal` setting for most tags collapses them, you can use `white-space: pre` or `white-space: pre-wrap` to display them. Those minifiers don’t take the CSS into account, and assume the default behavior, collapsing spaces outside of `<pre>` tags. Which is wrong if you override `white-space` on other elements, and “wasteful” if you do `pre { white-space: normal }` for some unusual reason (yeah, don’t do that.)
+
+Collapsing whitespace could be worked around with a `<pre>` tag around each line of code, but Firefox will add extra newlines when copying (so the actual code is on every other line of the copied text). This is not avoidable and hard-coded (the plaintext conversion does not look at CSS either, and has a special case for `<pre>` since it makes sense for normal use of that tag. And you can’t wrap the entire table in a `<pre>` tag. If I added one, browsers would move it outside of the table to make the HTML valid. But if browsers do that, some of those clever minifiers might fix HTML syntax as well.
+
+I decided to use a different solution, and work around these tools, by using non-breaking spaces for longer runs of spaces. This depends on web browsers replacing those with regular spaces when copying. Luckily, all browsers do this, and considering a 2008 4chan meme (“can’t triforce”, search results might be NSFW), that’s been a thing since forever and is not likely to change.
+
+The selected solution of replacing runs of spaces with non-breaking spaces can lead to the code overflowing the box/adding a horizontal scrollbar. Those will happen only in very specific edge cases, i.e. very narrow windows + very large fonts + large indents + no regular (single) spaces close to the indent.
+
+I also decided not to apply it to tabs (\t, ^I, U+0009 HORIZONTAL TAB), because tab width can be random, and tabs move the caret to a place, not by a set amount (so in `"a\tb"` and `"aa\tb"`, the `"b"` appears in the same place on the line). Which is generally difficult to handle properly, and you should be using spaces to indent your code anyway.
+
+You should also note that GitHub uses both of these techniques, and BitBucket uses the first one. And that it’s easier for everyone to find a better tool if their current tool does stupid stuff.
+
+License
+=======
+
+Copyright © 2020-2023, Chris Warrick. Licensed under the 3-clause BSD license.
+
+Many parts of the code are taken from Pygments’ original HTMLFormatter, which is copyright © 2006-2022 by the Pygments team, and is licensed under the 2-clause BSD license.
```

### Comparing `pygments_better_html-0.1.4/README.md` & `pygments_better_html-0.1.5/pygments_better_html.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: pygments-better-html
+Version: 0.1.5
+Summary: Better HTML formatter for Pygments
+Home-page: https://github.com/Kwpolska/pygments_better_html
+Author: Chris Warrick
+Author-email: chris@chriswarrick.com
+License: 3-clause BSD
+Keywords: pygments,html,code,highlighting
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE.pygments
+License-File: AUTHORS
+
 Better line numbers for Pygments HTML
 =====================================
 
 This library provides improved line numbers for the Pygments HTML formatter. The `BetterHtmlFormatter` supports two styles:
 
 * `linenos="table"` (the default) — every line of the code is a separate table row (a 2xN table, as opposed to Pygments’ standard 2x1 table) This improves the appearance if the code contains characters with unusual line-height, and allows for the code to be word-wrapped with the numbers kept in the right places.
 * `linenos="ol"` — lines are `<li>` elements in an `<ol>` list.
@@ -70,10 +89,10 @@
 I also decided not to apply it to tabs (\t, ^I, U+0009 HORIZONTAL TAB), because tab width can be random, and tabs move the caret to a place, not by a set amount (so in `"a\tb"` and `"aa\tb"`, the `"b"` appears in the same place on the line). Which is generally difficult to handle properly, and you should be using spaces to indent your code anyway.
 
 You should also note that GitHub uses both of these techniques, and BitBucket uses the first one. And that it’s easier for everyone to find a better tool if their current tool does stupid stuff.
 
 License
 =======
 
-Copyright © 2020, Chris Warrick. Licensed under the 3-clause BSD license.
+Copyright © 2020-2023, Chris Warrick. Licensed under the 3-clause BSD license.
 
-Many parts of the code are taken from Pygments’ original HTMLFormatter, which is copyright © 2006-2019 by the Pygments team, and is licensed under the 2-clause BSD license.
+Many parts of the code are taken from Pygments’ original HTMLFormatter, which is copyright © 2006-2022 by the Pygments team, and is licensed under the 2-clause BSD license.
```

### Comparing `pygments_better_html-0.1.4/demo.py` & `pygments_better_html-0.1.5/demo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 """Demo for BetterHTMLFormatter."""
 
 from pygments import highlight
-from pygments.lexers import HtmlLexer
+from pygments.lexers import PythonLexer
 from pygments_better_html import BetterHtmlFormatter
 
 CODE = """\
 class BetterHtmlFormatter(HtmlFormatter):
     name = "HTML"
     aliases = ["html"]
     filenames = ["*.html", "*.htm"]
@@ -24,19 +24,19 @@
 \t\tAnd this line is indented with two tab characters.
     ""\")
 
 print("Hello, world!")
 """
 
 for linenos, anchorlinenos in (("table", True), ("ol", False)):
-    with open("demo-output-" + linenos + ".html", "w") as fh:
+    with open("demo-output-" + linenos + ".html", "w", encoding="utf-8") as fh:
         fh.write(
             highlight(
                 CODE,
-                HtmlLexer(),
+                PythonLexer(),
                 BetterHtmlFormatter(
                     linenos=linenos,  # "table" or "ol"
                     full=True,
                     hl_lines=[1, 3, 10],
                     linenostart=55,
                     linenostep=2,
                     lineanchors="x",
```

### Comparing `pygments_better_html-0.1.4/pygments_better_html/__init__.py` & `pygments_better_html-0.1.5/pygments_better_html/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """Better HTML formatter for Pygments.
 
-Copyright © 2020, Chris Warrick.
+Copyright © 2020-2021, Chris Warrick.
 License: 3-clause BSD.
 Portions copyright © 2006-2019, the Pygments authors. (2-clause BSD).
 """
 
 __all__ = ["BetterHtmlFormatter"]
 __version__ = "0.1.4"
 
@@ -66,14 +66,18 @@
         new_styles = (
             ("{0} table, {0} tr, {0} td", "border-spacing: 0; border-collapse: separate; padding: 0"),
             ("{0} pre", "white-space: pre-wrap; line-height: normal"),
             (
                 "{0}table td.linenos",
                 "vertical-align: top; padding-left: 10px; padding-right: 10px; user-select: none; -webkit-user-select: none",
             ),
+            (
+                "{0}table td.linenos .special",
+                "padding: 0",
+            ),
             # Hack for Safari (user-select does not affect copy-paste)
             ("{0}table td.linenos code:before", "content: attr(data-line-number)"),
             ("{0}table td.code", "overflow-wrap: normal; border-collapse: collapse"),
             (
                 "{0}table td.code code",
                 "overflow: unset; border: none; padding: 0; margin: 0; white-space: pre-wrap; line-height: unset; background: none",
             ),
@@ -245,13 +249,13 @@
             if self.lineanchors:
                 source = self._wrap_lineanchors(source)
             if self.linespans:
                 source = self._wrap_linespans(source)
             if self.linenos_val == BetterLinenos.TABLE:
                 source = self._wrap_tablelinenos(source)
             if self.linenos_val == BetterLinenos.OL:
-                source = self.wrap(source, outfile)
+                source = self.wrap(source)
             if self.full:
                 source = self._wrap_full(source, outfile)
 
         for t, piece in source:
             outfile.write(piece)
```

### Comparing `pygments_better_html-0.1.4/pygments_better_html.egg-info/PKG-INFO` & `pygments_better_html-0.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,99 +1,98 @@
 Metadata-Version: 2.1
-Name: pygments-better-html
-Version: 0.1.4
+Name: pygments_better_html
+Version: 0.1.5
 Summary: Better HTML formatter for Pygments
 Home-page: https://github.com/Kwpolska/pygments_better_html
 Author: Chris Warrick
 Author-email: chris@chriswarrick.com
 License: 3-clause BSD
-Description: Better line numbers for Pygments HTML
-        =====================================
-        
-        This library provides improved line numbers for the Pygments HTML formatter. The `BetterHtmlFormatter` supports two styles:
-        
-        * `linenos="table"` (the default) — every line of the code is a separate table row (a 2xN table, as opposed to Pygments’ standard 2x1 table) This improves the appearance if the code contains characters with unusual line-height, and allows for the code to be word-wrapped with the numbers kept in the right places.
-        * `linenos="ol"` — lines are `<li>` elements in an `<ol>` list.
-        
-        Both styles allow for copy-pasting into a code editor. Directly copy-pasting into Microsoft Word (or similar) might produce something ugly. The first style is inspired by GitHub, and the second can be seen at pastebin.com.
-        
-        The `table` style is more flexible and looks better. The `ol` style is slightly more compatible with broken browsers and minifiers. Pick whichever one works best for you.
-        
-        Usage
-        =====
-        
-        In most cases, it’s a drop-in replacement for `HtmlFormatter`. Just add the import:
-        
-            from pygments_better_html import BetterHtmlFormatter
-        
-        and when calling `highlight()`, instead of `HtmlFormatter`, pass the `BetterHtmlFormatter` class:
-        
-            BetterHtmlFormatter(linenos="table", …other options…)
-            BetterHtmlFormatter(linenos="ol", …other options…)
-        
-        You can see a simple demo in `demo.py`.
-        
-        Required CSS
-        ------------
-        
-        To make this work, you will need to add the following CSS:
-        
-        ```css
-        .highlight table, .highlight tr, .highlight td { border-spacing: 0; border-collapse: separate; padding: 0 }
-        .highlight pre { white-space: pre-wrap; line-height: normal }
-        .highlighttable td.linenos { vertical-align: top; padding-left: 10px; padding-right: 10px; user-select: none; -webkit-user-select: none }
-        .highlighttable td.linenos code:before { content: attr(data-line-number) }
-        .highlighttable td.code { overflow-wrap: normal; border-collapse: collapse }
-        .highlighttable td.code code { overflow: unset; border: none; padding: 0; margin: 0; white-space: pre-wrap; line-height: unset; background: none }
-        .highlight .lineno.nonumber { list-style: none }
-        ```
-        
-        If you’re using ``get_style_defs``, those will be included for you.
-        
-        Browser support
-        ===============
-        
-        All reasonably modern versions of reasonable browsers are supported. Internet Explorer is neither, so it isn’t supported. Firefox, Chrome and Safari are supported. Either mode works with these browsers, although I’ve seen Firefox add extra spaces to the front of lines randomly, and Safari requires an ugly hack for the table mode.
-        
-        Known limitations
-        =================
-        
-        1. The `anchorlinenos` option is not supported for `linenos="ol"`.
-        2. Third-party minifier tools may destroy your indentation if you use tabs. Spaces use a work-around, described in the following point.
-        3. Because of overly clever HTML minifiers, `&nbsp;` tags are used for indentation and sequences of whitespace longer than one character. This might break in the event web browsers decide to copy non-breaking spaces as non-breaking instead of regular spaces. Currently, browsers do the right thing on all platforms. It might also lead to degraded apperance in some edge cases (indentation longer than the code box width, or long runs of spaces inside the code).
-        4. Some completely broken HTML minifiers will remove line numbers, because they are empty tags (that’s the only way to make Safari ignore them on copy-paste). Removing empty tags is just wrong, considering how many browser hacks were built on top of these throughout the years. I saw this issue with HTML Tidy, which is an antique tool detached from reality (even in the HTML5 fork).
-        
-        If you care about compatiblity with bad tools or unusual scenarios, and don’t mind losing `anchorlinenos`, consider using the `lineos="ol"` mode instead of `lineos="table"`.
-        
-        Browsers vs code vs minifiers
-        -----------------------------
-        
-        Limitations (3) and (4) might be considered bugs in my code and not the minifiers. But note that browsers don’t ignore whitespace when parsing, and although the default `white-space: normal` setting for most tags collapses them, you can use `white-space: pre` or `white-space: pre-wrap` to display them. Those minifiers don’t take the CSS into account, and assume the default behavior, collapsing spaces outside of `<pre>` tags. Which is wrong if you override `white-space` on other elements, and “wasteful” if you do `pre { white-space: normal }` for some unusual reason (yeah, don’t do that.)
-        
-        Collapsing whitespace could be worked around with a `<pre>` tag around each line of code, but Firefox will add extra newlines when copying (so the actual code is on every other line of the copied text). This is not avoidable and hard-coded (the plaintext conversion does not look at CSS either, and has a special case for `<pre>` since it makes sense for normal use of that tag. And you can’t wrap the entire table in a `<pre>` tag. If I added one, browsers would move it outside of the table to make the HTML valid. But if browsers do that, some of those clever minifiers might fix HTML syntax as well.
-        
-        I decided to use a different solution, and work around these tools, by using non-breaking spaces for longer runs of spaces. This depends on web browsers replacing those with regular spaces when copying. Luckily, all browsers do this, and considering a 2008 4chan meme (“can’t triforce”, search results might be NSFW), that’s been a thing since forever and is not likely to change.
-        
-        The selected solution of replacing runs of spaces with non-breaking spaces can lead to the code overflowing the box/adding a horizontal scrollbar. Those will happen only in very specific edge cases, i.e. very narrow windows + very large fonts + large indents + no regular (single) spaces close to the indent.
-        
-        I also decided not to apply it to tabs (\t, ^I, U+0009 HORIZONTAL TAB), because tab width can be random, and tabs move the caret to a place, not by a set amount (so in `"a\tb"` and `"aa\tb"`, the `"b"` appears in the same place on the line). Which is generally difficult to handle properly, and you should be using spaces to indent your code anyway.
-        
-        You should also note that GitHub uses both of these techniques, and BitBucket uses the first one. And that it’s easier for everyone to find a better tool if their current tool does stupid stuff.
-        
-        License
-        =======
-        
-        Copyright © 2020, Chris Warrick. Licensed under the 3-clause BSD license.
-        
-        Many parts of the code are taken from Pygments’ original HTMLFormatter, which is copyright © 2006-2019 by the Pygments team, and is licensed under the 2-clause BSD license.
-        
 Keywords: pygments,html,code,highlighting
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE.pygments
+License-File: AUTHORS
+
+Better line numbers for Pygments HTML
+=====================================
+
+This library provides improved line numbers for the Pygments HTML formatter. The `BetterHtmlFormatter` supports two styles:
+
+* `linenos="table"` (the default) — every line of the code is a separate table row (a 2xN table, as opposed to Pygments’ standard 2x1 table) This improves the appearance if the code contains characters with unusual line-height, and allows for the code to be word-wrapped with the numbers kept in the right places.
+* `linenos="ol"` — lines are `<li>` elements in an `<ol>` list.
+
+Both styles allow for copy-pasting into a code editor. Directly copy-pasting into Microsoft Word (or similar) might produce something ugly. The first style is inspired by GitHub, and the second can be seen at pastebin.com.
+
+The `table` style is more flexible and looks better. The `ol` style is slightly more compatible with broken browsers and minifiers. Pick whichever one works best for you.
+
+Usage
+=====
+
+In most cases, it’s a drop-in replacement for `HtmlFormatter`. Just add the import:
+
+    from pygments_better_html import BetterHtmlFormatter
+
+and when calling `highlight()`, instead of `HtmlFormatter`, pass the `BetterHtmlFormatter` class:
+
+    BetterHtmlFormatter(linenos="table", …other options…)
+    BetterHtmlFormatter(linenos="ol", …other options…)
+
+You can see a simple demo in `demo.py`.
+
+Required CSS
+------------
+
+To make this work, you will need to add the following CSS:
+
+```css
+.highlight table, .highlight tr, .highlight td { border-spacing: 0; border-collapse: separate; padding: 0 }
+.highlight pre { white-space: pre-wrap; line-height: normal }
+.highlighttable td.linenos { vertical-align: top; padding-left: 10px; padding-right: 10px; user-select: none; -webkit-user-select: none }
+.highlighttable td.linenos code:before { content: attr(data-line-number) }
+.highlighttable td.code { overflow-wrap: normal; border-collapse: collapse }
+.highlighttable td.code code { overflow: unset; border: none; padding: 0; margin: 0; white-space: pre-wrap; line-height: unset; background: none }
+.highlight .lineno.nonumber { list-style: none }
+```
+
+If you’re using ``get_style_defs``, those will be included for you.
+
+Browser support
+===============
+
+All reasonably modern versions of reasonable browsers are supported. Internet Explorer is neither, so it isn’t supported. Firefox, Chrome and Safari are supported. Either mode works with these browsers, although I’ve seen Firefox add extra spaces to the front of lines randomly, and Safari requires an ugly hack for the table mode.
+
+Known limitations
+=================
+
+1. The `anchorlinenos` option is not supported for `linenos="ol"`.
+2. Third-party minifier tools may destroy your indentation if you use tabs. Spaces use a work-around, described in the following point.
+3. Because of overly clever HTML minifiers, `&nbsp;` tags are used for indentation and sequences of whitespace longer than one character. This might break in the event web browsers decide to copy non-breaking spaces as non-breaking instead of regular spaces. Currently, browsers do the right thing on all platforms. It might also lead to degraded apperance in some edge cases (indentation longer than the code box width, or long runs of spaces inside the code).
+4. Some completely broken HTML minifiers will remove line numbers, because they are empty tags (that’s the only way to make Safari ignore them on copy-paste). Removing empty tags is just wrong, considering how many browser hacks were built on top of these throughout the years. I saw this issue with HTML Tidy, which is an antique tool detached from reality (even in the HTML5 fork).
+
+If you care about compatiblity with bad tools or unusual scenarios, and don’t mind losing `anchorlinenos`, consider using the `lineos="ol"` mode instead of `lineos="table"`.
+
+Browsers vs code vs minifiers
+-----------------------------
+
+Limitations (3) and (4) might be considered bugs in my code and not the minifiers. But note that browsers don’t ignore whitespace when parsing, and although the default `white-space: normal` setting for most tags collapses them, you can use `white-space: pre` or `white-space: pre-wrap` to display them. Those minifiers don’t take the CSS into account, and assume the default behavior, collapsing spaces outside of `<pre>` tags. Which is wrong if you override `white-space` on other elements, and “wasteful” if you do `pre { white-space: normal }` for some unusual reason (yeah, don’t do that.)
+
+Collapsing whitespace could be worked around with a `<pre>` tag around each line of code, but Firefox will add extra newlines when copying (so the actual code is on every other line of the copied text). This is not avoidable and hard-coded (the plaintext conversion does not look at CSS either, and has a special case for `<pre>` since it makes sense for normal use of that tag. And you can’t wrap the entire table in a `<pre>` tag. If I added one, browsers would move it outside of the table to make the HTML valid. But if browsers do that, some of those clever minifiers might fix HTML syntax as well.
+
+I decided to use a different solution, and work around these tools, by using non-breaking spaces for longer runs of spaces. This depends on web browsers replacing those with regular spaces when copying. Luckily, all browsers do this, and considering a 2008 4chan meme (“can’t triforce”, search results might be NSFW), that’s been a thing since forever and is not likely to change.
+
+The selected solution of replacing runs of spaces with non-breaking spaces can lead to the code overflowing the box/adding a horizontal scrollbar. Those will happen only in very specific edge cases, i.e. very narrow windows + very large fonts + large indents + no regular (single) spaces close to the indent.
+
+I also decided not to apply it to tabs (\t, ^I, U+0009 HORIZONTAL TAB), because tab width can be random, and tabs move the caret to a place, not by a set amount (so in `"a\tb"` and `"aa\tb"`, the `"b"` appears in the same place on the line). Which is generally difficult to handle properly, and you should be using spaces to indent your code anyway.
+
+You should also note that GitHub uses both of these techniques, and BitBucket uses the first one. And that it’s easier for everyone to find a better tool if their current tool does stupid stuff.
+
+License
+=======
+
+Copyright © 2020-2023, Chris Warrick. Licensed under the 3-clause BSD license.
+
+Many parts of the code are taken from Pygments’ original HTMLFormatter, which is copyright © 2006-2022 by the Pygments team, and is licensed under the 2-clause BSD license.
```

### Comparing `pygments_better_html-0.1.4/setup.py` & `pygments_better_html-0.1.5/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- encoding: utf-8 -*-
 import io
 from setuptools import setup, find_packages
 
 
 setup(
     name="pygments_better_html",
-    version="0.1.4",
+    version="0.1.5",
     description="Better HTML formatter for Pygments",
     keywords="pygments,html,code,highlighting",
     author="Chris Warrick",
     author_email="chris@chriswarrick.com",
     url="https://github.com/Kwpolska/pygments_better_html",
     license="3-clause BSD",
     long_description=io.open("./README.md", "r", encoding="utf-8").read(),
@@ -18,17 +18,13 @@
     platforms="any",
     zip_safe=False,
     # http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Topic :: Software Development",
     ],
     packages=find_packages(),
     include_package_data=True,
-    install_requires=["Pygments>=2.0.0"],
+    install_requires=["Pygments>=2.15.1"],
 )
```

