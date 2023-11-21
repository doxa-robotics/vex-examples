category: looks  
signature: TouchLED.setFade(fade);  
device_class: led  
description: Sets the fade speed of the touchLED.

# Set TouchLED Fade

Sets how fast the color of the VEX IQ TouchLED fades between colors.

```cpp
TouchLED.setFade(fade);
```

## How To Use

The first part of the command is the device instance.

```cpp
TouchLED1.setFade(fast);
TouchLED2.setFade(slow);
```
Choose how fast the TouchLED will fade between colors. Replace `fade` with one of the following options:

* **slow** - The TouchLED will slowly fade to a new color.
* **fast** - The TouchLED will quickly fade to a new color.
* **off** - The TouchLED will change colors instantly.

## Example

This example will slowly fade the TouchLED from red to blue.

```cpp
TouchLED.setColor(red);
TouchLED.setFade(slow);
TouchLED.setColor(blue);
```

<advanced>
</advanced>