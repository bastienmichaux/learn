# Java

## First program

The following sample must be written to a `Hello.java` file:

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
- all applications must contain a `main` method with mandatory signature `public static void main (String[] args)`
- however the parameter of the `main` method can be named freely
- `args` parameter = mechanism through which runtime system passes info to the app, each string in the array is a command-line argument
- conventionally, `public` comes before `static`

### Program lifecycle

- `javac` compiles
- `java` runs:

```
javac Hello.java
java Hello
```

- **javac** (Java compiler) creates a `Hello.class` file, which contains Java bytecode (an intermediate representation)
- **compilation** errors are produced here (if any)
- javac also links libraries to the program after it's compiled
- **java** runs the class file using the **JVM** (Java Virtual Machine)
- **runtime** errors are produced here (if any)
- JVM runs Java bytecode, turns bytecode into platform-specific machine code
- JVM is basically an interpreter boosted by a  Just-In-Time (JIT) compiler

### Mandatory file naming

A `.java` file that contains a `public` class `Foo` must be named `Foo.java`, otherwise the compiler emits an error at compile-time.

Classes that aren't public won't cause that compilation error if their source file isn't named according to the class identifier.