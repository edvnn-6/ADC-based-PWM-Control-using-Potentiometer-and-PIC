# ADC-Based PWM Control with PIC Microcontroller

This project demonstrates how to generate a Pulse Width Modulated (PWM) signal using a PIC microcontroller, where the PWM duty cycle is controlled in real-time by reading the voltage from a potentiometer through the Analog-to-Digital Converter (ADC).

## 👨‍💻 Author
**Edvin Jose Vakaparamban**  
📅 Created on: April 25, 2025

---

## 🎛️ Description

- The system reads analog voltage from a potentiometer (connected to AN0).
- The ADC converts the voltage (0–5V) into a 10-bit digital value (0–1023).
- This digital value is used to adjust the PWM duty cycle in real-time.
- The PWM output can be used to control external components like motors or LEDs.

This simple yet powerful project helps in understanding:
- ADC operation on PIC microcontrollers
- Real-time PWM signal generation
- Hardware-based duty cycle adjustment via analog inputs

---

## 🧰 Components Used

- **PIC Microcontroller** (tested with PIC16F877A)
- **Potentiometer** (5k–10k)
- **Breadboard and Wires**
- **Optional Output Device** (e.g., DC motor, LED with current limiting resistor)

---

## ⚙️ Features

- Real-time ADC to PWM conversion
- PWM output on `RC2 (CCP1 pin)`
- PWM frequency set to approximately **5kHz**
- Fully written in **C (XC8 Compiler)** and configured with MPLAB

---

## 📂 File

- **adcpwm.c** – Main program file:
  - Initializes ADC and PWM
  - Reads analog input from `AN0`
  - Dynamically adjusts PWM duty cycle based on the ADC result

---

## 🔌 Pin Configuration

| Function         | PIC Pin         |
|------------------|-----------------|
| Potentiometer IN | AN0 (RA0)       |
| PWM Output       | CCP1 (RC2)      |

---



