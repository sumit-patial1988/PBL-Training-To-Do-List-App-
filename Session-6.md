
# **Day 4 – How Can We Repeat Tasks? Mastering JavaScript Loops**

---

## **1. Main Project (PBL Context): Building a To-Do List Web Application**

**Project Vision:**  
Learners are building a dynamic **To-Do list web application** where users can:
- Add and manage tasks
- Track task status (complete/incomplete)
- Store tasks and display lists dynamically

> **Today’s Focus:** Learn how to use **loops in JavaScript** to process multiple tasks, display them in the UI, and perform repetitive logic (like counting or clearing).

---

## **2. Today’s Problem Statement (PSBL)**

### **Standard Problem Statement:**
> Your app will have multiple tasks. How do you go through each one to display, update, or check them?

### **Rewritten as User Stories:**
- *As a user, I want to see all my tasks displayed clearly, even when there are many.*
- *As a developer, I want to loop through tasks to render them dynamically.*
- *As a learner, I want to understand how loops help repeat actions efficiently.*

---

## **3. Learning Objectives**

By the end of this session, learners will be able to:
- Use `for`, `while`, and `do-while` loops in JavaScript
- Loop through arrays of tasks
- Dynamically display a list of tasks using JavaScript and DOM
- Understand loop control: `break`, `continue`

---

## **4. Scenario-Based Framing**

> You’ve built the logic to add tasks. But now, you want to **display all tasks from an array** each time the user opens the app or adds a new task. Manually coding each one isn’t efficient. **Loops** let you automate this based on task count.

You need to:
- Loop through an array of tasks
- Dynamically display tasks in the HTML
- Count completed and pending tasks

---

## **5. Mini Visual Roadmap (Descriptive)**

```
[Start]
   ↓
Understand when and why to use loops
   ↓
Explore `for`, `while`, and `do-while` with examples
   ↓
Loop through a static task array
   ↓
Render each task using `innerHTML` or DOM methods
   ↓
Practice loop control with `break` and `continue`
   ↓
[End]
```

---

## **6. Conceptual Explanation (Notes + Code Walkthroughs)**

### 🔹 Types of Loops:
- `for`: Traditional and most commonly used
- `while`: Used when number of iterations isn’t predetermined
- `do-while`: Executes at least once before condition check

---

### 🔹 Sample Loop Examples:

```javascript
// For Loop
for (let i = 0; i < 5; i++) {
  console.log("Task number", i);
}

// While Loop
let count = 0;
while (count < 3) {
  console.log("Counting task:", count);
  count++;
}

// Do-While Loop
let index = 0;
do {
  console.log("Do at least once:", index);
  index++;
} while (index < 1);
```

---

### 🔹 Looping Over an Array of Tasks:

```javascript
const tasks = ["Buy groceries", "Finish project", "Call John"];

for (let i = 0; i < tasks.length; i++) {
  console.log(`Task ${i + 1}: ${tasks[i]}`);
}
```

---

## **7. Hands-On Implementation (Code + Integration in Project)**

### 🔸 Task:
- Create an array of 5 dummy task names
- Use a `for` loop to display them in the console
- Use DOM methods to render each task as a `<li>` in an unordered list

### 🔸 Bonus:
- Track completed task count using a loop and condition (`if (isCompleted)`)
- Practice breaking a loop early (`if (task === "Break") break;`)

---

## **8. Output-Based Assessment (with GitHub Push)**

### ✅ Task 1:
- Build a JavaScript function to loop through a task array and display them in the UI

### ✅ Task 2:
- Use at least two types of loops (`for` and `while`)
- Push changes to GitHub  
  **Commit message:** `"Implemented task list rendering using loops"`

---

## **9. Interview Preparation (5 Output-Based Qs)**

### **Q1:**
What is the output of:
```javascript
for (let i = 0; i < 3; i++) {
  console.log(i);
}
```

- a) `0 1 2`  
- b) `1 2 3`  
- c) `0 1 2 3`  
✅ **Answer:** a) `0 1 2`

---

### **Q2:**
What’s the difference between `while` and `do-while`?

- a) Nothing  
- b) `while` executes once by default  
- c) `do-while` runs at least once  
✅ **Answer:** c) `do-while` runs at least once

---

### **Q3:**
Which loop is best when the number of iterations is known?

- a) `while`  
- b) `do-while`  
- c) `for`  
✅ **Answer:** c) `for`

---

### **Q4:**
What keyword skips to the next iteration in a loop?

- a) `skip`  
- b) `continue`  
- c) `next`  
✅ **Answer:** b) `continue`

---

### **Q5:**
What is the value of `i` after this loop?
```javascript
let i = 0;
while (i < 3) {
  i++;
}
```

- a) `2`  
- b) `3`  
- c) `4`  
✅ **Answer:** b) `3`

---

## **10. Connection to the Next Problem Statement**

> **Next Up:** Now that we can display tasks using loops, we’ll focus on how to handle user input and events to create dynamic interactions.

📌 **Next Session:**  
**Problem:** How Do We Handle User Actions?  
You will learn:
- JavaScript event listeners
- Capturing user input to add tasks
- Real-time updates with DOM manipulation
