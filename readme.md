# Sheryians Coding School – Notes Repository

---

## ✨ Overview

Welcome to the **Sheryians Coding School** notes collection – a beautifully styled, **single‑page** web portal that showcases a curated set of DevOps, cloud, and JavaScript tutorials.  All notes are written in clean HTML with a sleek, dark‑mode friendly design, powered by a reusable **shared navbar** component.

---

## 🎨 Design Highlights

- **Modern color palette** – dark background with vibrant accent colors defined via CSS custom properties.
- **Responsive layout** – the sidebar (`nav`) collapses on screens < 768 px, while the main content scales gracefully.
- **Smooth interactions** – hover effects, active link highlighting, and a scroll‑aware navbar that hides when you scroll down and reappears when you scroll up.
- **Dynamic nav‑highlight** – the script automatically adds the `.active` class to the current page link.

---

## 📂 Folder Structure

```
Sheryians-Notes/
├─ index.html                # Landing page with a grid of note cards
├─ readme.md                 # This file (you are reading it)
├─ notes/                    # Individual note pages
│   ├─ CICD.html
│   ├─ codespace.html
│   ├─ ejs.html
│   ├─ eks.html
│   ├─ jest-testing.html
│   ├─ jwt-auth.html
│   ├─ kuber.html
│   ├─ kubernetes.html
│   ├─ MCP.html
│   ├─ mutliagent.html
│   ├─ rate-limiting.html
│   ├─ redis.html
│   ├─ sandbox.html
│   ├─ skaffold.html
│   └─ shared-navbar.html   # Reusable navigation component
└─ assets/ (optional)       # Place images, icons, etc.
```

---

## 🚀 Getting Started

1. **Open the portal** – simply double‑click `index.html` in a browser, or serve the directory with any static file server (e.g., `npx -y serve .`).
2. **Navigate** – use the left‑hand navbar (or the cards on the homepage) to jump between notes.
3. **Add a new note**
   - Create a new HTML file inside `notes/`.
   - Add a corresponding entry to `shared-navbar.html` using the same pattern:
     ```html
     <a href="/notes/your-note.html" data-page="your-note">Your Note Title</a>
     ```
   - Add a card to `index.html` if you want it displayed on the home grid.

---

## 🛠️ Development & Deployment

- **Local development** – no build step required; edit the HTML/CSS directly.
## 🚀 Deployment

This project is a static site and can be hosted on any static‑hosting platform. Below are quick steps to publish it with **GitHub Pages**:

1. **Create a repository** on GitHub (e.g., `mannatgupta146/Notes`).
2. **Push** this code to the `main` (or `gh-pages`) branch.
3. In the repository **Settings → Pages**, set the source to the `main` branch and the folder to `/ (root)`.
4. GitHub will generate a URL like https://mannatgupta146.github.io/Sheryians-Notes/. Access any note via https://mannatgupta146.github.io/Sheryians-Notes/notes/CICD.html.
5. For other hosts (Netlify, Vercel, Render) simply drag‑and‑drop the repository or connect the GitHub repo; the site will be served automatically.

> **Note:** Ensure the `shared-navbar.html` path uses `../shared-navbar.html` (already configured) so navigation works from the `notes/` subdirectory.
---

## 📚 Adding Content

When adding new topics:
1. **Write the note** – keep the same `<style>` block and `<script>` block as the other notes for consistency.
2. **Update the navbar** – as shown above.
3. **Update the home grid** – copy one of the existing `<a class="card" href="./notes/your-note.html">…</a>` blocks in `index.html` and adjust the title/icon.

---

## 📖 About This Repository

This repository is part of **Sheryians Coding School – Cohort 2.0**. All notes are created thanks to the guidance of **Ankur Bvhaaoya**. If you’d like to add more notes, feel free to contribute – you’re welcome! Finally, consider ⭐️ starring this repo to show your support.

---
*Thank you for exploring! Contributions are welcome – feel free to open issues or submit pull requests. 🌟⭐️*
