# Learn-Java
This Repository All About Java &amp; Framework Projects
# Java Versions Feature Comparison

# Java 8 (2014, LTS)
--> Major Features:

Lambdas & Functional Interfaces → (x) -> x * 2

Streams API → functional-style data processing

java.time (Date/Time API) → modern replacement for Date

Optional<T> → null-safety wrapper

Default & Static Methods in Interfaces

Nashorn JavaScript Engine

⚠️ Still widely used, but outdated (no modules, no new APIs).

# Java 11 (2018, LTS)

--> New Features:

HTTP Client API (standardized) → supports HTTP/2 & WebSockets

var in lambda parameters

String API improvements:

isBlank(), lines(), repeat(n)

Files API:

readString(), writeString()

Collection API:

toArray(IntFunction<T[]>)

Flight Recorder (JFR) – production profiling

New Garbage Collectors:

ZGC (scalable), Epsilon (no-op)

⚠️ JavaFX, CORBA, and Java EE modules removed.

# Java 17 (2021, LTS)

--> Language & API Features:

Sealed Classes & Interfaces → restricted inheritance

Records → concise data classes

Pattern Matching for instanceof

Text Blocks (""" multiline strings) – started in Java 13, standardized in 15

RandomGenerator API

Enhanced Pseudo-Random Number Generators

Foreign Function & Memory API (Incubator) – JNI alternative

Strong encapsulation of JDK internals (module enforcement)

# Java 21 (2023, LTS)

--> Major Innovations:

Virtual Threads (Project Loom) → lightweight concurrency

Structured Concurrency API → task-scoped concurrency

Record Patterns → destructuring with instanceof

Pattern Matching for switch (finalized)

Sequenced Collections API → ordered List/Set/Map views

Foreign Function & Memory API (standardized) → safe native interop

Unnamed Classes & Instance main methods (preview) → simpler HelloWorld

Scoped Values → thread-local alternative for immutability

# Java 23 (2024, Non-LTS)

--> Mostly preview/incubator features:

Scoped Values (2nd preview)

Structured Concurrency (3rd preview)

Stream Gatherers → custom intermediate ops

Class-File API → bytecode manipulation

Region Pinning for FFM API

Primitive Types in Patterns (preview)

Implicitly Declared Classes/Methods (preview) → script-like Java

Markdown in Javadoc (final)

⚠️ Experimental playground → not stable for production.

# Java 25 (2025, LTS, upcoming)

--> Expected Highlights (early JEP list, not final):

Value Objects (Project Valhalla) → memory-efficient primitives & tuples

Universal Generics (Valhalla + Panama) → List<int> without boxing

More Vector API enhancements → high-performance computing

String Templates (likely finalized) → STR."Hello {name}!"

Classfile API refinements

Foreign Function & Memory (mature)

Pattern Matching expansions (arrays, records, more exhaustive)

👉 Java 25 will unify Valhalla (value types), Panama (FFI), and Loom (virtual threads) into a stable LTS baseline.

# Feature Evolution Summary
| Version | Language Features                                                                        | APIs                             | JVM / Other                           |
| ------- | ---------------------------------------------------------------------------------------- | -------------------------------- | ------------------------------------- |
| **8**   | Lambdas, Streams, Default Methods, `Optional`, Date/Time                                 | Streams, java.time               | Nashorn JS                            |
| **11**  | `var` in lambdas                                                                         | HTTP Client, String & Files APIs | TLS 1.3, Flight Recorder, ZGC/Epsilon |
| **17**  | Records, Sealed Classes, Pattern Matching (`instanceof`), Text Blocks                    | RandomGenerator API              | Strong encapsulation, FFM (incubator) |
| **21**  | Virtual Threads, Structured Concurrency, Record & Switch Patterns, Sequenced Collections | Foreign Function & Memory API    | Loom concurrency model                |
| **23**  | Scoped Values, Primitive Patterns, Implicit Classes (preview)                            | Stream Gatherers, Classfile API  | Markdown Javadoc                      |
| **25**  | Value Objects, Universal Generics, String Templates (likely)                             | Vector API, refined FFM          | Valhalla + Panama + Loom convergence  |

