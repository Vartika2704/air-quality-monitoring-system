# 🌫️ Air Quality Monitoring System using Arduino

This project uses an Arduino microcontroller to monitor air quality in real time. It reads analog values from an air quality sensor (e.g., MQ135), displays readings on an LCD, and activates alerts like a buzzer and LED when the air quality crosses a specified threshold.

---

## 🛠️ Features

- 📟 Real-time display of air quality (PPM) on a 16x2 LCD
- 🚨 Buzzer and LED alert when air quality is poor
- 📊 Serial output of air quality levels
- 📦 Compact and suitable for portable setups

---

## 🔌 Components Required

- Arduino Uno/Nano
- Air Quality Sensor (e.g., MQ135) – connected to A0
- 16x2 LCD Display
- Buzzer
- LED
- Jumper Wires
- Breadboard

---

## 🔧 Circuit Connections

| Component       | Arduino Pin |
|----------------|-------------|
| LCD RS         | 12          |
| LCD EN         | 11          |
| LCD D4         | 5           |
| LCD D5         | 4           |
| LCD D6         | 3           |
| LCD D7         | 2           |
| Air Sensor OUT | A0          |
| Buzzer         | 8           |
| LED            | 9           |

---

## 🧠 How It Works

- The Arduino reads analog values from the air quality sensor.
- If the value exceeds the set `threshold` (default: 70), the system:
  - Turns on the buzzer
  - Activates the LED
  - Displays **"AQ Level HIGH"** on the LCD
- Otherwise, it displays **"AQ Level Good"** and turns alerts off.

---

## 📟 Sample Output

```
Air Quality: 62
AQ Level Good

Air Quality: 125
AQ Level HIGH
```

---

## 📝 Customization

- **Threshold**: You can adjust the `threshold` value in the code to fine-tune the sensitivity:
  ```cpp
  int threshold = 70;  // Change this value as needed
  ```

---

## 💡 Applications

- Indoor air quality tracking
- Educational demonstrations
- DIY pollution detector
- Home automation safety

---

## 👩‍💻 Author

- 👩‍💻 **Vartika Chaudhary**
