# REACT TO DO LIST

I developed the To-Do list based on how I would create one for myself every day. The To-Do list has main headings and subtasks for each job. After completing a task, the user can edit, delete, and check it, as well as edit the main heading and duplicate the entire task to create a new task and edit it. 

![ToDoMain](https://user-images.githubusercontent.com/60220627/203139793-23f0dca2-9f77-4cab-b296-96ed6d9c42a4.png)


## Break The UI Into A Component Hierarchy
The tasks are divided into subcomponents so that each subcomponent follows to the principle of single responsibility, in which each subcomponent is responsible for a single task.

![Web 1920 – 2](https://user-images.githubusercontent.com/60220627/203139797-f63cf19f-5709-4992-983d-763f833ce7c2.png)

## My components are split into 5 tasks

OverallAppComponent - contains entirety of the app
MainTaskTable - contains all task components
EachTaskGroup - Each task is put into groups
DailyTask - Daily task information 
UserTask - User duplicates main task group 
UserInput -  User inputs data and buttons


### Arranging components into hierarchy: 
OverallAppComponent
UserTask
MainTaskTable
EachTaskGroup
DailyTask
UserInput


## Identify The Minimal (but complete) Representation Of UI State

#### Noting all of the data from our components. 
1. User input would be needed 
2. The value of checked boxes 
3. Duplication of the task group 
4. Delete a task 
5. Appearance of add task

#### The States are:
1. Adding New task
2. Value of checkboxes
3. Deleting a task

## Identify Where The State Should Live
The list of tasks must be updated when a new task is added, deleted, or checked, and the form must be displayed. The component's common owner is the main application component, OverallAppComponent. The two states should therefore reside in the OverallAppComponent. 
Changes in input and status are reflected in the Main Task Table.



