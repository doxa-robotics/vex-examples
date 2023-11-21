category: looks  
signature: monitor_variable()
description: The monitor_variable function is used to add variables to the monitor console.

# Monitor Variable

The `monitor_variable()` command is used to add variables to the monitor console so that the value of the variables can be monitored.

```don
monitor_variable("my_variable", "my_boolean", ...)
```

## How To Use

To add variables to the monitor console, use the `monitor_variable()` command. Add the name of the variable(s) as strings in the command. Only global variables can be monitored with the `monitor_variable()` command.

## Examples

In this project, the robot will score 20 points by picking up the Yellow Mobile Goal and dropping it off in the Alliance Home Zone.

- Starting Position: A
- Orientation: Facing Yellow Mobile Goal
- Preload: Zero Rings

```don
spin_amount = 0

def main():
    global spin_amount
    monitor_variable("spin_amount")

    # Set the spin_amount variable to 1000
    spin_amount = 1000

    # Spin the Fork Motor Group down for 1700 degrees
    fork_motor_group.spin_for(FORWARD, 1700, DEGREES)
    drivetrain.drive_for(FORWARD, 1300, MM)

    # Pick up the Mobile Goal by spinning 
    # the Fork Motor Group up for spin_amount (1000)
    fork_motor_group.spin_for(REVERSE, spin_amount, DEGREES)
    drivetrain.drive_for(REVERSE, 900, MM)

    # Drop off the Mobile Goal by spinning
    # the Fork Motor Group up for spin_amount (1000)
    fork_motor_group.spin_for(FORWARD, spin_amount, DEGREES)
    drivetrain.drive_for(REVERSE, 300, MM)

    # Update the spin_amount by 700 (1000 + 700 = 1700)
    spin_amount = spin_amount + 700

    # Spin the Fork Motor Group up for spin_amount (1700) 
    fork_motor_group.spin_for(REVERSE, spin_amount, DEGREES)


main()
```

<advanced>
</advanced>
