# Comparing `tmp/mdnet-0.1.1.tar.gz` & `tmp/mdnet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdnet-0.1.1.tar", last modified: Sun Jul 16 12:23:50 2023, max compression
+gzip compressed data, was "mdnet-0.1.2.tar", last modified: Tue Jul 25 07:32:31 2023, max compression
```

## Comparing `mdnet-0.1.1.tar` & `mdnet-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 gnat      (1000) gnat      (1000)        0 2023-07-16 12:23:50.395879 mdnet-0.1.1/
--rw-r--r--   0 gnat      (1000) gnat      (1000)       49 2023-07-16 12:23:50.394879 mdnet-0.1.1/PKG-INFO
--rw-r--r--   0 gnat      (1000) gnat      (1000)     2502 2023-07-16 12:21:28.000000 mdnet-0.1.1/README.md
-drwxr-xr-x   0 gnat      (1000) gnat      (1000)        0 2023-07-16 12:23:50.394879 mdnet-0.1.1/mdnet/
--rw-r--r--   0 gnat      (1000) gnat      (1000)     2133 2023-07-16 12:13:07.000000 mdnet-0.1.1/mdnet/mdnet.py
--rw-r--r--   0 gnat      (1000) gnat      (1000)      303 2023-07-16 12:17:34.000000 mdnet-0.1.1/mdnet/setup.py
-drwxr-xr-x   0 gnat      (1000) gnat      (1000)        0 2023-07-16 12:23:50.394879 mdnet-0.1.1/mdnet.egg-info/
--rw-r--r--   0 gnat      (1000) gnat      (1000)       49 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/PKG-INFO
--rw-r--r--   0 gnat      (1000) gnat      (1000)      215 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/SOURCES.txt
--rw-r--r--   0 gnat      (1000) gnat      (1000)        1 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/dependency_links.txt
--rw-r--r--   0 gnat      (1000) gnat      (1000)       43 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/entry_points.txt
--rw-r--r--   0 gnat      (1000) gnat      (1000)       35 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/requires.txt
--rw-r--r--   0 gnat      (1000) gnat      (1000)        6 2023-07-16 12:23:50.000000 mdnet-0.1.1/mdnet.egg-info/top_level.txt
--rw-r--r--   0 gnat      (1000) gnat      (1000)       38 2023-07-16 12:23:50.395879 mdnet-0.1.1/setup.cfg
+drwxr-xr-x   0 gnat      (1000) users      (100)        0 2023-07-25 07:32:31.576781 mdnet-0.1.2/
+-rw-r--r--   0 gnat      (1000) users      (100)       49 2023-07-25 07:32:31.576781 mdnet-0.1.2/PKG-INFO
+-rwxr-xr-x   0 gnat      (1000) users      (100)     3859 2023-07-25 07:17:37.000000 mdnet-0.1.2/README.md
+drwxr-xr-x   0 gnat      (1000) users      (100)        0 2023-07-25 07:32:31.575781 mdnet-0.1.2/mdnet/
+-rw-r--r--   0 gnat      (1000) users      (100)        0 2023-07-25 07:21:58.000000 mdnet-0.1.2/mdnet/__init__.py
+-rwxr-xr-x   0 gnat      (1000) users      (100)     3148 2023-07-25 07:07:48.000000 mdnet-0.1.2/mdnet/mdnet.py
+drwxr-xr-x   0 gnat      (1000) users      (100)        0 2023-07-25 07:32:31.576781 mdnet-0.1.2/mdnet.egg-info/
+-rwxr-xr-x   0 gnat      (1000) users      (100)       49 2023-07-25 07:32:31.000000 mdnet-0.1.2/mdnet.egg-info/PKG-INFO
+-rwxr-xr-x   0 gnat      (1000) users      (100)      227 2023-07-25 07:32:31.000000 mdnet-0.1.2/mdnet.egg-info/SOURCES.txt
+-rwxr-xr-x   0 gnat      (1000) users      (100)        1 2023-07-25 07:32:31.000000 mdnet-0.1.2/mdnet.egg-info/dependency_links.txt
+-rwxr-xr-x   0 gnat      (1000) users      (100)       43 2023-07-25 07:32:31.000000 mdnet-0.1.2/mdnet.egg-info/entry_points.txt
+-rwxr-xr-x   0 gnat      (1000) users      (100)       35 2023-07-25 07:32:31.000000 mdnet-0.1.2/mdnet.egg-info/requires.txt
+-rwxr-xr-x   0 gnat      (1000) users      (100)        6 2023-07-25 07:32:31.000000 mdnet-0.1.2/mdnet.egg-info/top_level.txt
+-rw-r--r--   0 gnat      (1000) users      (100)       38 2023-07-25 07:32:31.576781 mdnet-0.1.2/setup.cfg
+-rwxr-xr-x   0 gnat      (1000) users      (100)      303 2023-07-25 07:29:34.000000 mdnet-0.1.2/setup.py
```

### Comparing `mdnet-0.1.1/README.md` & `mdnet-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,94 @@
 # MDNet: A Static Site Generator
