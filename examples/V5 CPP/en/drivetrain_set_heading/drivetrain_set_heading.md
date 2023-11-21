category: drive  
signature: Drivetrain.setHeading(90, degrees);  
device_class: smartdrive  
description: Sets the Gyro of the Drivetrain to an exact heading.  

# Drivetrain Set Heading

Sets the Gyro of the Drivetrain to an exact heading.

```cpp
Drivetrain.setHeading(heading, degrees);
```

## How To Use

The `Drivetrain.setHeading();` command can be used to set the Drivetrain's position to any given heading. This command can be used to reset the orientation of the Drivetrain's Gyro when the heading is set to a value of 0.

`Drivetrain.setHeading();` accepts a range of **0 to 360** degrees.

```cpp
// Reset the Drivetrain heading to 0

Drivetrain.setHeading(0, degrees);
```

<advanced>
</advanced>