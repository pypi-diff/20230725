# Comparing `tmp/popcornshow-0.1.1.tar.gz` & `tmp/popcornshow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popcornshow-0.1.1.tar", max compression
+gzip compressed data, was "popcornshow-0.1.2.tar", max compression
```

## Comparing `popcornshow-0.1.1.tar` & `popcornshow-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0       30 2023-07-16 06:40:25.287069 popcornshow-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-07-08 04:34:41.268232 popcornshow-0.1.1/popcorn/__init__.py
--rw-r--r--   0        0        0     7672 2023-07-09 04:14:08.738462 popcornshow-0.1.1/popcorn/api/api.py
--rw-r--r--   0        0        0      448 2023-07-08 20:30:49.768143 popcornshow-0.1.1/popcorn/api/models/PersonApi.py
--rw-r--r--   0        0        0      182 2023-07-08 19:58:56.355271 popcornshow-0.1.1/popcorn/api/models/Result.py
--rw-r--r--   0        0        0     3418 2023-07-08 20:30:49.783769 popcornshow-0.1.1/popcorn/api/models/SearchApi.py
--rw-r--r--   0        0        0     8167 2023-07-24 21:45:48.324416 popcornshow-0.1.1/popcorn/cli.py
--rw-r--r--   0        0        0       35 2023-07-08 19:57:50.362411 popcornshow-0.1.1/popcorn/config.py
--rw-r--r--   0        0        0     2596 2023-07-17 02:03:01.016953 popcornshow-0.1.1/popcorn/controller.py
--rw-r--r--   0        0        0      619 2023-07-17 02:03:01.017951 popcornshow-0.1.1/popcorn/dto.py
--rw-r--r--   0        0        0      291 2023-03-16 02:28:48.138564 popcornshow-0.1.1/popcorn/models/AlsoWatched.py
--rw-r--r--   0        0        0      394 2023-07-08 20:30:49.785775 popcornshow-0.1.1/popcorn/models/Content.py
--rw-r--r--   0        0        0      967 2023-07-08 19:58:56.402579 popcornshow-0.1.1/popcorn/models/Creative.py
--rw-r--r--   0        0        0      115 2023-07-08 19:58:56.402579 popcornshow-0.1.1/popcorn/models/Ios.py
--rw-r--r--   0        0        0     8032 2023-07-17 02:03:01.017951 popcornshow-0.1.1/popcorn/models/ItemMovie.py
--rw-r--r--   0        0        0     8300 2023-07-17 02:03:01.018953 popcornshow-0.1.1/popcorn/models/ItemShow.py
--rw-r--r--   0        0        0      282 2023-07-08 19:58:56.355271 popcornshow-0.1.1/popcorn/models/Links.py
--rw-r--r--   0        0        0      246 2023-03-16 02:25:09.533167 popcornshow-0.1.1/popcorn/models/ListingKey.py
--rw-r--r--   0        0        0      118 2023-07-08 19:58:56.355271 popcornshow-0.1.1/popcorn/models/Metadata.py
--rw-r--r--   0        0        0      847 2023-07-08 20:30:49.815419 popcornshow-0.1.1/popcorn/models/Person.py
--rw-r--r--   0        0        0      300 2023-07-08 19:58:56.370912 popcornshow-0.1.1/popcorn/models/Rank.py
--rw-r--r--   0        0        0      578 2023-07-08 19:58:56.380927 popcornshow-0.1.1/popcorn/models/ReelgoodScores.py
--rw-r--r--   0        0        0      601 2023-07-08 19:58:56.386939 popcornshow-0.1.1/popcorn/models/RegionalAvailability.py
--rw-r--r--   0        0        0      354 2023-07-08 20:30:49.815419 popcornshow-0.1.1/popcorn/models/ScoreBreakdown.py
--rw-r--r--   0        0        0      903 2023-07-17 02:03:01.018953 popcornshow-0.1.1/popcorn/models/Search.py
--rw-r--r--   0        0        0      832 2023-07-08 19:58:56.386939 popcornshow-0.1.1/popcorn/models/Seasons.py
--rw-r--r--   0        0        0     1770 2023-07-08 20:30:49.831042 popcornshow-0.1.1/popcorn/models/SourceAdPlacement.py
--rw-r--r--   0        0        0      161 2023-07-08 19:58:56.386939 popcornshow-0.1.1/popcorn/models/Streamability.py
--rw-r--r--   0        0        0      183 2023-07-08 19:58:56.386939 popcornshow-0.1.1/popcorn/models/Tag.py
--rw-r--r--   0        0        0      206 2023-07-08 19:58:56.386939 popcornshow-0.1.1/popcorn/models/Trailer.py
--rw-r--r--   0        0        0     3452 2023-03-25 22:50:45.329984 popcornshow-0.1.1/popcorn/models/TVShowEpisode.py
--rw-r--r--   0        0        0     1951 2023-07-17 02:03:01.019953 popcornshow-0.1.1/popcorn/tables/people.py
--rw-r--r--   0        0        0     5478 2023-07-17 02:03:01.019953 popcornshow-0.1.1/popcorn/tables/sources.py
--rw-r--r--   0        0        0     1473 2023-07-17 02:03:01.020951 popcornshow-0.1.1/popcorn/tables/table_details_movie.py
--rw-r--r--   0        0        0     1221 2023-07-17 02:03:01.020951 popcornshow-0.1.1/popcorn/tables/table_person.py
--rw-r--r--   0        0        0     1321 2023-07-17 02:03:01.021952 popcornshow-0.1.1/popcorn/tables/table_search.py
--rw-r--r--   0        0        0     1243 2023-07-08 20:30:49.846667 popcornshow-0.1.1/popcorn/tables/tableDetailsShow.py
--rw-r--r--   0        0        0      357 2023-07-08 19:58:56.418205 popcornshow-0.1.1/popcorn/tables/TableInterface.py
--rw-r--r--   0        0        0     2376 2023-07-17 02:03:01.021952 popcornshow-0.1.1/popcorn/utils.py
--rw-r--r--   0        0        0     1672 2023-07-24 21:48:16.190210 popcornshow-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2287 2023-07-22 21:17:14.185532 popcornshow-0.1.1/README.md
--rw-r--r--   0        0        0     3131 1970-01-01 00:00:00.000000 popcornshow-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-07-16 06:40:25.287069 popcornshow-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-08 04:34:41.268232 popcornshow-0.1.2/popcorn/__init__.py
+-rw-r--r--   0        0        0     7676 2023-07-25 00:36:21.677008 popcornshow-0.1.2/popcorn/api/api.py
+-rw-r--r--   0        0        0      448 2023-07-08 20:30:49.768143 popcornshow-0.1.2/popcorn/api/models/PersonApi.py
+-rw-r--r--   0        0        0      182 2023-07-08 19:58:56.355271 popcornshow-0.1.2/popcorn/api/models/Result.py
+-rw-r--r--   0        0        0     3418 2023-07-08 20:30:49.783769 popcornshow-0.1.2/popcorn/api/models/SearchApi.py
+-rw-r--r--   0        0        0     8216 2023-07-25 01:57:42.544941 popcornshow-0.1.2/popcorn/cli.py
+-rw-r--r--   0        0        0       35 2023-07-08 19:57:50.362411 popcornshow-0.1.2/popcorn/config.py
+-rw-r--r--   0        0        0     2650 2023-07-25 01:48:24.057027 popcornshow-0.1.2/popcorn/controller.py
+-rw-r--r--   0        0        0      619 2023-07-17 02:03:01.017951 popcornshow-0.1.2/popcorn/dto.py
+-rw-r--r--   0        0        0      291 2023-03-16 02:28:48.138564 popcornshow-0.1.2/popcorn/models/AlsoWatched.py
+-rw-r--r--   0        0        0      394 2023-07-08 20:30:49.785775 popcornshow-0.1.2/popcorn/models/Content.py
+-rw-r--r--   0        0        0      967 2023-07-08 19:58:56.402579 popcornshow-0.1.2/popcorn/models/Creative.py
+-rw-r--r--   0        0        0      115 2023-07-08 19:58:56.402579 popcornshow-0.1.2/popcorn/models/Ios.py
+-rw-r--r--   0        0        0     8105 2023-07-25 01:48:15.970312 popcornshow-0.1.2/popcorn/models/ItemMovie.py
+-rw-r--r--   0        0        0     8305 2023-07-25 00:43:17.172712 popcornshow-0.1.2/popcorn/models/ItemShow.py
+-rw-r--r--   0        0        0      282 2023-07-08 19:58:56.355271 popcornshow-0.1.2/popcorn/models/Links.py
+-rw-r--r--   0        0        0      246 2023-03-16 02:25:09.533167 popcornshow-0.1.2/popcorn/models/ListingKey.py
+-rw-r--r--   0        0        0      118 2023-07-08 19:58:56.355271 popcornshow-0.1.2/popcorn/models/Metadata.py
+-rw-r--r--   0        0        0      847 2023-07-08 20:30:49.815419 popcornshow-0.1.2/popcorn/models/Person.py
+-rw-r--r--   0        0        0      300 2023-07-08 19:58:56.370912 popcornshow-0.1.2/popcorn/models/Rank.py
+-rw-r--r--   0        0        0      578 2023-07-08 19:58:56.380927 popcornshow-0.1.2/popcorn/models/ReelgoodScores.py
+-rw-r--r--   0        0        0      601 2023-07-08 19:58:56.386939 popcornshow-0.1.2/popcorn/models/RegionalAvailability.py
+-rw-r--r--   0        0        0      354 2023-07-08 20:30:49.815419 popcornshow-0.1.2/popcorn/models/ScoreBreakdown.py
+-rw-r--r--   0        0        0      920 2023-07-25 01:42:26.121757 popcornshow-0.1.2/popcorn/models/Search.py
+-rw-r--r--   0        0        0      832 2023-07-08 19:58:56.386939 popcornshow-0.1.2/popcorn/models/Seasons.py
+-rw-r--r--   0        0        0     1770 2023-07-08 20:30:49.831042 popcornshow-0.1.2/popcorn/models/SourceAdPlacement.py
+-rw-r--r--   0        0        0      161 2023-07-08 19:58:56.386939 popcornshow-0.1.2/popcorn/models/Streamability.py
+-rw-r--r--   0        0        0      183 2023-07-08 19:58:56.386939 popcornshow-0.1.2/popcorn/models/Tag.py
+-rw-r--r--   0        0        0      206 2023-07-08 19:58:56.386939 popcornshow-0.1.2/popcorn/models/Trailer.py
+-rw-r--r--   0        0        0     3452 2023-03-25 22:50:45.329984 popcornshow-0.1.2/popcorn/models/TVShowEpisode.py
+-rw-r--r--   0        0        0     1951 2023-07-17 02:03:01.019953 popcornshow-0.1.2/popcorn/tables/people.py
+-rw-r--r--   0        0        0     5478 2023-07-17 02:03:01.019953 popcornshow-0.1.2/popcorn/tables/sources.py
+-rw-r--r--   0        0        0     1473 2023-07-17 02:03:01.020951 popcornshow-0.1.2/popcorn/tables/table_details_movie.py
+-rw-r--r--   0        0        0     1221 2023-07-17 02:03:01.020951 popcornshow-0.1.2/popcorn/tables/table_person.py
+-rw-r--r--   0        0        0     1329 2023-07-25 01:42:47.556228 popcornshow-0.1.2/popcorn/tables/table_search.py
+-rw-r--r--   0        0        0     1243 2023-07-08 20:30:49.846667 popcornshow-0.1.2/popcorn/tables/tableDetailsShow.py
+-rw-r--r--   0        0        0      357 2023-07-08 19:58:56.418205 popcornshow-0.1.2/popcorn/tables/TableInterface.py
+-rw-r--r--   0        0        0     2154 2023-07-25 01:45:56.245154 popcornshow-0.1.2/popcorn/utils.py
+-rw-r--r--   0        0        0     1672 2023-07-25 02:40:44.263427 popcornshow-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2287 2023-07-22 21:17:14.185532 popcornshow-0.1.2/README.md
+-rw-r--r--   0        0        0     3131 1970-01-01 00:00:00.000000 popcornshow-0.1.2/PKG-INFO
```

### Comparing `popcornshow-0.1.1/popcorn/api/api.py` & `popcornshow-0.1.2/popcorn/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     )
     if result.status_code == requests.codes.ok:
         return Result(value=result.text)
     else:
         return Result(error=Exception(result.content))
 
 
