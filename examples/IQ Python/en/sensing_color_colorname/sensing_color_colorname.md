category: sensing  
signature: color.color()  
device-class: colorsensor  
description: Reports the color currently being detected by a VEX IQ Color Sensor  

# Color

Reports the color currently being detected by a VEX IQ Color Sensor.

```python
color.color()
```

## How To Use

Compare the value returned by `Color` to one of the following colors to check if a specific color is being detected:
 
- `Color.RED`
- `Color.RED_VIOLET`
- `Color.VIOLET`
- `Color.BLUE_VIOLET`
- `Color.BLUE`
- `Color.BLUE_GREEN`
- `Color.GREEN`
- `Color.YELLOW_GREEN`
- `Color.YELLOW`
- `Color.YELLOW_ORANGE`
- `Color.ORANGE`
- `Color.RED_ORANGE`

## Example

The example below prints "Red" to the IQ Brain's screen if a red object is currently being detected by a Color Sensor.

```python
if color.color() == Color.RED:
    brain.screen.print("Red")
```

<advanced>
</advanced>