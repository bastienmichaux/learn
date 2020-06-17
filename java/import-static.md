# Java

## Import

### Static import

A static import allows referencing a class static member without referencing the class name (without qualifying the class member). This was introduced by Java 1.5.

Static imports are useful for simplifying a program by making it more readable.

Use them only when you need frequent access to static members from one or two classes. Overuse of static imports pollutes, and can make the program unreadable and unmaintainable.

```java
import static java.lang.System.out;

public class HelloWorld {
  public static void main(String[] args) {
    out.println("Hello World!");
  }
}
```

#### Ambiguity

A static import can introduce ambiguity if a class member's identifier could belong to 2 different classes.

```java
// this code fails to compile because of ambiguous "MAX_VALUE"
import static java.lang.Integer.*;
import static java.lang.Long.*;

public class HelloWorld {
  public static void main(String[] args) {
    System.out.println(MAX_VALUE);
  }
}
```

#### Notes

- static imports prevent the use of the Constant Interface Antipattern (see Effective Java item 17).