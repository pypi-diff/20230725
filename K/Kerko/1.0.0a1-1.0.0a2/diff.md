# Comparing `tmp/Kerko-1.0.0a1.tar.gz` & `tmp/Kerko-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kerko-1.0.0a1.tar", last modified: Thu Jun 29 21:20:35 2023, max compression
+gzip compressed data, was "Kerko-1.0.0a2.tar", last modified: Wed Jul 12 18:49:38 2023, max compression
```

## Comparing `Kerko-1.0.0a1.tar` & `Kerko-1.0.0a2.tar`

### file list

```diff
@@ -1,219 +1,221 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.673548 Kerko-1.0.0a1/
--rw-rw-r--   0 david     (1000) david     (1000)    30568 2023-06-29 21:13:54.000000 Kerko-1.0.0a1/CHANGELOG.md
--rw-rw-r--   0 david     (1000) david     (1000)    35149 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/LICENSE.txt
--rw-rw-r--   0 david     (1000) david     (1000)      215 2023-06-27 00:18:19.000000 Kerko-1.0.0a1/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)    45279 2023-06-29 21:20:35.673548 Kerko-1.0.0a1/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)    12761 2023-06-29 02:32:04.000000 Kerko-1.0.0a1/README.md
--rw-rw-r--   0 david     (1000) david     (1000)       94 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/babel.cfg
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.657548 Kerko-1.0.0a1/docs/
--rw-rw-r--   0 david     (1000) david     (1000)     3085 2023-06-28 13:58:59.000000 Kerko-1.0.0a1/docs/about.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/docs/assets/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.657548 Kerko-1.0.0a1/docs/assets/images/
--rw-rw-r--   0 david     (1000) david     (1000)   118374 2023-06-29 00:25:36.000000 Kerko-1.0.0a1/docs/assets/images/kerko-zotero-mapping.png
--rw-rw-r--   0 david     (1000) david     (1000)       22 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/docs/changelog.md
--rw-rw-r--   0 david     (1000) david     (1000)     7656 2023-06-28 22:32:39.000000 Kerko-1.0.0a1/docs/config-basics.md
--rw-rw-r--   0 david     (1000) david     (1000)    29022 2023-06-29 13:44:46.000000 Kerko-1.0.0a1/docs/config-params.md
--rw-rw-r--   0 david     (1000) david     (1000)     4040 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/docs/contributing.md
--rw-rw-r--   0 david     (1000) david     (1000)      885 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/docs/deployment.md
--rw-rw-r--   0 david     (1000) david     (1000)    14801 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/docs/getting-started.md
--rw-rw-r--   0 david     (1000) david     (1000)    18059 2023-06-29 02:31:46.000000 Kerko-1.0.0a1/docs/index.md
--rw-rw-r--   0 david     (1000) david     (1000)     3351 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/docs/localization.md
--rw-rw-r--   0 david     (1000) david     (1000)    11858 2023-06-29 13:33:33.000000 Kerko-1.0.0a1/docs/recipes.md
--rw-rw-r--   0 david     (1000) david     (1000)     5410 2023-06-28 17:36:03.000000 Kerko-1.0.0a1/docs/synchronization.md
--rw-rw-r--   0 david     (1000) david     (1000)     2646 2023-06-28 23:08:58.000000 Kerko-1.0.0a1/docs/troubleshooting.md
--rw-rw-r--   0 david     (1000) david     (1000)     2216 2023-06-29 12:28:30.000000 Kerko-1.0.0a1/mkdocs.yml
--rw-rw-r--   0 david     (1000) david     (1000)      629 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)     3407 2023-06-29 21:20:35.673548 Kerko-1.0.0a1/setup.cfg
--rwxrwxr-x   0 david     (1000) david     (1000)     1336 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.657548 Kerko-1.0.0a1/src/Kerko.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)    45279 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     9111 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       39 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)      522 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        6 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/Kerko.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.657548 Kerko-1.0.0a1/src/kerko/
--rw-rw-r--   0 david     (1000) david     (1000)      962 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     7810 2023-06-29 20:49:30.000000 Kerko-1.0.0a1/src/kerko/cli.py
--rw-rw-r--   0 david     (1000) david     (1000)     6795 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/codecs.py
--rw-rw-r--   0 david     (1000) david     (1000)    36005 2023-06-27 19:41:10.000000 Kerko-1.0.0a1/src/kerko/composer.py
--rw-rw-r--   0 david     (1000) david     (1000)    11971 2023-06-28 21:41:17.000000 Kerko-1.0.0a1/src/kerko/config_helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     7621 2023-06-27 20:14:00.000000 Kerko-1.0.0a1/src/kerko/criteria.py
--rw-rw-r--   0 david     (1000) david     (1000)     4747 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/datetime.py
--rw-rw-r--   0 david     (1000) david     (1000)    18342 2023-06-28 18:38:21.000000 Kerko-1.0.0a1/src/kerko/default_config.toml
--rw-rw-r--   0 david     (1000) david     (1000)     1294 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)    26611 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/extractors.py
--rw-rw-r--   0 david     (1000) david     (1000)      511 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/forms.py
--rw-rw-r--   0 david     (1000) david     (1000)     2123 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/jinja2.py
--rw-rw-r--   0 david     (1000) david     (1000)     1674 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/renderers.py
--rw-rw-r--   0 david     (1000) david     (1000)    12863 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/searcher.py
--rw-rw-r--   0 david     (1000) david     (1000)      836 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/shortcuts.py
--rw-rw-r--   0 david     (1000) david     (1000)    27169 2023-06-27 19:33:34.000000 Kerko-1.0.0a1/src/kerko/specs.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/static/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/static/kerko/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.657548 Kerko-1.0.0a1/src/kerko/static/kerko/css/
--rw-rw-r--   0 david     (1000) david     (1000)     2027 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/static/kerko/css/styles.css
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.661548 Kerko-1.0.0a1/src/kerko/static/kerko/js/
--rw-rw-r--   0 david     (1000) david     (1000)      404 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/static/kerko/js/item.js
--rw-rw-r--   0 david     (1000) david     (1000)     1289 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/static/kerko/js/open_in_zotero.js
--rw-rw-r--   0 david     (1000) david     (1000)     1369 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/static/kerko/js/print.js
--rw-rw-r--   0 david     (1000) david     (1000)     2259 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/static/kerko/js/search.js
--rw-rw-r--   0 david     (1000) david     (1000)     2564 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/storage.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.661548 Kerko-1.0.0a1/src/kerko/sync/
--rw-rw-r--   0 david     (1000) david     (1000)       30 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/sync/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4139 2023-06-27 18:19:44.000000 Kerko-1.0.0a1/src/kerko/sync/attachments.py
--rw-rw-r--   0 david     (1000) david     (1000)     5330 2023-06-27 18:19:02.000000 Kerko-1.0.0a1/src/kerko/sync/cache.py
--rw-rw-r--   0 david     (1000) david     (1000)     3852 2023-06-27 18:19:02.000000 Kerko-1.0.0a1/src/kerko/sync/index.py
--rw-rw-r--   0 david     (1000) david     (1000)    11723 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/sync/zotero.py
--rw-rw-r--   0 david     (1000) david     (1000)     3035 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/tags.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/templates/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/templates/kerko/
--rw-rw-r--   0 david     (1000) david     (1000)      155 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_attributes.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      632 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_badges.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1234 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_breadbox.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1623 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_collapse.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      375 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_facet_breadbox.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      560 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_facet_field.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      281 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_facet_search.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     6610 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_facets.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1464 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_item-relations.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)       95 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_navbar_brand.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      280 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_navbar_items.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     3908 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_pager.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     4013 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_preferences.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1819 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_search-form.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)    10118 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_search-help.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      578 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_search-metas.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     5479 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_search-result.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1228 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/_sorter.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     4282 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/atom.xml.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     2184 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/base.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)    20525 2023-06-27 19:54:48.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/item.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     6640 2023-06-26 23:55:07.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/layout.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)     1701 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/search-item.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)    12963 2023-06-27 20:14:43.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/search.html.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      348 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/sitemap.xml.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      325 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/templates/kerko/sitemap_index.xml.jinja2
--rw-rw-r--   0 david     (1000) david     (1000)      868 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/text.py
--rw-rw-r--   0 david     (1000) david     (1000)     2579 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/transformers.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/translations/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/translations/de/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/translations/de/LC_MESSAGES/
--rw-r--r--   0 david     (1000) david     (1000)    18452 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/kerko/translations/de/LC_MESSAGES/kerko.mo
--rw-rw-r--   0 david     (1000) david     (1000)    26381 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/translations/de/LC_MESSAGES/kerko.po
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/translations/fr/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/translations/fr/LC_MESSAGES/
--rw-r--r--   0 david     (1000) david     (1000)    22918 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/kerko/translations/fr/LC_MESSAGES/kerko.mo
--rw-rw-r--   0 david     (1000) david     (1000)    33607 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/translations/fr/LC_MESSAGES/kerko.po
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.653548 Kerko-1.0.0a1/src/kerko/translations/pt/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/translations/pt/LC_MESSAGES/
--rw-rw-r--   0 david     (1000) david     (1000)    20867 2023-06-29 21:20:35.000000 Kerko-1.0.0a1/src/kerko/translations/pt/LC_MESSAGES/kerko.mo
--rw-rw-r--   0 david     (1000) david     (1000)    30605 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/translations/pt/LC_MESSAGES/kerko.po
--rw-rw-r--   0 david     (1000) david     (1000)      868 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/tree.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/views/
--rw-rw-r--   0 david     (1000) david     (1000)       52 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2329 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/breadbox.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/src/kerko/views/item/
--rw-rw-r--   0 david     (1000) david     (1000)     1361 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/item/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1660 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/item/creators.py
--rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/item/facets.py
--rw-rw-r--   0 david     (1000) david     (1000)     4160 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/item/meta.py
--rw-rw-r--   0 david     (1000) david     (1000)     2937 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/item/relations.py
--rw-rw-r--   0 david     (1000) david     (1000)     2399 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/pager.py
--rw-rw-r--   0 david     (1000) david     (1000)    17134 2023-06-27 19:55:17.000000 Kerko-1.0.0a1/src/kerko/views/routes.py
--rw-rw-r--   0 david     (1000) david     (1000)    11265 2023-06-27 19:55:24.000000 Kerko-1.0.0a1/src/kerko/views/search.py
--rw-rw-r--   0 david     (1000) david     (1000)      690 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/src/kerko/views/sorter.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/tests/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.665548 Kerko-1.0.0a1/tests/integration_testing/
--rw-rw-r--   0 david     (1000) david     (1000)     1649 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/README.md
--rw-rw-r--   0 david     (1000) david     (1000)    10620 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-06-29 21:20:35.673548 Kerko-1.0.0a1/tests/integration_testing/api_responses/
--rw-rw-r--   0 david     (1000) david     (1000)     1071 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/collections.json
--rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/fulltext.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_artwork.json
--rw-rw-r--   0 david     (1000) david     (1000)      329 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_audioRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_bill.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_blogPost.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_book.json
--rw-rw-r--   0 david     (1000) david     (1000)      498 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_bookSection.json
--rw-rw-r--   0 david     (1000) david     (1000)      242 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_case.json
--rw-rw-r--   0 david     (1000) david     (1000)      172 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_computerProgram.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_conferencePaper.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_dictionaryEntry.json
--rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_document.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_email.json
--rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_encyclopediaArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)      336 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_film.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_forumPost.json
--rw-rw-r--   0 david     (1000) david     (1000)       88 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_hearing.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_instantMessage.json
--rw-rw-r--   0 david     (1000) david     (1000)      347 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_interview.json
--rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_journalArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_letter.json
--rw-rw-r--   0 david     (1000) david     (1000)      341 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_magazineArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_manuscript.json
--rw-rw-r--   0 david     (1000) david     (1000)      265 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_map.json
--rw-rw-r--   0 david     (1000) david     (1000)      341 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_newspaperArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_note.json
--rw-rw-r--   0 david     (1000) david     (1000)      259 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_patent.json
--rw-rw-r--   0 david     (1000) david     (1000)      244 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_podcast.json
--rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_preprint.json
--rw-rw-r--   0 david     (1000) david     (1000)      170 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_presentation.json
--rw-rw-r--   0 david     (1000) david     (1000)      495 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_radioBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)      337 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_report.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_statute.json
--rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_thesis.json
--rw-rw-r--   0 david     (1000) david     (1000)      495 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_tvBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)      421 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_videoRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeCreatorTypes_webpage.json
--rw-rw-r--   0 david     (1000) david     (1000)     1129 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_artwork.json
--rw-rw-r--   0 david     (1000) david     (1000)     1574 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)     1251 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_bill.json
--rw-rw-r--   0 david     (1000) david     (1000)      803 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_blogPost.json
--rw-rw-r--   0 david     (1000) david     (1000)     1637 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_book.json
--rw-rw-r--   0 david     (1000) david     (1000)     1706 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_bookSection.json
--rw-rw-r--   0 david     (1000) david     (1000)     1128 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_case.json
--rw-rw-r--   0 david     (1000) david     (1000)     1423 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json
--rw-rw-r--   0 david     (1000) david     (1000)     1631 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json
--rw-rw-r--   0 david     (1000) david     (1000)     1718 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json
--rw-rw-r--   0 david     (1000) david     (1000)     1047 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_document.json
--rw-rw-r--   0 david     (1000) david     (1000)      649 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_email.json
--rw-rw-r--   0 david     (1000) david     (1000)     1722 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)     1284 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_film.json
--rw-rw-r--   0 david     (1000) david     (1000)      808 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_forumPost.json
--rw-rw-r--   0 david     (1000) david     (1000)     1338 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_hearing.json
--rw-rw-r--   0 david     (1000) david     (1000)      645 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json
--rw-rw-r--   0 david     (1000) david     (1000)     1050 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_interview.json
--rw-rw-r--   0 david     (1000) david     (1000)     1711 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)     1043 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_letter.json
--rw-rw-r--   0 david     (1000) david     (1000)     1328 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)     1191 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_manuscript.json
--rw-rw-r--   0 david     (1000) david     (1000)     1471 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_map.json
--rw-rw-r--   0 david     (1000) david     (1000)     1402 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json
--rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_note.json
--rw-rw-r--   0 david     (1000) david     (1000)     1532 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_patent.json
--rw-rw-r--   0 david     (1000) david     (1000)      906 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_podcast.json
--rw-rw-r--   0 david     (1000) david     (1000)     1560 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_preprint.json
--rw-rw-r--   0 david     (1000) david     (1000)      872 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_presentation.json
--rw-rw-r--   0 david     (1000) david     (1000)     1444 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)     1430 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_report.json
--rw-rw-r--   0 david     (1000) david     (1000)     1189 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_statute.json
--rw-rw-r--   0 david     (1000) david     (1000)     1265 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_thesis.json
--rw-rw-r--   0 david     (1000) david     (1000)     1444 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json
--rw-rw-r--   0 david     (1000) david     (1000)     1576 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json
--rw-rw-r--   0 david     (1000) david     (1000)      809 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_webpage.json
--rw-rw-r--   0 david     (1000) david     (1000)     2883 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypes.json
--rw-rw-r--   0 david     (1000) david     (1000)    42561 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/items.json
--rw-rw-r--   0 david     (1000) david     (1000)       22 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/items_versions.json
--rwxrwxr-x   0 david     (1000) david     (1000)     2577 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/integration_testing/api_responses/update.bash
--rw-rw-r--   0 david     (1000) david     (1000)     8683 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_atom_feed.py
--rw-rw-r--   0 david     (1000) david     (1000)     5321 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_config.py
--rw-rw-r--   0 david     (1000) david     (1000)    13271 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_datetime.py
--rw-rw-r--   0 david     (1000) david     (1000)    16760 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_item_meta.py
--rw-rw-r--   0 david     (1000) david     (1000)     4919 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_pager.py
--rw-rw-r--   0 david     (1000) david     (1000)     2514 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_sitemap.py
--rw-rw-r--   0 david     (1000) david     (1000)     1863 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_sync.py
--rw-rw-r--   0 david     (1000) david     (1000)     8126 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tests/test_tags.py
--rw-rw-r--   0 david     (1000) david     (1000)      640 2023-06-26 22:51:54.000000 Kerko-1.0.0a1/tox.ini
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.501548 Kerko-1.0.0a2/
+-rw-rw-r--   0 david     (1000) david     (1000)    31552 2023-07-12 18:38:27.000000 Kerko-1.0.0a2/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)    35149 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/LICENSE.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      215 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)    46263 2023-07-12 18:49:38.501548 Kerko-1.0.0a2/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)    12761 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)       94 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/babel.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/docs/
+-rw-rw-r--   0 david     (1000) david     (1000)     3085 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/docs/about.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/docs/assets/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/docs/assets/images/
+-rw-rw-r--   0 david     (1000) david     (1000)   118374 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/docs/assets/images/kerko-zotero-mapping.png
+-rw-rw-r--   0 david     (1000) david     (1000)       22 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/docs/changelog.md
+-rw-rw-r--   0 david     (1000) david     (1000)     7632 2023-07-09 12:04:15.000000 Kerko-1.0.0a2/docs/config-basics.md
+-rw-rw-r--   0 david     (1000) david     (1000)    10772 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/docs/config-guides.md
+-rw-rw-r--   0 david     (1000) david     (1000)    33399 2023-07-12 17:53:19.000000 Kerko-1.0.0a2/docs/config-params.md
+-rw-rw-r--   0 david     (1000) david     (1000)     4040 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/docs/contributing.md
+-rw-rw-r--   0 david     (1000) david     (1000)    10856 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/docs/deploying.md
+-rw-rw-r--   0 david     (1000) david     (1000)    15155 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/docs/getting-started.md
+-rw-rw-r--   0 david     (1000) david     (1000)    18148 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/docs/index.md
+-rw-rw-r--   0 david     (1000) david     (1000)     3417 2023-07-08 22:47:38.000000 Kerko-1.0.0a2/docs/localization.md
+-rw-rw-r--   0 david     (1000) david     (1000)     5140 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/docs/synchronization.md
+-rw-rw-r--   0 david     (1000) david     (1000)     2450 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/docs/troubleshooting.md
+-rw-rw-r--   0 david     (1000) david     (1000)    10023 2023-07-12 17:53:19.000000 Kerko-1.0.0a2/docs/upgrading.md
+-rw-rw-r--   0 david     (1000) david     (1000)     2238 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/mkdocs.yml
+-rw-rw-r--   0 david     (1000) david     (1000)      629 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)     3407 2023-07-12 18:49:38.501548 Kerko-1.0.0a2/setup.cfg
+-rwxrwxr-x   0 david     (1000) david     (1000)     1336 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/src/Kerko.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)    46263 2023-07-12 18:49:38.000000 Kerko-1.0.0a2/src/Kerko.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     9184 2023-07-12 18:49:38.000000 Kerko-1.0.0a2/src/Kerko.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-07-12 18:49:38.000000 Kerko-1.0.0a2/src/Kerko.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       39 2023-07-12 18:49:38.000000 Kerko-1.0.0a2/src/Kerko.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      522 2023-07-12 18:49:38.000000 Kerko-1.0.0a2/src/Kerko.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        6 2023-07-12 18:49:38.000000 Kerko-1.0.0a2/src/Kerko.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.489548 Kerko-1.0.0a2/src/kerko/
+-rw-rw-r--   0 david     (1000) david     (1000)      962 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8355 2023-07-09 11:42:27.000000 Kerko-1.0.0a2/src/kerko/cli.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6795 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/codecs.py
+-rw-rw-r--   0 david     (1000) david     (1000)    36573 2023-07-12 17:53:19.000000 Kerko-1.0.0a2/src/kerko/composer.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14764 2023-07-12 17:53:19.000000 Kerko-1.0.0a2/src/kerko/config_helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7621 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/criteria.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4747 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/datetime.py
+-rw-rw-r--   0 david     (1000) david     (1000)    18704 2023-07-12 17:53:19.000000 Kerko-1.0.0a2/src/kerko/default_config.toml
+-rw-rw-r--   0 david     (1000) david     (1000)     1294 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    26611 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/extractors.py
+-rw-rw-r--   0 david     (1000) david     (1000)      511 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/forms.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2123 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/jinja2.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1674 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/renderers.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12863 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/searcher.py
+-rw-rw-r--   0 david     (1000) david     (1000)      836 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/shortcuts.py
+-rw-rw-r--   0 david     (1000) david     (1000)    29106 2023-07-12 17:53:19.000000 Kerko-1.0.0a2/src/kerko/specs.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/src/kerko/static/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/src/kerko/static/kerko/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.489548 Kerko-1.0.0a2/src/kerko/static/kerko/css/
+-rw-rw-r--   0 david     (1000) david     (1000)     2027 2023-07-08 16:19:09.000000 Kerko-1.0.0a2/src/kerko/static/kerko/css/styles.css
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.489548 Kerko-1.0.0a2/src/kerko/static/kerko/js/
+-rw-rw-r--   0 david     (1000) david     (1000)      404 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/static/kerko/js/item.js
+-rw-rw-r--   0 david     (1000) david     (1000)     1289 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/static/kerko/js/open_in_zotero.js
+-rw-rw-r--   0 david     (1000) david     (1000)     1369 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/static/kerko/js/print.js
+-rw-rw-r--   0 david     (1000) david     (1000)     2259 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/static/kerko/js/search.js
+-rw-rw-r--   0 david     (1000) david     (1000)     2564 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/storage.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.489548 Kerko-1.0.0a2/src/kerko/sync/
+-rw-rw-r--   0 david     (1000) david     (1000)       30 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/sync/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4139 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/sync/attachments.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5330 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/sync/cache.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3852 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/sync/index.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11723 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/sync/zotero.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3035 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/tags.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/src/kerko/templates/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.493548 Kerko-1.0.0a2/src/kerko/templates/kerko/
+-rw-rw-r--   0 david     (1000) david     (1000)      155 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_attributes.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      632 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_badges.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1234 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_breadbox.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1896 2023-07-12 17:53:19.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_breadcrumb.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1623 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_collapse.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      375 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_facet_breadbox.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      560 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_facet_field.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      281 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_facet_search.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     6610 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_facets.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1464 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_item-relations.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)       95 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_navbar_brand.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      299 2023-07-12 17:53:19.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_navbar_items.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     3908 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_pager.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     4013 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_preferences.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1819 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_search-form.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)    10118 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_search-help.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      578 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_search-metas.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     5479 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_search-result.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1228 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/_sorter.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     4282 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/atom.xml.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     2184 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/base.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)    20710 2023-07-12 16:18:46.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/item.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     7019 2023-07-08 18:38:17.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/layout.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)     1988 2023-07-12 17:53:19.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/search-item.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)    13208 2023-07-08 18:38:17.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/search.html.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      348 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/sitemap.xml.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      325 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/templates/kerko/sitemap_index.xml.jinja2
+-rw-rw-r--   0 david     (1000) david     (1000)      868 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/text.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2579 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/transformers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/src/kerko/translations/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/src/kerko/translations/de/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.493548 Kerko-1.0.0a2/src/kerko/translations/de/LC_MESSAGES/
+-rw-r--r--   0 david     (1000) david     (1000)    18452 2023-07-12 18:49:38.000000 Kerko-1.0.0a2/src/kerko/translations/de/LC_MESSAGES/kerko.mo
+-rw-rw-r--   0 david     (1000) david     (1000)    26381 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/translations/de/LC_MESSAGES/kerko.po
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/src/kerko/translations/fr/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.493548 Kerko-1.0.0a2/src/kerko/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 david     (1000) david     (1000)    22915 2023-07-12 18:49:38.000000 Kerko-1.0.0a2/src/kerko/translations/fr/LC_MESSAGES/kerko.mo
+-rw-rw-r--   0 david     (1000) david     (1000)    33684 2023-07-08 19:48:43.000000 Kerko-1.0.0a2/src/kerko/translations/fr/LC_MESSAGES/kerko.po
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.485548 Kerko-1.0.0a2/src/kerko/translations/pt/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.493548 Kerko-1.0.0a2/src/kerko/translations/pt/LC_MESSAGES/
+-rw-rw-r--   0 david     (1000) david     (1000)    20867 2023-07-12 18:49:38.000000 Kerko-1.0.0a2/src/kerko/translations/pt/LC_MESSAGES/kerko.mo
+-rw-rw-r--   0 david     (1000) david     (1000)    30605 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/translations/pt/LC_MESSAGES/kerko.po
+-rw-rw-r--   0 david     (1000) david     (1000)      868 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/tree.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.493548 Kerko-1.0.0a2/src/kerko/views/
+-rw-rw-r--   0 david     (1000) david     (1000)       52 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2329 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/views/breadbox.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.493548 Kerko-1.0.0a2/src/kerko/views/item/
+-rw-rw-r--   0 david     (1000) david     (1000)     1361 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/views/item/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1660 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/views/item/creators.py
+-rw-rw-r--   0 david     (1000) david     (1000)      915 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/views/item/facets.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4160 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/views/item/meta.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2937 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/views/item/relations.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2399 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/views/pager.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17134 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/views/routes.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11265 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/src/kerko/views/search.py
+-rw-rw-r--   0 david     (1000) david     (1000)      690 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/src/kerko/views/sorter.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.493548 Kerko-1.0.0a2/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.493548 Kerko-1.0.0a2/tests/integration_testing/
+-rw-rw-r--   0 david     (1000) david     (1000)     1649 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/tests/integration_testing/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)    10620 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/tests/integration_testing/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-07-12 18:49:38.501548 Kerko-1.0.0a2/tests/integration_testing/api_responses/
+-rw-rw-r--   0 david     (1000) david     (1000)     1071 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/collections.json
+-rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/fulltext.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_artwork.json
+-rw-rw-r--   0 david     (1000) david     (1000)      329 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_audioRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_bill.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_blogPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_book.json
+-rw-rw-r--   0 david     (1000) david     (1000)      498 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_bookSection.json
+-rw-rw-r--   0 david     (1000) david     (1000)      242 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_case.json
+-rw-rw-r--   0 david     (1000) david     (1000)      172 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_computerProgram.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_conferencePaper.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_dictionaryEntry.json
+-rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_document.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_email.json
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_encyclopediaArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)      336 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_film.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_forumPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)       88 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_hearing.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_instantMessage.json
+-rw-rw-r--   0 david     (1000) david     (1000)      347 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_interview.json
+-rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_journalArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)      246 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_letter.json
+-rw-rw-r--   0 david     (1000) david     (1000)      341 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_magazineArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_manuscript.json
+-rw-rw-r--   0 david     (1000) david     (1000)      265 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_map.json
+-rw-rw-r--   0 david     (1000) david     (1000)      341 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_newspaperArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_note.json
+-rw-rw-r--   0 david     (1000) david     (1000)      259 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_patent.json
+-rw-rw-r--   0 david     (1000) david     (1000)      244 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_podcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)      417 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_preprint.json
+-rw-rw-r--   0 david     (1000) david     (1000)      170 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_presentation.json
+-rw-rw-r--   0 david     (1000) david     (1000)      495 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_radioBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)      337 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_report.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_statute.json
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_thesis.json
+-rw-rw-r--   0 david     (1000) david     (1000)      495 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_tvBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)      421 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_videoRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)      248 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeCreatorTypes_webpage.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1129 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_artwork.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1574 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1251 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_bill.json
+-rw-rw-r--   0 david     (1000) david     (1000)      803 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_blogPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1637 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_book.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1706 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_bookSection.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1128 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_case.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1423 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1631 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1718 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1047 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_document.json
+-rw-rw-r--   0 david     (1000) david     (1000)      649 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_email.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1722 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1284 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_film.json
+-rw-rw-r--   0 david     (1000) david     (1000)      808 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_forumPost.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1338 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_hearing.json
+-rw-rw-r--   0 david     (1000) david     (1000)      645 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1050 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_interview.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1711 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1043 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_letter.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1328 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1191 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_manuscript.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1471 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_map.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1402 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json
+-rw-rw-r--   0 david     (1000) david     (1000)        2 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_note.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1532 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_patent.json
+-rw-rw-r--   0 david     (1000) david     (1000)      906 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_podcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1560 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_preprint.json
+-rw-rw-r--   0 david     (1000) david     (1000)      872 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_presentation.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1444 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1430 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_report.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1189 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_statute.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1265 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_thesis.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1444 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json
+-rw-rw-r--   0 david     (1000) david     (1000)     1576 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json
+-rw-rw-r--   0 david     (1000) david     (1000)      809 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_webpage.json
+-rw-rw-r--   0 david     (1000) david     (1000)     2883 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypes.json
+-rw-rw-r--   0 david     (1000) david     (1000)    42561 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/items.json
+-rw-rw-r--   0 david     (1000) david     (1000)       22 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/items_versions.json
+-rwxrwxr-x   0 david     (1000) david     (1000)     2577 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/tests/integration_testing/api_responses/update.bash
+-rw-rw-r--   0 david     (1000) david     (1000)     8683 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/tests/test_atom_feed.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5321 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/tests/test_config.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13271 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/tests/test_datetime.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16760 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/test_item_meta.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4919 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/tests/test_pager.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2514 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/test_sitemap.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1863 2023-07-04 16:15:25.000000 Kerko-1.0.0a2/tests/test_sync.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8126 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tests/test_tags.py
+-rw-rw-r--   0 david     (1000) david     (1000)      640 2023-06-26 22:51:54.000000 Kerko-1.0.0a2/tox.ini
```

### Comparing `Kerko-1.0.0a1/CHANGELOG.md` & `Kerko-1.0.0a2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,38 @@
 # Changelog
 
