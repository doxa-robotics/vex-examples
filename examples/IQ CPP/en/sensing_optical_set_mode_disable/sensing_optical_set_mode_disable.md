category: sensing  
signature: OPTICAL.gestureDisable();  
device_class: optical  
description: Sets an IQ Optical Sensor to detect colors  

# Optical Gesture Disable

Sets an IQ Optical Sensor to detect colors.

```cpp
Optical.gestureDisable();
```

## How To Use

The `Optical Gesture Disable` command allows you to set an IQ Optical Sensor to detect colors.

By default, an IQ Optical Sensor will be set to detect colors.

## Examples

The example shows how to correctly set an IQ Optical Sensor to detect colors after checking for gestures.

```cpp
// Detect gestures
Optical.gestureEnable();
while (Optical.getGesture().type != gestureType::up) {
  wait(0.1, seconds);
}
Brain.Screen.print("Up!");

wait(1, seconds);

// Detect colors
Optical.gestureDisable();
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  if (Optical.color() == red) {
    Brain.Screen.print("Red Object!");
  } else {
    Brain.Screen.print("Not Red Object!");
  }
  wait(0.02, seconds);
}
```

<advanced>
</advanced>







