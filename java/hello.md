# Java

## First program

The name of the file where this code is written must be named `Hello.java`. Each Java file must be named after the identifier of its `public` class (if it has one).

```java
// single line comment

/* multiple line comment */

public class Hello {
  public static void main(String[] args) {
    System.out.println("Hello world");
  }
}
```

- `class` keyword starts the class definition block.
- all applications must contain a `main` method
- conventionally, `public` comes before `static`

## Program lifecycle

`javac` compiles, `java` runs:

```
javac Hello.java
java Hello
```

- **javac** (Java compiler) creates a `Hello.class` file, which contains Java bytecode (an intermediate representation), **compilation** errors are produced here
- javac also links libraries to the program after it's compiled
- **java** runs the class file using the **JVM** (Java Virtual Machine), **runtime** errors are produced here
- JVM runs Java bytecode, turns bytecode into platform-specific machine code
- JVM is basically an interpreter boosted by a  Just-In-Time (JIT) compiler

## Java bytecode

Java bytecode has opcodes (instruction code) of single-byte length, so there are only 256 possible instructions ; currently about 200 are in use, some of them legacy.