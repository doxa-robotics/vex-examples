category: sensing  
signature: GPS.quality()  
device_class: gps  
description: Reports a GPS Sensor's current signal quality.  

# GPS Signal Quality

Reports a GPS Sensor's current signal quality.

```cpp
GPS.quality()
```

## How To Use

The `GPS.quality()` command reports an *integer* representing the current signal quality of a GPS Sensor.

When the reported value is **100**, it means that all reported positional and heading data from a GPS Sensor is valid.

However, a reported value of **90** signals that any positional data is no longer being calculated by capturing information from the VEX Field Code, but rather through alternative means.

At **80**, only GPS Sensor heading values are valid, but as more time goes by where a GPS Sensor is not scanning enough of the VEX Field Code to accurately determine positiona and heading information, the reported signal quality will continue to drop until **0**, where any GPS Sensor data is effectively frozen and no longer valid.

```cpp
Brain.Screen.print("GPS Signal Quality: %d", GPS.quality());
```

<advanced>
</advanced>