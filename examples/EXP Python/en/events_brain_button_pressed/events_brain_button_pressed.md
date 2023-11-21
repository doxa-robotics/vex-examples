category: events  
signature: brain.button.pressed(callback)  
description: Runs the callback function when one of the VEX EXP Brain's buttons is pressed  

# Brain Button Pressed

Runs the callback function when one of the VEX EXP Brain's buttons is pressed.

```python
brain.button.pressed(callback)
```

## How To Use

You will need to create a function to call when a Brain Button is pressed.

```python
def button_pressed():
    brain.screen.print("Button pressed")
```

The `Brain Button Pressed` function can be used with the different buttons on the VEX EXP Brain.

Supported Brain buttons are as follows:

- `buttonLeft`
- `buttonRight`
- `buttonCheck`

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```python
def callback_function():
    brain.screen.print("Pressed")

brain.buttonCheck.pressed(callback_function)
```

<advanced>
</advanced>