# Spider-Robot-Arduino-Uno-
### Description: For the purpose of providing extra files and clarification for the original Quad Spider Robot instructable (http://www.instructables.com/id/DIY-Spider-RobotQuad-robot-Quadruped/)

Hello wandering maker! As you may have found, there are some things that are missing, information wise, from the spider robot instructions. This repository is meant for people who are like how I was when I started this project and are confused about particular things, such as how to arrange the wires for breadboarding, how to use an Ardunio Uno instead of a Pro Mini, and how to configure the hardware for bluetooth usage.

Below is a breakdown of what each file is used for and how it will help in your construction of the spider robot:

1) CH341SER_MAC.ZIP
This driver download was useful when I encoutered this error when uploading the bluetooth code to the Arduino: "avrdude: ser_open(): can't open device "/dev/cu.mydev": Resource busy". If you encounter this, you can download this driver onto your Mac. If you are working on something other than a Mac, you can find its driver here by scrolling down under "Related information": http://www.wch.cn/download/CH341SER_MAC_ZIP.html
If you need more context about my issue, you can refer to this forum: https://arduino.stackexchange.com/questions/37981/osx-upload-error-avrdude-ser-open-cant-open-device-dev-cu-mydev-resou

2) Serial Command.zip
This is one of the libraries needed for the Arduino code.

3) Spider_no_bluetooth.fzz
This is a Fritzing to show what is needed, placement of servos, breadboard layout, etc.

4) Spider_with_bluetooth.fzz
This is a Fritzing to show what is needed, placement of servos, breadboard layout, etc. for use with a bluetooth module.

5) flexitimer2-master.zip
Another library needed for the Arduino code.

6) 

### Additional Links:

Bluetooth to Ardunio configuration guide: http://42bots.com/tutorials/hc-06-bluetooth-module-datasheet-and-configuration-with-arduino/

Bluetooth to Andriod configuation guide: http://42bots.com/tutorials/how-to-connect-arduino-uno-to-android-phone-via-bluetooth/
