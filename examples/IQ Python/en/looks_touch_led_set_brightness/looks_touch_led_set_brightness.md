category: looks  
signature: touchled.set_brightness(BRIGHTNESS)  
device_class: touchled  
description: Sets the brightness of an IQ TouchLED  

# Set TouchLED Brightness

Sets the brightness of an IQ TouchLED.

```python
touchled.set_brightness(BRIGHTNESS)
```

## How To Use

`Set TouchLED Brightness` accepts a range of **0 to 100** for the `BRIGHTNESS` parameter.
 
```python
touchled.set_brightness(50)
```

## Example

This example will illuminate the TouchLED green at 25% brightness.

```python
touchled.set_brightness(25)
touchled.set_color(Color.GREEN)
```

<advanced>
</advanced>