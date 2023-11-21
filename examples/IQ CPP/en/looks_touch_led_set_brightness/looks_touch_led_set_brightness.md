category: looks  
signature: TouchLED.brightness();  
device_class: led  
description: Sets the brightness of the touchLED.  

# Set TouchLED Brightness

Sets the brightness level of the VEX IQ TouchLED.

```cpp
TouchLED.setBrightness(brightness);
```

## How To Use

`TouchLED.setBrightness` accepts a range of **0 to 100** for the `brightness` parameter.

The first part of the command is the device instance. 

```cpp
TouchLED1.setBrightness(100);
TouchLED2.setBrightness(50);
```

## Example

This example will illuminate the TouchLED green at 25% brightness.

```cpp
TouchLED.setBrightness(25);
TouchLED.setColor(green);
```

<advanced>
</advanced>