# Libraries
This repository have all the main [Otto DIY robot](https://www.ottodiy.com/)) libraries for Arduino IDE for all Arduino compatible boards

## Installation:
How to install the Arduino IDE and libraries?
There are multiple ways to include these libraries to your Arduino, the easiest way is:
1. [Download the .zip Otto libraries here](https://github.com/OttoDIY/OttoDIYLib/archive/master.zip)
2. Open Arduino IDE and navigate to Sketch > Include Library > Add .ZIP Library. At the top of the drop down list, select the option to "Add .ZIP Library''.
3. You will be prompted to select the library. Navigate to the .zip file's location, that you just downloaded and open it.
4. In the main window you will see in the bottom back area a message that it has been installed. 
5. To verify they are properly installed, go to Sketch > Include Library menu. You should now see the library at the bottom of the drop-down menu. That means is ready to use Otto example codes! you can find them in File > Examples > OttoDIYLib
[for more details or other way to install libraries visit this link](https://www.arduino.cc/en/Guide/Libraries) 
 
## Compatibility:

Multiple dependant Otto Libraries are included:

Robot  | Library can use
------------- | -------------
DIY  | Otto9
PLUS | Otto9
Eyes* | Otto9 
Humanoid  | Otto9Humanoid
Wheels  | Servo

*For Eyes you will need to install [Adafruit_LEDBackpack](https://github.com/adafruit/Adafruit_LED_Backpack) and [Adafruit_GFX](https://github.com/adafruit/Adafruit-GFX-Library)

* Otto contains all the main functions
* Otto_gestures contains all the gestures functions
* Otto_mouth 	contains all the mouth functions
* Otto_sound contains all the sound functions
* Otto_Matrix contains all the matrix functions
* US contains the functions of the ultrasonic sesnor
* SerialCommand is for Bluetooth communication
* Oscillator is the main algorithm for the servos smooth movement
 
## Wiring:
We follow these connections in all our robots, but some Otto remixes do not use all pins or interchange them according to their needs, you can do that too, so you can play with the pins to add new sensors, more motors, displays, LEDs and so on.


Servos| Pin
------------- | -------------
Left Leg or Left Wheel |  2 
Right  Leg or Right Wheel |  3
Left Foot | 4 
Right Foot |  5 
Left arm for Humanoid  |  6 
Right arm for Humanoid |  7 

Ultrasonic | Pin
------------- | -------------
Trigger | 8 
Echo | 9  

Bluetooth | Pin
------------- | -------------
STATE |  10  not required
TX | 11
RX | 12  
ENABLE |  not required

Buzzer | Pin
------------- | -------------
Positive | 13 
 
Touch sensor or Button | Pin
------------- | -------------
OUT | A0 

LED MATRIX 8x8 for the Mouth (MAX7219) | Pin
------------- | -------------
CLK Clock | A1 
CS Chip Select | A2  
DIN Data In | A3 

LED MATRIX 16x8 for the Eyes (i2C*)| Pin
------------- | -------------
SDA Synchronous Data | A4   
SCL Synchronous Clock | A5   

*More i2C devices like OLED or Gyro can be added in parallel by using different address

Sound sesnor | Pin
------------- | -------------
OUT | A6 


 ## How to Contribute:
Contributing to this software is warmly welcomed. There are 3 ways you can contribute to this project:
1. Test and if find a problem then post an issue.
2. Helps us solve the issues or other bugs.
3. Improve and optimize the curren libraries.
You can do this [basically by forking](https://help.github.com/en/articles/fork-a-repo), committing modifications and then [pulling requests](https://help.github.com/en/articles/about-pull-requests). 

Please add a change log and your contact into file header.

Thanks for your contribution and Welcome to the [Otto DIY community](http://builders.ottodiy.com/)