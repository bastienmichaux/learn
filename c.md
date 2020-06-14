# C Programming Language

## Lifecycle

1. a successfully compiled C file creates an **object file** (`.obj`)
1. object files are linked by the linker,
1. if no errors after the linking phase, an executable file is created
1. the executable can still emit runtime errors

## First program

```c
// pre-processing directive importing a library
#include stdio.h

// "main" method is mandatory,
// the returned integer is the program exit code
int main(void){
  printf("Hello world!");
  return 0;
}
```

## String interpolation

```c
int main(void){
  int salary;
  salary = 10000;
  printf("My salary is %d.\n", salary);
  return 0;
}
```

## Modulo

```c
#include stdio.h
int main(void){
  int cookies = 45;
  int children = 7;
  int cookies_per_child = 0;
  int cookies_left_over = 0;
  cookies_per_child = cookies/children;
  cookies_left_over = cookies%children;
  printf("You have %d children and %d cookies\n", children, cookies);
  printf("Give each child %d cookies.\n", cookies_per_child);
  printf("There are %d cookies left over.\n", cookies_left_over);
  return 0;
}
```

## Flow

### Ternary operator

```c
int age = 17;
bool isMinor = (age >= 18) ? true : false;
```