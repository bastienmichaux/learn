# Java

## Intro

### Jargon

- JDK: Java Development Kit, for compiling & running
- JRE: Java Runtime Environment, runs 3rd-party Java programs
- SDK: outdated term for JDK (y 98-2006)
- SE: Standard Edition, for simple programs
- EE: Enterprise Edition, for complex programs
- ME: Micro Edition, for cell phones / small devices
- JavaFx: toolkit for desktop graphical applications
- OpenJDK: free & open-source SE implementation, no browser integration or JavaFX

"Java SE 8" is the same as "Java 1.8".

"Java 8u5" is 5th update of Java 1.8.

### History

- Java 1.0 (1996): 8 packages, 212 classes. Still backward compatible today.
- Java 1.1 (1997): inner classes, Java Beans, JDBC, RMI, Reflection API, JIT compiler.
- Java 1.2 (1998): Collections API. Aka Java 2.
- Java 1.3 (2000): Java platform debugger architecture (JPDA).
- Java 1.4 (2002): improved perf, low-level IO (image IO, nio), regexp, XML, XSLT libs, SSL support, logging API, cryptography, IPv6 support.
- Java 5 (2004): generics, enums, annotations, varags methods, autoboxing, enhanced for.
- Java 6 (2006): Compiler API, external language bindings.
- Java 7 (2011): Oracle bought Java, try-with-resources, NIO.2 API, Method Handles API.
- Java 8 (2014): huge update, lambda expressions, new date & time API, concurrency libs updated.
- Java 9 (2017): platform modularity.
- Since Java 10 (2018), releases follow a 6-month cycle and are smaller.
- Java 11 (sep 18): long-term support (LTS) release, HTTP/2 API.

## Characteristics

- statically typed
- multithreaded
- bytecode has extensive static checking
- dispatch is virtual by default (? $TODO)
- no preprocessor ala C
- no operator overloading
- no pointers
- automatic memory mgmt via garbage collection
- runtime can be extensively instrumented (?)
- class-based objects
- namespaces
- object encapsulation
- no structs: no low-level memory layout
- class files are portable as long as the running system has a JVM
- is always pass-by-value (but a value can be an object reference)
- no support for full multiple inheritance
- generics are less powerful (but also less dangerous) than C++ templates
- keywords are case-sensitive