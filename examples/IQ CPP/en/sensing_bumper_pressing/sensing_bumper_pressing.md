category: sensing  
signature: Bumper.pressing()  
device-class: bumper
description: Reports if the VEX IQ Bumper is pressed.

# Bumper Pressing

Reports if the VEX IQ Bumper is being pressed.

```cpp
Bumper.pressing()
```

## How To Use

`Bumper.pressing` reports **true** if the Bumper is being pressed.

`Bumper.pressing` reports **false** if the Bumper is not being pressed.

The first part of the command is the device instance.

```cpp
Bumper2.pressing()
Bumper4.pressing()
```

## Example

The example below prints whether a Bumper is being pressed to the VEX IQ brain's screen.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Bumper Pressed: %s", Bumper2.pressing() ? "TRUE" : "FALSE");

  // Brief delay to prevent print distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>
