# Obstruction Sensor

This is my first attempt in making a device using the raspberry pi.  
This project mainly presents the VL53L0X.  

A bit of an introduction on how the VL53L0X works:  
The VL53L0X emmits a laser towards a direction.
It then calculates for the distance based on how long the laser bounces back.

## Build Instructions

### System Diagram
The VL53L0X continously reads data(distance) while the SSD1306 continously displays that data.
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/UML.JPG?raw=true)  

### [Budget and Parts](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Budget.xlsx)
You will be needing the following parts in order to create the obstruction sensor:  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/Budget.JPG?raw=true)  
NOTE: The Socket Pin Headers are optional, depends if you will be building the PCB or not.  

### Assembly
Raspberry Pi 2 Pin Layout  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/rp2_pinout.png?raw=true)  

VL53L0X Pin Layout  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/VL53L0Xonline.jpg?raw=true)  

SSD1306 Pin Layout  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/SSD1306online.jpg?raw=true)  

1. Connect the VL53L0X and SSD1306's VCC pin to the Raspberry Pi's 3v3 pin.  
2. Connect the  VL53L0X and SSD1306's GND pin to any of the Raspberry Pi's GND pin.  
3. Connect the VL53L0X and SSD1306's SDA pin to the Raspberry Pi's SDA pin.  
4. Connect the VL53L0X and SSD1306's SLA pin to the Raspberry Pi's SLA pin.  

Your assembly should look similar to this:  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/circuit.jpg?raw=true)  

### [PCB](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Obstruction%20Sensor%20PCB%20Sketch.fzz)
This is entirely optional, you do not need this for the device to work.  
For the PCB, you will need the program, Fritzing.  
This is how the PCB will look like this:  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Obstruction%20Sensor%20PCB%20Sketch_pcb.png?raw=true)  

### [Enclosure](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Pi2CaseX6%20-%20Obstruction%20Sensor.cdr)
This is also optional.  
For the enclosure, we will be using a laser cutter along with the program, CorelDRAW.  
This is how the Enclosure will be:  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/Enclosure%20SS.jpg?raw=true)  

And this is how it looks after assembly:  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/Enclosure.jpg?raw=true)  

### Software and Setup

1. Clone and follow the instructions for [VL53L0X](https://github.com/adafruit/Adafruit_CircuitPython_VL53L0X) from [Adafruit](https://github.com/adafruit), credits to them.  
2. Clone and follow the instructions for [SSD1306](https://github.com/adafruit/Adafruit_CircuitPython_SSD1306) from [Adafruit](https://github.com/adafruit), credits to them.  
3. Download all the files in this [folder](https://github.com/AldousMendoza/ObstructionSensor/tree/master/ProjectDocumentation/O-Sensor) to your raspberry pi  

The actual code to run it is the text.py located inside the folder.  
Run it using "Python3 test.py".

### [Schedule](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Project%20Schedule.mpp)
Having all the parts, and excluding PCB and Enclosure creation times, the project can be made in less than a day.  
