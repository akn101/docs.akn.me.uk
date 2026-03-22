---
sidebar_position: 2
title: EC Timetable Viewer
---

# EC Timetable Viewer — tt.ec.playground.akn.me.uk

**URL:** [https://tt.ec.playground.akn.me.uk](https://tt.ec.playground.akn.me.uk)
**Docs:** [tt.ec.playground.akn.me.uk/docs](https://tt.ec.playground.akn.me.uk/docs/)
**Type:** Playground — School Productivity Tool
**Audience:** Eton College students

---

## Overview

The **EC Timetable Viewer** is a web application that transforms an **Eton College student timetable** (saved as an HTML file) into a clean, interactive weekly view — with the bonus of exporting the timetable to a calendar (`.ics` / iCal format) for use in Google Calendar, Apple Calendar, Outlook, and similar apps.

---

## How It Works

The tool works in two steps:
1. The student saves their timetable as an HTML file from the Eton student portal
2. The student uploads the file to the tool, which parses and renders it

---

## Step 1: Getting Your Timetable File

### Laptop (Windows / macOS) — Recommended

1. Visit the Eton student timetable portal and sign in with your **Microsoft school account**
2. Wait for your full timetable to load in the browser
3. Save the page as an HTML file using your browser's save function:

| Browser | Save shortcut | Format to select |
|---------|--------------|-----------------|
| Chrome | `Ctrl+S` / `Cmd+S` | "Webpage, HTML only" |
| Edge | `Ctrl+S` / `Cmd+S` | "Webpage, HTML only" |
| Firefox | `Ctrl+S` / `Cmd+S` | "Webpage, HTML only" |
| Safari | `Cmd+S` | Select **"Page Source"** format |

> **Important:** Always choose **"HTML only"** or **"Page Source"** — do NOT save as "Web Archive" or "Complete Webpage", as these formats are not supported.

### iOS / iPadOS

Using a laptop is **strongly recommended** for iOS users. iOS browsers typically save pages as Web Archives (`.webarchive`) rather than plain HTML files, which this tool **cannot process**.

If you must use iOS:
- Try a third-party browser that supports HTML-only saving
- Otherwise, save the file on a laptop and transfer it to your device

### Android

Similarly, using a laptop is recommended. Chrome on Android's "Download page" feature typically saves as **MHTML** (`.mhtml`), which this tool **does not support**.

---

## Step 2: Using the Tool

Once you have the HTML file:

1. Open [tt.ec.playground.akn.me.uk](https://tt.ec.playground.akn.me.uk) — you will be redirected to the docs/upload page
2. Upload your saved HTML file
3. The tool parses the file and displays your timetable

---

## Features

### Weekly Timetable View
- Displays your schedule **organised by day** in a clear weekly layout
- Colour-coded by subject or lesson type
- Shows lesson time, subject, teacher, and room

### Timetable Statistics
After loading your timetable, the tool displays:

| Statistic | Description |
|-----------|-------------|
| **Allocated lessons** | Total number of timetabled lessons |
| **Free periods** | Number of free periods in the week |
| **Subject count** | Number of distinct subjects |
| **Teacher count** | Number of distinct teachers |

### Teacher Name Mapping
- Teacher names are mapped from abbreviated codes (as they appear in the raw timetable) to full readable names where known

### Room Information
- Room and location data is extracted and displayed alongside each lesson

### Early Work (EW) Indicators
- Lessons designated as **Early Work (EW)** are highlighted with a visual indicator

### School Letter Assignment
- The tool detects and displays the current **school letter** (the Eton week-letter system, e.g. A, B, C...)

---

## Calendar Export

The calendar export feature is one of the most useful aspects of the tool.

### Export Format
- Exports as a standard **ICS (iCalendar)** file, compatible with all major calendar applications

### Export Options

| Option | Description |
|--------|-------------|
| **Select specific weeks** | Choose individual weeks to include in the export |
| **Date range** | Specify a start and end date |

### Importing the ICS File

Once exported:
- **Google Calendar:** Settings → Import & Export → Import
- **Apple Calendar:** File → Import
- **Outlook:** File → Open & Export → Import/Export → Import an iCalendar file

---

## Platform Compatibility

| Platform | Supported | Notes |
|----------|-----------|-------|
| Windows (Chrome/Edge/Firefox) | ✅ Yes | Full support |
| macOS (Chrome/Edge/Firefox) | ✅ Yes | Full support |
| macOS (Safari) | ✅ Yes | Use "Page Source" when saving |
| iOS / iPadOS | ⚠️ Limited | Web Archive format not supported; use laptop |
| Android | ⚠️ Limited | MHTML format not supported; use laptop |

---

## Access

The EC Timetable Viewer is **publicly accessible** at the URL above. No login is required. The tool processes files locally in the browser — timetable files are not uploaded to any server.

---

## Notes

- This is a **playground project** — it is maintained on a best-effort basis
- The tool is specifically designed for **Eton College** timetable HTML exports; other school timetable formats are not supported
