
COMPONENT SELECTION 

Motor (Kyle C)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------|
| ![oops](motor%201.png)SE10G0UTMAF  | Simplistic data sheet. Torque charts show amperage per torque. Speed reaches almost about 11100 min with no load.| Component chassis is small. Shaft too small to operate around. Data sheet missing data such as operating temperature| 
| ![oops](motor2.png) SE8G0NTMCA | Easy to mount (can be placed anywhere on the product). Gives details about how much power the motor can operate. No load speed at 12500 mins| Component chassis is small. Shaft too small to operate around. Data sheet too simplistic, showing only one version of the component and it’s data | 
| ![oops](motor3.png)***F17FA-03MC*** | ***Data sheet includes detailed specs on the fans operation. Requires little power to operate. No need for high voltage. Gives data about the static pressure vs airflow.***| ***Components have pre-made fan/chassis. Limited placement on product. Fan data sheet seems to be too simplistic. No information about reverse direction.***| 

Chosen Component: Option 3

Rational: Though the motor for the product is embedded within a fan and chassis, this meet’s the requirements of what the product wants to do. Though mounting is a bit limited, the specs allow us to operate the motor to the desired speed for its purpose. The only thing needed to test is the directional operation of the fan.



Motor Controller (Kyle C)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------|
| ![oops](driver1.png)***IFX9201SGAUMA1*** |  ***Reliable component (used in previous assignment). Includes over temp shutdown mechanic. Gives Simple understanding of what each pin does. Includes commands for motor operation.***| ***Register commands are complicated to understand without some sort of guidence. Surface mount prongs are small and compact to each other. Requires only certain prongs to be connected to operate properly.***| 
| ![oops](Driver2.png)DRV8876PWPR | Includes a proper chart of pins and what each pin does. Operation conditions are noted and shown for guidance. Includes logic for forward and reverse drive.Most cost effective component out of the 3| Component requires solder paste mounting. Temperature ranges are small for comfort. Pin connection requires further inspection | 
| ![oops](Driver3.png)A3950SLPTR-T | Includes typical application Diagrams. Showcases Load conditions with Oscilloscope images. Includes drive currents and equations for it.***|***Component requires solder paste mounting. Package has a low thermal resistance. Power voltage higher than necessary.| 

Chosen Component: Option 1

Rational: When choosing which component to use, option 1 is the most reasonable choice. The component is well known and used in previous assignments. Included with this component are example diagrams of how to connect the component to both the controller and the motors and what commands are needed for operating the motor.
 

Humidity Sensor (Enrique C)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------|
| ![oops](hum1.png)ENS211-LQFM |This humidity sensor is extremely cheapDoes not require extra considerationsCheapest optionLow response time @ 3 secConsumes less voltage| Surface mount does not have pinsNo extra pins for alerts| 
| ![oops](hum2.png)HIH6030-021-001 | Surface mounting pins No extra considerations requireMiddle priceHas two extra pins for alerts | Consumes more voltage than cheaper oneHas lower accuracy @ +- 4.5%Higher response time @ 6 sec | 
| ![oops](hum3.png)***HIH7130-000-001*** | ***Better accuracy @ +- 3% than the middle priced one Consumes less voltage than HIH6030Surface mount pinsHas two extra pins for alerts*** | ***Most expensive out of the threeHigher response time @ 6 sec***| 

Chosen Component: Option 3

Rational: For the price of less than 3 dollars I choose to purchase the ENS211 to verify if the soldering is achievable. If mounting the ENS211 is difficult I would like to be able to have a back up hence why i also choose the HIH7130. The PCB can be constructed having both the HIH7130 or ENS211 mounting ports. Since both are I2C i believe we can have both in the same PCB.


