# JavaScript

## Flow

### Traditional control flow

Most of JavaScript flow control is identical to C and Java.

```js
if (condition) {
  // executed when condition == true
} else if (anotherCondition) {
  // executed when anotherCondition == true
} else {
  // executed if (condition && anotherCondition) == false
}

for (let i = 0; i < 100; i++) {
  console.log(i);
}

let i = 0;
while (i < 100) {
  i++;
  console.log(i);
}

let i = 0;
do {
  i++;
  console.log(i);
} while (i < 100);
```

### Ternary operator

Behaves the same as ternary operators in C and Java.

```js
let age = 17;
let isMinor = (age >= 18) ? true : false;
```
