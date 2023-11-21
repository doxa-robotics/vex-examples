category: sensing  
signature: gps.heading()  
description: Reports the heading that a robot is currently facing based on a GPS Sensor's readings from the VEX GPS Field Code.  

# GPS Heading

Reports the heading that a robot is currently facing based on a GPS Sensor's readings from the VEX GPS Field Code.

```python
gps.heading()
```

## How To Use

The `gps.heading()` command reports a range of heading values from **0.00** to **359.99** degrees, increasing in value when a GPS Sensor is rotated clockwise.

By default, a GPS Sensor should be mounted facing behind a robot. Then, for example, if the GPS Sensor is facing the South wall as defined by the VEX GPS Field Code, the reported heading will be **0.00** degrees, which is the heading that the front of the robot is facing.


## Example

The example below uses the `gps.heading()` command to stop the Drivetrain's turn when the reported GPS Sensor heading is more than or equal to 180 degrees.

```python
drivetrain.set_turn_velocity(25, PERCENT)
drivetrain.turn(RIGHT)

while gps.heading() < 180:
    wait(5, MSEC)

drivetrain.stop()
```

<advanced>
</advanced>
