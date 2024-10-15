Simple To-Do List Application
This project is a basic command-line To-Do List application written in Python. It allows users to manage their tasks by adding, viewing, and deleting tasks, which are stored in a text file (tasks.txt).

Features
Add Task: Allows users to add tasks to a text file.
View Tasks: Lists all the tasks saved in the text file.
Delete Task: Deletes a specific task based on its number from the list.
Persistent Storage: Tasks are saved in a tasks.txt file, so they are not lost when the program exits.
Requirements
This application does not require any external libraries beyond Python's standard library. Ensure you have Python 3.x installed.

Usage
Clone or Download this repository.

Run the Script using Python:

bash
Copy code
python todo.py
Menu Options:

1. Add Task: Enter the task you want to add. It will be stored in the tasks.txt file.
2. View Tasks: Displays all tasks from the tasks.txt file with a task number.
3. Delete Task: Enter the task number you wish to delete. The selected task will be removed from the list.
4. Exit: Closes the application.
Code Breakdown
add_task(task):

Appends the new task to the tasks.txt file.
Prints a message confirming that the task was added.
view_tasks():

Reads all tasks from the tasks.txt file.
Displays the tasks in a numbered list format. If no tasks are found, it alerts the user.
delete_task(task_number):

Deletes the task corresponding to the provided task number from tasks.txt.
Handles invalid task numbers gracefully.
main():

Runs an interactive menu system that allows the user to select one of the available options (add, view, delete, or exit).
File Structure
plaintext
Copy code
todo.py     # Main script for the To-Do List
tasks.txt   # (Auto-generated) File to store tasks
Customization
Task Storage File: The tasks are stored in a file named tasks.txt by default. You can change this by modifying the TODO_FILE variable.

Error Handling: The application handles common user errors such as invalid task numbers and non-existent files. You can modify the messages or add more robust error handling as needed.

Example Output
plaintext
Copy code
To-Do List
1. Add Task
2. View Tasks
3. Delete Task
4. Exit
Enter your choice: 2
No tasks found.

To-Do List
1. Add Task
2. View Tasks
3. Delete Task
4. Exit
Enter your choice: 1
Enter the task: Buy groceries
Task "Buy groceries" added.

To-Do List
1. Add Task
2. View Tasks
3. Delete Task
4. Exit
Enter your choice: 2
Your tasks:
1. Buy groceries
License
This project is open-source and free to use for personal or educational purposes.

