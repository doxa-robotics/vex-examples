category: drivetrain
signature: Drivetrain.setTurnVelocity(50, percent);  
device_class: drivetrain  
description: Sets the velocity of the Drivetrain when turning. If this is used when the drivetrain is turning, the drivetrain will be updated with the new speed.  

# Set Turn Velocity

Sets the velocity of the Drivetrain when turning. 

If this is used when the drivetrain is turning, the drivetrain will be updated with the new speed.

```cpp
Drivetrain.setTurnVelocity(velocity, units);
```

## How To Use

`Drivetrain.setTurnVelocity` will set the speed of the Drivetrain when turning, but will not cause the Drivetrain to move when used by itself. 

`Drivetrain.setTurnVelocity` accepts a range from **-100 to 100** when using **percent** units.

`Drivetrain.setTurnVelocity` accepts a range from **-127 to 127** when using **rpm** units.

Setting a Drivetrain's turn velocity to a negative value will cause the Drivetrain to turn in the opposite direction.

Setting a Drivetrain's turn velocity to 0 will prevent the Drivetrain from turning.

## Example

This example will make the Drivetrain turn to the left at 25% speed.

```cpp
Drivetrain.setTurnVelocity(25, percent);
Drivetrain.turn(left);
```

<advanced>
</advanced>
