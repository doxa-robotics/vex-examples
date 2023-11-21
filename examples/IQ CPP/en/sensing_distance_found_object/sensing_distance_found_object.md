category: sensing  
signature: Distance.foundObject()  
device-class: sonar
description: Reports if the VEX IQ Distance Sensor sees an object within its field of view. 

# Distance Found Object

Reports if the VEX IQ Distance Sensor detects an object within its field of view. 

```cpp
Distance.foundObject()
```

## How To Use

Reports **true** when the Distance Sensor sees an object or surface within its field of view. Reports **false** when the Distance Sensor does not detect an object or surface.

The first part of the command is the device instance.

```cpp
Distance3.foundObject()
Distance4.foundObject()
```

## Example

The example below prints whether the Distance Sensor detects an object or surface in its range.

```cpp
Brain.Screen.print("Found Object: %s", Distance.foundObject() ? "TRUE" : "FALSE");
```

<advanced>
</advanced>