# 📝 To-Do List Web App

A clean and responsive **To-Do List** web application built with **HTML, CSS, and JavaScript**.  
This project demonstrates **modern front-end development skills**, including:

- Local storage persistence  
- Dynamic DOM manipulation  
- Responsive and elegant UI design  
- User-friendly interactions like **marking tasks completed** and **deleting tasks**

---

## 🚀 Features

- ✅ **Add Tasks** – Create new tasks quickly and efficiently.
- ✅ **Mark as Completed** – Click a task to toggle completion with a stylish line-through effect.
- ✅ **Delete Tasks** – Remove tasks instantly using a dedicated delete button.
- ✅ **Persistent Storage** – All tasks are stored in the browser’s `localStorage`, so your list is saved even after refreshing or reopening the browser.
- ✅ **Responsive UI** – Optimized for desktop and mobile screens.

---

## 🖼️ Preview

*(Add a screenshot or animated GIF of your app here for maximum impact, e.g. `screenshot.png`)*

![To-Do List Preview](screenshot.png)

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **HTML5** | Structure of the application |
| **CSS3**  | Responsive and elegant styling |
| **Vanilla JavaScript (ES6)** | Dynamic interactions and localStorage persistence |

---

## 📂 Project Structure
.
├── index.html # Main HTML page
├── style.css # All styles and animations
├── script.js # App logic (add, delete, mark complete, save to localStorage)
└── README.md # Project documentation


---

## ⚡ Getting Started

### 1️⃣ Clone the repository

---

## ⚡ Getting Started

### 1️⃣ Clone the repository
```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name> 
```
### 2️⃣ Open the app

Simply open index.html in your browser.

Or run a local server (recommended):
# Using VS Code Live Server
```bash
Right click on index.html → "Open with Live Server"
```
---
✨ Code Highlights

Task Persistence

let tasks = JSON.parse(localStorage.getItem("tasks")) || [];
localStorage.setItem("tasks", JSON.stringify(tasks));

---
Toggle Completion

```bash
li.addEventListener("click", (event) => {
  if (event.target.tagName === "BUTTON") return;
  task.completed = !task.completed;
  li.classList.toggle("completed");
  saveTask();
});
```

---
Delete with Smooth UX

```bash 
deleteBtn.addEventListener('click',(event)=>{
    event.stopPropagation();
    tasks = tasks.filter(t=> t.id !== task.id);
    li.remove();
    saveTask();
});
```
---
### 🌟 Key Learning & Takeaways

Mastered DOM manipulation without external libraries.

Used localStorage to implement persistent data storage.

Designed a minimal, modern UI with CSS transitions and hover states.

---
### 🤝 How to Contribute

Pull requests and suggestions are welcome!
Feel free to fork the repo and submit a PR with enhancements like:

Task filtering (All / Completed / Pending)

Edit task feature

Drag & drop task sorting

---
### 📜 License

This project is open source and available under the MIT License.

---

### 💡 Why this project stands out to recruiters:

Pure Vanilla JavaScript: Demonstrates core front-end fundamentals without relying on heavy frameworks.

Clean and Modular Code: Easy-to-read structure with separated concerns (HTML/CSS/JS).

Real-World Features: Persistence, state management, and responsive UI are industry-relevant skills.

---
