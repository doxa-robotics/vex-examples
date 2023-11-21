category: sensing  
signature: optical.color()
description: Reports the color that the Optical Sensor is detecting.


# Optical Color Detection

Reports the color that the Optical Sensor is detecting.

```python
optical.color()
```

## How To Use
`optical.color()` will return a RGB (Red, Green, Blue) value that corresponds to a color. You can use the `Color` enums to compare to the value returned by `optical.color()`

You can compare to the following values

* Color.BLACK
* Color.WHITE
* Color.RED
* Color.GREEN
* Color.BLUE
* Color.YELLOW
* Color.ORANGE
* Color.PURPLE
* Color.CYAN

You can use these in a conditional statement like this:

```python
if optical.color() == Color.RED:
    brain.screen.print("Red Object")
```

<advanced>
</advanced>