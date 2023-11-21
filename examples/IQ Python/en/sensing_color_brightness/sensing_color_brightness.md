category: sensing  
signature: color.brightness()  
description: Reports the amount of light detected by a VEX IQ Color Sensor  

# Color Brightness

Reports the amount of light detected by a VEX IQ Color Sensor.

```python
color.brightness()
```

## How To Use

`Color Brightness` reports a range of values from **0 to 100** percent.

A larger amount of light will report a higher value, while a smaller amount of light will report a lower value.

## Example

The example below prints the amount of light detected by a Color Sensor.

```python
brain.screen.print("Brightness:", color.brightness())
```

<advanced>
</advanced>
