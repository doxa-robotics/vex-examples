category: control  
signature: break  
description: Exits a repeating loop immediately.

# Break

Exits a repeating loop immediately.

```python
break
```

## How To Use

When added inside of a loop, the `break` command will exit the loop it is currently running inside of. 

## Example

This example will drive the robot and check if its `bumper` has been pressed.

If the bumper is **pressed**, the `break` command will exit the `while` loop. The robot will then stop driving forward.

```python
while True:
    drivetrain.drive(FORWARD)
    if bumper.pressing():
        break

drivetrain.stop()
```
<advanced>
</advanced>
