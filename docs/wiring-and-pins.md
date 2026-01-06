# Wiring & Pins

## Hardware
- Arduino Uno
- TF-Luna LiDAR
- 16x2 Character LCD (parallel)
- LEDs (green/yellow/red) + resistors
- Passive buzzer

## Pin Map (fill in your exact pins)
> Update these to match your current wiring.

### LiDAR (TF-Luna)
- VCC → 5V
- GND → GND
- TX → Arduino RX (SoftwareSerial RX pin)
- RX → Arduino TX (SoftwareSerial TX pin)

### Buzzer
- Signal → D? (PWM not required for passive buzzer patterns)
- GND → GND

### LEDs
- Green → D?
- Yellow → D?
- Red → D?

### LCD 16x2 (Parallel)
- RS → D?
- E  → D?
- D4 → D?
- D5 → D?
- D6 → D?
- D7 → D?
- VSS → GND
- VDD → 5V
- VO  → potentiometer (contrast)
- A/K → backlight +/-

## Notes
- Use current-limiting resistors for LEDs.
- Keep LiDAR wiring short for stable UART.
