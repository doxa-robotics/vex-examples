category: sensing  
signature: brain.button.pressing()  
description: Reports if the specified button on the VEX IQ Brain is being pressed  

# Brain Button Pressing

Reports if the specified button on the VEX IQ Brain is being pressed.

```python
brain.button.pressing()
```

## How To Use

Reports **True** if the specified Brain button is pressed. Reports **False** if the specified Brain button is not pressed.

After `brain.` enter a Brain button to receive the pressed status on.

Supported Brain buttons are as follows:

- `buttonUp` / `buttonLeft`
- `buttonDown` / `buttonRight`
- `buttonCheck`

## Example

This example will make the VEX IQ robot drive forward.

Then, it will check for a press on the Brain's **buttonUp** and then turn the robot right indefinitely.

```python
drivetrain.drive(FORWARD)

while True:
    if brain.buttonUp.pressing():
        drivetrain.turn(RIGHT)
        break
```

<advanced>
</advanced>