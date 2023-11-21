category: events  
signature: controller.button.released(callback)  
description: Runs the callback function when the VEX IQ Controller button is released  

# Controller Button Released

Runs the **callback function** when the VEX IQ Controller button is released.

```python
controller.button.released(callback)
```

## How To Use

You will need to create a **callback function** that will be called when a Controller button is released.

Choose which Controller button to call the `Controller Button Released` function with:

* `buttonEUp`
* `buttonEDown`
* `buttonFUp`
* `buttonFDown`
* `buttonLUp`
* `buttonLDown`
* `buttonRUp`
* `buttonRDown`
* `buttonL3`
* `buttonR3`

## Example

The example below prints to the IQ Brain's screen when the Controller's L3 button is released.

```python
def button_released():
    brain.screen.print("Button released")
    
controller.buttonL3.released(button_released)
```

<advanced>
</advanced>