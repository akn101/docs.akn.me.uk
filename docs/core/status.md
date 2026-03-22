---
sidebar_position: 2
title: Status Page
---

# Status — status.akn.me.uk

**URL:** [https://status.akn.me.uk](https://status.akn.me.uk)
**Type:** Infrastructure monitoring
**Powered by:** Checkmate (self-hosted)

---

## Overview

`status.akn.me.uk` is the **live uptime and incident monitoring dashboard** for all services within the akn ecosystem. It provides a real-time view of service health and a historical record of past incidents.

The status page is powered by **Checkmate**, a self-hosted monitoring platform. The AKN logo is displayed prominently at the top of the page.

---

## Page Structure

### Incidents Panel

The page is divided into two incident sections:

| Section | Description |
|---------|-------------|
| **Active Incidents** | Any currently ongoing service disruptions or degraded performance |
| **Past Incidents** | Historical record of all resolved incidents |

When no incidents are occurring, both sections display **"None recorded"**.

### Service Reports

Each monitored service is displayed as a report card containing:

| Field | Description |
|-------|-------------|
| **Title** | The name of the monitored service |
| **Status** | Current operational status (Up / Down / Degraded) |
| **URL** | The endpoint being monitored |
| **Uptime** | Rolling 30-day uptime percentage visualisation |

The service list is loaded dynamically via JavaScript (`genAllReports()`) when the page finishes loading.

---

## How It Works

On page load, two JavaScript functions run automatically:

1. **`genAllReports()`** — Fetches the current status of all monitored services and renders their report cards.
2. **`genIncidentReport()`** — Fetches and renders any active or past incidents.

This means the page requires JavaScript to be enabled for full functionality. While the page is loading, a `"Loading status information..."` message is displayed.

---

## Interpreting the Status Page

### Status Colours

Typically status monitoring pages use the following colour conventions (consistent with Checkmate's design):

| Colour | Meaning |
|--------|---------|
| Green | Operational — service is up and responding normally |
| Yellow / Orange | Degraded — service is up but performance is reduced |
| Red | Down — service is not responding |

### Uptime Bar

The 30-day uptime bar shows a day-by-day breakdown of availability. Each segment represents one day; colour indicates whether the service was up, degraded, or down that day. The overall uptime percentage is shown as a number (e.g. `99.9%`).

---

## Incident Reporting

Incidents are tracked with:

- **Title** — a short description of the issue
- **Status** — open or resolved
- **Affected services** — which monitors were impacted
- **Timeline** — when the incident started and ended

---

## Access

The status page is **publicly accessible** without authentication, so anyone can check the health of akn services at any time.
