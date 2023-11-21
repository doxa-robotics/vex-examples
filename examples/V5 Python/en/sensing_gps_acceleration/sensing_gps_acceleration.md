category: sensing  
signature: gps.acceleration(AxisType.XAXIS)  
description: Reports the acceleration value of the specified axis on a GPS Sensor.  

# GPS Acceleration

Reports the acceleration value of the specified axis on a GPS Sensor.

```python
gps.acceleration(AXIS)
```

## How To Use

The `gps.acceleration()` command reports a numerical value in the range of **-4.0** to **4.0** Gs.

It can report acceleration values from three different axes based on the value passed as the `AXIS` parameter.

* Used with the **AxisType.XAXIS** parameter, the value reported will be the acceleration value of a GPS Sensor's forward and backward rotations

* Used with the **AxisType.YAXIS** parameter, the value reported will be the acceleration value of a GPS Sensor's left and right rotations

* Used with the **AxisType.ZAXIS** parameter, the value reported will be the acceleration value of a GPS Sensor's up and down movements

## Example

```python
# Print the current acceleration on the GPS Sensor's X axis
brain.screen.print("Acceleration on X: ", gps.acceleration(AxisType.XAXIS))
```

<advanced>
</advanced>
