category: control  
signature: control_if_else
description: Runs the code inside the else-statement's curly brackets, if the if-statement's condition is false. This command must have an if-statement preceding for it to compile.  

# If/else

A control statement that runs the code inside the first or second set of curly brackets based on the Boolean value of the conditional.

```cpp
if (condition) {
  // Some code to run if the condition returns true
} else {
  // Some code to run if the condition returns false
}
```

## How To Use

The if/else statement will only check the Boolean condition once.

If the Boolean `(condition)` is reported as **true**, the code inside of `if's` curly brackets will run.

If the Boolean `(condition)` is **false**, the code inside of `else's` curly brackets will run.

## Example

In this example, the VEX IQ TouchLED will glow green if it is pressed and will glow red when it is not pressed.

An if/else conditional can be “nested” or placed inside a while loop to ensure that the Touch LED can turn red and green more than once.

```cpp
while (true) {
  if (TouchLED.pressing()) {
    TouchLED.setColor(green);
  } else {
    TouchLED.setColor(red);
  }

  wait(20, msec);
}
```

<advanced>
</advanced>