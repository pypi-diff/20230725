# Comparing `tmp/jijmodeling-1.0.0rc3-cp39-none-win_amd64.whl.zip` & `tmp/jijmodeling-1.0.0rc4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 743481 bytes, number of entries: 8
--rw-r--r--  4.6 unx     2902 b- defN 23-Jul-13 11:16 jijmodeling-1.0.0rc3.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jul-13 11:16 jijmodeling-1.0.0rc3.dist-info/WHEEL
--rw-r--r--  4.6 unx     3445 b- defN 23-Jul-13 11:16 jijmodeling-1.0.0rc3.dist-info/license_files/LICENSE.txt
--rw-r--r--  4.6 unx      127 b- defN 23-Jul-13 11:16 jijmodeling/__init__.py
--rw-r--r--  4.6 unx   129449 b- defN 23-Jul-13 11:16 jijmodeling/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Jul-13 11:16 jijmodeling/py.typed
--rwxr-xr-x  4.6 unx  2172928 b- defN 23-Jul-13 11:16 jijmodeling/jijmodeling.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      678 b- defN 23-Jul-13 11:16 jijmodeling-1.0.0rc3.dist-info/RECORD
-8 files, 2309623 bytes uncompressed, 742297 bytes compressed:  67.9%
+Zip file size: 759942 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     2902 b- defN 23-Jul-25 12:34 jijmodeling-1.0.0rc4.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jul-25 12:34 jijmodeling-1.0.0rc4.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3445 b- defN 23-Jul-25 12:34 jijmodeling-1.0.0rc4.dist-info/license_files/LICENSE.txt
+-rw-r--r--  4.6 unx      127 b- defN 23-Jul-25 12:34 jijmodeling/__init__.py
+-rw-r--r--  4.6 unx   131169 b- defN 23-Jul-25 12:34 jijmodeling/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Jul-25 12:34 jijmodeling/py.typed
+-rwxr-xr-x  4.6 unx  2202624 b- defN 23-Jul-25 12:34 jijmodeling/jijmodeling.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      678 b- defN 23-Jul-25 12:34 jijmodeling-1.0.0rc4.dist-info/RECORD
+8 files, 2341039 bytes uncompressed, 758758 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: jijmodeling-1.0.0rc3.dist-info/METADATA
+Filename: jijmodeling-1.0.0rc4.dist-info/METADATA
 Comment: 
 
-Filename: jijmodeling-1.0.0rc3.dist-info/WHEEL
+Filename: jijmodeling-1.0.0rc4.dist-info/WHEEL
 Comment: 
 
-Filename: jijmodeling-1.0.0rc3.dist-info/license_files/LICENSE.txt
+Filename: jijmodeling-1.0.0rc4.dist-info/license_files/LICENSE.txt
 Comment: 
 
 Filename: jijmodeling/__init__.py
 Comment: 
 
 Filename: jijmodeling/__init__.pyi
 Comment: 
 
 Filename: jijmodeling/py.typed
 Comment: 
 
 Filename: jijmodeling/jijmodeling.cp39-win_amd64.pyd
 Comment: 
 
-Filename: jijmodeling-1.0.0rc3.dist-info/RECORD
+Filename: jijmodeling-1.0.0rc4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jijmodeling/__init__.pyi