Temperature Sensor (Rishik A)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------|
| ![oops](tem1.png)TS-3032-C7-QA |Cost-effective. I2C output .Within Voltage Operation Range (3.3V). Digital| Smallest temperature sensing range. More complex calibration is required for higher precision. More expensive than the average temp sensors.| 
| ![oops](tem2.png)***TMP1075DGKR*** | ***Within Voltage Operation Range (3.3V). Greatest Temperature sensing range. Digital. Uses a standard I2C protocol which makes integration with microcontrollers easier.***| ***Temperature readings may become slightly less precise at the extremes of its operational range. Cannot withstand harsh conditions like high humidity, dust or outdoor use.*** | 
| ![oops](tem3.png)P3T1755DPZ | Extremely cost effective. Flexibility with output types (I2C, 2-Wire Serial). Surface mount. Very wide temperature operating range. Within Voltage Operation Range (3.3V). Digital| Very small in size.  Moderate accuracy. Lack of integrated features. Sensitive to power supply fluctuations.|  

Chosen Component: Option 2

Rational: As a requirement our sensors need to communicate with I2C, Option 2 stands out as a better choice compared to Options 1 and 3 due to its balance of high accuracy (±0.5°C), low power consumption, and ease of integration via the I2C interface. It offers a broad temperature range and compact size, making it ideal for battery or solar-powered applications like our micro-greenhouse project. Additionally, it's more cost-effective while providing reliable
performance, making it a practical choice over the more complex and potentially pricier alternatives


Battery (Damien D)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------|
| ![oops](bat1.png)NH22NBP |Meets ideal power requirements. Rechargeable| Not cost effective. Low current production (175mAh). Not Scalable| 
| ![oops](bat2.png)***AA-NIMH-DURACELL*** | ***Rechargeable Scalable Voltage. Common to find in local stores. Very high current capacity ( 2500mAH). Cost effective***| ***Scaling is space intensive. Scaling requires increased complexity*** | 
| ![oops](bat3.png)A1604 BK210J | Meets ideal power requirements. High current capacity (614mAh). Cost effective| Single use. Not Scalable| 

Chosen Component: Option 2

Our team is currently undergoing consideration and possible changes for power. We are considering potentially making our device rechargeable with solar power. So batteries which have this capability would allow us to make a switch if necessary. So while option 3 the A1604, is the most cost effective while in the ideal voltage range, it is eliminated as a potential choice. Leaving just options 1 and 2. Option 1 falls inside our ideal voltage range as well. However our device will have a motor and that motor is going to consume a lot of current, possibly enough to make option 1’s output of 175mAh problematic. Additionally it is the most expensive option. While option 2 is less voltage, it is cost effective enough to use multiple to get to 9V while still being reasonably close to option 1 ($28 vs $20), with the added benefit of way more current capacity, dramatically increasing the battery life. It is with these consideration, our team has chosen option two 

Voltage Regulator (Damien D)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------|
| ![oops](reg1.png)TPS562201DDCR |Cost effective. Can handle high current if necessary (4A). Step down allows for use of higher voltage| Minimum input voltage is on higher end (4.5V)| 
| ![oops](reg2.png)***AZ34063UMTR-G1*** | ***Cost effective ($0.34). Dual step up, step down functionality. Large input voltage range (3V to 35V). Large current output (1.5A)***| ***Increased complexity*** | 
| ![oops](reg3.png)AP3015KTR-G1 | Step down allows for use of lower voltage. Large output voltage range (1.25V-34V)| Very low output current. Not cost effective ($0.54 the most expensive)| 

Chosen Component: Option 2

There is a high chance our device will use a power source which is rated higher than the operating voltage of most of our components so out of the two step down options, option 2 gives us the best cost effectiveness and most flexibility, as the input and output voltage ranges are high while also having a solid current capacity.

Using a step up is a possible route as well which occurs with option 3 and 2. This would allow us to use a lower rated power supply thus potentially making our device simpler and cheaper. However the output current for option 3 is very low at 300mAh which runs the risk of our motor consuming too much of the available current. It is also the most expensive of all the options. 

Considering that option 2 gives us the ability to pursue both the step up and down route with superior specs all for less money, this makes option 2 the best selection for our design

![Power Budget](PlanoDeEnergiaFinal.png)

