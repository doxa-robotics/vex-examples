category: Events
signature: `controller.axis.changed(callback) 
device_class: controller
description: Runs a callback function when the selected VEX IQ Controller joystick axis is moved  

# Controller Axis Changed

Runs the provided callback funtion when the selected VEX IQ Controller's joystick axis is moved.

```python
controller.axis.changed(callback)
```

## How To Use

You will need to create a callback function to call when a joystick axis on the Controller is moved.

Choose which Controller joystick axis to use and pass the callback function:

- `axisA`
- `axisB`
- `axisC`
- `axisD`

![controller_button_front](controller_button_front.jpg)

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```python
def callback_function():
    brain.screen.print("Changed")

controller.axisA.changed(callbackFunction)
```

<advanced>
</advanced>