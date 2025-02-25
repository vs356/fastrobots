# Lab 3: Time of Flight Sensors (Due 2/25/2025)

## Prelab
* The default sensor address of both Time of Flight (ToF) sensors is 0x52, but the address is also programmable.
* Since the two sensors cannot be addressed individually, we can change the address programmatically (while powered) or continuously enable/disable the two sensors separately through their shutdown pins. While continuously enabling/disabling the sensors can be timed well to ensure that all obstacles around the robot are detected using the programmable field of view of the sensors, I believe that this approach would be too error-prone to begin with, so I will elect to change the address of one ToF sensor by shutting down one sensor, changing the address of the other sensor, and continuing the program with independent I2C addresses.
* I plan to place the sensors on the front and back of the car, and detect obstacles on the sides by turning the car. I selected a symmetric orientation because I found that the car can flip over and turn in place very quickly and easily: I wanted to select an orientation that would allow the car to continue to obtain reliable readings regardless of the current orientation of the car. 
* Sketch of wiring diagram (with brief explanation if you want)

## Lab Tasks
* Picture of your ToF sensor connected to your QWIIC breakout board

* Screenshot of Artemis scanning for I2C device (and discussion on I2C address)

* Discussion and pictures of sensor data with chosen mode
* 2 ToF sensors and the IMU: Discussion and screenshot/video of sensors working in parallel
* Tof sensor speed: Discussion on speed and limiting factor; include code snippet of how you do this
* Time v Distance: Include graph of data sent over bluetooth (2 sensors)
* Time v Angle: Include graph of data sent over bluetooth