+## 1.0.0alpha2 (2023-07-12)
+
+Features:
+
+- Add new configuration parameters `kerko.link_groups.*.` for defining sets of
+  links that may be used for navigation.
+- Add a breadcrumb trail to all pages. One or more base links can be configured
+  (see configuration parameters `kerko.breadcrumb` and
+  `kerko_link_groups.breadcrumb_base`).
+
+Bug fixes:
+
+- Fix validation pattern too restrictive for the `kerko.zotero.csl_style`
+  configuration parameter.
+
+Backwards incompatible changes:
+
+- Items from the main navigation bar are now based on the
+  `kerko.link_groups.navbar` configuration. There is no default translation for
+  it. To change the default text or to translate it, you must override the
+  default `kerko.link_groups.navbar` in your configuration file. If you have
+  overridden the `_navbar_items.html.jinja2` template and wish to use the
+  configuration, you might want to adapt it, or revert to the default template.
+
+Other changes:
+
+- Improve documentation.
+
+
 ## 1.0.0alpha1 (2023-06-29)
 
 Features:
 
 - Add the `--full` option to the `sync` command line interface (CLI) command.
 
 Bug fixes:
@@ -61,19 +90,20 @@
 ```
 
 Features:
 
 - Add many new configuration parameters. Please refer to the configuration
   parameters documentation for the full list.
 - Add optional "Open in Zotero" and "View on zotero.org" buttons to item pages.
-  These are disabled by default (see the new settings `KERKO_OPEN_IN_ZOTERO_APP`
-  and `KERKO_OPEN_IN_ZOTERO_WEB`). Even when these settings are enabled, a user
-  who wishes to use such button must first enable it from the (also
-  new) Preferences dialog.
-- Add API for retrieving information about the last synchronization from Zotero.
+  These are disabled by default (see new parameters
+  `kerko.features.open_in_zotero_app` and `kerko.features.open_in_zotero_web`).
+  Even when these are enabled, a user who wishes to use such button must first
+  enable it from the (also new) Preferences dialog.
+- Add a web API endpoint for retrieving information about the last
+  synchronization from Zotero.
 - Add the `kerko config` command to the Flask command line interface for
   displaying all configuration parameters.
 
 Other changes:
 
 - Restructure and expand documentation into a unified documentation site for
   both Kerko and KerkoApp.
@@ -105,16 +135,14 @@
     - `KERKO_FEEDS_FIELDS` → `kerko.feeds.fields`
     - `KERKO_FEEDS_MAX_DAYS` → `kerko.feeds.max_days`
     - `KERKO_FEEDS_REJECT_ANY` → `kerko.feeds.reject_any`
     - `KERKO_FEEDS_REQUIRE_ANY` → `kerko.feeds.require_any`
     - `KERKO_FULLTEXT_SEARCH` → `kerko.search.fulltext`
     - `KERKO_HIGHWIREPRESS_TAGS` → `kerko.meta.highwirepress_tags`
     - `KERKO_JQUERY_VERSION` → `kerko.assets.jquery_version`
-    - `KERKO_OPEN_IN_ZOTERO_APP` → `kerko.features.open_in_zotero_app`
-    - `KERKO_OPEN_IN_ZOTERO_WEB` → `kerko.features.open_in_zotero_web`
     - `KERKO_PAGE_LEN` → `kerko.pagination.page_len`
     - `KERKO_PAGER_LINKS` → `kerko.pagination.pager_links`
     - `KERKO_POPPER_VERSION` → `kerko.assets.popper_version`
     - `KERKO_PRINT_CITATIONS_LINK` → `kerko.features.print_citations_link`
     - `KERKO_PRINT_CITATIONS_MAX_COUNT` → `kerko.features.print_citations_max_count`
     - `KERKO_PRINT_ITEM_LINK` → `kerko.features.print_item_link`
     - `KERKO_RELATIONS_INITIAL_LIMIT` → `kerko.features.relations_initial_limit`
@@ -140,14 +168,16 @@
     - `KERKO_ZOTERO_API_KEY` → `ZOTERO_API_KEY`
     - `KERKO_ZOTERO_BATCH_SIZE` → `kerko.zotero.batch_size`
     - `KERKO_ZOTERO_LIBRARY_ID` → `ZOTERO_LIBRARY_ID`
     - `KERKO_ZOTERO_LIBRARY_TYPE` → `ZOTERO_LIBRARY_TYPE`
     - `KERKO_ZOTERO_LOCALE` → `kerko.zotero.locale`
     - `KERKO_ZOTERO_MAX_ATTEMPTS` → `kerko.zotero.max_attempts`
     - `KERKO_ZOTERO_WAIT` → `kerko.zotero.wait`
+- The Kerko configuration should now be initialized by a call like
+  `kerko.config_helpers.config_update(app.config, kerko.DEFAULTS)`.
 - `Composer.__init__()` now only takes a configuration object as argument
   instead of a bunch of arguments. Thus, the initial values of the `Composer`
   instance now depend solely on the configuration.
 - Remove the `KERKO_USE_TRANSLATIONS` configuration variable. Kerko now relies
   on the application's default Babel domain and translation directories. Custom
   applications that wish to load Kerko's translations should now add
   `kerko.TRANSLATION_DOMAIN` and `kerko.TRANSLATION_DIRECTORIES` to their Babel
```

