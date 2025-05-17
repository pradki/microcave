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

```
microcave/
├── main.py # Async main loop
├── config.py # Config loader/saver
├── config.json # JSON-based device configuration
├── lib/
│ └── microcave/
│ ├── wifimanager/
│ ├── ftp/
│ ├── tcpclient/
│ ├── httpserver/
│ ├── modbus/
│ ├── switch/
│ ├── core_cwu/
│ └── shared/ # common utilities (e.g. rgbled, monotime)
```


## 📷 Example Use Cases

- 🛁 Domestic hot water control (CWU)
- 🔄 Modbus RTU to TCP bridge
- 🧲 Relay control (e.g. Sonoff Mini R4)
- 🪟 Smart window blind automation
- 💧 Irrigation controller
- 📈 Touch display interface

## 🧪 Getting Started

1. Clone the repo and upload files to your ESP32 using [mpremote](https://docs.micropython.org/en/latest/reference/mpremote.html) or FTP.
2. Adjust `config.json` with your Wi-Fi credentials and device name.
3. Boot the ESP32 — it will either connect to Wi-Fi or open its own config AP.
4. Access the device via browser (default IP: `192.168.4.1`) to configure it via web interface.

## 🧰 Requirements

- ESP32 / ESP32-S3 with MicroPython firmware
- Basic MicroPython knowledge
- Local Wi-Fi network (no internet required)

## 📖 Documentation

Full docs, wiring guides, and examples coming soon.

## 📜 License

MIT License. Some shared components (e.g. FTP server) originate from external MIT-licensed projects — credit is preserved in source headers.

## 🙌 Contributions

Suggestions, issues, and pull requests are welcome. This project aims to help both makers and pros build robust, offline-first ESP32-based devices with MicroPython.

---

Stay tuned for examples, hardware connection diagrams, and installation scripts.

