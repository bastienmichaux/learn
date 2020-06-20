# TypeScript

## Class interface

Can't be used for checking private members.

```ts
interface ClockInterface {
  currentTime: Date;
  setTime(d: Date): void;
}

class Clock implements ClockInterface {
  currentTime: Date = new Date();
  setTime(d: Date) {
    this.currentTime = d;
  }
  constructor(h: number, m: number) {}
}
```

$TODO: https://www.staging-typescript.org/docs/handbook/interfaces.html#difference-between-the-static-and-instance-sides-of-classes

$TODO: https://www.staging-typescript.org/docs/handbook/interfaces.html#interfaces-extending-classes