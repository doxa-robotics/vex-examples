category: events  
signature: bumper.released(callback)  
device_class: bumper  
description: Runs the specified function when the bumper is released.  

# Bumper Released

Runs the specified function when the bumper is released.

```python
bumper.released(callback)
```

## How To Use

You will need to create a function to call when the Bumper Sensor is released. 

Provide the name of the function that should run when the event occurs as the `callback` parameter.

```python
# Function to run when the event occurs
def run_on_bumper_released():
    brain.screen.print("Bumper released!")
 
# Register event with a callback function
bumper_a.released(run_on_bumper_released)
```

<advanced>
</advanced>