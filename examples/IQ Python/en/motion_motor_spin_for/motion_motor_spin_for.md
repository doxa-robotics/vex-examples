category: motion  
signature: motor.spin_for(FORWARD, 90, UNITS)  
description: Spins an IQ Motor or Motor Group for a given distance  

# Spin For
 
This command spins an IQ Motor or Motor Group for a given amount of degrees or turns.

```python
motor.spin_for(DIRECTION, AMOUNT, UNITS)
```

## How To Use

Choose which `DIRECTION` the Motor or Motor Group will spin to: **FORWARD** or **REVERSE**.

Choose the `UNIT` of measurement to be either **DEGREES** or **TURNS**.

Choose whether or not this command should be waited on by proceeding commands by setting an optional fourth parameter to either **wait=True** or **wait=False**. 

```python
motor.spin_for(FORWARD, 90, DEGREES, wait=False)
```

By default, this command is a blocking command unless **wait=False** is passed as the fourth parameter.

<advanced>
</advanced>
