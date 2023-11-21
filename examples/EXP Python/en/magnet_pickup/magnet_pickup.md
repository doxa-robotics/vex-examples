category: magnet  
signature: magnet.pickup() 
description: Allows the Electromagnet to pickup an object.

# Electromagnet pickup

Allows the Electromagnet to pick up an object.

```python
magnet.pickup()
```
After using the `magnet.pickup()` command, the magnet will need to cool down before it can be used again.

## Example
This example will use `magnet.pickup()` to pick up an object, drive forward, and then drop the object.

```python
magnet.pickup()
drivetrain.drive_for(FORWARD, 200, MM)
magnet.drop()
```

<advanced>
</advanced>