```diff
@@ -339,16 +339,17 @@
 @typing.final
 class ArrayLength:
     """
     A class for referring to the length of an array at a given axis.
     
     The ArrayLength class is to refer to the number of elements of an axis in an array.
     
-    This class is not intended to be instantiated directly. Instead, you can use
-    the `len_at` method in of `Placeholder`, `Element` or `Subscript`.
+    This class is not intended to be constructed directly. Instead, we
+    recommend using the `len_at` method of `Placeholder`, `Element` or
+    `Subscript`.
     
     Attributes:
         array: A variable with `ndim >= 1`.
         axis: An axis index. A $n$-dimensional variable has $n$ axes. Axis 0 is the array's outermost axis and $n-1$ is the innermost.
         description (str, optional): A description of the ArrayLength instance.
     
     Raises:
@@ -357,15 +358,15 @@
     Examples:
         Create a length of axis 0 in a 2-dimensional placeholder.
     
         >>> import jijmodeling as jm
         >>> a = jm.Placeholder("a", ndim=2)
         >>> N = a.len_at(0, latex="N")
     """
-    def __new__(cls):
+    def __new__(cls, array, axis, *, latex=None, description=None):
         pass
 
     def __add__(self, value, /):
         """
         Return self+value.
         """
         pass
@@ -1153,18 +1154,21 @@
     
     The Element class is used to create an element.
     It is used in the following cases:
     - an index of summation $\displaystyle \sum$ (:obj:`SumOp`)
     - an index of product $\displaystyle \prod$ (:obj:`ProdOp`)
     - a bound variable of the universal quantifier $\forall$ (:obj:`Forall`)
     
-    It has a set that it belongs to.
-    There are two options for this set:
-    1. A half-open range, where the lower bound is included and the upper bound is excluded
-    2. A `Placeholder`, `Element`, or `Subscript` variable with `ndim` >= 1
+    Elements specify a set to which they belong. The set can be:
+    1. A half-open range, where the lower bound is included and the upper bound is excluded.
+    2. A `Placeholder`, `Element`, or `Subscript` object with `ndim` >= 1.
+    
+    Ranges are generally specified with tuples as `(start, end)`. For
+    convenience, passing a single number or scalar object as the argument is
+    interpreted as the `end` of a range starting from zero.
     
     The index operator (`[]`) of an element with `ndim >= 1` returns a :obj:`Subscript` object.
     
     Attributes:
         name (str): A name of the element.
         ndim (int): The number of dimensions of the element. The value is one less than the value of `belong_to.ndim`.
         description (str): A description of the element.
@@ -1174,40 +1178,51 @@
         name (str): A name of the element.
         belong_to: A set the element belongs to.
         latex (str, optional): A LaTeX-name of the element to be represented in Jupyter notebook.
             It is set to :obj:`name` by default.
         description (str, optional): A description of the element.
     
     Examples:
+        Note that `belong_to` is a positional argument, not a keyword
+        argument, and so does not need to be written out. This is done in some
+        of these examples for clarity.
+    
         Create an element that belongs to a half-open range.
     
         >>> import jijmodeling as jm
         >>> i = jm.Element("i", belong_to=(0,10))
     
-        If you pass an object with `ndim` as the `belong_to` argument, the set that the element belongs to is a range with a start of 0 and an end of the object.
+        If you pass a scalar as the `belong_to` argument, the set that the element belongs to is a range starting at 0 going up to that value.
     
         >>> import jijmodeling as jm
-        >>> i = jm.Element("i", belong_to=10)
+        >>> i = jm.Element("i", 10)
         >>> assert jm.is_same(i, jm.Element("i", belong_to=(0,10)))
     
+        The applies not just to numbers, but certain scalars, like `Placeholder` (with `ndim == 0`).
+    
+        >>> import jijmodeling as jm
+        >>> n = jm.Placeholder("N")
+        >>> i = jm.Element("i", n)
+        >>> assert jm.is_same(i, jm.Element("i", belong_to=(0,n)))
+    
         Create an element that belongs to a 1-dimensional placeholder.
     
         >>> import jijmodeling as jm
         >>> E = jm.Placeholder("E", ndim=1)
-        >>> e = jm.Element("e", belong_to=E)
+        >>> e = jm.Element("e", E)
     
         Create a 1-dimensional element with the index of `123`.
     
         >>> import jijmodeling as jm
         >>> a = jm.Placeholder("a", ndim=2)
-        >>> e = jm.Element("e", belong_to=a)
+        >>> e = jm.Element("e", a)
         >>> e[123]
         Element(name='e', belong_to=Placeholder(name='a', ndim=2))[NumberLit(value=123)]
     """
-    def __new__(cls, name: str, *, belong_to, latex=None, description=None):
+    def __new__(cls, name: str, belong_to, *, latex=None, description=None):
         pass
 
     def __add__(self, value, /):
         """
         Return self+value.
         """
         pass
@@ -1425,15 +1440,15 @@
         energy (numpy.ndarray): The value of energy of each sample.
         objective (numpy.ndarray): The value of an objective function of each sample.
         constraint_violations (dict[str, numpy.ndarray]): The constraint violation of each sample.
         constraint_forall (dict[str, numpy.ndarray]): The constraint forall of each sample.
         constraint_values (numpy.ndarray): The constraint value of each sample.
         penalty (dict[str, numpy.ndarray]): The penalty of each sample.
     """
-    def __new__(cls, energy=Ellipsis, objective=Ellipsis, constraint_violations=Ellipsis, constraint_forall=Ellipsis, constraint_values=Ellipsis, penalty=Ellipsis):
+    def __new__(cls, energy=None, objective=None, constraint_violations=None, constraint_forall=None, constraint_values=None, penalty=None):
         pass
 
     constraint_expr_values: typing.Any
     constraint_forall: typing.Any
     constraint_values: typing.Any
     constraint_violations: typing.Any
     energy: typing.Any
@@ -2614,15 +2629,15 @@
     A class for storing time to be measured.
     
     Attributes:
         solve (SolvingTime): Time to solve the problem.
         system (SystemTime): Time to measure system time.
         total (float, optional): Total time to solve the problem. Defaults to None.
     """
-    def __new__(cls, solve=Ellipsis, system=Ellipsis, total=None):
+    def __new__(cls, solve=None, system=None, total=None):
         pass
 
     @staticmethod
     def from_dict(dict):
         """
         Create a MeasuringTime object from the given dict.
         
@@ -3920,24 +3935,24 @@
     A sparse solution is a dict whose key is a variable name and the value is a list of tuples with three elements,
     where the first element is a list of indices, the second element is a list of non-zero values, and the third element is a shape of the array.
     The length of the list of solutions must be the same as the length of the list of num_occurrences.
     Each index of the list of solutions corresponds to the same index of the list of non-zero values.
     
     As an example, consider the following solutions:
     
-    ```python
+    ```
     {
         "x": [np.array([[0.0, 1.0, 0.0], [2.0, 0.0, 3.0]]), np.array([[1.0, 0.0, 0.0], [2.0, 3.0, 4.0]])],
         "y": [np.array([0.0, 0.0, 1.0]), np.array([0.0, 1.0, 0.0])]
     }
     ```
     
     This is a dense solution. The corresponding sparse solution is as follows:
     
