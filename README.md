# ESP-UWB

## Spesification
- esp32 wroom
- dwm1004c
- connected with serial uart between esp and dwm
- header i2c for oled display
- header pinout esp32
- pad smd dwm1004c
- modul charger tp4056
- switch on off

## Preview Hardware
<p align="center">
  <img src="DOC/PINOUT-DWM1004C.jpeg" width="75%" height="75%">
  <img src="DOC/PINOUT-ESP32.jpeg" width="75%" height="75%">
</p>


# Documentation 
- [Dimension](https://github.com/juarendra/ESP-UWB/blob/main/HARDWARE/dimension_esp-uwb.pdf)
- [BOM](https://github.com/juarendra/ESP-UWB/blob/main/DOC/BOM_ESP-UWB.csv)

## Connection ESP32 to DWM1004c
<p align="center">
  <img src="DOC/ESP32_Pin_Mapping.png" width="75%" height="75%">
  <img src="DOC/UWB_Pin_Mapping.png" width="75%" height="75%">
</p>
ESP32 and DWM1004c are connection with serial , you can see that ESP32 use pin IO16 and IO7 for serial and connected with DWM1004C with pin PB7 and PB6. Serial Connection is interface that STM32L have, and STM32 connected with DMW1000 with SPI. You must flash STM32 for reading data from DWM1000 and send it VIA Serial to ESP32.

You can flash STM32L using STlink and connected to SMD pad on Bottom of PCB