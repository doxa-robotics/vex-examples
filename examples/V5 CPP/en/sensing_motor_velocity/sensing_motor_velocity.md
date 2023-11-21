category: sensing  
signature: MOTOR.velocity()  
device_class: motor  
description: Reports the current velocity of the V5 Smart Motor or Motor Group.  

# Motor Velocity

Reports the current velocity of a V5 Smart Motor or the first motor of a Motor Group.

```cpp
Motor.velocity(percent)
```

## How to Use

`Motor.velocity()` returns a decimal value (as a *double*) to report the current velocity of a Motor or the first motor of a Motor Group. 

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

Specify the unit when using this command. The two unit options are:

`percent` - will return a value from **-100% to 100%**.
 
```cpp
Brain.Screen.print("%f", ArmMotor.velocity(percent));
```
  
`Motor.velocity()` will return a `rpm` (rotations per minute) range based on the Gear Cartridge installed in a V5 Smart Motor or the first motor of a Motor Group.

**Red Cartridge:** -100rpm to 100rpm  
**Green Cartridge:** -200rpm to 200rpm  
**Blue Cartridge:** -600rpm to 600rpm  

```cpp
Brain.Screen.print("%f", ArmMotor.velocity(rpm));
``` 
<advanced>
</advanced>