# TypeScript

## Indexable interface

An indexable type is an array element or an object property.

An indexable type is described by an index signature.

An index signature describes the type for indexing into the object (the indexer type) + the corresponding return type when indexing.

Only `string` and `number` are supported index signatures. They can both type the indexer, but only a subtype can type the returned value (because when indexing, JS converts a number to a string: `x[10]` is the same as `x["10"]`).

```ts
interface StringArray {
  [index: number]: string;
}

let myArray: StringArray;
myArray = ["Bob", "Fred"];

let myStr: string = myArray[0];
```