# TypeScript

## Interfaces

Interfaces define contracts with the code.

TS checks an object has at least the specified property-type pairs.

Interfaces can be literals (useful for one-shots):

```ts
function printLabel(labeledObj: { label: string }) {
  console.log(labeledObj.label);
}

let myObj = {
  size: 10,
  label: "Size 10 Object"
};

printLabel(myObj);
```

Interfaces can be interface-blocks (recommended):

```ts
interface LabeledValue {
  label: string;
}

function printLabel(labeledObj: LabeledValue) {
  console.log(labeledObj.label);
}
```

### Optional properties

Compiler won't scream if an optional property is missing from an object.

```ts
interface Foo {
  mandatoryProperty: any;
  optionalProperty?: any;
}
```

If an interface has only optional properties, an object implementing that interface must have at least one property described by the interface.

```ts
interface SquareConfig {
  color?: string;
  width?: number;
}

let squareOptions = { colour: "red", width: 100 };
let mySquare = createSquare(squareOptions); // ok

let squareOptions = { colour: "red" };
let mySquare = createSquare(squareOptions); // error
```

### Readonly properties

Can be only modified when an object is created.

```ts
interface Point {
  readonly x: number;
  readonly y: number;
}

let p1: Point = { x: 10, y: 20 };
p1.x = 5; // error!
```

### Excess property

Allow adding any property to an object:

```ts
interface SquareConfig {
  color?: string;
  width?: number;
  [propName: string]: any;
}
```

### Interface extension

```ts
interface Shape {
  color: string;
}

interface PenStroke {
  penWidth: number;
}

interface Square extends Shape, PenStroke {
  sideLength: number;
}

let square = {} as Square;
square.color = "blue";
square.sideLength = 10;
square.penWidth = 5.0;
```

$TODO: https://www.staging-typescript.org/docs/handbook/interfaces.html#hybrid-types