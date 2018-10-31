## Week 9 - [PCB Creation](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Obstruction%20Sensor%20PCB%20Sketch.fzz)
Gerber file has been sent to prototypelab@humber.ca

### Status Report
Financial Status: Budget has been surpassed.  
Schedule: The project is on track.  
Programming has already been started, trying to figure out how to change the I2C address of the VL53L0X to 24 (default 29) using software.  

![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Obstruction%20Sensor%20PCB%20Sketch_pcb.png?raw=true)  

UPDATE:
i2c address table:  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/i2cNEW.jpg?raw=true)  

Connection has been changed  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/circuit.jpg?raw=true)  

New Display purchased (SSD1306)  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/ssd1306.jpg?raw=true)

## Week 8 - Breadboard

### Resolution
I dropped by Humber's prototype lab to seek help.
The device was still not being detected by their platform.
It doesn't help that we couldn't find the datasheet for the specific board I had, as the device has different setups depending on how the board was laid out.
After troubleshooting and tracing the board, they hinted that one of the pins on the sensor attached to the board had a tiny smudge of solder that connected it to another pin on the sensor.
I am proud to announce that the pins I soldered were not contributing to the issue.
Nonetheless, I will not rule myself out in possibly causing this issue because even though the shorted pins were on the opposite side of the pins I soldered, it is still possible that I have splashed a tiny amount of solder on the opposite side (be very careful on soldering).
After removing they smudge, being as careful as possible as the sensor is very small, the device was now being detected.
Below is the screenshot of the default address it has (0x29).
I still have to change it to 0x24, which will require me more time as it will be changed thru software, rather than hardware.
I am just glad that I did not need to buy another sensor as the shipping fee on Adafruit is expensive.
Shout-outs to Vlad and Kelly as they really saved me here.  
![Alt_text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/defaultAddress.jpg?raw=true)


### Issue
The wiring is correct as I tested other's sensors with i2cdetect -y 1, and their devices showed up.
Mine does not show up, I already checked the soldering with the microscope and do not see any issues.
I also checked the voltage on the multimeter and oscilloscope, based on my research, the voltage should spike when using the i2cdetect command.
It is having a constant voltage, which for me, suggests that the board is defective.
I will go and ask help from Kelly and Vlad tomorrow as the lab is closed for today.
If the issue persists after tomorrow, I will purchase a new sensor from Adafruit, a company well trusted.  
![Alt text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/boardConnect.jpg?raw=true)  
![Alt text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/piConnect.jpg?raw=true)  
![Alt text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/wholeConnect.jpg?raw=true)

## Week 7 - Purchased Parts
![Alt text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/Display.jpg?raw=true)  
![Alt text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/Wires.jpg?raw=true)  
![Alt text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/ToF.jpg?raw=true)

## Week 6 - Holiday

## Week 5 -[Submitted Purchases](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases.docx)  
![Alt text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/4-Digit%207-Segment%20Display.png?raw=true)  
![Alt text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/Cables.png?raw=true)  
![Alt text](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Purchases/ToF.png?raw=true)

## Week 4 - [Submitted Budget](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Budget.xlsx)

## Week 3 - [Submitted Project Schedule](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Project%20Schedule.mpp)

## Week 2 - [Submitted Project Proposal](https://github.com/AldousMendoza/ObstructionSensor/blob/master/ProjectDocumentation/Project%20Proposal.xlsx)

## Week 1 - Debriefing
