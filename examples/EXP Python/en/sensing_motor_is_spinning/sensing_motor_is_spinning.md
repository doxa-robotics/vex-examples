category: sensing  
signature: motor.is_spinning()
description:  Reports if the selected EXP Smart Motor or Motor Group is currently spinning.

# Motor Is Spinning

Reports if the selected EXP Smart Motor or Motor Group is currently spinning.

```python
motor.is_spinning()
```

## How To Use

Motor is spinning reports **True** when the selected Motor or Motor Group is still moving.

Motor is spinning reports **False** when the selected Motor or Motor Group is stopped.

**Note:** This command will always return **false** if the Motor or Motor Group is spinning because of a `spin()` command.

<advanced>
</advanced>
