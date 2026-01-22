---
title: "6. System Alerts / Telemetry"
weight: 7
---

# 6.5 Telemetry Codes

## Alert Levels
- **Warning**: Yellow alerts indicate conditions approaching dangerous levels
- **Critical**: Red alerts indicate dangerous conditions requiring immediate attention

## ESC (Motor Controller) Alerts

### Temperature Alerts

| Alert | Abbreviation | Warning Threshold | Critical Threshold | Meaning |
| :--- | :--- | :--- | :--- | :--- |
| ESC MOSFET Temperature | MC-F | >90°C / <-10°C | >110°C / <-20°C | High/low temperature on the ESC’s power MOSFETs |
| ESC MCU Temperature | MC-C | >80°C / <-10°C | >95°C / <-20°C | High/low temperature on the ESC’s microcontroller |
| ESC Capacitor Temperature | MC-P | >85°C / <-10°C | >100°C / <-20°C | High/low temperature on the ESC’s capacitor |
| Motor Temperature | MC-M | >105°C / <-20°C | >115°C / <-25°C | High/low temperature on the motor |

### Running Errors (Critical Only)

| Alert | Abbreviation | Trigger Condition | Meaning |
| :--- | :--- | :--- | :--- |
| ESC Over Current | MC-RE-0 | Active when true | ESC detected excessive current draw |
| ESC Locked Rotor | MC-RE-1 | Active when true | Motor is locked or jammed |
| ESC Over Temperature | MC-RE-2 | Active when true | ESC temperature protection triggered |
| ESC Over Voltage | MC-RE-6 | Active when true | Input voltage too high |
| ESC Voltage Drop | MC-RE-7 | Active when true | Input voltage dropped too low |

### Self-Check Errors (Critical - Boot-time Hardware Faults)

| Alert | Abbreviation | Trigger Condition | Meaning |
| :--- | :--- | :--- | :--- |
| Motor Current Output Bad | MC-SE-0 | Active when true | Motor current sensor malfunction |
| Total Current Output Bad | MC-SE-1 | Active when true | Total current sensor malfunction |
| Motor Voltage Output Bad | MC-SE-2 | Active when true | Motor voltage sensor malfunction |
| Capacitor NTC Bad | MC-SE-3 | Active when true | Capacitor temperature sensor malfunction |
| MOS NTC Bad | MC-SE-4 | Active when true | MOSFET temperature sensor malfunction |
| Bus Voltage Range Bad | MC-SE-5 | Active when true | Bus voltage sensor range error |
| Bus Voltage Sample Bad | MC-SE-6 | Active when true | Bus voltage sensor sampling error |
| Motor Z Too Low | MC-SE-7 | Active when true | Motor impedance too low |
| Motor Z Too High | MC-SE-8 | Active when true | Motor impedance too high |
| Motor Voltage Detect 1 Bad | MC-SE-9 | Active when true | Motor voltage detection 1 malfunction |
| Motor Voltage Detect 2 Bad | MC-SE-10 | Active when true | Motor voltage detection 2 malfunction |
| Motor Current Detect 2 Bad | MC-SE-11 | Active when true | Motor current detection 2 malfunction |
| Software/Hardware Incompatible | MC-SE-13 | Active when true | Firmware/hardware version mismatch |
| Bootloader Unsupported | MC-SE-14 | Active when true | Bootloader version not supported |

## BMS (Battery Management System) Alerts

### BMS Temperature Alerts

| Alert | Abbreviation | Warning Threshold | Critical Threshold | Meaning |
| :--- | :--- | :--- | :--- | :--- |
| BMS MOSFET Temperature | BC-F | >50°C / <-10°C | >60°C / <-15°C | High/low temperature on BMS power MOSFETs |
| BMS Balance Temperature | BC-B | >50°C / <-10°C | >60°C / <-15°C | High/low temperature on balance resistors |
| BMS Cell Temperatures | BC-T1/2/3/4 | >50°C / <-10°C | >56°C / <-15°C | High/low temperature in battery cell group 1-4 |

### Voltage and SOC Alerts

| Alert | Abbreviation | Warning Threshold | Critical Threshold | Meaning |
| :--- | :--- | :--- | :--- | :--- |
| BMS High Cell Voltage | BC-CV-H | >4.19V | >4.20V | Individual cell voltage too high |
| BMS Low Cell Voltage | BC-CV-L | <3.2V | <3.0V | Individual cell voltage too low |
| BMS State of Charge | BC-SOC | <15% | <5% | Battery charge level too low |
| BMS Total Voltage | BC-Vtot | <79.2V or >100.4V | <69.6V or >100.8V | Total battery pack voltage out of range |
| BMS Voltage Differential | BC-dV | >0.2V | >0.4V | Voltage difference between cells too high |

### MOSFET State Alerts

| Alert | Abbreviation | Trigger Condition | Meaning |
| :--- | :--- | :--- | :--- |
| BMS Discharge MOS | BC-DSG | Active when false (MOS off) | Discharge MOSFET turned off |

## Internal System Alerts

| Alert | Abbreviation | Warning Threshold | Critical Threshold | Meaning |
| :--- | :--- | :--- | :--- | :--- |
| CPU Temperature | CPU-T | >60°C / <0°C | >80°C / <-10°C | ESP32-S3 processor temperature too high/low |
| Baro initialized | Baro-I | Active when false | | Barometer failed to initialize |

### Notes
- All temperature sensors use hysteresis to prevent alert bouncing (±1°C deadband)
- Voltage thresholds are absolute values without hysteresis
- Boolean alerts (errors/faults) are either active (true) or inactive (false)
- Critical alerts trigger red screen border and vibration
- Warning alerts are displayed in yellow
