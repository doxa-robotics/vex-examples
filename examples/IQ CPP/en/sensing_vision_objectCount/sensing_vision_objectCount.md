category: sensing  
signature: Vision.objectCount  
device_class: vision  
description: Reports how many objects the Vision Sensor detects. 

# Vision Object Count

Reports how many objects the Vision Sensor detects. 

```cpp
Vision.objectCount
```

## How To Use

Make sure you specify the Vision Sensor when using this command. 

A signature will need to be configured before the `Vision.objectCount` command can detect it.

Before the `Vision.objectCount` can report the number of objects detected, `Vision.takeSnapshot` will need to be called to capture a snapshot with the specified signature.

`Vision.objectCount` will return the number of objects detected from the last snapshot.

## Example

The example below prints the number of objects detected by the Vision Sensor with the specified signature to the VEX IQ Brain's screen.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);

  // Take a snapshot with the specified signature
  Vision.takeSnapshot(SIGNATURE);

  Brain.Screen.print("Number of Objects Detected: %d", Vision.objectCount);

  // Take a new snapshot every 20 milliseconds
  wait(20, msec);
}
```

<advanced>
</advanced>