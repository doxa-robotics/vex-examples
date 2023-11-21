category: sensing  
signature: gps.changed(callback)  
description: Runs the specified callback function when a GPS Sensor detects a heading change.  

# GPS When Heading Changed

Runs the specified callback function when a GPS Sensor detects a heading change.

```python
gps.changed(callback)
```

## How To Use

You will need to define a function to call when the GPS Sensor detects a heading change.

Provide the name of the defined function that should run when the event occurs as the `callback` parameter.

```python
# Function to run when the event occurs
def run_on_heading_change():
    brain.screen.print("GPS Heading Change Detected")

# Register event with a callback function
gps.changed(run_on_heading_change)
```

<advanced>
</advanced>
