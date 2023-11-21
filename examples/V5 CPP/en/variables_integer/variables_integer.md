category: variables 
signature: variables_intergers
description: Sets a variable to a `int` type.

# Integer Variable

Sets an integer variable with a declared name and value.

`int myNumber = 10;`

## How To Use

Create a unique and descriptive variable name.

`int driveTime = 60;`

Assign a value to your variable. A variable can equal the returned value of a sensing command or the result of an equation, as long as it is declared using the correct **type**.

```cpp
int lowBatteryLifeWarning = Brain.Battery.capacity(percent);
```


## Example

This example will assign the distance (in inches) detected by the VEX V5 Distance Sensor to the "myVariable" variable and use the value of "myVariable" to set the speed of the Drivetrain.

```cpp
int myVariable = Distance7.objectDistance(inches);

Drivetrain.setDriveVelocity(myVariable, percent);
```

<advanced>
</advanced>