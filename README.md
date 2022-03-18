# dog_gun

## Rpi setup 
### enable i2c by following this guide:  
https://learn.adafruit.com/adafruits-raspberry-pi-lesson-4-gpio-setup/configuring-i2c  
### enter commands below
`sudo apt-get install python-smbus`  
`sudo apt-get install i2c-tools`  
`sudo i2cdetect -y 1` to check if it works  

### Install servokit library by following this guide:  
https://learn.adafruit.com/adafruit-16-channel-servo-driver-with-raspberry-pi/using-the-adafruit-library  
#### or enter commands below:
`sudo pip3 install adafruit-circuitpython-servokit`

## python script
`from adafruit_servokit import ServoKit`  
`kit = ServoKit(channels=16)`  
`kit.servo[0].angle = 180`

## install opencv
follow this link:  
https://forums.raspberrypi.com/viewtopic.php?t=307157  
you may need to upgrade numpy
`pip install numpy --upgrade`


