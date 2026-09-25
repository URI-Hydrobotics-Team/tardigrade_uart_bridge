# Tardigrade UART Bridge PCB
A small board that connectes to a host via UART and provides PWM output and GPIO for other boards such as and ESC stack or power management board.


## Techinical Overview
Will be based around the Atmega328p SMD package (which has six configurable PWM outputs). The chip will talk to the host via UART biderctionally. We will flash an arduino bootloader on the MCU for ease of programming.

## Pins
### Main Power Conenctor
- GND
- Power (3.3 - 5v)

### Host Connector
- Serial RX
- Serial TX
- GND

### Power Board Connector
- GND
- V_BATT_MEASURE (analog, voltage divider output for battery voltage)
- 3.3V control
- 5.5V control

### ESC Stack Connector
- GND
- KILL_STATUS (digital, kill switch detection)
- KILL (digital, if kill switch in we can overide it with this)
- PWM_0 - PWM_5 (6x, analog, pwm outputs)











