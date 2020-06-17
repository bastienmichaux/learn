# TypeScript

## Tuple

When accessing an element with a known index, the correct type is retrieved.

Accessing an element outside the set of known indices fails with an error.

```ts
let x: [string, number];
x = [`hello`, 10]; // ok
x = [10, `hello`]; // error

x[0].substring(1); // error:
// Property 'substring' does not exist on type 'number'.

x[3] = "world"; // Error, Property '3' does not exist on type '[string, number]'.
// Tuple type '[string, number]' of length '2' has no element at index '3'.
```