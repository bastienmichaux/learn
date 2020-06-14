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
- Java 1.1 (1997): inner classes, Reflection API.
- Java 1.2 (1998): Collections API. Aka Java 2.
- Java 1.4 (2002): improved perf, low-level IO, regexp, XML, XSLT libs, SSL support, logging API, cryptography.
- Java 5 (2004): generic types, enums, annotations, varags methods, autoboxing, enhanced for.
- Java 6 (2006): Compiler API, external language bindings.
- Java 7 (2011): Oracle bought Java, try-with-resources, NIO.2 API, Method Handles API.
- Java 8 (2014): huge update, lambda expressions, new date & time API, concurrency libs updated.
- Java 9 (2017): platform modularity.
- Since Java 10 (2018), releases follow a 6-month cycle and are smaller.
- Java 11 (sep 18): long-term support (LTS) release, HTTP/2 API.

### Install

1. Download JDK from Oracle (SE or EE)
1. Path:
    - Windows (recommended): `c:\Java\jdk1.xx`
    - OSX: `/Library/Java/JavaVirtualMachines/jdk1.xx/Contents/Home`
    - Linux: uncompress `.tar.gz` where you want (like `/usr/java/jdk1.xx`)
1. Windows: add to path `jdk/bin;` where jdk is the correct path
1. Linux: add to `~/.bashrc` or `~/bash_profile` the following: `export PATH=jdk/bin:$PATH`, where jdk is the correct path
1. test installation in console with `javac -version`
