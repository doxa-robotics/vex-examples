category: sensing  
signature: Gyro.rotation()  
device_class: gyro  
description: Reports a Gyro Sensor's current rotation in degrees.

# Gyro Rotation

Reports a VEX IQ Gyro Sensor's current rotation in degrees.

```cpp
Gyro.rotation()
```

## How To Use

`Gyro.rotation` reports an increasing value when the Gyro Sensor turns in the **counter-clockwise** direction.

`Gyro.rotation` reports a decreasing value when the Gyro Sensor turns in the **clockwise** direction.

## Example

The example below prints the rotation of the Gyro Sensor to the VEX IQ brain's screen.

```cpp
Drivetrain.turn(left);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Gyro Rotation: %.2f", Gyro.rotation());

  // Brief delay to prevent print distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>