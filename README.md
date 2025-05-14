# **Day 2 – JavaScript Basics: Variables and Data Types**

---

## **1. Main Project (PBL Context): Building a To-Do List Web Application**

**Project Vision:**  
By the end of this project-based training, learners will build a **fully functional To-Do application** that:
- Allows users to add, edit, delete, and mark tasks as complete
- Stores data in the browser (local storage)
- Features a clean and responsive UI
- Is built using HTML, CSS, and JavaScript only (no frameworks)

> **Today’s Focus:** Strengthening the JavaScript foundation by exploring variables, constants, and data types used in building application logic.

---

## **2. Today’s Problem Statement (PSBL)**

### **Standard Problem Statement:**
> Your app needs to store task information like names, status, and IDs. To do that, you need to understand how variables work and what type of data you’re handling.

### **Rewritten as User Stories:**
- *As a user, I want my task details to be stored accurately so I can manage my work efficiently.*
- *As a developer, I want to choose the right type of variable and data type so that my app behaves predictably.*
- *As a beginner, I want to learn how to declare variables and identify data types in JavaScript.*

---

## **3. Learning Objectives**

By the end of this session, learners will be able to:
- Declare variables using `var`, `let`, and `const`
- Identify and use JavaScript data types correctly
- Use `typeof` to check data types
- Log and debug variable values in the console

---

## **4. Scenario-Based Framing**

> You are working on the logic of your to-do app and need to store tasks, their statuses (complete/incomplete), and manage counts. Choosing the right variable and data type ensures your app is accurate and easy to scale.

You need to:
- Store task names as strings
- Track completed status as booleans
- Keep count of total tasks using numbers

---

## **5. Mini Visual Roadmap (Descriptive)**

[Start]
↓
Discuss variable declaration and differences between var, let, const
↓
Understand primitive data types
↓
Use typeof to debug and check values
↓
Try declaring different types of task-related data
↓
[End]

markdown
Copy
Edit

---

## **6. Conceptual Explanation (Notes + Code Walkthroughs)**

### 🔹 JavaScript Variable Declarations:
- `var` – function-scoped (legacy)
- `let` – block-scoped, allows reassignment
- `const` – block-scoped, immutable reference

### 🔹 Primitive Data Types:
- String (`"Complete assignment"`)
- Number (`5`, `3.14`)
- Boolean (`true`, `false`)
- Null, Undefined, Symbol (brief mention)

### 🔹 Sample Snippet 1:
```javascript
let taskName = "Write report";
const totalTasks = 5;
var isComplete = false;
console.log(typeof taskName); // "string"
```
### 🔹 Sample Snippet 2 (undefined vs null):
```
let taskDescription;
console.log(taskDescription); // undefined

let taskNotes = null;
console.log(taskNotes); // null
```
### 7. Hands-On Implementation (Code + Integration in Project)
🔸 Task:
Open script.js in the project folder

Declare variables to store:

Task name (string)

Task status (boolean)

Task count (number)

Use console.log() to check types

🔸 Bonus:
Change let values and try reassigning const

Observe browser console behavior

### 8. Output-Based Assessment (with GitHub Push)
✅ Task 1:
Declare 3 types of variables: string, number, boolean

Use console.log() to display them

✅ Task 2:
Add comments explaining the data type of each variable

Push to GitHub with commit message: "Added JS variable examples"

### 9. Interview Preparation (5 Output-Based Qs)
Q1:
Which keyword prevents reassignment of a variable?

a) var

b) let

c) const

d) static
✅ Answer: c) const

Q2:
What is the output of this code?

let a;
console.log(typeof a);
a) "undefined"

b) "null"

c) "object"

d) "string"
✅ Answer: a) "undefined"

Q3:
Which of the following is a valid JavaScript variable name?

a) 123task

b) task-name

c) taskList

d) let
✅ Answer: c) taskList

Q4:
What is the output of typeof null?

a) "null"

b) "undefined"

c) "object"

d) "boolean"
✅ Answer: c) "object" (quirk in JavaScript)

Q5:
What is the default value of an uninitialized let variable?

a) null

b) undefined

c) 0

d) false
✅ Answer: b) undefined

10. Connection to the Next Problem Statement
Next Up: Now that we know how to declare variables and store data, we’ll learn how to use control structures to make decisions in our application.

📌 Next Session:
Problem: How Can We Check and Control Task Behavior?
You will learn:

Conditional logic using if, else, and switch

Comparison and logical operators


---

Let me know when you'd like the **PDF version**, or if you'd like help building the **next s
