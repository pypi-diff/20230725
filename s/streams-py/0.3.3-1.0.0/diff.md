# Comparing `tmp/streams_py-0.3.3.tar.gz` & `tmp/streams_py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streams_py-0.3.3.tar", max compression
+gzip compressed data, was "streams_py-1.0.0.tar", max compression
```

## Comparing `streams_py-0.3.3.tar` & `streams_py-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0    35149 2023-07-25 11:02:49.403561 streams_py-0.3.3/LICENSE
--rw-r--r--   0        0        0    10867 2023-07-25 11:02:49.403561 streams_py-0.3.3/README.md
--rw-r--r--   0        0        0      733 2023-07-25 11:02:49.407561 streams_py-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      157 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/__init__.py
--rw-r--r--   0        0        0      336 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/__iterate.py
--rw-r--r--   0        0        0     3910 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/__optional.py
--rw-r--r--   0        0        0     3483 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/__stream.py
--rw-r--r--   0        0        0     1654 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/__stream_converter.py
--rw-r--r--   0        0        0        0 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_itertools/__init__.py
--rw-r--r--   0        0        0     1713 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_itertools/tools.py
--rw-r--r--   0        0        0        0 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_lazy/__init__.py
--rw-r--r--   0        0        0      626 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_lazy/process.py
--rw-r--r--   0        0        0      593 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_lazy/queue.py
--rw-r--r--   0        0        0        0 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_parallel/__init__.py
--rw-r--r--   0        0        0     3885 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_parallel/fork_and_join.py
--rw-r--r--   0        0        0      787 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_parallel/parallelizer.py
--rw-r--r--   0        0        0    16037 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/__base_stream.py
--rw-r--r--   0        0        0        0 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/__init__.py
--rw-r--r--   0        0        0     3380 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/__parallel_stream.py
--rw-r--r--   0        0        0     2227 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/__sequential_stream.py
--rw-r--r--   0        0        0     3062 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/error/__error.py
--rw-r--r--   0        0        0      258 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/error/__levels.py
--rw-r--r--   0        0        0      307 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/error/__sentinel.py
--rw-r--r--   0        0        0     3595 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/numeric/__numeric_base_stream.py
--rw-r--r--   0        0        0      861 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
--rw-r--r--   0        0        0      686 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
--rw-r--r--   0        0        0      221 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/__init__.py
--rw-r--r--   0        0        0      307 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/combiners.py
--rw-r--r--   0        0        0    10878 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/date.py
--rw-r--r--   0        0        0     4937 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/numeric.py
--rw-r--r--   0        0        0     1385 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/string.py
--rw-r--r--   0        0        0      735 2023-07-25 11:02:49.407561 streams_py-0.3.3/pystreamapi/conditions/types.py
--rw-r--r--   0        0        0    11722 1970-01-01 00:00:00.000000 streams_py-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 15:31:42.633015 streams_py-1.0.0/LICENSE
+-rw-r--r--   0        0        0    11424 2023-07-25 15:31:42.633015 streams_py-1.0.0/README.md
+-rw-r--r--   0        0        0      733 2023-07-25 15:31:42.637014 streams_py-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/__iterate.py
+-rw-r--r--   0        0        0     3910 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/__optional.py
+-rw-r--r--   0        0        0     3483 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/__stream.py
+-rw-r--r--   0        0        0     1654 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/__stream_converter.py
+-rw-r--r--   0        0        0        0 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_itertools/__init__.py
+-rw-r--r--   0        0        0     1713 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_itertools/tools.py
+-rw-r--r--   0        0        0        0 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_lazy/__init__.py
+-rw-r--r--   0        0        0      626 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_lazy/process.py
+-rw-r--r--   0        0        0      593 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_lazy/queue.py
+-rw-r--r--   0        0        0        0 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_parallel/__init__.py
+-rw-r--r--   0        0        0     3885 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_parallel/fork_and_join.py
+-rw-r--r--   0        0        0      787 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_parallel/parallelizer.py
+-rw-r--r--   0        0        0    16037 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/__base_stream.py
+-rw-r--r--   0        0        0        0 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/__init__.py
+-rw-r--r--   0        0        0     3380 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/__parallel_stream.py
+-rw-r--r--   0        0        0     2227 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/__sequential_stream.py
+-rw-r--r--   0        0        0     3062 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/error/__error.py
+-rw-r--r--   0        0        0      258 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/error/__levels.py
+-rw-r--r--   0        0        0      307 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/error/__sentinel.py
+-rw-r--r--   0        0        0     3595 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/numeric/__numeric_base_stream.py
+-rw-r--r--   0        0        0      861 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/numeric/__parallel_numeric_stream.py
+-rw-r--r--   0        0        0      686 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/_streams/numeric/__sequential_numeric_stream.py
+-rw-r--r--   0        0        0      221 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/__init__.py
+-rw-r--r--   0        0        0      307 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/combiners.py
+-rw-r--r--   0        0        0    10878 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/date.py
+-rw-r--r--   0        0        0     4937 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/numeric.py
+-rw-r--r--   0        0        0     1385 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/string.py
+-rw-r--r--   0        0        0      735 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/conditions/types.py
+-rw-r--r--   0        0        0     1688 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/loaders/__csv_loader.py
+-rw-r--r--   0        0        0       74 2023-07-25 15:31:42.637014 streams_py-1.0.0/pystreamapi/loaders/__init__.py
+-rw-r--r--   0        0        0    12279 1970-01-01 00:00:00.000000 streams_py-1.0.0/PKG-INFO
```

### Comparing `streams_py-0.3.3/LICENSE` & `streams_py-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/README.md` & `streams_py-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 Although it closely mirrors the Java API, PyStreamAPI adds some innovative features to make streams in Python even more 
 innovative, declarative and easy to use.
 
 PyStreamAPI offers both sequential and parallel streams and utilizes lazy execution.
 
 Now you might be wondering why another library when there are already a few implementations? Well, here are a few advantages of this particular implementation:
 
