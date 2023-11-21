category: sensing  
signature: sensing_brain_timer_value
description: Reports the VEX IQ Brain's timer value in seconds. 

# Timer Value

Reports the value of the VEX IQ Brain's timer in seconds.

```cpp
Brain.Timer.value()
```

## How To Use

The Brain's timer starts at 0 seconds when the program starts, and returns the timer's value as a decimal value (as a *double*).

## Example

The example below prints the value of the Brain's timer.

```cpp
while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Timer: %.2f", Brain.Timer.value());
  
  // Brief delay to prevent distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>