-def getMovieApi(id: str) -> Result:
+def get_movie_api(id: str) -> Result:
     """
     Busca por informações da filme, retornando um json
     Parameters:
         id: texto com ID completo de um filme
     Returns:
         Retorna um object Result onde se tem objetos internos, como value contento o json do resultado
     Exemplos:
@@ -116,15 +116,15 @@
     result = requests.get(f"https://api.reelgood.com/v3.0/content/movie/{id}")
     if result.status_code == requests.codes.ok:
         return Result(value=result.text)
     else:
         return Result(error=Exception(result.content))
 
 
-def getTvShowApi(id: str) -> Result:
+def get_tvshow_api(id: str) -> Result:
     """
     Busca por informações da série, retornando um json
     Parameters:
         id: texto com ID completo de um Série
     Returns:
         Retorna um object Result onde se tem objetos internos, como value contento o json do resultado
     Exemplos:
```

### Comparing `popcornshow-0.1.1/popcorn/api/models/SearchApi.py` & `popcornshow-0.1.2/popcorn/api/models/SearchApi.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/cli.py` & `popcornshow-0.1.2/popcorn/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,78 +6,78 @@
 from rich.prompt import Prompt
 from rich.table import Table
 from rich.tree import Tree
 
 from popcorn.api.models.PersonApi import PersonApi
 from popcorn.api.models.Result import Result
 from popcorn.api.models.SearchApi import Item
