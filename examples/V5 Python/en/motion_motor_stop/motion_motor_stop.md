category: motion  
signature: motor.stop()  
description: Stops a V5 Smart Motor or Motor Group.

# Stop Motor

Stops a V5 Smart Motor or Motor Group.

```python
motor.stop()
```

## Example

This example shows a motor spinning for 3 seconds before stopping.

```python
motor.spin(FORWARD)
wait(3, SECONDS)
motor.stop()
```

<advanced>
</advanced>
