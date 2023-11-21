category: sensing  
signature: Vision.takeSnapshot(signature);  
device_class: vision  
description: Takes a snapshot from the Vision Sensor. A user defined signature or color code will need to replace the "SIGNATURE" parameter in order for this example snippet to compile.

# Vision Take Snapshot

Takes a snapshot from the Vision Sensor.

```cpp
Vision.takeSnapshot(signature);
```

## How To Use

`Vision.takeSnapshot` will capture a signature from the Vision Sensor to be processed and analyzed for color signatures and codes.

To use the `Vision.takeSnapshot` command, the Vision Sensor will need to be configured with at least one signature before this command is called. The signature name will be automatically generated.

For example, if the instance of the Vision Sensor has the name `Vision1` and the signature is configured with the name `REDBOX`, the name of the signature will be `Vision1__REDBOX` and to take the snapshot with that signature you would then call:

```cpp
Vision1.takeSnapshot(Vision1__REDBOX);
```

Typically, the `Vision.takeSnapshot` will need to be called first before using any other Vision Sensor commands.

Make sure you specify the Vision Sensor and the vision signature when using this command. Vision signatures are configured from the Robot Configuration window.

<advanced>
</advanced>