# Oven-operating-system
Project Overview
This project implements a Smart Oven Controller using the PIC16F877A microcontroller.
The system allows the user to enter a cooking time, start or pause the countdown, monitor temperature
and humidity, detect gas leakage, activate a child lock, and display the system status on a 16x2 LCD.
The controller uses a non-blocking main loop with a Timer0-based system tick for time management.
Main Features
 Time entry using a 4x3 keypad in MMSS format.
 Start, pause/resume, reset, and mode buttons.
 Countdown timer controlled by Timer0 interrupt.
 Temperature and humidity monitoring using DHT22.
 Gas leakage detection using an MQ-2 digital output.
 Emergency stop mode when gas is detected.
 Emergency reset requires the gas signal to become safe and the reset button to be held for 3
seconds.
 Child lock using a long press on the * key.
 Direct access to the temperature screen using a long press on the # key.
 Four LCD screens:
 Main screen
 Temperature and humidity screen
 Safety screen
 System screen
 10-segment bargraph for countdown progress.
 Green, yellow, and red status LEDs.
 Buzzer patterns for finished and emergency states.
 Button and keypad debouncing.
 Temporary LCD notification messages.
Microcontroller and Software
 Microcontroller: PIC16F877A
 Oscillator Frequency: 20 MHz
 Oscillator Mode: HS
 Compiler: MPLAB XC8
 Development Environment: MPLAB X IDE
 Programming Language: Embedded C
Required Hardware
 PIC16F877A microcontroller
 20 MHz crystal oscillator
 Two crystal capacitors
 16x2 LCD
 4x3 matrix keypad
 DHT22 temperature and humidity sensorPage 2
 MQ-2 gas sensor module
 10-segment LED bargraph
 Green LED
 Yellow LED
 Red LED
 Buzzer
 Start button
 Pause button
 Reset button
 Mode button
 Pull-up and current-limiting resistors
 5 V regulated power supply
 PIC programmer such as PICkit
