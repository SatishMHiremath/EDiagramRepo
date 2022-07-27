# ER-Diagram : ToDoList App

![image](https://user-images.githubusercontent.com/17871885/180851293-842fb120-1105-4d46-8e52-17eaa3277dfa.png)


# Task Manager App

## JSON Entities

### Task
    {
	    "taskId": 1,
	    "title": "Task 1",
	    "description": "Task 1 description",
	    "dueDate": "dd/mm/yyyy",
      "completed": false,
      "notes": [
        { "noteId": 1
          "title": "Note title 1",
          "body": "Note body 1"
        },
        {
          "noteId": 2
          "title": "Note title 2",
          "body": "Note body 2"
        },
        {
          "noteId": 3
          "title": "Note title 3",
          "body": "Note body 3"
        }
      ]
    }

## API Endpoints 

### `POST /tasks` 
Create a new task

### `GET /tasks`
Get all tasks
Available filters - 
- `/articles?completed=true/false`

### `GET /tasks/{task_id}`
Get the details of a particular task including notes

### `PATCH /tasks/{task_id}`
Edit a task - Add / Remove notes from the task. Mark a task completed.

### `PATCH /tasks/{task_id}`

### `DELETE /tasks/{task_id}`
Delete a particular task
