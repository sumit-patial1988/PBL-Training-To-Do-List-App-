
# **Day 7 – How Can We Control and Protect Data in Functions? Understanding Scope and Closures**

---

## **1. Main Project (PBL Context): Building a To-Do List Web Application**

**Project Vision:**  
Learners are creating a fully functional To-Do app where task logic is modular, secure, and scalable. They need to:
- Store task data efficiently
- Ensure internal variables aren't exposed unnecessarily
- Organize code that maintains state across user interactions

> **Today’s Focus:** Learn how JavaScript uses **scope** and **closures** to manage data access and create private, persistent function states.

---

## **2. Today’s Problem Statement (PSBL)**

### **Standard Problem Statement:**
> Your app’s logic must manage task counters and track internal states (e.g., completed tasks) without exposing everything globally. How do you protect this data?

### **Rewritten as User Stories:**
- *As a user, I want the task count to update accurately, even after multiple actions.*
- *As a developer, I want to limit what variables are accessible globally to avoid bugs.*
- *As a learner, I want to understand how scope and closures help in preserving and protecting function data.*

---

## **3. Learning Objectives**

By the end of this session, learners will be able to:
- Understand block, function, and global **scope**
- Define and use **closures** in JavaScript
- Create **private variables** using closures
- Apply closures to store task counts or flags in the To-Do app

---

## **4. Scenario-Based Framing**

> You're working on a feature to show the number of completed tasks. You want this value to be updated when a task is completed — but not accidentally modified elsewhere in your code. Using closures, you can protect this logic while still accessing the data when needed.

You need to:
- Track task status changes safely
- Avoid exposing variables globally
- Return functions that remember previous values

---

## **5. Mini Visual Roadmap (Descriptive)**

```
[Start]
   ↓
What is scope? (block, function, global)
   ↓
What is a closure? Why is it useful?
   ↓
Write examples of functions that return functions
   ↓
Use closure to create a private task counter
   ↓
[End]
```

---

## **6. Conceptual Explanation (Notes + Code Walkthroughs)**

### 🔹 JavaScript Scope

```javascript
let globalVar = "Global";

function exampleScope() {
  let localVar = "Local";
  console.log(globalVar); // Accessible
  console.log(localVar);  // Accessible
}

console.log(localVar); // ❌ Error: not defined
```

---

### 🔹 What Is a Closure?

A **closure** is when a function **remembers the variables** from the scope in which it was created, even after that scope is closed.

---

### 🔹 Closure Example – Task Counter

```javascript
function taskCounter() {
  let count = 0;
  return function () {
    count++;
    return count;
  };
}

const increment = taskCounter();
console.log(increment()); // 1
console.log(increment()); // 2
```

---

### 🔹 Use Case: Private Completed Task Tracker

```javascript
function createCompletedTracker() {
  let completed = 0;

  return {
    increment: () => completed++,
    getCount: () => completed
  };
}

const tracker = createCompletedTracker();
tracker.increment();
tracker.increment();
console.log(tracker.getCount()); // 2
```

---

## **7. Hands-On Implementation (Code + Integration in Project)**

### 🔸 Tasks:
- Create a closure to track the number of completed tasks
- Use a function that returns another function
- Integrate the closure with task status toggling in your app

### 🔸 Bonus:
- Create a closure to generate unique task IDs

---

## **8. Output-Based Assessment (with GitHub Push)**

### ✅ Task 1:
- Build a closure that maintains a private `completedCount`
- Log `getCompletedCount()` result to verify correct output

### ✅ Task 2:
- Push code to GitHub  
  **Commit message:** `"Implemented closure for private task counter"`

---

## **9. Interview Preparation (5 Output-Based Qs)**

### **Q1:**
What type of scope is created inside a function?

- a) Global  
- b) Block  
- c) Function  
✅ **Answer:** c) Function

---

### **Q2:**
Which keyword defines block scope?

- a) `var`  
- b) `let`  
- c) `function`  
✅ **Answer:** b) `let`

---

### **Q3:**
What will this code output?

```javascript
function makeCounter() {
  let count = 0;
  return () => ++count;
}

const counter = makeCounter();
console.log(counter()); // ?
```

✅ **Answer:** `1`

---

### **Q4:**
Why use closures?

- a) To log to console  
- b) To reset scope  
- c) To maintain private persistent data  
✅ **Answer:** c) To maintain private persistent data

---

### **Q5:**
True or False: Closures can access variables from their outer function even after the outer function has finished executing.

✅ **Answer:** True

---

## **10. Connection to the Next Problem Statement**

> **Next Up:** We’ve learned to organize and protect our logic — now it’s time to persist user data with **Local Storage** so tasks don’t disappear on refresh.

📌 **Next Session:**  
**Problem:** How Can We Save Tasks in the Browser?  
You will learn:
- Reading from and writing to local storage
- Serializing data with `JSON.stringify()` and `JSON.parse()`
- Auto-saving tasks to browser memory
