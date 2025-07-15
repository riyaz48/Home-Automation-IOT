# 🏠 Home Automation System using NodeMCU and Blynk (IoT)

## 🔧 Description
This is Task 2 of the CodTech Internship. It demonstrates a simple home automation prototype using NodeMCU and Blynk app to control light and fan.

## 🧰 Components
- NodeMCU ESP8266
- 2 LEDs or Relays
- Breadboard, jumper wires
- Blynk app (mobile)
- Arduino IDE

## ⚡ Circuit Connections

| Device | NodeMCU Pin |
|--------|-------------|
| Light  | D1 (GPIO5)  |
| Fan    | D2 (GPIO4)  |

## 📱 Blynk Setup
1. Create a project on Blynk app
2. Device: NodeMCU
3. Connection: Wi-Fi
4. Add 2 buttons:
   - Light → V1
   - Fan → V2
5. Set buttons to switch mode
6. Use the Auth Token from email in Arduino code

## 📤 Deliverable
A working home automation system that controls devices using the Blynk mobile app.

## 🎯 Result
- Light ON/OFF from mobile
- Fan ON/OFF from mobile
