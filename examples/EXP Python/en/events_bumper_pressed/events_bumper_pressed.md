category: events  
signature: bumper.pressed(callback)  
device_class: bumper  
description: Runs the specified function when the bumper is pressed.  

# Bumper Pressed

Runs the specified function when the bumper is pressed.

```python
bumper.pressed(callback)
```

## How To Use

You will need to create a function to call when the Bumper Sensor is pressed. 

Provide the name of the function that should run when the event occurs as the `callback` parameter.

```python
# Function to run when the event occurs
def run_on_bumper_pressed():
    brain.screen.print("Bumper pressed!")
 
# Register event with a callback function
bumper_a.pressed(run_on_bumper_pressed)
```

<advanced>
</advanced>