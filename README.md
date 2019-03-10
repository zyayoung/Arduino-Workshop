# Arduino-Workshop

## Outline

- [Foundations](#foundations-%E5%9F%BA%E7%A1%80)
  - [Arduino (A/D, PWM)](#arduino)
  - [Arduino IDE (prepared)](#arduino-ide)
  - Serial (output HW)
  - Power supply (input, supply by portable charger)
- [Components](#components-%E7%BB%84%E4%BB%B6)
  - [LED & Breadboard & resistance](#led--resistance-led%E5%92%8C%E7%94%B5%E9%98%BB)
  - Servo
  - DC Motor (L298N)
- [Remote Control](#remote-control-%E8%BF%9C%E7%A8%8B%E6%8E%A7%E5%88%B6)
  - PS2
  - model remote control
  - bluetooth
- [EEPROM](#eeprom)

## Foundations 基础

![foundations](https://www.arduino.cc/en/uploads/Main/foundations.svg)

From: [https://www.arduino.cc](https://www.arduino.cc)

### Arduino

#### What is Arduino? 什么是 Arduino？

#### How to purchase an Arduino board? 如何选购 Arduino 版？

|              | Uno      | Nano  | Mega      |
| ------------ | -------- | ----- | --------- |
| Power supply | enough   | weak  | ??        |
| Size         | moderate | small | large     |
| Price        | moderate | low   | expensive |
| Image        | ![Uno](https://www.arduino.cc/en/uploads/Products/Uno.jpg) | ![Nano](https://www.arduino.cc/en/uploads/Products/Nano.jpg) | ![Mega](https://www.arduino.cc/en/uploads/Products/Mega.jpg) |

**\*Tip: If not necessary, please NEVER take Nano into consideration!**

#### Recommended

- [Boards](https://www.arduino.cc/en/Main/Products)
- [Tutorial](https://www.arduino.cc/en/Tutorial/HomePage)
- [Projects](https://create.arduino.cc/projecthub)

### Arduino IDE

#### How to configure an Arduino development environment? 如何配置 Arduino 开发环境？

[Downlaod](https://www.arduino.cc/en/Main/Software)

*Windows users please use Installer to ensure the driver can be installed correctly

*Windows 用户请使用 Installer 以保证驱动正常安装

#### Introduction of usage 使用简介

open the sample program 打开例程

![Code](https://www.arduino.cc/en/uploads/Guide/UNO_Load_Blink.jpg)

choose board type and port 选择版型和端口

![BoardType_UNO](https://www.arduino.cc/en/uploads/Guide/UNO_BoardType.jpg)

![Port](https://www.arduino.cc/en/uploads/Guide/UNO_Port.jpg)

compile and upload your program 编译并上传程序

![Upload](https://www.arduino.cc/en/uploads/Guide/UNO_Upload.png)

From: [https://www.arduino.cc/en/Guide/ArduinoUno](https://www.arduino.cc/en/Guide/ArduinoUno)

### Serial 串口



### Power 供电

## Components 组件

### LED & Resistance LED 和电阻

#### Circut 电路

Arudino has a built-in LED on `LED_BUILTIN` port Arduino 内置 LED 于`LED_BUILTIN`引脚。

connect the long pin of the outside LED with 13 port 将外部 LED 较长的引脚（正极）接在 13 口

connect the short pin of the outside LED with GND port 较短引脚接在 GND（负极）

![Circut](https://www.arduino.cc/en/uploads/Tutorial/ExampleCircuit_bb.png)

#### Code

[More](https://www.arduino.cc/en/Tutorial/Blink)

### Breadboard 面包板

### Servo 舵机

### DC Motor 直流电机

## Remote Control 远程控制

### PS2

### Radio System Transmitter 航模遥控

### Bluetooth

## EEPROM
