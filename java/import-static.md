# Java

## Import

### Static import

A static import allows referencing a method without referencing the class. This was introduced by Java 1.5.

Static imports are useful for simplifying code.

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