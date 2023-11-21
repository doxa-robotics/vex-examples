category: sensing  
signature: distance.found_object()  
device-class: sonar
description: Reports if a VEX IQ Distance Sensor detects an object within its field of view  

# Distance Found Object

Reports if a VEX IQ Distance Sensor (1st generation) detects an object within its field of view. 

```python
distance.is_object_detected()
```

## How To Use

Reports **True** when a Distance Sensor detects an object or surface within its field of view.

Reports **False** when a Distance Sensor does not detect an object or surface.

## Example

The example below prints whether the Distance Sensor detects an object or surface in its range.

```python
brain.screen.print("True" if distance.is_object_detected() else "False")
```

<advanced>
</advanced>