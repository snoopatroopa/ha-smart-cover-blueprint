# 🪟 Smart Cover Blueprint

A simplified Home Assistant blueprint for automatic roller shutter and blind control — based on time, sun position, brightness, and weather.

> **Status:** Work in progress / private fork

## Features

- ⏲️ Time-based open/close (fixed time, sunrise/sunset, or sensor)
- ☀️ Sun elevation & brightness-based control
- 🥵 Sun shading / sun protection
- 💨 Ventilation position via window contact sensors
- 👤 Presence-aware behavior
- 🙈 Privacy protection (Sichtschutz): presence + light gated cover position
- 🔀 Manual override protection
- 🎯 Cover type aware: Roller shutter or blind (tilt settings only shown for blinds)
- 🔄 Recovery after a Home Assistant restart or an outage (catches up a missed opening/closing)

## Requirements

- Home Assistant 2024.10.0 or newer
- One `input_text` helper per automation (length: 254 chars) for status tracking

## Installation

1. Copy `blueprints/automation/smart_cover.yaml` into your HA config under:  
   `config/blueprints/automation/`
2. Restart Home Assistant or reload blueprints
3. Create a new automation using this blueprint

## Examples

The `examples/` folder contains Lovelace card YAML for displaying cover status.

## License

Based on [Cover Control Automation](https://github.com/hvorragend/ha-blueprints) by hvorragend.  
Open-source — attribution required for modifications.
