# **Day 3 – How Do We Operate on Tasks? Understanding JavaScript Operators & Expressions**

---

## **1. Main Project (PBL Context): Building a To-Do List Web Application**

**Project Vision:**  
By the end of this project-based training, learners will have created a **To-Do application** that:
- Allows users to manage a list of tasks
- Supports interactivity using JavaScript logic
- Uses expressions to control UI behaviors and user interactions

> **Today’s Focus:** Learn to apply JavaScript operators and expressions to evaluate and manipulate data, especially for user-driven actions like task updates.

---

## **2. Today’s Problem Statement (PSBL)**

### **Standard Problem Statement:**
> Your app needs to make decisions — like marking tasks as complete or counting pending items. How do you process these conditions and values in code?

### **Rewritten as User Stories:**
- *As a user, I want to see how many tasks I’ve completed or missed.*
- *As a developer, I want to use expressions to update UI behavior based on task data.*
- *As a learner, I want to practice writing and evaluating JavaScript expressions.*

---

## **3. Learning Objectives**

By the end of this session, learners will be able to:
- Use arithmetic, assignment, comparison, and logical operators
- Understand expression evaluation in JavaScript
- Write conditional and mathematical expressions
- Apply operators in To-Do app logic (e.g., counters, toggles)

---

## **4. Scenario-Based Framing**

> You’re implementing the logic for tracking task progress. Each time a task is added or marked complete, you must update counters, change UI states, and validate input. Operators and expressions help you process this logic reliably.

You need to:
- Calculate totals (`totalTasks + 1`)
- Toggle task completion status
- Compare values to trigger specific code paths

---

## **5. Mini Visual Roadmap (Descriptive)**

[Start]
↓
Introduce operators and types
↓
Write simple arithmetic and logic-based expressions
↓
Apply operators to real task scenarios
↓
Build dynamic counters and toggles
↓
[End]

markdown
Copy
Edit

---

## **6. Conceptual Explanation (Notes + Code Walkthroughs)**

### 🔹 Types of Operators:

- **Arithmetic Operators**: `+`, `-`, `*`, `/`, `%`
- **Assignment Operators**: `=`, `+=`, `-=`
- **Comparison Operators**: `==`, `===`, `!=`, `>`, `<`, `>=`, `<=`
- **Logical Operators**: `&&`, `||`, `!`
- **Ternary Operator**: `condition ? true : false`

---

### 🔹 Sample Code 1: Arithmetic & Assignment

```javascript
let totalTasks = 3;
totalTasks += 1; // totalTasks is now 4
let completedTasks = 2;
let pendingTasks = totalTasks - completedTasks;
```
### 🔹Sample Code 2: Logical & Comparison
```
let isCompleted = false;

if (!isCompleted) {
  console.log("Task is still pending.");
}

let message = completedTasks === totalTasks ? "All done!" : "Tasks remaining!";
console.log(message);
```
### 7. Hands-On Implementation (Code + Integration in Project)
🔸 Task:
Declare totalTasks and completedTasks

Calculate pending tasks

Use a ternary expression to log a message based on task status

🔸 Bonus:
Create a Boolean isCompleted variable

Toggle its value using !isCompleted

Log different UI states based on its value

### 8. Output-Based Assessment (with GitHub Push)
✅ Task 1:
Use arithmetic and logical operators to simulate task tracking

Log each calculation using console.log()

✅ Task 2:
Push the script to GitHub with the commit message:
"Added task logic using operators and expressions"

### 9. Interview Preparation (5 Output-Based Qs)
Q1:
What is the output of:

5 + "3"
a) 8

b) 53

c) "53"

d) Error
✅ Answer: c) "53" – string concatenation

Q2:
What does !== check for?

a) Value only

b) Reference

c) Value and type

d) Nothing
✅ Answer: c) Value and type

Q3:
What is the result of true && false?

a) true

b) false

c) undefined

d) Error
✅ Answer: b) false

Q4:
What does !true return?

a) true

b) false
✅ Answer: b) false

Q5:
What is the result of:

let x = 4;
x += 2;
console.log(x);
a) 6

b) 2

c) 4
✅ Answer: a) 6

10. Connection to the Next Problem Statement
Next Up: Now that we know how to store and evaluate data, let’s use it to control app behavior using conditions and loops.

📌 Next Session:
Problem: How Do We Control What Happens Next?
You will learn:

if-else, switch-case, and loops (for, while, do-while)

Apply logic to display, hide, or modify tasks dynamically