### Comparing `Kerko-1.0.0a1/LICENSE.txt` & `Kerko-1.0.0a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/PKG-INFO` & `Kerko-1.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kerko
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A Flask blueprint that provides a faceted search interface for bibliographies based on Zotero.
 Home-page: https://whiskyechobravo.github.io/kerko/
 Author: David Lesieur
 Author-email: kerko@whiskyechobravo.com
 Project-URL: Documentation, https://whiskyechobravo.github.io/kerko/
 Project-URL: Code, https://github.com/whiskyechobravo/kerko
 Project-URL: Changes, https://github.com/whiskyechobravo/kerko/blob/main/CHANGELOG.md
@@ -255,14 +255,43 @@
 [Zotero_demo]: https://www.zotero.org/groups/2348869/kerko_demo/items
 [Zotero_export]: https://www.zotero.org/support/dev/web_api/v3/basics#export_formats
 [Zotero_schema]: https://api.zotero.org/schema
 [Zotero_styles]: https://www.zotero.org/styles/
 
 # Changelog
 
+## 1.0.0alpha2 (2023-07-12)
+
+Features:
+
+- Add new configuration parameters `kerko.link_groups.*.` for defining sets of
+  links that may be used for navigation.
+- Add a breadcrumb trail to all pages. One or more base links can be configured
+  (see configuration parameters `kerko.breadcrumb` and
+  `kerko_link_groups.breadcrumb_base`).
+
+Bug fixes:
+
+- Fix validation pattern too restrictive for the `kerko.zotero.csl_style`
+  configuration parameter.
+
+Backwards incompatible changes:
+
+- Items from the main navigation bar are now based on the
+  `kerko.link_groups.navbar` configuration. There is no default translation for
+  it. To change the default text or to translate it, you must override the
+  default `kerko.link_groups.navbar` in your configuration file. If you have
+  overridden the `_navbar_items.html.jinja2` template and wish to use the
+  configuration, you might want to adapt it, or revert to the default template.
+
+Other changes:
+
+- Improve documentation.
+
+
 ## 1.0.0alpha1 (2023-06-29)
 
 Features:
 
 - Add the `--full` option to the `sync` command line interface (CLI) command.
 
 Bug fixes:
@@ -320,19 +349,20 @@
 ```
 
 Features:
 
 - Add many new configuration parameters. Please refer to the configuration
   parameters documentation for the full list.
 - Add optional "Open in Zotero" and "View on zotero.org" buttons to item pages.
-  These are disabled by default (see the new settings `KERKO_OPEN_IN_ZOTERO_APP`
-  and `KERKO_OPEN_IN_ZOTERO_WEB`). Even when these settings are enabled, a user
-  who wishes to use such button must first enable it from the (also
-  new) Preferences dialog.
-- Add API for retrieving information about the last synchronization from Zotero.
+  These are disabled by default (see new parameters
+  `kerko.features.open_in_zotero_app` and `kerko.features.open_in_zotero_web`).
+  Even when these are enabled, a user who wishes to use such button must first
+  enable it from the (also new) Preferences dialog.
+- Add a web API endpoint for retrieving information about the last
+  synchronization from Zotero.
 - Add the `kerko config` command to the Flask command line interface for
   displaying all configuration parameters.
 
 Other changes:
 
 - Restructure and expand documentation into a unified documentation site for
   both Kerko and KerkoApp.
@@ -364,16 +394,14 @@
     - `KERKO_FEEDS_FIELDS` → `kerko.feeds.fields`
     - `KERKO_FEEDS_MAX_DAYS` → `kerko.feeds.max_days`
     - `KERKO_FEEDS_REJECT_ANY` → `kerko.feeds.reject_any`
     - `KERKO_FEEDS_REQUIRE_ANY` → `kerko.feeds.require_any`
     - `KERKO_FULLTEXT_SEARCH` → `kerko.search.fulltext`
     - `KERKO_HIGHWIREPRESS_TAGS` → `kerko.meta.highwirepress_tags`
     - `KERKO_JQUERY_VERSION` → `kerko.assets.jquery_version`
-    - `KERKO_OPEN_IN_ZOTERO_APP` → `kerko.features.open_in_zotero_app`
-    - `KERKO_OPEN_IN_ZOTERO_WEB` → `kerko.features.open_in_zotero_web`
     - `KERKO_PAGE_LEN` → `kerko.pagination.page_len`
     - `KERKO_PAGER_LINKS` → `kerko.pagination.pager_links`
     - `KERKO_POPPER_VERSION` → `kerko.assets.popper_version`
     - `KERKO_PRINT_CITATIONS_LINK` → `kerko.features.print_citations_link`
     - `KERKO_PRINT_CITATIONS_MAX_COUNT` → `kerko.features.print_citations_max_count`
     - `KERKO_PRINT_ITEM_LINK` → `kerko.features.print_item_link`
     - `KERKO_RELATIONS_INITIAL_LIMIT` → `kerko.features.relations_initial_limit`
@@ -399,14 +427,16 @@
     - `KERKO_ZOTERO_API_KEY` → `ZOTERO_API_KEY`
     - `KERKO_ZOTERO_BATCH_SIZE` → `kerko.zotero.batch_size`
     - `KERKO_ZOTERO_LIBRARY_ID` → `ZOTERO_LIBRARY_ID`
     - `KERKO_ZOTERO_LIBRARY_TYPE` → `ZOTERO_LIBRARY_TYPE`
     - `KERKO_ZOTERO_LOCALE` → `kerko.zotero.locale`
     - `KERKO_ZOTERO_MAX_ATTEMPTS` → `kerko.zotero.max_attempts`
     - `KERKO_ZOTERO_WAIT` → `kerko.zotero.wait`
+- The Kerko configuration should now be initialized by a call like
+  `kerko.config_helpers.config_update(app.config, kerko.DEFAULTS)`.
 - `Composer.__init__()` now only takes a configuration object as argument
   instead of a bunch of arguments. Thus, the initial values of the `Composer`
   instance now depend solely on the configuration.
 - Remove the `KERKO_USE_TRANSLATIONS` configuration variable. Kerko now relies
   on the application's default Babel domain and translation directories. Custom
   applications that wish to load Kerko's translations should now add
   `kerko.TRANSLATION_DOMAIN` and `kerko.TRANSLATION_DIRECTORIES` to their Babel
```

### Comparing `Kerko-1.0.0a1/README.md` & `Kerko-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/docs/about.md` & `Kerko-1.0.0a2/docs/about.md`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/docs/assets/images/kerko-zotero-mapping.png` & `Kerko-1.0.0a2/docs/assets/images/kerko-zotero-mapping.png`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/docs/config-basics.md` & `Kerko-1.0.0a2/docs/config-basics.md`

 * *Files 2% similar despite different names*

```diff
@@ -132,27 +132,27 @@
 KerkoApp requires environment variable names to be prefixed with `KERKOAPP_`.
 The `SECRET_KEY` parameter, for example, becomes `KERKOAPP_SECRET_KEY` when
 specified as an environment variable.
 
 For hierarchical parameters, each dot separator (`.`) must be replaced by two
 underscore characters (`__`). The `kerko.meta.title` parameter, for example,
 becomes `KERKOAPP_kerko__meta__title` when specified as an environment variable.
-It is much easier to manage hierarchical parameters in TOML files.
+Such conversion is not necessary in TOML files.
 
 Note that Windows does not allow lowercase environment variable names.
 Consequently, Windows users have no choice but to set lowercase parameters in
 TOML files.
 
 Environment variables may be set from various locations, in the following order
 (refer to the [Flask documentation][Flask_dotenv] for more details):
 
-1. As entries in a file specified by the `--env-file` command line option.
 1. As entries in a `.flaskenv` file.
-1. As entries in a `.env` file.
-1. As environment variables.
+2. As entries in a `.env` file.
+3. As entries in a file specified by the `--env-file` command line option.
+4. As environment variables.
 
 The above list is in ascending order of precedence. This means that a given
 parameter set earlier can be overridden later as values get loaded. Files are
 located by scanning directories upwards from the directory you call flask from.
 
 ## Configuration in custom applications
 
@@ -170,22 +170,22 @@
 from kerko.config_helpers import config_set
 config_set(app.config, "kerko.meta.title", "My Awesome Bibliography")
 ```
 
 Such assignments must be done during the initialization process. The application
 cannot change a setting while responding to a request.
 
-## Verifying the configuration
+## Viewing the configuration
 
 With configuration parameters potentially taking values from different sources
-(default values defined by Kerko, environment variables, configuration files),
-you may sometimes want to verify the actual values taken by each parameter.
+(default values, configuration files, environment variables), you may sometimes
+want to verify the actual values taken by each parameter.
 
-The following command will show the parameters of the application and their
-values:
+The following command will show the configuration parameters of the application
+and their values:
 
 ```bash
 flask kerko config
 ```
 
 
 [Flask_dotenv]: https://flask.palletsprojects.com/en/2.3.x/cli/#environment-variables-from-dotenv
```

### Comparing `Kerko-1.0.0a1/docs/config-params.md` & `Kerko-1.0.0a2/docs/config-params.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
 !!! note
 
     Flask and Flask extensions loaded by the application may provide additional
     configuration parameters that are not described in this manual. To find
     those, please refer to the documentation of the relevant package.
 
-!!! warning "Changing configuration can be disruptive"
+!!! warning "Changing the configuration can be disruptive"
 
     Making any change to a configuration file requires that you at least restart
     the application afterwards for the change to become effective.
 
     Moreover, some parameters have an effect on the structure of the cache or
-    the search index that Kerko depends on. Changing such parameters may require
-    that you rebuild either. The documentation of each concerned parameters
-    indicates what actions are required after a change.
+    the search index that Kerko depends on. Changing this kind of parameter may
+    require that you rebuild either. Refer to the documentation of the parameter
+    to check if specific actions need to be taken after a change.
 
 !!! warning "Prefix your environment variables"
 
     KerkoApp users must prefix parameter names with `KERKOAPP_` when configuring
-    them as environment variables. However, that prefix should be used when the
-    same parameter is set in a TOML file. See [environment variables] for
-    details on setting such variables.
+    them as environment variables. However, that prefix should be omitted when
+    the same parameter is set in a TOML file. See [environment variables] for
+    details.
 
 ---
 
 ## `BABEL_DEFAULT_LOCALE`
 
 The default language of the user interface.
 
@@ -238,14 +238,64 @@
 Relative position of the format in lists. Formats with low weights (small
 numbers) rise above heavier ones (large numbers).
 
 Type: Integer
 
 ---
 
