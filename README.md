<div id="readme" class="Box-body readme blob js-code-block-container">
 <article class="markdown-body entry-content p-3 p-md-6" itemprop="This needs to locked down and 'never' changed"><p><a href="https://www.microchip.com" rel="nofollow"><img src="images/Microchip.png" alt="MCHP" width="300";"></a></p>

# Analog-to-Digital Converter (ADC) - Differential Conversion Using AVR128DA48 Microcontroller


This repository contains an application in which the ADC is configured to convert data from a differential input.

## Related Documentation

- [AVR128DA48 Data Sheet](http://ww1.microchip.com/downloads/en/DeviceDoc/40002183A.pdf)
- [AVR128DA48 Product Family Page](https://www.microchip.com/design-centers/8-bit/avr-mcus/device-selection/avr-da)
- [Using 12-Bit ADC for Conversions, Accumulation, and Triggering Events](https://www.microchip.com/wwwappnotes/appnotes.aspx?appnote=en1001530)

## Software Used

- [MPLAB® X IDE v6.15 or newer](https://www.microchip.com/en-us/tools-resources/develop/mplab-x-ide)
- [MPLAB® XC8 v2.45 or newer](https://www.microchip.com/en-us/tools-resources/develop/mplab-xc-compilers)
- [AVR-Dx Series Device Pack v2.3.272 or newer](https://packs.download.microchip.com)

## Hardware Used

- AVR128DA48 Curiosity Nano [(DM164151)](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/DM164151)
- Curiosity Nano Base for Click boards™ [(AC164162)](https://www.microchip.com/developmenttools/ProductDetails/AC164162)
  <br><img src="images/Curiosity-Nano-Adapter.jpg" width="400">
- Two POT Click boards
  <br><img src="images/pot-click.jpg" width="350">

## Setup

The AVR128DA48 Curiosity Nano Development board is used as the test platform. To integrate the POT Click boards, the Curiosity Nano Base Click boards is used to integrate the POT Click boards.

<br><img src="images/AVR128DA48_CNANO_instructions.png" width="500">

<br>The following configurations must be made:

|Pin           | Configuration      |
| :----------: | :----------------: |
|PD3 (AIN3)    | Analog input       |
|PD4 (AIN4)    | Analog input       |
|PC0 (TX)      | Digital output     |

## Demo

  - Open the Data Visualizer
  <br><img src="images/0_3.png" width="600">
  - Open the drop-down list from the Curiosity Nano COMn port
  <br><img src="images/1.png">

  **Note:** Set the baud rate to 115200.

  - From the drop-down list, select New variable streamer...:
  <br><img src="images/2.png">
  - Configure the Variable Streamer Name and add the desired variable, then click **Next**:
  <br><img src="images/3.png" width="600">
  - Select all the variables to plot, select New axis per data type, and click **Finish**:
  <br><img src="images/4.png" width="600">

Result:
The ADC result will be plotted on the graph by rotating the potentiometers on the POT click boards (after starting the application), as shown in the image below.
<br><img src="images/5.png" alt="Demo" width="800"/>

## Summary 

This application showcases the differential conversion feature of the AVR® DA ADC. 

## How to Program the Curiosity Nano Board

This chapter shows how to use the MPLAB X IDE to program an AVR device with an `Example_Project.X`. This can be applied to any other projects.

- Connect the board to the PC

- Open the `Example_Project.X` project in MPLAB® X IDE

- Set the `Example_Project.X` project as main project

  - Right click the project in the **Projects** tab and click Set as Main Project
    <br><img src="images/Program_Set_as_Main_Project.PNG" width="400">

- Clean and build the `Example_Project.X` project

  - Right click the `Example_Project.X` project and select Clean and Build
    <br><img src="images/Program_Clean_and_Build.PNG" width="400">

- Select AVRxxxxx Curiosity Nano in the Connected Hardware Tool section of the project settings:

  - Right click the project and click **Properties**
  - Click the arrow under the Connected Hardware Tool
  - Select the AVRxxxxx Curiosity Nano (click the **SN**), click **Apply** and then **OK**:
    <br><img src="images/Program_Tool_Selection.PNG" width="600">

- Program the project to the board
  - Right click the project and then Make and Program Device
    <br><img src="images/Program_Make_and_Program_Device.PNG" width="600">

<br>

[Back to Top](#analog-to-digital-converter-adc---differential-conversion-using-avr128da48-microcontroller)<br>
[Back to Related Documentation](#related-documentation)<br>
[Back to Software Used](#software-used)<br>
[Back to Hardware Used](#hardware-used)<br>
[Back to Setup](#setup)<br>
[Back to Demo](#demo)<br>
[Back to Summary](#summary)<br>
[Back to How to program the curiosity nano board](#how-to-program-the-curiosity-nano-board)<br>