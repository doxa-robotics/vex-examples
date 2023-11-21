category: motion  
signature: MOTOR.setPosition(0, degrees);  
device_class: motor  
description: Sets the V5 Smart Motor or Motor Group's encoder(s) to a position.  

# Motor Set Position

Sets the V5 Smart Motor or Motor Group's encoder(s) to a specified position.

```cpp
Motor.setPosition(position, units);
```

## How To Use

The `Motor.setPosition();` command can be used to set the Motor or Motor Group's position to any given value.

The `Motor.setPosition();` command is typically used to set the position to 0 to reset the Motor or Motor Group's encoder(s) position.

Set the position of the Motor or Motor Group by providing the `position` to any number. 

You can specify the units of the value in either `degrees` or `turns`. 

```cpp
ArmMotor.setPosition(50, degrees);
```

<advanced>
</advanced>