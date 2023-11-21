category: sensing  
signature: Motor.isSpinning()  
device_class: motor  
description: Reports if the selected Motor or Motor Group is currently spinning.

# Motor Is Spinning

Reports if the selected VEX IQ Smart Motor or Motor Group is currently spinning.

```cpp
Motor.isSpinning()
```

## How To Use

This command returns **true** if the specified Motor/Motor Group is currently spinning.

This command returns **false** if the specified Motor/Motor Group is not currently spinning.

**Note:** This command will always return **false** if the Motor/Motor Group is spinning as a result of a previous `Motor.spin` command (which does *not* specify a set distance to spin).

## Example

The example below will print whether the ArmMotor is still spinning to the VEX IQ brain's screen.

```cpp
ArmMotor.spinFor(forward, 270, degrees, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("ArmMotor is Spinning: %s", ArmMotor.isSpinning() ? "TRUE" : "FALSE");

  // Brief delay to prevent print distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>