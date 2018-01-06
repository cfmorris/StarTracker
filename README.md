# StarTracker 

StarTracker is student project intended to generate altitude and azimuth data of any celestial body and use that data to accurately update the orientation of a directional antenna in real time.

A Raspberry Pi 3 will be used to calculate the data, drive stepper motors, collect raw data, and serve that data one a webserver wirelessly accessable to remote users.  If this proves to be to much for the Pi's processor to handle, the alt-az data may lag behind the position of the celestial body.  In such a case an ESP-32 or ESP-8266 will be used to read orientation data from the webserver and appropriately appropriately controll the stepper motors.

# Required Non-standard Python 3 Libraries
StarTracker requires modules which are not included in the python3 Standard library.  To get these modules try entering the following in the command line:

  "sudo apt-get install python3-pip python3-astropy" and "sudo pip3 install astropy jplephem"
