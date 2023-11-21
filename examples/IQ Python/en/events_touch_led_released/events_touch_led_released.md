category: events  
signature: touchled.released(callback)  
device_class: touchled  
description: Runs the specified callback function when an IQ Touch LED is released  

# TouchLED Released

Runs the specified **callback function** when an IQ TouchLED is released.

```python
touchled.released(callback)
```

## How To Use

You will need to create a function to call when the TouchLED is released. Provide the name of the function that should run when the event occurs as the **callback** parameter.

```python
def touchled_released():
    brain.screen.print("Touch LED released")
```

Then, the function is passed as the parameter of the `TouchLED Released` function call.

```python
touchled.released(touchled_released)
```

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```python
def callback_function():
    brain.screen.print("Released")

touchled.released(callback_function)
```

<advanced>
</advanced>