-from popcorn.controller import person_reel, searchReel, transformItem
+from popcorn.controller import person_reel, search_reel, transform_item
 from popcorn.models.ItemMovie import ItemMovie
 from popcorn.models.ItemShow import ItemShow
 from popcorn.models.Person import Person
 from popcorn.models.Search import Search
 from popcorn.tables.people import people, people_biography, person_media
-from popcorn.tables.sources import columns, columnsSeasons
+from popcorn.tables.sources import collumn_seasons, pop_collumns
 from popcorn.tables.table_details_movie import table_details
 from popcorn.tables.table_person import table_details_person
-from popcorn.tables.table_search import tableSearch
+from popcorn.tables.table_search import table_search
 from popcorn.tables.tableDetailsShow import table_details_show
-from popcorn.utils import formatDate
+from popcorn.utils import format_date
 
 app = typer.Typer(help="PopCorn Show")
 console = Console()
 
 
 @app.command(name="search")
 def search(
     name: str,
     year: int = typer.Option(None, "--year", "-y", help="type Year"),
     type: str = typer.Option(None, "--type", "-t", help="'m' or 's'"),
     luck: bool = typer.Option(False, "--luck", "-l"),
 ):
-    list = searchReel(name, year=year, type=type)
+    list = search_reel(name, year=year, type=type)
     if list:
         if luck:
