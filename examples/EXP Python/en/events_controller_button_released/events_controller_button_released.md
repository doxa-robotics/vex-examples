category: events  
signature: controller.button.released(callback)  
device_class: controller  
description: Runs the specified function when the controller button is released.  

# Controller Button Released

Runs the specified function when the controller button is released.

```python
controller.button.released(callback)
```

## How To Use

Choose which Controller Button to monitor.

* `buttonA`
* `buttonB`
* `buttonUp`
* `buttonDown`
* `buttonL1`
* `buttonL2`
* `buttonL3`
* `buttonR1`
* `buttonR2`
* `buttonR3`

You will need to create a function to call when the Controller Button is released. 

Provide the name of the function that should run when the event occurs as the `callback` parameter.

```python
# Function to run when the event occurs
def run_on_button_released():
    brain.screen.print("Button released!")

# Register event with a callback function.
controller_1.buttonA.released(run_on_button_released)
```

<advanced>
</advanced>