-    ```python
+    ```
     {
         "x": [(([0, 1, 1], [1, 0, 2]), [1.0, 2.0, 3.0], (2, 3)), (([0, 1, 1, 1], [0, 0, 1, 2]), [1.0, 2.0, 3.0, 4.0], (2, 3))],
         "y": [(([2],), [1.0], (3,)), (([1],), [1.0], (3,))]
     }
     ```
     
     Attributes:
@@ -5070,37 +5085,69 @@
     
     Raises:
         ModelingError: Raises if the input contains a decision variable.
     """
     pass
 
 
-def extract_nodes(obj, type):
+def concatenate(sample_sets):
+    """
+    Concatenate some SampleSet objects into a single SampleSet object.
+    
+    Args:
+        sample_sets (list[SampleSet]): A list of SampleSet objects.
+    
+    Returns:
+        SampleSet: A SampleSet object which is concatenated from the given SampleSet objects.
+    
+    Note:
+        This function will be deprecated in v1.1.0.
+    """
+    pass
+
+
+def extract_nodes(obj, class_or_tuple):
     """
     Extract all nodes from the given object.
     
     Args:
         obj: An expression defined by JijModeling's module, or a `Problem`, `Constraint`, `CustomPenaltyTerm`, or a list of forall object.
-        type: A type of node to extract.
+        class_or_tuple: A type or tuple of types of nodes to be extracted.
     
     Returns:
         list: A list of nodes whose type is `type`.
     
     Examples:
         Extract all placeholders from the given expression.
     
-        ```python
+        ```
         >>> from itertools import zip_longest
         >>> import jijmodeling as jm
         >>> a = jm.Placeholder("a")
         >>> b = jm.Placeholder("b")
         >>> expr = jm.Placeholder("a") + jm.Placeholder("b")
         >>> for actual, expect in zip_longest(jm.extract_nodes(expr, jm.Placeholder), [a, b]):
         >>>     assert jm.is_same(actual, expect)
         ```
