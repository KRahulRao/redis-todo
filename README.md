
# RedisTodo

RedisTodo is a todo list API for users to consume and build your own client or use the default client.

## API

Nike has a RESTful API that supports CRUD operations on users and their todos.

### TODO

- Retrieve all the user's todos: `GET /users/:userId/todos`.

- Retrieve a single todo: `GET /users/:userId/todos/:todoId`.

- Create a todo: `POST /users/:userId/todos`.
- Allowed params: `content`, `status`.
- Request payload: `{content: 'your todo content', status: 'whatever your client uses'}`.

- Update a todo: `PATCH /users/:userId/todos/:todoId`.
- Allowed params: `status`, `content`.
- Request payload: `{status: 'your updated status', content: 'your updated content'}`.

- Delete a todo: `DELETE /users/:userId/todos/:todoId`.

### USER

- Create a user: `POST /users/`.
- Allowed params: `name`, `id`.
- Request payload: `{name: 'your name', id: 'yourusername'}`.

- Update a user: `PATCH /users/:userId`.
- Allowed params: `name`.
- Request payload: `{name: 'your corrected name'}`.

- Retrieve a user (and a list of the user's todos): `GET /users/:userId`.

- Delete a user (Not yet implemented): `DELETE /users/:userId`.

## Stack

### Server
- NodeJS
- Express
- Redis
