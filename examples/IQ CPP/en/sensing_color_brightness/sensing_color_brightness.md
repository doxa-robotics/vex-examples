category: sensing  
signature: Color.brightness()  
description: Reports if a button on the VEX IQ Brain is pressed.

# Color Brightness

Reports the amount of light detected by the VEX IQ Color Sensor.

```cpp
Color.brightness()
```

## How To Use

`Color.brightness` reports a range of values from **0% to 100%**.

The first part of the command is the device instance.

```cpp
Color2.brightness()
Color4.brightness()
```

A larger amount of light will report a higher value, while a smaller amount of light will report a lower value.

## Example

The example below prints the amount of light detected by the Color Sensor.

```cpp
Brain.Screen.print("Brightness: %d", Color.brightness());
```

<advanced>
</advanced>
