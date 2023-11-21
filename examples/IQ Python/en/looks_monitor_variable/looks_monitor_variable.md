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

This example will monitor a variable that increments every 0.5 seconds. It will also print the value to the console.

```don
counter = 0

def main():
    global counter
    monitor_variable("counter")
    while True:
        counter = counter + 1
        brain.screen.print(counter)
        brain.screen.next_row()
        wait(0.5, SECONDS)
```

<advanced>
</advanced>
