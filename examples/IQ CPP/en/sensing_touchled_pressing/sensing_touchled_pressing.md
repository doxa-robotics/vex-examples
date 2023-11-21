category: sensing  
signature: TouchLED.pressing()  
device_class: TouchLED
description: Reports if the VEX IQ Touch LED is pressed. 

# TouchLED Pressing

Reports if the VEX IQ TouchLED is pressed.

```cpp
TouchLED.pressing()
```

## How To Use

Reports **true** if the selected TouchLED is being pressed. Reports **false** if the selected TouchLED is not being pressed.

The first part of the command is the device instance. 

```cpp
TouchLED2.pressing()
TouchLED4.pressing()
```

## Example

The example below sets the TouchLED to **red**. When the TouchLED is pressed, its color is set to **green**.

```cpp
TouchLED.setColor(red);

while (!TouchLED.pressing()) {
  wait(20, msec);
}

TouchLED.setColor(green);
```

<advanced>
</advanced>