+    
+        Extract all BinaryVar objects and Placeholder objects from the given expression.
+    
+        ```
+        >>> from itertools import zip_longest
+        >>> import jijmodeling as jm
+        >>> a = jm.Placeholder("a")
+        >>> b = jm.Placeholder("b")
+        >>> x = jm.BinaryVar("x")
+        >>> y = jm.ContinuousVar("y", lower_bound=0, upper_bound=1)
+        >>> expr = a * x + b * y + 123
+        >>> actual = jm.extract_nodes(expr, (jm.BinaryVar, jm.Placeholder))
+        >>> expect = [a, x, b, y]
+        >>> for actual, expect in zip_longest(actual, expect):
+        >>>     assert jm.is_same(actual, expect)
+        ```
     """
     pass
 
 
 def extract_variables(obj):
     """
     Extract all variables from the given object without duplication.
@@ -5115,15 +5162,15 @@
     
     Returns:
         list: A list of variables, which are `Placeholder`, `Element`, `ArrayLength`, `BinaryVar`, `IntegerVar`, `ContinuousVar`, `SemiIntegerVar`, or `SemiContinuousVar`.
     
     Examples:
         Extract all variables from a problem without duplication.
     
-        ```python
+        ```
         >>> n = jm.Placeholder("n")
         >>> i = jm.Element("i", belong_to=n)
         >>> x = jm.BinaryVar("x", shape=[10])
         >>> y = jm.IntegerVar("y", shape=[10], lower_bound=0, upper_bound=1)
         >>> z = jm.ContinuousVar("z", shape=[10], lower_bound=0, upper_bound=1)
         >>> problem = jm.Problem("problem")
         >>> problem += jm.sum(i, x[i])
@@ -5178,15 +5225,15 @@
     
     Returns:
         bool: True if degree of the expression is determined dynamically.
     
     Examples:
         Check if the degree of the following expression is determined dynamically.
     
-        ```python
+        ```
         a = jm.Placeholder("a", ndim=1)
         i = jm.Element("i", belong_to=a)
         x = jm.BinaryVar("x", shape=(a.len_at(0),))
         # The number of multiplication is not determined until the value of a is given.
         expr = jm.prod(i, x[i])
         assert jm.is_dynamic_degree(expr)
         ```
@@ -5352,15 +5399,15 @@
     
     Returns:
         obj: The `MaxOp` object whose operands are the inputs.
     
     Examples:
         Create the `MaxOp` object whose operands are three placeholders.
     
-        ```python
+        ```
         >>> import jijmodeling as jm
         >>> a = jm.Placeholder("a")
         >>> b = jm.Placeholder("b")
         >>> c = jm.Placeholder("c")
         >>> jm.max(a, b, c)
         ```
     
@@ -5379,15 +5426,15 @@
     
     Returns:
         obj: The `MinOp` object whose operands are the inputs.
     
     Examples:
         Create the `MinOp` object whose operands are three placeholders.
     
