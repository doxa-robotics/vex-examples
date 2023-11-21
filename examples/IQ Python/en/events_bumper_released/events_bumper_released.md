category: events  
signature: bumper.released(callback)  
device_class: bumper  
description: Runs the specified function when a bumper is released  

# Bumper Released

Runs the specified function when a bumper is released.

```python
bumper.released(callback)
```

## How To Use

Create a function to call when the Bumper is released. Provide the name of the function that should run when the event occurs as the **callback** parameter.

```python
def bumper_released():
    brain.screen.print("Bumper released")
```

Then, the function is passed as the parameter of the `Bumper Released` function call.

```python
bumper.released(bumper_released)
```

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```python
def callback_function():
    brain.screen.print("Released")

bumper.released(callback_function)
```

<advanced>
</advanced>