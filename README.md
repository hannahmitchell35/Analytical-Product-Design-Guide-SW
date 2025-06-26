
## 🔄 Summary of Key Differences Between `index.html` and `launch -> launch.html`

This table compares the two main HTML pages used in the Analytical Product Design Guide website.

| Feature                      | `index.html` (Homepage)                             | `launch.html` (Launch Page)                          |
|------------------------------|------------------------------------------------------|------------------------------------------------------|
| **Main Role**                | Homepage for docs/navigation                         | One-off intro/announcement page                      |
| **Navigation Tabs**          | ✅ Yes — links to all key sections                   | ❌ Not typically included                            |
| **Hero Section**             | ✅ Yes                                              | ✅ Yes                                               |
| **Feature Cards/Links**      | ✅ Yes — links to sections like “Naming Conventions” | ❌ No (or very few)                                  |
| **Video Embed**              | ❌ No                                                | ✅ Yes — launch event                                |
| **Expandable Content**       | ✅ Structured for growth                             | ❌ Meant to stay static                              |
| **Tied to MkDocs Sidebar**   | ✅ Yes                                              | ❌ Not usually connected                             |
| **Used Routinely**           | ✅ Entry point for most users                        | ❌ Typically viewed once or on first visit           |

---

### ✅ When to Use Each

- Use `index.html` as the **main homepage** for navigation and exploration
- Use `launch -> launch.html` as a **celebratory or promotional landing page**, possibly linked from a button like:
  ```html
  <a href="launch" class="md-button">View our launch</a>
  ```

As you create additional standalone pages, add them to this comparison table to keep track of their roles.
