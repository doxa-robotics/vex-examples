category: looks  
signature: touchLED.color();  
device_class: led  
description: Sets the color of the touchLED.  

# Set TouchLED Color

Sets the color of the VEX IQ TouchLED.

```cpp
TouchLED.setColor(color);
```

## How To Use

The first part of the command is the device instance.

```cpp
TouchLED1.setColor(red);
TouchLED2.setColor(green);
```
Choose the color that will be displayed.  

Color Options:

- `red`
- `green`
- `blue`
- `white`
- `yellow`
- `orange`
- `purple`
- `red_violet`
- `violet`
- `blue_violet`
- `blue_green`
- `yellow_green`
- `yellow_orange`
- `red_orange`

To turn the TouchLED off, set the color to **colorType::none**.

```cpp
TouchLED.setColor(colorType::none);
```

<advanced>
</advanced>