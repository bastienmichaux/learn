# TypeScript

## Generics

```ts
// T is the "type variable"
function identity<T>(arg: T): T {
  return arg;
}

let output = identity<string>("myString");
```

With arrays:

```ts
function loggingIdentity<T>(arg: T[]): T[] {
  console.log(arg.length);
  return arg;
}

function loggingIdentity<T>(arg: Array<T>): Array<T> {
  console.log(arg.length);
  return arg;
}
```