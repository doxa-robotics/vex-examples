category: sensing  
signature: distance.is_object_detected()  
device_class: distance  
description: Reports if a VEX IQ Distance Sensor detects an object or surface in its range  

# Distance Object Detected

Reports if a VEX IQ Distance Sensor (2nd generation) detects an object or surface in its range.

```python
distance.is_object_detected()
```

## How To Use

`Distance Object Detected` returns **True** if an object or surface is detected in its range, and **False** if not.

## Example

The example below prints "True" to a VEX IQ Brain's screen if an object or surface is detected by a Distance Sensor.

```python
if dstance.is_object_detected():
    brain.screen.print("True")
```

<advanced>
</advanced>




