category: control  
signature: while(true) { }  
description: A loop that repeats the code inside the curly brackets while the condition returns true. 

# While
A loop that repeats the code inside the curly brackets while the condition evaluates as **true**.   

```cpp
while (condition) {

}
```

## How To Use

The `while` loop will only check condition inside the parenthesis at the beginning of each loop. 

If the condition evaluates as **true**, the code inside of `while` will run.

If the condition evaluates as **false**, the code inside of `while` will be skipped.

The `while` loop accepts anything that evaluates to true or false as its condition. You can place Booleans, and expressions using comparison and logical operators. You can also put numbers; **0** evaluates to **false**, and any **non-zero numbers** evaluates to **true**. 

```cpp
// Drive forward while the timer value is less than 10 seconds

while(Brain.Timer.time(seconds) < 10) {
  Drivetrain.drive(forward);
}

Drivetrain.stop();
```

<advanced>
</advanced>