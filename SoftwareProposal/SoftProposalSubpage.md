# Software Implementation
Our team's software offers a streamlined solution for users to monitor and control temperature based on their input for both temperature and humidity. The following sections provide detailed explanations of the code blocks, outlining their functionality and the logic behind each operation. 
## Main Loop
Below is the final diagram illustrating how our code interacts with the PCB. Each section of the diagram, outlined in bold font, represents a distinct block providing more details about its specific functionality.

Due to time constraints and issues with the PCB not functioning properly, we had to remove the debugging and low-power features from the final diagram. These features could not be implemented within the available timeframe.

The original design included a debugging block (located at the bottom of the diagram) to verify communication between the sensors, the H-bridge, and the MCU. Additionally, a low-power design was planned but could not be implemented due to challenges in understanding how to code it with our PCB setup.

![](FinalMain.drawio.png)

## System Initialization Block
This block ensures the initialization of all peripherals used in the code, including UART, SPI, I2C, the system clock, and pins. It also verifies that all necessary header files are included in the main code.

![](systeminit.png)

## Sensor Read Block
This block activates either SPI or I2C to retrieve data from the temperature and humidity sensors via their respective peripherals. The data is then returned to the main code to determine whether the motor should be turned on or off.

![](read.PNG)

## Motor Block
This block evaluates the temperature data to decide whether the motor should be activated or deactivated, ensuring it operates within the specified range.

![](motor.png)

## Original Diagram & Version 2.0
This is the original diagram we planned to implement, but changes were necessary due to time constraints and issues with our PCB. If we had not encountered issues with our PCB, we would have liked to include the debugging and low-power features to make our product more user-friendly and power-efficient.

For the low-power feature, the goal was to have the product activate only when pinged by either the temperature or humidity sensor. The respective datasheets included sections on low-power modes, but I was unable to fully understand how to implement these features in our code. Ideally, the temperature sensor would activate only when the temperature exceeded a set threshold, while the humidity sensor would ping the MCU if humidity dropped below 30% or exceeded 40%. If the temperature rose above 25°C, the MCU would turn on the motor to reduce heat and bring in fresh air from outside the greenhouse.

This approach was intended to maximize power efficiency by minimizing unnecessary operations, which is critical since the product relies on batteries. The goal was to extend battery life as much as possible.

The debugging feature, on the other hand, would allow customers to easily verify that everything was functioning correctly without needing much—if any—technical knowledge about how the sensors or motor communicate with the MCU. I believe this feature would have been a key selling point, as it simplifies setup and ensures the product works as expected before installation in the greenhouse.  

![](mainloop.png)

## Debugging Block
The debugging block was designed to use a single button to verify communication between the sensors and the MCU. It would change the state of a multi-color LED to indicate the status of each peripheral being checked. For example, if the temperature sensor was functioning correctly, the LED would turn blue. If the sensor was not working, the LED would turn red to signal an issue. This process was planned for all components communicating with the MCU, except for the ESP32. Each component would have a designated color, with red universally indicating a communication failure.

![](debug.PNG)
