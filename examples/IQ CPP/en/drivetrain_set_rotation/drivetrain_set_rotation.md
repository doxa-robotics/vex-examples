category: drive  
signature: Drivetrain.setRotation(90, degrees);  
device_class: smartdrive  
description: Sets the Drivetrain's angle of rotation when configured with a VEX IQ Gyro or Brain Inertial Sensor.    

# Set Rotation

Sets the Drivetrain's angle of rotation when configured with a VEX IQ Gyro or Brain Inertial Sensor.

```cpp
Drivetrain.setRotation(rotation, degrees);
```
## How To Use

### IQ (1st generation) Brain

The `Drivetrain.setRotation` command can be used to set the Drivetrain's angle of rotation to any given positive or negative value.

### IQ (2nd generation) Brain

`Drivetrain.setRotation` can also be used to set the Drivetrain's rotation to any given positive or negative value. However, drivetrain rotation references can differ depending on whether a gyro or the integrated inertial sensor is configured in the Drivetrain configuration.

If the Drivetrain is configured with the integrated inertial sensor, the Drivetrain will have a clockwise-positive rotation, meaning that rotation will increase as the Drivetrain turns right.

Alternatively, if the Drivetrain is configured with a gyro sensor, the Drivetrain will have a counter-clockwise-positive rotation, meaning that rotation will increase as the Drivetrain turns left.

## Example

This example will turn the robot a total of 210 degrees:

```cpp
Drivetrain.turnToRotation(120, degrees);
Drivetrain.setRotation(-45, degrees);
Drivetrain.turnToRotation(45, degrees);
```

(The descriptions below are based on an IQ (1st generation) Brain + Drivetrain configuration, or an IQ (2nd generation) Brain + Drivetrain configuration with a gyro sensor)

- Turn left (counter-clockwise) to rotation 120 degrees.
- Set the robot's current position as rotation of -45 degrees.
- Turn left (counter-clockwise) an additional 90 degrees (-45 degrees to +45 degrees).

<advanced>
</advanced>