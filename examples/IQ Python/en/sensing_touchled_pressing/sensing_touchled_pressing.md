category: sensing  
signature: touchled.pressing()  
device_class: touchled
description: Reports if a VEX IQ TouchLED is currently being pressed  

# TouchLED Pressing

Reports if a VEX IQ TouchLED is currently being pressed.

```python
touchled.pressing()
```

## How To Use

Reports **True** if the selected TouchLED is being pressed. Reports **False** if the selected TouchLED is not being pressed.

## Example

The example below sets the TouchLED to red. When the TouchLED is pressed, its color is set to green.

```python
touchled.set_color(Color.RED)

while not touchled.pressing():
    wait(0.1, SECONDS);

touchled.set_color(Color.GREEN)
```

<advanced>
</advanced>