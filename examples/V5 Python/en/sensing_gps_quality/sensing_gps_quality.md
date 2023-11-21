category: sensing  
signature: gps.quality()  
description: Reports a GPS Sensor's current signal quality.  

# GPS Signal Quality

Reports a GPS Sensor's current signal quality.

```python
gps.quality()
```

## How To Use

The `gps.quality()` command reports a numerical value representing the current signal quality of a GPS Sensor.

When the reported value is **100**, it means that all reported positional and heading data from a GPS Sensor is valid.

However, a reported value of **90** signals that any positional data is no longer being calculated by capturing information from the VEX Field Code, but rather through alternative means.

At **80**, only GPS Sensor heading values are valid, but as more time goes by where a GPS Sensor is not scanning enough of the VEX Field Code to accurately determine positiona and heading information, the reported signal quality will continue to drop until **0**, where any GPS Sensor data is effectively frozen and no longer valid.

## Example

```python
# Print a GPS Sensor's signal quality
brain.screen.print("GPS Signal Quality: ", gps.quality())
```

<advanced>
</advanced>
