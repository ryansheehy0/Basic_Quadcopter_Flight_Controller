# DIY Quadcopter Flight Controller
Raspberry Pi Pico code for a DIY flight controller for a quadcopter.

<!-- Image and video of drone -->
<!-- Image of code diagram -->

## Future features
1. Basic drone
	- Custom PCB with female header pins and male on components.
	- Stabilized flying mode
	- Signal loss then hover and other safty checks
	- FPV Camera with battery voltage displayed

2. Advanced drone
	- Larger battery
	- Advanced stabilized algos
		- Accelerometer Averaging -> Butterworth filter
		- Complimentary filter -> Madgwick filter
	- Switch to thermal camera
	- Waterproof PCB

3. Future featues
	- Switch to much larger 6s batteries
	- Impliment different capabilities.
	- Partial autonomy
		- Right pot selects the object to track with a rectangle around the object.
			- When set to 0 it doesn't show rectangles and doesn't track.
			- When you twist the right pot, it shows all the rectangles and highlights the one that's being currently tracked.
			- You have to wait a little before it starts tracking.
		- Left pot selects at what distance to track the object.
	- Custom device that quickly changes frequencies to get around jamming.
		- Uses mosfets on an antena to change frequency.
	- Drone swarm

## Capabilities
- Cameras: Visible light, IR, Thermal
- Drop a payload
- Speaker and microphone
- Powerful lights
- Lidar for terrain mapping
- Picking up things

## Sources
- [BMI160 Datasheet](https://www.bosch-sensortec.com/products/motion-sensors/imus/bmi160/)
- [Overview video](https://youtu.be/CHSYgLfhwUo?si=-crvyPy1awxu9ZyM)
- [Accelerometer video](https://youtu.be/7VW_XVbtu9k?si=ISFqyUkHYZV7qJ2G)
- [Simple flight controller video](https://youtu.be/4vpgjjYizVU?si=5Lh_3cyaq6MKLBy_)