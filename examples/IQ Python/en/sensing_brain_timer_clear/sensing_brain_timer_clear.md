category: sensing  
signature: brain.timer.clear()  
description: Resets the IQ Brain's timer  

# Reset Timer

Resets the IQ Brain's timer.

```python 
brain.timer.clear()
```

## How To Use

The Brain's timer begins at the beginning of each project. The `Reset Timer` command can be used to reset the timer value back to 0 seconds.

## Example

In this example, the timer will be reset before moving the Drivetrain forward for 3 seconds. After 3 seconds has elapsed, the Drivetrain will stop.

```python
brain.timer.clear()
while brain.timer.time(SECONDS) <= 3:
    drivetrain.drive(FORWARD)
drivetrain.stop()
```
	
<advanced>
</advanced>
