<!-- Please do not change this logo with link -->
[![MCHP](../images/microchip.png)](https://www.microchip.com)

 # ADC Event Triggered - Use Case for the ATmega4809 Microcontroller with Microchip Studio

This project provides the Analog-to-Digital (ADC) configuration required to trigger a conversion on a specific event. In this example, the Real-Time Clock (RTC) triggers the ADC conversion, while the on-board LED will toggle each time a conversion is triggered.

## Related Documentation

More details and code examples on the ATMEGA4809 can be found at the following links:
- [TB3209-Getting Started with Analog-to-Digital Converter (ADC)](https://ww1.microchip.com/downloads/en/Appnotes/TB3209-Getting-Started-with-ADC-DS90003209.pdf)
- [ATMEGA4809 Product Page](https://www.microchip.com/wwwproducts/en/ATMEGA4809)
- [ATMEGA4809 Code Examples on GitHub](https://github.com/microchip-pic-avr-examples?q=atmega4809)
- [ATMEGA4809 Project Examples in START](https://start.atmel.com/#examples/ATMEGA4809XplainedPro)

## Software Used
- Microchip Studio 7.0.2594 or newer [(https://www.microchip.com/mplab/microchip-studio)](https://www.microchip.com/mplab/microchip-studio)
- ATmega_DFP 2.1.506 or newer Device Pack

## Hardware Used
- ATMEGA4809 Xplained Pro [(ATMEGA4809-XPRO)](https://www.microchip.com/developmenttools/ProductDetails/ATMEGA4809-XPRO)

## Setup
The ATMEGA4809 Xplained Pro development board is used as test platform.

<br><img src="../images/atmega4809_xplainedpro.jpg" height="300">

The following configurations must be made for this project:

- The CPU frequency is 3.33 MHz
- Configure pin PD6 as input, ADC input channel, and disable the digital input buffer and the pull-up resistor
- ADC configuration: 10-bit mode, use internal voltage reference, use the peripheral clock divided by four as clock source, enable RESRDY interrupt and Event Trigger
- Configure pin PB5 as output, used by LED, and with initial value HIGH, which represents LED OFF
- RTC configured to overflow at 500 ms, and to use 32.768 kHz Oscillator with 32 prescaler
- Event Generator: RTC overflow
- Event User: ADC Start Conversion

 |Pin                       | Configuration      |
 | :---------------------:  | :----------------: |
 |            PB5           |   Digital output   |
 |            PD6           |   Analog input     |

 ## Operation
 1. Connect the board to the PC.

 2. Open the **atmega4809-getting-started-with-adc-studio.atsln** solution in Microchip Studio.

 3. Set the **Event_Triggered** project as Start-Up project. Right click the project in the **Solution Explorer** tab and click **Set as StartUp Project**.

<br><img src="../images/Start_Up_Project.PNG" height="500">

 4. Build the **Event_Triggered** project: Right click the **atmega4809-getting-started-with-adc-studio** solution and select **Build Solution**.

<br><img src="../images/Build_Solution.PNG"  height="500">

 5. Select the **ATMEGA4809 Xplained Pro** in the Connected Hardware Tool section of the project settings:
   - Right click the project and click **Properties**
   - Click the **Tool** tab
   - Select the ATMEGA4809 Xplained Pro (click on the **SN**) in the **Selected debugger/programmer** section and Save (CTRL + S):

<br><img src="../images/Select_Tool.PNG" height="500">

 6. Program the project to the board: Click the **Debug** tab and click **Start Without Debugging**.

<br><img src="../images/Start_Without_Debugging.PNG" height="500">

## Summary

This project shows how to configure the ADC peripheral to execute conversions every time a certain event happens. In this specific example, the RTC overflow, at 500 ms, is used as event generator. Every time a conversion cycle is triggered, the on-board LED is toggled to signal the end of a conversion.
