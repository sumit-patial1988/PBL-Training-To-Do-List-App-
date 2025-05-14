# PBL-Training-To-Do-List-App-

# **Day 1 – Where Do We Start? Understanding To-Do App Architecture**

---

## **1. Main Project (PBL Context): Building a To-Do List Web Application**

**Project Vision:**  
By the end of this project-based training, learners will build a **fully functional To-Do application** that:
- Allows users to add, edit, delete, and mark tasks as complete
- Stores data in the browser (local storage)
- Features a clean and responsive UI
- Is built using HTML, CSS, and JavaScript only (no frameworks)

> **Today’s Focus:** Introduce the project, break down its architecture, and cover JavaScript fundamentals to prepare for logic building in upcoming sessions.

---

## **2. Today’s Problem Statement (PSBL)**

### **Standard Problem Statement:**
> You're tasked with building a To-Do app, but before jumping into code, you must understand what parts make up the app and how JavaScript will drive its behavior.

### **Rewritten as User Stories:**
- *As a user, I want to add tasks to a list so I can remember what to do.*
- *As a developer, I want to break the app into logical components so I can write cleaner code.*
- *As a beginner in JavaScript, I want to understand variables, data types, and basic syntax to start implementing logic.*

---

## **3. Learning Objectives**

By the end of this session, learners will be able to:
- Explain the core features and UI of a typical To-Do app
- Identify major architectural components: UI, logic, and data storage
- Understand JavaScript basics: syntax, variables, data types, and operators
- Set up a basic HTML/CSS structure for the app

---

## **4. Scenario-Based Framing**

> You’re hired as a junior web developer at a productivity startup. Your first task is to create the foundation for a to-do app that thousands of users will rely on daily. You need to break it down into parts and get the structure ready before adding full functionality.

You need to:
- Create the base layout for a task manager
- Learn the basic JavaScript building blocks to control behavior
- Prepare for logic like adding or deleting tasks in future sessions

---

## **5. Mini Visual Roadmap (Descriptive)**

```
[Start]
   ↓
Project overview and feature breakdown
   ↓
Understand HTML structure of To-Do UI
   ↓
Style basic layout with CSS
   ↓
Learn JavaScript syntax and variables
   ↓
Practice: Declare variables and log them
   ↓
[End]
```

---

## **6. Conceptual Explanation (Notes + Code Walkthroughs)**

### 🔹 To-Do App Breakdown:
- **Input field** to add new tasks
- **Task list** to display all tasks
- **Buttons** to mark complete or delete
- **Storage** using localStorage (future session)

### 🔹 HTML Essentials:
- `<input type="text">`, `<button>`, `<ul>`, `<li>`
- Semantic structure: `<header>`, `<main>`

### 🔹 JavaScript Basics:
- `var`, `let`, `const` and their scopes
- Data types: string, number, boolean, null, undefined
- Simple operations and `console.log()`

### 🔹 Sample HTML Skeleton:
```html
<header>
  <h1>📝 My To-Do List</h1>
</header>

<main>
  <input type="text" id="taskInput" placeholder="Enter a new task" />
  <button id="addBtn">Add Task</button>
  <ul id="taskList"></ul>
</main>
```

### 🔹 Sample JavaScript Snippet:
```javascript
let taskName = "Buy groceries";
console.log("Task:", taskName); // Output: Task: Buy groceries
```

---

## **7. Hands-On Implementation (Code + Integration in Project)**

### 🔸 Folder Structure:
```
/todo-app
  ├── index.html
  ├── style.css
  └── script.js
```

### 🔸 Task:
- Set up basic HTML structure with input, button, and empty list
- Link CSS and JS files
- Write JS code to declare a task variable and print to console

---

## **8. Output-Based Assessment (with GitHub Push)**

### ✅ Task 1:
- Build a static layout with an input field and a button
- Include an empty list area for tasks
- Use placeholder content and basic CSS styling

### ✅ Task 2:
- Push code to GitHub with README
- Commit message: `"Initial layout and basic JavaScript setup"`

---

## **9. Interview Preparation (5 Output-Based Qs)**

### **Q1:**
What does this code output?
```javascript
let task = "Read book";
console.log(typeof task);
```
✅ **Answer:** `"string"`

---

### **Q2:**
What will happen if you use `const` but try to change its value?

- a) Changes value normally  
- b) Throws an error  
- c) Ignores the change  
- d) Converts to `let`

✅ **Answer:** b) Throws an error

---

### **Q3:**
What tag is best used to group tasks in a list?

- a) `<div>`  
- b) `<table>`  
- c) `<ul>`  
- d) `<form>`

✅ **Answer:** c) `<ul>`

---

### **Q4:**
Which of the following is a valid variable name?

- a) `2task`  
- b) `task-list`  
- c) `_task`  
- d) `let`

✅ **Answer:** c) `_task`

---

### **Q5:**
What does `console.log("3" + 3)` output?

- a) `6`  
- b) `33`  
- c) `Error`  
- d) `undefined`

✅ **Answer:** b) `33`

---

## **10. Connection to the Next Problem Statement**

> **Next Up:** Now that we have a layout and basic JavaScript setup, we’ll build interactivity — capturing tasks from the input field and displaying them on the screen.

📌 **Next Session:**  
**Problem:** How Can We Add Tasks Dynamically?  
You will learn:
- DOM selection and manipulation
- Event handling with `addEventListener`
- Dynamically adding elements with JavaScript
