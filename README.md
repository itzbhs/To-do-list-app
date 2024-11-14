# To-do-list-app

## Functional REiqeruiements

1. **User Interface:**
   - Provide a console-based menu for interacting with the application.

2. **Add a Task:**
   - Allow the user to add a task to the to-do list.
   - If the list is full, notify the user that no more tasks can be added. The limit is 5 tasks.

3. **View Tasks:**
   - Display all the tasks in the to-do list with their respective numbers.

4. **Remove a Task:**
   - Allow the user to remove a task by specifying its number.
   - Shift the remaining tasks up in the list to fill the gap.
   - If the specified task number is invalid, notify the user.

5. **Exit the Application:**
   - Provide an option to exit the application gracefully.

## Non-Functional Requirements

1. **Usability:**
   - The application should be easy to use with clear instructions and prompts.
   - Input validation should be performed to ensure valid choices are made by the user.

2. **Maintainability:**
   - The code should be organized and commented to make it easy to understand and maintain.
   - Methods should be modular, each performing a single task.

## User Interface Flow

1. **Main Menu:**
   - Display the following options:
     1. Add a task
     2. View tasks
     3. Remove a task
     4. Exit

2. **Add Task:**
   - Prompt the user to enter a task description.
   - Add the task to the list and tell the user addition was successful or not.

3. **View Tasks:**
   - Display all tasks with their respective numbers.

4. **Remove Task:**
   - Prompt the user to enter the task number to remove.
   - Confirm that the user wants to remove the task.
   - Remove the specified task and tell the user that removal was successful or not.

5. **Exit:**
   - Exit the application with a goodbye message.

## Additional Considerations

1. **Error Handling:**
   - Handle cases where the user inputs invalid choices or task numbers.
   - Notify the user of any errors and prompt them to try again.
2. **User Interface::**
   - After each action from the user is complete, display the menu again until the user quits the application.

## Example
```bash
$ java ToDoList.java

To-Do List Application
1. Add a task
2. View tasks
3. Remove a task
4. Exit
Choose an option: 1
Enter a task: Buy groceries
Task added.

To-Do List Application
1. Add a task
2. View tasks
3. Remove a task
4. Exit
Choose an option: 1
Enter a task: Walk the dog
Task added.

To-Do List Application
1. Add a task
2. View tasks
3. Remove a task
4. Exit
Choose an option: 2
To-Do List:
1. Buy groceries
2. Walk the dog

To-Do List Application
1. Add a task
2. View tasks
3. Remove a task
4. Exit
Choose an option: 3
Enter the task number to remove: 9
Invalid choice: There is no task number 9.

To-Do List Application
1. Add a task
2. View tasks
3. Remove a task
4. Exit
Choose an option: 3
Enter the task number to remove: 1
Are you sure you want to remove task "Buy groceries"? No
Task not removed.

To-Do List Application
1. Add a task
2. View tasks
3. Remove a task
4. Exit
Choose an option: 3
Enter the task number to remove: 1
Are you sure you want to remove task "Buy groceries"? Yes
Task removed.

To-Do List Application
1. Add a task
2. View tasks
3. Remove a task
4. Exit
Choose an option: 2
To-Do List:
1. Walk the dog

To-Do List Application
1. Add a task
2. View tasks
3. Remove a task
4. Exit
Choose an option: 4
Goodbye!
```