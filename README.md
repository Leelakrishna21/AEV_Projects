# 🌡️ LM35 Temperature Sensor Interfacing with Microcontroller (ADC + Serial Plot)

This project demonstrates how to interface the **LM35 analog temperature sensor** with a microcontroller (e.g., Arduino, ESP32, or STM32) using the **ADC (Analog-to-Digital Converter)** and visualize the **real-time temperature data** using a **serial plotter**.

---

## 🚀 Features

- Reads analog temperature data from LM35 sensor
- Converts ADC value to temperature in °C
- Sends temperature data over serial port
- Plots real-time temperature on Serial Plotter

---

## 🧰 Hardware Required

- LM35 Temperature Sensor  
- Microcontroller Board (Arduino UNO / ESP32 / STM32)  
- Jumper Wires  
- Breadboard (optional)  
- USB Cable (for programming and serial communication)  

---

## 🔌 Circuit Diagram

| LM35 Pin | Connection           |
|----------|----------------------|
| VCC      | 5V (or 3.3V for ESP) |
| OUT      | ADC input (e.g., A0) |
| GND      | GND                  |

---

## 📦 Files Included

| File Name           | Description                            |
|---------------------|----------------------------------------|
| `LM35_Arduino.ino`  | Arduino code for LM35 interfacing      |
| `LM35_ESP32.ino`    | ESP32-compatible version (3.3V logic)  |
| `README.md`         | Project overview and instructions      |

---

## 🧪 How to Use

### ✅ For Arduino

1. Open `LM35_Arduino.ino` in the Arduino IDE.
2. Connect the LM35 to A0, 5V, and GND.
3. Select your board and COM port.
4. Upload the code.
5. Open **Serial Plotter** (Baud: 9600) from Tools → Serial Plotter.

### ✅ For ESP32

1. Open `LM35_ESP32.ino` in Arduino IDE.
2. Connect LM35 to any ADC-capable pin (e.g., GPIO34), 3.3V, and GND.
3. Set board to **ESP32 Dev Module**.
4. Upload and open **Serial Plotter** (Baud: 115200).

---

## 📏 Temperature Conversion Formula

- **LM35 Output**: 10 mV per °C
- **Arduino (10-bit ADC, 5V)**: