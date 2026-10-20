# 👥 Employee Management System

A browser-based CRUD application for managing employee records, built with vanilla JavaScript using a clean **MVC (Model-View-Controller)** architecture.

## 🚀 Live Demo

**[👉 Try it live](https://mhummadhamza321-commits.github.io/employee-management-system/)**

## ✨ Features

- ➕ Add new employees (name, email, role, salary)
- ✏️ Edit existing records
- 🗑️ Delete employees with confirmation
- 💾 Automatic persistence via `localStorage` — no backend required
- 📱 Responsive layout
- 🏗️ Separation of concerns: Model / View / Controller

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Structure | HTML5 |
| Styling | CSS3 (Flexbox, Grid, Glassmorphism) |
| Logic | Vanilla JavaScript (ES6) |
| Persistence | Browser `localStorage` API |

## 📐 Architecture


### Responsibilities

| Layer | File / Module | Responsibility |
|-------|--------------|----------------|
| **Model** | `EmployeeModel` (IIFE) | Owns the data array. Handles `add`, `update`, `remove`, `getAll`, `getById`, `init`, `count`. Persists to `localStorage` on every mutation. |
| **View** | `EmployeeView` (IIFE) | Caches DOM nodes. Renders table rows via template literals. Manages "Add" vs "Edit" form mode. Provides `render()`, `resetForm()`, `fillForm()`, `getFormData()`. |
| **Controller** | `EmployeeController` (IIFE) | Wires events to actions. Tracks `editingId` state. Validates input. Calls Model methods, then instructs the View to re-render. |

### Why MVC here?

- **Testability** — The Model can be unit-tested in isolation.
- **Scalability** — Swap `localStorage` for a REST API by rewriting only the Model.
- **Clarity** — A future developer reads one file and immediately sees what each section does.
- **Interview-ready** — Demonstrates architectural thinking, not just "it works."

---

## 📸 Screenshots

> **⚠️ ACTION REQUIRED:** Add your own screenshots below. Recruiters ignore READMEs without visuals.

### Main View
![Main interface showing form and employee table](./screenshots/main-view.png)

### Add Employee
![Adding a new employee record](./screenshots/add-employee.png)

### Edit Mode
![Editing an existing employee record](./screenshots/edit-mode.png)

### Mobile Responsive
![Mobile view of the application](./screenshots/mobile-view.png)

**How to add screenshots:**
1. Run the app locally (open `index.html`)
2. Take screenshots (`Win+Shift+S` on Windows, `Cmd+Shift+4` on Mac)
3. Create a `screenshots/` folder in your repo
4. Drag-and-drop images into a new file `screenshots/main-view.png` on GitHub (or commit via VS Code)
5. Update the paths above to match your filenames

---

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- **[Optional]** [VS Code](https://code.visualstudio.com) with the [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) for auto-reload
- **[Optional]** [Git](https://git-scm.com/downloads) if you want to clone the repo

### Installation

**Option 1 — Just open the file (fastest):**

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/employee-management-system.git

# 2. Navigate into it
cd employee-management-system

# 3. Open index.html in your browser
#    Windows:  start index.html
#    macOS:    open index.html
#    Linux:    xdg-open index.html
