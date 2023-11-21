category: sensing  
signature: brain.timer.time(UNITS)  
description: Reports the value of the EXP Brain's timer in the provided UNITS.

# Timer Value

Reports the value of the EXP Brain's timer in the provided UNITS.

```python
brain.timer.time(UNITS)
```

## How To Use

The timer starts at 0 seconds when the program starts, and reports the timer's value as a decimal value.

The `UNITS` parameter accepts either **SECONDS** or **MSEC** (milliseconds) as a valid argument.

```python
while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)
    brain.screen.print("Timer in Seconds: ", brain.timer.time(SECONDS))

    # A brief wait to print values without distortion or tearing
    wait(20, MSEC)
```
	
<advanced>
</advanced>
