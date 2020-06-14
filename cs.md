# CS

- endianness: byte ordering, can be big-endian or $TODO
- interpreted language: source files are directly interpreted by the compiler (usually by constructing an abstract syntax tree from the input source file).
- JIT: just-in-time compilation. $TODO

## Static checking

[$TODO](https://www.coursera.org/lecture/programming-languages-part-b/what-is-static-checking-H25ra)

Static checking: anything done to reject a program after is successfully parses, but before it runs.

Dynamically-typed language do almost no static checking.

Static checking is usually done via a type system. Each variable, expression, has a type. Purpose: avoid misuse of primitives, enforce abstraction, avoid dynamic (run-time) checking.