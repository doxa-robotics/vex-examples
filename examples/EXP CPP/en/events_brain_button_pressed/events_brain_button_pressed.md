category: events  
signature: Brain.buttonUp.pressed(callback);  
description: Runs the callback function when the Brain’s touchscreen is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

#  Brain Button Pressed

Runs the callback function when the VEX EXP Brain button is pressed.

```cpp
Brain.Button.pressed(callback);
```

## How To Use

You will need to create a function to call when a Brain Button is pressed.

```cpp
void buttonPressed() {
  Brain.Screen.print("Button pressed.");
}
```

The `Brain.Button.pressed` function can be used with the different buttons on the VEX EXP Brain.


Supported Brain buttons are as follows:

- `buttonLeft`
- `buttonRight`
- `buttonCheck`

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Brain.Button.pressed(callbackFunction);
}
```

<advanced>
</advanced>