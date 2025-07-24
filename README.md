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

## 📌 Future Work
- Phase 2: Arduino/JavaScript port  
- Phase 3: Web-based version using React or p5.js  

