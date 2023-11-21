category: drivetrain 
signature: drivetrain.turn(RIGHT)  
description: Turns the Drivetrain to the right or left  

# Turn

Turns the Drivetrain to the right or left indefinitely.

```python
drivetrain.turn(DIRECTION)
```

## How To Use

The `Turn` command will rotate the Drivetrain in the given direction forever until a new Drivetrain command is used, or until the program is stopped.

Use the `LEFT` argument in all-capital letters to turn the Drivetrain to the left.

```python
drivetrain.turn(LEFT)
```

Use the `RIGHT` argument in all-capital letters to turn the Drivetrain to the right.

```python
drivetrain.turn(RIGHT)
```

## Example

In this example, the robot will drive forward 200 MM before turning right indefinitely.

```python
drivetrain.drive_for(FORWARD, 200, MM)
drivetrain.turn(RIGHT)
```

<advanced>
</advanced>
