category: events  
signature: Bumper.released(callback);  
device_class: bumper  
description: Runs the specified function when the bumper is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Bumper Released

Runs the specified function when the bumper is released.

```cpp
Bumper.released(callback);
```

## How To Use

Create a function to call when the Bumper is released. Provide the name of the function that should run when the event occurs as the `callback` parameter.

```cpp
void bumperReleased() {
  Brain.Screen.print("Bumper released.");
}
```
Then, the function is passed as the parameter of the `Bumper.released` function call.

```cpp
Bumper.released(bumperReleased);
```

## Callback Functions

A callback function is a function passed into another function as an argument. The code inside the **callback function** will run whenever the **event** occurs. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Bumper.released(callbackFunction);
}
```

<advanced>
</advanced>