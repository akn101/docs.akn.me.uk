---
sidebar_position: 3
title: Nalu (Coral Disease Modeller)
---

# Nalu — nalu.playground.akn.org.uk

**URL:** [https://nalu.playground.akn.org.uk](https://nalu.playground.akn.org.uk)
**Type:** Playground — Environmental / Scientific Tool
**Stack:** Next.js

---

## Overview

**Nalu** is a web-based **predictive disease modelling platform for coral reefs**. It enables marine scientists, reef conservation professionals, and researchers to model and predict the spread of coral diseases by inputting environmental and biological variables.

The tagline summarises its purpose:

> "Predicted coral disease growth, handled."

Nalu takes in location data, environmental readings, and biological metrics, then runs a predictive analysis to forecast how coral disease may spread — helping researchers and conservationists plan interventions before disease takes hold.

---

## Use Cases

- **Marine biology research** — model disease spread under different environmental conditions
- **Reef conservation planning** — identify at-risk areas before disease proliferates
- **Climate impact studies** — simulate how rising sea temperatures or changing salinity affect disease risk
- **Academic analysis** — compare model outputs using different predictive methodologies

---

## Inputs & Data Variables

### File Upload
- Users can upload existing datasets directly into the tool

### Location
- A **geographic location selector** allows users to specify and edit the reef location being modelled
- Location data is used to contextualise environmental parameters

### Date
- A **date field** sets the reference date for the model (e.g. `09/03/2025`)

### Environmental Variables

Users can select and input the following environmental metrics (via checkboxes for customisable inclusion):

| Variable | Description |
|----------|-------------|
| **Temperature** | Sea surface or water column temperature |
| **Salinity** | Salt concentration of the water |
| **Water Turbidity** | Clarity of the water (affects photosynthesis and stress) |
| **Water Current** | Speed and direction of water movement |
| **Sedimentation** | Level of sediment deposition on the reef |

### Biological Variables

| Variable | Description |
|----------|-------------|
| **Coral Disease Species** | The specific coral disease pathogen or disease type being modelled |
| **Drupella Density** | Population density of Drupella (corallivorous snails that stress coral) |
| **Parrotfish Density** | Density of parrotfish (which graze algae and influence reef health) |
| **Butterflyfish Density** | Density of butterflyfish (indicators of reef health) |
| **Total Coral Cover** | Percentage of the reef area covered by coral |
| **Coral Density** | Number of coral colonies per unit area |

---

## Controls

| Control | Description |
|---------|-------------|
| **Variable checkboxes** | Select which variables to include in the model run |
| **Use New Model** | Toggle to select between modelling methodologies |
| **Generate** | Run the predictive analysis with the current inputs |

---

## Output

After clicking **Generate**, Nalu produces a prediction of coral disease spread based on the provided inputs. Outputs typically include:

- Predicted disease growth rate or spread area
- Risk assessment for the defined location and time period
- Visualisation or tabular summary of the model results

---

## Technical Details

| Property | Value |
|----------|-------|
| Framework | Next.js (React) |
| Data input | Manual form entry + file upload |
| Modelling | Predictive algorithm (selectable model versions) |
| Visualisation | Rendered in-browser |

---

## Access

Nalu is **publicly accessible** at the URL above. No authentication is required. It is hosted under `playground.akn.org.uk`, indicating it is an experimental or research-phase tool maintained on a best-effort basis.

---

## Notes

- Nalu is a **playground project** — it is in active development and functionality may change
- The tool is intended for **scientific and educational use**
- Model accuracy depends on the quality and completeness of input data provided
