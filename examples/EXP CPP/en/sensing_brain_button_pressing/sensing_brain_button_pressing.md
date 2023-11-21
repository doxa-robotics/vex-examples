category: sensing  
signature: Brain.Button.pressing()  
description: Reports if a button on the EXP Brain is pressed.

# Brain Button Pressing

Reports if the specified button on the EXP Brain is being pressed.

```cpp
Brain.Button.pressing()
```

## How To Use

Reports **true** if the specified Brain button is pressed. Reports **false** if the specified Brain button is not pressed.

After `Brain.` enter a Brain button to receive the pressed status on.


Supported Brain buttons are as follows:

- `buttonLeft` 
- `buttonRight`
- `buttonCheck`

## Example

This example will make the EXP robot drive forward.

Then, it will check for a press on the Brain's **buttonUp** and then turn the robot right indefinitely.

```cpp
Drivetrain.drive(forward);

while (true) {
  if (Brain.buttonUp.pressing()) {
    Drivetrain.turn(right);
    break;
  }

  wait(20, msec);
}
```

<advanced>
</advanced>