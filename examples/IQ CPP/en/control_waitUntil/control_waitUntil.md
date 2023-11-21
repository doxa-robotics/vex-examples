category: control  
signature: control_waitUntil 
description: Waits for a condition to return true before moving to the next command.

# Wait Until

Repeats a segment of code until the provided **condition** returns **true**.

```cpp
while (!condition) { 
  // Code to repeat until condition returns true
}
```

## How To Use

This control statement will repeatedly check its condition, and will **not** execute any proceeding code until the condition returns **true**. At the same time, it will repeat any code provided between its curly braces.

```cpp
while (!TouchLED.pressing()) {
  wait(20, msec);
}
```

## Example 

This example will turn the TouchLED to Yellow and wait until the TouchLED is pressed. Once pressed, the TouchLED will then change to green.

```cpp
TouchLED.setColor(yellow);

while (!TouchLED.pressing()) {
  wait(1, seconds);
}

TouchLED.setColor(green);
```

<advanced>
</advanced>