-* It provides both sequential and parallel versions.
+* It provides both sequential and parallel streams.
 * Lazy execution is supported, enhancing performance.
 * It boasts high speed and efficiency.
 * The implementation achieves 100% test coverage.
 * It follows Pythonic principles, resulting in clean and readable code.
 * It adds some cool innovative features such as conditions or error handling and an even more declarative look.
+* It provides loaders for various data sources such as CSV
 
 Let's take a look at a small example:
 
 ```python
 from pystreamapi import Stream
 
 Stream.of([" ", '3', None, "2", 1, ""]) \
@@ -208,14 +209,31 @@
 ```python
 Stream.concat(Stream.of([1, 2]), Stream.of([3, 4])) 
 # Like Stream.of([1, 2, 3, 4])
 ```
 
 Creates a new Stream from multiple Streams. Order doesn't change.
 
+## Use loaders: Load data from CSV files in just one line
+
+PyStreamAPI offers a convenient way to load data from CSV files. Like that you can start processing your CSV right away without having to worry about reading and parsing the file.
+
+You can import the loader with:
+
+```python
+from pystreamapi.loaders import csv
+```
+Now you can use the loader directly when creating your Stream:
+
+```python
+Stream.of(csv("data.csv", delimiter=";")) \
+    .map(lambda x: x["name"]) \
+    .for_each(print)
+```
+
 ## API Reference
 For a more detailed documentation view the docs on GitBook: [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/)
 
 ## Complex Examples
 
 #### Get all numbers from list of different types. Use parallelization.
```

#### html2text {}

