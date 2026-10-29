# Back-EMF Detector (ESP32)

Detects back EMF from an inductor or motor using the ESP32's ADC — useful for checking whether a motor is spinning or for basic motor-feedback experiments.

## Hardware
- ESP32 development board
- Inductor or DC motor
- Voltage divider feeding GPIO 35 (keep the input below 3.3 V)

## How it works
The sketch samples GPIO 35 every 100 ms and reports a detection whenever the raw ADC value exceeds a noise threshold of 100.

## Usage
1. Open `inductor.ino` in the Arduino IDE with ESP32 board support installed.
2. Upload, then open the Serial Monitor at **115200 baud**.

## License

Released under the [MIT License](LICENSE).
