# EmbeddedSecuritySystem
Secure STM32-Based Home Security System

This project is a secure home security system using the STM32F103C8T6 microcontroller. It includes RFID authentication, keypad access, intrusion detection, and secure firmware updates while maintaining low power consumption.

Features:
Secure access using RFID and Keypad authentication
Magnetic switches detect unauthorized door/window access
LCD display, LEDs, and a buzzer provide alerts
Secure firmware with readout protection and AES encryption
Low power consumption with optimized component activation
Secure firmware updates with rollback support

Components:
STM32F103C8T6 microcontroller
ST-Link V2 programmer
4×4 Keypad & MFRC522 RFID module
LCD 1602 with I2C, LEDs, Buzzer, Servo Motor
Magnetic switches, Push Button, Breadboard, Wiring

How It Works:
The system remains idle, waiting for user input.
Users authenticate using an RFID card or Keypad.
If authentication is successful, the servo motor unlocks the door, and feedback is provided through the LCD and LED.
If unauthorized access is detected, the red LED and buzzer activate, and the event is logged.

Security & Debugging:
Alerts trigger when tampering is detected.
Secure debugging via STM32 Secure Debug Authentication.
Self-test mode checks hardware integrity.
Secure logging over UART, SWD, or JTAG.

Environmental Requirements:
Operates between -20°C and +70°C.
Dust and moisture resistant (IP54).
Shock and vibration resistant.
