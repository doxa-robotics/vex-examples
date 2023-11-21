category: events  
signature: brain.screen.released(callback)  
description: Runs the callback function when the V5 Brain’s touchscreen is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

#  Brain Screen Released

Runs the callback function when the V5 Brain’s touchscreen is released.

```python
brain.screen.released(callback)
```

## How To Use

The `brain.screen.released()` command can be used to trigger actions or behaviors based on touch interaction with the V5 Brain's touchscreen. 

Used together with the `brain.screen.x_position()` and `brain.screen.y_position()` commands, users can create custom interfaces to their V5 Brain by detecting when and where touches occur on the screen.

You will need to create a function to call when the screen gets released. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```python
# Function to run when the event occurs
def run_on_event():
    brain.screen.print("Event has occurred")
  
# Register event with a callback function
brain.screen.released(run_on_event)
```


<advanced>
</advanced>