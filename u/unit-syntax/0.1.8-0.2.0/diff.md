# Comparing `tmp/unit_syntax-0.1.8.tar.gz` & `tmp/unit_syntax-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_syntax-0.1.8.tar", max compression
+gzip compressed data, was "unit_syntax-0.2.0.tar", max compression
```

## Comparing `unit_syntax-0.1.8.tar` & `unit_syntax-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5284 2023-07-13 20:16:38.757753 unit_syntax-0.1.8/README.md
--rw-r--r--   0        0        0      641 2023-07-13 20:16:38.761753 unit_syntax-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2048 2023-07-13 20:16:38.761753 unit_syntax-0.1.8/unit_syntax/__init__.py
--rw-r--r--   0        0        0   149629 2023-07-13 20:16:38.761753 unit_syntax-0.1.8/unit_syntax/parser.py
--rw-r--r--   0        0        0     5039 2023-07-13 20:16:38.761753 unit_syntax-0.1.8/unit_syntax/transform.py
--rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 unit_syntax-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     4894 2023-07-25 01:01:25.036554 unit_syntax-0.2.0/README.md
+-rw-r--r--   0        0        0      644 2023-07-25 01:01:25.036554 unit_syntax-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2104 2023-07-25 01:01:25.036554 unit_syntax-0.2.0/unit_syntax/__init__.py
+-rw-r--r--   0        0        0   149661 2023-07-25 01:01:25.036554 unit_syntax-0.2.0/unit_syntax/parser.py
+-rw-r--r--   0        0        0     5039 2023-07-25 01:01:25.036554 unit_syntax-0.2.0/unit_syntax/transform.py
+-rw-r--r--   0        0        0     5570 1970-01-01 00:00:00.000000 unit_syntax-0.2.0/PKG-INFO
```

### Comparing `unit_syntax-0.1.8/README.md` & `unit_syntax-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-`unit-syntax` extends the Python language in Jupyter/IPython to support expressions with physical units:
+`unit-syntax` adds support for physical units to the Python language:
 
 ```python
 >>> speed = 5 meters/second
 >>> (2 seconds) * speed
 10 meter
 ```
 
