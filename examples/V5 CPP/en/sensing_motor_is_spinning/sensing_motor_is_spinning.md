category: sensing  
signature: MOTOR.isSpinning()  
device_class: motor  
description: Reports if the selected V5 Smart Motor or Motor Group is currently spinning.

# Motor Is Spinning

Reports if the selected V5 Smart Motor or Motor Group is currently spinning.

```cpp
Motor.isSpinning()
```

## How To Use

Commands that return a value are normally used inside of other statements (such as print statements) or inside of control structures (such as while loops) and do not use a semicolon.

This command returns **true** if the Motor or Motor Group is moving because of a `spinFor()` command that *does* specify a set distance.

This command returns **false** if the Motor or Motor Group movement has completed.

**Note:** This command will always return **false** if the Motor or Motor Group is moving because of a `spin()` command that does *not* specify a set distance.

```cpp
// The example below flashes an LED while the V5 Arm is being raised or lowered

ArmMotor.spinFor(forward, 720, degrees, false);

while (ArmMotor.isSpinning()) {
    LEDA.on();
    wait(0.5, seconds);
    LEDA.off();
    wait(0.5, seconds);
}
```
<advanced>
</advanced>