-        ```python
+        ```
         >>> import jijmodeling as jm
         >>> a = jm.Placeholder("a")
         >>> b = jm.Placeholder("b")
         >>> c = jm.Placeholder("c")
         >>> jm.min(a, b, c)
         ```
     
@@ -5445,25 +5492,25 @@
     Args:
        expr: A target math expression.
        replacer: A callable object that takes an expression node and returns a new expression node.
     
     Examples:
         Replace a placeholder with a binary variable.
     
-        ```python
+        ```
         >>> import jijmodeling as jm
         >>> ph = jm.Placeholder("placeholder")
         >>> var = jm.BinaryVar("x")
         >>> replaced = jm.replace(ph, lambda x: var if isinstance(x, jm.Placeholder) else x)
         >>> assert jm.is_same(replaced, var)
         ```
     
         Replace a subscripted variable with a binary variable if it is a placeholder.
     
-        ```python
+        ```
         >>> import jijmodeling as jm
         >>> ph = jm.Placeholder("ph", ndim=2)
         >>> x = jm.BinaryVar("x", shape=(1000, 1000))
         >>> elt = jm.Element("elt", belong_to=ph)
         >>> expr = ph[123, 456] + elt[123]
         >>> replacer = (
             lambda node: x[node.subscripts]
```

## Comparing `jijmodeling-1.0.0rc3.dist-info/METADATA` & `jijmodeling-1.0.0rc4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jijmodeling
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `jijmodeling-1.0.0rc3.dist-info/license_files/LICENSE.txt` & `jijmodeling-1.0.0rc4.dist-info/license_files/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `jijmodeling-1.0.0rc3.dist-info/RECORD` & `jijmodeling-1.0.0rc4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-jijmodeling-1.0.0rc3.dist-info/METADATA,sha256=bd0B4Ka_3Ddzsxw14g0LHExIWsFmILfJSJvLA90TsmM,2902
-jijmodeling-1.0.0rc3.dist-info/WHEEL,sha256=AEr5m1XkYiXdLchbOjtn7VSjoPs_2BeqH39awFrbrB0,94
-jijmodeling-1.0.0rc3.dist-info/license_files/LICENSE.txt,sha256=llUjgcEN5bUeFlj1RqxJxDMxUnlYvowLsldCF6Lwq8c,3445
+jijmodeling-1.0.0rc4.dist-info/METADATA,sha256=e77FkZ4IurgO_N0EchXpqR29r1H38u2qfoYk_Fk64p0,2902
+jijmodeling-1.0.0rc4.dist-info/WHEEL,sha256=AEr5m1XkYiXdLchbOjtn7VSjoPs_2BeqH39awFrbrB0,94
+jijmodeling-1.0.0rc4.dist-info/license_files/LICENSE.txt,sha256=llUjgcEN5bUeFlj1RqxJxDMxUnlYvowLsldCF6Lwq8c,3445
 jijmodeling/__init__.py,sha256=dTz5lvd2qXlLmjsXX3Pq7v2_dptMkGNTWIf37gSrvwE,127
-jijmodeling/__init__.pyi,sha256=SSZHOgCB8V1iH7BaEIh91IrMKYww2okkkzTMd9hjDdg,129449
+jijmodeling/__init__.pyi,sha256=N7t4R5GhH0R6YTI8PT54e0pkjOko2BZwYYNiEmT-o70,131169
 jijmodeling/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-jijmodeling/jijmodeling.cp39-win_amd64.pyd,sha256=t6HiyXzvhOOPXTNq590_f1ZcRjuhuWB4u1qeP4MWMhg,2172928
-jijmodeling-1.0.0rc3.dist-info/RECORD,,
+jijmodeling/jijmodeling.cp39-win_amd64.pyd,sha256=zN2jvLi_1OwIv3cNR04mngjYs19AzfLsz4XlFCE1D54,2202624
+jijmodeling-1.0.0rc4.dist-info/RECORD,,
```

