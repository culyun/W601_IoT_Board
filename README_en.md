# RT-Thread W60X SDK Description

## brief introduction

RT-Thread W60X SDK consists of a detailed introduction to the development platform W601 IoT Board and rich software resources.

With the rise of the Internet of Things, new development needs continue to emerge, and more and more devices need to add networking functions. At this time, the traditional development method is no longer sufficient to cope with the increasingly rich needs. In order to improve development efficiency, more common components are needed. Therefore, in the W60X SDK, there is not only content on how to use the development board resources, but also an introduction to the common components in RT-Thread and a rich set of software packages for IoT applications. With the help of these software packages, it will bring great convenience to developers in the development process.

## W601 IoT Board Development Board Resources Introduction

### Hardware Resource Description

The W601 IoT Board development board is shown in the figure below:

![W601 IoT Board Development Board](docs/figures/hardware/W60x_HW_origin.png)

The core chip resources of the development board are as follows:

Supports multi-interface, multi-protocol wireless LAN IEEE802.11n (1T1R). Integrated Cortex-M3 core, main frequency 80Mhz. Built-in 1MB Flash and 288KByte SRAM. Integrated RF transceiver front-end RF Transceiver, CMOS PA power amplifier, baseband processor/media access control. Supports SDIO, SPI, UART, GPIO, I²C, PWM, I²S, 7816 and other interfaces, supports multiple encryption and decryption protocols, such as PRNG/SHA1/MD5/RC4/DES/3DES/AES/CRC/RSA, etc.

### Software Resource Description

In this section, we will introduce the software resources of W60X SDK. W60X SDK will provide a wealth of examples for everyone to use. Each example has corresponding comments to facilitate everyone to understand the code. Each example provides MDK and IAR projects, and supports GCC development environment. After getting the project, developers can see the experimental phenomenon by simply compiling and downloading it.

The list of routines is as follows:

| Number| Category| Folder| Description|
| ---- | ------ | ---------------- | ------------------ -------------------------- |
| 01 | Basics | led_blink | LED blinks continuously |
| 02 | Basics | key | Onboard buttons |
| 03 | Basics | rgb_led | RGB LED color changing |
| 04 | Basics | beep | Use buttons to control the buzzer |
| 05 | Basics | ir | Simulating infrared remote control |
| 06 | Driver | lcd | LCD displays text and images |
| 07 | Driver | temp_humi | Driver for temperature and humidity sensor |
| 08 | Driver | als_ps | Driver light/proximity sensor |
| 09 | Components | fs_tf_card | File system examples based on TF card |
| 10 | Components | fal | Use the Flash Abstraction Layer (FAL) component to manage Flash and partitions |
| 11 | Components | kv | Use EasyFlash to store KV parameters |
| 12 | Components | fs_flash | SPI Flash-based file system examples |
| 13 | Components | ulog | Log system routines |
| 14 | Components | adbd | ADB remote debugging tool examples |
| 15 | Components | micropython | Controlling hardware with MicroPython |
| 16 | Internet of Things | wifi_manager | Use WiFi Manager to manage and operate WiFi networks |
| 17 | Internet of Things | web_config_wifi | Quickly access WiFi network using web |
| 18 | Internet of Things | airkiss | Use AirKiss to quickly access WiFi networks |
| 19 | Internet of Things | atk_module | ATK module examples |
| 20 | Internet of Things | at_server | AT command (server side) routine |
| 21 | Internet of Things | mqtt | Using Paho-MQTT package to implement MQTT protocol communication |
| 22 | Internet of Things | http_client | Implementing HTTP Client using the Web Client package |
| 23 | Internet of Things | web_server | Using Web Server Components: WebNet |
| 24 | Internet of Things | websocket | Communicate using the websocket package |
| 25 | Internet of Things | cjson | Parsing JSON data format routine |
| 26 | IoT | tls | TLS communication using mbedtls package |
| 27 | Internet of Things | hw_crypto | Hardware encryption and decryption routines |
| 28 | Internet of Things | ota_ymodem | OTA firmware upgrade via serial Ymodem protocol |
| 29 | Internet of Things | ota_http | OTA firmware upgrade via HTTP protocol |
| 30 | Internet of Things | netutils | Network gadget set usage examples |
| 31 | Internet of Things | cloud_rtt | Access RT-Thread IoT Device Management Cloud Platform |
| 32 | Internet of Things | cloud_onenet | Access to China Mobile OneNET cloud platform |
| 33 | Internet of Things | cloud_ali_iotkit | Connect to Alibaba Cloud IoT Platform |
| 34 | Internet of Things | cloud_ms_azure | Connect to Microsoft Azure Internet of Things Platform |
| 35 | Internet of Things | cloud_tencent | Connect to Tencent Cloud IoT Platform |
| 36 | Comprehensive | demo | Comprehensive example demo |

