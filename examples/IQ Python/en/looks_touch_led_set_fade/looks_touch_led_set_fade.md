category: looks  
signature: touchled.set_fade(TYPE)  
device_class: touchled  
description: Sets how fast the color of an IQ TouchLED fades between colors  

# Set TouchLED Fade

Sets how fast the color of an IQ TouchLED fades between colors.

```python
touchled.set_fade(TYPE)
```

## How To Use

Choose how fast the TouchLED will fade between colors. Replace **TYPE** with one of the following options:

* **FadeType.SLOW** - The TouchLED will slowly fade to a new color.
* **FadeType.FAST** - The TouchLED will quickly fade to a new color.
* **FadeType.OFF** - The TouchLED will change colors instantly.

```python
touchled.set_fade(FadeType.SLOW)
```

## Example

This example will slowly fade the TouchLED from red to blue.

```python
touchled.set_color(Color.RED)
touchled.set_fade(FadeType.SLOW)
touchled.set_color(Color.BLUE)
```

<advanced>
</advanced>