category: sensing  
signature: Drivetrain.isDone()  
device_class: drivetrain  
description: Reports if the Drivetrain has completed its movement.

# Drivetrain Is Done

Reports if the Drivetrain has completed its movement.

```cpp
Drivetrain.isDone()
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

`Drivetrain.isDone()` reports **true** when the Drivetrain's motors have completed their movement.

`Drivetrain.isDone()` reports **false** when the Drivetrain's motors are still moving.

```cpp
waitUntil(Drivetrain.isDone());
```

This command returns **true** if the drivetrain is moving because of a `drive()` or `turn()` command.

<advanced>
</advanced>