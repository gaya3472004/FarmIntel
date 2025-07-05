# 🌾 FarmIntel – Smart Farming with Edge AI on ESP32S3

**FarmIntel** is an Edge AI-powered IoT solution built on the **XIAO ESP32S3** microcontroller to perform real-time classification of fruits and bugs. It uses a **custom-trained ML model** built with **Edge Impulse**, running completely offline — ideal for remote or resource-constrained environments.

---

## 🔍 Project Overview

This project aims to assist farmers by enabling real-time detection of:
- 🐛 **Pests** damaging crops
- 🍎 **Fruits** ready for harvest

The model runs entirely on the ESP32S3, eliminating the need for cloud connectivity, making it suitable for **on-field, low-power** smart agriculture use.

---

## 🧠 ML Model

- Trained on the **Edge Impulse** platform
- Dataset: Images of fruits and insects
- Model type: Image classification
- Accuracy: ~85% in real-world conditions
- Exported as **Arduino-compatible C++ library**
- Deployed to **XIAO ESP32S3**

---

## 🔧 Tools & Technologies

- **XIAO ESP32S3** (Edge AI-capable microcontroller)
- **Edge Impulse** (Model training & dataset handling)
- **Arduino IDE** (with Edge Impulse Arduino library)
- **Camera Module** (connected to ESP32S3)
- **C/C++** for firmware
- **Serial Monitor or OLED Display** for predictions

---

## 📦 Setup & Deployment

1. **Train & Export Model from Edge Impulse**
   - Train with datasets or images .
   - Export as Arduino library (ZIP)

2. **Integrate Library in Arduino IDE**
   - Include `.zip` in Arduino
   - Add `#include <edge-impulse-project-name>` in code

3. **Connect camera to ESP32S3**
   - Use pins compatible with XIAO ESP32S3

4. **Upload the firmware**
   ```bash
   Select board: XIAO ESP32S3
   Select Port : COM8 (USB we connect to system. )
   Upload via Arduino IDE
