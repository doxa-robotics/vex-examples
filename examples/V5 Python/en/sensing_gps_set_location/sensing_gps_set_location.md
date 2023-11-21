category: sensing  
signature: gps.set_location()  
description: Sets the location for a GPS Sensor to a defined positional value.  

# GPS Set Location

Sets the location for a GPS Sensor to a defined positional value.

```python
gps.set_location(x, y, units, heading, DEGREES)
```

## How To Use

When a GPS Sensor is too close to the field walls to read accurate data (for example, when a robot is in a game's starting position on a field), unexpected behaviors can often occur if the program relies on the GPS's positional and heading data to work correctly.

The `gps.set_location()` command can be used to set the location and heading of a GPS Sensor if this information is known before the program is ran, which may help reduce GPS data inaccuracies due to a GPS Sensor's proximity to the field walls when a program is started.

The **x** and **y** parameters are the X and Y offsets of the GPS Sensor, or a defined origin point on a robot relative to the center of a field. The **units** parameter can either be **MM** or **INCHES**.

The **heading** parameter is the heading of the robot in its defined position. For example, if the GPS Sensor is mounted facing behind a robot and the robot is facing the West wall (heading of 270), the **heading** value that should be passed is 270.

```python
# Setting the approximate location of a GPS Sensor
# when a robot is facing West and
# starting at the bottom right corner of a field
gps.set_location(56, -45, INCHES, 270, DEGREES)
```

<advanced>
</advanced>
