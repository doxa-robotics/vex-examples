category: events  
signature: optical.object_detected(callback)   
device_class: optical  
description: Runs the callback function when an object is detected by an Optical Sensor  

# Optical Object Detected

Runs the callback function when an object is detected by an Optical Sensor.

```python
optical.object_detected(callback)
```

## How To Use

The `optical.object_detected` command can be used to trigger actions or behaviors when an object is detected by an Optical Sensor.

You will need to create a function to call when an object is detected. Provide the name of the function that should run when the event occurs as the **callback** parameter.

```python
# Function to run when the event occurs
def run_on_object_detected():
    brain.screen.print("Object detected!")

# Register an event with a callback function
optical.object_detected(run_on_object_detected)
```

<advanced>
</advanced>







