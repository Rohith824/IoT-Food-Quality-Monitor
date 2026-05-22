# 🥗 IoT Food Quality Monitor

**IoT-Driven Smart Mess Tracking & Evaluation System**

## 📖 Overview

The **IoT Food Quality Monitor** is a reliable, automated dashboard designed to help mess administrators and students monitor food safety in real-time. By combining IoT sensor data and AI-driven image analysis, this system aims to reduce health risks caused by spoiled or substandard food.

## ✨ Features

* **Real-Time Sensor Tracking:** Monitor temperature, humidity, gas levels, and color values via dynamic live charts.
* **AI Image Analysis:** Integrates a MobileNetV2 Convolutional Neural Network (CNN) to detect fungus/mold in food using your device's built-in camera or an external USB webcam.
* **Data Simulation:** Test the system without physical hardware by simulating "Normal," "Spoiled," and "Warning" conditions.
* **History & Feedback:** Log historical sensor data and collect user feedback on daily meal quality.
* **Responsive UI:** A futuristic, dark-themed dashboard built for seamless monitoring across all devices.

## ⚙️ System Components & Sensors

* ☁️ **MQ-135 Aroma Sensor:** Air quality and spoilage detection. *(0–25% → FRESH, 26–55% → WARNING, 56–100% → SPOILED)*
* 🔥 **MQ-3 Smoke/Gas Sensor:** Smoke and overcooking detection. *(0–20% → NORMAL, 21–50% → WARNING, 51–100% → OVERCOOKED)*
* 🎨 **TCS3200 Color Sensor:** Visual food condition analysis. Identifies RGB shifts (e.g., green shift = mold, dark brown = overcooked).
* 🌡️ **DHT11 Sensor:** Temperature and humidity tracking for optimal food preservation.
* 🧠 **AI Image Analysis (CNN):** A MobileNetV2 model trained on 2,400 images across 5 epochs, achieving 93.8% accuracy for freshness classification.

## 🚀 Live Demo

You can view and interact with the live simulation of the dashboard here:

**[IoT Food Quality Monitor Live Site](https://rohith824.github.io/IoT-Food-Quality-Monitor/)**

## 🛠️ Technologies Used

* **Frontend:** HTML5, CSS3, Vanilla JavaScript
* **Data Visualization:** [Chart.js](https://www.chartjs.org/)
* **AI/ML:** MobileNetV2 architecture for image processing
* **Hardware Target:** ESP32 Microcontroller

## 📝 How to Use the Dashboard

1. **Select Food Item:** Use the top dropdown menu to select the meal being monitored (e.g., Rice, Bread, Chicken, Lunch Box).
2. **View Charts:** Navigate to the **Charts** tab to see real-time graphical trends for temperature, gases, humidity, and RGB values.
3. **Run Image AI:** Go to the **Image AI** tab, click refresh to detect cameras, allow browser permissions, and click **Capture & Analyze** to inspect food for mold or spoilage.
4. **Simulate Data:** If physical sensors are not connected, use the **Simulate** tab to trigger dummy data and test the UI's reaction to different food conditions.
