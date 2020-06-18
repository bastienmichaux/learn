# TypeScript

## Function interface

An interface can be designed for a function.

The parameter names don't matter for the compiler.

```ts
interface SearchFunc {
  (source: string, subString: string): boolean;
}

let mySearch: SearchFunc;

mySearch = function (src: string, substr: string): boolean {
  let result = source.search(subString);
  return result > -1;
};
```