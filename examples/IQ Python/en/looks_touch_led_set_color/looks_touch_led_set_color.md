category: looks  
signature: touchled.set_color(COLOR)  
device_class: touchled  
description: Sets the color of an IQ TouchLED  

# Set TouchLED Color

Sets the color of an IQ TouchLED.

```python
touchled.set_color(COLOR)
```

## How To Use

Replace the **COLOR** parameter with one of the following options:

- `Color.RED`
- `Color.GREEN`
- `Color.BLUE`
- `Color.WHITE`
- `Color.YELLOW`
- `Color.ORANGE`
- `Color.PURPLE`
- `Color.RED_VIOLET`
- `Color.VIOLET`
- `Color.BLUE_VIOLET`
- `Color.BLUE_GREEN`
- `Color.YELLOW_GREEN`
- `Color.YELLOW_ORANGE`
- `Color.RED_ORANGE`

To turn the TouchLED off, set the color to `Color.BLACK`.

```python
touchled.set_color(Color.BLACK)
```

<advanced>
</advanced>