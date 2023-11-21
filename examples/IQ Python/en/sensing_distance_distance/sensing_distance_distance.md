category: sensing  
signature: distance.distance(UNITS)  
device-class: sonar  
description: Reports the distance of the nearest object from a VEX IQ Distance Sensor  

# Distance From

Reports the distance of the nearest object from a VEX IQ Distance Sensor (1st generation).

```python
distance.distance(UNITS)
```

## How To Use

`Distance From` reports a range of values between **24 to 1000** mm (millimeters) or **1 to 40** in (inches).

Specify whether the value returned by `Distance From` is reported in **inches** or **mm** (millimeters) by replacing the **UNITS** parameter with either **INCHES** or **MM**, respectively.

## Example

The example below prints to an IQ Brain's screen if an object or surface is detected within 100 mm.

```python
if distance.distance(MM) < 100:
    brain.screen.print("Detected")
```

<advanced>
</advanced>