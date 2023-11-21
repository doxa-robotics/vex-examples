category: events  
signature: TouchLED.released(callback);  
device_class: touchled  
description: Runs the specified callback function when the Touch LED is released.  

# TouchLED Released

Runs the specified **callback function** when the TouchLED is released.

```cpp
TouchLED.released(callback);
```

## How To Use

You will need to create a function to call when the TouchLED is released. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
void touchLEDReleased() {
  Brain.Screen.print("Touch LED released.");
}
```
Then, the function is passed as the parameter of the `TouchLED.released` function call.

```cpp
TouchLED.released(touchLEDReleased);
```

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  TouchLED.released(callbackFunction);
}
```

<advanced>
</advanced>