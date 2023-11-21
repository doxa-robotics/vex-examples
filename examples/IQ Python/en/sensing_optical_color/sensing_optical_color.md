category: sensing  
signature: optical.color()  
device_class: optical  
description:  Returns the color detected by a VEX IQ Optical Sensor  

# Optical Color

Returns the color detected by a VEX IQ Optical Sensor.

```python
optical.color()
```

## How To Use

The `Optical Color` command returns the closest color match base on the hue of a detected object.

The following colors can be used as a comparison to the color detected by an IQ Optical Sensor:

- `Color.RED`
- `Color.GREEN`
- `Color.BLUE`
- `Color.YELLOW`
- `Color.ORANGE`
- `Color.PURPLE`
- `Color.CYAN`

## Example

The example prints to a VEX IQ Brain's screen if a red object is detected by an Optical Sensor.

```python
if optical.color() == Color.RED:
    brain.screen.print("Red!")
```

<advanced>
</advanced>







