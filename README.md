# Boitshoko Soomo Portfolio

A personal portfolio website styled as a Windows desktop environment. Projects open as interactive windows, with a taskbar, start menu, live clock, and desktop icons.

## Overview

This portfolio presents SAP, full-stack development, data dashboard, and enterprise system projects in a memorable desktop-style interface.

## Tech Stack

- HTML
- CSS
- JavaScript
- No external libraries or CDN dependencies

## Project Structure

```text
.
├── AGENTS.md
├── README.md
└── index.html
```

All portfolio code lives in `index.html`.

## How To Run Locally

Open `index.html` directly in a browser, or run a simple local server:

```powershell
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Adding A Project

Projects are defined in the `W` array inside `index.html`.

Add a new object using this shape:

```js
{
  id: "project-id",
  icon: "📋",
  title: "Project Name",
  color: "#4f8ef7",
  bg: "linear-gradient(135deg,#4f8ef7,#7c5cfc)",
  w: 520,
  h: 540,
  body: `
    <div class="ws">
      <div class="wh1">Project Name</div>
      <p class="wp">Project description.</p>
    </div>
  `
}
```

Do not add project cards manually in the HTML body. Desktop icons, start menu entries, taskbar items, and windows are generated from the project data.

## Deployment

This is a static site, so it can be deployed with GitHub Pages or Vercel.

### GitHub Pages

1. Push the repo to GitHub.
2. Go to repository `Settings`.
3. Open `Pages`.
4. Choose `Deploy from a branch`.
5. Select the `main` branch and `/root`.
6. Save.

### Vercel

1. Import the GitHub repository into Vercel.
2. Use the default static site settings.
3. Deploy.

## Suggested Portfolio Links

- Static frontend projects: GitHub Pages or Vercel
- React/Vite projects: Vercel
- Express/API projects: Render, Railway, or another backend host
- PDF/document projects: GitHub Pages file link

## Author

Boitshoko Soomo

- GitHub: <https://github.com/BoitshokoSoomo>
- LinkedIn: <https://linkedin.com/in/boitshoko-soomo-13a0b7220>
