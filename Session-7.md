
# **Day 5 – How Do We Organize Logic? Understanding JavaScript Functions**

---

## **1. Main Project (PBL Context): Building a To-Do List Web Application**

**Project Vision:**  
Learners are developing a To-Do app that allows users to:
- Add, view, and manage tasks
- Structure functionality for scalability
- Reuse logic across the application

> **Today’s Focus:** Learn how to define and use **JavaScript functions** using declarations and expressions to make code reusable, readable, and organized.

---

## **2. Today’s Problem Statement (PSBL)**

### **Standard Problem Statement:**
> As the application grows, repetitive logic needs to be reusable. How can we structure such logic to avoid rewriting and reduce complexity?

### **Rewritten as User Stories:**
- *As a developer, I want to reuse task-related logic like adding or deleting tasks without repeating code.*
- *As a user, I want the app to behave consistently each time I add or manage a task.*
- *As a learner, I want to understand how to write and use JavaScript functions effectively.*

---

## **3. Learning Objectives**

By the end of this session, learners will be able to:
- Define functions using **declarations** and **expressions**
- Understand function syntax and the concept of parameters and return values
- Write functions for specific To-Do operations
- Call and test functions using real data

---

## **4. Scenario-Based Framing**

> You’ve written working code to add tasks to a list. However, as your app expands, you're duplicating logic. You need to isolate this into functions so that your logic can be reused with different inputs or events.

You need to:
- Create functions for task creation
- Use function parameters for flexibility
- Return values where necessary (e.g., to calculate counts)

---

## **5. Mini Visual Roadmap (Descriptive)**

```
[Start]
   ↓
What is a function and why use one?
   ↓
Function declarations and syntax
   ↓
Function expressions and calling functions
   ↓
Build functions for adding and displaying tasks
   ↓
[End]
```

---

## **6. Conceptual Explanation (Notes + Code Walkthroughs)**

### 🔹 Function Declaration

```javascript
function addTask(taskName) {
  console.log("Adding task:", taskName);
}
addTask("Buy groceries");
```

### 🔹 Function Expression

```javascript
const showTask = function(taskName) {
  console.log("Task is:", taskName);
};
showTask("Submit homework");
```

### 🔹 Key Concepts:
- Function **parameters** accept input
- `return` keyword sends data back
- Named vs anonymous functions

---

### 🔹 Task-Specific Example:

```javascript
function createTaskElement(task) {
  const li = document.createElement("li");
  li.textContent = task;
  return li;
}
const taskItem = createTaskElement("Read book");
document.getElementById("taskList").appendChild(taskItem);
```

---

## **7. Hands-On Implementation (Code + Integration in Project)**

### 🔸 Tasks:
- Create a function `addTask(task)` that logs the task name
- Create another function `renderTask(task)` that appends a `<li>` to the task list
- Test both functions by calling them with different task names

### 🔸 Bonus:
- Modify `renderTask()` to include a "Delete" button
- Wrap the delete logic in a `deleteTask()` function

---

## **8. Output-Based Assessment (with GitHub Push)**

### ✅ Task 1:
- Create and test functions for adding and displaying tasks
- Log relevant output using `console.log()`

### ✅ Task 2:
- Push code to GitHub  
  **Commit message:** `"Added reusable functions for adding and rendering tasks"`

---

## **9. Interview Preparation (5 Output-Based Qs)**

### **Q1:**
What is the correct way to define a function?

- a) `function = myFunc() {}`  
- b) `func myFunc() {}`  
- c) `function myFunc() {}`  
✅ **Answer:** c) `function myFunc() {}`

---

### **Q2:**
What is the main difference between a function declaration and expression?

- a) Declarations are hoisted  
- b) Expressions are faster  
- c) Both are the same  
✅ **Answer:** a) Declarations are hoisted

---

### **Q3:**
What will this code output?

```javascript
function greet(name) {
  return "Hi " + name;
}
console.log(greet("Sara"));
```

✅ **Answer:** `"Hi Sara"`

---

### **Q4:**
What does `return` do in a function?

- a) Logs to console  
- b) Exits the program  
- c) Sends data out of the function  
✅ **Answer:** c) Sends data out of the function

---

### **Q5:**
Can you assign a function to a variable?

- a) No  
- b) Only in ES6  
- c) Yes, using function expressions  
✅ **Answer:** c) Yes, using function expressions

---

## **10. Connection to the Next Problem Statement**

> **Next Up:** Now that we understand how to write reusable logic using functions, we’ll explore arrow functions and how they simplify our syntax and interact with scope.

📌 **Next Session:**  
**Problem:** How Can We Write Shorter Functions That Remember Context?  
You will learn:
- Arrow function syntax
- Function scope and lexical `this`
- Writing callbacks with arrow functions
