# TypeScript

## Basic types

```ts
let x: boolean = false;
let x: number = 0;
let color: string = "blue";

function warnUser(): void {
  console.log("Lookout, behind you!");
}
```

- all numbers are floating-point values (as in JS)

### Null & undefined

- null & undefined are subtyles of all other types, so you can assign null and undefined to something like number
- However, when using the --strictNullChecks flag, null and undefined are only assignable to any and their respective types (the one exception being that undefined is also assignable to void). This helps avoid many common errors. In cases where you want to pass in either a string or null or undefined, you can use the union type string | null | undefined.

### Never

- can be applied to functions that `throw`

```ts
function err(message: string): never {
  throw new Error(message);
}
```

### Object
