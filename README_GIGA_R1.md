# RadioHead GIGA R1 WiFi support

This fork adds compatibility for the Arduino GIGA R1 WiFi using the Arduino Mbed framework.

## Changes
- `RHHardwareSPI.cpp`: handles the GIGA `BitOrder` type used by `SPISettings`.
- `RH_ASK.cpp`: uses Mbed `Ticker` on `ARDUINO_GIGA` instead of AVR timer registers / legacy `HardwareTimer`.

The existing RadioHead API remains unchanged. RFM95/RH_RF95 uses the normal Arduino `SPI` interface.
