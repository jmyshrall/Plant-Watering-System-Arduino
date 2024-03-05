# Automated Plant Watering System

## Overview
This repository contains code for an automated plant watering system using a Raspberry Pi and soil moisture sensor. It monitors the soil moisture level and activates a water pump when the soil is dry.

## Developer
- **Name:** Justin Myshrall
- **Date:** 4/6/2023

## Requirements
- Raspberry Pi
- Soil moisture sensor
- Water pump
- Adafruit ADS1115 ADC (Analog-to-Digital Converter)
- Python 3.x
- RPi.GPIO library
- Adafruit_ADS1x15 library

## Installation
1. Clone this repository to your Raspberry Pi.
2. Install the necessary libraries:
    ```bash
    pip install RPi.GPIO adafruit-ads1x15
    ```

## Usage
1. Connect the soil moisture sensor and water pump to the appropriate GPIO pins on the Raspberry Pi.
2. Run the Python script:
    ```bash
    python automated_watering.py
    ```
3. The script will continuously monitor the soil moisture level.
4. If the soil is dry (moisture level > 20000), the water pump will be activated for a specified runtime to water the plant.
5. The pump will only be activated once per day to prevent overwatering.
6. Make sure to adjust the GPIO pin numbers and other parameters as necessary in the code.

## Acknowledgments
- Thanks to Adafruit for the ADS1115 library.