-            order = sorted(list, key=lambda x: x.imdbStr(), reverse=True)
-            result = transformItem(order[0].slug, order[0].type)
-            chooseTypes(result)
+            order = sorted(list, key=lambda x: x.imdb_str(), reverse=True)
+            result = transform_item(order[0].slug, order[0].type)
+            choose_types(result)
         else:
-            console.print(tableSearch(list))
-            chooseNumber(list)
+            console.print(table_search(list))
+            choose_number(list)
     else:
         typer.echo("Not Found")
 
 
 def person(name: str):
     result: Result = person_reel(name)
     if result.error is None:
-        __showPerson(result.value)
+        __show_person(result.value)
     else:
         console.print(result.error)
 
 
-def chooseTypes(result: Result):
+def choose_types(result: Result):
     if result.error:
         console.print(result.error)
     else:
-        fillByType(result)
+        fill_by_type(result)
 
 
-def fillByType(result: Result):
+def fill_by_type(result: Result):
     if isinstance(result.value, ItemMovie):
-        __showMovie(result.value)
+        __show_movie(result.value)
     elif isinstance(result.value, ItemShow):
-        __showTvshow(result.value)
+        __show_tvshow(result.value)
 
 
-def __showTvshow(show: ItemShow):
+def __show_tvshow(show: ItemShow):
     tree = Tree("")
     tree.add(__rich__())
     details = Tree(
-        f":blue_book: [blue][b]Details - {show.title} {formatDate(show.released_on).year}[/b] - :link: [blue][link={show.createUrl()}]Details in Reelgood.com[/link]",
+        f":blue_book: [blue][b]Details - {show.title} {format_date(show.released_on).year}[/b] - :link: [blue][link={show.createUrl()}]Details in Reelgood.com[/link]",
         expanded=True,
     )
     details.add(table_details_show(show), highlight=False)
 
     person = Tree(":busts_in_silhouette:[bold][purple] People")
     person.add(people(show.people))
 
@@ -85,69 +85,69 @@
     if person.children.__len__() > 0:
         tree.add(person)
     if show.seasons.__len__() > 0:
         tv = Tree(
             f":movie_camera: [red][b]Where to Watch: {show.title} [/red]| [yellow]With Season {show.seasons.__len__()}"
         )
         tv.add(
-            columnsSeasons(show.episodes, reversed(show.seasons)),
+            collumn_seasons(show.episodes, reversed(show.seasons)),
             expanded=True,
             highlight=False,
         )
         tree.add(tv)
     tree.add(__footer__(show))
     console.print(tree)
 
     if show.people.__len__() > 0:
