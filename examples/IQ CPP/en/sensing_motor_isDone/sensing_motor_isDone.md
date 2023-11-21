category: sensing  
signature: Motor.isDone()  
device_class: motor  
description: Reports if the Motor or Motor Group has completed its movement.

# Motor Is Done

Reports if the VEX IQ Smart Motor or Motor Group has completed its movement.

```cpp
Motor.isDone()
```

## How To Use

`Motor.isDone` reports **true** when the specified Motor/Motor Group has completed its movement.

`Motor.isDone` reports **false** when the specified Motor/Motor Group has not completed its movement.

## Example

The example below prints whether the ArmMotor has completed its movements to the VEX IQ brain's screen.

```cpp
ArmMotor.spinFor(forward, 270, degrees, false);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("ArmMotor is Done: %s", ArmMotor.isDone() ? "TRUE" : "FALSE");

  // Brief delay to prevent print distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>