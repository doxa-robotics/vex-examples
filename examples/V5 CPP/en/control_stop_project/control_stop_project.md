category: control  
signature: vexSystemExitRequest();  
description: Stops a running project.  

# Stop Project

Stops a running project.

```cpp
vexSystemExitRequest();
```

## How To Use

The `Stop Project` command can be used to programmatically stop an actively running project.

## Example

The example below will drive a V5 Robot forward 200mm and turn right for 90 degrees before stopping the project.

```cpp
Drivetrain.driveFor(forward, 200, mm);
Drivetrain.turnFor(right, 90, degrees);
vexSystemExitRequest();
```

<advanced>
</advanced>