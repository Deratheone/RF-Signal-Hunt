# RF Signal Hunt

![RF Signal Hunt Banner](https://via.placeholder.com/800x200/0d1117/3b82f6?text=RF+Signal+Hunt)

A campus-wide RF treasure hunt game for educational events, developed by IEEE APS CUSAT Student Branch.

## 🎯 Overview

RF Signal Hunt turns RF signal theory into an interactive game where participants build receivers that track hidden 433MHz transmitters around campus. The project demonstrates practical applications of antenna design, signal propagation, and embedded systems.

## 🛠️ Hardware Requirements

### Receiver
- ESP32 DevKit module
- 433MHz RF receiver module
- Battery for portable operation

### Transmitter
- Arduino Uno board
- 433MHz RF transmitter module
- Battery for portable operation

## 🚀 Features

- **Interactive Radar Interface** - Real-time visualization of RF signals
- **Multi-Transmitter Tracking** - Track up to 6 transmitters simultaneously
- **Signal Strength Indication** - Visual representation of signal strength
- **Distance Estimation** - Approximate distance to transmitters
- **Score System** - Points awarded for discovering transmitters
- **Persistent Storage** - Game progress saved between power cycles
- **Mobile-Friendly UI** - Responsive design works on any smartphone

## 📋 Workshop Structure

This project is designed as a two-phase educational event:

1. **Phase 1: Workshop** - Participants build and understand RF receivers
2. **Phase 2: Signal Hunt** - Campus-wide competition to find hidden transmitters

## 📚 Documentation

- [Hardware Setup](docs/HARDWARE.md) - Detailed hardware assembly instructions
- [Setup Guide](docs/SETUP_GUIDE.md) - Software setup and configuration
- [Workshop Guide](docs/WORKSHOP.md) - How to run the workshop event

## 📱 Web Interface

![RF Signal Hunt Interface](https://via.placeholder.com/300x500/0d1117/3b82f6?text=Radar+Interface)

The web interface features:
- Interactive radar display
- Signal strength indicators
- Score tracking
- Transmitter discovery list
- Battery monitoring

## 📡 Technology Stack

- ESP32 (Receiver)
- Arduino (Transmitter)
- RCSwitch library for 433MHz communication
- ESP32 WebServer for hosting the interface
- HTML/CSS/JS for the radar UI
- EEPROM for persistent storage

## 🔄 How It Works

1. Transmitters broadcast unique IDs via 433MHz signals
2. Receivers detect signals and estimate distance based on signal strength
3. Web interface visualizes signals on a radar display
4. Participants navigate campus to find hidden transmitters
5. Points are awarded when a transmitter is found (within 5m range)

## 🔧 Installation

1. Clone this repository
2. Open `transmitter/rf_signal_transmitter.ino` in Arduino IDE
3. Set unique `TRANSMITTER_ID` for each transmitter
4. Upload to Arduino Uno devices
5. Open `receiver/rf_signal_hunt_receiver.ino` in Arduino IDE
6. Upload to ESP32 devices
7. Connect to ESP32 WiFi AP (SSID: RF-SIGNAL-HUNT)
8. Navigate to http://192.168.4.1 in a web browser

## 📄 License

Released under the MIT License. See [LICENSE](LICENSE) for details.

## ✨ Credits

Developed by IEEE Antennas and Propagation Society (APS) CUSAT Student Branch.

---

Last Updated: June 26, 2025
