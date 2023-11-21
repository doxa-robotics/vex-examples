category: sensing  
signature: controller.axis.position()  
device_class: controller  
description: Reports the position of a joystick on the VEX IQ Controller along the specified axis  

# Controller Axis Position

Reports the position of a joystick on the VEX IQ Controller along the specified axis.

```python
controller.axis.position()
```

## How To Use

`Controller Axis Position` reports a range between **-100 to 100**.

`Controller Axis Position` will report **0** when a joystick axis is centered.

Choose which Controller axis to report.

* `axisA` - left joystick (up and down)
* `axisB` - left joystick (left and right)
* `axisC` - right joystick (left and right)
* `axisD` - right joystick (up and down)

## Example

The example below will print the position of the Controller's A axis to the VEX IQ brain's screen.

```python
while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)
    brain.screen.print("AxisA:", controller.axisA.position())

    # Brief wait to prevent print distortion or tearing
    wait(0.1, SECONDS)
```

<advanced>
</advanced>