category: sensing  
signature: gps.orientation(OrientationType.ROLL, DEGREES)  
description: Reports the angle of the specified orientation axis on a GPS Sensor.  

# GPS Orientation

Reports the angle of the specified orientation axis on a GPS Sensor.

```python
gps.orientation(AXIS, DEGREES)
```

## How To Use

`gps.orientation()` reports a numerical value representing the angle of rotation about the specified orientation `AXIS`:

* The **OrientationType.ROLL** axis reports a value between **-180** to **180** degrees, representing the angle of a GPS Sensor when tilted left or right

* The **OrientationType.PITCH** axis reports a value between **-90** to **90** degrees, representing the angle of a GPS Sensor when tilted forward or backwards

* The **OrientationType.YAW** axis reports a value between **-180** to **180** degrees, representing the angle of a GPS Sensor when rotated about the vertical axis

## Example

```python
# Print the orientation of a GPS Sensor's yaw axis in a loop
while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)
    brain.screen.print("GPS Yaw Orientation: ", gps.orientation(OrientationType.YAW, DEGREES))
    wait(0.1, SECONDS)
```

<advanced>
</advanced>
