# Pressure Run Game (MATLAB)

**Developer:** Ta'shawnna Green  
**Technologies Used:** MATLAB, App Designer, FSR, ADXL337 Accelerometer, DAQ, Signal Filtering

## 🧠 Overview
Pressure Run is a 2-player obstacle maze game built in MATLAB App Designer. Players control a dot using real-world sensors: an FSR for rightward movement and an accelerometer for up/down. The goal is to navigate through obstacles to reach a green flag.

## 🎮 Features
- Force-sensitive resistor (FSR) controls forward X-axis movement  
- ADXL337 accelerometer controls Y-axis up/down movement  
- Obstacle collision detection  
- Win condition with flag visual and timer  
- Turn-based system with two players (red and blue)  
- DAQ interface integration  
- UNC-themed colors and design  
- Optional confetti animation and timer scoring

## 📸 Screenshots
*(Add gameplay screenshots here once uploaded)*

## 🛠 Hardware
- SparkFun FSR (SEN-09376)  
- ADXL337 analog accelerometer  
- RC filter to smooth accelerometer signal  
- Circuit includes voltage divider and DAQ (AD3) integration

## 🧪 Engineering & Signal Processing
- Capacitor filtering to reduce accelerometer noise  
- Voltage divider circuit design  
- MATLAB code to interpret real-time analog voltages

## 📂 File Structure
- `pressure_run_game.mlapp` — Full App Designer GUI  
- `fsr_read.m`, `accel_filter.m`, `collision.m` — Sub-functions  
- `README.md` — You’re here!

## ⚠️ Important Note

This MATLAB game **requires real-time sensor input** from a physical circuit using a Force Sensitive Resistor (FSR), an ADXL337 analog accelerometer, and a DAQ (AD3). The game will not run correctly without this hardware.

For testing/demo purposes, you can simulate signals in MATLAB by replacing analog input functions with dummy data.


% Simulated FSR/accelerometer input for testing GUI
fsr_sim = 0.5 + 0.1 * randn(1, 1000);  % Fake FSR signal
accel_sim = sin(linspace(0, 2*pi, 1000));  % Fake Y-axis motion


