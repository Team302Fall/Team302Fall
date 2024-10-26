

| DESIGN CONSIDERATIONS | PROJECT SPECIFIC REQUIRMENTS | PIC 1 (PIC24FV16KM204-I/PT) ![](PIC24FV16KM204.jpg)           | 
|-----------------------|---------------------------------------------------|------------------|
|How many GPIO Pins?|   (4)temp sensor + (4)humidity sensor + (2)esp32 + (4)subsystem debug LED + (7)motor driver +(3) Programmer = 24 total GPIO PINs |37|          21|      36|
|Built-in Analog to Digital Converter? How many?|none|                 2|
|Built-in Hardware PWM? How many?|1 PWM for motor driver|                 5|
|Built-in I2C? SPI? How many?|3 I2C for temp and humidity sensor, 1 SPI|                2|
|Built-in UART? How many?|1 for esp32 (RX&TX) |                 1|          2|      1|
|Other Required Built-In Features?|none. preferably comes with sleep mode|                 4 low power modes|
|Additional considerations |none|                 x|          x|      x|
|Part Number|                                              ---|                 PIC24F16KM204|          
|Link (URL) to product page|                               ---|                 [link](https://www.digikey.com/en/products/detail/duracell-industrial-operations-inc/AA-NIMH-DURACELL/16164081) | 
|Links (URL) to Data Sheets|                               ---|                 [Link](https://ww1.microchip.com/downloads/aemDocuments/documents/MCU16/ProductDocuments/DataSheets/PIC24FV16KM204-Family-Data-Sheet-DS30003030C.pdf)|  
|Links (URL) to Application Notes|                         ---|                 [Link](https://www.microchip.com/en-us/application-notes/an1044)  [Link](https://www.microchip.com/en-us/application-notes/an1095) [Link](https://www.microchip.com/en-us/application-notes/an1157) [Extreme Low Power Mode](https://www.microchip.com/en-us/application-notes/an1267) [Low Power Guide](https://www.microchip.com/en-us/application-notes/an1416) [Audio amping](https://www.microchip.com/en-us/application-notes/an1848-1) [CLC Capabilities](https://www.microchip.com/en-us/application-notes/an2133) [Low Cost Mostor Applications](https://www.microchip.com/en-us/application-notes/tb3152) | 
|Links (URL) to Code Examples|                             ---|                 [Link](https://www.microchip.com/en-us/code-examples?magellan=HA3XCZ3WpVgXyYVTLVgXiVaWJVgXSDF1LVgXClrLDU2HjUaWZZhXiUaWfHhUWT1PDkbTXik1pWfBkUnmOkx1WGo1JmrYHHxLOlJQTRbTukt1Wll9NIgLTREfASJQTRaKAS5aWivHtIfYmkaKASLMTR0G0VtLjUnW2IpE3FaKASLMTRaKAStaGlrTuVgXSYbWpVgXiknTtld9lUaWfZgXiUaWfHhImUaWZZhXiUaWpkdoGllXtlxU2FaKASKgTR)|
|Links (URL) to External Resources|                        ---|                 [Link](https://mu.microchip.com/)|
|Production Unit Cost|                                     ---|                 $3.83|
|Supply Voltage Range|                                     ---|                 1.8V-3.6V|
|Absolute Maximum Current for entire IC|                   ---|                 250mA|
|Maximum GPIO Pin Current (Source/Sink)|                   ---|                 25mA|
| 8-bit or 16-bit Architecture|                            ---|                 16-bit|
|Available IC Packages / Footprints |                      ---|                 4 lead plastic thin quad flat pack (TQFP)  Lead Plastic Quad Flat, No Lead Package (QFN) | 
|Supports External Interrupts? |                           ---|                 Yes|
|In-System Programming Capability and Type|                ---|                 ICSP, Enhanced ICSP| 
|Programming Hardware, Cost, and URL|                      ---|                 [Link](https://www.microchip.com/en-us/tools-resources/debug/programmers-debuggers)|
|Works with MPLAB® X Integrated Development Environment (IDE)?|                             -|                 Yes|
|Works with Microchip Code Configurator?|                  ---|                 Yes|
|Overall Pros|(At least 2)|                 a] is within device operation voltage 1.8-3.6V b] more capability at similar price to other configurations in family c] 16 bit allows for more speed and more capability for potential upgradesd] lots of low power settings|
|Overall Cons|(At least 2)|                 a] not very many packaging types b] Not very many supporting resources |
|Ranking|  1 = first, 2 = second, 3 = third |                 1| 

Final Considerations:
Our team chose the PIC24F16KM204 (PIC 1) as our primary option due to its favorable operating voltage range of 1.8-3.6V, which aligns well with our device's power requirements. This microcontroller offers enhanced capabilities at a competitive price compared to other configurations within its family. The PIC24F16KM104 16-bit architecture provides increased processing speed and scalability for potential future upgrades, making it a good choice for our project. Additionally, the various low power settings available allow us to mitigate most concerns regarding power consumption, which would ensure efficient operation without sacrificing the overall performance of our device. While there are fewer packaging options, specifically a through hole version for testing and supporting resources, the overall advantages in capability, voltage compatibility, and power efficiency made the PIC 1 the best fit for our project's needs.






