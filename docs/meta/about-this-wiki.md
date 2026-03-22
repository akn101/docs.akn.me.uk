---
sidebar_position: 1
title: About aknWiki
---

# About aknWiki — docs.akn.me.uk

**URL:** [https://docs.akn.me.uk](https://docs.akn.me.uk)
**Type:** Documentation site
**Powered by:** Docusaurus 3.4.0
**Stack:** Next.js (via Docusaurus), TypeScript, React

---

## Overview

**aknWiki** is the central documentation hub for the akn ecosystem. It provides detailed, structured documentation for every service, project, and tool built and maintained by Ahnaf Kabir.

The wiki is built on **Docusaurus** — a static site generator optimised for documentation — and is deployed at `docs.akn.me.uk`.

---

## Purpose

- Serve as a single source of truth for all akn services
- Provide onboarding guides, feature references, and technical details for each project
- Be accessible to collaborators, users, and the public

---

## Structure

The wiki is organised into four top-level sections:

| Section | Contents |
|---------|---------|
| **Core** | Main portfolio site (akn.me.uk), Status page, Startpage |
| **Projects** | Agora, AuraCare, The Pathway Initiative, Applis |
| **Playground** | Waves, EC Timetable Viewer, Nalu |
| **Meta** | Information about the wiki itself |

---

## Authentication

The wiki itself is publicly readable. Some linked services within it require authentication via **aknClient**.

The footer note on the wiki reads:

> "akn © Access via aknClient"

This refers to aknClient — the authentication layer used across private akn services.

---

## Running the Wiki Locally

### Requirements
- Node.js 18.0 or above
- Yarn

### Commands

```bash
# Install dependencies
yarn

# Start development server (hot reload)
yarn start

# Build for production
yarn build

# Preview production build
yarn serve

# Type-check TypeScript
yarn typecheck
```

The development server runs at `http://localhost:3000` by default.

---

## Technical Details

| Property | Value |
|----------|-------|
| Generator | Docusaurus 3.4.0 |
| Preset | `@docusaurus/preset-classic` |
| Language | TypeScript |
| Node requirement | ≥ 18.0 |
| Syntax highlighting | Prism (GitHub theme / Dracula dark) |
| i18n | English (en) |
| Base URL | `/` |
| Production URL | `https://docs.akn.me.uk` |

---

## Configuration

The Docusaurus config lives at `docusaurus.config.ts` in the repository root.

Key settings:

```ts
title: 'aknWiki'
url: 'https://docs.akn.me.uk'
baseUrl: '/'
onBrokenLinks: 'throw'
onBrokenMarkdownLinks: 'warn'
```

Broken internal links will cause the build to **throw an error** — all internal doc links must be valid for the site to build successfully.