```diff
@@ -6,79 +6,80 @@
 PyStreamAPI is a Python stream library that draws inspiration from the Java
 Stream API. Although it closely mirrors the Java API, PyStreamAPI adds some
 innovative features to make streams in Python even more innovative, declarative
 and easy to use. PyStreamAPI offers both sequential and parallel streams and
 utilizes lazy execution. Now you might be wondering why another library when
 there are already a few implementations? Well, here are a few advantages of
 this particular implementation: * It provides both sequential and parallel
-versions. * Lazy execution is supported, enhancing performance. * It boasts
-high speed and efficiency. * The implementation achieves 100% test coverage. *
-It follows Pythonic principles, resulting in clean and readable code. * It adds
+streams. * Lazy execution is supported, enhancing performance. * It boasts high
+speed and efficiency. * The implementation achieves 100% test coverage. * It
+follows Pythonic principles, resulting in clean and readable code. * It adds
 some cool innovative features such as conditions or error handling and an even
-more declarative look. Let's take a look at a small example: ```python from
-pystreamapi import Stream Stream.of([" ", '3', None, "2", 1, ""]) \ .filter
-(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter
-(lambda x: len(x) > 0) \ .map(int) \ .sorted() \ .for_each(print) # Output: 1 2
-3 ``` And here's the equivalent code in Java: ```java Object[] words = { " ",
-'3', null, "2", 1, "" }; Arrays.stream( words ) .filter( Objects::nonNull )
-.map( Objects::toString ) .map( String::trim ) .filter( s -> ! s.isEmpty() )
-.map( Integer::parseInt ) .sorted() .forEach( System.out::println ); // Output:
-1 2 3 ``` ## What is a Stream? A `Stream` is a powerful abstraction for
-processing sequences of data in a functional and declarative manner. It enables
-efficient and concise data manipulation and transformation. Similar to its
-counterparts in Java and Kotlin, a Stream represents a pipeline of operations
-that can be applied to a collection or any iterable data source. It allows
-developers to express complex data processing logic using a combination of
-high-level operations, promoting code reusability and readability. With
-Streams, you can perform a wide range of operations on your data, such as
-filtering elements, transforming values, aggregating results, sorting, and
-more. These operations can be seamlessly chained together to form a processing
-pipeline, where each operation processes the data and passes it on to the next
-operation. One of the key benefits of Stream is lazy evaluation. This means
-that the operations are executed only when the result is actually needed,
-optimizing resource usage and enabling efficient processing of large or
-infinite datasets. Furthermore, Stream supports both sequential and parallel
-execution. This allows you to leverage parallel processing capabilities when
-dealing with computationally intensive tasks or large amounts of data,
-significantly improving performance. `pystreamapi.Stream` represents a stream
-that facilitates the execution of one or more operations. Stream operations can
-be categorized as either intermediate or terminal. Terminal operations return a
-result of a specific type, while intermediate operations return the stream
-itself, enabling method chaining for multi-step operations. Let's examine an
-example using Stream: ```python Stream.of([" ", '3', None, "2", 1, ""]) \
-.filter(lambda x: x is not None) \ # Intermediate operation .map(str) \ #
-Intermediate operation .map(lambda x: x.strip()) \ # Intermediate operation
-.filter(lambda x: len(x) > 0) \ # Intermediate operation .map(int) \ #
-Intermediate operation .sorted() \ # Intermediate operation .for_each(print) #
-Terminal Operation (Output: 1 2 3) ``` Operations can be performed on a stream
-either in parallel or sequentially. A parallel stream executes operations
-concurrently, while a sequential stream processes operations in order.
-Considering the above characteristics, a stream can be defined as follows: * It
-is not a data structure itself but operates on existing data structures. * It
-does not provide indexed access like traditional collections. * It is designed
-to work seamlessly with lambda functions, enabling concise and expressive code.
-* It facilitates easy aggregation of results into lists, tuples, or sets. * It
-can be parallelized, allowing for concurrent execution of operations to improve
-performance. * It employs lazy evaluation, executing operations only when
-necessary. ## Use conditions to speed up your workflow! ![Conditions](https://
-raw.githubusercontent.com/PickwickSoft/pystreamapi/main/assets/conditions.png)
-Conditions provide a convenient means for performing logical operations within
-your Stream, such as using `filter()`, `take_while()`, `drop_while()`, and
-more. With PyStreamAPI, you have access to a staggering 111 diverse conditions
-that enable you to process various data types including strings, types,
-numbers, and dates. Additionally, PyStreamAPI offers a powerful combiner that
-allows you to effortlessly combine multiple conditions, facilitating the
-implementation of highly intricate pipelines. ## Error handling: Work with data
-that you don't know PyStreamAPI offers a powerful error handling mechanism that
-allows you to handle errors in a declarative manner. This is especially useful
-when working with data that you don't know. PyStreamAPI offers three different
-error levels: - `ErrorLevel.RAISE`: This is the default error level. It will
-raise an exception if an error occurs. - `ErrorLevel.IGNORE`: This error level
-will ignore any errors that occur and won't inform you. - `ErrorLevel.WARN`:
-This error level will warn you about any errors that occur and logs them as a
+more declarative look. * It provides loaders for various data sources such as
+CSV Let's take a look at a small example: ```python from pystreamapi import
+Stream Stream.of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not
+None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter(lambda x: len(x) > 0) \
+.map(int) \ .sorted() \ .for_each(print) # Output: 1 2 3 ``` And here's the
+equivalent code in Java: ```java Object[] words = { " ", '3', null, "2", 1, ""
+}; Arrays.stream( words ) .filter( Objects::nonNull ) .map( Objects::toString )
+.map( String::trim ) .filter( s -> ! s.isEmpty() ) .map( Integer::parseInt )
+.sorted() .forEach( System.out::println ); // Output: 1 2 3 ``` ## What is a
+Stream? A `Stream` is a powerful abstraction for processing sequences of data
+in a functional and declarative manner. It enables efficient and concise data
+manipulation and transformation. Similar to its counterparts in Java and
+Kotlin, a Stream represents a pipeline of operations that can be applied to a
+collection or any iterable data source. It allows developers to express complex
+data processing logic using a combination of high-level operations, promoting
+code reusability and readability. With Streams, you can perform a wide range of
+operations on your data, such as filtering elements, transforming values,
+aggregating results, sorting, and more. These operations can be seamlessly
+chained together to form a processing pipeline, where each operation processes
+the data and passes it on to the next operation. One of the key benefits of
+Stream is lazy evaluation. This means that the operations are executed only
+when the result is actually needed, optimizing resource usage and enabling
+efficient processing of large or infinite datasets. Furthermore, Stream
+supports both sequential and parallel execution. This allows you to leverage
+parallel processing capabilities when dealing with computationally intensive
+tasks or large amounts of data, significantly improving performance.
+`pystreamapi.Stream` represents a stream that facilitates the execution of one
+or more operations. Stream operations can be categorized as either intermediate
+or terminal. Terminal operations return a result of a specific type, while
+intermediate operations return the stream itself, enabling method chaining for
+multi-step operations. Let's examine an example using Stream: ```python
+Stream.of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not None) \ #
+Intermediate operation .map(str) \ # Intermediate operation .map(lambda x:
+x.strip()) \ # Intermediate operation .filter(lambda x: len(x) > 0) \ #
+Intermediate operation .map(int) \ # Intermediate operation .sorted() \ #
+Intermediate operation .for_each(print) # Terminal Operation (Output: 1 2 3)
+``` Operations can be performed on a stream either in parallel or sequentially.
+A parallel stream executes operations concurrently, while a sequential stream
+processes operations in order. Considering the above characteristics, a stream
+can be defined as follows: * It is not a data structure itself but operates on
+existing data structures. * It does not provide indexed access like traditional
+collections. * It is designed to work seamlessly with lambda functions,
+enabling concise and expressive code. * It facilitates easy aggregation of
+results into lists, tuples, or sets. * It can be parallelized, allowing for
+concurrent execution of operations to improve performance. * It employs lazy
+evaluation, executing operations only when necessary. ## Use conditions to
+speed up your workflow! ![Conditions](https://raw.githubusercontent.com/
+PickwickSoft/pystreamapi/main/assets/conditions.png) Conditions provide a
+convenient means for performing logical operations within your Stream, such as
+using `filter()`, `take_while()`, `drop_while()`, and more. With PyStreamAPI,
+you have access to a staggering 111 diverse conditions that enable you to
+process various data types including strings, types, numbers, and dates.
+Additionally, PyStreamAPI offers a powerful combiner that allows you to
+effortlessly combine multiple conditions, facilitating the implementation of
+highly intricate pipelines. ## Error handling: Work with data that you don't
+know PyStreamAPI offers a powerful error handling mechanism that allows you to
+handle errors in a declarative manner. This is especially useful when working
+with data that you don't know. PyStreamAPI offers three different error levels:
+- `ErrorLevel.RAISE`: This is the default error level. It will raise an
+exception if an error occurs. - `ErrorLevel.IGNORE`: This error level will
+ignore any errors that occur and won't inform you. - `ErrorLevel.WARN`: This
+error level will warn you about any errors that occur and logs them as a
 warning with default logger. This is how you can use them: ```python from
 pystreamapi import Stream, ErrorLevel Stream.of([" ", '3', None, "2", 1, ""]) \
 .error_level(ErrorLevel.IGNORE) \ .map_to_int() \ .error_level
 (ErrorLevel.RAISE) \ .sorted() \ .for_each(print) # Output: 1 2 3 ``` The code
 above will ignore all errors that occur during mapping to int and will just
 skip the elements. For more details on how to use error handling, please refer
 to the documentation. ## Get started: Installation To start using PyStreamAPI