-MDNet is a simple static site generator that converts Markdown files into HTML files. It uses Jinja2 for templating and supports metadata in the form of YAML Front Matter
+MDNet is a simple static site generator that converts Markdown files into HTML files. It uses Jinja2 for templating and supports metadata in the form of YAML Front Matter.
 
 ## Features
-- Coverts Markdown files to HTML
+- Converts Markdown files to HTML
 - Supports YAML Front Matter for metadata
 - Generates an index page with links to all posts
+- Generates tag pages with links to all posts with a given tag
 - Customizable with Jinja2 templates
 
 ## Installation
 You can install MDNet with pip:
-```
+
+```bash
 pip install mdnet
 ```
 This will install MDNet and its dependencies, and create a command line script that you can use to run MDNet.
 
 ## Usage
 After installing MDNet, you can use it like this:
 ```
-mdnet input_dir output_dir template_path index_template_path
+mdnet input_dir output_dir post_template_path index_template_path tag_template_path
 ```
-- input_dir is the directory containing the Markdown files.
-- output_dir is the directory to output the HTML files to.
-- template_path is the path to the HTML template for the posts.
-- index_template_path is the path to the HTML template for the index page.
+- `input_dir` is the directory containing the Markdown files.
+- `output_dir` is the directory to output the HTML files to.
+- `post_template_path` is the path to the HTML template for the posts.
+- `index_template_path` is the path to the HTML template for the index page.
+- `tag_template_path` is the path to the HTML template for the tag pages.
+
+The templates should be Jinja2 templates.
+
+The post template will be rendered with the following variables:
 
-The templates should be Jinja2 templates. The post template will be rendered with the following variables:
 - 'title': The title of the post
 - 'date': the date of the post
 - 'content': the content of the post
 
-The index template will be rendered with a posts variable, which is a list of dictionaries. Each dictionary contains the 'title', 'date', and 'file' (filename) of a post.
+The index template will be rendered with the following variables:
+
+- 'posts': a list of dictionaries. Each dictionary contains the 'title', 'date', 'tldr', and 'file' (filename) of a post.
+- 'tags': a list of all unique tags used in the posts.
+
+The tag template will be rendered with the following variables:
+
+- 'posts': a list of dictionaries. Each dictionary contains the 'title', 'date', 'tldr', and 'file' (filename) of a post with the given tag.
+- 'tag': the name of the tag.
 
 ## Writing Posts
 Posts should be written in Markdown and include YAML Front Matter. Front Matter is a block of YAML at the top of the file that is used for storing metadata about the file. Here's an example of a post:
 ```
 ---
 title: My First Post
 date: 2023-07-14
 tldr: This is a short description of my post.
+tags:
+  - tag1
+  - tag2
 ---
 # My First Post
 
 This is the content of my post. You can write anything you want here, in Markdown format.
 ```
-
-In this example, the Front Matter is the part between the '---' lines. It includes a 'title', a 'date', and a 'tldr' summary. These values will be used to populate the template when generating the HTML file.
+In this example, the Front Matter is the part between the '---' lines. It includes a 'title', a 'date', a 'tldr' summary, and a list of 'tags'. These values will be used to populate the templates when generating the HTML files.
 
 The rest of the file, after the second '---', is the content of the post. This should be written in Markdown, and it will be converted to HTML when generating the site.
 
+## Assumptions
+MDNet makes the following assumptions:
+- All Markdown files are located directly in the input_dir directory. Subdirectories are not searched.
+- All Markdown files have the '.md' extension.
+- All Markdown files include YAML Front Matter with 'title', 'date', and 'tldr' fields. The 'tags' field is optional.
+- The 'date' field in the Front Matter is in a format that can be sorted using the standard comparison operators, such as "YYYY-MM-DD".
+- The 'tags' field in the Front Matter, if present, is a list of strings.
+- The HTML templates are located at the paths specified by post_template_path, index_template_path, and tag_template_path.
+- The HTML templates use the Jinja2 syntax and include placeholders for all the variables mentioned in the "Usage" section above.
+
 ## Example
 Here's an example of how you might structure your project:
 ```
 my_blog/
     templates/
         post.html
         index.html
+        tag.html
     posts/
         post1.md
         post2.md
     output/
 ```
 You can generate the site with this command:
 ```
-mdnet posts output templates/post.html templates/index.html
+mdnet posts output templates/post.html templates/index.html templates/tag.html
 ```
 This will generate HTML files in the output directory.
```

