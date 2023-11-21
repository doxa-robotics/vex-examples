category: sensing  
signature: optical.brightness()  
device_class: optical  
description: Reports the amount of light detected by a VEX IQ Optical Sensor  

# Optical Brightness

Reports the amount of light detected by a VEX IQ Optical Sensor.

```python
optical.brightness()
```

## How To Use

`Optical Brightness` reports a range of values from **0 to 100** percent.

A large amount of light detected will report a high brightness value.

A small amount of light detected will report a low brightness value.

```python
brain.screen.print("Brightness:", optical.brightness())
```

<advanced>
</advanced>






