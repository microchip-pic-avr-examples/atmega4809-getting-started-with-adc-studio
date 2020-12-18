<!-- Please do not change this logo with link -->
[![MCHP](images/microchip.png)](https://www.microchip.com)

# Getting Started with Analog-to-Digital Converter (ADC) Examples (Microchip Studio)

  This repository contains examples of bare metal source code for Analog-to-Digital Converter (ADC) as described in [TB3209-Getting Started with Analog-to-Digital Converter (ADC)](http://ww1.microchip.com/downloads/en/Appnotes/TB3209-Getting-Started-with-ADC-90003209A.pdf) document from Microchip. The repository contains a Microchip Studio Solution with multiple projects inside:

* [<strong>ADC Event Triggered:</strong>](Event_Triggered) The purpose of this project is to provide an example on how to configure the ADC to trigger a conversion on a specific event (for more details, see [<strong>ADC Event Triggered</strong>](Event_Triggered))
* [<strong>ADC Free Running:</strong>](Free_Running) This example uses ADC in Free-Running mode. When configuring the ADC in Free-Running mode, the next conversion starts immediately after the previous one completes (for more details, see [<strong>ADC Free Running</strong>](Free_Running))
* [<strong>ADC Sample Accumulator:</strong>](Sample_Accumulator) This example uses the ADC in Sample Accumulator mode. In Sample Accumulator mode the ADC can add up to 64 samples in an accumulator register (for more details, see [<strong>ADC Sample Accumulator</strong>](Sample_Accumulator))
* [<strong>ADC Single Conversion:</strong>](Single_Conversion) The simplest mode of using the ADC is to make a single conversion (for more details, see [<strong>ADC Single Conversion</strong>](Single_Conversion))
* [<strong>ADC Window Comparator:</strong>](Window_Comparator) This example uses the ADC in Window Comparator mode. In this mode, the device can detect if the ADC result is below or above a specific threshold value (for more details, see [<strong>ADC Window Comparator</strong>](Window_Comparator))

## Related Documentation
More details and code examples on the ATMEGA4809 can be found at the following links:
- [TB3209-Getting Started with Analog-to-Digital Converter (ADC)](http://ww1.microchip.com/downloads/en/Appnotes/TB3209-Getting-Started-with-ADC-90003209A.pdf)
- [ATMEGA4809 Product Page](https://www.microchip.com/wwwproducts/en/ATMEGA4809)
- [ATMEGA4809 Code Examples on GitHub](https://github.com/microchip-pic-avr-examples?q=atmega4809)
- [ATMEGA4809 Project Examples in START](https://start.atmel.com/#examples/ATMEGA4809XplainedPro)


## Software Used
- Microchip Studio 7.0.2542 or newer [(https://www.microchip.com/mplab/microchip-studio)](https://www.microchip.com/mplab/microchip-studio)
- ATmega_DFP 1.5.362 or newer Device Pack


## Hardware Used
- ATMEGA4809 Xplained Pro [(ATMEGA4809-XPRO)](https://www.microchip.com/developmenttools/ProductDetails/ATMEGA4809-XPRO)
