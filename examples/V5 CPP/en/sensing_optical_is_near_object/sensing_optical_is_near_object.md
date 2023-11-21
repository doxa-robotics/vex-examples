category: sensing  
signature: OPTICAL.isNearObject()  
device_class: optical  
description: Reports if a V5 Optical Sensor detects an object in its range  

# Optical Is Near Object

Reports if a V5 Optical Sensor detects an object in its range.

```cpp
Optical.isNearObject()
```

## How To Use

`Optical.isNearObject()` returns **true** if an object is detected, and returns **false** otherwise.

It should be used to check if an object is close to the Optical Sensor so that the color readings from the `Optical.color()` command is accurate.

```cpp
if (Optical.isNearObject() && Optical.color() == red) {
  Brain.Screen.print("Red object detected!");
}
```

<advanced>
</advanced>







