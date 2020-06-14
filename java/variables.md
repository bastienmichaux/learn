# Java

## Variables

### Data types (primitive types)

```java
boolean x;

char x;

byte x;
short x;
int x = 1234;
long x = 1234L; // mandatory suffix

float x = 0.31f; // mandatory suffix
double x = 0.31;
double x = 0.31d; // optional suffix
```

### Constants (`final`)

Variables declared with `final` can be initialized only once.

Final variables must be initialized in their class declaration.

Prefer constants over variables whenever possible.

Prefer CONSTANT_CASE for identifiers.

```java
class Book {
  final static int MAX_AMOUNT_OF_PAGES = 500;
  // error: constant must be initialized
  final static int MAX_AMOUNT_OF_AUTHORS;
}
```

### Static class members

A static property cannot be invoked with `this`, because `this` is a non-static variable and cannot be refrenced from a static context.

```java
public class MyTest {
  final static String message = "Hello";
  public static void main(String args[]) {
    // compilation error
    System.out.println(this.message);
  }
}
```

### instanceof

$TODO

In general, the use of instanceof is discouraged among Java programmers. It is often a sign of questionable program design. Under normal circumstances, the usage of instanceof can be avoided; it is only needed on rare occasions (but note that there are some cases where it is needed).

```java
Object o = new int[] {1,2,3};
o instanceof int[] // True: the array value is an int array
o instanceof byte[] // False: the array value is not a byte array
o instanceof Object // True: all arrays are instances of Object
```