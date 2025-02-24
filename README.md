[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=18360588)
# CSSE6400 Week 1 Practical

Construction of a simple HTTP server in Python.

Please see the [instructions](https://csse6400.uqcloud.net/practicals/week01.pdf) for more details.

## How to Run
The server in the project can be run using the command:
```
poetry run flask --app todo run -p 6400
```
This initialises the server with port 6400, and the port number can be changed.
### Debug mode
To run the app in debug mode (enables hot reloading), add the command `--debug`. The command may look like:
```
poetry run flask --app todo run -p 6400 --debug
```
Currently, if the server is run using the [command above](#how-to-run), the server has the following URL paths:
http://localhost:6400/api/v1/health
http://localhost:6400/api/v1/todos
http://localhost:6400/api/v1/todos/1

The URLs can accept the following methods:
- http://localhost:6400/api/v1/health
    - GET
- http://localhost:6400/api/v1/todos
    - GET
    - POST
- http://localhost:6400/api/v1/todos/1
    - GET
    - PUT
    - DELETE