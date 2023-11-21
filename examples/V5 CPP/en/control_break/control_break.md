category: control  
signature: break;  
description: Exits a repeating loop immediately.

# Break

Exits a repeating loop immediately.

```cpp
break;
```

## How To Use

When added inside of a loop, the `break;` command will exit the loop it is currently running inside of. 

## Example

This example will move the Drivetrain forward and check if the V5 Brain’s screen has been pressed. 

If the screen is **pressed**, the `break;` command will exit the while loop and stop the Drivetrain.

```cpp
while (true) {
  Drivetrain.drive(forward);
  if(Brain.Screen.pressing()) {
    break;
  }
}

Drivetrain.stop();
```
<advanced>
</advanced>