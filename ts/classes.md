# TypeScript

## Classes

Classes are public by default.

### Inheritance

```ts
class Animal {}

class Dog extends Animal {}
```

Super method:

```ts
class Animal {
  name: string;
  constructor(theName: string) {
    this.name = theName;
  }
  move(distanceInMeters: number = 0) {
    console.log(`${this.name} moved ${distanceInMeters}m.`);
  }
}

class Snake extends Animal {
  // super ctor is called
  constructor(name: string) {
    super(name);
  }
  // super method is called
  move(distanceInMeters = 5) {
    console.log("Slithering...");
    super.move(distanceInMeters);
  }
}

class Horse extends Animal {
  constructor(name: string) {
    super(name);
  }
  move(distanceInMeters = 45) {
    console.log("Galloping...");
    super.move(distanceInMeters);
  }
}

let sam = new Snake("Sammy the Python");
let tom: Animal = new Horse("Tommy the Palomino");

sam.move();
tom.move(34);
```

### Private fields

[$TODO](https://devblogs.microsoft.com/typescript/announcing-typescript-3-8-beta/#ecmascript-private-fields)

```ts
class Animal {
  #name: string;
  constructor (theName: string) {
    this.#name = theName;
  }
}

// error:
new Animal("Cat").#name
```

### Readonly class members
