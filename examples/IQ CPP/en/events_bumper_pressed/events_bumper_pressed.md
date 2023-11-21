category: events  
signature: BUMPER.pressed(callback);  
device_class: bumper  
description: Runs the specified function when the bumper is pressed.  

# Bumper Pressed

Runs the specified **callback function** when the bumper is pressed.

```cpp
Bumper.pressed(callback);
```

## How To Use

You will need to create a function to call when the Bumper Sensor is pressed. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
void bumperPressed() {
  Brain.Screen.print("Bumper pressed.");
}
```
Then, the function is passed as the parameter of the `Bumper.pressed` function call.

```cpp
Bumper.pressed(bumperPressed);
```

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Bumper.pressed(callbackFunction);
}
```

<advanced>
</advanced>