@@ -104,21 +105,28 @@
 numeric) Stream.of_noneable(None) ``` If the source is `None`, you get an empty
 `Stream` --- ```python Stream.iterate(0, lambda n: n + 2) ``` Creates a Stream
 of an infinite Iterator created by iterative application of a function f to an
 initial element seed, producing a Stream consisting of seed, f(seed), f(f
 (seed)), etc. > **Note** > Do not forget to limit the stream with `.limit()` --
 - ```python Stream.concat(Stream.of([1, 2]), Stream.of([3, 4])) # Like
 Stream.of([1, 2, 3, 4]) ``` Creates a new Stream from multiple Streams. Order
-doesn't change. ## API Reference For a more detailed documentation view the
-docs on GitBook: [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/) ##
-Complex Examples #### Get all numbers from list of different types. Use
-parallelization. ```python Stream.parallel_of([" ", '3', None, "2", 1, ""]) \
-.filter(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \
-.filter(lambda x: len(x) > 0) \ .map(int) \ .sorted()\ .for_each(print) # 1 2 3
-``` #### Generate a Stream of 10 Fibonacci numbers ```python def fib(): a, b =
-0, 1 while True: yield a a, b = b, a + b Stream.of(fib()) \ .limit(10) \
-.for_each(print) # 0 1 1 2 3 5 8 13 21 34 ``` ## Performance Note that parallel
-Streams are not always faster than sequential Streams. Especially when the
-number of elements is small, we can expect sequential Streams to be faster. ##
-Bug Reports Bug reports can be submitted in GitHub's [issue tracker](https://
-github.com/PickwickSoft/pystreamapi/issues). ## Contributing Contributions are
-welcome! Please submit a pull request or open an issue.
+doesn't change. ## Use loaders: Load data from CSV files in just one line
+PyStreamAPI offers a convenient way to load data from CSV files. Like that you
+can start processing your CSV right away without having to worry about reading
+and parsing the file. You can import the loader with: ```python from
+pystreamapi.loaders import csv ``` Now you can use the loader directly when
+creating your Stream: ```python Stream.of(csv("data.csv", delimiter=";")) \
+.map(lambda x: x["name"]) \ .for_each(print) ``` ## API Reference For a more
+detailed documentation view the docs on GitBook: [PyStreamAPI Docs](https://
+pystreamapi.pickwicksoft.org/) ## Complex Examples #### Get all numbers from
+list of different types. Use parallelization. ```python Stream.parallel_of(["
+", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not None) \ .map(str) \
+.map(lambda x: x.strip()) \ .filter(lambda x: len(x) > 0) \ .map(int) \ .sorted
+()\ .for_each(print) # 1 2 3 ``` #### Generate a Stream of 10 Fibonacci numbers
+```python def fib(): a, b = 0, 1 while True: yield a a, b = b, a + b Stream.of
+(fib()) \ .limit(10) \ .for_each(print) # 0 1 1 2 3 5 8 13 21 34 ``` ##
+Performance Note that parallel Streams are not always faster than sequential
+Streams. Especially when the number of elements is small, we can expect
+sequential Streams to be faster. ## Bug Reports Bug reports can be submitted in
+GitHub's [issue tracker](https://github.com/PickwickSoft/pystreamapi/issues).
+## Contributing Contributions are welcome! Please submit a pull request or open
+an issue.
```

### Comparing `streams_py-0.3.3/pyproject.toml` & `streams_py-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streams.py"
-version = "0.3.3"
+version = "1.0.0"
 authors = ["Stefan Garlonta <stefan@pickwicksoft.org>"]
 description = "A stream library for Python inspired by Java Stream API"
 keywords = ["streams", "parallel", "data"]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/PickwickSoft/pystreamapi"
 repository = "https://github.com/PickwickSoft/pystreamapi"
 readme = "README.md"
