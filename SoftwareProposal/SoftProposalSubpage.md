# Software Implementation
Our team's software offers a streamlined solution for users to monitor and control temperature based on their input for both temperature and humidity. The following sections provide detailed explanations of the code blocks, outlining their functionality and the logic behind each operation. 
## Main Loop
Below is the final diagram illustrating how our code interacts with the PCB. Each section of the diagram, outlined in bold font, represents a distinct block providing more details about its specific functionality.

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

## Debugging Block
![](debug.PNG)
