<div align="center">

# 👥 Employee Management System

### A lightweight CRUD application for managing employee records — built with vanilla JavaScript using the **MVC** pattern and browser `localStorage` for persistence.

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-Visit_App-1e6f9f?style=for-the-badge)](https://YOUR_USERNAME.github.io/employee-management-system/)
[![GitHub Repo](https://img.shields.io/badge/📂_Source_Code-GitHub-181717?style=for-the-badge&logo=github)](https://github.com/YOUR_USERNAME/employee-management-system)
[![Made with JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

</div>

---

## 📖 Table of Contents

- [Overview](#-overview)
- [Live Demo](#-live-demo)
- [Features](#-features)
- [Tech Stack](#️-tech-stack)
- [Architecture](#️-architecture)
- [Screenshots](#-screenshots)
- [Getting Started](#-getting-started)
- [Usage Guide](#-usage-guide)
- [Project Structure](#-project-structure)
- [How It Works](#-how-it-works)
- [Roadmap](#-roadmap)
- [Testing](#-testing)
- [Contributing](#-contributing)
- [License](#-license)
- [Author](#-author)
- [Acknowledgments](#-acknowledgments)

---

## 🔍 Overview

The **Employee Management System** is a front-end-only web application that lets you create, view, update, and delete employee records without any backend server.

All data is stored in the browser using the `localStorage` API, so your records persist between page refreshes and browser sessions.

The application is deliberately built **without any frameworks or libraries** — pure HTML, CSS, and ES6 JavaScript — to demonstrate a clear understanding of the fundamentals, including a hand-rolled **MVC (Model-View-Controller)** architecture.

> **Why this project exists:** A portfolio piece showcasing clean architecture, DOM manipulation, event delegation, and persistent client-side storage — the three pillars every junior-to-mid front-end interview touches on.

---

## 🚀 Live Demo

**👉 [Try the live app here](https://YOUR_USERNAME.github.io/employee-management-system/)**

| Action | Try this |
|--------|----------|
| **Add** an employee | Fill the form → click "Add employee" |
| **Edit** a record | Click "✏️ Edit" on any row → modify → click "Update employee" |
| **Delete** a record | Click "🗑️ Delete" → confirm |
| **Test persistence** | Refresh the page (`F5`) — your data survives ✅ |

> ⏱️ *First load may take ~3 seconds if the GitHub Pages CDN is cold.*

---

## ✨ Features

- ➕ **Create** — Add employees with name, email, role, and salary
- 📋 **Read** — View all employees in a clean, sortable table
- ✏️ **Update** — Edit any existing record inline via the form
- 🗑️ **Delete** — Remove employees with a confirmation prompt
- 💾 **Persistent Storage** — Automatic `localStorage` sync after every change
- 🔍 **Form Validation** — Required fields, salary > 0, basic email format check
- 🎨 **Responsive Design** — Glassmorphism UI that adapts to mobile and desktop
- ⚡ **Zero Dependencies** — No React, no jQuery, no build tools. Just open the file.
- 🏗️ **MVC Architecture** — Model, View, and Controller cleanly separated
- ♿ **Keyboard-Friendly** — Tab-navigable form and buttons

---

## 🛠️ Tech Stack

| Layer | Technology | Purpose |
|-------|------------|---------|
| **Structure** | HTML5 | Semantic markup |
| **Styling** | CSS3 | Flexbox, Grid, custom properties, glassmorphism |
| **Logic** | JavaScript (ES6) | Modules, arrow functions, template literals, `const`/`let` |
| **Persistence** | `localStorage` API | Browser-based key-value storage |
| **Hosting** | GitHub Pages | Free static-site deployment |
| **Version Control** | Git + GitHub | Source management |

**No frameworks. No bundlers. No `npm install`. Zero dependencies.**

---

## 🏗️ Architecture

This project implements a **lightweight hand-written MVC pattern** to keep concerns separated:
