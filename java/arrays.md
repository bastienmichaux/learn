# Java

## Arrays

### Declaration & initialization

Declaration doesn't allow specifying the array size.

General syntax:

`type[] arrayName`

Square brackets here are the **indexing operator**

```java
// declaration:
int[] numbers;

// initialization:
// allocate contiguous memory for holding 10 int
// & assign the memory address of the first element to the variable "numbers"
// so, 10 * 4 bytes
numbers = new int[10];
```

Arrays elements are initialized with a default value, **but** array of objects are initialized with `null`.

### Array initialization using array literals

Array size is determined based on the number of initializers specified in curly braces.

Also called **aggregate initialization**.

```java
int[] numbers = {15, 2, 9, 200, 18};
```

### Array initialization using `for` loop

```java
int[] numbers;
final int ARRAY_SIZE = 10;
numbers = new int[10];
for (int i = 0; i < ARRAY_SIZE; i++) {
  numbers[i] = i;
}
```

### Accessing an array element

```java
numbers[0] = 133;
```

Trying to access an element that is outside of the array's bounds results in the generation of an `ArrayIndexOutOfBonds` exception.

### Array initialization performance

Don't use arrays to store large amount of data because the compiler will create lots of bytecode to initialize the array.

Store the data in an external file.

### Multi-dimensional arrays

```java
final int NUMBER_OF_STUDENTS = 50;
final int NUMBER_OF_COURSES = 5;

// declaration
int[][] marks;

// initialization
marks = new int[NUMBER_OF_COURSES][NUMBER_OF_STUDENTS];
```
