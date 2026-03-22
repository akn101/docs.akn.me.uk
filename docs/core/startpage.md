---
sidebar_position: 3
title: Startpage
---

# Startpage — startpage.akn.me.uk

**URL:** [https://startpage.akn.me.uk](https://startpage.akn.me.uk)
**Type:** Personal browser startpage / productivity dashboard
**Stack:** Next.js, JetBrains Mono

---

## Overview

`startpage.akn.me.uk` is a personal **browser startpage** — a custom homepage designed to be set as a browser's new-tab or home URL for fast access to tools, links, and quick utilities.

It is built as a Progressive Web App (PWA), meaning it can be installed on desktop or mobile devices and run in a full-screen app-like experience.

---

## Features

### Command Palette

The primary navigation mechanism is a **command palette**, activated with:

```
⌘K  (macOS)
Ctrl+K  (Windows / Linux)
```

The palette provides fast keyboard-driven access to all features and links. Typing a query instantly filters available commands.

### Quick Commands

The following slash commands are available from the command palette:

| Command | Description |
|---------|-------------|
| `/record` | Triggers a screen/audio recording utility |
| `/alarm` | Sets an alarm or timer |
| `/dim` | Adjusts screen brightness or activates a dim overlay |
| `/camera` | Activates the device camera |

### Theme

- Supports a **dark theme** by default (`theme-color: #06060f` — near-black)
- Designed for minimal eye strain during long browser sessions

### Typography

- Uses **JetBrains Mono** as the primary font — a monospace typeface designed for readability in developer-oriented UIs

---

## PWA Capabilities

The startpage is configured as a **Progressive Web App**, which means:

- Can be installed on desktop via the browser's "Install app" prompt
- Appears as a standalone app (no browser chrome) when installed
- Supports Apple Touch Icon for iOS home screen installation
- Includes a Web App Manifest for consistent app metadata
- `user-scalable` is disabled for an native app-like feel on mobile

---

## Technical Details

| Property | Value |
|----------|-------|
| Framework | Next.js (React) |
| Font | JetBrains Mono |
| Theme colour | `#06060f` |
| PWA | Yes (manifest + apple-touch-icon) |
| Mobile optimised | Yes (viewport meta, user-scalable disabled) |

---

## Usage

1. Navigate to [startpage.akn.me.uk](https://startpage.akn.me.uk)
2. Set it as your browser's homepage or new-tab URL
3. Optionally install it as a PWA for a full-screen experience
4. Use `⌘K` / `Ctrl+K` to open the command palette and navigate quickly

---

## Access

The startpage is **publicly accessible** but is intended as a personal tool. No authentication is required to visit the URL.