-Behind the scenes this is translated into standard Python that uses the excellent [Pint](https://pint.readthedocs.io/) units library.
+Why? I often use Python as an interactive calculator for physical problems, and wished it had the type safety of explicit units along with the readability of normal notation.
+
+Where? `unit-syntax` currently supports Jupyter notebooks and the IPython interpreter; support for standalone scripts is planned.
+
+How? A syntax transformer based on the official Python grammar turns these expression into calls to the excellent [Pint](https://pint.readthedocs.io/) units library.
 
 ## Getting Started
 
 Install the package:
 
 ```shell
 $ pip install unit-syntax
@@ -19,96 +23,80 @@
 To enable unit-syntax in a Jupyter/IPython session run:
 
 ```python
 import unit_syntax
 unit_syntax.enable_ipython()
 ```
 
-Note: in Jupyter this must be run in its own cell before any units expressions are evaluated.
+Tip: In Jupyter this must be run in its own cell before any units expressions are evaluated.
 
 ## Usage
 
 [An interactive notebook to play around with units](https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV)
 
-Units apply to the immediately preceding value:
+Units can be applied to any "simple" expression:
 
-```python
-1.21 gigawatts # literal number
-(30 + 7) watts # parenthesized expression
-[5, 7] meters # literal list
-(9, 11) lumens # literal tuple
-# variable reference
-y becquerel
-position.x attoparsec
-velocity[player_id] meters/s
-```
+- number: `1 meter`
+- variables: `x parsec`, `y.z watts`, `area[id] meters**2`
+- lists and tuples: `[1., 37.] newton meters`
+- unary operators: `-x dBm`
+- power: `x**2 meters`
 
-Units are parsed greedily and bind only to the immediately preceding value:
+To apply units within a more complex expression, use parentheses:
 
 ```python
-x * 5 meters # x * (5 meters), not (x*5) meters
+one_lux = (1 lumen)/(1 meter**2)
 ```
 
+Units can be used in other places where Python allows expressions like:
+
+- function arguments: `area_of_circle(radius=1 meter)`
+- list comprehensions: `[x meters for x in range(10)]`
+
 Quantities can be converted to another measurement system:
 
 ```python
 >>> (88 miles / hour) furlongs / fortnight
 236543.5269120001 furlong / fortnight
 >>> (0 degC) degF
 31.999999999999936 degree_Fahrenheit
 ```
 
-It's _highly_ recommended to parenthesize any complex that include units. For example:
-
-```python
-1 meters * sin(degrees)
-```
-
-This is desugared to `Quantity(1, "meters * sin(degrees)")`, when you probably wanted `(1 meters) * sin(degrees)`.
+Compound units (e.g. `newtons/meter**2`) are supported and follow the usual precedence rules.
 
 Units _may not_ begin with parentheses (consider the possible
 interpretations of `x (meters)`). Parentheses are allowed anywhere else:
 
 ```python
-x (newton meters)/(second*kg) # parsed as a function call, will result in a runtime error
-x newton meters/(second*kg) # ok
+# parsed as a function call, will result in a runtime error
+x (newton meters)/(second*kg)
+# a-ok
+x newton meters/(second*kg)
 ```
 
-## Syntax Details
+## Why only allow units on simple expressions?
 
-The full grammar for units is:
+The rule for applying units only to "simple" expressions rather than treating it as a typical operator is to avoid unintentional error. Imagine units were instead parsed as operator with high precedence and you wrote this reasonable looking expression:
 
-```
-units:
-    | units '/' units_group
-    | units '*' units_group
-    | units units_group
-    | units '**' NUMBER
-    | NAME
-
-units_group:
-    | '(' units ')'
-    | units
+```python
+ppi = 300 pixels/inch
+y = x inches * ppi
 ```
 
-Compound units allow the usual operators multiplication, division, and exponentiation with the usual precedence rules. Adjacent units without an operator are treated as multiplication.
+`inches * ppi` would be parsed as the unit, leading to (at best) a runtime error sometime later and at worst an incorrect calculation. This could be avoided by parenthesizing the expression (e.g. `(x inches) * ppi`, but in general it's too error prone to allow free intermixing of operators and units. (Note: This is not a hypoethical concern, I hit this within 10 minutes of first trying out the idea)
 
 ## Help!
 
-If you're getting an unexpected result, try using `unit_syntax.enable_ipython(debug_transform=True)`. This will log the transformed python code to the console.
-
-## Why? How? Are you sure this a good idea?
+If you're getting an unexpected result, try using `unit_syntax.enable_ipython(debug_transform=True)`. This will log the transformed Python code to the console.
 
-I like using Python with [Jupyter Notebook](https://jupyter.org/) as a calculator for physical problems and often wish it had the clarity and type checking of explicit units. [Pint](https://pint.readthedocs.io/) is great, but its (necessary) verbosity makes it hard to see the underlying calculation that's going. Ultimately I want something that is as readable as what I'd write on paper using normal notation.
+If you're stuck, feel free to open an issue.
 
-`unit-syntax` is an IPython [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`. The parser is a lightly modified version of the Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself.
+## How does it work?
 
-Should you use this? There are tradeoffs. When using unit-syntax as an interactive calculator the clarity of explicit units improves both readability and correctness. However, the new syntax also introduces _new_ opportunities for error if an expression is parsed in an unexpected way. Usually this is obvious when used interactively, but it's something to be aware of.
-
-`unit-syntax` cannot (currently) be used for standalone python scripts outside of IPython/Jupyter, but that's in principle possible through [meta_path import hooks](https://docs.python.org/3/reference/import.html#the-meta-path).
+The parser is derived from the official Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself. The transformer hooks into IPython/Jupyter using [custom input transformers](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html).
 
 ## Prior Art
 
 The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf) from Sun Microsystems. Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
 
 F# (an OCaml derivative from Microsoft) also [has first class support for units](https://en.wikibooks.org/wiki/F_Sharp_Programming/Units_of_Measure).
 
@@ -121,26 +109,22 @@
 To regenerate the parser:
 
 `python -m pegen grammar.txt -o unit_syntax/parser.py`
 
 Running tests:
 
 ```
-
 $ poetry install --with dev
 $ poetry run pytest
-
 ```
 
 ## Future work and open questions
 
 - Test against various ipython and python versions
 - Support standalone scripts through sys.meta_path
 - Check units at parse time
 - Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
 - Expand the demo Colab notebook
 - Typography of output
-- Its too easy to get an unexpected parse if you forget parentheses.
-
-```
-
-```
+- make it work with numba
+- understand how numpy interop works
+- fail more clearly when units are used in an invalid location
```

### Comparing `unit_syntax-0.1.8/unit_syntax/__init__.py` & `unit_syntax-0.2.0/unit_syntax/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,28 +37,32 @@
         do_transform = transform_lines
     ip.input_transformers_post.append(do_transform)
 
     # Overide default formatters to use reduced units.  This lets us keep using the
     # default registry for interop with other pint-using libraries, but gives more
     # sensible output in the notebook.
     def add_formatter(mime, display_fn_name):
-        formatter = ip.display_formatter.formatters.get(mime)
-        if formatter is None:
-            return
-
         fn = getattr(pint.Quantity, display_fn_name, None)
         if fn is None:
             return
 
         def fmt_reduced(q, *args):
             return fn(q.to_reduced_units(), *args)
 
+        formatter = ip.display_formatter.formatters[mime]
         formatter.for_type(pint.Quantity, fmt_reduced)
 
     add_formatter("text/markdown", "_repr_markdown_")
     add_formatter("text/html", "_repr_html_")
     add_formatter("text/plain", "_repr_pretty_")
     add_formatter("text/latex", "_repr_latex_")
 
     # ensure the module is still visible if imported via
     # `from unit_syntax import ipython` for some reason
     ip.run_cell("import unit_syntax")
+
+    try:
+        import matplotlib
+
+        pint.setup_matplotlib(True)
+    except ImportError:
+        pass
```

### Comparing `unit_syntax-0.1.8/unit_syntax/parser.py` & `unit_syntax-0.2.0/unit_syntax/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1641,17 +1641,22 @@
         ):
             return expression;
         self._reset(mark)
         return None;
 
     @memoize
     def expression(self) -> Optional[Any]:
-        # expression: disjunction 'if' disjunction 'else' expression | disjunction | lambdef
+        # expression: factor_with_units | disjunction 'if' disjunction 'else' expression | disjunction | lambdef
         mark = self._mark()
         if (
+            (factor_with_units := self.factor_with_units())
+        ):
+            return factor_with_units;
+        self._reset(mark)
+        if (
             (disjunction := self.disjunction())
             and
             (literal := self.expect('if'))
             and
             (disjunction_1 := self.disjunction())
             and
             (literal_1 := self.expect('else'))
@@ -2271,17 +2276,30 @@
         if (
             (sum := self.sum())
         ):
             return sum;
         self._reset(mark)
         return None;
 
+    @memoize
+    def factor_with_units(self) -> Optional[Any]:
+        # factor_with_units: factor units
+        mark = self._mark()
+        if (
+            (p := self.factor())
+            and
+            (u := self.units())
+        ):
+            return ( 'value_with_units' , p , u );
+        self._reset(mark)
+        return None;
+
     @memoize_left_rec
     def units(self) -> Optional[Any]:
-        # units: units '/' units_group | units '*' units_group | units units_group | units '**' NUMBER | units '^' NUMBER | NAME
+        # units: units '/' units_group | units '*' units_group | units units_group | units '**' NUMBER | NAME
         mark = self._mark()
         if (
             (units := self.units())
             and
             (literal := self.expect('/'))
             and
             (units_group := self.units_group())
@@ -2310,23 +2328,14 @@
             (literal := self.expect('**'))
             and
             (number := self.number())
         ):
             return [units, literal, number];
         self._reset(mark)
         if (
-            (units := self.units())
-            and
-            (literal := self.expect('^'))
-            and
-            (number := self.number())
-        ):
-            return [units, literal, number];
-        self._reset(mark)
-        if (
             (name := self.name())
         ):
             return name;
         self._reset(mark)
         return None;
 
     @memoize
@@ -2464,33 +2473,26 @@
         ):
             return power;
         self._reset(mark)
         return None;
 
     @memoize
     def power(self) -> Optional[Any]:
-        # power: await_primary '**' factor | await_primary units | await_primary
+        # power: await_primary '**' factor | await_primary
         mark = self._mark()
         if (
             (await_primary := self.await_primary())
             and
             (literal := self.expect('**'))
             and
             (factor := self.factor())
         ):
             return [await_primary, literal, factor];
         self._reset(mark)
         if (
-            (a := self.await_primary())
-            and
-            (u := self.units())
-        ):
-            return ( 'value_with_units' , a , u );
-        self._reset(mark)
-        if (
             (await_primary := self.await_primary())
         ):
             return await_primary;
         self._reset(mark)
         return None;
 
     @memoize
```

### Comparing `unit_syntax-0.1.8/unit_syntax/transform.py` & `unit_syntax-0.2.0/unit_syntax/transform.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.1.8/PKG-INFO` & `unit_syntax-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: unit-syntax
-Version: 0.1.8
+Version: 0.2.0
 Summary: Physical unit literals for Jupyter and IPython
 Home-page: https://github.com/ahupp/unit-syntax
 Author: Adam Hupp
 Author-email: adam@hupp.org
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pint (>=0.20,<0.21)
+Requires-Dist: Pint (>0.20)
 Requires-Dist: ipython (>=7)
 Requires-Dist: pegen (>=0.2,<0.3)
 Project-URL: Repository, https://github.com/ahupp/unit-syntax
 Description-Content-Type: text/markdown
 
-`unit-syntax` extends the Python language in Jupyter/IPython to support expressions with physical units:
+`unit-syntax` adds support for physical units to the Python language:
 
 ```python
 >>> speed = 5 meters/second
 >>> (2 seconds) * speed
 10 meter
 ```
 
-Behind the scenes this is translated into standard Python that uses the excellent [Pint](https://pint.readthedocs.io/) units library.
+Why? I often use Python as an interactive calculator for physical problems, and wished it had the type safety of explicit units along with the readability of normal notation.
+
+Where? `unit-syntax` currently supports Jupyter notebooks and the IPython interpreter; support for standalone scripts is planned.
+
+How? A syntax transformer based on the official Python grammar turns these expression into calls to the excellent [Pint](https://pint.readthedocs.io/) units library.
 
 ## Getting Started
 
 Install the package:
 
 ```shell
 $ pip install unit-syntax
@@ -38,96 +42,80 @@
 To enable unit-syntax in a Jupyter/IPython session run:
 
 ```python
 import unit_syntax
 unit_syntax.enable_ipython()
 ```
 
-Note: in Jupyter this must be run in its own cell before any units expressions are evaluated.
+Tip: In Jupyter this must be run in its own cell before any units expressions are evaluated.
 
 ## Usage
 
 [An interactive notebook to play around with units](https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV)
 
-Units apply to the immediately preceding value:
+Units can be applied to any "simple" expression:
 
-```python
-1.21 gigawatts # literal number
-(30 + 7) watts # parenthesized expression
-[5, 7] meters # literal list
-(9, 11) lumens # literal tuple
-# variable reference
-y becquerel
-position.x attoparsec
-velocity[player_id] meters/s
-```
+- number: `1 meter`
+- variables: `x parsec`, `y.z watts`, `area[id] meters**2`
+- lists and tuples: `[1., 37.] newton meters`
+- unary operators: `-x dBm`
+- power: `x**2 meters`
 
-Units are parsed greedily and bind only to the immediately preceding value:
+To apply units within a more complex expression, use parentheses:
 
 ```python
-x * 5 meters # x * (5 meters), not (x*5) meters
+one_lux = (1 lumen)/(1 meter**2)
 ```
 
+Units can be used in other places where Python allows expressions like:
+
+- function arguments: `area_of_circle(radius=1 meter)`
+- list comprehensions: `[x meters for x in range(10)]`
+
 Quantities can be converted to another measurement system:
 
 ```python
 >>> (88 miles / hour) furlongs / fortnight
 236543.5269120001 furlong / fortnight
 >>> (0 degC) degF
 31.999999999999936 degree_Fahrenheit
 ```
 
-It's _highly_ recommended to parenthesize any complex that include units. For example:
-
-```python
-1 meters * sin(degrees)
-```
-
-This is desugared to `Quantity(1, "meters * sin(degrees)")`, when you probably wanted `(1 meters) * sin(degrees)`.
+Compound units (e.g. `newtons/meter**2`) are supported and follow the usual precedence rules.
 
 Units _may not_ begin with parentheses (consider the possible
 interpretations of `x (meters)`). Parentheses are allowed anywhere else:
 
 ```python
-x (newton meters)/(second*kg) # parsed as a function call, will result in a runtime error
-x newton meters/(second*kg) # ok
+# parsed as a function call, will result in a runtime error
+x (newton meters)/(second*kg)
+# a-ok
+x newton meters/(second*kg)
 ```
 
-## Syntax Details
+## Why only allow units on simple expressions?
 
-The full grammar for units is:
+The rule for applying units only to "simple" expressions rather than treating it as a typical operator is to avoid unintentional error. Imagine units were instead parsed as operator with high precedence and you wrote this reasonable looking expression:
 
-```
-units:
-    | units '/' units_group
-    | units '*' units_group
-    | units units_group
-    | units '**' NUMBER
-    | NAME
-
-units_group:
-    | '(' units ')'
-    | units
+```python
+ppi = 300 pixels/inch
+y = x inches * ppi
 ```
 
-Compound units allow the usual operators multiplication, division, and exponentiation with the usual precedence rules. Adjacent units without an operator are treated as multiplication.
+`inches * ppi` would be parsed as the unit, leading to (at best) a runtime error sometime later and at worst an incorrect calculation. This could be avoided by parenthesizing the expression (e.g. `(x inches) * ppi`, but in general it's too error prone to allow free intermixing of operators and units. (Note: This is not a hypoethical concern, I hit this within 10 minutes of first trying out the idea)
 
 ## Help!
 
-If you're getting an unexpected result, try using `unit_syntax.enable_ipython(debug_transform=True)`. This will log the transformed python code to the console.
-
-## Why? How? Are you sure this a good idea?
+If you're getting an unexpected result, try using `unit_syntax.enable_ipython(debug_transform=True)`. This will log the transformed Python code to the console.
 
-I like using Python with [Jupyter Notebook](https://jupyter.org/) as a calculator for physical problems and often wish it had the clarity and type checking of explicit units. [Pint](https://pint.readthedocs.io/) is great, but its (necessary) verbosity makes it hard to see the underlying calculation that's going. Ultimately I want something that is as readable as what I'd write on paper using normal notation.
+If you're stuck, feel free to open an issue.
 
-`unit-syntax` is an IPython [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`. The parser is a lightly modified version of the Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself.
+## How does it work?
 
-Should you use this? There are tradeoffs. When using unit-syntax as an interactive calculator the clarity of explicit units improves both readability and correctness. However, the new syntax also introduces _new_ opportunities for error if an expression is parsed in an unexpected way. Usually this is obvious when used interactively, but it's something to be aware of.
-
-`unit-syntax` cannot (currently) be used for standalone python scripts outside of IPython/Jupyter, but that's in principle possible through [meta_path import hooks](https://docs.python.org/3/reference/import.html#the-meta-path).
+The parser is derived from the official Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself. The transformer hooks into IPython/Jupyter using [custom input transformers](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html).
 
 ## Prior Art
 
 The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf) from Sun Microsystems. Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
 
 F# (an OCaml derivative from Microsoft) also [has first class support for units](https://en.wikibooks.org/wiki/F_Sharp_Programming/Units_of_Measure).
 
@@ -140,27 +128,23 @@
 To regenerate the parser:
 
 `python -m pegen grammar.txt -o unit_syntax/parser.py`
 
 Running tests:
 
 ```
-
 $ poetry install --with dev
 $ poetry run pytest
-
 ```
 
 ## Future work and open questions
 
 - Test against various ipython and python versions
 - Support standalone scripts through sys.meta_path
 - Check units at parse time
 - Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
 - Expand the demo Colab notebook
 - Typography of output
-- Its too easy to get an unexpected parse if you forget parentheses.
-
-```
-
-```
+- make it work with numba
+- understand how numpy interop works
+- fail more clearly when units are used in an invalid location
```