## WM_Librarie Introduction

WM_Librarie is a development software package provided by Beijing Lianshengde Microelectronics Co., Ltd. This software package provides many basic functions such as underlying hardware drivers, WiFi protocol stack, firmware download, one-click network configuration, etc. The functions of these functions will be introduced below.

### WM_Librarie Function Introduction

### One-click network configuration function

The one-click network configuration function can send the WiFi name and password to the development board through the APP, so that the development board can access the WiFi network. It supports network configuration for most mobile phones and routers on the market, with a high success rate and fast network configuration speed.

### Chip peripheral driver library

Provide driver support for various peripheral modules of W60X chip, including UART, SPI, TIMER, PWM, WDG, etc. It has the characteristics of high operation efficiency and small resource occupation.

WiFi Function Library

It provides complete WiFi protocol stack functions, including support for STA, SOFTAP, AP/STA. The more complete WiFi functions make it easier for ordinary users to operate WiFi, and also enable advanced users to operate WiFi more flexibly.

### Firmware packaging function

It provides a firmware packaging function suitable for various environments. The firmware generator is compiled using a cross-platform language and can run on multiple platforms. It can also generate multiple different types of firmware to suit different upgrade scenarios.

## Documentation

### SDK Documentation

SDK related documents are in the docs folder. The document list is as follows:

