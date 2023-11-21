category: sensing  
signature: controller.button.pressing()  
device_class: controller  
description: Reports if the specified button on the Controller is being pressed  

# Controller Button Pressing

Reports if the specified button on the VEX IQ's Controller is being pressed.

```python
controller.button.pressing()
```

## How To Use

Choose which Controller button to detect a press on:

- `buttonEUp`
- `buttonEDown`
- `buttonFUp`
- `buttonFDown`
- `buttonLUp`
- `buttonLDown`
- `buttonRUp`
- `buttonRDown`
- `buttonL3`
- `buttonR3`

![controller_button_back](controller_button_front.jpg)

`Controller Button Pressing` reports **True** if the specified Controller button is being pressed.

`Controller Button Pressing` reports **False** if the specified Controller button is not being pressed.

## Example

The example below drives the VEX IQ robot forward. If the Controller's E Up button is pressed, the robot will then stop driving.

```python
drivetrain.drive(FORWARD)

while True:
    if controller.buttonEUp.pressing():
        drivetrain.stop()
        break
```

<advanced>
</advanced>