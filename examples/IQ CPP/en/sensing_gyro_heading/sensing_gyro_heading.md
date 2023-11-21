category: sensing  
signature: Gyro.heading() 
device_class: gyro  
description: Reports a Gyro Sensor's current heading in degrees.

# Gyro Heading

Reports a Gyro Sensor's current heading in degrees.

```cpp
Gyro.heading()
```

## How To Use

`Gyro.heading` reports a range from **0.00 to 359.99**.

The `Gyro.heading` command reports an increase in heading when rotating **counter-clockwise**.

The `Gyro.heading` command reports a decrease in heading when rotating **clockwise**.

## Example

The example below prints the heading of the Gyro Sensor to the VEX IQ brain's screen.

```cpp
Drivetrain.turn(left);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Gyro Heading: %.2f", Gyro.heading());

  // Brief delay to prevent print distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>