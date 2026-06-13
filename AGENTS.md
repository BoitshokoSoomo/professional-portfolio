# AGENTS.md - Windows 12 Portfolio

## Project
Personal portfolio website styled as a Windows 12 desktop environment. Each project opens as a draggable window. Built with vanilla HTML, CSS, JavaScript or REACT in a single file.

## Stack
- Single file: index.html (all CSS and JS inline)
- Frameworks, build tools, dependencies if needed
- Fonts: Segoe UI (system), fallback to system-ui

## Design Language
- Background: dark navy (#0a0e1a) with subtle grid pattern
- Windows: glassmorphism cards (rgba white, backdrop-filter blur)
- Accent: #4f8ef7 (blue), #7c5cfc (purple)
- Taskbar: bottom, fixed, frosted glass
- Start button: bottom left
- Clock: bottom right, live

## Rules
- Everything lives in one index.html file. You can use separate CSS or JS or REACT files.
- Each project is a window object in the windows[] array at the top of the script.
- To add a project: add one object to windows[]. Do not add HTML manually.
- Window state (open, minimised, position, z-index) lives in the windowState object.
- Do not use any external libraries or CDN links.
- Do not add animations that run on every scroll or mouse move (performance).

## Window Object Shape
{
  id: "leaveflow",
  icon: "📋",
  title: "LeaveFlow",
  description: "Employee Leave Management System",
  stack: ["Node.js", "Express", "JavaScript", "SQL"],
  github: "https://github.com/BoitshokoSoomo/...",
  demo: "",
  details: "Full paragraph describing what it does and what problems it solves."
}

## Desktop Icons (current)
- LeaveFlow (Project 2)
- SA Data Dashboard (Project 4)
- Footprint Logger
- Express Book Review API
- Paradise Nursery
- PHMS Proposal (PDF link)

## Taskbar Items (always visible)
- Start button (opens skills/certs menu)
- Open window buttons (dynamic)
- Clock (live time)
- GitHub link icon
- LinkedIn link icon

## What NOT to touch
- Do not change the single-file structure
- Do not add a backend
- Do not change the window drag logic once it works

## Current Status
To be built after Project 4.