************
* READ ME  *
************

All code found at https://github.com/WilliamEcoCAR/obd_software



1. obd_recorder.py

this program creates the log items for rmp, speed,
		throttle position, load (wieght), fuel status
								
this is the file executed by the pi to run the remote diagnostic system

it checks to see if there is a connection to the car and 
		then uses the local time to stream the data to the pi

							
							
2. obd_utils.py

this progam scans for different serial ports and allows
						use of Bluetooth or USB devices

the pi can use this to connect to other devices such
					as a monitor or a wireless device



3. obd_sensors.py 

sets up all the sensors that can be read in from the car to the pi

converts the data from the car to hexidecimal so the it can be processed by the pi

stores sensor name, ID, and value
