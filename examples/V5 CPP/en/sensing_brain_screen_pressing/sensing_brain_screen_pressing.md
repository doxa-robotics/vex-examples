category: sensing  
signature: Brain.Screen.pressing()  
description: Reports if the V5 Brain's touchscreen is currently being pressed.

# Brain.Screen.pressing()

Reports if the V5 Brain's touchscreen is currently being pressed.

```cpp
Brain.Screen.pressing()
```

## How To Use

The `Brain.Screen.pressing()` command can be used together with the `Brain.Screen.xPosition()` and `Brain.Screen.yPosition()` to detect when and where a touch has occured on the V5 Brain's touchscreen.

`Brain.Screen.pressing()` reports **true** when the V5 Brain's touchscreen is being pressed.

`Brain.Screen.pressing()` reports **false** when the V5 Brain's touchscreen is not being pressed.

```cpp
if (Brain.Screen.pressing()) {
  Brain.Screen.print("Screen is being pressed!");
}
```


<advanced>
</advanced>