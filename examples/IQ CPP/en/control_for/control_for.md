category: control  
signature: control_for
description: A type of loop that repeats the code contained inside for a set number of iterations. 

# For

Repeats the code inside the curly braces for a set number of times.

```cpp
for (initialization; condition; increment/decrement) {
  // some code to repeat
}
```

## How To Use

Enter a value to indicate how many times the code will **repeat** using 3 expressions:

* initialization
* condition
* increment/decrement

**Initialization** declares the starting value of the iterating variable.

**Condition** specifies how long the for loop will run. The loop will stop repeating when the condition becomes **false**.

**Increment/decrement** changes the iterating variable at the end of each loop.

## Example 1

This example will print the numbers 0 to 9 to the VEX IQ Brain's screen.

```cpp
for (int i = 0; i < 10; i++) {
  Brain.Screen.print("%d", i);
  wait(20, msec);
}
```
## Example 2

This example will drive the VEX IQ robot forward ten inches then turn the robot 60 degrees three times to the right. 

```cpp
Drivetrain.driveFor(forward, 10.0, inches);

for (int i = 0; i < 3; i++) {
  Drivetrain.turnFor(right, 60, degrees);
  wait(20, msec);
}
```

<advanced>
</advanced>