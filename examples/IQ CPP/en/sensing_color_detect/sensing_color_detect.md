category: sensing  
signature: Color.detects(color)  
device-class: colorsensor
description: Reports if a color sensor detects a specific color.

# Color Detects

Reports if the VEX IQ Color Sensor detects the specified color.

```cpp
Color.detects(color)
```

## How To Use

Reports **true** when the Color Sensor detects the specified color. Reports **false** when the Color Sensor detects a different color than the one specified.

The first part of the command is the device instance.

```cpp
Color1.detects(red)
Color2.detects(blue)
```

Choose which color to detect.

- `red`
- `orange`
- `yellow`
- `green`
- `blue`
- `purple`
- `violet`
- `red_violet`
- `blue_violet`
- `blue_green`
- `yellow_green`
- `yellow_orange`
- `red_orange`
- `white`

You can also pass **colorType::none** as the specified `color` to check if the Color Sensor does **not** detect an object.

## Example

This example will print "Color Red" or "Other Color" depending on whether or not the Color Sensor detects the color "red".

```cpp
if (Color.detects(red)) { 
  Brain.Screen.print("Color Red");
} else {
  Brain.Screen.print("Other Color");
}
```

<advanced>
</advanced>