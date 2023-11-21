category: sensing  
signature: color.is_near_object()  
device-class: colorsensor  
description: Reports if a VEX IQ Color Sensor detects an object or surface  

# Color Is Near Object

Reports if a VEX IQ Color Sensor detects an object or surface.

```python
color.is_near_object()
```

## How To Use

Reports **True** when a Color Sensor detects an object or surface close to the front of the sensor. 

Reports **False** when a Color Sensor does not detect an object or surface close to the front of the sensor.

## Example

The example below prints whether an object or surface is being detected by a Color Sensor.

```python
brain.screen.print("True" if color.is_near_object() else "False")
```

<advanced>
</advanced>