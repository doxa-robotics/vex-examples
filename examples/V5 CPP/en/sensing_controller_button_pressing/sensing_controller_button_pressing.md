category: sensing  
signature: Controller.buttonUp.pressing()  
device_class: controller  
description: Reports if a button on the V5 Controller is pressed.

# Controller Button Pressing

Reports if a button on the V5 Controller is pressed.

```cpp
Controller.Button.pressing()
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Controller.Button.pressing()` reports **true** if the specified Controller button is being pressed.

`Controller.Button.pressing()` reports **false** if the specified Controller button is not pressed.

The following Controller buttons are valid options to check if it is being pressed:
* ButtonUp
* ButtonDown
* ButtonLeft
* ButtonRight
* ButtonX
* ButtonB
* ButtonY
* ButtonA
* ButtonL1
* ButtonL2
* ButtonR1
* ButtonR2

```cpp
waitUntil(Controller1.ButtonUp.pressing());
```
<advanced>
</advanced>
