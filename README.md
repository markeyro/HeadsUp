# HeadsUp
Microcontroller project for the nerdy paramotor pilot

**Goal:**
This project is devoted to bringing to the forefront those key pieces of data that most paramotor pilots might want to have in view at any given time. 

**Vision:**
  Chassis mounted 3D Printed Enclosure to contain:
    - Microcontroller (Feather M4 Express SAMD51 based chipset as of 9/21/21)
    - LiPo Battery capable of minimal 2hr of flight time
    - Sensor Interfaces
      - GPS (ultimate gps featherwing, adafruit)
      - BME280 (temp,barometer/altitude,humidity)
      - Thermocouple (type K, w/ amp, for cylinder head temp)
      - Analog pins for Hall Sensor (rpm) and capacitance sensor (fuel level)
  External OLED Display on GoPro helmet mount to display data
    - 128x128 OLED, over i2C, 4 wire
    - Plug into chassis unit once harnessed in
  Looping Program to query all sensors for data, and print on a 1x/second refresh
  
**Timeline:**
  2019: Idea and some brainstorming
  2020: More of the same but lots of idle nothing time
  2021:
    June 15: Beginning to research and conceptualize in more detail
    July 15: Begin to acquire components and organize thoughts
    August 15: Begin to assemble hardware and test code for sensors
    September 15: Most hardware acquired; Testing individual sensors and output variables; Each sensor able to output data successfully; 
    September 20: Decision to move up to M4 Cortext Feather for increased storage and RAM
    September 20: Testing combing of sensors in master code.py file ; multiple issues / conflicts; need some assistance from discord.
    September 21:
    
**Hardware:**
  Microcontroller
    M4 Express Feather        $23
  Featherwings/Modules
    Ultimate GPS Featherwing  $22
    Sparkfun i2C Feather      $7
    BME280                    $11
    128x128 GS OLED           $22
    Thermocouple Amp          $12
    Thermocouple              $10
    Hall Sensors              $13
    Misc Supplies             $30

**Code Structure:**
  Main File
    Code.py - main file (obviously) which will contain it all at the end
  Supporting Files
    GPS.py
    BME.py
    OLED.py
    FUEL.py
    Hall.py
    Thermocouple.py
 
 **Issues:**
  09/21/21
    When combining code into 1 file seems to be getting conflicts and memory errors. could be lots of things. will be simplifying and building code stepwise to see what i'm breaking as i go.
    
