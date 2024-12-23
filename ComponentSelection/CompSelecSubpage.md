Motor (Kyle C)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------|
| ![oops](motor3.png)***F17FA-03MC*** | ***Data sheet includes detailed specs on the fans operation. Requires little power to operate. No need for high voltage. Gives data about the static pressure vs airflow.***| ***Components have pre-made fan/chassis. Limited placement on product. Fan data sheet seems to be too simplistic. No information about reverse direction.***| 

Chosen Component: Option 3

Rational: Though the motor for the product is embedded within a fan and chassis, this meet’s the requirements of what the product wants to do. Though mounting is a bit limited, the specs allow us to operate the motor to the desired speed for its purpose. The only thing needed to test is the directional operation of the fan.



Motor Controller (Kyle C)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------|
| ![oops](driver1.png)***IFX9201SGAUMA1*** |  ***Reliable component (used in previous assignment). Includes over temp shutdown mechanic. Gives Simple understanding of what each pin does. Includes commands for motor operation.***| ***Register commands are complicated to understand without some sort of guidence. Surface mount prongs are small and compact to each other. Requires only certain prongs to be connected to operate properly.***| 

Chosen Component: Option 1

Rational: When choosing which component to use, option 1 is the most reasonable choice. The component is well known and used in previous assignments. Included with this component are example diagrams of how to connect the component to both the controller and the motors and what commands are needed for operating the motor.
 


Humidity Sensor (Enrique C)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------|
| ![oops](hum3.png)***HIH7130-000-001*** | ***Better accuracy @ +- 3% than the middle priced one Consumes less voltage than HIH6030Surface mount pinsHas two extra pins for alerts*** | ***Most expensive out of the threeHigher response time @ 6 sec***| 

Chosen Component: Option 3

Rational: For the price of less than 3 dollars I choose to purchase the ENS211 to verify if the soldering is achievable. If mounting the ENS211 is difficult I would like to be able to have a back up hence why i also choose the HIH7130. The PCB can be constructed having both the HIH7130 or ENS211 mounting ports. Since both are I2C i believe we can have both in the same PCB.


Temperature Sensor (Rishik A)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------| 
| ![oops](tem2.png)***TMP1075DGKR*** | ***Within Voltage Operation Range (3.3V). Greatest Temperature sensing range. Digital. Uses a standard I2C protocol which makes integration with microcontrollers easier.***| ***Temperature readings may become slightly less precise at the extremes of its operational range. Cannot withstand harsh conditions like high humidity, dust or outdoor use.*** | 
 

Chosen Component: Option 2

Rational: As a requirement our sensors need to communicate with I2C, Option 2 stands out as a better choice compared to Options 1 and 3 due to its balance of high accuracy (±0.5°C), low power consumption, and ease of integration via the I2C interface. It offers a broad temperature range and compact size, making it ideal for battery or solar-powered applications like our micro-greenhouse project. Additionally, it's more cost-effective while providing reliable
performance, making it a practical choice over the more complex and potentially pricier alternatives


Battery (Damien D)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------|
| ![oops](bat2.png)***AA-NIMH-DURACELL*** | ***Rechargeable Scalable Voltage. Common to find in local stores. Very high current capacity ( 2500mAH). Cost effective***| ***Scaling is space intensive. Scaling requires increased complexity*** | 

Chosen Component: Option 2

Our team is currently undergoing consideration and possible changes for power. We are considering potentially making our device rechargeable with solar power. So batteries which have this capability would allow us to make a switch if necessary. So while option 3 the A1604, is the most cost effective while in the ideal voltage range, it is eliminated as a potential choice. Leaving just options 1 and 2. Option 1 falls inside our ideal voltage range as well. However our device will have a motor and that motor is going to consume a lot of current, possibly enough to make option 1’s output of 175mAh problematic. Additionally it is the most expensive option. While option 2 is less voltage, it is cost effective enough to use multiple to get to 9V while still being reasonably close to option 1 ($28 vs $20), with the added benefit of way more current capacity, dramatically increasing the battery life. It is with these consideration, our team has chosen option two 


Voltage Regulator (Damien D)

| Component | Pro's | Cons |
|------|----------------------------|-----------------------------|
| ![oops](reg2.png)***AZ34063UMTR-G1*** | ***Cost effective ($0.34). Dual step up, step down functionality. Large input voltage range (3V to 35V). Large current output (1.5A)***| ***Increased complexity*** | 
 

Chosen Component: Option 2

There is a high chance our device will use a power source which is rated higher than the operating voltage of most of our components so out of the two step down options, option 2 gives us the best cost effectiveness and most flexibility, as the input and output voltage ranges are high while also having a solid current capacity.

Using a step up is a possible route as well which occurs with option 3 and 2. This would allow us to use a lower rated power supply thus potentially making our device simpler and cheaper. However the output current for option 3 is very low at 300mAh which runs the risk of our motor consuming too much of the available current. It is also the most expensive of all the options. 

Considering that option 2 gives us the ability to pursue both the step up and down route with superior specs all for less money, this makes option 2 the best selection for our design


![Power Budget](PlanoDeEnergiaFinal.png)


Located above is our final calculated Power Budget. To begin we first calculated, what the maximum current on our line would be to get an idea of the capacity for our design. This number was calculated to be 1.5A. Hitting such a maximum however was not necessary as our device is quite non energy demanding, topping out at only 720mA when considering a 25% safety margin. 

Lastly was battery life. Running at full capacity, our device is expected to last around three and a half hours. Which our team found was quite fast. This is mainly due to 2 components, the Microcontroller (250mA) and the ESP32(240mA), which combined consume over 3/4 of the device current. Our team found various solutions to explore for this issue. First, our microcontroller comes with 4 low power settings availible for us to use. However the exact specificications of savings are unknown and not provided by our controller provider. Testing will have to be done to see which setting produces the maximum power savings. Additionally, our team has decided to sense in cycles. This allows the device to not be on all the time leading to more savings. Testing will have to be done to see how much savings can be gained from this solution

