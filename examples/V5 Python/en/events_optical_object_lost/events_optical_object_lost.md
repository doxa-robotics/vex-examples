category: events  
signature: optical.object_lost(callback)   
device_class: optical  
description: Runs the callback function when an object is no longer being detected by a V5 Optical Sensor  

# Optical Object Lost

Runs the callback function when an object is no longer being detected by a V5 Optical Sensor.

```python
optical.object_lost(callback)
```

## How To Use

The `optical.object_lost` command can be used to trigger actions or behaviors when an object is no longer being detected by a V5 Optical Sensor.

You will need to create a function to call when an object is no longer being detected. Provide the name of the function that should run when the event occurs as the **callback** parameter.

```python
# Function to run when the event occurs
def run_on_object_lost():
    brain.screen.print("Object lost!")

# Register an event with a callback function
optical.object_lost(run_on_object_lost)
```

<advanced>
</advanced>







