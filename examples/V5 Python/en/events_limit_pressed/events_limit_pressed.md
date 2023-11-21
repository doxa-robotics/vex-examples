category: events  
signature: limit.pressed(callback)  
device_class: limit  
description: Runs the specified function when the Limit Switch is pressed.  

# Limit Pressed

Runs the specified function when the Limit Switch is pressed.

```python
limit.pressed(callback)
```

## How To Use

You will need to create a function to call when the Limit Switch is pressed. 

Provide the name of the function that should run when the event occurs as the `callback` parameter.

```python
# Function to run when the event occurs
def run_on_limit_pressed():
    brain.screen.print("Limit pressed!")
 
# Register event with a callback function
limit_a.pressed(run_on_limit_pressed)
```

<advanced>
</advanced>