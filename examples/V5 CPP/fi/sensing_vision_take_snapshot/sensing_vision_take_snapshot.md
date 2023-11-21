category: sensing  
signature: VISION.takeSnapshot(SIGNATURE);  
device_class: vision  
description: Takes a snapshot from the Vision Sensor. A user defined signature or color code will need to replace the "SIGNATURE" parameter in order for this example snippet to compile.

# Vision Take Snapshot

Takes a snapshot from the Vision Sensor.

```cpp
Vision.takeSnapshot(SIG_1);
```

## How To Use

`Vision.takeSnapshot()` will capture the current image from the Vision Sensor, filter out the requested signatures, and copies the detected objects's data for further analysis.

Typically, `Vision.takeSnapshot()` is required first before using any other Vision Sensor commands.

Make sure you specify the Vision Sensor and the vision signature when using this command. Vision signatures are configured from the Robot Configuration window.

<advanced>
</advanced>