| Document Name | Description |
| -------------------------------------------------- -- |----------------------------------------|
| board folder | Development board related documentation, such as schematics, data sheets, etc. |
| AN0001-RT-Thread-Serial Device Application Notes.pdf | Serial Driver Notes |
| AN0002-RT-Thread-Generic GPIO Device Application Note.pdf | Generic GPIO Device Application Note |
| AN0003-RT-Thread-I2C Device Application Note.pdf | I2C Device Application Note |
| AN0004-RT-Thread-SPI Device Application Note.pdf | SPI Device Application Note |
| AN0006-RT-Thread-Using QEMU for simulation debugging.pdf | Using QEMU to debug RT-Thread |
| AN0009-RT-Thread_Using SystemView Analysis Tool.pdf | Using SystemView for Debugging |
| AN0010-RT-Thread-Network Protocol Stack Driver Porting Notes.pdf | lwip driver porting |
| AN0011-RT-Thread-Network Development Application Notes.pdf | Network Development Application Notes |
| AN0012-RT-Thread-File System Application Note.pdf | RT-Thread File System Application Note |
| AN0014-RT-Thread-AT Component Application Notes - Client Side.pdf | RT-Thread AT Component Application Notes - Client Side |
| AN0017-RT-Thread-Creating Standard Projects.pdf | Creating RT-Thread Standard Projects |
| AN0018-RT-Thread-Network Toolset Application Note.pdf | RT-Thread Network Toolset (NETUTILS) Application Note |
| AN0020-RT-Thread-Debugging with Eclipse + QEMU.pdf | Debugging RT-Thread with Eclipse + QEMU |
| AN0021-RT-Thread-Debugging with VS Code + QEMU.pdf | Debugging RT-Thread with VS Code + QEMU |
| AN0022-RT-Thread-ulog Log Component Application Notes - Basics.pdf | RT-Thread ulog Log Component Application Notes - Basics |
| AN0023-RT-Thread-Using QEMU to run dynamic modules.pdf | Using QEMU to run RT-Thread dynamic modules |
| AN0024-RT-Thread-ulog Log Component Application Notes - Advanced Edition.pdf | RT-Thread ulog Log Component Application Notes - Advanced Edition |
| AN0025-RT-Thread-Power Management Components Application Note.pdf | Power Management Application Note |
| RT-Thread Programming Guide.pdf | RT-Thread Programming Guide |
| UM1001-RT-Thread-WebClient User Manual.pdf | WEBCLIENT User Manual |
| UM1002-RT-Thread-ali-iotkit User Manual.pdf | RT-Thread ALI-IOTKIT User Manual |
| UM1003-RT-Thread-OneNET User Manual.pdf | RT-Thread ONENET User Manual |
| UM1004-RT-Thread-OTA User Manual.pdf | RT-Thread OTA User Manual |
| UM1005-RT-Thread-Paho-MQTT User Manual.pdf | PAHO-MQTT User Manual |
| UM1006-RT-Thread-MbedTLS User Manual.pdf | RT-Thread MBEDTLS User Manual |
| UM1007-RT-Thread-Azure-IoT-SDK User Manual.pdf | AZURE-IOT-SDK User Manual |
| UM1008-RT-Thread-Device Maintenance Cloud Platform User Manual.pdf | RT-Thread Cloud Platform User Manual |
| UM1009-RT-Thread-Power Management Component User Manual.pdf | POWER MANAGEMENT User Manual |
| UM1010-RT-Thread-Web Server (WebNet) User Manual.pdf | RT-Thread WEBNET User Manual |
| UM3101-RT-Thread-W60X-SDK Development Manual.pdf | RT-Thread W60X SDK Development Manual |
| UM3102-RT-Thread-W60X-SDK Introduction.pdf | RT-Thread W60X SDK Description |
| UM3103-RT-Thread-W60X-SDK Quick Start.pdf | RT-Thread W60X SDK Quick Start |
| UM3104-RT-Thread-W60X-SDK Release Notes.pdf | RT-Thread W60X SDK Development Manual |

### WM_Librarie Documentation

There are also many documents in the WM_Library library for your reference and study. The following only introduces some documents related to the current SDK. The document path is: RT-Thread_W60X_SDK/libraries/WM_Libraries/Doc.

| Document Name | Description |
| -------------------------------------------------- ----- | ---------------------------- |
| OneShot Lib&Demo folder | One-click network configuration source code and APP |
| W60X_QFLASH_Driver_for_SWD folder | Keil QFLASH driver using JTAG debugging |
| WM_W600_OneShotConfig2.0(Android) SDK User Manual_V1.0.pdf | One-click network configuration Android SDK User Manual |
| WM_W600_OneShotConfig2.0(IOS) SDK User Manual_V1.0.pdf | One-click network configuration IOS SDK User Manual |
| WM_W600_ROM Function Description_V1.1.pdf | ROM Function User Manual |
| WM_W600_SECBOOT Function Description_V1.0.pdf | SECBOOT Function Description Manual |
| WM_W600_SWD Debug Configuration Guide_V1.2.pdf | SWD Debug Configuration Manual |
| WM_W600_Parameter Area User Manual_V1.1.pdf | Parameter Area User Manual |
| WM_W600_Firmware Upgrade Guide_V1.1.pdf | Firmware Upgrade Guide |
| WM_W600_Firmware Generation Instructions_V1.1.pdf | Firmware Generation Instructions Manual |
| WM_W601_Register Manual_v1.2.pdf | Register Manual |

## Prerequisites

The prerequisites for using W60X SDK are as follows:

- RT-Thread Basic Knowledge
- RT-Thread Development Environment

Basic knowledge of RT-Thread can be learned from the RT-Thread Document Center [Document Center](https://www.rt-thread.org/document/site/)