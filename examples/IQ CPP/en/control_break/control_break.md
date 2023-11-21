category: control  
signature: control_break
description: Exits a repeating loop immediately.

# Break

Exits a repeating loop immediately.

```cpp
break;
```

## How To Use

When added inside of a loop, the `break` command will exit the loop it is currently in. 

## Example

This example will move the Drivetrain forward and repeatedly check if the VEX IQ Brain’s up button is pressed.

If the up button is pressed, the `break` command will exit the `while` loop and stop the Drivetrain.

```cpp
while (true) {
  Drivetrain.drive(forward);
  if (Brain.buttonUp.pressing()) {
    break;
  }
  wait(20, msec);
}

Drivetrain.stop();
```
<advanced>
</advanced>
