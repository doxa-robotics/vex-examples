category: events  
signature: controller.button.pressed(callback)  
description: Runs the callback function when the VEX IQ Controller button is pressed  

# Controller Button Pressed

Runs the **callback function** when the VEX IQ Controller button is pressed.

```python
controller.button.pressed(callback)
```

## How To Use

You will need to create a **callback function** that will be called when a Controller button is pressed.

Choose which Controller button to call the `Controller Button Pressed` function with:

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

The example below prints to the IQ Brain's screen when the Controller's L3 button is pressed.

```python
def button_pressed():
    brain.screen.print("Button pressed")
    
controller.buttonL3.pressed(button_pressed)
```

<advanced>
</advanced>