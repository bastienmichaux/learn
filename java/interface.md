# Java

## Interface

An interface is a named block that contains methods. Methods must have empty bodies.

A class can implement one or more interfaces. When a class implements an interface, the compiler checks at build time that the class contains the variables and methods declared by the interface.

```java
interface Bicycle {
  public void speedUp(int increment);
}

public class MyBicycle implement Bicycle {
  private int speed = 0;

  public void speedUp(int increment) {
    speed = speed + increment;
  }
}
```

An interface is a reference type.
