# 🧭 Overview: What the `index.html` Code Does

This HTML file builds the homepage of the **NHS Analytical Product Design Guide – South West** using the [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) theme.

It acts as a launchpad for:
- Style guidance for dashboard/report design (e.g. in Tableau)
- Standardized templates and naming conventions
- Clear navigation to best practices and resources

---

## ✅ What This Page Includes

| **Section**               | **Purpose**                                                                 |
|---------------------------|------------------------------------------------------------------------------|
| **Header**                | Shows NHS logo, site title, GitHub repo link, and search button             |
| **Navigation Tabs**       | Top-bar links to each section (e.g., Dashboard Design, Lifecycle, etc.)     |
| **Hero Section**          | A prominent welcome banner with title, blurb, and call-to-action buttons    |
| **Feature Cards**         | Clickable tiles linking to key content areas like templates and rules       |
| **Footer**                | Includes contact, licensing info, and project links                         |
| **Responsive Scripts**    | Enables mobile sidebar, search, lightbox viewer, and markdown styling       |

---

## 🔧 Technologies Used

- **HTML5**: The markup structure
- **CSS (via MkDocs/Material)**: For layout and design
- **JavaScript**: Lightbox, search, and dynamic functionality
- **MkDocs**: Static site generator used to produce this page
- **Google Fonts & NHS Styling**: For visual consistency

---


## ➕ How to Add a New Section to the Homepage

This guide explains how to add a **new content area** to the homepage and navigation of the Analytical Product Design Guide site.

For example, you might want to add a new section like **“Accessibility Guidelines”**.

---

### 🧩 What This Will Add:

- A new **tab** in the top navigation
- A new **feature tile** on the homepage
- A new **linked page** with your content

---

### 1️⃣ Add a New Tab to the Navigation Bar

**Open your `index.html`** and find this section:

```html
<ul class="md-tabs__list">
  <!-- existing nav items here -->
</ul>
```

**Add your new tab inside this list**:

```html
<li class="md-tabs__item">
  <a href="accessibility/" class="md-tabs__link">Accessibility</a>
</li>
```

This creates a new tab in the top menu bar called "Accessibility".

---

### 2️⃣ Add a New Feature Tile (Homepage Box)

**Still in `index.html`**, scroll down to the `<div class="top-hr">` section. This controls the homepage feature tiles.

Add this new block inside it:

```html
<a href="accessibility/" class="feature-item">
  <h2>Accessibility Guidelines</h2>
  <p>Ensure your dashboard is usable by all users, including those with disabilities.</p>
</a>
```

This will appear as a new card underneath the hero banner.

---

### 3️⃣ Create the Content Page

If you're using MkDocs:

- Create a new file at:  
  `docs/accessibility/index.md`

- Add your content using Markdown:
  ```markdown
  # Accessibility Guidelines

  This guide explains how to make dashboards inclusive and usable for everyone...
  ```

---

### 4️⃣ Update `mkdocs.yml`

Finally, open your `mkdocs.yml` file and add your new page to the navigation:

```yaml
nav:
  - Home: index.md
  - Accessibility: accessibility/index.md
  - Dashboard Design: dashboard_design/index.md
  ...
```

This makes sure the page shows up in the site's sidebar and structure.

---

### ✅ Summary

| **What You're Adding**     | **Where to Edit**                | **What to Add**                                      |
|----------------------------|----------------------------------|------------------------------------------------------|
| Navigation tab (top menu)  | `<ul class="md-tabs__list">`     | `<li><a href="folder/">Name</a></li>`                |
| Feature tile (home card)   | `<div class="top-hr">`           | `<a href="folder/" class="feature-item">...</a>`     |
| New content page           | `docs/folder/index.md`           | Write your Markdown content                          |
| MkDocs sidebar nav         | `mkdocs.yml`                     | Add `- Name: folder/index.md`                        |

---

📌 That's it! Once you've made these updates, your new section will appear on the homepage, in the top navigation bar, and load your custom content.


