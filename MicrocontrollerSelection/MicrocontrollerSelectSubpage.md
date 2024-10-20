

| DESIGN CONSIDERATIONS | PROJECT SPECIFIC REQUIRMENTS | PIC 1            | PIC 2     | PIC 3 | 
|-----------------------|------------------------------|------------------|-----------|-------|
|How many GPIO Pins?|   (4)temp sensor + (4)humidity sensor + (2)esp32 + (4)subsystem debug LED +(7) -motor driver +(3) Programmer = 24 total GPIO PINs |                 x|          x|      x|
|Built-in Analog to Digital Converter? How many?|none|                 x|          x|      x|
|Built-in Hardware PWM? How many?|1 PWM for motor driver|                 x|          x|      x|
|Built-in I2C? SPI? How many?|3 I2C for temp and humidity sensor, 1 SPI|                 x|          x|      x|
|Built-in UART? How many?|1 for esp32 (RX&TX) |                 x|          x|      x|
|Other Required Built-In Features?|none. preferably comes with sleep mode|                 x|          x|      x|
|Additional considerations |none|                 x|          x|      x|
|Part Number|                                              ---|                 x|          x|      x|
|Link (URL) to product page|                               ---|                 x|          x|      x|
|Links (URL) to Data Sheets|                               ---|                 x|          x|      x|
|Links (URL) to Application Notes|                         ---|                 x|          x|      x|
|Links (URL) to Code Examples|                             ---|                 x|          x|      x|
|Links (URL) to External Resources|                        ---|                 x|          x|      x|
|Production Unit Cost|                                     ---|                 x|          x|      x|
|Supply Voltage Range|                                     ---|                 x|          x|      x|
|Absolute Maximum Current for entire IC|                   ---|                 x|          x|      x|
|Maximum GPIO Pin Current (Source/Sink)|                   ---|                 x|          x|      x|
| 8-bit or 16-bit Architecture|                            ---|                 x|          x|      x|
|Available IC Packages / Footprints |                      ---|                 x|          x|      x|
|Supports External Interrupts? |                           ---|                 x|          x|      x|
|In-System Programming Capability and Type|                ---|                 x|          x|      x|
|Programming Hardware, Cost, and URL|                      ---|                 x|          x|      x|
|Works with MPLAB® X Integrated Development Environment (IDE)?|                             -|                 x|          x|      x|
|Works with Microchip Code Configurator?|                  ---|                 x|          x|      x|
|Overall Pros|(At least 2)|                 x|          x|      x|
|Overall Cons|(At least 2)|                 x|          x|      x|
|Ranking|  1 = first, 2 = second, 3 = third |                 x|          x|      x|

Final Considerations:
Our team chose the PIC24F16KM204 (PIC 1) as our primary option due to its favorable operating voltage range of 1.8-3.6V, which aligns well with our device's power requirements. This microcontroller offers enhanced capabilities at a competitive price compared to other configurations within its family. The PIC24F16KM104 16-bit architecture provides increased processing speed and scalability for potential future upgrades, making it a good choice for our project. Additionally, the various low power settings available allow us to mitigate most concerns regarding power consumption, which would ensure efficient operation without sacrificing the overall performance of our device. While there are fewer packaging options, specifically a through hole version for testing and supporting resources, the overall advantages in capability, voltage compatibility, and power efficiency made the PIC 1 the best fit for our project's needs.






