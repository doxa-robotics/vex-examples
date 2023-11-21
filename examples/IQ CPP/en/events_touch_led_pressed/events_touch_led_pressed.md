category: events  
signature: TouchLED.pressed(callback);  
device_class: TouchLED  
description: Runs the specified callback function when the Touch LED is pressed.  

# TouchLED Pressed

Runs the specified **callback function** when the TouchLED is pressed.

```cpp
TouchLED.pressed(callback);
```

## How To Use

You will need to create a function to call when the TouchLED is pressed. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
void touchLEDPressed() {
  Brain.Screen.print("Touch LED pressed.");
}
```
Then, the function is passed as the parameter of the `TouchLED.pressed` function call.

```cpp
TouchLED.pressed(touchLEDPressed);
```

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  TouchLED.pressed(callbackFunction);
}
```

<advanced>
</advanced>