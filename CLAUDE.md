# CLAUDE.md — Project Guide for Claude Code

## Project Overview
This is the personal academic website for Dr. Irum Rauf, hosted on GitHub Pages at https://ircode.github.io/irumrauf/. It is a static HTML site built on the HTML5 UP "Spectral" template.

## Site Structure
```
irumrauf/
├── index.html              # Homepage with bio and photo
├── reserachInterests.html  # Research interests (note: filename has typo, keep as-is for URL stability)
├── teaching.html           # Teaching page
├── Professional.html       # Professional services
├── technicalskills.html    # Technical skills
├── publications.html       # Publications list
├── blog.html               # Blog listing page
├── blog/                   # Individual blog posts
│   └── YYYY-MM-DD-post-slug.html
├── images/                 # Site images
├── assets/
│   ├── css/main.css        # Main stylesheet (HTML5 UP Spectral)
│   ├── css/noscript.css
│   └── js/                 # jQuery + template scripts
└── CLAUDE.md               # This file
```

## Template & Styling
- Template: HTML5 UP "Spectral" (https://html5up.net)
- All pages share the same header, nav menu, footer, and script includes
- CSS lives in `assets/css/main.css` — do NOT modify this file unless explicitly asked
- Navigation menu is in a `<div id="menu">` inside the header on every page

## Blog Conventions
- Blog listing page: `blog.html`
- Individual posts go in `blog/` directory
- Post filename format: `YYYY-MM-DD-post-slug.html`
- Posts link back to `../blog.html` and use `../assets/` for CSS/JS paths
- Each new post needs a corresponding entry added to `blog.html`
- Blog post template: use the `<article id="main">` pattern with `<section class="wrapper style5">`
- Tags/categories go in the subtitle line under the post title

## Adding a New Blog Post
1. Create `blog/YYYY-MM-DD-title-slug.html` using an existing post as template
2. Add an entry to `blog.html` in the blog entries section (newest first)
3. Commit and push to deploy

## Important Notes
- This is a GitHub Pages site — changes deploy automatically on push to the default branch
- Keep all URLs relative (no absolute localhost paths)
- The nav menu must be updated on ALL pages when adding new menu items
- Keep the footer consistent across all pages
- British English spelling (e.g., "colour", "organisation", "behaviour")
- Content voice: professional but approachable academic tone
