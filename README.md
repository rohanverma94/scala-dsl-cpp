# scala-dsl-cpp
Scala Domain Specific Language for C++17. Now parallelize your code with spark, akka and many other frameworks.

This project defines a Scala library for the core C++ language and some useful STL
libraries. It also provides implementations of Scala collections such as HashMap
or List in the C++ DSL.

The C++ language
-------------------

The functionality of the C++ language itself is provided in the package.
This includes functions such as `sizeof`, address-taking and dereferencing.

The following import
is also needed in order to use it:

```scala
import scalapp._
```

To use the JNI implementations, the code needs to load the library
generated during compilation:

```scala
System.loadLibrary("scalapp")
```