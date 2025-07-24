# Pressure Run – Hardware Version

This is the original version of **Pressure Run**, a 2-player MATLAB-based maze game. Players control a red or blue dot through physical sensors:
- **FSR (Force Sensitive Resistor)** for rightward movement (X-axis)
- **ADXL337 Accelerometer** for up/down movement (Y-axis)

🏁 Goal: Navigate through an obstacle maze and reach the green flag before the other player.

## ⚙️ Hardware Requirements
- SparkFun small circular FSR (SEN-09376)
- ADXL337 analog accelerometer
- 10kΩ resistor (for FSR voltage divider)
- Capacitor (for smoothing accelerometer signal)
- DAQ interface (AD3)
- Breadboard + jumper wires
- MATLAB App Designer

## 🖥️ Software Setup
1. Download the `PressureRun_Hardware.mlapp` file from this repository.
2. Open MATLAB and launch App Designer.
3. Connect FSR to analog input 1+, and accelerometer Y-axis to input 2+ of AD3.
4. Make sure DAQ drivers are installed and MATLAB can read analog inputs.
5. Run the game and control the dot using the FSR and accelerometer!

## 🧪 Notes
- Ensure all sensor circuits are properly powered and grounded.
- A capacitor is recommended between the Y-axis and ground to reduce noise.
- Designed and tested on macOS with MATLAB R2024a.

## 📸 Screenshots
Include circuit diagram and game screenshots here.

## 👩🏽‍💻 Author
Ta'shawnna Green – [GitHub](https://github.com/tasgreenunc)

