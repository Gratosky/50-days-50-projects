# Simple To-Do List

A basic to-do list app that lets users add tasks to an unordered list.

## Features

- Add tasks via an input field
- Display tasks in an unordered list

## Example

```html
<input type="text" id="taskInput" placeholder="Enter a task" />
<button onclick="addTask()">Add</button>
<ul id="taskList"></ul>

<script>
  function addTask() {
    const input = document.getElementById("taskInput");
    const task = input.value.trim();
    if (task) {
      const li = document.createElement("li");
      li.textContent = task;
      document.getElementById("taskList").appendChild(li);
      input.value = "";
    }
  }
</script>
```

## Usage

1. Enter a task in the input field.
2. Click "Add" to append it to the list.
