# ikea-plugget-esphome
Connect Ikea Plugget LCD Clock to ESPHome for Basic Actions

## Overview
The light of Plugget disturbed me at night, so i wanted to turn it off automatically. Also, changing from and to daylight time should be easier.

# Installation

## Hardware

- Ikea Plugget
- ESP32-C3 Microcontroller

## Wiring 
- Wired the ESP up to the 5v Input of the Plugget.
- Wired positive side of Plus, Minus and Clock Button to GPIO 0,1,3

# Usage
[Use this code](plugget.yaml)
- ESP pulls Pins HIGH on Boot
- When Button in HA is pressed, ESP pulls LOW and therefore simulates physical button press
- Code contains pre-defined HA Buttons for adding or substracing hour / minutes which are basically macros
- Light is also a macro, but reflects assumed state in HA to allow use in Automations


<img width="427" alt="image" src="https://github.com/chriopter/ikea-plugget-esphome/assets/82179548/77b9141d-65e3-4b52-b14b-567ef10f91ec">

<img width="408" alt="image" src="https://github.com/chriopter/ikea-plugget-esphome/assets/82179548/653c031d-6bd7-4359-a996-9796d9e2acd4">

<img width="336" alt="image" src="https://github.com/chriopter/ikea-plugget-esphome/assets/82179548/29391b21-0808-44fd-acf0-2628314a8bcc">

