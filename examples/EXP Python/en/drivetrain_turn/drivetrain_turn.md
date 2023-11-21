category: drivetrain 
signature: drivetrain.turn(RIGHT)  
description: Turns the Drivetrain to the right or left.  

# Turn

Turns the Drivetrain to the right or left.

```don
drivetrain.turn(DIRECTION)
```

## How To Use

The `drivetrain.turn` command will rotate the Drivetrain in the given direction forever until a new drivetrain command is used, or until the program is stopped.

Use the `LEFT` argument in all-capital letters to turn the Drivetrain to the left.

```don
drivetrain.turn(LEFT)
```

Use the `RIGHT` argument in all-capital letters to turn the Drivetrain to the right.

```don
drivetrain.turn(RIGHT)
```

## Example

In this example, the robot will drive forward 200 MM before turning right indefinitely.

```don
drivetrain.drive_for(FORWARD, 200, MM)

drivetrain.turn(RIGHT)
```

<advanced>
</advanced>
