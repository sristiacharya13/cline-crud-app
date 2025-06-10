---
description: Process for creating, updating, and deleting todo items.
author:Sristi
version:1.0
globs:["**/*.js", "**/*.ts"]
tags:["process","todo-app","react","strapi"]
---
#Todo App Process
##Creating a new todo item
1. User fills out the form with the title and description of the todo item.
2. User clicks the "Add" button.
3. The form data is sent to the backend via a POST request to the /api/items endpoint.
4. The backend creates a new todo item in the items Collection type with the provided data and a status of "active".
5. The backend returns the newly created todo item to the frontend.
6. The frontend adds the new todo item to the list of todo items and clears the form.

##Updating an existing todo item
1. User clicks on the todo item they want to update.
2. The frontend sends a GET request to the /api/items/:id endpoint to retrieve the todo item data.
3. The backend returns the todo item data to the frontend.
4. The frontend displays the todo item data in the form.
5. User updates the title and/or description of the todo item.
6. User clicks the "Save" button.
7. The updated todo item data is sent to the backend via a PATCH request to the /api/items/:id endpoint.
8. The backend updates the todo item in the items Collection type with the provided data.
9. The backend returns the updated todo item to the frontend.
10. The frontend updates the todo item in the list of todo items.

##Deleting a todo item
1. User clicks on the todo item they want to delete.
2. The frontend sends a DELETE request to the /api/items/:id endpoint to delete the todo item.
3. The backend deletes the todo item from the items Collection type.
4. The backend returns a success message to the frontend.
5. The frontend removes the todo item from the list of todo items.

##Decision points
-If input is empty, then throw an error.
-If input is not empty, then create a new todo item.

##Tools used
-Axios
-useState, useEffect
-Strapi
-REST API

##Inputs/Outputs
-Input: Title and description of the todo item
-Output: New todo item created in the items Collection type in Strapi

##Dependencies
-Ensure Strapi is running and the items Collection type is created.