category: events  
signature: bumper.pressed(callback)  
device_class: bumper  
description: Runs the specified function when a bumper is pressed  

# Bumper Pressed

Runs the specified **callback function** when a bumper is pressed.

```python
bumper.pressed(callback)
```

## How To Use

You will need to create a function to call when the Bumper Sensor is pressed. Provide the name of the function that should run when the event occurs as the **callback** parameter.

```python
def bumper_pressed():
    brain.screen.print("Bumper Pressed")
```

Then, the function is passed as the parameter of the `Bumper Pressed` function call.

```python
bumper.pressed(bumper_pressed)
```

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```python
def callback_function():
    brain.screen.print("Pressed")

bumper.pressed(callback_function)
```

<advanced>
</advanced>