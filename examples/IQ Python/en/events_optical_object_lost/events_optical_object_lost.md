category: events  
signature: optical.object_lost(callback)  
device_class: optical  
description: Runs the callback function when a detected object is no longer being detected by an Optical Sensor  

# Optical Object Lost

Runs the callback function when a detected object is no longer being detected by an Optical Sensor.

```python
optical.object_lost(callback)
```

## How To Use

The `Optical Object Lost` command can be used to trigger actions or behaviors when an Optical Sensor no longer detects a previously-detected object.

You will need to create a function to call when the object is no longer being detected. Provide the name of the function that should run when the event occurs as the **callback** parameter.

```python
# Function to run when the event occurs
def run_on_event():
    brain.screen.print("Object lost!")

# Register event with a callback function
optical.object_lost(run_on_event)
```

<advanced>
</advanced>







