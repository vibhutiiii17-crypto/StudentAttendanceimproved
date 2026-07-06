# Lab 5 — Student Attendance System (Vanilla JS)

> **Christ University Bangalore · MCA · 1st Trimester · Full Stack Development**

---

## 📋 About

This is **Lab 5** of the Full Stack Development practical. It implements a **Student Attendance Management System** using **pure / vanilla HTML, CSS, and JavaScript** — no frameworks, no libraries, no build tools.

The project was built alongside a React.js version of the same app to demonstrate and compare the two development paradigms.

---

## 🚀 How to Run

No installation required. Simply open the file in any modern browser:

```
vanilla/index.html  →  double-click OR drag into browser
```

Or right-click → **Open with** → Chrome / Edge / Firefox.

---

## ✨ Features

| Feature | Details |
|---|---|
| **Student Form** | Enter name, register number, course, and attendance status |
| **Validation** | Inline error messages for empty / invalid fields |
| **Attendance Status** | Toggle between **Present** and **Absent** via pill buttons |
| **Result Panel** | Displays submitted student details with a status badge |
| **Animated Reveal** | Result panel fades in with a smooth animation on submit |
| **Responsive Layout** | Two-column grid collapses to single column on mobile |
| **No Dependencies** | Zero npm packages, zero CDN libraries |

---

## 🗂 File Structure

```
vanilla/
├── index.html    ← entire app (HTML + CSS + JS in one file)
└── README.md     ← this file
```

### Inside `index.html`

| Section | Lines | Description |
|---|---|---|
| `<head>` + `<style>` | 1–435 | CSS design tokens, layout, components |
| `<body>` HTML | 436–598 | Page markup — banner, form, result panel |
| `<script>` | 599–705 | JavaScript — validation, DOM manipulation, event listeners |

---

## ⚙️ Key JavaScript Concepts Used

- `document.getElementById()` — element selection
- `addEventListener('submit' / 'change' / 'input')` — event handling
- `classList.toggle()` / `classList.add()` — CSS class manipulation
- `element.textContent` — updating displayed text
- `document.createElement()` + `appendChild()` — dynamic DOM creation
- `requestAnimationFrame()` — smooth CSS transition triggering
- `querySelector()` — selecting checked radio button

---

## 🔍 How UI Updates Work (Vanilla JS)

```
User fills form → clicks Submit
        │
        ▼
submit event fires
        │
        ▼
JS reads values from DOM  (element.value)
        │
        ▼
JS validates fields        (classList.toggle 'has-error')
        │
        ▼
JS writes values to DOM    (element.textContent = ...)
        │
        ▼
JS shows result panel      (style.display = 'block')
        │
        ▼
requestAnimationFrame      (fade-in animation)
```

> There is **no shared state object**. The DOM itself is the store and the view.

---

## ⚡ Vanilla JS vs React.js — Key Differences

| Aspect | Vanilla JS (this file) | React.js |
|---|---|---|
| **UI update** | Manual DOM writes | Automatic re-render via `useState` |
| **Live preview** | ❌ Only after submit | ✅ Updates as you type |
| **Code style** | Imperative | Declarative |
| **State** | Scattered in DOM | Centralised `useState` hooks |
| **Reusability** | None (one-off HTML) | Components reused everywhere |
| **Setup** | Zero — open HTML in browser | `npm install` + `npm start` |

---

## 👨‍💻 Author

**Sohom Chakraborty** · MCA · Christ University Bangalore  
GitHub: [@sohom09](https://github.com/sohom09)

---

*Lab 5 · Full Stack Development · Christ University Bangalore*
