# TypeScript

## Array

```ts
// square brackets notation
let x: number[] = [1, 2, 3];

// generic array type
let x: Array<number> = [1, 2, 3];
```

### Readonly array

A readonly array cannot be modified after it's created.

Use readonly over const for typing properties: variables use `const`where properties use `readonly`.

```ts
let a: number[] = [1, 2, 3, 4];
let ro: ReadonlyArray<number> = a;
ro[0] = 12; // error!
ro.push(5); // error!
ro.length = 100; // error!
```

It cannot be assigned to a mutable type:

```ts
let a: number[] = [1, 2, 3, 4];
let ro: ReadonlyArray<number> = a;

// unless using a type assertion:
a = (number[]) ro;
```
