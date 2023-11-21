category: events  
signature: Brain.button.released();  
description: Runs the callback function when the Brain’s touchscreen is released.  

# Brain Button Released

Runs the callback function when the specified EXP Brain button is released.

```cpp
Brain.Button.released(callback);
```

## How To Use

You will need to create a function to call when a Brain Button is released.

```cpp
void buttonReleased() {
  Brain.Screen.print("Button released.");
}
```

The `Brain.Button.released` function can be used with the different buttons on the EXP Brain.


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
  Brain.Button.released(callbackFunction);
}
```

<advanced>
</advanced>