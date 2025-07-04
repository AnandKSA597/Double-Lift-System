# 🛗 SmartLift: Dual Elevator Control System

A smart, Arduino-based dual-elevator prototype that simulates real-world lift behavior with features such as real-time floor detection, load monitoring, priority-based lift dispatching, and user-friendly controls.

---

## 📌 Project Overview

Modern buildings demand efficient and safe vertical transport systems. **SmartLift** is a functional, small-scale **dual-lift system** designed to demonstrate key control strategies like floor sensing, overload detection, and request handling — all implemented using Arduino microcontrollers.

---

## 🎯 Project Objectives

- Design a **functional dual-elevator control** system with two independent lifts.
- Implement **real-time floor detection** using limit switches.
- Integrate a **load cell** to monitor cabin weight and prevent overload.
- Handle **internal and external requests** via push buttons.
- Develop a **priority-based dispatch logic** to assign the nearest lift.

---

## 🧩 Key Features

- 🚀 **Dual Lift Support:** Two independently controlled elevators sharing floor requests.
- ⚖️ **Load Monitoring:** A 1kg load cell measures cabin weight and prevents overloading.
- 🧠 **Smart Dispatch Logic:** The nearest available lift is dispatched based on distance, with a timestamp-based tie-breaker.
- 🔘 **Push Button Inputs:** Simulates internal/external requests for 5 floors.
- 💡 **LED Indicators:** Show active lift status and overload warnings.
- 📟 **LCD Display & Buzzer:** For feedback and alerts.
- 🛑 **Debounce Logic:** Smooth button handling with 20ms software debounce.

---



## 🧠 Logic Summary

- **Floor Detection:** Limit switches at each floor detect lift position.
- **Load Sensing:** Load cell outputs weight data; if overloaded, lift doesn’t move.
- **Lift Assignment:** Nearest idle lift gets assigned the call. If tied, a timestamp is used to resolve conflict.
- **Motion Control:** Controlled via L298N motor driver and Arduino PWM.
- **Overload Alert:** Buzzer and LEDs notify users when capacity is exceeded.

---

## 🧪 Challenges Faced

- **Call Tie Resolution:** Required implementation of timestamp logic when both lifts were equidistant.
- **Button Chatter:** Solved by introducing a 20ms software debounce.
- **Structural Instability:** Rebuilt compartments using plywood with added supports and motor holders for better stability.

---

## ✅ Conclusion

SmartLift successfully simulates a dual-elevator system with intelligent dispatching, real-time floor sensing, and overload protection. It tackles key aspects of vertical mobility design and sets the groundwork for future enhancements like remote monitoring, energy-saving features, or IoT-based control.

---


> 🚦 *"SmartLift: Bringing real-world elevator logic to a compact prototype."*
