category: sensing  
signature: OPTICAL.gestureEnable();  
device_class: optical  
description: Sets an Optical Sensor to detect gestures  

# Optical Gesture Enable

Sets an Optical Sensor to detect gestures.

```cpp
Optical.gestureEnable();
```

## How To Use

The `Optical Gesture Enable` command allows you to set an Optical Sensor to detect gestures.

By default, an Optical Sensor will be set to detect colors.

Before using any Optical Sensor gesture commands, an Optical Sensor must be correctly set to detect gestures.

## Examples

The example shows how to correctly set an Optical Sensor to detect gestures before checking for gestures.

```cpp
Optical.gestureEnable();
while (Optical.getGesture().type != gestureType::up) {
  wait(0.1, seconds);
}
Brain.Screen.print("Up!");
```

<advanced>
</advanced>







