# 48-hour Sprint: full-stack CRUD to-do list application

Designed and built a To-Do List App with client-side, server-side, and an SQL database

## Features:

* A front-end experience that allows a user to create and store tasks inside
  a database table and updates the DOM to display it as a new to-do item

* Tasks have buttons to 'Complete' or 'Delete'
  
  * When a task is marked a completed:
    * Its `isComplete` boolean value in the database table is updated to `TRUE`
    * When a task has been marked as completed a CSS class is applied to the task
      its "complete" button visibly appears grayed out

   * When a task is marked a deleted:
     * It is removed from the database table
     * The DOM updates task list without the deleted task

## CSS styling moves project aesthetic beyond basic HTML
  - Background color of the single page view is unique
  - Font family and size are adjusted to please the eye
  - Text or background color of Tasks indicate their status

## Database Created through Postico 
  - Runs the queries documented in `database.sql`
  - Creates a `todos` table and populates it with Tasks

## Testing Rubrics
  - A task's text has data-testid = "toDoTextInput"
  - New Task Button has data-testid = "submitButton"
  - Rendered Tasks have data-testid = "toDoItem"
  - HTML elements for tasks have <tr data-testid = "toDoItem">...</tr>
  - Delete buttons have data-testid ="deleteButton" and are children of data-testid = "toDoItem"
  - Complete buttons have data-testid ="completeButton" and are children of data-testid = "toDoItem"

## Future Feature Ideas
  - Colorize Creation, Completion and Delete Buttons
  - Add Bootstrap styles to Task text inputs 
  - Responsive screen sizes
  - Add Sweet Alert pop-ups as confirmations
  - Add TIMESTAMP column to the Task table
