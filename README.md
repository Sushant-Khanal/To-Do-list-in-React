# ✅ Todo List App

A clean, professional React todo list app with an animated gradient background, glassmorphism UI, and smooth animations.

---

## 🚀 Features

- **Add tasks** — type a task and hit Add
- **Complete tasks** — check the checkbox to mark a task done (strikethrough + fade effect)
- **Delete tasks** — remove any task with the Delete button
- **Persistent storage** — todos are saved to `localStorage` so they survive page refreshes
- **Empty state** — a friendly dotted container with a floating icon when no tasks exist
- **Animated background** — a moving deep-space gradient that shifts continuously
- **Glassmorphism cards** — frosted-glass form and todo items with backdrop blur
- **Smooth animations** — slide-in items, check pop, hover transitions, and more

---

## 🗂 Project Structure

```
src/
├── App.jsx            # Root component — state management (add, toggle, delete)
├── NewTodoForm.jsx    # Controlled input form for adding new todos
├── TodoList.jsx       # Renders the list or empty state
├── TodoItem.jsx       # Individual todo row (checkbox, label, delete button)
└── styles.css         # All styling — animations, layout, glassmorphism
```

---

## 🛠 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v16 or higher
- npm or yarn

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/todo-list-app.git
cd todo-list-app

# 2. Install dependencies
npm install

# 3. Start the development server
npm run dev
```

The app will be available at `http://localhost:5173` (Vite) or `http://localhost:3000` (Create React App).

---

## 📦 Built With

- [React](https://react.dev/) — UI library
- [Vite](https://vitejs.dev/) — build tool and dev server
- CSS3 — animations, glassmorphism, custom properties

---

## 🎨 Design Highlights

| Element | Style |
|---|---|
| Background | 8-stop gradient, `400% 400%` size, 16s shift animation |
| Form & cards | `rgba` fill + `backdrop-filter: blur(22px)` glassmorphism |
| Checkbox | Custom styled, gradient fill on check, pop animation |
| Empty state | Dashed purple border, floating icon, centered text |
| Todo item | Slides in from left, shifts right on hover |
| Delete button | Subtle red tint, glows red on hover |

---

## 📝 Usage

1. Type a task name into the **New Item** input field
2. Click **Add** (or press Enter) to add it to the list
3. Click the **checkbox** to mark a task as complete
4. Click **Delete** to permanently remove a task

---

## 🔧 Customization

**Change the gradient colors** — edit the `background` property in the `body` rule in `styles.css`:
```css
body {
  background: linear-gradient(
    135deg,
    #0d0d1a, #1a1040, #0f3460, ...
  );
}
```

**Change animation speed** — edit the `gradientShift` duration:
```css
animation: gradientShift 16s ease infinite; /* increase for slower */
```

**Change the max width** — update the `max-width` on `#root`, `.new-item-form`, `.list`, and `.empty-state` (all set to `480px` by default).

---

## 📄 Author

Sushant Khanal
---
 free to use and modify.