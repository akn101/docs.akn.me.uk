---
sidebar_position: 4
title: Applis (Applicant Manager)
---

# Applis — applis.helper.etonstem.akn.org.uk

**URL:** [https://applis.helper.etonstem.akn.org.uk](https://applis.helper.etonstem.akn.org.uk)
**Type:** Recruitment / Applicant Tracking System
**Stack:** Next.js
**Context:** Eton STEM — helper tooling

---

## Overview

**Applis** is a web-based **applicant management and recruitment tracking dashboard** designed to streamline the process of reviewing, filtering, and managing job or programme applicants.

It sits within the `helper.etonstem.akn.org.uk` subdomain structure, suggesting it is a supporting tool built for **Eton STEM** — likely used internally by staff to manage applications to STEM programmes, positions, or initiatives.

---

## Core Features

### Applicant Dashboard
- Centralised view of **all submitted applicants**
- Each applicant record contains relevant submission details
- Supports viewing individual applicant profiles

### CSV Upload — Batch Import
- Staff can **upload applicant data in bulk** via a CSV file
- Removes the need to manually enter each applicant — useful when applications are collected via Google Forms, Typeform, or other external tools
- The upload button is clearly labelled **"Upload Applications CSV"**

### Export

Applicant data can be exported in two formats:

| Format | Use case |
|--------|---------|
| **CSV** | For further processing in spreadsheet software (Excel, Google Sheets) |
| **PDF** | For sharing formatted reports with stakeholders or printing |

### Filtering & Search

The dashboard supports filtering applicants by:

| Filter | Description |
|--------|-------------|
| **All Blocks** | Filter by cohort block or group assignment |
| **All Positions** | Filter by the specific role or programme they applied for |

A **search field** allows staff to quickly locate a specific candidate by name or other identifier.

### Empty State

When no applicants match the current filters, the dashboard displays:

> "No applicants found matching your filters."

This confirms the filter logic is working correctly rather than indicating a system error.

---

## Typical Workflow

1. **Collect applications** via an external form (Google Forms, Typeform, etc.)
2. **Export** submissions as a CSV file from the form tool
3. **Upload the CSV** to Applis via the "Upload Applications CSV" button
4. **Review** applicants in the dashboard — filter by block or position
5. **Export** shortlists or full lists as CSV or PDF as needed

---

## Technical Details

| Property | Value |
|----------|-------|
| Framework | Next.js (React) |
| Data input | CSV file upload |
| Data export | CSV and PDF |
| Authentication | Internal / staff access assumed |

---

## Access

Applis is intended for **internal staff use**. While the URL is not publicly advertised, it is accessible at the subdomain above. It is expected that access is restricted to authorised Eton STEM staff or administrators.
