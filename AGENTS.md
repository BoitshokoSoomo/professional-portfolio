# AGENTS.md - Windows 12 Portfolio

## Project
Personal portfolio website styled as a Windows 12 desktop environment. Each project opens as a draggable window. Built with vanilla HTML, CSS, JavaScript in a single file.

## Stack
- Single file: index.html (all CSS and JS inline)
- No external libraries or CDN links
- Fonts: Segoe UI (system), fallback to system-ui

## Design Language
- Background: dark navy (#080c14) with subtle grid pattern and radial gradient glows
- Windows: glassmorphism cards (rgba white, backdrop-filter blur)
- Accent: #4f8ef7 (blue), #7c5cfc (purple), #22c55e (green), #f59e0b (yellow)
- Taskbar: bottom, fixed, frosted glass
- Start button: bottom left
- Clock: bottom right, live (en-ZA locale)

## Rules
- Everything lives in one index.html file.
- Each project is a window object in the `W` array at the top of the script.
- To add a project: add one object to `W[]`. Do not add HTML manually.
- Window state (open, minimised, position, z-index) lives in the `S` object.
- Do not use any external libraries or CDN links.
- Do not add animations that run on every scroll or mouse move (performance).
- External links must have `rel="noopener noreferrer"`.

## Window Object Shape
```js
{
  id: "leaveflow",        // unique string ID
  icon: "📋",            // emoji icon
  title: "LeaveFlow",    // display title
  color: "#22c55e",      // accent color
  bg: "linear-gradient(135deg,#22c55e,#06b6d4)",  // icon gradient
  w: 530,                // default width
  h: 540,                // default height
  body: `                // raw HTML content (template literal)
    <div class="ws">...</div>
    <div class="wbr">
      <a class="wab ab" href="DEMO_URL" target="_blank">🚀 Live Demo</a>
      <a class="wab ag" href="GITHUB_URL" target="_blank">⎇ GitHub</a>
    </div>
  `
}
```

## Desktop Icons (current)
- About Me (auto-opens on load)
- Skills
- Certifications
- LeaveFlow — github.com/BoitshokoSoomo/leave-system
- SA Insight Dashboard — sa-dashboard.vercel.app
- Footprint Logger — footprint-logger.vercel.app
- Book Review API — github.com/BoitshokoSoomo/expressBookReviews
- Hospital System (PHMS)
- Finance App — finance-app-web-oteu.vercel.app

## Taskbar Items (always visible)
- Start button (opens all windows list)
- Open window buttons (dynamic)
- Clock (live time)
- GitHub link icon
- LinkedIn link icon

## What NOT to touch
- Do not change the single-file structure
- Do not add a backend
- Do not change the window drag/resize logic once it works

## Current Status
All 9 windows implemented. Finance App added as latest project.
