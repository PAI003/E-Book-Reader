# E-Book-Reader

  OpenBook is a minimalist eBook reader built on the ESP32-C6 platform, featuring a 7.5-inch e-paper display, a Li-Po battery, USB-C charging, and physical control buttons.
The device is designed to be energy-efficient and user-friendly, with a straightforward interface managed via GPIOs. Its text display functionality is tailored to deliver a clean, comfortable e-reading experience.

# Block Diagram


![SchemaBloc](https://github.com/user-attachments/assets/b8347619-2053-4680-8157-0329855542f4)

# BOM

| Component  | Purchase Link | DataSheet |
| ------------- | ------------- | -------------  
| BOOT_BUTTON  | https://ro.mouser.com/ProductDetail/Panasonic/EVQ-P7L01P?qs=rJ%252BziJWpyszWhhNszc02jQ%3D%3D&_gl=1*xzqk3l*_ga*dW5kZWZpbmVk*_ga_15W4STQT4T*dW5kZWZpbmVk*_ga_1KQLCYKRX3*dW5kZWZpbmVk | https://componentsearchengine.com/Datasheets/2/EVQP7L01P.pdf |
| C1  | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C1_BAT | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C1_BAT2 |	https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 |	https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C2 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C2_BAT | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C3 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C4 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C4_USB | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C5 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C5_USB | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C6 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C7 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C8 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C9 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C10 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| C10_SUPERCAP | https://ro.mouser.com/ProductDetail/Seiko-Semiconductors/CPH3225A | https://ro.mouser.com/datasheet/2/360/Seiko_Instruments_MicroBattery_E_20230330_2024Jan_-3561061.pdf |
| CHANGE_BUTTON | https://ro.mouser.com/ProductDetail/Panasonic/EVQ-P7L01P | https://componentsearchengine.com/Datasheets/2/EVQP7L01P.pdf |
| C_DELAY | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| D1 | https://ro.mouser.com/ProductDetail/STMicroelectronics/USBLC6-2SC6Y | https://ro.mouser.com/datasheet/2/389/usblc6_2sc6y-1852505.pdf |
| D2 | https://ro.mouser.com/ProductDetail/KYOCERA-AVX/SD0805S020S1R0 | https://ro.mouser.com/datasheet/2/40/schottky-3165252.pdf |
| D3 | https://ro.mouser.com/ProductDetail/Vishay-Semiconductors/MBR0530 | https://www.onsemi.com/pdf/datasheet/mbr0530-d.pdf |
| D4 | https://ro.mouser.com/ProductDetail/Vishay-Semiconductors/MBR0530 | https://www.onsemi.com/pdf/datasheet/mbr0530-d.pdf |
| D5 | https://ro.mouser.com/ProductDetail/Vishay-Semiconductors/MBR0530 | https://www.onsemi.com/pdf/datasheet/mbr0530-d.pdf |
| D6 | https://ro.mouser.com/ProductDetail/Littelfuse/PGB1010603MR | https://www.littelfuse.com/assetdocs/pulseguard-esd-suppressors-pgb1-datasheet?assetguid=8a337998-d54d-466b-be4e-dc5bcd1f9321 |
| D7 | https://ro.mouser.com/ProductDetail/KYOCERA-AVX/SD0805S020S1R0	https://ro.mouser.com/datasheet/2/40/schottky-3165252.pdf |
| D8 | https://ro.mouser.com/ProductDetail/Littelfuse/PGB1010603MR | https://www.littelfuse.com/assetdocs/pulseguard-esd-suppressors-pgb1-datasheet?assetguid=8a337998-d54d-466b-be4e-dc5bcd1f9321 |
| D9 | https://ro.mouser.com/ProductDetail/Littelfuse/PGB1010603MR | https://www.littelfuse.com/assetdocs/pulseguard-esd-suppressors-pgb1-datasheet?assetguid=8a337998-d54d-466b-be4e-dc5bcd1f9321 |
| D10 | https://ro.mouser.com/ProductDetail/Littelfuse/PGB1010603MR | https://www.littelfuse.com/assetdocs/pulseguard-esd-suppressors-pgb1-datasheet?assetguid=8a337998-d54d-466b-be4e-dc5bcd1f9321 |
| D11 |	https://ro.mouser.com/ProductDetail/Littelfuse/PGB1010603MR |	https://www.littelfuse.com/assetdocs/pulseguard-esd-suppressors-pgb1-datasheet?assetguid=8a337998-d54d-466b-be4e-dc5bcd1f9321 |
| D12 | https://ro.mouser.com/ProductDetail/Littelfuse/PGB1010603MR | https://www.littelfuse.com/assetdocs/pulseguard-esd-suppressors-pgb1-datasheet?assetguid=8a337998-d54d-466b-be4e-dc5bcd1f9321 |
| EPD_C1 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| EPD_C2 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| EPD_C3 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| EPD_C4 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| EPD_C5 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| EPD_C6 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| EPD_C7 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| EPD_C8 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| EPD_C9 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| EPD_C10 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| EPD_C11 | https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 | https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| EPD_C12 |	https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106 |	https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf |
| IC1 |	https://ro.mouser.com/ProductDetail/ROHM-Semiconductor/BD5229G-TR |	https://fscdn.rohm.com/en/products/databook/datasheet/ic/power/voltage_detector/bd52xxg-e.pdf |
| IC4 | https://ro.mouser.com/ProductDetail/Torex-Semiconductor/XC6220A331MR-G | https://ro.mouser.com/datasheet/2/760/xc6220-3371556.pdf |
| J1 | https://ro.mouser.com/ProductDetail/Hirose-Connector/FH34SRJ-24S-0.5SH99 |	https://ro.mouser.com/datasheet/2/185/FH34SRJ_24S_0_5SH_99__CL0580_1255_6_99_2DDrawing_0-1615044.pdf |
| J2 | https://ro.mouser.com/ProductDetail/GCT/USB4110-GF-A |	https://ro.mouser.com/datasheet/2/837/GCT_USB4110_Product_Drawing___20k_cycles-3455479.pdf |
| J3 | https://ro.mouser.com/ProductDetail/SparkFun/PRT-14417 |	https://ro.mouser.com/datasheet/2/813/Qwiic_Connector_Datasheet-1223982.pdf |
| J4 | https://store.comet.srl.ro/Catalogue/Product/43497/ | https://store.comet.bg/download-file.php?id=8824 |
| L1 | https://ro.mouser.com/ProductDetail/Wurth-Elektronik/744043680 | https://www.we-online.com/components/products/datasheet/744043680.pdf |
| PFMF.050.1 | https://ro.mouser.com/ProductDetail/KEMET/VE1812K401R050 | https://ro.mouser.com/datasheet/2/447/KEM_V0003_VE-3316901.pdf |
| Q1 | https://ro.mouser.com/ProductDetail/Diodes-Incorporated/DMG2305UX-7 | https://www.diodes.com/assets/Datasheets/DMG2305UX.pdf |
| Q2 | https://ro.mouser.com/ProductDetail/Diodes-Incorporated/DMG2305UX-7 | https://www.diodes.com/assets/Datasheets/DMG2305UX.pdf |
| Q3 | https://ro.mouser.com/ProductDetail/Vishay-Semiconductors/SI1308EDL-T1-GE3 | https://www.vishay.com/docs/63399/si1308edl.pdf |
| R1 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R1_PINH | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R1_PINH1 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R1_BAT | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R1_PWRUSB | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R2 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R2_PINH |	https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R2_PINH1 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL |	https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R2_USB | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R2_USB1 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R2_BAT | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R3 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R4 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL |	https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R5 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL |	https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R6 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R7 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R8 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R9 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R10 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| RESET_BUTTON | https://ro.mouser.com/ProductDetail/Panasonic/EVQ-P7L01P | https://componentsearchengine.com/Datasheets/2/EVQP7L01P.pdf |
| R_BOOT | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R_CAPACITOR |	https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R_CHANGE | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R_CL1 | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| R_RESET | https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL | https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf |
| SENSOR2 | https://ro.mouser.com/ProductDetail/Bosch-Sensortec/BME680 | https://ro.mouser.com/datasheet/2/783/BST_BME680_DS001-1509608.pdf |
| SJ1 | https://grabcad.com/library/solder-jumpers-1 | https://grabcad.com/library/solder-jumpers-1 |
| TP1 | CUSTOM | CUSTOM |
| TP2 |	CUSTOM | CUSTOM |
| TP3 | CUSTOM | CUSTOM |
| TP4 |	CUSTOM | CUSTOM |
| TP5 |	CUSTOM | CUSTOM |
| TP6 |	CUSTOM | CUSTOM |
| TP7 |	CUSTOM | CUSTOM |
| TP8 | CUSTOM | CUSTOM |
| TP9 |	CUSTOM | CUSTOM |
| TP10 | CUSTOM |	CUSTOM |
| TP11 | CUSTOM | CUSTOM |
| TP12 | CUSTOM |	CUSTOM |
| TP13 | CUSTOM |	CUSTOM |
| TP14 | CUSTOM |	CUSTOM |
| TP15 | CUSTOM |	CUSTOM |
| TP16 | CUSTOM |	CUSTOM |
| TP17 | CUSTOM |	CUSTOM |
| U1 | https://ro.mouser.com/ProductDetail/Winbond/W25Q512JVEIQ |	https://ro.mouser.com/datasheet/2/949/Winbond_W25Q512JV_Datasheet-3240039.pdf |
| U2 | https://ro.mouser.com/ProductDetail/Espressif-Systems/ESP32-C6-WROOM-1-N8 | https://ro.mouser.com/datasheet/2/891/Espressif_ESP32_C6_WROOM_1__Datasheet_V0_1_PRELIMI-3239987.pdf |
| U3 | https://ro.mouser.com/ProductDetail/Analog-Devices-Maxim-Integrated/DS3231SN | https://ro.mouser.com/datasheet/2/609/DS3231-3421123.pdf |
| U4 | https://ro.mouser.com/ProductDetail/Analog-Devices-Maxim-Integrated/MAX17048G+T10 | https://ro.mouser.com/datasheet/2/609/MAX17048_MAX17049-3469099.pdf |
| U5 | https://ro.mouser.com/ProductDetail/Microchip-Technology/MCP73831T-2ACI-OT	https://ro.mouser.com/datasheet/2/268/MCP73831_Family_Data_Sheet_DS20001984H-3441711.pdf |


# Specifications

## Screen: ##
 * Type: E-paper display
 * Diagonal: 7.5"
 * Resolution: 800x480 pixels
 * Connectivity: SPI

## Memory: ##
 * Internal: 64 MB NOR Flash
 * External: SD Card
 * RTC module
 * Model: DS3231
 * Connectivity: I2C

## USB-C port: ##
 * Role: Power and data communication
 * Power
 * Battery: Li-Po 3.7V, 2500 mAh
 * Charging circuit: MCP73831
 * Battery level monitoring: MAX17048 (I2C protocol)
 * Voltage regulator: LDO, 3.3V for ESP32-C6

## Sensors: ## 
 * Model: BME688
 * Connectivity: I2C

## Touch control: ##
 * Buttons: 3 buttons connected to the microcontroller's GPIO pins

# Hardware Description #
 * ESP32-C6-WROOM-1-N8 – Serves as the main microcontroller, featuring built-in Wi-Fi and Bluetooth Low Energy (BLE). It handles system communication, sensor data, and display control.

 * BME688 – A multi-functional environmental sensor capable of measuring temperature, humidity, pressure, and gas levels. Interfaces via I²C.

 * DS3231SN – A high-accuracy Real-Time Clock (RTC) module that ensures precise timekeeping. Connected through I²C.

 * MAX17048 – A battery monitoring chip with I²C support, offering real-time State of Charge (SOC) readings.

 * SD Card Module – Enables local data storage and communicates with the ESP32 over the SPI bus.

 * E-Ink Display – An energy-efficient e-paper display that operates through SPI; utilizes control lines like EPD_CS, EPD_DC, EPD_RST, and EPD_BUSY.

 * W25Q512JVEIQ (64MB NOR Flash) – External SPI flash memory used for storing firmware, logs, or large data sets.

 * BOOT and RESET Buttons – Linked to GPIOs for entering bootloader mode and performing hardware resets.

 * MCP73831 – A dedicated Li-Po battery charging IC that manages the charging cycle.

 * XC6220A331MR-G (LDO Regulator) – A low-dropout (LDO) regulator that supplies 3.3V to system components from either battery or USB input.

 * USB-C Port (USB4110-GF-A) – Provides power delivery and acts as a serial interface for uploading code and debugging.

#  ESP32-C6 Microcontroller #


![Screenshot (63)](https://github.com/user-attachments/assets/5f35fd77-12d4-4d87-a3dc-6184afb85af8)

## IO0 - INT_RTC ##
 * Interrupt signal that can wake up the ESP32 from deep sleep.
 * Used by RTC.

## IO1 – 32KHZ ##
 * The DS3231’s 32.768 kHz clock output, routed to the ESP32‐C6.
 * Used by ESP32‐C6.

## IO2 – MISO ##
 * Hardware-dedicated SPI pin, offering high speed and native compatibility.
 * Used by NOR Flash, E-Paper, microSD.

## IO3 - EPD_BUSY ##
 * GPIO status signal sent by the EPD driver, ESP32 reads it to check if the screen is busy.
 * Used by E-Paper Display.

## IO4 – SS_SD ##
 * Selects the SD card during reading; chosen to avoid conflicts with other CS lines already in use.
 * Used by microSD Card.

## IO5 – EPD_DC ##
 * Control signal specific to EPD to differentiate between commands and data.
 * Used by E-Paper Display.

## IO6 – SCK ##
 * Recommended pin for SPI clock in multi-device implementations; allows SPI bus sharing.
 * Used by NOR Flash, E-Paper, microSD.

## IO7 – MOSI ##
 * Utilized for SPI data transmission, compatible with all connected SPI peripherals.
 * Used by NOR Flash, E-Paper, microSD.

## IO9 – IO/BOOT ##
 * Standard pin for entering programming mode on the ESP32-C6.
 * Used by BOOT Button.

## IO10 - EPD_CS ##
 * Selects the display during SPI transfers; doesn’t interfere with the rest of the SPI devices.
 * Used by E-Paper Display.

## IO11 – FLASH_CS ##
 * Dedicated pin to activate the external Flash memory without interfering with other SPI peripherals.
 * Used by External NOR Flash Memory.

## IO12 – USB_D- ##
 * Direct USB data lines for the built‐in USB peripheral, going to the USB connector.
 * Used by USB-C connector.

## IO13 – USB_D+ ##
 * Direct USB data lines for the built‐in USB peripheral, going to the USB connector.
 * Used by USB-C connector.

## IO15 – IO/CHANGE ##
 * General-purpose GPIO chosen for user-defined actions (e.g. Next Page).
 * Used by CHANGE Button.

## IO16 – TX ##
 * Traditional serial line used for flashing the older ESP chips and debug logs.
 * Used by Serial Debug.

## IO17 – RX ##
* Traditional serial line used for flashing the older ESP chips and debug logs.
* Used by Serial Debug.

## IO18 – RTC_RST ##
* External manual reset for the RTC, useful for initial synchronization or watchdog purposes.
* Used by RTC.

## IO19 – I2C_PW ##
 * 3.3V rail dedicated to powering I2C peripherals (sensors, RTC, battery gauge).
 * Used by RTC, BME680, Qwiic.

## IO20 – EPD_3V3_C ##
 * 3.3V supply line that powers the E‐paper Display module.
 * Used by E-Paper Display.

## IO21 – SDA ##
 * Data line for I2C communication; can be shared between multiple sensors.
 * Used by RTC, BME680, Qwiic.

## IO22 – SCL ##
 * I2C clock line; synchronizes with SDA for reliable transmission.
 * Used by RTC, BME680, Qwiic.

## IO23 – EPD_RST ##
 * Resets the EPD circuit before initialization or display updates.
 * Used by E-Paper Display.

