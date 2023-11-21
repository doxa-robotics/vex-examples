category: events  
signature: brain.button.released(callback)  
description: Runs the callback function when one of the VEX EXP Brain's buttons is released  

# Brain Button Released

Runs the callback function when one of the VEX EXP Brain's buttons is released.

```python
brain.button.released(callback)
```

## How To Use

You will need to create a function to call when a Brain Button is released.

```python
def button_released():
    brain.screen.print("Button released")
```

The `Brain Button Released` function can be used with the different buttons on the VEX EXP Brain.

Supported Brain buttons are as follows:

- `buttonLeft`
- `buttonRight`
- `buttonCheck`

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```python
def callback_function():
    brain.screen.print("Released")

brain.buttonCheck.released(callback_function)
```

<advanced>
</advanced>