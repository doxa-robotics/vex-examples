category: events  
signature: CONTROLLER.AXIS.changed(callback);  
device_class: controller  
description: Runs the specified function when the controller axis value changes.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Controller Axis Changed

Runs the provided callback funtion when the selected EXP Controller's joystick axis is moved.

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

- `Controller.Axis1.changed(axisMoved);`
- `Controller.Axis2.changed(axisMoved);`
- `Controller.Axis3.changed(axisMoved);`
- `Controller.Axis4.changed(axisMoved);`

![controller_button_front](controller_button_front.png)

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Controller.Axis1.changed(callbackFunction);
}
```

<advanced>
</advanced>