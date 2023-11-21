category: control  
signature: while(true) { }  
description: A loop that repeats the code inside the curly brackets while the condition returns true. 

# While

A loop that repeats the code inside its curly brackets while the **condition** provided evaluates to **true**. 

```cpp
while (condition) {

}
```

## How To Use

The `while` loop will only check the condition inside the rounded parenthesis at the beginning of each loop. 

If the condition evaluates as **true**, the code inside of `while` will run.

If the condition evaluates as **false**, the code inside of `while` will be skipped.

The `while` loop accepts anything that evaluates to **true** or **false** as its condition. Conditions can be Booleans or expressions using comparison or logical operators.  

```cpp
// Drive forward while the timer value is less than 10 seconds

while(Brain.Timer.time(seconds) < 10) {
  Drivetrain.drive(forward);
}

Drivetrain.stop();
```
## Example

This example will drive the robot forward while the timer value is less than 60 seconds.

After 60 seconds, the robot will stop.

```cpp
while(Brain.Timer.value() < 60) {
  Drivetrain.drive(forward);
  wait(20, msec);
}

Drivetrain.stop();
```

<advanced>
</advanced>