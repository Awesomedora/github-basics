# github-basics
Learning github

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>To-Do List App</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="container">
    <h1>To-Do List</h1>
    <form id="task-form">
      <input type="text" id="task-input" placeholder="Add a new task" required>
      <button type="submit">Add Task</button>
    </form>
    <ul id="task-list"></ul>
  </div>
  <script src="script.js"></script>
</body>
</html>




* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.container {
  background: #fff;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  width: 100%;
  max-width: 400px;
}

h1 {
  text-align: center;
  margin-bottom: 20px;
}

#task-form {
  display: flex;
  justify-content: space-between;
  margin-bottom: 20px;
}

#task-input {
  flex: 1;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
  margin-right: 10px;
}

#task-form button {
  padding: 10px 20px;
  background-color: #28a745;
  color: #fff;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

#task-form button:hover {
  background-color: #218838;
}

#task-list {
  list-style: none;
}

.task-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
  margin-bottom: 10px;
  background-color: #f9f9f9;
}

.task-item.completed {
  text-decoration: line-through;
  opacity: 0.7;
}

.task-item .actions {
  display: flex;
  gap: 10px;
}

.task-item .actions button {
  padding: 5px 10px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.task-item .actions .edit-btn {
  background-color: #ffc107;
  color: #000;
}

.task-item .actions .delete-btn {
  background-color: #dc3545;
  color: #fff;
}

.task-item .actions .complete-btn {
  background-color: #007bff;
  color: #fff;
}
