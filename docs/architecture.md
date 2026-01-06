# System Architecture

This prototype is a layered embedded sensing system:

## Layers
1) Sensing
- TF-Luna LiDAR provides distance measurements (serial/UART).

2) Control
- Arduino reads distance, applies filtering (optional), and evaluates proximity states.

3) Feedback
- LEDs: multi-stage visual feedback (safe / warning / critical)
- Buzzer: alert patterns based on state
- LCD: live distance readout

## Data Flow
LiDAR → Arduino (state logic) → LEDs + buzzer + LCD

## Design Goals
- Deterministic, state-driven behavior
- Non-blocking timing for alert patterns
- Easy threshold tuning and extension
