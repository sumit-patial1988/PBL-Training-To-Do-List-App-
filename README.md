
# **Day 5 – Task Type Detected! What Should Happen?**

---

## **1. Main Project (PBL Context): Building a To-Do App with HTML, CSS, and JavaScript**

**Project Vision:**  
By the end of this project, learners will build a **functional To-Do List application** that:
- Allows users to manage daily tasks efficiently
- Supports task filtering and categorization
- Uses **JavaScript control structures** for dynamic interactions
- Features an extendable UI for multiple task types and logic layers

> **Today’s Focus:** Using the **`switch` statement** in JavaScript to handle task types and actions in a structured, scalable manner.

---

## **2. Today’s Problem Statement (PSBL)**

### **Standard Problem Statement:**
> Your To-Do app supports different types of tasks: personal, work, and urgent. Each task type needs to be handled differently in terms of UI and behavior. How can you write clean, scalable logic for this?

### **Rewritten as User Stories:**
- *As a user, I want different icons/colors for task types like personal, work, or urgent.*
- *As a developer, I want to use a structured control method (like `switch`) to avoid long chains of `if-else` conditions.*
- *As a developer, I want to build scalable logic that’s easy to extend if new task types are added later.*

---

## **3. Learning Objectives**

By the end of this session, learners will be able to:
- Understand the syntax and behavior of the `switch` statement
- Use `switch` to execute specific logic based on task type
- Implement branching logic in a scalable format
- Apply dynamic CSS classes or icons based on task types

---

## **4. Scenario-Based Framing**

> You’ve received feedback that your To-Do app needs to **differentiate between task categories** like “Personal,” “Work,” and “Urgent.” Each type should look different and behave differently.

You decide to use a `switch` statement to handle this logic cleanly.

---

## **5. Mini Visual Roadmap (Descriptive)**

```
[Start]
   ↓
User adds a task and selects type
   ↓
switch (type) {
  case "personal" → Add blue tag
  case "work" → Add green tag
  case "urgent" → Add red tag
}
   ↓
Display task with tag or icon
   ↓
[End]
```

---

## **6. Conceptual Explanation (Notes + Code Walkthroughs)**

### 🔹 JavaScript Switch Statement

```js
switch (expression) {
  case value1:
    // code block
    break;
  case value2:
    // code block
    break;
  default:
    // code block
}
```

### 🔹 Example: Tagging Tasks Based on Type

```js
function getTaskTag(type) {
  let tagClass;
  switch (type) {
    case "personal":
      tagClass = "tag-blue";
      break;
    case "work":
      tagClass = "tag-green";
      break;
    case "urgent":
      tagClass = "tag-red";
      break;
    default:
      tagClass = "tag-default";
  }
  return tagClass;
}
```

### 🔹 HTML Sample

```html
<select id="taskType">
  <option value="personal">Personal</option>
  <option value="work">Work</option>
  <option value="urgent">Urgent</option>
</select>
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

### 🔸 `index.html`

```html
<input id="taskInput" placeholder="Add a task" />
<select id="taskType">
  <option value="personal">Personal</option>
  <option value="work">Work</option>
  <option value="urgent">Urgent</option>
</select>
<button onclick="addTask()">Add</button>
<ul id="taskList"></ul>
```

### 🔸 `style.css`

```css
.tag-blue { background-color: lightblue; }
.tag-green { background-color: lightgreen; }
.tag-red { background-color: lightcoral; }
```

### 🔸 `script.js`

```js
function addTask() {
  const taskText = document.getElementById("taskInput").value.trim();
  const taskType = document.getElementById("taskType").value;
  const taskList = document.getElementById("taskList");

  if (taskText === "") {
    alert("Task cannot be empty!");
    return;
  }

  const li = document.createElement("li");
  const tagClass = getTaskTag(taskType);
  li.textContent = taskText;
  li.classList.add(tagClass);
  taskList.appendChild(li);
}

function getTaskTag(type) {
  let tagClass;
  switch (type) {
    case "personal":
      tagClass = "tag-blue";
      break;
    case "work":
      tagClass = "tag-green";
      break;
    case "urgent":
      tagClass = "tag-red";
      break;
    default:
      tagClass = "tag-default";
  }
  return tagClass;
}
```

---

## **8. Output-Based Assessment (with GitHub Push)**

### ✅ Task 1:
Use `switch` to apply different styles based on task type.

### ✅ Task 2:
Add a new task type called `"misc"` and apply a yellow tag.

### ✅ Task 3:
Push the working app to GitHub with the message: `"Added switch logic for task type styling"`.

---

## **9. Interview Preparation (5 Output-Based Qs)**

### **Q1:**
```js
switch(3) {
  case 1:
    console.log("One");
    break;
  case 2:
    console.log("Two");
    break;
  default:
    console.log("Default");
}
```

What will be printed?

- a) One  
- b) Two  
- c) Default  
- d) Error  

✅ **Answer:** c) Default

---

### **Q2:**  
What happens if you omit `break` in a switch statement?

- a) The code exits the switch  
- b) It throws an error  
- c) The next case executes (fall-through)  
- d) Skips the case entirely  

✅ **Answer:** c) The next case executes (fall-through)

---

### **Q3:**  
Which of the following is NOT valid in a switch statement?

- a) `switch(variable)`  
- b) `case "value"`  
- c) `case > 10:`  
- d) `default:`  

✅ **Answer:** c) `case > 10:`

---

### **Q4:**  
Switch is most useful when:

- a) All conditions are boolean  
- b) Many numeric or string cases need checking  
- c) Only two cases exist  
- d) None of the above  

✅ **Answer:** b) Many numeric or string cases need checking

---

### **Q5:**  
Which switch syntax is correct?

- a) `switch x { case 1: ... }`  
- b) `switch (x) { case 1: ... }`  
- c) `switch(x) case 1: {}`  
- d) `switch => x {}`  

✅ **Answer:** b) `switch (x) { case 1: ... }`

---

## **10. Connection to the Next Problem Statement**

> **Next Up:** You’re showing tags now — but users want to **filter** tasks by type. How do you implement filters efficiently?

📌 **Next Session:**  
**Problem:** "Only Show Me Work Tasks!"  
You will learn:
- How to use **filtering with JavaScript**
- Dynamic DOM manipulation
- Conditional rendering based on user selection
