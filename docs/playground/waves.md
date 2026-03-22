---
sidebar_position: 1
title: Waves (Audio Visualiser)
---

# Waves — waves.playground.akn.me.uk

**URL:** [https://waves.playground.akn.me.uk](https://waves.playground.akn.me.uk)
**Type:** Playground — Creative / Audio Tool
**Also known as:** Resonance

---

## Overview

**Waves** (internally titled **Resonance**) is an interactive, browser-based **audio wave visualiser** that generates animated dot-grid patterns synchronised in real time to audio files.

It uses the **Web Audio API** to analyse audio frequency data frame-by-frame and modulates visual parameters (amplitude, frequency, speed, colour) in response to the music — producing a dynamic, reactive animation.

---

## Getting Started

1. Open [waves.playground.akn.me.uk](https://waves.playground.akn.me.uk)
2. Upload an audio file by **drag-and-drop** or using the file picker
3. Press **Play** to start playback and the visualisation simultaneously
4. Customise the wave pattern and parameters using the control panel

---

## Audio Input & Playback

### Supported Formats
- MP3
- WAV
- OGG

### Playback Controls

| Control | Function |
|---------|---------|
| **Play / Pause** | Start or pause audio and animation |
| **Stop** | Stop playback and reset position to start |
| **Progress bar** | Scrub to any point in the audio |

---

## Visualisation Modes

Nine distinct wave pattern types are available:

| Mode | Description |
|------|-------------|
| **Horizontal** | Wave flows left-to-right across the grid |
| **Vertical** | Wave flows top-to-bottom |
| **Diagonal** | Wave flows diagonally across the canvas |
| **Radial** | Wave emanates outward from a central point |
| **Spiral** | Wave follows a spiral path from the centre |
| **Ripple** | Circular ripples from a single fixed source |
| **Random Ripples** | Multiple simultaneous ripple sources at random positions |
| **Sine** | Classic sine wave with configurable direction |

---

## Customisation Controls

The collapsible control panel is divided into organised sections:

### Grid Settings

| Parameter | Description |
|-----------|-------------|
| **Grid Size** | Density of the dot grid — more dots = finer grain |
| **Dot Radius** | Base size of each dot |
| **Scale Effect** | How much dot size modulates with the wave |
| **Spacing** | Distance between dots |

### Wave Parameters

| Parameter | Description |
|-----------|-------------|
| **Amplitude** | Height/intensity of the wave |
| **Frequency** | Number of wave cycles across the canvas |
| **Speed** | Animation speed of the wave |
| **Direction** | Angle of wave travel (0–360°) |
| **Position Displacement** | Offset of the wave origin |

### Radial / Ripple Specific

| Parameter | Description |
|-----------|-------------|
| **Center X / Center Y** | Position of the radial origin on the canvas |
| **Ripple Source Count** | Number of simultaneous ripple origins (Random Ripples mode) |

### Audio Reactivity

| Parameter | Description |
|-----------|-------------|
| **Modulate** | Choose what the audio drives: Amplitude, Frequency, or Speed |
| **Sensitivity** | How strongly the audio signal affects the chosen parameter |
| **Smoothing** | How quickly the visualiser responds to sudden changes in audio |
| **Frequency Band** | Select which part of the audio spectrum drives the effect — **Bass** or **Treble** |

---

## Colour Behaviour

The visualiser dynamically shifts dot colour in response to audio intensity:

- At rest / low intensity: **Blue tones**
- At high intensity / loud peaks: **Purple tones**

This provides a natural visual cue for the energy in the audio at any given moment.

---

## Export Options

Three export formats are available:

| Format | Description |
|--------|-------------|
| **PNG** | Static snapshot of the current canvas frame |
| **GIF** | 3-second animated GIF export |
| **WebM** | 3-second video recording in WebM format |

Exports capture the visualisation exactly as it appears on screen, including current settings and audio state.

---

## UI Layout

| Region | Content |
|--------|---------|
| **Header** | Title ("Resonance"), minimal branding |
| **Main canvas** | Full-screen dot-grid visualisation |
| **Control panel** | Collapsible sidebar with all parameters |
| **Footer** | Attribution |

---

## Technical Notes

- Built using the browser's native **Web Audio API** — no external audio library required
- Real-time frequency analysis runs every animation frame
- The canvas is rendered using HTML5 `<canvas>` with requestAnimationFrame for smooth 60fps animation
- No server-side processing — fully client-side

---

## Access

Waves is **publicly accessible** with no authentication required. It runs entirely in the browser and does not upload audio files to any server.
