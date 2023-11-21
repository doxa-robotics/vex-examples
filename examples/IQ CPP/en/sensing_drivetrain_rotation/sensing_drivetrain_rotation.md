category: sensing  
signature: Drivetrain.rotation(degrees)  
device-class: drivetrain
description: Reports the Drivetrain's angle of rotation in degrees when configured with a VEX IQ Gyro or Brain Inertial Sensor.  

# Drive Rotation

Reports the Drivetrain's angle of rotation in degrees when configured with a VEX IQ Gyro or Brain Inertial Sensor.

```cpp
Drivetrain.rotation(degrees)
```

## How To Use

### IQ (1st generation) Brain

`Drivetrain.rotation` reports an increasing value when the Drivetrain turns in the **counter-clockwise** direction.

`Drivetrain.rotation` reports a decreasing value when the Drivetrain turns in the **clockwise** direction.

### IQ (2nd generation) Brain

The `Drivetrain.rotation` command can report a counter-clockwise or clockwise rotation depending on whether the intergrated brain inertial or a gyro sensor is configured in the Drivetrain configuration.

If the Drivetrain is configured with the integrated inertial sensor, the Drivetrain will have a clockwise-positive rotation, meaning that rotation will increase as the Drivetrain turns right.

Alternatively, if the Drivetrain is configured with a gyro sensor, the Drivetrain will have a counter-clockwise-positive rotation, meaning that rotation will increase as the Drivetrain turns left.


## Example

The example below prints the rotation of the Drivetrain to the VEX IQ brain's screen.

```cpp
Drivetrain.turn(left);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Drivetrain Rotation: %.2f", Drivetrain.rotation(degrees));

  // Brief delay to prevent print distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>