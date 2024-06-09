
# Todo App
This is a simple Todo application built using GoLang. It provides APIs for managing todo items such as creating, updating, deleting, and retrieving todos.

## Installation

1. Clone the repository:
	 ```bash
	git clone https://github.com/roopeshkp34/todo-go
	```
2. Navigate to the project directory:
	```bash
	cd todo-go
	```
3. Build the project:
	```bash
	go build
	```
## Usage


### Running the Application

To start the application, run the executable generated after building:

  ```bash
	go run ./main.go
```

By default, the application will run on port `9000`. You can access it at `http://localhost:9000`.

### Endpoints
1.  `GET /`
	Retrieves all todos.
3.  `POST /`
	Creates a new todo.
	
	Example request body:

	```json
	{
		"Title": "Example todo",
		"Completed": false
	}
	```

3.  `PUT /{id}`
Updates an existing todo identified by its id.

	Example request body:

	```json
	{
		"title": "Updated todo",
		"Completed": false
	}
	```
4.  `DELETE /{id}`
	Delete an existing todo