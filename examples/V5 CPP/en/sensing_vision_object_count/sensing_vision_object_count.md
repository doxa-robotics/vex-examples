category: sensing  
signature: VISION.objectCount  
device_class: vision  
description: Reports how many objects the Vision Sensor detects. 

# Vision Object Count

Reports how many objects the Vision Sensor detects. 

An object will need to be configured before the `Vision.objectCount` command can detect it.

```cpp
Vision.objectCount
```

## How To Use

Make sure you specify the Vision Sensor when using this command. 

Before the `Vision.objectCount` can report a number of objects, `Vision.takeSnapshot()` will need to be used.

`Vision.objectCount` will only detect the number of objects from the last snapshot signature.

<advanced>
</advanced>