
---

# Todo App

A simple and efficient command-line Todo application, built in Go. This app allows users to manage their tasks effectively, with functionalities like adding, completing, and deleting tasks, along with a visually appealing display of todo items.

## Features

- **Add tasks:** Quickly add new tasks.
- **Complete tasks:** Mark tasks as completed.
- **Delete tasks:** Remove tasks from the list.
- **List tasks:** Display all tasks with their status.
- **Visual Appeal:** Uses colored text and table format for better readability.

## Installation

To install the Todo app, you need to have Go installed on your machine. Follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/stevel705/todo-app.git
   ```
2. Navigate to the cloned directory:
   ```bash
   cd todo-app
   ```

## Usage

After installation, you can run the app using the following commands:

- **Adding a task:**
  ```bash
  go run cmd/todo/main.go -add "Your task here"
  ```
- **Completing a task:**
  ```bash
  go run cmd/todo/main.go -complete [task number]
  ```
- **Deleting a task:**
  ```bash
  go run cmd/todo/main.go -del [task number]
  ```
- **Listing all tasks:**
  ```bash
  go run cmd/todo/main.go -list
  ```

## Structure

The application's structure is as follows:

```
├── LICENSE
├── Makefile
├── README.md
├── cmd
│   └── todo
│       └── main.go
├── colors.go
├── go.mod
├── go.sum
├── todo.go
└── todos.json
```

- `main.go`: The entry point of the application, handling command-line arguments and user interaction.
- `todo.go`: Contains the core functionalities and structures of the Todo application.
- `colors.go`: Provides functions for colored text output to enhance the UI.
- `todos.json`: Stores the todo items in a JSON format.
- `Makefile`: Contains commands for building and running the application.

## Example 

```diff
╔═══╤═══════════════════════════════╤═══════╤═════════════════════╤═════════════════════╗
║ # │             Task              │ Done? │           CreatedAt │         CompletedAt ║
╟━━━┼━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┼━━━━━━━┼━━━━━━━━━━━━━━━━━━━━━┼━━━━━━━━━━━━━━━━━━━━━╢
║ 1 │ ✅ Create todo app on golang  │ yes   │ 09 Dec 23 21:21 +04 │ 11 Dec 23 22:38 +04 ║
║ 2 │ ✅ write readme               │ yes   │ 09 Dec 23 21:24 +04 │ 11 Dec 23 22:38 +04 ║
║ 3 │ another task                  │ no    │ 11 Dec 23 22:29 +04 │ 01 Jan 01 00:00 UTC ║
║ 4 │ another task from pipe        │ no    │ 11 Dec 23 22:30 +04 │ 01 Jan 01 00:00 UTC ║
╟━━━┼━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┼━━━━━━━┼━━━━━━━━━━━━━━━━━━━━━┼━━━━━━━━━━━━━━━━━━━━━╢
║                               You have 2 pending todos                                ║
╚═══╧═══════════════════════════════╧═══════╧═════════════════════╧═════════════════════╝
```


## Contributing

Contributions to improve the application are welcome. Feel free to fork the repository and submit pull requests.

## License

Distributed under the MIT License. See `LICENSE` for more information.

---

You can adjust the content as per your project's specifics and any additional features or instructions you might want to add.