```

### Comparing `streams_py-0.3.3/pystreamapi/__optional.py` & `streams_py-1.0.0/pystreamapi/__optional.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/__stream.py` & `streams_py-1.0.0/pystreamapi/__stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/__stream_converter.py` & `streams_py-1.0.0/pystreamapi/__stream_converter.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_itertools/tools.py` & `streams_py-1.0.0/pystreamapi/_itertools/tools.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_lazy/process.py` & `streams_py-1.0.0/pystreamapi/_lazy/process.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_lazy/queue.py` & `streams_py-1.0.0/pystreamapi/_lazy/queue.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_parallel/fork_and_join.py` & `streams_py-1.0.0/pystreamapi/_parallel/fork_and_join.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_parallel/parallelizer.py` & `streams_py-1.0.0/pystreamapi/_parallel/parallelizer.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_streams/__base_stream.py` & `streams_py-1.0.0/pystreamapi/_streams/__base_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_streams/__parallel_stream.py` & `streams_py-1.0.0/pystreamapi/_streams/__parallel_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_streams/__sequential_stream.py` & `streams_py-1.0.0/pystreamapi/_streams/__sequential_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_streams/error/__error.py` & `streams_py-1.0.0/pystreamapi/_streams/error/__error.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_streams/numeric/__numeric_base_stream.py` & `streams_py-1.0.0/pystreamapi/_streams/numeric/__numeric_base_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_streams/numeric/__parallel_numeric_stream.py` & `streams_py-1.0.0/pystreamapi/_streams/numeric/__parallel_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/_streams/numeric/__sequential_numeric_stream.py` & `streams_py-1.0.0/pystreamapi/_streams/numeric/__sequential_numeric_stream.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/conditions/date.py` & `streams_py-1.0.0/pystreamapi/conditions/date.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/conditions/numeric.py` & `streams_py-1.0.0/pystreamapi/conditions/numeric.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/conditions/string.py` & `streams_py-1.0.0/pystreamapi/conditions/string.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/pystreamapi/conditions/types.py` & `streams_py-1.0.0/pystreamapi/conditions/types.py`

 * *Files identical despite different names*

### Comparing `streams_py-0.3.3/PKG-INFO` & `streams_py-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streams-py
-Version: 0.3.3
+Version: 1.0.0
 Summary: A stream library for Python inspired by Java Stream API
 Home-page: https://github.com/PickwickSoft/pystreamapi
 License: GPL-3.0-or-later
 Keywords: streams,parallel,data
 Author: Stefan Garlonta
 Author-email: stefan@pickwicksoft.org
 Requires-Python: >=3.7,<4.0
@@ -37,20 +37,21 @@
 Although it closely mirrors the Java API, PyStreamAPI adds some innovative features to make streams in Python even more 
 innovative, declarative and easy to use.
 
 PyStreamAPI offers both sequential and parallel streams and utilizes lazy execution.
 
 Now you might be wondering why another library when there are already a few implementations? Well, here are a few advantages of this particular implementation:
 
-* It provides both sequential and parallel versions.
+* It provides both sequential and parallel streams.
 * Lazy execution is supported, enhancing performance.
 * It boasts high speed and efficiency.
 * The implementation achieves 100% test coverage.
 * It follows Pythonic principles, resulting in clean and readable code.
 * It adds some cool innovative features such as conditions or error handling and an even more declarative look.
