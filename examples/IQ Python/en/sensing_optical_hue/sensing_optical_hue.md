category: sensing  
signature: optical.hue()  
device_class: optical  
description: Reports the hue of the object detected by a VEX IQ Optical Sensor  

# Optical Hue

Reports the hue of the object detected by a VEX IQ Optical Sensor.

```python
optical.hue()
```

## How To Use

`Optical Hue` reports a range of values from **0 to 359**, which represents the location of the detected color on a color wheel.

```python
brain.screen.print("Hue: ", optical.hue())
```

<advanced>
</advanced>







