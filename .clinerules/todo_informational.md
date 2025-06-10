---
description: Basic overview and architecture of the Todo App.
author:Sristi
version:1.0
globs:["**/*.js", "**/*.ts"]
tags:["documentation","todo-app","react","strapi]
---
#Todo App Overview
##Objective
This is a simple todo application which allows the users to perform crud operations on todo items.

##Tech Stack
-Frontend: React
-Backend: Strapi

##Features
-Create a new todo item
-Update an existing todo item
-Delete a todo item
-Mark a todo item as completed
-Filter todo items based on their status (all, active, completed)
-Sort todo items based on their creation date
-Persist todo items into items Collection type in Strapi
-Display the number of active todo items
-Clear all completed todo items
-Display a message when there are no todo items

##Architecture
The application is built using the following architecture:
-Frontend: React
-Backend: Strapi
-API: REST API

##API Endpoints
The following API endpoints are used in the application:
-GET /api/items: Get all todo items
-POST /api/items: Create a new todo item
-PATCH /api/items/:id: Update an existing todo item
-DELETE /api/items/:id: Delete a todo item

##Definitions
-Todo Item: A todo item is a task that needs to be completed. It has the following properties:
    -id: Unique identifier for the todo item
    -title: Title of the todo item
    -description: Description of the todo item
    -status: Status of the todo item (active, completed)
    -createdAt: Date and time when the todo item was created
