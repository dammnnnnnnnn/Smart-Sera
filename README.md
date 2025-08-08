# 🌱 Smart Serra: Smart Farming IoT System

Smart Serra is an IoT-based smart agriculture system that automates irrigation and monitors environmental conditions in real-time. Designed for sustainability, this system helps reduce water waste and harmful emissions caused by traditional greenhouse practices — contributing to the fight against global warming.

---

## 📌 Features

- 🌡️ Monitors temperature and humidity
- 🌾 Detects soil moisture levels
- 💧 Monitors water availability
- 🚿 Automatically controls water pump
- 🔄 Servo motor control for valve or feeder
- 🌈 RGB LED indicators based on system state
- 📟 Real-time LCD status display
- ☁️ Integrated with Arduino IoT Cloud for remote monitoring and control
- 📲 Push notifications when water is low

---

## 🧠 How It Works

1. **Environment Monitoring**
   - The system continuously reads soil moisture, temperature, humidity, and water level.
2. **Smart Control**
   - If the soil is dry, it activates the pump automatically.
   - If water level is low, it sends a warning via the cloud.
3. **Servo Function**
   - Servo rotates based on cloud commands (0° or 180°).
4. **LED Status**
   - RGB LEDs reflect the system’s current status via color indication.
5. **LCD Display**
   - Shows temperature and humidity in real-time.

---

## ⚙️ Technologies Used

- **Platform**: ESP32
- **Programming**: Arduino C++
- **IoT Platform**: Arduino IoT Cloud
- **Data Display**: LCD 16x2
- **Control**: Cloud dashboard + automated logic

---

## ♻️ Environmental Impact

Smart Serra contributes to reducing greenhouse gas emissions by:
- Preventing overwatering, which reduces **nitrous oxide (N₂O)** emissions from soil.
- Optimizing energy use by controlling the water pump only when needed.
- Supporting sustainable agricultural practices to mitigate the **greenhouse effect**.

---

## 🚀 Getting Started

### 🛠️ Hardware Setup
Connect your components as follows:
| Function        | Pin          |
|----------------|--------------|
| DHT Sensor      | GPIO 13      |
| Soil Moisture   | GPIO 34      |
| Water Level     | GPIO 35      |
| Servo Motor     | GPIO 33      |
| Relay (Pump)    | GPIO 32      |
| RGB LED         | GPIO 25 (R), 26 (G), 27 (B) |
| LCD (I2C)       | SDA/SCL (Default ESP32 I2C pins) |

> Ensure your Arduino IoT Cloud variables match the ones used in the code:
> - `humidity_sensor`
> - `soil_moisture`
> - `pumpActive`
> - `waterlevel`
> - `servo1`
> - `lED` (for RGB color & switch)

---

## 🧾 Cloud Variables

| Variable Name     | Type       | Direction   |
|-------------------|------------|-------------|
| `humidity_sensor` | Float      | Read        |
| `soil_moisture`   | Int        | Read        |
| `pumpActive`      | Boolean    | Read/Write  |
| `servo1`          | Boolean    | Read/Write  |
| `waterlevel`      | Boolean    | Read        |
| `lED`             | Color + Switch | Read/Write |

---

## 📸 System Preview

> (Add photos or GIFs of your hardware setup and dashboard here.)

---

## 🧑‍💻 Author

**Smart Serra Project**  
Created by [Your Name]  
📍 Malaysia  
📧 your@email.com

---

## 📄 License

This project is licensed under the MIT License.

---

## 💬 Motto

**"Water Wisely, Grow Sustainably."**

---

