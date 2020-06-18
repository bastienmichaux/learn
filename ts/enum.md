# TypeScript

## Enum

```ts
enum Color {Red, Green, Blue}

let c: Color = Color.Green;
// same:
let c: Color = Color[1];
```

Change numbering:

```ts
enum Color {Red =1, Green, Blue}
let c: Color = Color[2]; // Color.Green
```