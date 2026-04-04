# mxvoice.app website

The marketing site and documentation for [Mx. Voice](https://mxvoice.app/), built with [Astro](https://astro.build/).

## Development

**Requirements:** Node.js 24+ (use [mise](https://mise.jdx.dev/) — a `mise.toml` is included).

```bash
# Install dependencies
npm install

# Start dev server (http://localhost:4321)
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Project Structure

```
src/
├── assets/img/          # Images (optimized by Astro)
├── components/          # Astro components (Navbar, Footer, DocsSidebar)
├── layouts/             # Page layouts (Base, Docs)
├── pages/
│   ├── index.astro      # Landing page
│   └── docs/            # Documentation (Markdown)
├── styles/
│   └── global.css       # All styles
public/
├── CNAME                # Custom domain
├── favicon.png
└── fonts/               # Nexa font files
```

## Adding Documentation

Create a new `.md` file in `src/pages/docs/`:

```markdown
---
title: Page Title
subtitle: A short description
layout: ../../layouts/Docs.astro
---

Your content in Markdown...
```

Then add a link in `src/components/DocsSidebar.astro`.

## Deployment

Pushes to `main` automatically build and deploy to GitHub Pages via the workflow in `.github/workflows/github-pages.yml`.

The site is live at https://mxvoice.app/
