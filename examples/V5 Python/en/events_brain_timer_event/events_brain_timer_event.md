category: events  
signature: brain.timer.event(callback, 1000)
description: Runs the specified function when the V5 Brain's timer is greater than the given value.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Brain Timer Event

Runs the specified callback function when the V5 Brain's timer is greater than the given value.

```python
brain.timer.event(callback, 1000)
```

## How To Use

The V5 Brain's timer begins at the beginning of each project.

Specify the amount of time. The `brain.timer.event()` event will run once the V5 Brain's timer is **greater than** the entered amount.

The `brain.timer.event()` command can accept integer values for the number of milliseconds.

You will need to create a function to call when the timer is greater than the entered amount. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```python
# Function to run when the event occurs
def run_on_event():
    brain.screen.print("Event has occurred")
  
# Register event with a callback function
brain.timer.event(run_on_event, 2000)
```


<advanced>
</advanced>