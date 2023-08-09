# Simple tasks
## 1. ToDo List Application 
Create the basic structure of the database of a simple ToDo List application.
The following tables / models should be available:
- **todo_list** model
- **entry** model
- **category** model
- **user** model

The following requrements should be met:
- the application should support > 1 todo list
- each todo list should support > 1 entries
- each todo list should have up to 1 category
- each todo list should have the following properties:
    - title
    - summary
    - category
- each category should have the following properties:
    - label
    - description
- each entry should have the following properties:
    - description
    - is_complete (boolean, showing whether it is marked or not)
    - timestamp of creation
    - timestamp of update
    - the user, who has created it
    - the user, who has updated it
- each user should have the following properties:
    - username
    - email
    - timestamp of creation

The scope of the task is to perform the following action:
- create the set of models, which meet the above mentioned requirements
- create all the needed relations (Foreign Keys, Primary Keys, etc)
- create the following metrics (queries, which will return the needed data):
    - show information about the percentage of category of todo lists out of all todo lists
    For example - if we have 3 categories (shopping, electric bills, car), what is the percentage of the todo lists for each category?
    - show the count of todo lists per user (for the user you can just show the username)
    - show a summary of how many entries are marked as *done* for each todo list
    - show the entries in a single todo list with the following information:
        - todo_list.title
        - todo_list.summary
        - category.label
        - description
        - is_complete
        - timestamp of creation
        - timestamp of last update
        - user.username (the creator)
        - user.email (the creator)
        - user.username (the one who has last updated it)
        - user.email (the one who has last updated it)


