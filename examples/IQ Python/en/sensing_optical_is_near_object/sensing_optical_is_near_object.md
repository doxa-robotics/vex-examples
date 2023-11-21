category: sensing  
signature: optical.is_near_object()  
device_class: optical  
description: Reports if a VEX IQ Optical Sensor detects an object in its range  

# Optical Is Near Object

Reports if a VEX IQ Optical Sensor detects an object in its range.

```python
optical.is_near_object()
```

## How To Use

`Optical Is Near Object` returns **True** if an object is detected, and returns **False** otherwise.

It should be used to check if an object is close to the IQ Optical Sensor so that the color readings from the Optical Sensor's `Color` command is accurate.

```python
if optical.is_near_object() and optical.color() == Color.Red:
    brain.screen.print("Red object!")
```

<advanced>
</advanced>







