# 1975 Honda CB 750 Electric Conversion:
Spec'ing major electronics, modeling structural battery components, welding 110V 50.4Ah pack, desiging custom temp monitoring board

Hello! Welcome to my repo documenting my electric motorcycle conversion. I started this repo on 2026/06/16 and will be updating it as my project continues. Please reach out with any questions or recommendations; I started this project to learn, after all.

# Motivation:

I started this project to have a complex engineering project and to build a small commuter vehicle that could (mostly) replace my car. I wanted to make an e-bike until I found the power limit of 750W. At that point, I decided to convert a motorcycle which would need registration while offering much more power. I need enough power to keep up with city traffic, but I don't plan on taking the bike on the highway or freeway.

The main reason for this project, though, was to have something interesting to work on in my free time. I wanted to learn more about power, power electronics, PCB design, electric vehicles, batteries, and embedded systems. This project provided obvious avenues to pursue each of these subjects at my own pace.


# Build Thread:

I post updates and ask questions in the thread below if anyone is curious about following along more closely.

https://endless-sphere.com/sphere/threads/1975-honda-cb-750-conversion.129692/



# Key Design Specs:


Average max discharge of >10kW (100A at 104V = 11kW)
~30 minutes at average max discharge (100A * 0.5hrs = 50Ah capacity)
Registerable



# Timeline of work so far:

**2025 Nov-Dec**

Purchased titled disassembled ‘75 Honda CB 750 (more parts not pictured)

<img src="https://github.com/JoshRizzolo/1975-Honda-CB-750-Electric-Conversion/blob/main/Frame.jpg" width="30%" height=30%>


Purchased 200 extra 18650 cells at 2000mAh and 10A Peak discharge

Purchased 18650 Spacers 4x5

Purchased 0.15mm copper and nickel strip

Discovered the capacity and discharge on the above cells would be far too low

Purchased new triple tree and front stanchions for the Bike


<img src="https://github.com/JoshRizzolo/1975-Honda-CB-750-Electric-Conversion/blob/main/Wheel%2C%20Triple%20Tree%2C%20Stanchions.jpg" width="30%" height=30%>



----------------------------------------------------------------------------------------------------------------

**2026 Jan-April**

Spec’d Molicel 21700 P42A cells at 4200mAh and 45A peak discharge

Modeled and printed 8x10 spacers x 8 for 320 cells in 20s16p config (72V)

Performed power calculations and rough loss estimates

With help from others on Endless Sphere, decided that loss at 72V for 10kW was far too high, changed design to 104V

Spec’d 336 cells for 28s12p config at 104V and 50.4Ah (28 * 3.7 = 103.6 ~= 104)

Spec’ed ANT 21-30S BMS

Designed and printed 6x14 21700 spacers (x16)

<img src="https://github.com/JoshRizzolo/1975-Honda-CB-750-Electric-Conversion/blob/main/Spacers%20v2%20and%20bus%20bars.jpg" width="30%" height=30%>


<img src="https://github.com/JoshRizzolo/1975-Honda-CB-750-Electric-Conversion/blob/main/Frame%20and%20Spacers%20Model%201.png" width="30%" height=30%>

Designed, ordered, and received pre-fabbed 0.8mm copper bus bars

<img src="https://github.com/JoshRizzolo/1975-Honda-CB-750-Electric-Conversion/blob/main/Bus%20Bars%202.jpg" width="30%" height=30%>


----------------------------------------------------------------------------------------------------------------


**2026 May-June**

Purchased battery spot-welder (AWithZ UF20B) with 10.5kW output capacity

Purchased Analog discovery 2 for oscilloscope and function generator features

Spec’d Temp sensors and MCU for Battery Monitoring Board (BMB) (DS18B20 and STM32G0B1 respectively)

Purchased temp sensors and MCU breakout board for BMB

Planned for 4 temp sensors per GPIO pin on the MCU and wanted many extra GPIO pins for future functions including microSD and BLE functionality to store and transmit data logs

<img src="https://github.com/JoshRizzolo/1975-Honda-CB-750-Electric-Conversion/blob/main/STM32G0B1%20Breakout%20board%20and%20DS18B20.jpg" width="30%" height=30%>

Installed STM32CubeIDE for VSCode

Investigated connecting to the breakout board and starting projects




 
