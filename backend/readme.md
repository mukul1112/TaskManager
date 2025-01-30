# Task Manager

A simple task management web application built with React. This app allows you to create, update, and delete tasks with editable fields for task title, description, priority, and status. It also includes validation for required fields and provides user feedback when interacting with tasks.

## Features
- **Create Tasks**: Add a new task with a title, description, priority, and status.
- **Update Tasks**: Modify task details such as title, description, priority, and status.
- **Delete Tasks**: Remove tasks from the list.
- **Field Validation**: Required fields (Title and Description) are validated before submission, with visual feedback (red border and error message).


## Technology Stack

- **Backend**: Express.js & Node.js


## Demo
To run a demo, clone this repository and set up the project as described below.

## Getting Started

### Prerequisites
Make sure you have Node.js and npm installed. You can download them from [here]https://github.com/mukul1112/TaskManager.git.

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mukul1112/task-manager.git
   cd task-manager
   ```
2. **Install dependencies:**
   ```bash
   npm install
   ```
3. **Set up the db with mongo** Make process.env in root and give it your mongo url to connect your specific db

4. **Start the development server:**
      node server.js

   This will start the React development server at `http://localhost:5000`.

5. **Access the app:** Open `http://localhost:500` in your browser to see the task manager in action.

## Usage
- **Add a Task**: Click on "Add Task", fill in the task details, and click the "Add Task" button.
- **Edit Task**: To edit an existing task, click on the "Edit" button next to it. Update the title, description, priority, or status, and click the "Update Task" button.
- **Delete Task**: To delete a task, click the "Delete" button next to it.

## API Endpoints (for backend developers)
If you're setting up the backend API, here are the required routes:

- **GET `/tasks`** - Fetch all tasks.
- **POST `/tasks`** - Create a new task (requires title, description, priority, and status).
- **PUT `/tasks/:id`** - Update a task's title, description, priority, or status.
- **DELETE `/tasks/:id`** - Delete a task by ID.

### Example Response (GET `/tasks`):
```json
[
  {
    "_id": "1",
    "title": "Task 1",
    "description": "Task 1 description",
    "priority": "High",
    "status": "Pending"
  },
  {
    "_id": "2",
    "title": "Task 2",
    "description": "Task 2 description",
    "priority": "Medium",
    "status": "In Progress"
  }
]
```



