# stm32-adc-voltage-reading
completed reading raw analog value from the potentiometer and printed as digitalvalues
## Overview
This project demonstrates how to configure and use the ADC peripheral
in an STM32 microcontroller to read analog voltage and convert it into
a digital value.

## Microcontroller
- STM32F407 (or your MCU)

## Features
- 12-bit ADC resolution
- Single-channel ADC conversion
- Voltage calculation from ADC value
- HAL-based implementation

## Hardware Connections
- Potentiometer middle pin → PA0 (ADC Channel 0)
- 3.3V → Potentiometer VCC
- GND → Potentiometer GND

## Working Principle
1. ADC is configured using STM32CubeMX.
2. ADC conversion is started using HAL.
3. Raw ADC value is read.
4. ADC value is converted to voltage using formula.
5. Voltage can be monitored using debugger / UART.

## Formula Used
Voltage = (ADC_Value × 3.3) / 4095

## What I Learned
- STM32 ADC configuration using CubeMX
- Sampling time and resolution effects
- HAL ADC APIs
- Analog signal handling in STM32

## Future Improvements
- ADC with DMA
- Multi-channel ADC scanning
- UART output of ADC values
