# 🌾 FarmIntel – Edge AI Smart Farming using ESP32S3 and Edge Impulse

**FarmIntel** is a real-time fruit and insect detection system developed using the **XIAO ESP32S3** microcontroller with camera support. The project uses a **custom-trained machine learning model** built on **Edge Impulse** and runs it directly on the microcontroller using the **Arduino IDE**.

This project demonstrates how low-power embedded devices can use **Edge AI** for smart agriculture — even without internet access.

---

## 🧠 What I Did

- Collected a dataset of fruits and bugs
- Used the **Edge Impulse platform** to train an **image classification model**
- Exported the model as a **ZIP Arduino Library** from Edge Impulse
- Configured my **ESP32S3** device on Edge Impulse (including device ID and connection)
- Imported the Arduino library into Arduino IDE and wrote code to classify camera input
- Connected a compatible camera module to the ESP32S3
- Displayed classification results via **Serial Monitor**

---

## 🔧 Tools & Components Used

- **XIAO ESP32S3** microcontroller (with onboard camera support)
- **Edge Impulse** (for training the ML model)
- **Arduino IDE** (for programming the ESP32S3)
- **Custom camera module** (OV2640 or similar)
- Serial monitor for output (or OLED display optionally)

---

## ⚙️ How It Works

1. **Train the model**
   - Collected images of bugs and fruits
   - Labeled them using Edge Impulse's data labeling tools
   - Trained the model using their vision/image classification pipeline
   - Follow the example Object detection model documenation attached here to create and train a model.

2. **Download model as Arduino library**
   - Exported as `.zip` file directly from Edge Impulse

3. **Program the ESP32S3**
   - Imported the ZIP library into Arduino IDE
   - Wrote a sketch to initialize the camera, capture frames, and run the model
   - Viewed classification results in the Serial Monitor

4. **Edge device performs prediction**
   - No internet required
   - Works offline directly on the ESP32S3 board

---

## ✅ Output Example

On the serial monitor:
![Screenshot 2025-06-15 223833](https://github.com/user-attachments/assets/f77c2497-dd6d-479d-9a76-161f308fc99f)
![Screenshot 2025-06-15 214743](https://github.com/user-attachments/assets/b6bbaeb3-d826-48ff-97c0-2379795ad0b0)

