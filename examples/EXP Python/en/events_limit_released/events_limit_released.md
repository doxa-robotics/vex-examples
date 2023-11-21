category: events  
signature: limit.released(callback)  
device_class: limit  
description: Runs the specified function when the Limit Switch is released.  

# Limit Released

Runs the specified function when the Limit Switch is released.

```python
limit.released(callback)
```

## How To Use

You will need to create a function to call when the Limit Switch is released. 

Provide the name of the function that should run when the event occurs as the `callback` parameter.

```python
# Function to run when the event occurs
def run_on_limit_released():
    brain.screen.print("Limit released!")
 
# Register event with a callback function
limit_a.released(run_on_limit_released)
```

<advanced>
</advanced>