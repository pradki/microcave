# microcave

**Offline-ready MicroPython IoT system for ESP32 — modular, extensible, and easy to use.**

`microcave` is a collection of lightweight MicroPython modules and tools designed to run on ESP32-based devices such as ESP32-S3, Sonoff Mini R4, and others. It's built for **offline-first** operation — using local Wi-Fi (without internet), ideal for environments with solar power, rural setups, or privacy-sensitive applications.

## ✨ Features

- 🔌 Wi-Fi manager with fallback AP and auto-reconnect
- 📦 Modular structure with reusable shared components
- 🔁 Async TCP communication (Modbus client/gateway, relay control, etc.)
- 🌐 Built-in HTTP server with WebSocket support
- 📁 Embedded FTP server for code updates
- 🔄 JSON-based configuration system
- 🎛️ Touchscreen GUI support (ILI9488 + XPT2046)
- 📡 UDP discovery mechanism
- 🧠 Watchdog & system monitoring

## 📦 Project Structure

