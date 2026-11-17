<div align="center">
  <h1>Fyers Desktop App</h1>
  <p>Ultra-Fast, Low-Latency Desktop Application for Fyers Trading Terminal</p>
</div>

---

## 📖 Overview

**Fyers Desktop** is a high-performance, standalone Windows application engineered for active Indian stock and options traders. It wraps the official Fyers Web platform into an isolated, GPU-accelerated environment that completely eliminates the freezing, lag, tab throttling, and memory overhead common in standard web browsers.

By leveraging hardware-accelerated rendering, dedicated process priority scheduling, and zero-throttling WebSocket pipelines, Fyers Desktop delivers the smoothest real-time charting and tick-by-tick execution experience.

---

## ✨ Core Performance Highlights

* ⚡ **Zero-Throttling Live Feeds**
  Unlike consumer browsers that throttle background tabs to save battery, Fyers Desktop completely disables background timer and renderer throttling. Your live WebSocket price feeds and order book ticks never drop or freeze.

* 🚀 **Direct GPU Hardware Rasterization**
  TradingView candlestick charts, indicator drawings, and canvas plots are rendered directly on your dedicated GPU at up to 120fps/144fps without consuming excess CPU cycles.

* 🧠 **4GB Dedicated V8 Heap**
  Allocated with 4GB V8 JavaScript heap memory to prevent garbage collection (GC) micro-pauses during heavy morning volatility (9:15 AM - 10:30 AM).

* 🛡️ **Windows High Process Priority**
  Automatically scheduled with High Priority on the Windows kernel to prevent background apps from starving your trading terminal of CPU cycles.

* ⌨️ **Trader Productivity Shortcuts**
  - **F11**: Fullscreen Mode (maximize screen real estate for multi-timeframe analysis)
  - **F5 / Ctrl + R**: Instant Refresh
  - **Ctrl + / Ctrl -**: Zoom in / Zoom out for 4K and ultra-wide monitor setups
  - **Ctrl + 0**: Reset Zoom to default

---

## 🚀 Getting Started

### Prerequisites
* Windows 10 or Windows 11 (64-bit)
* Minimum 4GB RAM (8GB+ recommended)

### Downloads & Installation

Choose between the portable executable or the full installer:

1. **Portable Version (`Fyers Desktop 1.0.0.exe`):**
   - No installation required.
   - Simply download, place in your preferred folder, and double-click to launch.

2. **Windows Installer (`Fyers Desktop Setup 1.0.0.exe`):**
   - Automatically installs the application and creates Desktop and Start Menu shortcuts.

---

## 🛠️ Technical Architecture

* **Runtime:** Electron v33 & Node.js v24
* **Graphics:** Angle / Direct3D11 GPU Rasterization (Zero-Copy)
* **Packaging:** NSIS Installer & Portable Binary via Electron-Builder
* **Network:** TCP Fast Open, Uncapped Connection Pooling

---

## 🔄 Updates & Versioning

Track `fyers-version.json` in this directory for active release parameters and version tracking.

---
*Developed and maintained with ❤️ by [HikerHarsh](https://github.com/HikerHarsh).*
