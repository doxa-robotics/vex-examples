category: looks  
signature: Brain.Screen.clearScreen();  
description: Clears the entire V5 Brain screen.  

# Clear Screen

Clears the entire VEX IQ Brain's Screen.

```cpp
Brain.Screen.clearScreen();
```

## How To Use

`Brain.Screen.clearScreen` will not reset the Brain's screen cursor. 

Use the `Brain.Screen.setCursor` command to set the Brain's cursor to the desired position.

## Example

This example will print "Hello", wait one second, and then clear the entire screen before printing "Goodbye".

```cpp
Brain.Screen.print("Hello");
wait(1.0, seconds);
Brain.Screen.clearScreen();
Brain.Screen.print("Goodbye");
```

<advanced>
</advanced>