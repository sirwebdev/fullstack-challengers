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

### Requirements

1. POST => Create a new TODO.
2. GET => List all TODOS.
3. GET => Show TODO by ID.
4. PUT => Update TODO by ID.
5. DELETE => Delete a todo by ID.

#### POST - /todos

#### Rules

1. Should not be able to create a todo without any data.
2. Should be able to create a new TODO with is_completed false by default.
3. Should return 201 status code.

```typescript
interface CreateTodoDTO {
  name: string;
}
```

```typescript
interface CreateTodoPresenter {
  id: string;
  name: string;
  is_completed: boolean;
  created_at: Date;
  updated_at: Date;
}
```

### GET - /todos

#### Rules

1. Should list all storaged TODO's.

```typescript
interface ListTodoPresenter {
  id: string;
  name: string;
  is_completed: boolean;
  created_at: Date;
  updated_at: Date;
}
[];
```

### GET - /todos/:id

#### Rules

1. Should get the selected todo by id.
2. Should not be able to show a non-existent todo. (it has to return error message here and status code 400)

```typescript
interface ShowTodoPresenter {
  id: string;
  name: string;
  is_completed: boolean;
  created_at: Date;
  updated_at: Date;
}
```

### PUT - /todos/:id

#### Rules

1. Should update the selected todo by id.
2. Should not be able to update a non-existent todo. (it has to return error message here and status code 400)

```typescript
interface UpdateTodoDTO {
  name: string;
  is_completed: boolean;
}
```

```typescript
interface UpdateTodoPresenter {
  id: string;
  name: string;
  is_completed: boolean;
  created_at: Date;
  updated_at: Date;
}
```

## Frontend

Create a web app inspired into FIGMA prototype.

### DELETE - /todos/:id

#### Rules

1. Should delete the selected todo by id.
2. Should not be able to delete non-existent todo. (it has to return error message here and status code 400)

```typescript
interface UpdateTodoDTO {
  name: string;
  is_completed: boolean;
}
```

```typescript
interface UpdateTodoPresenter {
  id: string;
  name: string;
  is_completed: boolean;
  created_at: Date;
  updated_at: Date;
}
```

### Requirements

1. Need to create a new TODO.
2. Need to update the TODO data.
3. Need to delete a TODO.
4. Need to list all storaged TODOS.
5. Need to complete a TODO.
6. Need to select a TODO.
