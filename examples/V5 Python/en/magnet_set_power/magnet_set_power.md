category: magnet  
signature: magnet.set_power(50)
description: Changes the power used by the V5 Electromagnet when picking up objects.

# Electromagnet set power

Changes the power used by the V5 Electromagnet when picking up an object.

```python
magnet.set_power(50)
```
The power can be set from **0% to 100%**.

## Example

This example will use `magnet.set_power()` to set the electromagnet to full power, pick up an object, drive forward, and then drop the object.

```python
magnet.set_power(100)
magnet.pickup()
drivetrain.drive_for(FORWARD, 200, MM)
magnet.drop()
```

<advanced>
</advanced>