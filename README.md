
## 🔄 Summary of Key Differences Between `index.html`, `launch.html`, and `404.html`

This table compares the three main HTML page types used in the Analytical Product Design Guide website.

| Feature                      | `index.html` (Homepage)                             | `launch.html` (Launch Page)                          | `404.html` (Error Page)                                 |
|------------------------------|------------------------------------------------------|------------------------------------------------------|---------------------------------------------------------|
| **Main Role**                | Homepage for docs/navigation                         | One-off intro/announcement page                      | Shown when user visits a missing or broken link         |
| **Navigation Tabs**          | ✅ Yes — links to all key sections                   | ❌ Not typically included                            | ✅ Yes — consistent layout                              |
| **Hero Section**             | ✅ Yes                                              | ✅ Yes                                               | ❌ No                                                    |
| **Feature Cards/Links**      | ✅ Yes — homepage menu                              | ❌ No (just launch content)                          | ❌ No                                                    |
| **Video Embed**              | ❌ No                                                | ✅ Yes — launch video                                | ❌ No                                                    |
| **Expandable Content**       | ✅ Structured for growth                             | ❌ Meant to stay static                              | ❌ Static 404 message only                               |
| **Tied to MkDocs Sidebar**   | ✅ Yes                                              | ❌ Not usually connected                             | ✅ Yes — same nav as other pages                         |
| **Used Routinely**           | ✅ Entry point for most users                        | ❌ Typically viewed once                             | ⚠️ Only shown on error or broken link                    |

---

### ✅ When to Use Each

- **Use `index.html`** as the homepage of your documentation.
- **Use `launch.html`** to introduce or promote your guide/project.
- **Use `404.html`** as a fallback when users land on a missing or incorrect page.

