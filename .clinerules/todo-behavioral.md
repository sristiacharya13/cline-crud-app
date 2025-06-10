---
description: Instructional rules for AI assisting with Todo App development.
author:Sristi
version:1.0
globs:["**/*.js", "**/*.ts"]
tags:["behavioral","todo-app","react","strapi"]
---
#AI Assistance for Todo App Development

##⚠️ CRITICAL ⚠️
-✅ Always validate todo title before submitting a new todo item.
-❌ Never submit a new todo item without a title.

##Implement validation
✅ Correct:
```jsx
if (!input.trim()) {
  setError("Todo cannot be empty");
}

❌ Incorrect:
```jsx
if (input == "") alert("error");
```
###Test each feature
-✅ Create
-✅ Update
-✅ Delete
-✅ Mark as completed
-✅ Filter
-✅ Sort
-✅ Display number of active todo items
-✅ Display message when there are no todo items
⚠️ DO NOT PROCEED IF ANY FAIL

##DO NOT SKIP❗
✅ STOP AND VERIFY:
-All features tested individually.
-Output format is consistent (e.g., id, title, completed).
-No console errors.

##Key Requirements
-✅ Must validate input on frontend and backend.
-✅ Must use error boundaries and logs.
-✅ Must verify every endpoint with real input.
-✅ Must NOT deploy untested code.