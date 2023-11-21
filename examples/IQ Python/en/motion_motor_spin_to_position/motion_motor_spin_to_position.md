category: motion  
signature: motor.spin_to_position(POSITION, UNITS)
description: Spins an IQ Motor or Motor Group to a given position  

# Spin To Position

Spins an IQ Motor or Motor Group to a given position.

```python 
motor.spin_to_position(POSITION, UNITS)
```

## How To Use

This command will tell a Motor or Motor Group to travel to a specific position. Based on the current position of the Motor or Motor Group, `Spin To Position` will determine the direction to rotate the Motor or Motor Group.

Choose the unit of measurement to be either **DEGREES** or **TURNS**.

Choose whether or not this command should be waited on by other commands by changing the optional third parameter to either **wait=True** or **wait=False**.

```python
motor.spin_to_position(90, DEGREES, wait=False)
```

Setting **wait=True** means that proceeding commands will not execute until the motor spin is completed. Conversely, **wait=False** will not wait for it to be completed.  

By default, this command will have the wait to be set to **True**.

<advanced>
</advanced>