+* It provides loaders for various data sources such as CSV
 
 Let's take a look at a small example:
 
 ```python
 from pystreamapi import Stream
 
 Stream.of([" ", '3', None, "2", 1, ""]) \
@@ -229,14 +230,31 @@
 ```python
 Stream.concat(Stream.of([1, 2]), Stream.of([3, 4])) 
 # Like Stream.of([1, 2, 3, 4])
 ```
 
 Creates a new Stream from multiple Streams. Order doesn't change.
 
+## Use loaders: Load data from CSV files in just one line
+
+PyStreamAPI offers a convenient way to load data from CSV files. Like that you can start processing your CSV right away without having to worry about reading and parsing the file.
+
+You can import the loader with:
+
+```python
+from pystreamapi.loaders import csv
+```
+Now you can use the loader directly when creating your Stream:
+
+```python
+Stream.of(csv("data.csv", delimiter=";")) \
+    .map(lambda x: x["name"]) \
+    .for_each(print)
+```
+
 ## API Reference
 For a more detailed documentation view the docs on GitBook: [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/)
 
 ## Complex Examples
 
 #### Get all numbers from list of different types. Use parallelization.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streams-py Version: 0.3.3 Summary: A stream library
+Metadata-Version: 2.1 Name: streams-py Version: 1.0.0 Summary: A stream library
 for Python inspired by Java Stream API Home-page: https://github.com/
 PickwickSoft/pystreamapi License: GPL-3.0-or-later Keywords:
 streams,parallel,data Author: Stefan Garlonta Author-email:
 stefan@pickwicksoft.org Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -18,79 +18,80 @@
 PyStreamAPI is a Python stream library that draws inspiration from the Java
 Stream API. Although it closely mirrors the Java API, PyStreamAPI adds some
 innovative features to make streams in Python even more innovative, declarative
 and easy to use. PyStreamAPI offers both sequential and parallel streams and
 utilizes lazy execution. Now you might be wondering why another library when
 there are already a few implementations? Well, here are a few advantages of
 this particular implementation: * It provides both sequential and parallel
-versions. * Lazy execution is supported, enhancing performance. * It boasts
-high speed and efficiency. * The implementation achieves 100% test coverage. *
-It follows Pythonic principles, resulting in clean and readable code. * It adds
+streams. * Lazy execution is supported, enhancing performance. * It boasts high
+speed and efficiency. * The implementation achieves 100% test coverage. * It
+follows Pythonic principles, resulting in clean and readable code. * It adds
 some cool innovative features such as conditions or error handling and an even
-more declarative look. Let's take a look at a small example: ```python from
-pystreamapi import Stream Stream.of([" ", '3', None, "2", 1, ""]) \ .filter
-(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter
-(lambda x: len(x) > 0) \ .map(int) \ .sorted() \ .for_each(print) # Output: 1 2
-3 ``` And here's the equivalent code in Java: ```java Object[] words = { " ",
-'3', null, "2", 1, "" }; Arrays.stream( words ) .filter( Objects::nonNull )
-.map( Objects::toString ) .map( String::trim ) .filter( s -> ! s.isEmpty() )
-.map( Integer::parseInt ) .sorted() .forEach( System.out::println ); // Output:
-1 2 3 ``` ## What is a Stream? A `Stream` is a powerful abstraction for
-processing sequences of data in a functional and declarative manner. It enables
-efficient and concise data manipulation and transformation. Similar to its
-counterparts in Java and Kotlin, a Stream represents a pipeline of operations
-that can be applied to a collection or any iterable data source. It allows
-developers to express complex data processing logic using a combination of
-high-level operations, promoting code reusability and readability. With
-Streams, you can perform a wide range of operations on your data, such as
-filtering elements, transforming values, aggregating results, sorting, and
-more. These operations can be seamlessly chained together to form a processing
-pipeline, where each operation processes the data and passes it on to the next
-operation. One of the key benefits of Stream is lazy evaluation. This means
-that the operations are executed only when the result is actually needed,
-optimizing resource usage and enabling efficient processing of large or
-infinite datasets. Furthermore, Stream supports both sequential and parallel
-execution. This allows you to leverage parallel processing capabilities when
-dealing with computationally intensive tasks or large amounts of data,
-significantly improving performance. `pystreamapi.Stream` represents a stream
-that facilitates the execution of one or more operations. Stream operations can
-be categorized as either intermediate or terminal. Terminal operations return a
-result of a specific type, while intermediate operations return the stream
-itself, enabling method chaining for multi-step operations. Let's examine an
-example using Stream: ```python Stream.of([" ", '3', None, "2", 1, ""]) \
-.filter(lambda x: x is not None) \ # Intermediate operation .map(str) \ #
-Intermediate operation .map(lambda x: x.strip()) \ # Intermediate operation
-.filter(lambda x: len(x) > 0) \ # Intermediate operation .map(int) \ #
-Intermediate operation .sorted() \ # Intermediate operation .for_each(print) #
-Terminal Operation (Output: 1 2 3) ``` Operations can be performed on a stream
-either in parallel or sequentially. A parallel stream executes operations
-concurrently, while a sequential stream processes operations in order.
-Considering the above characteristics, a stream can be defined as follows: * It
-is not a data structure itself but operates on existing data structures. * It
-does not provide indexed access like traditional collections. * It is designed
-to work seamlessly with lambda functions, enabling concise and expressive code.
-* It facilitates easy aggregation of results into lists, tuples, or sets. * It
-can be parallelized, allowing for concurrent execution of operations to improve
-performance. * It employs lazy evaluation, executing operations only when
-necessary. ## Use conditions to speed up your workflow! ![Conditions](https://
-raw.githubusercontent.com/PickwickSoft/pystreamapi/main/assets/conditions.png)
-Conditions provide a convenient means for performing logical operations within
-your Stream, such as using `filter()`, `take_while()`, `drop_while()`, and
-more. With PyStreamAPI, you have access to a staggering 111 diverse conditions
-that enable you to process various data types including strings, types,
-numbers, and dates. Additionally, PyStreamAPI offers a powerful combiner that
-allows you to effortlessly combine multiple conditions, facilitating the
-implementation of highly intricate pipelines. ## Error handling: Work with data
-that you don't know PyStreamAPI offers a powerful error handling mechanism that
-allows you to handle errors in a declarative manner. This is especially useful
-when working with data that you don't know. PyStreamAPI offers three different
-error levels: - `ErrorLevel.RAISE`: This is the default error level. It will
-raise an exception if an error occurs. - `ErrorLevel.IGNORE`: This error level
-will ignore any errors that occur and won't inform you. - `ErrorLevel.WARN`:
-This error level will warn you about any errors that occur and logs them as a
+more declarative look. * It provides loaders for various data sources such as
+CSV Let's take a look at a small example: ```python from pystreamapi import
+Stream Stream.of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not
+None) \ .map(str) \ .map(lambda x: x.strip()) \ .filter(lambda x: len(x) > 0) \
+.map(int) \ .sorted() \ .for_each(print) # Output: 1 2 3 ``` And here's the
+equivalent code in Java: ```java Object[] words = { " ", '3', null, "2", 1, ""
+}; Arrays.stream( words ) .filter( Objects::nonNull ) .map( Objects::toString )
+.map( String::trim ) .filter( s -> ! s.isEmpty() ) .map( Integer::parseInt )
+.sorted() .forEach( System.out::println ); // Output: 1 2 3 ``` ## What is a
+Stream? A `Stream` is a powerful abstraction for processing sequences of data
+in a functional and declarative manner. It enables efficient and concise data
+manipulation and transformation. Similar to its counterparts in Java and
+Kotlin, a Stream represents a pipeline of operations that can be applied to a
+collection or any iterable data source. It allows developers to express complex
+data processing logic using a combination of high-level operations, promoting
+code reusability and readability. With Streams, you can perform a wide range of
+operations on your data, such as filtering elements, transforming values,
+aggregating results, sorting, and more. These operations can be seamlessly
+chained together to form a processing pipeline, where each operation processes
+the data and passes it on to the next operation. One of the key benefits of
+Stream is lazy evaluation. This means that the operations are executed only
+when the result is actually needed, optimizing resource usage and enabling
+efficient processing of large or infinite datasets. Furthermore, Stream
+supports both sequential and parallel execution. This allows you to leverage
+parallel processing capabilities when dealing with computationally intensive
+tasks or large amounts of data, significantly improving performance.
+`pystreamapi.Stream` represents a stream that facilitates the execution of one
+or more operations. Stream operations can be categorized as either intermediate
+or terminal. Terminal operations return a result of a specific type, while
+intermediate operations return the stream itself, enabling method chaining for
+multi-step operations. Let's examine an example using Stream: ```python
+Stream.of([" ", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not None) \ #
+Intermediate operation .map(str) \ # Intermediate operation .map(lambda x:
+x.strip()) \ # Intermediate operation .filter(lambda x: len(x) > 0) \ #
+Intermediate operation .map(int) \ # Intermediate operation .sorted() \ #
+Intermediate operation .for_each(print) # Terminal Operation (Output: 1 2 3)
+``` Operations can be performed on a stream either in parallel or sequentially.
+A parallel stream executes operations concurrently, while a sequential stream
+processes operations in order. Considering the above characteristics, a stream
+can be defined as follows: * It is not a data structure itself but operates on
+existing data structures. * It does not provide indexed access like traditional
+collections. * It is designed to work seamlessly with lambda functions,
+enabling concise and expressive code. * It facilitates easy aggregation of
+results into lists, tuples, or sets. * It can be parallelized, allowing for
+concurrent execution of operations to improve performance. * It employs lazy
+evaluation, executing operations only when necessary. ## Use conditions to
+speed up your workflow! ![Conditions](https://raw.githubusercontent.com/
+PickwickSoft/pystreamapi/main/assets/conditions.png) Conditions provide a
+convenient means for performing logical operations within your Stream, such as
+using `filter()`, `take_while()`, `drop_while()`, and more. With PyStreamAPI,
+you have access to a staggering 111 diverse conditions that enable you to
+process various data types including strings, types, numbers, and dates.
+Additionally, PyStreamAPI offers a powerful combiner that allows you to
+effortlessly combine multiple conditions, facilitating the implementation of
+highly intricate pipelines. ## Error handling: Work with data that you don't
+know PyStreamAPI offers a powerful error handling mechanism that allows you to
+handle errors in a declarative manner. This is especially useful when working
+with data that you don't know. PyStreamAPI offers three different error levels:
+- `ErrorLevel.RAISE`: This is the default error level. It will raise an
+exception if an error occurs. - `ErrorLevel.IGNORE`: This error level will
+ignore any errors that occur and won't inform you. - `ErrorLevel.WARN`: This
+error level will warn you about any errors that occur and logs them as a
 warning with default logger. This is how you can use them: ```python from
 pystreamapi import Stream, ErrorLevel Stream.of([" ", '3', None, "2", 1, ""]) \
 .error_level(ErrorLevel.IGNORE) \ .map_to_int() \ .error_level
 (ErrorLevel.RAISE) \ .sorted() \ .for_each(print) # Output: 1 2 3 ``` The code
 above will ignore all errors that occur during mapping to int and will just
 skip the elements. For more details on how to use error handling, please refer
 to the documentation. ## Get started: Installation To start using PyStreamAPI
