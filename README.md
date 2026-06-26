# STM32_ADC_DMA
A multi-channel ADC data acquisition project built on the STM32F429ZI Discovery Board using STM32CubeIDE and HAL drivers. The project demonstrates efficient, non-blocking analog data acquisition using DMA, with TIM2 triggering periodic ADC conversions and UART used for real-time serial monitoring.

Hardware Used
STM32F429ZI Discovery Board
Potentiometer
LDR (Light Dependent Resistor)
Thermistor
Breadboard and jumper wires
Features
Multi-channel ADC Scan Mode
DMA-based data transfer
Timer-triggered ADC conversions (TIM2 TRGO)
Real-time UART output
Continuous sensor monitoring
Low CPU utilization through DMA
Working Principle

The ADC is configured to sample three analog input channels corresponding to a potentiometer, thermistor, and LDR. TIM2 periodically triggers the ADC conversion sequence. DMA automatically transfers the conversion results into memory without CPU intervention. After every predefined number of samples, the values are transmitted through UART to a serial terminal for monitoring.

Peripherals Used
ADC1
DMA2
TIM2
USART1
GPIO
Technologies
Embedded C
STM32CubeIDE
STM32 HAL Drivers
UART Communication
DMA
Timer Triggered ADC
Learning Outcomes

This project helped me gain practical experience with:

Multi-channel ADC configuration
DMA-based peripheral communication
Timer-triggered sampling
UART communication
Embedded firmware development
STM32 peripheral configuration and debugging
Future Improvements
Convert raw ADC values into engineering units
Display sensor values on an LCD/TFT
Log sensor data for long-term monitoring
Integrate the project into a FreeRTOS-based monitoring system