-        __choosePerson(show.people)
+        __choose_person(show.people)
 
 
-def __showMovie(movie: ItemMovie):
+def __show_movie(movie: ItemMovie):
     tree = Tree("")
     tree.add(__rich__())
     details = Tree(
-        f":blue_book:[blue][b] Details - {movie.title} {formatDate(movie.released_on).year if formatDate(movie.released_on) != None else '-- --'}[/b] - :link: [blue][link={movie.createUrl()}]Details in Reelgood.com[/link]",
+        f":blue_book:[blue][b] Details - {movie.title} {format_date(movie.released_on).year if format_date(movie.released_on) != None else '-- --'}[/b] - :link: [blue][link={movie.create_url()}]Details in Reelgood.com[/link]",
         expanded=True,
     )
     details.add(table_details(movie), highlight=False)
 
     person = Tree(":busts_in_silhouette:[bold][purple] People")
     person.add(people(movie.people))
 
     tree.add(details)
     if person.children.__len__() > 0:
         tree.add(person)
     if movie.availability:
         tv = Tree(f":movie_camera:[red][b] Where to Watch: {movie.title}")
-        tv.add(columns(movie.availability), expanded=True, highlight=False)
+        tv.add(pop_collumns(movie.availability), expanded=True, highlight=False)
         tree.add(tv)
     tree.add(__footer__(movie))
     console.print(tree)
     if movie.people.__len__() > 0:
-        __choosePerson(movie.people)
+        __choose_person(movie.people)
 
 
-def __choosePerson(list: list[Person]):
+def __choose_person(list: list[Person]):
     number = Prompt.ask(
         "[blue]Enter the person's number between 1 to "
         + f"{1 if list.__len__() == 1 else list.__len__()} "
         + "for details - Zero to exit\n"
     )
     try:
         value = int(number)
         if value < 1:
             return
         people = list[value - 1]
         person(people["slug"])
         return
     except (TypeError, ValueError, IndexError):
-        __choosePerson(list)
+        __choose_person(list)
 
 
-def __showPerson(person: PersonApi):
+def __show_person(person: PersonApi):
     tree = Tree("")
     tree.add(__rich__())
     tree.add(table_details_person(person), highlight=False)
     if person.biography is not None:
         tree.add(people_biography(person.biography))
     if person.initial_credits.__len__() > 0:
         tree.add(person_media(person.initial_credits))
@@ -166,16 +166,16 @@
         + "[red]for details - Zero to exit\n"
     )
     try:
         value = int(number)
         if value < 1:
             return
         item: Item = person.initial_credits[value - 1]
-        media: Result = transformItem(item["slug"], item["content_type"])
-        chooseTypes(media)
+        media: Result = transform_item(item["slug"], item["content_type"])
+        choose_types(media)
     except (IndexError, ValueError):
         choose_media_by_person(person)
 
 
 def __rich__() -> Panel:
     grid = Table.grid(expand=True)
     grid.add_column(justify="center", ratio=1)
@@ -214,32 +214,32 @@
         grid.add_row(
             "",
             f"[b][link=https://play.google.com/store/apps/details?id=br.com.icaro.filme][yellow]App Android => [/link]",
         )
     return Panel(grid, style="red1 on black")
 
 
-def chooseNumber(list: list[Search], hasError=False):
+def choose_number(list: list[Search], hasError=False):
     item: None
     number = Prompt.ask(
         f"[red]For details, write a number between 1 and {list.__len__()}. Zero to exit\n"
     )
     if hasError or number == "0":
         return
 
     try:
         number = int(number)
         if number > 0 and number <= list.__len__():
             item = list[number - 1]
         else:
             print("Number off the list.")
-            chooseNumber(list, True)
+            choose_number(list, True)
             return
 
     except ValueError:
         print("Number Error! - write '0' to exit ")
-        chooseNumber(list, True)
+        choose_number(list, True)
         return
 
     if item is not None:
-        result = transformItem(item.slug, item.type)
-        fillByType(result)
+        result = transform_item(item.slug, item.type)
+        fill_by_type(result)
```

### Comparing `popcornshow-0.1.1/popcorn/controller.py` & `popcornshow-0.1.2/popcorn/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-from popcorn.api.api import get_person_details, getMovieApi, getTvShowApi, search
+from popcorn.api.api import get_movie_api, get_person_details, get_tvshow_api, search
 from popcorn.api.models.PersonApi import PersonApi
 from popcorn.api.models.Result import Result
 from popcorn.api.models.SearchApi import ContentType
 from popcorn.dto import format_list
 from popcorn.models.ItemMovie import ItemMovie
 from popcorn.models.ItemShow import ItemShow
 from popcorn.models.Search import Search
@@ -13,15 +13,15 @@
 
 def search_reel(query: str, year: int | None, type: str | None) -> list[Search]:
     result: Result = search(query=query)
     if result.error is None:
         objJson = json.loads(result.value)
         if objJson["items"].__len__() == 0:
             return []
-        listSearch = filtersArgs(objJson["items"], year, type)
+        listSearch = filters_args(objJson["items"], year, type)
         return format_list(listSearch)
     else:
         []
 
 
 def person_reel(id) -> Result:
     result = get_person_details(id)
@@ -30,45 +30,47 @@
     else:
         return Result(Exception("Match not Found..."))
 
 
 def transform_item(slug: str, type: str) -> Result:
     match type:
         case ContentType.M.value:
-            movie = getMovieApi(slug)
+            movie = get_movie_api(slug)
             if movie.error is None:
                 return Result(value=ItemMovie(**json.loads(movie.value)))
             else:
                 return Result(Exception("Match not Found..."))
         case ContentType.S.value:
-            tv = getTvShowApi(slug)
+            tv = get_tvshow_api(slug)
             if tv.error is None:
                 return Result(value=ItemShow(**json.loads(tv.value)))
             else:
                 return Result(Exception("Match not Found..."))
         case _:
             return Result(Exception("Match not Found..."))
 
 
-def filterByYear(item, year) -> bool:
+def filter_by_year(item, year) -> bool:
     if item["released_on"] == None:
         return True
     return format_date(item["released_on"]).year == year
 
 
-def filterByType(item, type) -> bool:
+def filter_by_type(item, type) -> bool:
     if item["content_type"] == None:
         return True
     return item["content_type"] == type
 
 
-def filtersArgs(items: list[any], year: int | None, type: str | None):
+def filters_args(items: list[any], year: int | None, type: str | None):
     if year == None and type == None:
         return items
     if year != None and type == None:
-        return list(filter(lambda x: (filterByYear(x, year)), items))
+        return list(filter(lambda x: (filter_by_year(x, year)), items))
     if year == None and type != None:
-        return list(filter(lambda x: (filterByType(x, type)), items))
+        return list(filter(lambda x: (filter_by_type(x, type)), items))
     if year != None and type != None:
         return list(
-            filter(lambda x: (filterByType(x, type) and filterByYear(x, year)), items)
+            filter(
+                lambda x: (filter_by_type(x, type) and filter_by_year(x, year)), items
+            )
         )
```

### Comparing `popcornshow-0.1.1/popcorn/dto.py` & `popcornshow-0.1.2/popcorn/dto.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/models/Creative.py` & `popcornshow-0.1.2/popcorn/models/Creative.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/models/ItemMovie.py` & `popcornshow-0.1.2/popcorn/models/ItemMovie.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,18 @@
 from popcorn.models.ReelgoodScores import ReelgoodScores
 from popcorn.models.RegionalAvailability import RegionalAvailability
 from popcorn.models.ScoreBreakdown import ScoreBreakdown
 from popcorn.models.SourceAdPlacement import SourceAdPlacement
 from popcorn.models.Tag import Tag
 from popcorn.models.Trailer import Trailer
 from popcorn.tables.TableInterface import TableInterface
-from popcorn.utils import createUrl as fullUrl
-from popcorn.utils import (
-    filterTrailerByService,
-    format_date,
-    formatSources,
-    formatTrailers,
-)
+from popcorn.utils import create_url as full_urls
+from popcorn.utils import filterTrailerByService, format_date
+from popcorn.utils import format_sources as format_sources_util
+from popcorn.utils import format_trailers
 
 
 class References:
     web: Ios
     ios: Ios
     android: Optional[Ios]
     webos: Optional[Ios]
@@ -210,54 +207,54 @@
     def get_overview(self):
         return self.overview
 
     def get_date(self) -> str:
         return self.format_date()
 
     def get_time(self) -> str:
-        return self.formatTime()
+        return self.format_time()
 
     def get_imdb(self) -> str:
-        return self.imdbStr()
+        return self.imdb_str()
 
     def get_classification(self) -> str:
         return (
             f"[b][white]{self.classification}" if self.classification else "Who knows"
         )
 
     def get_trailers(self) -> str:
-        return self.getListTrailers()
+        return self.get_list_trailers()
 
     def format_date(self) -> str:
         return (
             str(format_date(self.released_on).date())
             if self.released_on is not None
             else "-- --"
         )
 
-    def formatTime(self) -> str:
+    def format_time(self) -> str:
         if self.runtime is not None:
             hours, minutes = divmod(self.runtime, 60)
             return f"{hours}h {minutes}m"
         else:
             return "-- --"
 
-    def getListTrailers(self) -> str:
+    def get_list_trailers(self) -> str:
         if self.trailer is not None:
             self.trailers.append(self.trailer)
-            return formatTrailers(filterTrailerByService(self.trailers))
+            return format_trailers(filterTrailerByService(self.trailers))
         else:
             search = self.slug.replace("-", "+")
             return f"[bold blue][link=https://www.youtube.com/results?search_query={search}]Search Youtube[/link]"
 
-    def formatSources(self) -> str:
+    def format_sources(self) -> str:
         values = list(map(lambda x: x["source_name"], self.availability))
-        return formatSources(values)
+        return format_sources_util(values)
 
-    def createUrl(self):
-        return fullUrl("m", self.slug)
+    def create_url(self):
+        return full_urls("m", self.slug)
 
-    def imdbStr(self) -> str:
+    def imdb_str(self) -> str:
         if self.imdb_rating != None:
             return str(self.imdb_rating)
         else:
             return "-.-"
```

### Comparing `popcornshow-0.1.1/popcorn/models/ItemShow.py` & `popcornshow-0.1.2/popcorn/models/ItemShow.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from popcorn.models.ScoreBreakdown import ScoreBreakdown
 from popcorn.models.Seasons import Season
 from popcorn.models.SourceAdPlacement import SourceAdPlacement
 from popcorn.models.Tag import Tag
 from popcorn.models.Trailer import Trailer
 from popcorn.models.TVShowEpisode import TVShowEpisode
 from popcorn.tables.TableInterface import TableInterface
-from popcorn.utils import createUrl as fullUrl
-from popcorn.utils import filterTrailerByService, format_date, formatTrailers
+from popcorn.utils import create_url as full_url
+from popcorn.utils import filterTrailerByService, format_date, format_trailers
 
 
 @dataclass
 class Android:
     episode_id: str
 
     @staticmethod
@@ -241,15 +241,15 @@
         self.rating_stats = rating_stats
         self.reviews_count = reviews_count
 
     def get_number_seasons(self):
         return str(self.season_count)
 
     def createUrl(self):
-        return fullUrl("s", self.slug)
+        return full_url("s", self.slug)
 
     def get_overview(self):
         return self.overview
 
     def get_date(self) -> str:
         return self.format_date()
 
@@ -266,15 +266,15 @@
 
     def get_trailers(self) -> str:
         return self.getListTrailers()
 
     def getListTrailers(self) -> str:
         if self.trailer is not None:
             self.trailers.append(self.trailer)
