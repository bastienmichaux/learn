# Java

## Program flow

### Ternary operator

Similar to C ternary operator.

```java
int age = 17;
bool isMinor = (age >= 18) ? true : false;
```

### for-each loop

Also called "enhanced for".

Is forward-only iterator.

Cannot be used for modifying an array element.

Cannot be used for comparing successive elements.

```java
// "myCollection" is an array
// iteration stops after the last array element is processed
for (int myInt : myCollection) {
  System.out.println(myInt);
}
```