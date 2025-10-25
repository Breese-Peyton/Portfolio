## Status: v2 snapshot (desktop-first, no media queries)

This version is a clean rebuild focused on clarity and speed. It is desktop-first with a fluid layout, and it does not use media queries yet. Keyboard navigation is not complete. This snapshot records the current state before any responsive or a11y upgrades.

### What is live right now
- **Pages/Sections:** Hero, About, Skills (icons), Projects (3 placeholders), Contact, Footer
- **Typography:** Inter and Sora via Google Fonts
- **Assets:** Headshot and tech-stack SVGs under `/assets`
- **Favicon:** `/assets/favicon.ico`
- **Links:** Project CTAs are placeholders
- **Build/Hosting:** Static HTML + CSS on GitHub Pages with custom domain

### What is intentionally not done yet
- No media queries
- Limited keyboard navigation
- No sticky navigation or mobile menu
- Project links are placeholders

### File structure (current)
/
├─ index.html
├─ style.css
├─ assets/
│ ├─ favicon.ico
│ ├─ peyton-headshot-modified.png
│ └─ tech-stack/
│ ├─ CSS3.svg
│ ├─ Express.svg
│ ├─ Figma.svg
│ ├─ Git.svg
│ ├─ Github.svg
│ ├─ HTML5.svg
│ ├─ JavaScript.svg
│ ├─ Node.js.svg
│ ├─ OpenAPI.svg
│ ├─ PostgresSQL.svg
│ ├─ React.svg
│ ├─ Redux.svg
│ ├─ Swagger.svg
│ └─ VS-Code.svg
└─ README.md

### Known limitations
- Keyboard navigation is incomplete. Some interactive elements are anchors styled as buttons, others are plain buttons, and focus visibility is inconsistent.
- Layout is desktop-first. On narrow screens content may compress or wrap awkwardly.
- Hero image may not have explicit width and height attributes, which can cause layout shift on first load.

### Next planned upgrades (v2.1 or v3)
1. Add a centered container with max-width for consistent line length
2. Ensure images are fluid and never overflow
3. Add visible focus states and a skip-to-content link
4. Add anchor offset so section headings are not hidden when navigating
5. Convert project CTAs to consistent, accessible anchors or buttons
6. Later: add media queries for small screens and refine type scale

### Tech notes
- Fonts: Inter, Sora via Google Fonts (preconnect enabled)
- Meta: viewport tag present
- Hosting: GitHub Pages with custom domain `peytonbreese.com`
