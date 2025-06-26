
# ❌ 404.html – Page Not Found Handler

This HTML file acts as the **“Page Not Found”** screen for the site. It's triggered when someone tries to visit a page that doesn't exist.

It is part of the MkDocs Material theme and includes the full site layout (header, nav, footer) — but shows only a **404 message** in the main content area.

---

## ✅ What This Page Does

| Feature                    | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| Full `<head>` section      | Loads fonts, stylesheets, and theme metadata like other pages               |
| Navigation header          | Maintains consistent top-bar with NHS branding and GitHub link              |
| Tabs + Sidebar             | Present but functional links lead back to valid parts of the site           |
| Main content               | Displays just a header: `404 - Not found`                                   |
| Footer                     | Same as other pages, with links to GitHub, contact, licence info            |
| Search bar + Scripts       | Still available — user can search for a valid page                          |

---

## ✍️ How to Customize the 404 Page

You can change the content by replacing this block:

```html
<div class="md-content" data-md-component="content">
  <article class="md-content__inner md-typeset">
    <h1>404 - Not found</h1>
  </article>
</div>
```

…with something more user-friendly, like:

```html
<h1>Oops! Page not found.</h1>
<p>Try using the search bar or return to the <a href="/">homepage</a>.</p>
```

---

## 📝 Purpose

This file is important for good UX:
- Helps users recover from broken or outdated links
- Keeps them inside the branded NHS documentation site
- Prevents confusion from blank/error browser screens

---

## 📁 File Location

This file is usually saved as:
```
404.html
```
MkDocs will automatically use this when needed, as long as it’s present at the root or properly routed via your hosting platform (e.g. GitHub Pages).

---
