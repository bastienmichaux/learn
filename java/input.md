# Java

## Input

An illegal argument can be handled by `IllegalArgumentException`.

```java
boolean parseYesOrNoResponse(char response) {
  switch(response) {
    case 'y':
    case 'Y': return true;
    case 'n':
    case 'N': return false;
  default:
    throw new IllegalArgumentException("Response must be Y or N");
  }
}
```