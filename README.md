<div align="center">

# 3D Warehouse QR Generator

**An interactive WebGL digital twin transforming autonomous intralogistics infrastructure into functional, high-contrast QR codes.**

[![Live Demo](https://img.shields.io/badge/Live_Demo-qr.vorky.fyi-FF5500?style=for-the-badge&logo=googlechrome&logoColor=white)](https://qr.vorky.fyi/)
[![Three.js](https://img.shields.io/badge/Three.js-r128-black?style=for-the-badge&logo=three.js&logoColor=white)](https://threejs.org/)
[![GSAP](https://img.shields.io/badge/GSAP-3.12-88CE02?style=for-the-badge&logo=greensock&logoColor=white)](https://greensock.com/gsap/)
[![Architecture](https://img.shields.io/badge/Architecture-Zero--Build_Single_File-blue?style=for-the-badge)](index.html)

[**Explore Live Demo →**](https://qr.vorky.fyi/)

</div>

---

## Overview

The **3D Warehouse QR Generator** bridges industrial automation engineering with creative web visualization. It dynamically constructs a procedural intralogistics fulfillment center—complete with multi-tier high-bay racking, autonomous mobile robots (AMRs), counterbalanced forklifts, and roller conveyors—and seamlessly flattens the environment into an optical, scannable QR code via real-time camera projection interpolation.

Built as a zero-dependency, self-contained single-file application powered by **Three.js**, **GSAP**, and the native **Web Audio API**.

---

## Key Features

### Dual-State Morphing Engine
* **Isometric 3D Facility:** Freeform 3D inspection view with soft shadow mapping, cruising automated guided vehicles (AGVs), animated AMRs, and real-time LiDAR plane sweeps.
* **Orthographic Scan Matrix:** Instant transition into a flat, high-contrast QR code optimized for smartphone camera recognition using **Error Correction Level H (30% redundancy)**.

### Asset-Reflected Regional Color Mapping
Instead of traditional monochrome rendering, modules in the scan matrix directly reflect the physical assets of the warehouse:
* **Corner Finder Patterns:** Mapped to structural racking uprights.
* **Center Data Grid:** Mapped to cross-beams, totes, and material-handling units.
* **Base Modules:** Mapped to facility floor slabs with verified luminance contrast ratios to guarantee instant scanning.

### Operational Shift Scenarios

| Shift Mode | Architectural Palette | Environmental Lighting | Atmospheric Particles |
| :--- | :--- | :--- | :--- |
| ☀️ **Day Shift** | Industrial Orange, Cobalt Racking, Amber Totes | Warm Sunlight (`2.4` intensity) | Luminous Golden Dust |
| ❄️ **Cold Storage** | Sub-zero Cyan, Glacial Azure, Cool Totes | Crisp Polar Luminescence (`2.2` intensity) | Ice-Blue Suspended Crystals |
| 🌙 **Night Shift** | Deep Obsidian Slate, Emerald AMRs, Safety Amber | Low-light Moonlight (`2.8` intensity) | Ambient Mint Fluorescents |

### VisionOS-Inspired Liquid Glass Interface
* **Glassmorphism:** Multi-layered blurred backdrops with dynamic specular edge highlights.
* **3D Tilt Hover Physics:** Real-time pointer perspective warping on desktop navigation cards.
* **Procedural Synthesis:** Synthesized mechanical servo hums, confirmation chimes, and arpeggiated C-major ambient chord progressions generated via the native Web Audio API.
* **Adaptive Mobile Layout:** Fully responsive touch interface with stacked typography and centered viewports.

---

## Technical Stack

* **Rendering Engine:** [Three.js](https://threejs.org/) (r128) utilizing `THREE.InstancedMesh` (rendering up to 55,000 blocks at 60 FPS) and PCF Soft Shadow Mapping.
* **Animation & Interpolation:** [GSAP 3.12](https://greensock.com/gsap/) handling non-linear camera frustum adjustments, FOV transformations, and material color lerping.
* **Matrix Logic:** [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) with custom coordinate parsers isolating finder patterns from data payloads.
* **Audio Synthesis:** Native browser `AudioContext` running real-time oscillator waveforms and exponential gain automation.
* **UI Architecture:** Pure CSS3 flexbox/grid, CSS custom properties, and variable font typography ([Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) & [Inter](https://fonts.google.com/specimen/Inter)).

---

## Local Development

Because this project uses a self-contained, zero-build architecture, no package managers (`npm`, `yarn`) or bundlers (`Vite`, `Webpack`) are required.

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/voruki/industrial-qr.git](https://github.com/voruki/industrial-qr.git)
   cd industrial-qr
