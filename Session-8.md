# **Day 6 – How Can We Write Shorter, Smarter Functions? Exploring Arrow Functions and Real-World Use Cases**

---

## **1. Main Project (PBL Context): Building a To-Do List Web Application**

**Project Vision:**  
Learners are developing a To-Do app that allows users to:
- Add, view, and manage tasks
- Use JavaScript functions for structured, reusable logic
- Simplify repetitive code using arrow functions and modular logic

> **Today’s Focus:** Learn how to use **arrow functions** in JavaScript and apply functions to real use cases like callbacks, filtering tasks, and handling user events.

---

## **2. Today’s Problem Statement (PSBL)**

### **Standard Problem Statement:**
> Your app needs to handle multiple user actions and task manipulations. How can you write concise, context-aware functions for repeated actions like filtering and updating tasks?

### **Rewritten as User Stories:**
- *As a developer, I want to write shorter and cleaner functions to simplify task operations.*
- *As a user, I want features like filtering completed tasks and responsive UI interactions.*
- *As a learner, I want to understand where arrow functions are useful and how function use cases apply to real projects.*

---

## **3. Learning Objectives**

By the end of this session, learners will be able to:
- Understand and use **arrow function syntax**
- Compare arrow functions with traditional function expressions
- Apply functions in **callbacks**, **event listeners**, and **task filtering**
- Recognize where arrow functions are not ideal (e.g., `this` context)

---

## **4. Scenario-Based Framing**

> Your app needs to display only completed tasks, add event listeners to buttons, and process task data. You need quick, modular, and clean functions that can be passed as callbacks. Arrow functions provide a perfect tool for such modern JS use cases.

You need to:
- Write concise callback functions
- Use arrow functions inside array methods (e.g., `filter()`, `forEach()`)
- Handle DOM events using arrow functions (when `this` is not required)

---

## **5. Mini Visual Roadmap (Descriptive)**

[Start]
↓
Arrow function syntax vs regular function
↓
Use in array methods: filter, forEach, map
↓
Event listeners with arrow functions
↓
Use cases: filtering tasks, button clicks, displaying output
↓
[End]

yaml
Copy
Edit

---

## **6. Conceptual Explanation (Notes + Code Walkthroughs)**

### 🔹 Arrow Function Syntax

```javascript
// Regular function
const greet = function(name) {
  return "Hello, " + name;
};

// Arrow function
const greetArrow = name => "Hello, " + name;
```
🔹 When to Use Arrow Functions
Inside array methods (map(), filter(), forEach())

For quick, inline functions

When this binding is not needed

🔹 When NOT to Use Arrow Functions
In object methods using this

As constructors

🔹 Use Case Example – Filtering Completed Tasks
```
const tasks = [
  { title: "Buy milk", completed: true },
  { title: "Study", completed: false },
  { title: "Call mom", completed: true }
];

const completedTasks = tasks.filter(task => task.completed);
console.log(completedTasks);
```
🔹 Use Case Example – Event Listener
```
document.getElementById("addBtn").addEventListener("click", () => {
  console.log("Task added!");
});
```
## **7. Hands-On Implementation (Code + Integration in Project)**
🔸 Task:
Convert one existing function in your project to an arrow function

Create a filter function to display only completed tasks

Use an arrow function in an event listener (e.g., add button)

🔸 Bonus:
Use forEach() with an arrow function to log each task title

## **8. Output-Based Assessment (with GitHub Push)**
✅ Task 1:
Refactor existing renderTask() or addTask() into an arrow function (if context allows)

Create and test a filterCompleted() arrow function

✅ Task 2:
Push changes to GitHub
Commit message: "Refactored functions to arrow syntax and added task filtering logic"

### **9. Interview Preparation (5 Output-Based Qs)**
Q1:
What is the key difference between an arrow function and a regular function?

a) Arrow functions are faster

b) Arrow functions use their own this

c) Arrow functions do not have their own this
✅ Answer: c) Arrow functions do not have their own this

Q2:
Which of the following is a valid arrow function?

const double = x => x * 2;
✅ Answer: Yes, correct syntax

Q3:
What does this return?

const sayHi = name => "Hi " + name;
console.log(sayHi("Alex"));
✅ Answer: "Hi Alex"

Q4:
When should arrow functions be avoided?

a) In array filtering

b) In event listeners

c) When using this inside object methods
✅ Answer: c) When using this inside object methods

Q5:
What is the output?

[1, 2, 3].forEach(num => console.log(num * 2));
✅ Answer: 2 4 6

## **10. Connection to the Next Problem Statement**
Next Up: Now that you’re organizing your logic into arrow functions and use cases, you’ll learn about scope and closures to retain and control access to variables in functions.

### 📌 Next Session:
Problem: How Can We Store and Protect Variables in Functions?
You will learn:

Function and block scope

Closures and persistent data

Practical closure examples for To-Do apps


---

You can now copy and paste this into any `.md` file (like `day-6-todo-app.md`) using any Markdown editor.

Let me know when you're ready for the next session: **Scope and Closures**!
