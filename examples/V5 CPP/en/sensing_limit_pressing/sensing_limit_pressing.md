category: sensing  
signature: LimitSwitch.pressing()  
device_class: limit  
description: Reports if the Limit Switch is pressed.

# LimitSwitch Pressing

Reports if the Limit Switch is pressed.

```cpp
LimitSwitch.pressing()
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`LimitSwitch.pressing()` reports **true** if the Limit Switch is being pressed.

`LimitSwitch.pressing()` reports **false** if the Limit Switch is not being pressed.

```cpp
waitUntil(LimitSwitchB.pressing());
``` 
<advanced>
</advanced>
