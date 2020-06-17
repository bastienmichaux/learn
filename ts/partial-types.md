# TypeScript

## Partial types

### Omit

An Omit type constructs a type by picking all properties except those specified as omitted.

```ts
interface Todo {
  title: string;
  description: string;
  completed: boolean;
}

type TodoPreview = Omit<Todo, 'description'>;

const todo: TodoPreview = {
  title: 'Clean room',
  completed: false;
}
```