MICROCONTROLLER



| DESIGN CONSIDERATIONS | PROJECT SPECIFIC REQUIRMENTS | PIC 1 (PIC24FV16KM204-I/PT) ![](PIC24FV16KM204.jpg)           | PIC 2 (PIC24FJ64GA002) ![](PIC24FJ64GA002.jpg)| PIC 3 (PIC16F18855)![](PIC16F18855-M3X-Regular.avif) | 
|-----------------------|---------------------------------------------------|------------------|-----------|-------|
|How many GPIO Pins?|   (4)temp sensor + (4)humidity sensor + (2)esp32 + (4)subsystem debug LED + (7)motor driver +(3) Programmer = 24 total GPIO PINs |37|          21|      36|
|Built-in Analog to Digital Converter? How many?|none|                 2|          13|      29|
|Built-in Hardware PWM? How many?|1 PWM for motor driver|                 5|          5|      4|
|Built-in I2C? SPI? How many?|3 I2C for temp and humidity sensor, 1 SPI|                2|          2|      2|
|Built-in UART? How many?|1 for esp32 (RX&TX) |                 1|          2|      1|
|Other Required Built-In Features?|none. preferably comes with sleep mode|                 4 low power modes|          x|      x|
|Additional considerations |none|                 x|          x|      x|
|Part Number|                                              ---|                 PIC24F16KM204|          PIC24FJ64GA002-I/SS|      PIC16F18855|
|Link (URL) to product page|                               ---|                 [link](https://www.digikey.com/en/products/detail/duracell-industrial-operations-inc/AA-NIMH-DURACELL/16164081) |          [Link](https://www.digikey.com/en/products/detail/microchip-technology/PIC24FJ64GA002-I-SS/1635680)|    [Link](https://www.microchip.com/en-us/product/pic16f18855)  |
|Links (URL) to Data Sheets|                               ---|                 [Link](https://ww1.microchip.com/downloads/aemDocuments/documents/MCU16/ProductDocuments/DataSheets/PIC24FV16KM204-Family-Data-Sheet-DS30003030C.pdf)|   [Link](https://ww1.microchip.com/downloads/en/DeviceDoc/39881e.pdf)       |     [Link](https://ww1.microchip.com/downloads/en/DeviceDoc/400001802D.pdf)|
|Links (URL) to Application Notes|                         ---|                 [Link](https://www.microchip.com/en-us/application-notes/an1044)  [Link](https://www.microchip.com/en-us/application-notes/an1095) [Link](https://www.microchip.com/en-us/application-notes/an1157) [Extreme Low Power Mode](https://www.microchip.com/en-us/application-notes/an1267) [Low Power Guide](https://www.microchip.com/en-us/application-notes/an1416) [Audio amping](https://www.microchip.com/en-us/application-notes/an1848-1) [CLC Capabilities](https://www.microchip.com/en-us/application-notes/an2133) [Low Cost Mostor Applications](https://www.microchip.com/en-us/application-notes/tb3152) | [Encryption Data](https://www.microchip.com/en-us/application-notes/an1044) [Compiler and SPI Module](https://www.microchip.com/en-us/application-notes/an1069) [Compiler and I2C](https://www.microchip.com/en-us/application-notes/an1079) [Interference](https://www.microchip.com/en-us/application-notes/an1096)|     [Link](https://www.microchip.com/en-us/application-notes/an1333) [Link](https://www.microchip.com/en-us/application-notes/an1473) [Link](https://www.microchip.com/en-us/application-notes/an1470)|
|Links (URL) to Code Examples|                             ---|                 [Link](https://www.microchip.com/en-us/code-examples?magellan=HA3XCZ3WpVgXyYVTLVgXiVaWJVgXSDF1LVgXClrLDU2HjUaWZZhXiUaWfHhUWT1PDkbTXik1pWfBkUnmOkx1WGo1JmrYHHxLOlJQTRbTukt1Wll9NIgLTREfASJQTRaKAS5aWivHtIfYmkaKASLMTR0G0VtLjUnW2IpE3FaKASLMTRaKAStaGlrTuVgXSYbWpVgXiknTtld9lUaWfZgXiUaWfHhImUaWZZhXiUaWpkdoGllXtlxU2FaKASKgTR)|         [Link](https://www.microchip.com/en-us/software-library?swsearch=16-bit%20CPU%20Self-test%20Library)|      [Link](https://ww1.microchip.com/downloads/en/Appnotes/90003251A.pdf)|
|Links (URL) to External Resources|                        ---|                 [Link](https://mu.microchip.com/)|          [Link](https://www.microchip.com/en-us/product/PIC24FJ64GA002)|    [Link](https://www.mouser.com/ProductDetail/Microchip-Technology/PIC16F18855-I-SP?qs=BA62vJVifGrE%2Fn9Q%252BW7gXw%3D%3D)  |
|Production Unit Cost|                                     ---|                 $3.83|          $3.83|      $1.97|
|Supply Voltage Range|                                     ---|                 1.8V-3.6V|          2.0V - 3.6V|      2.3V - 5.5V|
|Absolute Maximum Current for entire IC|                   ---|                 250mA|          250 mA|      350mA|
|Maximum GPIO Pin Current (Source/Sink)|                   ---|                 25mA|          25mA|      25mA|
| 8-bit or 16-bit Architecture|                            ---|                 16-bit|          16-bit|      8-bit|
|Available IC Packages / Footprints |                      ---|                 4 lead plastic thin quad flat pack (TQFP)  Lead Plastic Quad Flat, No Lead Package (QFN) |          x |      x|
|Supports External Interrupts? |                           ---|                 Yes|          Yes|      Yes|
|In-System Programming Capability and Type|                ---|                 ICSP, Enhanced ICSP|          In-Circuit Serial Programming™ (ICSP™)  Run-Time Self-Programming (RTSP)  Enhanced In-Circuit Serial Programming (Enhanced ICSP)|      ICSP|
|Programming Hardware, Cost, and URL|                      ---|                 [Link](https://www.microchip.com/en-us/tools-resources/debug/programmers-debuggers)|          [Link](https://www.microchip.com/en-us/tools-resources/debug/programmers-debuggers)|     [Link](https://www.microchip.com/en-us/development-tool/dv244140)|
|Works with MPLAB® X Integrated Development Environment (IDE)?|                             -|                 Yes|          Yes|      Yes|
|Works with Microchip Code Configurator?|                  ---|                 Yes|          Yes|      Yes|
|Overall Pros|(At least 2)|                 a] is within device operation voltage 1.8-3.6V b] more capability at similar price to other configurations in family c] 16 bit allows for more speed and more capability for potential upgradesd] lots of low power settings|         a]  Is In-system programmable so no need to remove from PCB 2] Low cost and power consumption|      a] Has an ample amount of I/O pins b] Enhanced core features with multiple PWM and EUSART modules for serial communication|
|Overall Cons|(At least 2)|                 a] not very many packaging types b] Not very many supporting resources |          a] Smaller Memory size b] Slower clock speed c] 21 IO pins not enough for our project|      a] Limited processing power b] Limited program memory|
|Ranking|  1 = first, 2 = second, 3 = third |                 1|          3|      2|

Final Considerations:
Our team chose the PIC24F16KM204 (PIC 1) as our primary option due to its favorable operating voltage range of 1.8-3.6V, which aligns well with our device's power requirements. This microcontroller offers enhanced capabilities at a competitive price compared to other configurations within its family. The PIC24F16KM104 16-bit architecture provides increased processing speed and scalability for potential future upgrades, making it a good choice for our project. Additionally, the various low power settings available allow us to mitigate most concerns regarding power consumption, which would ensure efficient operation without sacrificing the overall performance of our device. While there are fewer packaging options, specifically a through hole version for testing and supporting resources, the overall advantages in capability, voltage compatibility, and power efficiency made the PIC 1 the best fit for our project's needs.







