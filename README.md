# Spider Robot: Arduino Uno
### Description: For the purpose of providing extra files and clarification for the original Quad Spider Robot Instructable (http://www.instructables.com/id/DIY-Spider-RobotQuad-robot-Quadruped/)

Hello wandering maker! As you may have found, there are some things that are missing, information wise, from the spider robot instructions. This repository is meant for people who are like how I was when I started this project and are confused about particular things, such as how to arrange the wires for breadboarding, how to use an Arduino Uno instead of a Pro Mini, and how to configure the hardware for bluetooth usage.

Below is a breakdown of what each file is used for and how it will help in your construction of the spider robot:

1) Media folder

   This folder includes images that may be helpful to you as you build the robot. Images in the folder include images of the Fritzings [with](../master/Media/Spider_with_bluetooth_fritzing.jpg) and [without](../master/Media/Spider_no_bluetooth_fritzing.jpg) bluetooth,  [the robot without Arduino connected](../master/Media/SpiderRobot-base-constructed.jpg), [robot with everything connected d](../master/Media/SpiderRobot-connected-arduino.jpg), the [control panel for the robot once bluetooth is enabled](../master/Media/Bluetooth_Control_Screen_SR.png), and the [setup for just the LED](../master/Media/SpiderRobotLED-setup.jpg) to ensure that power is safely being fed to the Arduino.

2) [CH341SER_MAC.ZIP](../master/CH341SER_MAC.ZIP)

   This driver download was useful when I encountered this error when uploading the bluetooth code to the Arduino: "avrdude: ser_open(): can't open device "/dev/cu.mydev": Resource busy". If you encounter this, you can download this driver onto your Mac. If you are working on something other than a Mac, you can find its driver here by scrolling down under "Related information": http://www.wch.cn/download/CH341SER_MAC_ZIP.html. If you need more context about my issue, you can refer to this forum: https://arduino.stackexchange.com/questions/37981/osx-upload-error-avrdude-ser-open-cant-open-device-dev-cu-mydev-resou

3) [Fixing_avrdude:stk500_getsync_error.png](../master/Fixing_avrdude:stk500_getsync_error.png)

   I kept having an error with the Arduino not uploading the code. If this happens to you, try downloading the driver above and/or following this tip I found on a forum online. If you would like to read the whole thread where I found the screenshot, you can find the forum at this link: https://forum.arduino.cc/index.php?topic=28223.30

4) [Serial_Command.zip](../master/Serial_Command.zip)

   This is one of the libraries needed for the Arduino code.

5) [Spider_no_bluetooth.fzz](../master/Spider_no_bluetooth.fzz)

   This is a Fritzing to show what is needed, placement of servos, breadboard layout, etc.

   ![alt text](https://github.com/angelicaortiz909/Spider-Robot-Arduino-Uno/blob/master/Media/Spider_no_bluetooth_fritzing.jpg "Spider Robot Fritzing without Bluetooth")


6) [Spider_with_bluetooth.fzz](../master/Spider_with_bluetooth.fzz)

   This is a Fritzing to show what is needed, placement of servos, breadboard layout, etc. for use with a bluetooth module.

   ![alt text](https://github.com/angelicaortiz909/Spider-Robot-Arduino-Uno/blob/master/Media/Spider_with_bluetooth_fritzing.jpg "Spider Robot Fritzing with Bluetooth")


7) [flexitimer2-master.zip](../master/flexitimer2-master.zip)

   Another library needed for the Arduino code.

8) [quad-spider-moving.ino](../master/quad-spider-moving.ino)

   This is the Arduino code for the spider robot *without* any bluetooth capabilities. The functions of the robot continually loop.

9) [spider-bluetooth.ino](../master/spider-bluetooth.ino)

   This is the Arduino code for the spider robot *with* bluetooth capabilities. The functions of the robot can be controlled by downloading Bluetooth SPP Tools Pro or equivalent program onto your Android device. To learn more about adapting bluetooth capabilities, refer to the original spider robot bluetooth instructions (http://www.instructables.com/id/DIY-Spider-Robot-PART-II-Remote-control/) and the links below for further assistance.


### Additional Links:

Bluetooth to Arduino configuration guide: http://42bots.com/tutorials/hc-06-bluetooth-module-datasheet-and-configuration-with-arduino/


Bluetooth to Android configuration guide: http://42bots.com/tutorials/how-to-connect-arduino-uno-to-android-phone-via-bluetooth/


Spider Robot in Action:
https://youtu.be/Vyh3SaYLo_0?list=PLuz-GQZtyIjUuq_W8g9vByreekWgkh9nj


### Credits:

Credit goes out to [Regis Hsu](https://github.com/regishsu) for creating the original Instructable, as well as [Donnie Plumly](https://github.com/dplumly) and [Rob Edwards](https://github.com/robertcedwards) for guiding me through the process of making this robot a reality.
