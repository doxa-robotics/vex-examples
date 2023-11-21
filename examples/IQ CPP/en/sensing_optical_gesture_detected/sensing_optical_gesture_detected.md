category: sensing  
signature: OPTICAL.getGesture()  
device_class: optical  
description: Reports detected gesture data from an IQ Optical Sensor  

# Optical Gesture Detected

Reports detected gesture data from an IQ Optical Sensor.

```cpp
Optical.getGesture()
```

## How To Use

The `Optical Gesture Detected` command returns an object with gesture information. To check the type of the detected gesture, access the `type` property on the returned object.

```cpp
Optical.getGesture().type
```

Before using any IQ Optical Sensor gesture commands, an IQ Optical Sensor must be correctly set to detect gestures with the `Optical.gestureEnable();` command.

Below are the gestures that an IQ Optical Sensor can detect:

- `gestureType::up`
- `gestureType::down`
- `gestureType::left`
- `gestureType::right`

## Example

The example shows how to correctly set an IQ Optical Sensor to detect gestures before checking for gestures.

```cpp
Optical.gestureEnable();
while (Optical.getGesture().type != gestureType::up) {
  wait(0.1, seconds);
}
Brain.Screen.print("Up!");
```

<advanced>
</advanced>







