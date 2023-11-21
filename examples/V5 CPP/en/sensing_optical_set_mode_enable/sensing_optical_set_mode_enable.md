category: sensing  
signature: OPTICAL.gestureEnable();  
device_class: optical  
description: Sets a V5 Optical Sensor to detect gestures  

# Optical Gesture Enable

Sets a V5 Optical Sensor to detect gestures.

```cpp
Optical.gestureEnable();
```

## How To Use

The `Optical Gesture Enable` command allows you to set a V5 Optical Sensor to detect gestures.

By default, a V5 Optical Sensor will be set to detect colors.

Before using any V5 Optical Sensor gesture commands, a V5 Optical Sensor must be correctly set to detect gestures.

## Examples

The example shows how to correctly set a V5 Optical Sensor to detect gestures before checking for gestures.

```cpp
Optical.gestureEnable();
while (Optical.getGesture().type != gestureType::up) {
  wait(0.1, seconds);
}
Brain.Screen.print("Up!");
```

<advanced>
</advanced>







