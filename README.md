# arduino-python
How to use arduino and python together.

# Setting up Arduino in python

Import serial
import time

# Connect arduino to serial port

arduino = serial.Serial("/dev/ttyUSB0", 9600)
time.sleep(2) #wait until the connection stabilizes

#Sending command 
