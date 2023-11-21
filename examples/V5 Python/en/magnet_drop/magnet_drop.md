category: magnet  
signature: magnet.drop() 
description: Allows the V5 Electromagnet to drop the object it is currently holding.  


# Electromagnet drop

Allows the V5 Electromagnet to drop the object it is currently holding.

```python
magnet.drop()
```
After using the `magnet.drop()` command, the magnet will need to cool down before it can be used again.

## Example
This example will pickup an object, drive forward, then use `magnet.drop()` to drop the object.

```python
magnet.pickup()
drivetrain.drive_for(FORWARD, 200, MM)
magnet.drop()
```

<advanced>
</advanced>