# How to send a command to arduino with python.

# Setting up Arduino in python

Import serial
import time

# Connect arduino to serial port

arduino = serial.Serial('/dev/ttyUSB0', 9600)
time.sleep(2) #wait until the connection stabilizes

#Sending command to turn on the led

arduino.write(b'1')
print("led on")

arduino.write(b'0')
print("led off")

arduino.close()
