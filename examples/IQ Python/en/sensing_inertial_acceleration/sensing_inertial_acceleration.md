category: sensing  
signature: inertial.acceleration(AXIS)  
device_class: inertial  
description: Reports the acceleration value from one of the axes (x, y, or z) on the VEX IQ (2nd generation) Brain's Inertial Sensor  

# Inertial Acceleration

Reports the acceleration value from one of the axes (x, y, or z) on the VEX IQ (2nd generation) Brain's Inertial Sensor.  

```python
brain_inertial.acceleration(AXIS)
```

## How To Use

Replace the **AXIS** parameter with one of the following options to get the acceleration values along the selected axis:

* **AxisType.XAXIS**: reports acceleration of an Inertial Sensor's **forward to backward** movements
* **AxisType.YAXIS**: reports acceleration of an Inertial Sensor's **side to side** movements
* **AxisType.ZAXIS**: reports acceleration of an Inertial Sensor's **up to down** movements

`Inertial Acceleration` returns a decimal value that ranges from **-4.0 to 4.0** Gs.

## Example

The example below prints an Inertial Sensor's acceleration values to the VEX IQ Brain in a loop.

```python
# Set a smaller font to ensure lines fit when printed
brain.screen.set_font(FontType.MONO12)

while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)
    
    # X Axis
    brain.screen.print("X:", brain_inertial.acceleration(AxisType.XAXIS))
    brain.screen.next_row()
    
    # Y Axis
    brain.screen.print("Y:", brain_inertial.acceleration(AxisType.YAXIS))
    brain.screen.next_row()
    
    # Z Axis
    brain.screen.print("Z:", brain_inertial.acceleration(AxisType.ZAXIS))
    brain.screen.next_row()

    # Brief wait to prevent tearing when printing values
    wait(0.1, SECONDS)
```

<advanced>
</advanced>
