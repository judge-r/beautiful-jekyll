---
type: posts
layout: base
title: My Arduino Low Power Temperature Logger
---

Hi everyone,

I have recently finished writing the code for my Arduino-based temperature datalogger and it is now publicly available on my github page. This was certainly a long and arduous piece of work for me as I am new to computer programming and picked up my coding and electronics skills for this project from scratch. The logger's program uses the C/C++ programming language used in conjunction with the Arduino Integrated Development Environment.

The temperature logger is utilizes two Type K thermocouple sensors hooked up to two MAX31850 amplifiers that utilize a 3-5V bi-directional level shifter to change the voltage to the correct level for compatibility with the Arduino's 5V power output. The type K thermocouples are One-Wire, I2C devices and are thus compatible with the OneWire.h and DallasTemp.h libraries. The wiring for my device is shown in the photo attached to this post, but step-by-step details on how to wire up the device can be found in the Adafruit tutorial. One of the most important components of this logger, however, is the DLS 2.0 DeadBug extreme low power datalogging shield made by DeadBug Prototypes from Norway. This shield has the ability to save significant battery power by completely shutting down the Arduino in between temperature measurements. It is equipped with a DS1307 (or DS1337) real-time clock and a slot for a microSD card for logging temperatures. The RTC will run continuously even when the board is powered off- you just need to pop a CR1220 coin-cell battery into the round battery slot. In addition, the shield can be used with a simple 9V battery. The one I would recommend using is the Energizer Ultimate Lithium 9V for longest performance.

Here are the electronic components (and costs) needed for the logger:

Arduino UNO R3 - $22.00 https://store.arduino.cc/usa/arduino-uno-rev3

DeadBug DLS 2.0 Low-Power Shield - $24.00 https://www.tindie.com/products/Dead_Bug_Prototypes/extreme-low-power-data-logging-shield-for-arduino/

(2) MAX 31850K Type K thermocouple amplifiers - $14.95 ea. https://www.adafruit.com/product/1727

(2) REED Instruments Type K thermocouples - $15.00 ea. https://www.reed-direct.com/product/reed-tp-01-type-k-thermocouple

Bi-Directional 4-channel Level Shifter - $3.95 https://www.adafruit.com/product/757

4GB MicroSD card and adapter - $7.95 https://www.adafruit.com/product/102

CR1220 Coin Cell Battery - $6.99 https://www.amazon.com/CR1220-Battery-Lithium-Button-Batteries/dp/B0751RLXSR/ref=sr_1_1_sspa?ie=UTF8&qid=1520555565&sr=8-1-spons&keywords=battery%2Bcr1220&th=1

TOTAL COST = $121.30 (note: this does not include the cost of any soldering materials, jumper wires, breadboard, or UNO R3 compatible header pins)

The next step of my project is to assemble the biomimetic mussel bed atop a Type S mortar pad and do waterproof testing for my waterproof electronics box. I will post more updates in the coming weeks! If you have questions about the hardware or software for this project, feel free to reach out to me.

-Richard

![http://judge-r.github.io/img/TempLogger.png]

Two Type-K thermocouples (blue) attached to the DeadBug DLS2.0 datalogging shield and Arduino UNO R3
