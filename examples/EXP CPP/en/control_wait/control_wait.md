category: control  
signature: wait(time, seconds);  
description: Waits for a specific amount of time before moving to the next command.

# Wait

Waits for a specific amount of time before moving to the next command.

```cpp
wait(time, seconds);
```

## How To Use

Set an amount of time in **seconds** to have your program **wait** before executing subsequent commands.

```cpp
// Wait for 5 seconds before driving forward
wait(5, seconds);
Drivetrain.drive(forward);
```

<advanced>
</advanced>