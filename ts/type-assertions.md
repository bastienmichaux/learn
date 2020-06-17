# TypeScript

## Type assertions

Type assertions tell the compiler what a variable's type is. They're like casts but with no special checking/restructuring. There's no runtime impact.

```ts
// type assertion using "angle-bracket" syntax
let x: any = `this is a string`;
let strLength: number = (<string>someValue).length;

// type assertion using "as" syntax
let x: any = `this is a string`;
let strLength: number = (x s string).length;
```