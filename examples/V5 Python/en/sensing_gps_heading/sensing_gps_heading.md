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

Usually, a GPS Sensor should be mounted facing behind a robot. In the GPS configuration, the Angle Offset is set to **180** degrees.

Then, for example, if the GPS Sensor is facing the South wall as defined by the VEX GPS Field Code, the reported heading will be **0.00** degrees, which is the heading that the front of the robot is facing.

However, a GPS Sensor can also be mounted facing other directions (e.g. the front of a robot).

In this situation, for example, the GPS Sensor's Angle Offset configuration would then need to be set to **0** degrees, which is the angular difference between the forward heading of the robot, and the heading that the GPS is facing. This way, the reported heading value will shift correctly in line with a robot's headings as it turns.

## Example

The example below uses the `gps.heading()` command to stop the Drivetrain's turn when the reported GPS Sensor heading is more than or equal to 180 degrees.

```python
drivetrain.turn(RIGHT)

while gps.heading() < 180:
    wait(50, MSEC)

drivetrain.stop()
```

<advanced>
</advanced>
