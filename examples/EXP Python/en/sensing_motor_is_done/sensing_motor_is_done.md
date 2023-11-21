category: sensing  
signature: motor.is_done()
description:  Reports if the selected EXP Smart Motor or Motor Group has completed its movement.

# Motor Is Done 

Reports if the selected EXP Smart Motor or Motor Group has completed its movement.

```python
motor.is_done()
```

## How To Use

Motor is done reports **True** when the selected Motor or Motor Group has completed its movement.

Motor is done reports **False** when the selected Motor or Motor Group is still moving.

**Note:** This command will always return **true** if the Motor or Motor Group is spinning because of a `spin()` command.


<advanced>
</advanced>
