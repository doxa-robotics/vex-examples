category: sensing  
signature: BUMPER.pressing()  
device_class: bumper  
description: Reports if the Bumper Switch is pressed.

# Bumper Pressing

Reports if the Bumper Switch is pressed.

```cpp
Bumper.pressing()
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Bumper.pressing()` returns **true** if the Bumper Switch is being pressed.

`Bumper.pressing()` returns **false** if the Bumper Switch is not pressed.

```cpp
waitUntil(BumperA.pressing());
Brain.Screen.print("BumperA pressed!");
```
<advanced>
</advanced>