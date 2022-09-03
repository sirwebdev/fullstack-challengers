# Challenger 01 - Todo App

This is a challenger for you practice your skills about React and Node with Javascript language.

## Requirements

1. Knowlegdes about Javascript.
2. Knowlegdes about React JS.
3. Knowlegdes about NodeJS.
4. Knowlegdes about HTML and CSS.
5. Installed NodeJS into your machine.

## About the challenger

Create a full aplication of a Todo App.

## Backend

We need to create an api who will have one endpoint.

### /todos

Need to have 4 METHODS

1. POST => Create a new TODO.
2. GET => List all TODOS.
3. GET => Show TODO by ID.
4. PUT => Update TODO by ID.
5. DELETE => Delete a todo by ID.

#### TODO - Entity

```typescript
interface TODO {
  id: string;
  name: string;
  isCompleted: boolean;
  created_at: Date;
  updated_at: Date;
}
```

## Frontend

Create a web app inspired into FIGMA prototype.

### Requirements

1. Need to create a new TODO.
2. Need to update the TODO data.
3. Need to delete a TODO.
4. Need to list all storaged TODOS.
5. Need to complete a TODO.
6. Need to select a TODO.
