# Ultrasonic Distance Meter (Arduino + HC-SR04)

This project uses the **HC-SR04 Ultrasonic Sensor** with an **Arduino Uno** to measure distances in centimeters. The measured values are displayed on the **Serial Monitor**. This is a great beginner project to understand ultrasonic sensors, timing, and basic electronics.

---

##  Components Used

- Arduino Uno
- HC-SR04 Ultrasonic Sensor
- Breadboard
- Jumper Wires
- (Optional) 16x2 LCD Display or OLED

---

## 🔌 Pin Connections

| HC-SR04 Pin | Arduino Pin |
|-------------|-------------|
| VCC         | 5V          |
| GND         | GND         |
| Trig        | 9           |
| Echo        | 10          |

---

## How It Works

- The **Trig pin** sends a short HIGH pulse (10 microseconds)
- The **Echo pin** receives the reflected signal
- Arduino calculates distance using the speed of sound

```cpp
distance = duration * 0.034 / 2;
