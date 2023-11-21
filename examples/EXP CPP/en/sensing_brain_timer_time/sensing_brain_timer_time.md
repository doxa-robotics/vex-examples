category: sensing  
signature: Brain.Timer.time(units)
description: Reports the value of the EXP Brain's timer in the provided units  

# Brain Timer Time

Reports the value of the EXP Brain's timer in the provided units.

```cpp
Brain.Timer.time(units)
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not require a semicolon.

The timer starts at 0 seconds when the program starts, and returns the timer's value as a decimal value (as a *double*).

The `units` parameter accepts either **seconds** or **msec** (milliseconds) as a valid argument.

```cpp
if(Brain.Timer.time(seconds) > 3.0){
  Brain.Screen.print("Timer has passed 3 seconds!");
}
```

<advanced>
</advanced>