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
- `arm_motor.is_done`
- `arm_motor.is_spinning`
- `arm_motor.position_degrees`
- `arm_motor.position_turns`
- `arm_motor.velocity_rpm`
- `arm_motor.velocity_percent`
- `intake_motor.is_done`
- `intake_motor.is_spinning`
- `intake_motor.position_degrees`
- `intake_motor.position_turns`
- `intake_motor.velocity_rpm`
- `intake_motor.velocity_percent`
- `intake_bumper.pressing`
- `front_distance.is_object_detected`
- `front_distance.object_distance_mm`
- `front_distance.object_distance_inches`
- `front_optical.is_near_object`
- `front_optical.color`
- `front_optical.brightness`
- `front_optical.hue`

When adding sensor identifiers to the monitor_sensor() command, they have to be added as strings - therefore enclosed with quotation marks:

```don
monitor_sensor("intake_bumper.pressing")
```
Multiple sensor identifiers, separated by commas, can be added to the monitor_sensor() command:

```don
monitor_sensor(front_distance.object_distance_mm”, “drivetrain.rotation”, “brain.timer.time”)
```

## Example

This code will have the robot spin around and monitor the drivetrain heading and the drivetrain velocity.

```don
def main():
    monitor_sensor("drivetrain.heading", "drivetrain.velocity_percent")
    drivetrain.turn_for(RIGHT, 10, TURNS)
```

<advanced>
</advanced>
