
# 🌐 GH-Launch Page Overview (HTML Explained)

This file represents a custom launch page for the **Analytical Product Design Guide - South West**, built with **MkDocs + Material for MkDocs**.

It includes:
- NHS branding
- A hero introduction
- Feature section cards
- Navigation menus
- Footer with GitHub/project info

---

## ✅ What This Page Does

| Section                    | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| `<head>`                   | Sets fonts, icons, styles, metadata, and theme configuration                |
| Header / Nav Bar           | Contains logo, title, GitHub link, and search button                       |
| Navigation Tabs            | Top tabs like "Dashboard lifecycle" or "Core Components"                   |
| Hero Section               | A banner with headline and CTA buttons                                     |
| Feature Cards (`.top-hr`)  | Clickable content blocks linking to key pages                              |
| Footer                     | Contact links, GitHub repo, copyright, etc.                                |
| Scripts                    | Adds functionality: drawer toggle, lightbox, tab memory, and search        |

---

## ➕ How to Add a New Section

You might want to add a section like **“User Research”** to the homepage and nav bar. Here’s how:

### 1️⃣ Add a Navigation Tab

Find this section:

```html
<ul class="md-tabs__list">
  ...
</ul>
```

Add a new item inside it:

```html
<li class="md-tabs__item">
  <a href="user_research/" class="md-tabs__link">User Research</a>
</li>
```

---

### 2️⃣ Add a Feature Tile (Homepage Box)

Locate this:

```html
<div class="top-hr">
  ...
</div>
```

Add this block:

```html
<a href="user_research/" class="feature-item">
  <h2>User Research</h2>
  <p>Learn how user testing improves dashboard outcomes and usability.</p>
</a>
```

---

### 3️⃣ Create a New Page

If using MkDocs:

- Create a new folder and Markdown file:
  ```bash
  mkdir docs/user_research
  touch docs/user_research/index.md
  ```

- Add content to `docs/user_research/index.md`:
  ```markdown
  # User Research
  Explore the value of engaging users early in the dashboard lifecycle...
  ```

---

### 4️⃣ Update `mkdocs.yml`

Update the `nav:` list:

```yaml
nav:
  - Home: index.md
  - User Research: user_research/index.md
  - Dashboard Design: dashboard_design/index.md
```

---

## ✅ Summary Table

| What                    | Where in HTML              | What to Add                                                   |
|-------------------------|----------------------------|----------------------------------------------------------------|
| Nav tab (top menu)      | `<ul class="md-tabs__list">` | `<li><a href="folder/">Label</a></li>`                         |
| Feature tile            | `<div class="top-hr">`       | `<a href="folder/" class="feature-item">...</a>`              |
| New content page        | `docs/folder/index.md`       | Markdown with your content                                    |
| MkDocs config           | `mkdocs.yml`                | Add a `- Label: folder/index.md` entry under `nav:`          |

---

## 📝 Tips

- Keep folder names lowercase and hyphenated (e.g. `user-research`)
- Check your local site build (`mkdocs serve`) to preview changes
- Use consistent heading levels and styling for readability

