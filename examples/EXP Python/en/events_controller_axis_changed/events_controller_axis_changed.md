category: events  
signature: controller.axis.changed(callback)  
device_class: controller  
description: Runs the specified function when the controller axis value changes.  

# Controller Axis Changed

Runs the specified function when the controller axis position changes.

```python
controller.axis.changed(callback)
```

## How To Use

Choose which Controller axis to monitor.

* `axis1`
* `axis2`
* `axis3`
* `axis4`

You will need to create a function to call when the Controller Axis position is changed. 

Provide the name of the function that should run when the event occurs as the `callback` parameter.

```python
# Function to run when the event occurs
def run_on_axis_changed():
    brain.screen.print("Axis changed!")

  
# Register event with a callback function.
controller_1.axis1.changed(run_on_axis_changed)
```

<advanced>
</advanced>