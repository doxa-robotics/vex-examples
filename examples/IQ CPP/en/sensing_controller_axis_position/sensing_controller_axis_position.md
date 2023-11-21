category: sensing  
signature: Controller.Axis.position()  
device_class: controller  
description: Reports the position of a joystick on the IQ Controller along an axis.  

# Controller Axis Position

Reports the position of a joystick on the VEX IQ's Controller along the specified axis.

```cpp
Controller.Axis.position()
```

## How To Use

`Controller.Axis.position` reports a range between **-100 to 100**.

`Controller.Axis.position` will report **0** when a joystick axis is centered.

Choose which Controller axis to report.

* `AxisA` - left joystick (up and down)
* `AxisB` - left joystick (left and right)
* `AxisC` - right joystick (left and right)
* `AxisD` - right joystick (up and down)

## Example

The example below will print the position of the Controller's AxisA axis to the VEX IQ brain's screen.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("AxisA Position: %.0f", Controller.AxisA.position());

  // Brief wait to prevent print distortion or tearing
  wait(20, msec);
}

```

<advanced>
</advanced>