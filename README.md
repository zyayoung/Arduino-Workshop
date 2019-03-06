# Arduino-Workshop

## Outline

- [Foundations](#foundations-%E5%9F%BA%E7%A1%80)
  - [Arduino (A/D, PWM)](#arduino)
  - [Arduino IDE (prepared)](#arduino-ide)
  - Serial (output HW)
  - 供电 (input, 充电宝供电)
- [Components](#components-%E7%BB%84%E4%BB%B6)
  - [LED & Breadboard & resistance](#led--resistance-led%E5%92%8C%E7%94%B5%E9%98%BB)
  - Servo
  - DC Motor (L298N)
- [Remote Control](#remote-control-%E8%BF%9C%E7%A8%8B%E6%8E%A7%E5%88%B6)
  - PS2
  - 航模遥控
  - 蓝牙
- [EEPROM](#eeprom)

## Foundations 基础

<img src="https://www.arduino.cc/en/uploads/Main/foundations.svg">

From: [https://www.arduino.cc](https://www.arduino.cc)

### Arduino

#### 什么是Arduino？

#### 如何选购Arduino版？

##### Uno

- 供电强
- 大小/接口数量适中

![Uno](https://www.arduino.cc/en/uploads/Products/Uno.jpg)

##### Leonardo

- USB口可模拟鼠标/键盘/手柄

![Leonardo](https://www.arduino.cc/en/uploads/Main/ArduinoLeonardo_mpp.jpg)

##### Nano

- 体积小
- 供电弱
- 便宜
- 折腾

![Nano](https://www.arduino.cc/en/uploads/Products/Nano.jpg)

##### Mega

- 体积大
- 接口多
- 供电？？

![Mega](https://www.arduino.cc/en/uploads/Products/Mega.jpg)

#### Recommended:
- [Boards](https://www.arduino.cc/en/Main/Products)
- [Tutorial](https://www.arduino.cc/en/Tutorial/HomePage)
- [Projects](https://create.arduino.cc/projecthub)

### Arduino IDE

#### 如何配置Arduino开发环境？

[Downlaod](https://www.arduino.cc/en/Main/Software)

*Windows用户请使用Installer以保证驱动正常安装


#### 使用简介

打开例程

![Code](https://www.arduino.cc/en/uploads/Guide/UNO_Load_Blink.jpg)

选择版型和端口

![BoardType_UNO](https://www.arduino.cc/en/uploads/Guide/UNO_BoardType.jpg)

![Port](https://www.arduino.cc/en/uploads/Guide/UNO_Port.jpg)

编译并上传程序

![Upload](https://www.arduino.cc/en/uploads/Guide/UNO_Upload.png)

From: [https://www.arduino.cc/en/Guide/ArduinoUno](https://www.arduino.cc/en/Guide/ArduinoUno)

### Serial 串口

### Power 供电

## Components 组件

### LED & Resistance LED和电阻

#### Circut

Arduino内置LED于`LED_BUILTIN`引脚。 

将外部LED较长的引脚（正极）接在13口，较短引脚接在GND（负极）

![Circut](https://www.arduino.cc/en/uploads/Tutorial/ExampleCircuit_bb.png)

#### Code

> Initialize LED_BUILTIN pin as an output pin with the line:
> 
> `pinMode(LED_BUILTIN, OUTPUT);`
> 
> Turn the LED on with the line:
> 
> `digitalWrite(LED_BUILTIN, HIGH);`
> 
> This supplies 5 volts to the LED anode.
> That creates a voltage difference across the pins of the LED, and lights it up.
>
> [Source](https://www.arduino.cc/en/Tutorial/Blink)

```Arduino
/*
  Blink

  Turns an LED on for one second, then off for one second, repeatedly.

  Most Arduinos have an on-board LED you can control. On the UNO, MEGA and ZERO
  it is attached to digital pin 13, on MKR1000 on pin 6. LED_BUILTIN is set to
  the correct LED pin independent of which board is used.
  If you want to know what pin the on-board LED is connected to on your Arduino
  model, check the Technical Specs of your board at:
  https://www.arduino.cc/en/Main/Products

  modified 8 May 2014
  by Scott Fitzgerald
  modified 2 Sep 2016
  by Arturo Guadalupi
  modified 8 Sep 2016
  by Colby Newman

  This example code is in the public domain.

  http://www.arduino.cc/en/Tutorial/Blink
*/

// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second
}
```

[More](https://www.arduino.cc/en/Tutorial/Blink)

### Breadboard 面包板

### Servo 舵机

### DC Motor 直流电机

## Remote Control 远程控制

### PS2

### Radio System Transmitter 航模遥控

## EEPROM
