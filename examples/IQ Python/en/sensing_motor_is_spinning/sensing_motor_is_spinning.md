category: sensing  
signature: motor.is_spinning()
description: Reports if an IQ Motor or Motor Group is currently spinning  

# Motor Is Spinning

Reports if an IQ Motor or Motor Group is currently spinning.

```python
motor.is_spinning()
```

## How To Use

`Motor Is Spinning` reports **True** when the selected Motor or Motor Group is still moving.

`Motor Is Spinning` reports **False** when the selected Motor or Motor Group is stopped.

**Note:** This command will always return **false** if the Motor/Motor Group is spinning as a result of a previous `motor.spin` command (which does *not* specify a set distance to spin).

## Example

The example below will print whether the ArmMotor is still spinning to the VEX IQ brain's screen.

```python
arm_motor.spin_for(FORWARD, 270, DEGREES, wait=False)

while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)
    brain.screen.print("ArmMotor is Spinning:", "TRUE" if arm_motor.is_spinning() else "FALSE")

    # Brief delay to prevent print distortion or tearing
    wait(20, MSEC);
```

<advanced>
</advanced>
