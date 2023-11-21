category: looks  
signature: monitor_sensor()
description: The monitor_sensor function is used to add sensors to the monitor console.

# Monitor Sensor

The `monitor_sensor()` command is used to add sensors to the monitor console so that the sensor values can monitored. 

```don
monitor_sensor("sensor_name", "another_sensor_name", ...)
```

## How To Use

To monitor sensor values in the monitor console, use the `monitor_sensor()` function by adding the identifiers of the sensors as string parameters. This function should be called at the start of the program.

Below is the list of supported sensor identifiers:

- `brain.timer.time`
- `drivetrain.is_done`
- `drivetrain.is_moving`
- `drivetrain.heading`
- `drivetrain.rotation`
- `drivetrain.velocity_rpm`
- `drivetrain.velocity_percent`
- `intake_motor_group.is_done`
- `intake_motor_group.is_spinning`
- `intake_motor_group.position_degrees`
- `intake_motor_group.position_turns`
- `intake_motor_group.velocity_rpm`
- `intake_motor_group.velocity_percent`
- `bottom_distance.is_object_detected`
- `bottom_distance.object_distance_mm`
- `bottom_distance.object_distance_inches`
- `bottom_line_tracker.reflectivity`
- `middle_line_tracker.reflectivity`
- `top_line_tracker.reflectivity`
- `roller_optical.is_near_object`
- `roller_optical.color`
- `roller_optical.brightness`
- `roller_optical.hue`
- `gps.position_mm`
- `gps.position_inches`
- `gps.heading`

When adding sensor identifiers to the monitor_sensor() command, they have to be added as strings - therefore enclosed with quotation marks:

```don
monitor_sensor("bottom_line_tracker.reflectivity")
```
Multiple sensor identifiers, separated by commas, can be added to the monitor_sensor() command:

```don
monitor_sensor(“distance.object_distance_mm”, “drivetrain.rotation”, “brain.timer.time”)
```

## Example

This project uses the gps position sensor identifier to show both the X and the Y position (in mm and inches) of the robot as it drives toward the vertical center of the field. It also uses the timer sensor identifier to show the time in seconds. These sensor identifiers are passed into the motor_sensor() command.

- Starting Position: A
- Orientation: Facing Red Alliance Mobile Goal
- Preload: Zero Rings

```don
def main():
    monitor_sensor("brain.timer.time", "gps.position_mm", "gps.position_inches")
    drivetrain.drive(FORWARD)
    while gps.x_position(MM) < 0:
        wait(5, MSEC)
    drivetrain.stop()
    drivetrain.turn_for(RIGHT, 90, DEGREES)

main()
```

<advanced>
</advanced>
