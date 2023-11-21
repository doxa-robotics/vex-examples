category: drivetrain  
signature: drivetrain.stop()  
description: Stops the Drivetrain  

# Stop

Stops the Drivetrain.

```python
drivetrain.stop()
```

## How To Use

The `Stop` command stops the Drivetrain. It does not take any arguments in its parentheses.

## Example

This example will stop the Drivetrain after the IQ Robot has driven forward for 3 seconds.

```python
drivetrain.drive(FORWARD)
wait(3, SECONDS)
drivetrain.stop()
```

<advanced>
</advanced>
