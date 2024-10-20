

| DESIGN CONSIDERATIONS | PROJECT SPECIFIC REQUIRMENTS | PIC 1 (PIC24FV16KM204-I/PT)            | PIC 2     | PIC 3 | 
|-----------------------|------------------------------|------------------|-----------|-------|
|How many GPIO Pins?|   (4)temp sensor + (4)humidity sensor + (2)esp32 + (4)subsystem debug LED +(7) -motor driver +(3) Programmer = 24 total GPIO PINs |37|          21|      36|
|Built-in Analog to Digital Converter? How many?|none|                 2|          13|      29|
|Built-in Hardware PWM? How many?|1 PWM for motor driver|                 5|          5|      4|
|Built-in I2C? SPI? How many?|3 I2C for temp and humidity sensor, 1 SPI|                2|          2|      2|
|Built-in UART? How many?|1 for esp32 (RX&TX) |                 1|          2|      1|
|Other Required Built-In Features?|none. preferably comes with sleep mode|                 4 low power modes|          x|      x|
|Additional considerations |none|                 x|          x|      x|
|Part Number|                                              ---|                 PIC24F16KM204|          PIC24FJ64GA002-I/SS|      PIC16F18855|
|Link (URL) to product page|                               ---|                 [Link]([URL](https://www.digikey.com/en/products/detail/microchip-technology/pic24fv16km204-i-pt/3872920))|          [LINK](URL)|      [LINK](URL)|
|Links (URL) to Data Sheets|                               ---|                 [FAMILY DATA SHEET](URL)|          [FAMILY DATASHEET](URL)|      [FAMILY DATASHEET](URL)|
|Links (URL) to Application Notes|                         ---|                 [LINK](URL) [LINK](URL) [LINK](URL) [LINK](URL) [LINK](URL) [LINK](URL) [LINK](URL) [LINK](URL) [LINK](URL) | [LINK](URL) [LINK](URL) [LINK](URL) [LINK](URL) [LINK](URL)|      [LINK](URL) [LINK](URL) [LINK](URL)|
|Links (URL) to Code Examples|                             ---|                 [LINK](URL)|          [LINK](URL)|      [LINK](URL)|
|Links (URL) to External Resources|                        ---|                 [LINK](URL)|          [LINK](URL)|      [LINK](URL)|
|Production Unit Cost|                                     ---|                 $3.83|          $3.83|      $1.97|
|Supply Voltage Range|                                     ---|                 1.8V-3.6V|          2.0V - 3.6V|      2.3V - 5.5V|
|Absolute Maximum Current for entire IC|                   ---|                 250mA|          250 mA|      350mA|
|Maximum GPIO Pin Current (Source/Sink)|                   ---|                 25mA|          25mA|      25mA|
| 8-bit or 16-bit Architecture|                            ---|                 16-bit|          16-bit|      8-bit|
|Available IC Packages / Footprints |                      ---|                 4 lead plastic thin quad flat pack (TQFP)  Lead Plastic Quad Flat, No Lead Package (QFN) |          x |      x|
|Supports External Interrupts? |                           ---|                 Yes|          Yes|      Yes|
|In-System Programming Capability and Type|                ---|                 ICSP, Enhanced ICSP|          In-Circuit Serial Programming™ (ICSP™)  Run-Time Self-Programming (RTSP)  Enhanced In-Circuit Serial Programming (Enhanced ICSP)|      ICSP|
|Programming Hardware, Cost, and URL|                      ---|                 [LINK](URL)|          [LINK](URL)|      [LINK](URL)|
|Works with MPLAB® X Integrated Development Environment (IDE)?|                             -|                 Yes|          Yes|      Yes|
|Works with Microchip Code Configurator?|                  ---|                 Yes|          Yes|      Yes|
|Overall Pros|(At least 2)|                 a] is within device operation voltage 1.8-3.6V b] more capability at similar price to other configurations in family c] 16 bit allows for more speed and more capability for potential upgradesd] lots of low power settings|         a]  Is In-system programmable so no need to remove from PCB 2] Low cost and power consumption|      a] Has an ample amount of I/O pins b] Enhanced core features with multiple PWM and EUSART modules for serial communication|
|Overall Cons|(At least 2)|                 a] not very many packaging types b] Not very many supporting resources |          a] Smaller Memory size b] Slower clock speed c] 21 IO pins not enough for our project|      a] Limited processing power b] Limited program memory|
|Ranking|  1 = first, 2 = second, 3 = third |                 1|          3|      2|

Final Considerations:
Our team chose the PIC24F16KM204 (PIC 1) as our primary option due to its favorable operating voltage range of 1.8-3.6V, which aligns well with our device's power requirements. This microcontroller offers enhanced capabilities at a competitive price compared to other configurations within its family. The PIC24F16KM104 16-bit architecture provides increased processing speed and scalability for potential future upgrades, making it a good choice for our project. Additionally, the various low power settings available allow us to mitigate most concerns regarding power consumption, which would ensure efficient operation without sacrificing the overall performance of our device. While there are fewer packaging options, specifically a through hole version for testing and supporting resources, the overall advantages in capability, voltage compatibility, and power efficiency made the PIC 1 the best fit for our project's needs.