+## `kerko.breadcrumb.`
+
+A breadcrumb is a navigational aid that displays the location of the current
+page in relation to the structure of a website.
+
+If enabled, the breadcrumb works in relation with the
+[`kerko.link_groups.breadcrumb_base`](#kerkolink_groups) parameter, which
+defines the base (starting links) of the breadcrumb trail, which Kerko
+dynamically completes with one or more links based on the current location
+within Kerko.
+
+### `enabled`
+
+Enable the breadcrumb.
+
+Type: Boolean <br>
+Default value: `true`
+
+### `include_current`
+
+Include the current page at the end of the breadcrumb trail. If set to `false`,
+the breadcrumb trail will end with the parent page instead of the current page.
+
+Type: Boolean <br>
+Default value: `true`
+
+### `text_max_length`
+
+Maximum length for a breadcrumb item's text (in number of characters). If text
+is to be truncated in the middle of a word, the whole word is discarded instead.
+Truncated text is appended with an ellipsis sign ("...").
+
+If set to `0`, no truncation will be applied.
+
+Type: Integer <br>
+Default value: `50`
+
+### `text_max_length_leeway`
+
+If the length of a breadcrumb item's text only exceeds
+`kerko.breadcrumb.text_max_length` by this tolerance margin or less (in number
+of characters), the text will not be truncated.
+
+This parameter has no effect if `text_max_length` is set to `0` (no truncation).
+
+Type: Integer <br>
+Default value: `10`
+
+---
+
 ## `kerko.facets.*.`
 
 Facets to provide in the search interface, where `*` is a facet key. The facet
 key is used internally by Kerko to identify the facet.
 
 The default facets are:
 
@@ -337,14 +387,16 @@
 
 - `"collection"`: Use a Zotero collection as source.
 - `"item_type"`: Use the item type as source.
 - `"link"`: Use item URL field as source.
 - `"tag"`: Use Zotero tags as source.
 - `"year"`: Use the item year field as source.
 
+This parameter is **required** and has no default value.
+
 Type: String
 
 ### `weight`
 
 Relative position of the facet in lists. Facets with low weights (small numbers)
 rise above heavier ones (large numbers).
 
@@ -352,15 +404,15 @@
 
 ---
 
 ## `kerko.features.`
 
 ### `download_attachment_new_window`
 
-Open attachments in new windows. In other words: add the HTML `target="_blank"`
+Open attachments in new tabs. In other words: add the HTML `target="_blank"`
 attribute to attachment links.
 
 Type: Boolean <br>
 Default value: `false`
 
 ### `download_results_link`
 
@@ -537,14 +589,137 @@
 last day of the month.
 
 Type: Integer <br>
 Default value: `0` (i.e., no age limit)
 
 ---
 
+## `kerko.link_groups.*.`
+
+Link groups, where `*` is an arbitrary key used for identifying the group. Each
+group is a list which must contain at least one link defined using one or more
+of the sub-parameters described below.
+
+Link groups can be used for navigation or anywhere hyperlinks are needed.
+Templates can use the key to retrieve a desired link group.
+
+Kerko provides default `navbar` and `breadcrumb_base` link groups. In TOML
+format, these are defined as below (the double brackets indicate a list item):
+
+```toml
+[[kerko.link_groups.navbar]]
+type = "endpoint"
+endpoint = "kerko.search"
+text = "Bibliography"
+
+[[kerko.link_groups.breadcrumb_base]]
+type = "endpoint"
+endpoint = "kerko.search"
+text = "Bibliography"
+```
+
+### `anchor`
+
+Anchor to append to the endpoint's URL.
+
+This optional parameter is only allowed when the [`type`](#type_1) parameter is
+set to `"endpoint"`.
+
+Type: String
+
+### `endpoint`
+
+Name of the endpoint within the application. Use this for internal links. For
+example, the endpoint for the Kerko search page is `"kerko.search"`.
+
+This parameter is **required** when the [`type`](#type_1) parameter is set to
+`"endpoint"` and has no default value.
+
+Type: String
+
+### `external`
+
+Generate a full URL (with scheme and domain) for the endpoint instead of an
+internal URL.
+
+This parameter is only allowed when the [`type`](#type_1) parameter is set to
+`"endpoint"`.
+
+Type: Boolean <br>
+Default value: `false`
+
+### `new_window`
+
+Open the link in a new tab.
+
+Type: Boolean <br>
+Default value: `false`
+
+### `parameters`
+
+Dictionary of parameters to pass to the endpoint. Unknown keys are appended to
+the URL as query string arguments, like `?a=b&c=d`.
+
+This optional parameter is only allowed when the [`type`](#type_1) parameter is
+set to `"endpoint"`.
+
+Type: Dictionary
+
+### `scheme`
+
+Protocol to use in the endpoint's URL.
+
+This parameter is only allowed when the [`type`](#type_1) parameter is set to
+`"endpoint"` and the [`external`](#external) parameter is set to `true`.
+
+Type: String <br>
+Default value: Same protocol as the current request
+
+### `text`
+
+Text to use for the link.
+
+This parameter is **required** and has no default value.
+
+Type: String
+
+### `type`
+
+Type of link. Other parameters may or may not be available depending on this
+value.
+
+Allowed values are:
+
+- `"endpoint"`: Define an internal link (served by a Flask endpoint).
+- `"url"`: Define a link to an arbitrary URL.
+
+This parameter is **required** and has no default value.
+
+Type: String
+
+### `url`
+
+URL of the external link.
+
+This parameter is **required** when the [`type`](#type_1) parameter is set to
+`"url"`.
+
+Type: String
+
+### `weight`
+
+Relative position of the link in lists. Links with low weights (small numbers)
+rise above heavier ones (large numbers). At equal weights, links are ordered
+based on their order of appearance in the configuration.
+
+Type: Integer <br>
+Default value: `0`
+
+---
+
 ## `kerko.meta.`
 
 ### `google_analytics_id`
 
 A Google Analytics stream ID, e.g., `'G-??????????'`.
 
 If the value is not empty *and* Flask is not running in debug mode, then the
@@ -1074,14 +1249,14 @@
 Number of values to trust for `X-Forwarded-Prefix`.
 
 Type: Integer <br>
 Default value: `0`
 
 
 [environment variables]: config-basics.md#environment-variables
-[Ensuring full-text indexing of your attachments in Zotero]: recipes.md#ensuring-full-text-indexing-of-your-attachments-in-zotero
+[Ensuring full-text indexing of your attachments in Zotero]: config-guides.md#ensuring-full-text-indexing-of-your-attachments-in-zotero
 [Flask instance folder]: https://flask.palletsprojects.com/en/2.3.x/config/#instance-folders
 [Flask proxy]: https://flask.palletsprojects.com/en/2.3.x/deploying/proxy_fix/
 [KerkoApp]: https://github.com/whiskyechobravo/kerkoapp
 [pytz]: https://pypi.org/project/pytz/
 [synchronization commands]: synchronization.md#command-line-interface-cli
 [Zotero Styles Repository]: https://www.zotero.org/styles/
```

### Comparing `Kerko-1.0.0a1/docs/contributing.md` & `Kerko-1.0.0a2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/docs/getting-started.md` & `Kerko-1.0.0a2/docs/getting-started.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,32 @@
 
 
 ### Standard installation
 
 This procedure requires that you have [Python], [pip], and [Git] installed on
 your computer.
 
-1. The first step is to install the software. Use the following commands:
+1. The first step is to install the desired version of KerkoApp. You may check
+   the list of [available versions][KerkoApp versions], but make sure to choose
+   one that matches the documentation version you are currently reading! For
+   version 1.0.0, for example, replace `VERSION` with `1.0.0` in the commands
+   below:
 
     === "POSIX"
         ```bash
-        git clone https://github.com/whiskyechobravo/kerkoapp.git
+        git clone --branch VERSION https://github.com/whiskyechobravo/kerkoapp.git
         cd kerkoapp
         python -m venv venv
         source venv/bin/activate
         pip install -r requirements/run.txt
         ```
 
     === "Windows"
         ```
-        git clone https://github.com/whiskyechobravo/kerkoapp.git
+        git clone --branch VERSION https://github.com/whiskyechobravo/kerkoapp.git
         cd kerkoapp
         python -m venv venv
         venv\Scripts\activate.bat
         pip install -r requirements\run.txt
         ```
 
     This will install all packages required by Kerko and KerkoApp within a
@@ -388,11 +392,12 @@
 [Docker]: https://www.docker.com/
 [Flask_production]: https://flask.palletsprojects.com/en/latest/deploying/
 [Flask-Babel_documentation]: https://python-babel.github.io/flask-babel/
 [Flask]: https://pypi.org/project/Flask/
 [Git]: https://git-scm.com/
 [Kerko]: https://github.com/whiskyechobravo/kerko
 [KerkoApp]: https://github.com/whiskyechobravo/kerkoapp
+[KerkoApp versions]: https://github.com/whiskyechobravo/kerkoapp/tags
 [KerkoStart]: https://github.com/whiskyechobravo/kerkostart
 [pip]: https://pip.pypa.io/
 [Python]: https://www.python.org/
 [venv]: https://docs.python.org/3.11/tutorial/venv.html
```

### Comparing `Kerko-1.0.0a1/docs/index.md` & `Kerko-1.0.0a2/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -115,16 +115,16 @@
         used for that purpose.
     - Full-text search: the text content of PDF attachments can be searched.
     - Scope of search: users may choose to search everywhere, in
         author/contributor names, in titles, in all fields (i.e., in metadata and
         notes), or in documents (i.e., in the text content of attachments).
         Applications may provide additional choices.
 - **Faceted browsing**: allows filtering by topic (Zotero tag), by resource type
-  (Zotero item type), by publication year. Moreover, you may define additional
-  facets modeled on collections and subcollections; in such case, any collection
+  (Zotero item type), by publication year. Moreover, you may define [additional
+  facets](config-guides.md#defining-custom-facets-based-on-zotero-collections) modeled on collections and subcollections; in such case, any collection
   can be represented as a facet, and each subcollection as a value within that
   facet. By taking advantage of Zotero's ability to assign any given item to
   multiple collections, a faceted classification scheme can be designed,
   including hierarchical subdivisions within facets.
 - **Relevance scoring**: provided by the [Whoosh] library and based on the
   [BM25F] algorithm, which determines how important a term is to a document in
   the context of the whole collection of documents, while taking into account
@@ -192,15 +192,15 @@
 - **DOI, ISBN and ISSN resolver**: items that have such identifier in your
   library can be referenced by appending their identifier to your Kerko site's
   base URL.
 - **Relations**: bibliographic record pages show links to related items, if any.
   You may define such relations using Zotero's _Related_ field. Moreover, Kerko
   adds the _Cites_ and _Cited by_ relation types, which can be managed in Zotero
   through notes (see [
-  guide](recipes.md#providing-cites-and-cited-by-relations)). Custom
+  guide](config-guides.md#providing-cites-and-cited-by-relations)). Custom
   applications can add more types of relations if desired.
 - **Badges**: custom applications can have icons conditionally displayed next to
   items.
 - **Responsive design**: the simple default implementation works on large
   monitors as well as on small screens. It is based on [Bootstrap].
 - **Google Analytics integration**: just provide a Google Analytics stream ID to
   have Kerko automatically include the tracking code into its pages.
@@ -235,15 +235,15 @@
 - [Babel]: utilities for internationalization and localization.
 - [Bootstrap-Flask]: helper for integrating [Bootstrap].
 - [Click]: command line interface creation kit.
 - [Flask]: web application framework.
 - [Flask-Babel]: integration of Flask and Babel.
 - [Flask-WTF]: integration of Flask and WTForms.
 - [Jinja2]: template engine.
-- [Pydantic]: configuration validation.
+- [Pydantic]: configuration parsing and validation.
 - [Pyzotero]: Python client for the Zotero API.
 - [w3lib]: URL and HTML manipulation utilities.
 - [Werkzeug]: WSGI web application library (also required by Flask).
 - [Whoosh]: pure Python full-text indexing and searching library.
 - [WTForms]: web forms validation and rendering library.
 
 The following front-end resources are loaded from CDNs by Kerko's default
```

### Comparing `Kerko-1.0.0a1/docs/localization.md` & `Kerko-1.0.0a2/docs/localization.md`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 
 ## Translating KerkoApp
 
 Although most user interface messages come from Kerko, KerkoApp also has
 messages of its own, and thus its own separate translation file.
 
-KerkoApp translations are managed with [Babel](http://babel.pocoo.org).
+KerkoApp translations are managed with [Babel].
 
 The following commands should be executed from the directory that contains
 `babel.cfg`, and the [virtual environment][venv] must have been activated
 beforehand.
 
 Create or update the PO file template (POT). Replace `CURRENT_VERSION` with your
 current KerkoApp version:
@@ -91,7 +91,11 @@
 ```
 
 Compile MO files:
 
 ```bash
 pybabel compile -l YOUR_LOCALE -d kerkoapp/translations
 ```
+
+
+[Babel]: http://babel.pocoo.org
+[venv]: https://docs.python.org/3.11/tutorial/venv.html
```

### Comparing `Kerko-1.0.0a1/docs/recipes.md` & `Kerko-1.0.0a2/docs/config-guides.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-# Recipes
+# Configuration guides
 
-## Defining a custom facet based on a Zotero collection
+This sections provides guidance on configuring specific aspects of Kerko.
+
+## Defining custom facets based on Zotero collections
 
 Zotero collections can be mapped to custom facets in Kerko. With this scheme, a
 collection in the Zotero library represents a facet, and its subcollections
 correspond to values (or user-selectable filters) within the facet. Figure 1
 below illustrates such mapping, taken from the [demo library] and its
 corresponding [demo site].
 
@@ -210,40 +212,12 @@
   In the meantime, using child notes is how Kerko handles it. If relation types
   are important to you, consider describing your use case in the [Zotero
   forums](https://forums.zotero.org/discussion/1317/semantic-relations/).
 - Custom Kerko applications can provide more types of relations, if desired, in
   addition to _Cites_ and _Cited by_.
 
 
-## Submitting your sitemap to search engines
-
-Kerko generates an [XML Sitemap][XML_Sitemap] that can help search engines
-discover your bibliographic records.
-
-The path of the sitemap is `BASE_URL/sitemap.xml`, where `BASE_URL` should be
-replaced with the protocol, domain, port, and Kerko URL path prefix that are
-relevant to your installation, e.g.,
-`https://example.com/bibliography/sitemap.xml`.
-
-Different search engines may have different procedures for submitting sitemaps
-([Google](https://developers.google.com/search/docs/advanced/sitemaps/build-sitemap#addsitemap),
-[Bing](https://www.bing.com/webmasters/help/Sitemaps-3b5cf6ed),
-[Yandex](https://yandex.com/support/webmaster/indexing-options/sitemap.html)).
-
-However, a standard method consists in adding a `Sitemap` directive to a
-`robots.txt` file served at the root of your site, to tell web crawlers where to
-find your sitemap. For example, one might add the following line to
-`robots.txt`:
-
-```
-Sitemap: https://example.com/bibliography/sitemap.xml
-```
-
-A `robots.txt` file can have multiple `Sitemap` directives, thus the Kerko
-sitemap can be specified alongside any other sitemaps you might already have.
-
-
 [Kerko]: https://github.com/whiskyechobravo/kerko
 [demo library]: https://www.zotero.org/groups/2348869/kerko_demo/items
 [demo site]: https://demo.kerko.whiskyechobravo.com
 [venv]: https://docs.python.org/3.11/tutorial/venv.html
-[XML_Sitemap]: https://www.sitemaps.org/
+[Zutilo]: https://github.com/wshanks/Zutilo
```

### Comparing `Kerko-1.0.0a1/docs/synchronization.md` & `Kerko-1.0.0a2/docs/synchronization.md`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 
 ## Command line interface (CLI)
 
 Kerko provides an integration with the [Flask command line interface][Flask_CLI].
 The `flask` command will work with your virtual environment active.
 
+Before running a command, go to the application's directory (where the `wsgi.py`
+file is found). That is the easiest way to help Flask discover the application.
+
 Some frequently used commands are:
 
 `flask kerko --help`
 
 : Lists all commands provided by Kerko.
 
 `flask kerko sync`
@@ -66,25 +69,14 @@
 
 : Shows help specifically about the `sync` command:
 
 `flask kerko sync index`
 
 : Synchronizes just the search index (from the cache).
 
-!!! tip "Tip: Running commands from outside the application's directory"
-
-    The above commands should work as-is when you are in the application's
-    directory (where the `wsgi.py` file is found). To run them from another
-    directory, you could use Flask's `--app` command line option, or to set the
-    `FLASK_APP` environment variable. For example:
-
-    ```bash
-    flask --app=/path/to/kerkoapp/wsgi:app kerko sync
-    ```
-
 `flask kerko sync cache --full`
 
 : When possible, the synchronization process performs an incremental update of
   just the new or changed items. Here, the `--full` option forces a full
   synchronization of the cache, even if no or just some items have been updated
   since the last synchronization of the cache.
```

### Comparing `Kerko-1.0.0a1/mkdocs.yml` & `Kerko-1.0.0a2/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 nav:
   - Introduction: index.md
   - getting-started.md
   - synchronization.md
   - config-basics.md
   - config-params.md
-  - localization.md
-  - deployment.md
-  - recipes.md
+  - config-guides.md
   - troubleshooting.md
+  - localization.md
+  - deploying.md
+  - upgrading.md
+  - changelog.md
   - contributing.md
   - about.md
-  - changelog.md
 
 theme:
   name: material
   features:
     - navigation.instant
     - navigation.tracking
     - navigation.sections
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 site_name: Kerko nav: - Introduction: index.md - getting-started.md -
-synchronization.md - config-basics.md - config-params.md - localization.md -
-deployment.md - recipes.md - troubleshooting.md - contributing.md - about.md -
-changelog.md theme: name: material features: - navigation.instant -
-navigation.tracking - navigation.sections - navigation.expand - navigation.top
-- navigation.footer - header.autohide - toc.follow - search.suggest -
-search.highlight - content.code.copy - content.action.view -
-content.action.edit palette: - scheme: default toggle: icon: material/
-brightness-7 name: Switch to dark mode - scheme: slate toggle: icon: material/
-brightness-4 name: Switch to light mode icon: repo: fontawesome/brands/github
-view: material/file-eye-outline edit: material/file-edit-outline plugins: -
-search repo_url: https://github.com/whiskyechobravo/kerko repo_name:
+synchronization.md - config-basics.md - config-params.md - config-guides.md -
+troubleshooting.md - localization.md - deploying.md - upgrading.md -
+changelog.md - contributing.md - about.md theme: name: material features: -
+navigation.instant - navigation.tracking - navigation.sections -
+navigation.expand - navigation.top - navigation.footer - header.autohide -
+toc.follow - search.suggest - search.highlight - content.code.copy -
+content.action.view - content.action.edit palette: - scheme: default toggle:
+icon: material/brightness-7 name: Switch to dark mode - scheme: slate toggle:
+icon: material/brightness-4 name: Switch to light mode icon: repo: fontawesome/
+brands/github view: material/file-eye-outline edit: material/file-edit-outline
+plugins: - search repo_url: https://github.com/whiskyechobravo/kerko repo_name:
 whiskyechobravo/kerko edit_uri: blob/main/docs/ markdown_extensions: # See
 https://squidfunk.github.io/mkdocs-material/setup/extensions/ # Python Markdown
 - abbr - admonition - attr_list - def_list - footnotes - md_in_html - tables -
 toc: permalink: true # Python Markdown Extensions - pymdownx.arithmatex:
 generic: true - pymdownx.betterem: smart_enable: all - pymdownx.caret -
 pymdownx.details - pymdownx.emoji: emoji_index: !!python/name:
 materialx.emoji.twemoji emoji_generator: !!python/name:materialx.emoji.to_svg -
```

### Comparing `Kerko-1.0.0a1/pyproject.toml` & `Kerko-1.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/setup.cfg` & `Kerko-1.0.0a2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Kerko
-version = 1.0.0alpha1
+version = 1.0.0alpha2
 author = David Lesieur
 author_email = kerko@whiskyechobravo.com
 license_files = LICENSE.txt
 url = https://whiskyechobravo.github.io/kerko/
 project_urls = 
 	Documentation = https://whiskyechobravo.github.io/kerko/
 	Code = https://github.com/whiskyechobravo/kerko
```

### Comparing `Kerko-1.0.0a1/setup.py` & `Kerko-1.0.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/Kerko.egg-info/PKG-INFO` & `Kerko-1.0.0a2/src/Kerko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kerko
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: A Flask blueprint that provides a faceted search interface for bibliographies based on Zotero.
 Home-page: https://whiskyechobravo.github.io/kerko/
 Author: David Lesieur
 Author-email: kerko@whiskyechobravo.com
 Project-URL: Documentation, https://whiskyechobravo.github.io/kerko/
 Project-URL: Code, https://github.com/whiskyechobravo/kerko
 Project-URL: Changes, https://github.com/whiskyechobravo/kerko/blob/main/CHANGELOG.md
@@ -255,14 +255,43 @@
 [Zotero_demo]: https://www.zotero.org/groups/2348869/kerko_demo/items
 [Zotero_export]: https://www.zotero.org/support/dev/web_api/v3/basics#export_formats
 [Zotero_schema]: https://api.zotero.org/schema
 [Zotero_styles]: https://www.zotero.org/styles/
 
 # Changelog
 
+## 1.0.0alpha2 (2023-07-12)
+
+Features:
+
+- Add new configuration parameters `kerko.link_groups.*.` for defining sets of
+  links that may be used for navigation.
+- Add a breadcrumb trail to all pages. One or more base links can be configured
+  (see configuration parameters `kerko.breadcrumb` and
+  `kerko_link_groups.breadcrumb_base`).
+
+Bug fixes:
+
+- Fix validation pattern too restrictive for the `kerko.zotero.csl_style`
+  configuration parameter.
+
+Backwards incompatible changes:
+
+- Items from the main navigation bar are now based on the
+  `kerko.link_groups.navbar` configuration. There is no default translation for
+  it. To change the default text or to translate it, you must override the
+  default `kerko.link_groups.navbar` in your configuration file. If you have
+  overridden the `_navbar_items.html.jinja2` template and wish to use the
+  configuration, you might want to adapt it, or revert to the default template.
+
+Other changes:
+
+- Improve documentation.
+
+
 ## 1.0.0alpha1 (2023-06-29)
 
 Features:
 
 - Add the `--full` option to the `sync` command line interface (CLI) command.
 
 Bug fixes:
@@ -320,19 +349,20 @@
 ```
 
 Features:
 
 - Add many new configuration parameters. Please refer to the configuration
   parameters documentation for the full list.
 - Add optional "Open in Zotero" and "View on zotero.org" buttons to item pages.
-  These are disabled by default (see the new settings `KERKO_OPEN_IN_ZOTERO_APP`
-  and `KERKO_OPEN_IN_ZOTERO_WEB`). Even when these settings are enabled, a user
-  who wishes to use such button must first enable it from the (also
-  new) Preferences dialog.
-- Add API for retrieving information about the last synchronization from Zotero.
+  These are disabled by default (see new parameters
+  `kerko.features.open_in_zotero_app` and `kerko.features.open_in_zotero_web`).
+  Even when these are enabled, a user who wishes to use such button must first
+  enable it from the (also new) Preferences dialog.
+- Add a web API endpoint for retrieving information about the last
+  synchronization from Zotero.
 - Add the `kerko config` command to the Flask command line interface for
   displaying all configuration parameters.
 
 Other changes:
 
 - Restructure and expand documentation into a unified documentation site for
   both Kerko and KerkoApp.
@@ -364,16 +394,14 @@
     - `KERKO_FEEDS_FIELDS` → `kerko.feeds.fields`
     - `KERKO_FEEDS_MAX_DAYS` → `kerko.feeds.max_days`
     - `KERKO_FEEDS_REJECT_ANY` → `kerko.feeds.reject_any`
     - `KERKO_FEEDS_REQUIRE_ANY` → `kerko.feeds.require_any`
     - `KERKO_FULLTEXT_SEARCH` → `kerko.search.fulltext`
     - `KERKO_HIGHWIREPRESS_TAGS` → `kerko.meta.highwirepress_tags`
     - `KERKO_JQUERY_VERSION` → `kerko.assets.jquery_version`
-    - `KERKO_OPEN_IN_ZOTERO_APP` → `kerko.features.open_in_zotero_app`
-    - `KERKO_OPEN_IN_ZOTERO_WEB` → `kerko.features.open_in_zotero_web`
     - `KERKO_PAGE_LEN` → `kerko.pagination.page_len`
     - `KERKO_PAGER_LINKS` → `kerko.pagination.pager_links`
     - `KERKO_POPPER_VERSION` → `kerko.assets.popper_version`
     - `KERKO_PRINT_CITATIONS_LINK` → `kerko.features.print_citations_link`
     - `KERKO_PRINT_CITATIONS_MAX_COUNT` → `kerko.features.print_citations_max_count`
     - `KERKO_PRINT_ITEM_LINK` → `kerko.features.print_item_link`
     - `KERKO_RELATIONS_INITIAL_LIMIT` → `kerko.features.relations_initial_limit`
@@ -399,14 +427,16 @@
     - `KERKO_ZOTERO_API_KEY` → `ZOTERO_API_KEY`
     - `KERKO_ZOTERO_BATCH_SIZE` → `kerko.zotero.batch_size`
     - `KERKO_ZOTERO_LIBRARY_ID` → `ZOTERO_LIBRARY_ID`
     - `KERKO_ZOTERO_LIBRARY_TYPE` → `ZOTERO_LIBRARY_TYPE`
     - `KERKO_ZOTERO_LOCALE` → `kerko.zotero.locale`
     - `KERKO_ZOTERO_MAX_ATTEMPTS` → `kerko.zotero.max_attempts`
     - `KERKO_ZOTERO_WAIT` → `kerko.zotero.wait`
+- The Kerko configuration should now be initialized by a call like
+  `kerko.config_helpers.config_update(app.config, kerko.DEFAULTS)`.
 - `Composer.__init__()` now only takes a configuration object as argument
   instead of a bunch of arguments. Thus, the initial values of the `Composer`
   instance now depend solely on the configuration.
 - Remove the `KERKO_USE_TRANSLATIONS` configuration variable. Kerko now relies
   on the application's default Babel domain and translation directories. Custom
   applications that wish to load Kerko's translations should now add
   `kerko.TRANSLATION_DOMAIN` and `kerko.TRANSLATION_DIRECTORIES` to their Babel
```

### Comparing `Kerko-1.0.0a1/src/Kerko.egg-info/SOURCES.txt` & `Kerko-1.0.0a2/src/Kerko.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 docs/about.md
 docs/changelog.md
 docs/config-basics.md
+docs/config-guides.md
 docs/config-params.md
 docs/contributing.md
-docs/deployment.md
+docs/deploying.md
 docs/getting-started.md
 docs/index.md
 docs/localization.md
-docs/recipes.md
 docs/synchronization.md
 docs/troubleshooting.md
+docs/upgrading.md
 docs/assets/images/kerko-zotero-mapping.png
 src/Kerko.egg-info/PKG-INFO
 src/Kerko.egg-info/SOURCES.txt
 src/Kerko.egg-info/dependency_links.txt
 src/Kerko.egg-info/entry_points.txt
 src/Kerko.egg-info/requires.txt
 src/Kerko.egg-info/top_level.txt
@@ -57,14 +58,15 @@
 src/kerko/sync/attachments.py
 src/kerko/sync/cache.py
 src/kerko/sync/index.py
 src/kerko/sync/zotero.py
 src/kerko/templates/kerko/_attributes.html.jinja2
 src/kerko/templates/kerko/_badges.html.jinja2
 src/kerko/templates/kerko/_breadbox.html.jinja2
+src/kerko/templates/kerko/_breadcrumb.html.jinja2
 src/kerko/templates/kerko/_collapse.html.jinja2
 src/kerko/templates/kerko/_facet_breadbox.html.jinja2
 src/kerko/templates/kerko/_facet_field.html.jinja2
 src/kerko/templates/kerko/_facet_search.html.jinja2
 src/kerko/templates/kerko/_facets.html.jinja2
 src/kerko/templates/kerko/_item-relations.html.jinja2
 src/kerko/templates/kerko/_navbar_brand.html.jinja2
```

### Comparing `Kerko-1.0.0a1/src/Kerko.egg-info/requires.txt` & `Kerko-1.0.0a2/src/Kerko.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/__init__.py` & `Kerko-1.0.0a2/src/kerko/__init__.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/cli.py` & `Kerko-1.0.0a2/src/kerko/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pprint
 from datetime import datetime
+from typing import Any
 
 import click
 import tomli_w
 import wrapt
 from flask import current_app
 from flask.cli import with_appcontext
 
@@ -129,31 +130,50 @@
     help="Secrets are hidden from the output by default. This option causes them to be revealed."
 )
 @with_appcontext
 def config(show_secrets=False):
     """
     Show the configuration.
 
-    Note that unset parameters and parameters that internally have 'None' values
-    will be omitted because such values cannot be represented in TOML files.
+    Note that parameters that internally have 'None' values will be omitted
+    because such values cannot be represented in TOML files.
     """
-    def copy_serializable(src: dict) -> dict:
-        dst = {}
-        for k, v in sorted(src.items()):
-            if isinstance(v, dict):
-                dst_v = copy_serializable(v)
-                if dst_v is not None:
-                    dst[k] = dst_v
-            elif is_toml_serializable(v):
-                if not show_secrets and k in ['SECRET_KEY', 'ZOTERO_API_KEY']:
-                    v = "*****"
-                dst[k] = v
-        return dst
+
+    def hide_secrets(d: dict):
+        for k in d.keys():
+            if k in ['SECRET_KEY', 'ZOTERO_API_KEY'] or k.find('PASSWORD') >= 0:
+                d[k] = "*****"
+
+    def copy_serializable(obj: Any) -> Any:
+        """
+        Copy the object, with some twists.
+
+        - Filter values that cannot be serialized as TOML.
+        - Sort dicts by key.
+        """
+        if isinstance(obj, dict):
+            new_dict = {}
+            for k, v in sorted(obj.items()):
+                new_v = copy_serializable(v)
+                if new_v is not None:
+                    new_dict[k] = new_v
+            return new_dict
+        elif isinstance(obj, list):
+            new_list = []
+            for v in obj:
+                new_v = copy_serializable(v)
+                if new_v is not None:
+                    new_list.append(new_v)
+            return new_list
+        elif is_toml_serializable(obj):
+            return obj
 
     serializable_config = copy_serializable(current_app.config)
+    if not show_secrets:
+        hide_secrets(serializable_config)
     click.echo(tomli_w.dumps(serializable_config))
 
 
 @cli.command()
 @click.argument('item_key')
 @with_appcontext
 def zotero_item(item_key):
```

### Comparing `Kerko-1.0.0a1/src/kerko/codecs.py` & `Kerko-1.0.0a2/src/kerko/codecs.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/composer.py` & `Kerko-1.0.0a2/src/kerko/composer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from whoosh.support.charset import accent_map
 from whoosh.util.text import rcompile
 
 from kerko import codecs, extractors, transformers
 from kerko.config_helpers import config_get
 from kerko.datetime import iso_to_datetime, iso_to_timestamp
 from kerko.specs import (BadgeSpec, BibFormatSpec, CollectionFacetSpec,
-                         FacetSpec, FieldSpec, FlatFacetSpec, RelationSpec,
-                         ScopeSpec, SortSpec, TreeFacetSpec)
+                         FacetSpec, FieldSpec, FlatFacetSpec, LinkGroupSpec,
+                         RelationSpec, ScopeSpec, SortSpec, TreeFacetSpec)
 
 
 class Composer:
     """
     A factory for the setting up the search elements.
 
     This class acts as a registry of search elements such as fields and facets,
@@ -68,20 +68,22 @@
         self.scopes: Dict[str, ScopeSpec] = {}
         self.fields: Dict[str, FieldSpec] = {}
         self.facets: Dict[str, FacetSpec] = {}
         self.sorts: Dict[str, SortSpec] = {}
         self.bib_formats: Dict[str, BibFormatSpec] = {}
         self.relations: Dict[str, RelationSpec] = {}
         self.badges: Dict[str, BadgeSpec] = {}
+        self.link_groups: Dict[str, LinkGroupSpec] = {}
         self.init_scopes(config)
         self.init_fields(config)
         self.init_facets(config)
         self.init_sorts(config)
         self.init_bib_formats(config)
         self.init_relations(config)
+        self.init_link_groups(config)
 
     def init_scopes(self, config: Config) -> None:
         """
         Initialize a set of `ScopeSpec` instances using config settings.
         """
         # Note: Default labels are defined here rather than in config so that they are translatable.
         selector_label = {
@@ -431,16 +433,16 @@
             )
         )
 
         #
         # Optional searchable fields from Zotero items (configurable).
         #
 
-        # Our field names are prefixed with 'z_' to prevent clashes should
-        # Zotero's schema change.
+        # Those field names are prefixed with 'z_' in the search schema to
+        # prevent clashes with other fields should Zotero's schema change.
         zotero_fields_dict = config_get(config, 'kerko.search_fields.zotero')
         for field_key, field_config in zotero_fields_dict.items():
             if field_config['enabled']:
                 analyzer = field_config['analyzer']
                 if analyzer == 'id':
                     # Identifier fields are indexed as-is.
                     self.add_field(
@@ -545,14 +547,15 @@
         )
 
     def init_facets(self, config: Config) -> None:
         """
         Initialize a set of `FacetSpec` instances using config settings.
         """
         # Note: Default titles are defined here rather than in config so that they are translatable.
+        # TODO: Refactor facet using factory methods in the models, as in init_link_groups().
         facets_dict = config_get(config, 'kerko.facets')
         for facet_key, facet_config in facets_dict.items():
             if facet_config['enabled']:
                 facet_type = facet_config['type']
                 kwargs = {
                     k: v
                     for k, v in facet_config.items() if k not in ['enabled', 'title', 'type']
@@ -806,14 +809,17 @@
                             label=rel_config.get('label') or _("Related"),
                             weight=rel_config['weight'],
                             id_fields=[self.fields['id']],
                             directed=False,
                         )
                     )
 
+    def init_link_groups(self, config: Config) -> None:
+        self.link_groups = config['kerko_config'].kerko.link_groups.to_spec()
+
     def add_scope(self, scope):
         self.scopes[scope.key] = scope
 
     def remove_scope(self, key):
         del self.scopes[key]
 
     def add_field(self, field):
@@ -864,14 +870,20 @@
 
     def add_relation(self, relation):
         self.relations[relation.key] = relation
 
     def remove_relation(self, key):
         del self.relations[key]
 
+    def add_link_group(self, key: str, link_group: LinkGroupSpec):
+        self.link_groups[key] = link_group
+
+    def remove_link_group(self, key: str):
+        del self.link_groups[key]
+
     def get_ordered_specs(self, attr):
         """
         Return a list of specifications, sorted by weight.
 
         :param str attr: Attribute name of the specifications dict. The
             specifications must themselves have a `weight` attribute.
         """
```

### Comparing `Kerko-1.0.0a1/src/kerko/config_helpers.py` & `Kerko-1.0.0a2/src/kerko/config_helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import abc
 import pathlib
+from abc import ABC, abstractmethod
 from datetime import date, datetime, time
 from decimal import Decimal
 from typing import Any, Dict, List, Optional, Type, Union
 
 from typing_extensions import Annotated, Literal
 
 try:
@@ -12,15 +12,18 @@
     import tomli as tomllib  # type: ignore
 
 import dpath
 import whoosh
 from flask import Config
 from pydantic import (BaseModel,  # pylint: disable=no-name-in-module
                       ConstrainedStr, Extra, Field, NonNegativeInt,
-                      ValidationError, validator)
+                      ValidationError, root_validator, validator)
+
+from kerko.specs import (LinkByEndpointSpec, LinkByURLSpec, LinkGroupSpec,
+                         LinkSpec)
 
 # pylint: disable=too-few-public-methods
 
 # Note: To preserve field ordering in Pydantic models, we annotate an
 # attribute's type even when it could be determined by its default value.
 # See https://docs.pydantic.dev/latest/usage/models/#field-ordering
 
@@ -108,14 +111,26 @@
     class Config:
         extra = Extra.forbid
 
     page_len: int = Field(ge=2)
     pager_links: int = Field(ge=2)
 
 
+class BreadcrumbModel(BaseModel):
+    """Model for the kerko.breadcrumb config table."""
+
+    class Config:
+        extra = Extra.forbid
+
+    enabled: bool
+    include_current: bool
+    text_max_length: NonNegativeInt
+    text_max_length_leeway: NonNegativeInt
+
+
 class TemplatesModel(BaseModel):
     """Model for the kerko.templates config table."""
 
     class Config:
         extra = Extra.forbid
 
     base: str
@@ -131,15 +146,15 @@
 
     class Config:
         extra = Extra.forbid
 
     batch_size: int = Field(ge=20)
     max_attempts: int = Field(ge=1)
     wait: int = Field(ge=120)
-    csl_style: SlugStr
+    csl_style: str
     locale: str = Field(regex=r'^[a-z]{2}-[A-Z]{2}$')
     item_include_re: str
     item_exclude_re: str
     tag_include_re: str
     tag_exclude_re: str
     child_include_re: str
     child_exclude_re: str
@@ -224,15 +239,15 @@
     class Config:
         extra = Extra.forbid
 
     core: CoreSearchFieldsModel
     zotero: Dict[FieldNameStr, ZoteroFieldModel]
 
 
-class BaseFacetModel(BaseModel, abc.ABC):
+class BaseFacetModel(BaseModel, ABC):
     """Base model for the kerko.facets config table."""
 
     class Config:
         extra = Extra.forbid
 
     enabled: bool = True
     filter_key: SlugStr
@@ -247,32 +262,36 @@
 class TagFacetModel(BaseFacetModel):
 
     type: Literal["tag"]
     title: Optional[str]
 
 
 class ItemTypeFacetModel(BaseFacetModel):
+
     type: Literal["item_type"]
     title: Optional[str]
     item_view: bool = False
 
 
 class YearFacetModel(BaseFacetModel):
+
     type: Literal["year"]
     title: Optional[str]
     item_view: bool = False
 
 
 class LinkFacetModel(BaseFacetModel):
+
     type: Literal["link"]
     title: Optional[str]
     item_view: bool = False
 
 
 class CollectionFacetModel(BaseFacetModel):
+
     type: Literal["collection"]
     title: str
     collection_key: str = Field(regex=r'^[A-Z0-9]{8}$')
 
 
 # Note: Discriminated unions ensure that a single unambiguous error gets
 # reported when validation fails. Reference:
@@ -321,25 +340,103 @@
         extra = Extra.forbid
 
     enabled: bool = True
     weight: int = 0
     label: Optional[str]
 
 
+class LinkModel(BaseModel, ABC):
+
+    class Config:
+        extra = Extra.forbid
+
+    text: str
+    weight: int = 0
+    new_window: bool = False
+
+    @abstractmethod
+    def to_spec(self) -> LinkSpec:
+        pass
+
+
+class LinkByEndpointModel(LinkModel):
+    """Model for endpoint items under the kerko.link_groups config table."""
+
+    type: Literal["endpoint"]
+    endpoint: str
+    anchor: Optional[str]
+    scheme: Optional[str]
+    external: bool = False
+    parameters: Optional[Dict[str, Any]]
+
+    @root_validator
+    def validate_scheme(cls, values):  # pylint: disable=no-self-argument
+        if values.get('scheme') and not values.get('external'):
+            raise ValueError("When specifying 'scheme', 'external' must be true.")
+        return values
+
+    def to_spec(self) -> LinkSpec:
+        return LinkByEndpointSpec(
+            text=self.text,
+            weight=self.weight,
+            new_window=self.new_window,
+            endpoint=self.endpoint,
+            anchor=self.anchor,
+            scheme=self.scheme,
+            external=self.external,
+            parameters=self.parameters,
+        )
+
+
+class LinkByURLModel(LinkModel):
+    """Model for URL items under the kerko.link_groups config table."""
+
+    type: Literal["url"]
+    url: str  # TODO: Validate as URL string
+
+    def to_spec(self) -> LinkSpec:
+        return LinkByURLSpec(
+            text=self.text,
+            weight=self.weight,
+            new_window=self.new_window,
+            url=self.url,
+        )
+
+
+LinkModelUnion = Annotated[
+    Union[
+        LinkByEndpointModel,
+        LinkByURLModel,
+    ], Field(discriminator='type')
+]
+
+
+class LinkGroupsModel(BaseModel):  # TODO: Pydantic v2: inherit RootModel.
+    __root__: Dict[SlugStr, Annotated[List[LinkModelUnion], Field(min_items=1)]]
+
+    def to_spec(self) -> Dict[str, LinkGroupSpec]:
+        return {
+            key: LinkGroupSpec(key, [link_model.to_spec() for link_model in links])
+            for key, links in self.__root__.items()
+        }
+
+
 class KerkoModel(BaseModel):
     """Model for the kerko config table."""
 
     class Config:
         extra = Extra.forbid
 
     assets: AssetsModel
     features: FeaturesModel
     feeds: FeedsModel
     meta: MetaModel
     pagination: PaginationModel
+    breadcrumb: BreadcrumbModel
+    link_groups: LinkGroupsModel
     templates: TemplatesModel
     zotero: ZoteroModel
     search: SearchModel
     scopes: Dict[SlugStr, ScopesModel]
     search_fields: SearchFieldsModel
     facets: Dict[FieldNameStr, FacetModelUnion]
     sorts: Dict[SlugStr, SortsModel]
@@ -414,31 +511,40 @@
     config: Config,
     key: Optional[str] = None,
     model: Type[BaseModel] = ConfigModel
 ) -> None:
     """
     Parse and validate configuration using `model`.
 
-    Parameter values get replaced by parsed ones. Values may thus get silently
-    coerced into the types specified by the model (unless strict typing is
-    enforced by the model, in which case an error will be raised).
+    Configuration values in the `config` object get replaced by validated ones.
+    Values may thus get silently coerced into the types specified by the model
+    (unless strict typing is enforced by the model, in which case an error will
+    be raised).
+
+    This function also inserts a parsed representation of the configuration
+    under key 'kerko_config'.
 
     If `key` is `None`, then the whole configuration gets parsed with the given
     `model`. Otherwise only the structure at the specified `key` gets parsed.
 
-    If `key` does not exists in the config, parsing is silently skipped.
+    If `key` is not `None` but is absent from the config, parsing is silently
+    skipped.
     """
     try:
         if key is None:
-            config.update(model.parse_obj(config).dict())
+            parsed = model.parse_obj(config)
+            config.update(parsed.dict())
+            config['kerko_config'] = parsed
         elif config.get(key):
             # The parsed models are stored in the config as dicts. This way, the
             # whole configuration structure is made of dicts only, allowing
             # consistent access for any element at any depth.
-            config_set(config, key, model.parse_obj(config[key]).dict())
+            parsed = model.parse_obj(config[key])
+            config_set(config, key, parsed.dict())
+            config[f'kerko_config.{key}'] = parsed
     except ValidationError as e:
         raise RuntimeError(f"Invalid configuration. {e}") from e
 
 
 def is_toml_serializable(obj: object) -> bool:
     """
     Check if the given object would be serializable into a TOML file.
```

### Comparing `Kerko-1.0.0a1/src/kerko/criteria.py` & `Kerko-1.0.0a2/src/kerko/criteria.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/datetime.py` & `Kerko-1.0.0a2/src/kerko/datetime.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/default_config.toml` & `Kerko-1.0.0a2/src/kerko/default_config.toml`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,33 @@
 google_analytics_id = ""
 
 [kerko.pagination]
 
 page_len = 20
 pager_links = 4
 
+[kerko.breadcrumb]
+
+enabled = true
+include_current = true
+text_max_length = 50
+text_max_length_leeway = 10
+
+[kerko.link_groups]
+
+    [[kerko.link_groups.navbar]]
+    text = "Bibliography"
+    type = "endpoint"
+    endpoint = "kerko.search"
+
+    [[kerko.link_groups.breadcrumb_base]]
+    text = "Bibliography"
+    type = "endpoint"
+    endpoint = "kerko.search"
+
 [kerko.templates]
 
 base = "kerko/base.html.jinja2"
 layout = "kerko/layout.html.jinja2"
 search = "kerko/search.html.jinja2"
 search_item = "kerko/search-item.html.jinja2"
 item = "kerko/item.html.jinja2"
```

### Comparing `Kerko-1.0.0a1/src/kerko/exceptions.py` & `Kerko-1.0.0a2/src/kerko/exceptions.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/extractors.py` & `Kerko-1.0.0a2/src/kerko/extractors.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/jinja2.py` & `Kerko-1.0.0a2/src/kerko/jinja2.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/renderers.py` & `Kerko-1.0.0a2/src/kerko/renderers.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/searcher.py` & `Kerko-1.0.0a2/src/kerko/searcher.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/shortcuts.py` & `Kerko-1.0.0a2/src/kerko/shortcuts.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/specs.py` & `Kerko-1.0.0a2/src/kerko/specs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
+from typing import Any, Dict, List, Optional
 
 from babel.numbers import format_decimal
-from flask import url_for
+from flask import Request, url_for
 from flask_babel import get_locale
+from w3lib.url import safe_url_string
 from werkzeug.datastructures import MultiDict
 from whoosh.fields import ID
 from whoosh.query import Prefix, Term
 
 from kerko import extractors, renderers
 from kerko.codecs import (BaseFacetCodec, CollectionFacetCodec,
                           IdentityFieldCodec)
@@ -752,7 +754,80 @@
 
         :return str: The rendered badge, or `''` if the badge is not activated
             on the item.
         """
         if self.is_active(item):
             return self.renderer.render(field=self.field, item=item, mode=mode)
         return ''
+
+
+class LinkSpec(ABC):
+
+    def __init__(self, *, text: str, new_window=False, weight=0):
+        self.text = text
+        self.new_window = new_window
+        self.weight = weight
+
+    def is_active(self, request: Request) -> bool:  # pylint: disable=unused-argument
+        return False
+
+    @property
+    @abstractmethod
+    def url(self) -> str:
+        pass
+
+
+class LinkByURLSpec(LinkSpec):
+
+    def __init__(self, *, url: str, **kwargs):
+        super().__init__(**kwargs)
+        self._url = url
+
+    @property
+    def url(self) -> str:
+        return safe_url_string(self._url)
+
+
+class LinkByEndpointSpec(LinkSpec):
+
+    def __init__(
+        self,
+        *,
+        endpoint: str,
+        external: bool = False,
+        anchor: Optional[str] = None,
+        scheme: Optional[str] = None,
+        parameters: Optional[Dict[str, Any]] = None,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+        self.endpoint = endpoint
+        self.external = external
+        self.anchor = anchor or None  # Replace empty string with None.
+        self.scheme = scheme or None  # Replace empty string with None.
+        self.parameters = parameters or {}
+
+    def is_active(self, request: Request) -> bool:
+        return request.endpoint == self.endpoint
+
+    @property
+    def url(self) -> str:
+        return url_for(
+            self.endpoint,
+            _anchor=self.anchor,
+            _scheme=self.scheme,
+            _external=self.external,
+            **self.parameters,
+        )
+
+
+class LinkGroupSpec:
+
+    def __init__(self, key: str, links: Optional[List[LinkSpec]] = None):
+        self.key = key
+        self.links = links or []
+
+    def add_item(self, item: LinkSpec):
+        self.links.append(item)
+
+    def get_ordered_links(self) -> List[LinkSpec]:
+        return sorted(self.links, key=lambda spec: spec.weight)
```

### Comparing `Kerko-1.0.0a1/src/kerko/static/kerko/css/styles.css` & `Kerko-1.0.0a2/src/kerko/static/kerko/css/styles.css`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/static/kerko/js/open_in_zotero.js` & `Kerko-1.0.0a2/src/kerko/static/kerko/js/open_in_zotero.js`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/static/kerko/js/print.js` & `Kerko-1.0.0a2/src/kerko/static/kerko/js/print.js`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/static/kerko/js/search.js` & `Kerko-1.0.0a2/src/kerko/static/kerko/js/search.js`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/storage.py` & `Kerko-1.0.0a2/src/kerko/storage.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/sync/attachments.py` & `Kerko-1.0.0a2/src/kerko/sync/attachments.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/sync/cache.py` & `Kerko-1.0.0a2/src/kerko/sync/cache.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/sync/index.py` & `Kerko-1.0.0a2/src/kerko/sync/index.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/sync/zotero.py` & `Kerko-1.0.0a2/src/kerko/sync/zotero.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/tags.py` & `Kerko-1.0.0a2/src/kerko/tags.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_badges.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_badges.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_breadbox.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_breadbox.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_collapse.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_collapse.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_facet_field.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_facet_field.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_facets.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_facets.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_item-relations.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_item-relations.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_pager.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_pager.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_preferences.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_preferences.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_search-form.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_search-form.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_search-help.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_search-help.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_search-metas.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_search-metas.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_search-result.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_search-result.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/_sorter.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/_sorter.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/atom.xml.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/atom.xml.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/base.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/base.html.jinja2`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/item.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/item.html.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -276,21 +276,24 @@
                 {%- include "kerko/_preferences.html.jinja2" %}
             </div>
         {%- endif %}
     {%- endblock preferences %}
 {%- endblock footer_inner %}
 
 {%- block content_header %}
-    <div class="row">
-        <div class="{% block top_link_wrapper_classes %}col-auto ml-auto my-2 d-print-none{% endblock %}">
-            <a class="{% block top_btn_classes %}btn btn-primary{% endblock %}" href="{{ url_for('kerko.search') }}">
-                <span class="fas fa-arrow-up" aria-hidden="true"></span> {{ _("Full bibliography") }}
-            </a>
+    {%- if not config.kerko.breadcrumb.enabled %}
+        {#- The back link is redundant and wastes space if the breadcrumb is present. -#}
+        <div class="row">
+            <div class="{% block top_link_wrapper_classes %}col-auto ml-auto my-2 d-print-none{% endblock %}">
+                <a class="{% block top_btn_classes %}btn btn-primary{% endblock %}" href="{{ url_for('kerko.search') }}">
+                    <span class="fas fa-arrow-up" aria-hidden="true"></span> {{ _("Full bibliography") }}
+                </a>
+            </div>
         </div>
-    </div>
+    {%- endif %}
     <div class="row">
         <div class="{% block item_heading_wrapper_classes %}col-auto my-3{% endblock %}">
             <h1 class="{% block item_heading_classes %}h2 mb-0{% endblock %}">
                 {{- badges(item, mode='item') -}}
                 {{- title|escape -}}
             </h1>
         </div>
```

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/layout.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/layout.html.jinja2`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {% extends config.kerko.templates.base %}
 {% from "kerko/_attributes.html.jinja2" import title_aria_label %}
+{% from "kerko/_breadcrumb.html.jinja2" import breadcrumb %}
 
 {%- block meta_title_inner -%}
     {%- if title %}{{ title|escape }} | {% endif %}{{ super() -}}
 {%- endblock %}
 
 {%- block metas %}
     {{- super() }}
@@ -56,20 +57,27 @@
                     </nav>
                 {%- endblock navbar %}
             {%- endblock header_inner %}
         </header>
     {%- endblock header %}
     {%- block main %}
         <main {% block main_attributes %}class="container"{% endblock %}>
+            {%- block breadcrumb %}
+                {{ breadcrumb([title]) }}
+            {%- endblock breadcrumb %}
             {%- block main_inner %}
                 <div {% block main_inner_attributes %}class="row"{% endblock %}>
                     {%- block content %}
                         <div {% block content_attributes %}class="col-12 {% if self.sidebar_inner() %}col-lg-8 order-lg-4{% endif %}"{% endblock %}>
                             {%- block content_header %}
-                                <h1 class="{% block content_heading_classes %}h2 my-2{% endblock %}">{{ title }}</h1>
+                                <div class="row">
+                                    <div class="col">
+                                        <h1 class="{% block content_heading_classes %}h2 my-2{% endblock %}">{{ title|escape }}</h1>
+                                    </div>
+                                </div>
                             {%- endblock content_header %}
                             {%- block messages %}
                                 {%- with messages = get_flashed_messages(with_categories=true) %}
                                     {%- for category, message in messages %}
                                         <div class="alert alert-{{ category }}">
                                             <a class="close" {{ title_aria_label(_('Remove this message')) }} href="#" data-dismiss="alert">&times;</a>
                                             {{ message }}
```

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/search-item.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/search-item.html.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 {% set apply_relations_initial_limit = True %}
 {% extends config.kerko.templates.item %}
+{% from "kerko/_breadcrumb.html.jinja2" import breadcrumb %}
 
 {%- block metas %}
     {{- super() }}
     {%- include "kerko/_search-metas.html.jinja2" %}
 {%- endblock metas %}
 
+{%- block breadcrumb %}
+    {%- if is_searching and back_url %}
+        {{ breadcrumb([{'url': back_url, 'text': _("Your search")}, title]) }}
+    {%- else %}
+        {{ super() }}
+    {%- endif %}
+{%- endblock breadcrumb %}
+
 {%- block content_header %}
     <div class="mt-2 row">
         <h1 class="{% block search_heading_classes %}h4 col-auto mr-auto pr-1 d-inline d-print-none{% endblock %}">
             {{- search_title -}}
         </h1>
         {%- if back_url %}
             <div class="{% block back_link_wrapper_classes %}col-auto ml-auto mb-2 pl-1 text-right d-print-none{% endblock %}">
```

### Comparing `Kerko-1.0.0a1/src/kerko/templates/kerko/search.html.jinja2` & `Kerko-1.0.0a2/src/kerko/templates/kerko/search.html.jinja2`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 {% extends config.kerko.templates.layout %}
 {% from "kerko/_attributes.html.jinja2" import title_aria_label %}
+{% from "kerko/_breadcrumb.html.jinja2" import breadcrumb %}
 
 {%- set show_print_link = config.kerko.features.print_results_max_count == 0 or total_count <= config.kerko.features.print_results_max_count %}
 {%- set show_print_link = show_print_link and config.kerko.features.print_results_link %}
 {%- set show_download_link = config.kerko.features.download_results_max_count == 0 or total_count <= config.kerko.features.download_results_max_count %}
 {%- set show_download_link = show_download_link and config.kerko.features.download_results_link and config.kerko_composer.bib_formats %}
 {%- set abstracts_toggler_title = _('Hide abstracts') if show_abstracts else _('Show abstracts') %}
 
 {%- block metas %}
     {{- super() }}
     {%- include "kerko/_search-metas.html.jinja2" %}
 {%- endblock metas %}
 
+{%- block breadcrumb %}
+    {%- if is_searching %}
+        {{ breadcrumb([_("Your search")]) }}
+    {%- else %}
+        {{ breadcrumb() }}
+    {%- endif %}
+{%- endblock breadcrumb %}
+
 {%- block content_header %}
     <div class="my-2 row">
         <h1 class="{% block search_heading_classes %}h2 col-auto pr-1 mr-auto d-inline{% endblock %}{% if not is_searching %} d-print-none{% endif %}">
             {%- if is_searching %}
                 {{ _("Your search") }}
             {%- else %}
                 {{ _("Search") }}
```

### Comparing `Kerko-1.0.0a1/src/kerko/text.py` & `Kerko-1.0.0a2/src/kerko/text.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/transformers.py` & `Kerko-1.0.0a2/src/kerko/transformers.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/translations/de/LC_MESSAGES/kerko.mo` & `Kerko-1.0.0a2/src/kerko/translations/de/LC_MESSAGES/kerko.mo`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/translations/de/LC_MESSAGES/kerko.po` & `Kerko-1.0.0a2/src/kerko/translations/de/LC_MESSAGES/kerko.po`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/translations/fr/LC_MESSAGES/kerko.mo` & `Kerko-1.0.0a2/src/kerko/translations/fr/LC_MESSAGES/kerko.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Kerko\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-05-12 16:19-0400\n"
-"PO-Revision-Date: 2023-05-12 16:19-0400\n"
+"POT-Creation-Date: 2023-07-08 15:46-0400\n"
+"PO-Revision-Date: 2023-07-08 15:46-0400\n"
 "Last-Translator: David Lesieur <kerko@whiskyechobravo.com>\n"
 "Language: fr\n"
 "Language-Team: fr <kerko@whiskyechobravo.com>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -115,20 +115,20 @@
 
 msgid "Between {} and {}"
 msgstr "Entre {} et {}"
 
 msgid "BibTeX"
 msgstr "BibTeX"
 
-msgid "Bibliography"
-msgstr "Bibliographie"
-
 msgid "Boolean operators must be entered in UPPERCASE."
 msgstr "Les opérateurs booléens doivent être saisis en MAJUSCULES."
 
+msgid "Breadcrumb"
+msgstr "Fil d'Ariane"
+
 msgid ""
 "Categories can be used to filter your search. Check a category to add it to "
 "your search criteria and narrow your search. Your search results will then "
 "only show entries that are associated with that category."
 msgstr ""
 "Les catégories peuvent servir à affiner votre recherche. Cochez une "
 "catégorie pour l’ajouter à vos critères de recherche. Les résultats seront "
```

### Comparing `Kerko-1.0.0a1/src/kerko/translations/fr/LC_MESSAGES/kerko.po` & `Kerko-1.0.0a2/src/kerko/translations/fr/LC_MESSAGES/kerko.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # This file is distributed under the same license as the Kerko project.
 # David Lesieur <kerko@whiskyechobravo.com>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version:  Kerko\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-05-12 16:19-0400\n"
-"PO-Revision-Date: 2023-05-12 16:19-0400\n"
+"POT-Creation-Date: 2023-07-08 15:46-0400\n"
+"PO-Revision-Date: 2023-07-08 15:46-0400\n"
 "Last-Translator: David Lesieur <kerko@whiskyechobravo.com>\n"
 "Language: fr\n"
 "Language-Team: fr <kerko@whiskyechobravo.com>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -30,133 +30,133 @@
 msgid "In {}"
 msgstr "En {}"
 
 #: src/kerko/codecs.py:216
 msgid "Between {} and {}"
 msgstr "Entre {} et {}"
 
-#: src/kerko/composer.py:247 src/kerko/composer.py:248
+#: src/kerko/composer.py:90 src/kerko/composer.py:97
 msgid "Everywhere"
 msgstr "Partout"
 
-#: src/kerko/composer.py:250
+#: src/kerko/composer.py:91 src/kerko/composer.py:98
+msgid "In authors or contributors"
+msgstr "Dans les auteurs ou contributeurs"
+
+#: src/kerko/composer.py:92 src/kerko/composer.py:99
+msgid "In titles"
+msgstr "Dans les titres"
+
+#: src/kerko/composer.py:93 src/kerko/composer.py:100
+msgid "In all fields"
+msgstr "Dans tous les champs"
+
+#: src/kerko/composer.py:94 src/kerko/composer.py:101
+msgid "In documents"
+msgstr "Dans les documents"
+
+#: src/kerko/composer.py:104
 msgid ""
 "Search your keywords in all bibliographic record fields and in the text "
 "content of the available documents."
 msgstr ""
 "repère vos mots-clés dans tous les champs des références bibliographiques"
 " ainsi que dans le contenu textuel des documents disponibles."
 
-#: src/kerko/composer.py:260 src/kerko/composer.py:261
-msgid "In authors or contributors"
-msgstr "Dans les auteurs ou contributeurs"
-
-#: src/kerko/composer.py:263
+#: src/kerko/composer.py:108
 msgid "Search your keywords in author or contributor names."
 msgstr "repère vos mots-clés dans les noms d’auteurs ou de contributeurs."
 
-#: src/kerko/composer.py:270 src/kerko/composer.py:271
-msgid "In titles"
-msgstr "Dans les titres"
-
-#: src/kerko/composer.py:273
+#: src/kerko/composer.py:109
 msgid "Search your keywords in titles."
 msgstr "repère vos mots-clés dans les titres."
 
-#: src/kerko/composer.py:280 src/kerko/composer.py:281
-msgid "In all fields"
-msgstr "Dans tous les champs"
-
-#: src/kerko/composer.py:283
+#: src/kerko/composer.py:110
 msgid "Search your keywords in all bibliographic record fields."
 msgstr "repère vos mots-clés dans tous les champs des notices bibliographiques."
 
-#: src/kerko/composer.py:290 src/kerko/composer.py:291
-msgid "In documents"
-msgstr "Dans les documents"
-
-#: src/kerko/composer.py:293
+#: src/kerko/composer.py:111
 msgid "Search your keywords in the text content of the available documents."
 msgstr "repère vos mots-clés dans le contenu textuel des documents disponibles."
 
-#: src/kerko/composer.py:1587
+#: src/kerko/composer.py:573
 msgid "Topic"
 msgstr "Sujet"
 
-#: src/kerko/composer.py:1610 src/kerko/templates/kerko/item.html.jinja2:121
+#: src/kerko/composer.py:587 src/kerko/templates/kerko/item.html.jinja2:121
 msgid "Resource type"
 msgstr "Type de ressource"
 
-#: src/kerko/composer.py:1630
+#: src/kerko/composer.py:601
 msgid "Publication year"
 msgstr "Année de publication"
 
-#: src/kerko/composer.py:1638
+#: src/kerko/composer.py:602
 msgid "Unknown"
 msgstr "Inconnue"
 
-#: src/kerko/composer.py:1650
+#: src/kerko/composer.py:615
 msgid "Online resource"
 msgstr "Ressource en ligne"
 
-#: src/kerko/composer.py:1681
+#: src/kerko/composer.py:646
 msgid "Relevance"
 msgstr "Pertinence"
 
-#: src/kerko/composer.py:1692
+#: src/kerko/composer.py:657
 msgid "Newest first"
 msgstr "Date décroissante"
 
-#: src/kerko/composer.py:1710
+#: src/kerko/composer.py:675
 msgid "Oldest first"
 msgstr "Date croissante"
 
-#: src/kerko/composer.py:1723
+#: src/kerko/composer.py:688
 msgid "Author A-Z"
 msgstr "Auteur A-Z"
 
-#: src/kerko/composer.py:1736
+#: src/kerko/composer.py:701
 msgid "Author Z-A"
 msgstr "Auteur Z-A"
 
-#: src/kerko/composer.py:1754
+#: src/kerko/composer.py:719
 msgid "Title A-Z"
 msgstr "Titre A-Z"
 
-#: src/kerko/composer.py:1767
+#: src/kerko/composer.py:732
 msgid "Title Z-A"
 msgstr "Titre Z-A"
 
-#: src/kerko/composer.py:1799
+#: src/kerko/composer.py:765
 msgid "RIS"
 msgstr "RIS"
 
-#: src/kerko/composer.py:1800
+#: src/kerko/composer.py:766
 msgid "Recommended format for most reference management software"
 msgstr ""
 "Format recommandé pour la plupart des logiciels de gestion de références "
 "bibliographiques"
 
-#: src/kerko/composer.py:1811
+#: src/kerko/composer.py:775
 msgid "BibTeX"
 msgstr "BibTeX"
 
-#: src/kerko/composer.py:1812
+#: src/kerko/composer.py:776
 msgid "Recommended format for BibTeX-specific software"
 msgstr "Format recommandé pour les logiciels spécialement conçus pour BibTeX"
 
-#: src/kerko/composer.py:1836
+#: src/kerko/composer.py:795
 msgid "Cites"
 msgstr "Cite"
 
-#: src/kerko/composer.py:1842
+#: src/kerko/composer.py:801
 msgid "Cited by"
 msgstr "Cité par"
 
-#: src/kerko/composer.py:1850
+#: src/kerko/composer.py:809
 msgid "Related"
 msgstr "Connexe"
 
 #: src/kerko/searcher.py:109
 #: src/kerko/templates/kerko/_search-help.html.jinja2:37
 #: src/kerko/templates/kerko/_search-help.html.jinja2:43
 msgid "AND"
@@ -179,18 +179,22 @@
 
 #: src/kerko/templates/kerko/_breadbox.html.jinja2:28
 msgid "None of your search criteria could be recognized."
 msgstr "Aucun de vos critères de recherche n’a pu être reconnu."
 
 #: src/kerko/templates/kerko/_breadbox.html.jinja2:29
 #: src/kerko/templates/kerko/_search-help.html.jinja2:22
-#: src/kerko/templates/kerko/search.html.jinja2:41
+#: src/kerko/templates/kerko/search.html.jinja2:50
 msgid "Reset search"
 msgstr "Réinitialiser la recherche"
 
+#: src/kerko/templates/kerko/_breadcrumb.html.jinja2:42
+msgid "Breadcrumb"
+msgstr "Fil d'Ariane"
+
 #: src/kerko/templates/kerko/_collapse.html.jinja2:6
 msgid "Show more"
 msgstr "Montrer plus"
 
 #: src/kerko/templates/kerko/_collapse.html.jinja2:9
 msgid "Show less"
 msgstr "Montrer moins"
@@ -211,18 +215,14 @@
 msgid "Expand subfilters"
 msgstr "Afficher les filtres plus spécifiques"
 
 #: src/kerko/templates/kerko/_facets.html.jinja2:20
 msgid "Collapse subfilters"
 msgstr "Masquer les filtres plus spécifiques"
 
-#: src/kerko/templates/kerko/_navbar_items.html.jinja2:3
-msgid "Bibliography"
-msgstr "Bibliographie"
-
 #: src/kerko/templates/kerko/_pager.html.jinja2:5
 msgid "Previous page"
 msgstr "Page précédente"
 
 #: src/kerko/templates/kerko/_pager.html.jinja2:13
 msgid "Next page"
 msgstr "Page suivante"
@@ -296,20 +296,20 @@
 "button allows you to view the record on zotero.org. It might be useful "
 "only if you were granted access to the Zotero library that holds the "
 "record."
 msgstr ""
 "Montrer ou cacher le bouton « {} » sur les pages de notices "
 "bibliographiques. Ce bouton vous permet de consulter la notice sur "
 "zotero.org. Celui-ci ne peut être utile que si vous avez obtenu la "
-"permission d’accéder à la bibliothèque Zotero dans laquelle est "
-"consignée la notice."
+"permission d’accéder à la bibliothèque Zotero dans laquelle est consignée"
+" la notice."
 
 #: src/kerko/templates/kerko/_preferences.html.jinja2:41
 #: src/kerko/templates/kerko/_search-help.html.jinja2:72
-#: src/kerko/templates/kerko/search.html.jinja2:191
+#: src/kerko/templates/kerko/search.html.jinja2:200
 msgid "Close"
 msgstr "Fermer"
 
 #: src/kerko/templates/kerko/_search-form.html.jinja2:8
 msgid "Search within results for..."
 msgstr "Chercher parmi les résultats..."
 
@@ -322,20 +322,20 @@
 msgstr "Chercher dans..."
 
 #: src/kerko/templates/kerko/_search-form.html.jinja2:19
 #: src/kerko/templates/kerko/_search-help.html.jinja2:16
 #: src/kerko/templates/kerko/_search-help.html.jinja2:17
 #: src/kerko/templates/kerko/_search-help.html.jinja2:18
 #: src/kerko/templates/kerko/_search-help.html.jinja2:67
-#: src/kerko/templates/kerko/search.html.jinja2:21
+#: src/kerko/templates/kerko/search.html.jinja2:30
 msgid "Search"
 msgstr "Rechercher"
 
 #: src/kerko/templates/kerko/_search-help.html.jinja2:8
-#: src/kerko/templates/kerko/search.html.jinja2:28
+#: src/kerko/templates/kerko/search.html.jinja2:37
 msgid "Help"
 msgstr "Aide"
 
 #: src/kerko/templates/kerko/_search-help.html.jinja2:9
 #: src/kerko/templates/kerko/_search-help.html.jinja2:72
 msgid "Close Help panel"
 msgstr "Fermer le panneau d’aide"
@@ -350,17 +350,17 @@
 "<strong>{}</strong>, <strong>{}</strong> et <strong>{}</strong>. Celles-"
 "ci sont décrites en détail ci-dessous."
 
 #: src/kerko/templates/kerko/_search-help.html.jinja2:16
 #: src/kerko/templates/kerko/_search-help.html.jinja2:17
 #: src/kerko/templates/kerko/_search-help.html.jinja2:49
 #: src/kerko/templates/kerko/_search-help.html.jinja2:68
-#: src/kerko/templates/kerko/search.html.jinja2:34
-#: src/kerko/templates/kerko/search.html.jinja2:173
-#: src/kerko/templates/kerko/search.html.jinja2:184
+#: src/kerko/templates/kerko/search.html.jinja2:43
+#: src/kerko/templates/kerko/search.html.jinja2:182
+#: src/kerko/templates/kerko/search.html.jinja2:193
 msgid "Explore"
 msgstr "Explorer"
 
 #: src/kerko/templates/kerko/_search-help.html.jinja2:16
 #: src/kerko/templates/kerko/_search-help.html.jinja2:57
 msgid "Results"
 msgstr "Résultats"
@@ -728,23 +728,23 @@
 msgstr "Lien permanent vers cette notice bibliographique"
 
 #: src/kerko/templates/kerko/item.html.jinja2:85
 msgid "Print this record"
 msgstr "Imprimer cette notice"
 
 #: src/kerko/templates/kerko/item.html.jinja2:93
-#: src/kerko/templates/kerko/search.html.jinja2:124
+#: src/kerko/templates/kerko/search.html.jinja2:133
 #, python-format
 msgid "Download this record"
 msgid_plural "Download %(count_formatted)s records"
 msgstr[0] "Télécharger cette notice"
 msgstr[1] "Télécharger %(count_formatted)s notices"
 
 #: src/kerko/templates/kerko/item.html.jinja2:97
-#: src/kerko/templates/kerko/search.html.jinja2:128
+#: src/kerko/templates/kerko/search.html.jinja2:137
 msgid "Download in {download_option} format"
 msgstr "Télécharger au format {download_option}"
 
 #: src/kerko/templates/kerko/item.html.jinja2:121
 msgid "Search the '{}' resource type"
 msgstr "Chercher le type de ressource '{}'"
 
@@ -783,77 +783,79 @@
 msgstr "Lien vers cette notice"
 
 #: src/kerko/templates/kerko/item.html.jinja2:220
 msgid "Relations"
 msgstr "Relations"
 
 #: src/kerko/templates/kerko/item.html.jinja2:262
-#: src/kerko/templates/kerko/search.html.jinja2:149
+#: src/kerko/templates/kerko/search.html.jinja2:158
 #, python-format
 msgid "Processing time: %(time)s seconds"
 msgstr "Temps de traitement: %(time)s seconds"
 
-#: src/kerko/templates/kerko/item.html.jinja2:286 src/kerko/views/search.py:122
+#: src/kerko/templates/kerko/item.html.jinja2:288 src/kerko/views/search.py:122
 #: src/kerko/views/search.py:200
 msgid "Full bibliography"
 msgstr "Bibliographie complète"
 
-#: src/kerko/templates/kerko/layout.html.jinja2:42
+#: src/kerko/templates/kerko/layout.html.jinja2:43
 msgid "Toggle navigation"
 msgstr "Basculer la navigation"
 
-#: src/kerko/templates/kerko/layout.html.jinja2:74
+#: src/kerko/templates/kerko/layout.html.jinja2:82
 msgid "Remove this message"
 msgstr "Retirer ce message"
 
-#: src/kerko/templates/kerko/layout.html.jinja2:102
+#: src/kerko/templates/kerko/layout.html.jinja2:110
 msgid "Powered by {zotero} and {kerko}."
 msgstr "Propulsé par {zotero} et {kerko}."
 
-#: src/kerko/templates/kerko/search-item.html.jinja2:17
+#: src/kerko/templates/kerko/search-item.html.jinja2:12
+#: src/kerko/templates/kerko/search.html.jinja2:18
+#: src/kerko/templates/kerko/search.html.jinja2:28
+#: src/kerko/views/search.py:120
+msgid "Your search"
+msgstr "Votre recherche"
+
+#: src/kerko/templates/kerko/search-item.html.jinja2:26
 msgid "Return to list of results"
 msgstr "Retourner à la liste des résultats"
 
-#: src/kerko/templates/kerko/search.html.jinja2:8
+#: src/kerko/templates/kerko/search.html.jinja2:9
 msgid "Hide abstracts"
 msgstr "Cacher les résumés"
 
-#: src/kerko/templates/kerko/search.html.jinja2:8
+#: src/kerko/templates/kerko/search.html.jinja2:9
 msgid "Show abstracts"
 msgstr "Montrer les résumés"
 
-#: src/kerko/templates/kerko/search.html.jinja2:19
-#: src/kerko/views/search.py:120
-msgid "Your search"
-msgstr "Votre recherche"
-
-#: src/kerko/templates/kerko/search.html.jinja2:68
+#: src/kerko/templates/kerko/search.html.jinja2:77
 #, python-format
 msgid "%(count_formatted)s resource"
 msgid_plural "%(count_formatted)s resources"
 msgstr[0] "%(count_formatted)s ressource"
 msgstr[1] "%(count_formatted)s ressources"
 
-#: src/kerko/templates/kerko/search.html.jinja2:93
+#: src/kerko/templates/kerko/search.html.jinja2:102
 msgid "Abstracts"
 msgstr "Résumés"
 
-#: src/kerko/templates/kerko/search.html.jinja2:116
+#: src/kerko/templates/kerko/search.html.jinja2:125
 #, python-format
 msgid "Print this citation"
 msgid_plural "Print %(count_formatted)s citations"
 msgstr[0] "Imprimer cette référence"
 msgstr[1] "Imprimer %(count_formatted)s références"
 
-#: src/kerko/templates/kerko/search.html.jinja2:152
+#: src/kerko/templates/kerko/search.html.jinja2:161
 #, python-format
 msgid "Last update from database: %(when)s"
 msgstr "Dernière mise à jour depuis la base de données&nbsp;: %(when)s"
 
-#: src/kerko/templates/kerko/search.html.jinja2:157
+#: src/kerko/templates/kerko/search.html.jinja2:166
 msgid ""
 "\n"
 "                <p>Suggestions:</p>\n"
 "                <ul>\n"
 "                    <li>Make sure that all words are spelled "
 "correctly.</li>\n"
 "                    <li>Try different words.</li>\n"
@@ -865,28 +867,28 @@
 "                <ul>\n"
 "                    <li>Vérifiez que tous les mots sont orthographiés "
 "correctement.</li>\n"
 "                    <li>Essayez des termes différents.</li>\n"
 "                    <li>Essayez des termes plus généraux.</li>\n"
 "                </ul>"
 
-#: src/kerko/templates/kerko/search.html.jinja2:185
-#: src/kerko/templates/kerko/search.html.jinja2:191
+#: src/kerko/templates/kerko/search.html.jinja2:194
+#: src/kerko/templates/kerko/search.html.jinja2:200
 msgid "Close Explore panel"
 msgstr "Fermer le panneau d’exploration"
 
-#: src/kerko/views/routes.py:131 src/kerko/views/search.py:250
+#: src/kerko/views/routes.py:126 src/kerko/views/search.py:250
 msgid "Custom feed"
 msgstr "Flux web personnalisé"
 
-#: src/kerko/views/routes.py:133 src/kerko/views/search.py:252
+#: src/kerko/views/routes.py:128 src/kerko/views/search.py:252
 msgid "Main feed"
 msgstr "Flux web principal"
 
-#: src/kerko/views/routes.py:242
+#: src/kerko/views/routes.py:231
 msgid ""
 "The document you have requested has been removed. Please check below for "
 "the latest documents available."
 msgstr ""
 "Le document demandé a été supprimé. Voyez ci-dessous pour les plus "
 "récents documents disponibles."
```

### Comparing `Kerko-1.0.0a1/src/kerko/translations/pt/LC_MESSAGES/kerko.mo` & `Kerko-1.0.0a2/src/kerko/translations/pt/LC_MESSAGES/kerko.mo`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/translations/pt/LC_MESSAGES/kerko.po` & `Kerko-1.0.0a2/src/kerko/translations/pt/LC_MESSAGES/kerko.po`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/tree.py` & `Kerko-1.0.0a2/src/kerko/tree.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/views/breadbox.py` & `Kerko-1.0.0a2/src/kerko/views/breadbox.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/views/item/__init__.py` & `Kerko-1.0.0a2/src/kerko/views/item/__init__.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/views/item/creators.py` & `Kerko-1.0.0a2/src/kerko/views/item/creators.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/views/item/facets.py` & `Kerko-1.0.0a2/src/kerko/views/item/facets.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/views/item/meta.py` & `Kerko-1.0.0a2/src/kerko/views/item/meta.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/views/item/relations.py` & `Kerko-1.0.0a2/src/kerko/views/item/relations.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/views/pager.py` & `Kerko-1.0.0a2/src/kerko/views/pager.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/views/routes.py` & `Kerko-1.0.0a2/src/kerko/views/routes.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/views/search.py` & `Kerko-1.0.0a2/src/kerko/views/search.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/src/kerko/views/sorter.py` & `Kerko-1.0.0a2/src/kerko/views/sorter.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/README.md` & `Kerko-1.0.0a2/tests/integration_testing/README.md`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/__init__.py` & `Kerko-1.0.0a2/tests/integration_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/collections.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/collections.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_artwork.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_artwork.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_audioRecording.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_bill.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_bill.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_blogPost.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_blogPost.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_book.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_book.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_bookSection.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_bookSection.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_case.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_case.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_computerProgram.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_conferencePaper.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_dictionaryEntry.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_document.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_document.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_email.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_email.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_encyclopediaArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_film.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_film.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_forumPost.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_forumPost.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_hearing.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_hearing.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_instantMessage.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_interview.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_interview.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_journalArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_letter.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_letter.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_magazineArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_manuscript.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_manuscript.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_map.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_map.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_newspaperArticle.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_patent.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_patent.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_podcast.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_podcast.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_preprint.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_preprint.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_presentation.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_presentation.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_radioBroadcast.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_report.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_report.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_statute.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_statute.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_thesis.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_thesis.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_tvBroadcast.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_videoRecording.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypeFields_webpage.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypeFields_webpage.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/itemTypes.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/itemTypes.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/items.json` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/items.json`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/integration_testing/api_responses/update.bash` & `Kerko-1.0.0a2/tests/integration_testing/api_responses/update.bash`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/test_atom_feed.py` & `Kerko-1.0.0a2/tests/test_atom_feed.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/test_config.py` & `Kerko-1.0.0a2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/test_datetime.py` & `Kerko-1.0.0a2/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/test_item_meta.py` & `Kerko-1.0.0a2/tests/test_item_meta.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/test_pager.py` & `Kerko-1.0.0a2/tests/test_pager.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/test_sitemap.py` & `Kerko-1.0.0a2/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/test_sync.py` & `Kerko-1.0.0a2/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tests/test_tags.py` & `Kerko-1.0.0a2/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `Kerko-1.0.0a1/tox.ini` & `Kerko-1.0.0a2/tox.ini`

 * *Files identical despite different names*

