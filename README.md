# ESP32 Smoker Controller

ESP32-based pellet grill controller powered by ESPHome. Replaces standard "dumb" controllers with a smart, PID-controlled system integrated with Home Assistant.

## Features
- **PID Temperature Control**: Native ESPHome PID for stable grill temperatures.
- **Hardware Acceleration**: Orchestrates Auger, Fan, and Igniter via Solid State Relays.
- **Multi-Probe Monitoring**: K-Type thermocouple for the grill and NTC probes for food.
- **Home Assistant Native**: Full dashboard control and mobile notifications.

## Hardware
- ESP32 DevKit V1
- MAX6675/MAX31855 Thermocouple Amplifier
- 4-Channel SSR Module (120V AC)
- NTC 10k/100k Food Probes

## Development
Validate the configuration using Docker:
```bash
docker compose run esphome compile smoker.yaml
```
