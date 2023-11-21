category: Events
signature: `Controller.AxisA.changed(callback)`  
device_class: Controller
description: Runs callback funtion when the selected VEX IQ Controller joystick axis is moved.

# Controller Axis Changed

Runs the provided callback funtion when the selected VEX IQ Controller's joystick axis is moved.

```cpp
Controller.Axis.changed(callback);
```

## How To Use

You will need to create a callback function to call when an Axis on the controller is moved.

```cpp
void axisMoved() {
  Brain.Screen.print("Axis moved.");
}
```

Choose which Controller joystick axis to use and pass the callback function

- `Controller.AxisA.changed(axisMoved);`
- `Controller.AxisB.changed(axisMoved);`
- `Controller.AxisC.changed(axisMoved);`
- `Controller.AxisD.changed(axisMoved);`

![controller_button_front](controller_button_front.jpg)

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Controller.AxisA.changed(callbackFunction);
}
```

<advanced>
</advanced>