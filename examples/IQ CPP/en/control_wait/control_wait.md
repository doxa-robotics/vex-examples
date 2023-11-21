category: control  
signature: wait(time, units);  
description: Waits for a specific amount of time before moving to the next command.  

# Wait

Waits for a specific amount of time before moving to the next command.

```cpp
wait(time, units);
```

## How To Use

Set an amount of time in **seconds** or **msec** (milliseconds) to have your program `wait` before executing additional commands.

```cpp
wait(10, seconds);
wait(100, msec);
```

<advanced>
</advanced>