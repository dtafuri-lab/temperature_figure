# temperature_figure

![status](https://img.shields.io/badge/status-in%20progress-yellow)

A 3D-printed ambient temperature object that physically signals what to wear —
jacket, hoodie, or t-shirt — by rotating a figure's arm based on outdoor temperature.

---

## How It Works

Two wireless units communicate over Bluetooth Low Energy (BLE):

**External Unit** — outdoors, sensing
- MCU: Teyleten ESP32-S3 Supermini
- Sensor: MCP9808 I²C temperature sensor
- Power: Qimoo 800mAh LiPo + HiLetgo TP4056 USB-C charger
- Reads temperature → broadcasts value over BLE

**Internal Unit** — indoors, movement
- MCU: Adafruit QT Py RP2040
- Actuator: MG90S metal-gear micro servo
- Power: PowerBoost 1000C + EEMB 1100mAh LiPo
- Receives BLE packet → moves servo to one of three positions

| Temperature | State   | Arm Angle |
|-------------|---------|-----------|
| Below 12°C  | Jacket  | −38°      |
| 12 – 22°C   | Hoodie  | 0°        |
| Above 22°C  | T-Shirt | +52°      |

---

## Progress

**April 19, 2026** — Body design complete, ready to 3D print.
All electronics fitted to enclosure. This week: print, assemble, and bring it to life.

---

🔗 [github.com/dtafuri-lab/temperature_figure](https://github.com/dtafuri-lab/temperature_figure)
