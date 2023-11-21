category: sensing  
signature: distance.object_distance(UNITS)  
device_class: distance  
description: Reports the distance of the nearest object or surface from a VEX IQ Distance Sensor  

# Distance Object Distance

Reports the distance of the nearest object or surface from a VEX IQ Distance Sensor (2nd generation).

```python
distance.object_distance(UNITS)
```

## How To Use

`Distance Object Distance` accepts **MM** or **INCHES** as the **UNITS** parameter and reports a range from **20 to 2000** mm (millimeters) or approximately **0.8 to 79.0** inches.

## Example

The example below prints to a VEX IQ Brain's screen if an object or surface is detected within 100 mm.

```python
if distance.object_distance(MM) < 100:
    brain.screen.print("Detected")
```

<advanced>
</advanced>





