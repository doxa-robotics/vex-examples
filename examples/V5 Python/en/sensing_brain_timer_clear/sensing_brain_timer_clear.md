category: sensing  
signature: brain.timer.clear()  
description: Clears the V5 Brain's timer.

# Reset Timer
Resets the V5 Brain's timer.

```don 
brain.timer.clear()
```

## How To Use

The Brain's timer begins at the beginning of each project. The clear timer command is reset the timer value back to 0 seconds.

## Example

In this example, the timer will be reset before moving the Drivetrain forward for 3 seconds. After 3 seconds has elapsed, the Drivetrain will stop.

```don
brain.timer.clear()
while not brain.timer.time(SECONDS) > 3:
    drivetrain.drive(FORWARD)
drivetrain.stop()
```
	
<advanced>
</advanced>
