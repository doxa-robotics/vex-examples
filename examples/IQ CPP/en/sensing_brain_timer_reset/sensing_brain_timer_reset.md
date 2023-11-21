category: sensing  
signature: sensing_brain_timer_reset 
description: Resets the Brain's timer.

# Reset Timer

Resets the VEX IQ Brain's timer.

```cpp
Brain.Timer.reset();
```

## How To Use

The Brain's timer begins at the start of running a program. `Brain.Timer.reset` is used to reset the timer back to 0 seconds.

## Example

In this example, the timer will be reset before moving the Drivetrain forward for 3 seconds. After 3 seconds has elapsed, the Drivetrain will stop.

```cpp
Brain.Timer.reset();
Drivetrain.drive(forward);

while (true) {
  if (Brain.Timer.value() > 3) {
    break;
  }

  wait(20, msec);
}

Drivetrain.stop();
```

<advanced>
</advanced>