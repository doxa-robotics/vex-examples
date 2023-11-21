category: events  
signature: touchled.pressed(callback)  
device_class: touchled  
description: Runs the specified callback function when an IQ TouchLED is pressed  

# TouchLED Pressed

Runs the specified **callback function** when an IQ TouchLED is pressed.

```python
touchled.pressed(callback)
```

## How To Use

You will need to create a function to call when the TouchLED is pressed. Provide the name of the function that should run when the event occurs as the **callback** parameter.

```python
def touchled_pressed():
    brain.screen.print("Touch LED pressed")
```

Then, the function is passed as the parameter of the `TouchLED Pressed` function call.

```python
touchled.pressed(touchled_pressed)
```

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```python
def callback_function():
    brain.screen.print("Pressed")

touchled.pressed(callback_function)
```

<advanced>
</advanced>