# LUMEX — Smart Nanoleaf Audio-Reactive Lighting System

Custom modular hex lighting system powered by ESP32 with real-time audio reactivity, capacitive touch interaction, and fully custom firmware architecture.

---

## 📌 Overview

**Role:** Embedded Engineer  
**Core Technologies:** ESP32, WS2812B, FastLED, Capacitive Touch, 3D Printing

LUMEX is a fully modular, open-source smart lighting system designed as a customizable alternative to commercial Nanoleaf-style panels. The system integrates real-time audio processing, touch interaction, and fluid animation rendering within an optimized embedded firmware architecture.

---

## ❗ Problem

Commercial smart lighting systems are:

- Expensive
- Closed-source
- Limited in customization
- Restricted in advanced effect control

There is a lack of affordable, modular, open-source lighting systems with advanced firmware flexibility and performance.

---

## 💡 Solution

Designed and engineered custom 3D-printed hex panels powered by an ESP32 core featuring:

- Audio-reactive visualization modes
- Capacitive touch interaction
- Modular interconnect system
- Expandable panel architecture
- Custom firmware built for performance and stability

---

## 🛠️ Technical Approach

### Firmware Architecture

- Developed a **state-machine based firmware system**
- Managed concurrent tasks:
  - Lighting animations
  - Touch interrupts
  - Audio sampling
  - Mode transitions
- Optimized memory and timing for stable long-term operation

### Audio Processing

- Implemented real-time audio sampling
- Performed FFT processing directly on ESP32
- Mapped frequency bands to lighting patterns
- Achieved smooth audio visualization

### LED Control

- WS2812B addressable LEDs
- FastLED library integration
- Optimized frame timing
- Power-stability handling

### Mechanical Design

- Custom 3D-printed hex enclosures
- Modular snap-fit connectors
- Expandable physical layout

---

## 🚀 Key Features

- Modular hex lighting panels
- Real-time audio-reactive visualization
- Capacitive touch mode switching
- Ripple, ambient, rotate & brightness modes
- Smooth transitions between lighting states
- Custom PCB-style interconnect system
- OTA-ready firmware architecture (expandable)

---

## 📊 Performance Achievements

- Achieved **60 FPS fluid animation** across multiple panels
- Stable multi-panel synchronization
- Low-latency audio-to-light response
- Efficient state-based firmware execution

---

## 🏗️ System Architecture

```
[Audio Input (MAX4466 Mic)]
        ↓
ESP32 ADC Sampling
        ↓
FFT Processing
        ↓
State Machine Controller
        ↓
FastLED Rendering Engine
        ↓
WS2812B LED Panels
```

Touch input interrupts integrate directly into the firmware state manager for seamless user interaction.

---

## 📂 Suggested Folder Structure

```
lumex-nanoleaf-system/
│
├── firmware/
│   ├── main.cpp
│   ├── state_machine.cpp
│   ├── audio_processing.cpp
│   ├── touch_controller.cpp
│   ├── led_renderer.cpp
│   └── config.h
│
├── hardware/
│   ├── wiring_diagram.png
│   ├── panel_design.stl
│   └── component_list.md
│
├── docs/
│   ├── architecture.png
│   └── setup_guide.md
│
└── README.md
```

---

## 🔮 Future Improvements

- Wireless panel synchronization
- Web-based control dashboard
- Mobile app integration
- Custom PCB development
- Advanced DSP optimizations
- Scene memory presets

---

## 🎯 Applications

- Smart home lighting
- Interactive art installations
- Gaming room ambient lighting
- Audio visualization systems
- Modular decorative lighting systems

---

## 👤 Author

**Jishnu Mahanta**  
Embedded & IoT Engineer  
Building intelligent systems & calm UX.

---

## 📜 License

MIT License 
