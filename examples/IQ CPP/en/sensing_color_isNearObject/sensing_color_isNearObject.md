category: sensing  
signature: Color.isNearObject()  
description: Reports if the Color Sensor is near an object.

# Color Is Near Object

Reports if the Color Sensor detects an object or surface. 

```cpp
Color.isNearObject()
```

## How To Use

The first part of the command is the device instance.

```cpp
Color5.isNearObject()
Color7.isNearObject()
```

Reports **true** when the Color Sensor detects an object or surface close to the front of the sensor. 

Reports **false** when the Color Sensor does not detect an object or surface close to the front of the sensor.

## Example

The example below prints whether an object or surface is being detected by the Color Sensor.

```cpp
Brain.Screen.print("Is Near Object: %s", Color.isNearObject() ? "TRUE" : "FALSE");
```

<advanced>
</advanced>