-            return formatTrailers(filterTrailerByService(self.trailers))
+            return format_trailers(filterTrailerByService(self.trailers))
         else:
             search = self.slug.replace("-", "+")
             return f"[bold blue][link=https://www.youtube.com/results?search_query={search}]Search Youtube[/link]"
 
     def format_date(self) -> str:
         return (
             str(format_date(self.released_on).date())
```

### Comparing `popcornshow-0.1.1/popcorn/models/Person.py` & `popcornshow-0.1.2/popcorn/models/Person.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/models/ReelgoodScores.py` & `popcornshow-0.1.2/popcorn/models/ReelgoodScores.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/models/RegionalAvailability.py` & `popcornshow-0.1.2/popcorn/models/RegionalAvailability.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/models/Seasons.py` & `popcornshow-0.1.2/popcorn/models/Seasons.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/models/SourceAdPlacement.py` & `popcornshow-0.1.2/popcorn/models/SourceAdPlacement.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/models/TVShowEpisode.py` & `popcornshow-0.1.2/popcorn/models/TVShowEpisode.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/tables/people.py` & `popcornshow-0.1.2/popcorn/tables/people.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/tables/sources.py` & `popcornshow-0.1.2/popcorn/tables/sources.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/tables/table_details_movie.py` & `popcornshow-0.1.2/popcorn/tables/table_details_movie.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/tables/table_person.py` & `popcornshow-0.1.2/popcorn/tables/table_person.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/tables/table_search.py` & `popcornshow-0.1.2/popcorn/tables/table_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 def table_search(items: list[Search]) -> Table:
     table = __init_table__()
     for index, item in enumerate(items):
         __tableItem__(
             table=table,
             id=str(index + 1),
             title=f"[white]{item.title}[/white]",
-            release=item.formatSimpleDateStr(),
-            type=item.formatLongType(),
-            imdb=item.imdbStr(),
-            online=item.formatOnline(),
-            url=item.createUrl(),
+            release=item.format_simple_date_str(),
+            type=item.format_long_type(),
+            imdb=item.imdb_str(),
+            online=item.format_online(),
+            url=item.create_url(),
         )
     return table
 
 
 def __tableItem__(
     table: Table,
     id: int,
```

### Comparing `popcornshow-0.1.1/popcorn/tables/tableDetailsShow.py` & `popcornshow-0.1.2/popcorn/tables/tableDetailsShow.py`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/popcorn/utils.py` & `popcornshow-0.1.2/popcorn/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,78 +10,69 @@
     try:
         formatDate = date[:19]
         return datetime.strptime(formatDate, "%Y-%m-%dT%H:%M:%S")
     except:
         return None
 
 
-def format_full_date(date: str | None) -> datetime | str:
-    if date is None:
-        return "- -"
-    try:
-        return datetime.strptime(date, "%Y-%m-%dT%H:%M:%S")
-    except ValueError:
-        return "- -"
-
-
 def format_date_str(date: str | None) -> str:
     if date is None:
         return "--"
 
     try:
         formatDate = date[:19]
         return str(datetime.strptime(formatDate, "%Y-%m-%dT%H:%M:%S").date())
     except:
         return "-- -- --"
 
 
-def createUrl(type: str, url: str) -> str:
+def create_url(type: str, url: str) -> str:
     if type == "m":
         return URL_BASE + "movie" + "/" + url
     else:
         return URL_BASE + "show" + "/" + url
 
 
-def formatType(type: chr) -> str:
+def format_type(type: chr) -> str:
     if type == "m":
         return "Movie"
     elif type == "s":
         return "Show"
     else:
         return "- -"
 
 
 def format_source(item: str) -> str:
     return item.replace("_", " ").title()
 
 
-def formatSources(sources: list[str]) -> str:
+def format_sources(sources: list[str]) -> str:
     result = ""
-    br = __hasBr(sources.__len__())
+    br = has_br(sources.__len__())
     sources = remove_dash(sources=sources)
     for index, source in enumerate(sources):
         result = result + source + (br if index != sources.__len__() - 1 else "")
     return result
 
 
 def remove_dash(sources: list[str]) -> list[str]:
     result = []
     for source in map(lambda x: x.replace("_", " ").capitalize(), sources):
         result.append(source)
     return result
 
 
-def __hasBr(length: int):
+def has_br(length: int):
     if length >= 15:
         return "\n"
     else:
         return " - "
 
 
-def formatTrailers(trailers: list[Trailer]) -> str:
+def format_trailers(trailers: list[Trailer]) -> str:
     result = ""
     values = set(map(lambda x: x["key"], trailers))
     for index, value in enumerate(values):
         result = (
             result
             + f":link: [bold blue][link=https://youtu.be/{value}]Trailer - {index + 1}[/link][/bold blue]\n"
         )
```

### Comparing `popcornshow-0.1.1/pyproject.toml` & `popcornshow-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "popcornshow"
 packages = [{include = "popcorn"}]
-version = "0.1.1"
+version = "0.1.2"
 description = "Show information about movie and movies"
 authors = ["Icaro Nunes <icarornunes@gmail.com>"]
 license = "BeerWare"
 readme = "README.md"
 classifiers = [
   "Topic :: Utilities",
   "Programming Language :: Python :: 3"
```

### Comparing `popcornshow-0.1.1/README.md` & `popcornshow-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `popcornshow-0.1.1/PKG-INFO` & `popcornshow-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popcornshow
-Version: 0.1.1
+Version: 0.1.2
 Summary: Show information about movie and movies
 License: Beerware
 Author: Icaro Nunes
 Author-email: icarornunes@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