@@ -116,21 +117,28 @@
 numeric) Stream.of_noneable(None) ``` If the source is `None`, you get an empty
 `Stream` --- ```python Stream.iterate(0, lambda n: n + 2) ``` Creates a Stream
 of an infinite Iterator created by iterative application of a function f to an
 initial element seed, producing a Stream consisting of seed, f(seed), f(f
 (seed)), etc. > **Note** > Do not forget to limit the stream with `.limit()` --
 - ```python Stream.concat(Stream.of([1, 2]), Stream.of([3, 4])) # Like
 Stream.of([1, 2, 3, 4]) ``` Creates a new Stream from multiple Streams. Order
-doesn't change. ## API Reference For a more detailed documentation view the
-docs on GitBook: [PyStreamAPI Docs](https://pystreamapi.pickwicksoft.org/) ##
-Complex Examples #### Get all numbers from list of different types. Use
-parallelization. ```python Stream.parallel_of([" ", '3', None, "2", 1, ""]) \
-.filter(lambda x: x is not None) \ .map(str) \ .map(lambda x: x.strip()) \
-.filter(lambda x: len(x) > 0) \ .map(int) \ .sorted()\ .for_each(print) # 1 2 3
-``` #### Generate a Stream of 10 Fibonacci numbers ```python def fib(): a, b =
-0, 1 while True: yield a a, b = b, a + b Stream.of(fib()) \ .limit(10) \
-.for_each(print) # 0 1 1 2 3 5 8 13 21 34 ``` ## Performance Note that parallel
-Streams are not always faster than sequential Streams. Especially when the
-number of elements is small, we can expect sequential Streams to be faster. ##
-Bug Reports Bug reports can be submitted in GitHub's [issue tracker](https://
-github.com/PickwickSoft/pystreamapi/issues). ## Contributing Contributions are
-welcome! Please submit a pull request or open an issue.
+doesn't change. ## Use loaders: Load data from CSV files in just one line
+PyStreamAPI offers a convenient way to load data from CSV files. Like that you
+can start processing your CSV right away without having to worry about reading
+and parsing the file. You can import the loader with: ```python from
+pystreamapi.loaders import csv ``` Now you can use the loader directly when
+creating your Stream: ```python Stream.of(csv("data.csv", delimiter=";")) \
+.map(lambda x: x["name"]) \ .for_each(print) ``` ## API Reference For a more
+detailed documentation view the docs on GitBook: [PyStreamAPI Docs](https://
+pystreamapi.pickwicksoft.org/) ## Complex Examples #### Get all numbers from
+list of different types. Use parallelization. ```python Stream.parallel_of(["
+", '3', None, "2", 1, ""]) \ .filter(lambda x: x is not None) \ .map(str) \
+.map(lambda x: x.strip()) \ .filter(lambda x: len(x) > 0) \ .map(int) \ .sorted
+()\ .for_each(print) # 1 2 3 ``` #### Generate a Stream of 10 Fibonacci numbers
+```python def fib(): a, b = 0, 1 while True: yield a a, b = b, a + b Stream.of
+(fib()) \ .limit(10) \ .for_each(print) # 0 1 1 2 3 5 8 13 21 34 ``` ##
+Performance Note that parallel Streams are not always faster than sequential
+Streams. Especially when the number of elements is small, we can expect
+sequential Streams to be faster. ## Bug Reports Bug reports can be submitted in
+GitHub's [issue tracker](https://github.com/PickwickSoft/pystreamapi/issues).
+## Contributing Contributions are welcome! Please submit a pull request or open
+an issue.
```

