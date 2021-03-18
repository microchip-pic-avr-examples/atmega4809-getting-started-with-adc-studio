<!-- Please do not change this logo with link -->
[![MCHP](../images/microchip.png)](https://www.microchip.com)

 # ADC Single Conversion

This code example demonstrates how to make a single conversion with the ADC.

The ADC input pin needs to have the digital input buffer and the pull-up resistor disabled to have the highest possible input impedance. Pin PD6/AIN6 is used for ADC input in this example.

## Related Documentation
More details and code examples on the ATMEGA4809 can be found at the following links:
- [TB3209-Getting Started with Analog-to-Digital Converter (ADC)](https://ww1.microchip.com/downloads/en/Appnotes/TB3209-Getting-Started-with-ADC-DS90003209.pdf)
- [ATMEGA4809 Product Page](https://www.microchip.com/wwwproducts/en/ATMEGA4809)
- [ATMEGA4809 Code Examples on GitHub](https://github.com/microchip-pic-avr-examples?q=atmega4809)
- [ATMEGA4809 Project Examples in START](https://start.atmel.com/#examples/ATMEGA4809XplainedPro)

## Software Used
- Microchip Studio 7.0.2542 or newer [(https://www.microchip.com/mplab/microchip-studio)](https://www.microchip.com/mplab/microchip-studio)
- ATmega_DFP 1.5.362 or newer Device Pack

## Hardware Used
- ATMEGA4809 Xplained Pro [(ATMEGA4809-XPRO)](https://www.microchip.com/developmenttools/ProductDetails/ATMEGA4809-XPRO)

## Setup
The ATMEGA4809 Xplained Pro Development Board is used as test platform.

<br><img src="../images/atmega4809_xplainedpro.jpg" height="300">

The following configurations must be made for this project:

- The CPU frequency is 3.33 MHz.
- Pin PD6 as input and disable the digital input buffer and the pull-up resistor. Pin PD6 will be used as ADC channel.
- Configure ADC as follows: 10-bit mode, use internal voltage reference and the peripheral clock divided by 4 as clock source.

 |Pin                       | Configuration      |
 | :---------------------:  | :----------------: |
 |            PD6           |   Analog input     |

 ## Operation
 1. Connect the board to the PC.

 2. Open the **atmega4809-getting-started-with-adc-studio.atsln** solution in Microchip Studio.

 3. Set the **Single_Conversion** project as Start-Up project. Right click on the project in the **Solution Explorer** tab and click **Set as StartUp Project**.

<br><img src="../images/Start_Up_Project.PNG" height="500">

 4. Build the **Single_Conversion** project: Right click on the **atmega4809-getting-started-with-adc-studio** solution and select **Build Solution**.

<br><img src="../images/Build_Solution.PNG"  height="500">

 5. Select the **ATMEGA4809 Xplained Pro** in the Connected Hardware Tool section of the project settings:
   - Right click on the project and click **Properties**
   - Click on the **Tool** tab
   - Select the ATMEGA4809 Xplained Pro (click on the **SN**) in the **Selected debugger/programmer** section and Save (CTRL + S):

<br><img src="../images/Select_Tool.PNG" height="500">

 6. Program the project to the board: Click on the **Debug** tab and click **Start Without Debugging**.

<br><img src="../images/Start_Without_Debugging.PNG" height="500">

## Summary

This project shows how to configure the ADC peripheral to execute a single conversion cycle.
