category: drivetrain  
signature: drivetrain.stop()  
description: Stops the Drivetrain.  

# Stop

Stops the Drivetrain.

```don
drivetrain.stop()
```

## How To Use

The `drivetrain.stop()` command stops the Drivetrain. It does not take any arguments in its parentheses.

## Example

This example will stop the Drivetrain after the V5 Robot has driven forward for 3 seconds.

```don
drivetrain.drive(FORWARD)
wait(3, SECONDS)
drivetrain.stop()
```

<advanced>
</advanced>
